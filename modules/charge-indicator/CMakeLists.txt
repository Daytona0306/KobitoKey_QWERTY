# 4mplelab/zmk-feature-charge-indicator を同梱したもの (MIT、LICENSE 参照)。
if(CONFIG_CHARGE_INDICATOR)
  target_sources(app PRIVATE src/charge_indicator.c)
endif()
