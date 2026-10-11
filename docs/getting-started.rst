Getting started
===============

This instance follows the standard FEMIC deployment-instance layout. Run all
commands from the instance root (or pass `--instance-root`).

.. code-block:: console

   femic prep validate-case --run-config config/run_profile.tsa16.yaml
   femic prep geospatial-preflight
   femic run --run-config config/run_profile.tsa16.yaml
   femic tsa post-tipsy --run-config config/run_profile.tsa16.yaml --tsa 16
   femic export woodstock --tsa 16
   femic export ws3-sections --woodstock-dir output/woodstock --output-dir output/ws3

The FreshForge graph for this MU lives in
`workflows/freshforge/tsa16_model_build_workflow.yaml` (plan/run from the
parent femic checkout with `--workdir runtime/freshforge --namespace tsa16/model-build`).
