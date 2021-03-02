Module Me2Pro
===============

同步订单调试代码 ::

        $synchronizationLog = Mage::getModel('M2ePro/Synchronization_Log');
        $synchronizationLog->setComponentMode(Ess_M2ePro_Helper_Component_Ebay::NICK);
        $odersProcessor = Mage::getModel('M2ePro/cron_task_ebay_channel_synchronizeChanges_ordersProcessor');
        $odersProcessor->setSynchronizationLog($synchronizationLog);
        $odersProcessor->process();
