<template>
    <div class="px-2 dark:bg-gray-800 dark:border-gray-700 ">
        <fwb-accordion :open-first-item="false">
            <fwb-accordion-panel>
                <fwb-accordion-header>What tech stack Am i using?</fwb-accordion-header>
                <fwb-accordion-content>
                    <div>
                        <p class="mb-2 text-gray-500 dark:text-gray-400">
                            I'm adept at mastering the latest .NET technologies, including .NET 6, and have a strong foundation in cloud services like Azure and AWS. My expertise extends to DevOps practices, ensuring efficient development processes through CI/CD pipelines and infrastructure as code.
                        </p>
                       
                    </div>
                </fwb-accordion-content>
            </fwb-accordion-panel>
            <fwb-accordion-panel>
                <fwb-accordion-header>Which is my previous project?</fwb-accordion-header>
                <fwb-accordion-content>
                    <div>
                        <p class="mb-2 text-gray-500 dark:text-gray-400">
                            I have worked on a variety of projects, including a web-based application for a client in the healthcare industry. The application was built using Blazor WebAssembly and hosted on Azure. I also developed a web-based solution for a client in the education sector, using Django and Vue.js.
                        </p>
                        
                    </div>
                </fwb-accordion-content>
            </fwb-accordion-panel>
            <fwb-accordion-panel>
                <fwb-accordion-header>
                    What is my design process?
                </fwb-accordion-header>
                <fwb-accordion-content>
                    <div>
                        <p class="mb-2 text-gray-500 dark:text-gray-400">
                            My design process is centered around user experience and accessibility. I start by understanding the client's requirements and the target audience. I then create wireframes and prototypes to visualize the user journey and interactions. I use design tools like Figma to create high-fidelity designs and iterate based on feedback.
                        </p>
                       
                    </div>
                </fwb-accordion-content>
            </fwb-accordion-panel>
        </fwb-accordion>
    </div>
</template>

<script setup>
import {
    FwbAccordion,
    FwbAccordionContent,
    FwbAccordionHeader,
    FwbAccordionPanel,
} from 'flowbite-vue'
</script>
