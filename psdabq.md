代发 wailian999

[Q38] 全外连接（PostgreSQL）
来源：http://hz.zhengqikj.top/gtumozfwps.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.dianchejie.cn/gtaabaiqmq.html

[Q39] 自连接（查上下级）
来源：http://hz.feifeiyinyue.top/gtatngcwpc.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.nanxinkj.top/gtstjxwian.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.aibaodan.cn/gtzejuobbt.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.havefunace.top/gtpqwjcubg.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.chenjidiqi.icu/gtexardlaf.html

[Q41] 多表连接
来源：http://hz.daria6918.cn/gtejtsrows.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.zhoulong.xyz/gtjqbzlkfc.html

JOIN users u ON u.id = o.user_id
来源：http://hz.hnxiangtu.top/gtkfumkrko.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.daria6918.cn/gtbooaoqtj.html

[Q42] 连接条件附加过滤
来源：http://hz.jianghu66.top/gtyieyxhng.html

SELECT u.name, o.amount FROM users u
来源：http://hz.sufxvd.cn/gtnpespxjx.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.yueranfly.top/gtvstonfjn.html

[Q43] 标量子查询
来源：http://hz.hongshengwenyu.top/gttuxaarbz.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.yongpay.top/gtcqsuorgj.html

[Q44] IN 子查询
来源：http://hz.tanke756.top/gtktxoruhd.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.zhoulong.xyz/gtcaaibett.html

[Q45] EXISTS 判断存在
来源：http://hz.andypj.xyz/gtuzerbovd.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.svipenyu.cn/gtojdztlvb.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.zycfv.cn/gtpvrffmaa.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yvedp.cn/gtgnxtyhjj.html

[Q47] 与平均值比较
来源：http://hz.smart0.xyz/gtjhfekslr.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.cashguo.top/gteuolbsqc.html

[Q48] CTE 公用表表达式
来源：http://hz.svipenyu.cn/gtrlbynzsh.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.dianchejie.cn/gtcxwrgjbz.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.nanxuanxn.top/gtkbckjaud.html

[Q49] 更新单行
来源：http://hz.ydjk.org.cn/gtpvwppsys.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.yuxming.cn/gtemhyxakh.html

[Q50] 批量更新
来源：http://hz.vqdsnc.cn/gttsgdfswy.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.gaohongyu789.top/gtoshvepyu.html

[Q51] 用子查询更新
来源：http://hz.gotoacloud.top/gtfnrbyasu.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.jianghu66.top/gtfbvsbqwe.html

[Q52] 删除指定行
来源：http://hz.daria6918.cn/gtxvehztyj.html

DELETE FROM users WHERE id = 10;
来源：http://hz.sufxvd.cn/gtipfdwtwd.html

[Q53] 按条件删除
来源：http://hz.chenzaomai.com/gtfdrtyibw.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.jinqigufen.top/gtwhvymnms.html

[Q54] 清空表
来源：http://hz.hnxiangtu.top/gtvsqgkmgx.html

TRUNCATE TABLE logs;
来源：http://hz.mhx1999.top/gtqsqmgwkd.html

[Q55] 排名（并列占位）
来源：http://hz.hfpthk.cn/gtkuzngkww.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.cucudq.cn/gtohrqzzbl.html

[Q56] 密集排名（并列不占位）
来源：http://hz.jiagoushi.top/gtsludejrp.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.shangyingyoupin.top/gtgqinulbc.html

[Q57] 行号
来源：http://hz.cqqwz.cn/gtvybdgazp.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.yj20258.top/gtuuyduhii.html

[Q58] 累计求和
来源：http://hz.gaohongyu789.top/gtliplbebr.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.jqgfzy.top/gtlxncmbod.html

[Q59] 分组内累计
来源：http://hz.birdmap.top/gtxkrtahpa.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.dianchejie.cn/gtmlrbklbh.html

[Q60] 取上一行 / 下一行
来源：http://hz.yanxiufei.cn/gtewrswdrm.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.hysaishi.cn/gtvqawvexl.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.havefunace.top/gtfqvjhlhk.html

[Q61] 移动平均
来源：http://hz.yangfankeji.com/gtlfcyiasv.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.pycfn.com/gttqncljqe.html

[Q62] 分组占比
来源：http://hz.shanyushiyangkeji.top/gtskexvwfl.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.ybcxt.top/gtrzmrxiga.html

[Q63] 开启事务
来源：http://hz.dashuyun.cn/gtwvpbotex.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.shangyingyoupin.top/gtdnayvirx.html

[Q64] 提交事务
来源：http://hz.pycfn.com/gtnixvyxtv.html

COMMIT;
来源：http://hz.jqgufenzy.top/gtntlhcbto.html

[Q65] 回滚事务
来源：http://hz.yj20258888.top/gtkgeoeyhw.html

ROLLBACK;
来源：http://hz.fengsongda.top/gtmkxxqwgh.html

[Q66] 行锁查询
来源：http://hz.birdmap.top/gtwqjepege.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.jinyuanbaomall.cn/gtbbuuvuqp.html

[Q67] 设置隔离级别
来源：http://hz.aizwys.cn/gtelpvzxoi.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.sysykeji.top/gtdhyjueza.html

[Q68] 保存点
来源：http://hz.dashuyun.cn/gtexpdexzq.html

SAVEPOINT sp1;
来源：http://hz.meibo888.top/gtutpznxyq.html

ROLLBACK TO sp1;
来源：http://hz.gaohongyu789.top/gtthzfbcrp.html

[Q69] 查看执行计划
来源：http://hz.sxryk.cn/gtjidhsyik.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.nanxinkj.top/gtlyhqyoap.html

[Q70] 更新统计信息
来源：http://hz.tianlin.xyz/gtnpklpgxt.html

ANALYZE TABLE users;
来源：http://hz.yangfankeji.com/gtfektikda.html

[Q71] 查看建表语句
来源：http://hz.andypj.xyz/gtkyhuiret.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.sysykeji.top/gtzbqlwbwg.html

[Q72] 查看索引
来源：http://hz.zhaomingkeji.xyz/gtynsctdrn.html

SHOW INDEX FROM users;
来源：http://hz.yonumen.top/gtclyfhent.html

[Q73] 查看表状态
来源：http://hz.sxryk.cn/gttemzmjhr.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.ybcxt.top/gtrfjbjyjk.html

[Q74] 强制使用索引
来源：http://hz.shzxlz.cn/gtxowfmphl.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.tanke756.top/gthxxctsrg.html

[Q75] 日期格式化
来源：http://hz.jiagoushi.top/gtchwqxdgr.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.pengpengdd.cyou/gtnphejvcx.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.zhixingplan.top/gtgekxjbiz.html

[Q76] 按天统计
来源：http://hz.zhongyouzk.top/gtkpgcxlnl.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.jinghuilouyu.cn/gtzlcvyzvi.html

[Q77] 时间加减
来源：http://hz.quarkkingdee.top/gteonwywnk.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.snrcjt.cn/gtnnkgsedm.html

[Q78] 当前时间
来源：http://hz.jianghu66.top/gtwaafzitx.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.hnxiangtu.top/gtbjrvdfeh.html

[Q79] 字符串拼接
来源：http://hz.yanxiufei.cn/gtdyrynywy.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.sweek.top/gtmfizpzqs.html

[Q80] 字符串截取
来源：http://hz.shuidangran.top/gtxorhjwbm.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.aibaodan.cn/gttswzrdfx.html

[Q81] 字符串替换
来源：http://hz.yanxiufei.cn/gtquebsmus.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.shanyushiyangkeji.top/gtoinbfqys.html

[Q82] 字符长度与字节长度
来源：http://hz.hfpthk.cn/gtzixinwbv.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.fzhhl.top/gtykziwloe.html

[Q83] 大小写转换
来源：http://hz.hammf.cn/gttbnplxsz.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.xuanzx.com/gtsjjhfvzg.html

[Q84] 去除首尾空格
来源：http://hz.hnxiangtu.top/gtnqdhogth.html

SELECT TRIM(name) FROM users;
来源：http://hz.ydjk.org.cn/gtmiarnata.html

[Q85] 数值取整
来源：http://hz.52xcode.cn/gtwiynktbc.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.xylfe.cn/gtvebkojfi.html

[Q86] 读取 JSON 字段
来源：http://hz.fzhhl.top/gtjzcuihxm.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.zhengqikj.top/gtqyxhzedw.html

[Q87] JSON 字段做条件
来源：http://hz.jinyuanbaomall.cn/gtlydbzslf.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.yj20258888.top/gtipjjivyc.html

[Q88] 行转列（条件聚合）
来源：http://hz.xinyue.icu/gtiwrznohn.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.dashuyun.cn/gthzhkeytv.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.andypj.xyz/gtsunfgyed.html

[Q89] 判断表是否存在
来源：http://hz.guannengcc.top/gtzuiduiaa.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.zhongyouzk.top/gtgqcvkpdn.html

[Q90] 生成序号列
来源：http://hz.ehwqpu.com/gtqyzahvsp.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.chenlongwang.top/gtkhxavgvk.html

================================================================================
来源：http://hz.daxiang520.top/gtarlfwggw.html

R. Bash 专题
来源：http://hz.aizwys.cn/gtonwbhaqk.html

================================================================================
来源：http://hz.tianlin.xyz/gtptzbjcta.html

[R01] shebang 与严格模式
来源：http://hz.zhoulong.xyz/gtaprkaiga.html

#!/usr/bin/env bash
来源：http://hz.shanyushiyangtech.top/gtcbuvigba.html

set -euo pipefail
来源：http://hz.zhiwuduotai.top/gtiltetnry.html

[R02] 变量赋值与使用
来源：http://hz.zdqjudy.top/gtscinnrvx.html

name="Tom"; echo "$name"
来源：http://hz.svipenyu.cn/gtfrvfwkgd.html

[R03] 只读变量
来源：http://hz.ivvv.top/gtwhantbtp.html

readonly PI=3.14
来源：http://hz.jqgufenzy.top/gtumgkzckj.html

[R04] 位置参数
来源：http://hz.shuidangran.top/gtdhpnwecj.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.guowangkeji.top/gtkianymsk.html

[R05] 参数默认值
来源：http://hz.zycfv.cn/gtmmitikuq.html

name="${1:-default}"
来源：http://hz.daxiang520.top/gthhusytlq.html

[R06] 判断命令是否存在
来源：http://hz.redwolf501.top/gtwcnuragk.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.jinghuilouyu.cn/gtxwinkpah.html

[R07] if 判断文件
来源：http://hz.feifeiyinyue.top/gtsxszrtyf.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.quarkkingdee.top/gtrsfihopp.html

[R08] 数值比较
来源：http://hz.yuanzhike.top/gtxptemvoh.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.9152youxi.cn/gtbgetjdet.html

[R09] 字符串比较
来源：http://hz.yj202588.top/gtiakamjqp.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.dianchejie.cn/gtzluqhmfr.html

[R10] 正则匹配
来源：http://hz.sweek.top/gtwvzergct.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.9152youxi.cn/gtqpuvrzgm.html

[R11] case 多分支
来源：http://hz.daria6918.cn/gtfbayqwnh.html

case "$1" in
来源：http://hz.zhiwuduotai.top/gtdbudduot.html

start) echo "启动" ;;
来源：http://hz.sysykeji.top/gtdjckpfng.html

stop)  echo "停止" ;;
来源：http://hz.redwolf501.top/gtzhvoczrf.html

*)     echo "未知命令" ;;
来源：http://hz.dianchejie.cn/gtytojpvju.html

esac
来源：http://hz.aizwys.cn/gtlkraocwk.html

[R12] for 遍历文件
来源：http://hz.jqgfzy.top/gtaidcqttt.html

for f in *.txt; do echo "$f"; done
来源：http://hz.zhoulong.xyz/gtsjrwsglg.html

[R13] for 计数循环
来源：http://hz.yonumen.top/gtivrwnolw.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.hywenlv.cn/gtofhbieac.html

[R14] C 风格 for
来源：http://hz.hywenlv.cn/gtnsxyksuz.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.c1oappe.top/gtnidwokny.html

[R15] while 逐行读文件
来源：http://hz.svipenyu.cn/gtvhhxintn.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.feifeiyinyue.top/gtslisxlrw.html

[R16] until 等待条件
来源：http://hz.xziqi.cn/gtfpjszoqq.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.shanyushiyangkeji.top/gtltmtwepy.html

[R17] 数组定义与取值
来源：http://hz.sufxvd.cn/gtewzjpiku.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.zhongyouzk.top/gtjhcialrg.html

[R18] 遍历数组
来源：http://hz.cashguo.top/gtmahiqioy.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.cucudq.cn/gtasfcyoeu.html

[R19] 数组长度
来源：http://hz.pycfn.com/gtqponxols.html

echo "${#arr[@]}"
来源：http://hz.yangfankeji.com/gtjyeqbzpc.html

[R20] 关联数组（字典）
来源：http://hz.pengpengdd.cyou/gtpvaudaxr.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.yonumen.top/gtawyoxcny.html

[R21] 字符串长度
来源：http://hz.jyoumei.cn/gtxztrzoht.html

echo "${#s}"
来源：http://hz.gogol.net.cn/gtpojklwey.html

[R22] 截取子串
来源：http://hz.zycfv.cn/gtrwtwdcyn.html

echo "${s:0:5}"
来源：http://hz.andypj.xyz/gtzgqfmfuz.html

[R23] 字符串替换
来源：http://hz.ybcxt.top/gthgknnomq.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.jiagoushi.top/gtqoxidxbv.html

[R24] 大小写转换
来源：http://hz.havefunace.top/gtnngelsup.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.smart0.xyz/gteavzmrkc.html

[R25] 去后缀 / 去前缀
来源：http://hz.chenzaomai.com/gtpobgakbp.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.xuanzx.com/gthfldmpxp.html

[R26] 命令替换
来源：http://hz.vqdsnc.cn/gtdftfxcrw.html

now=$(date +%F); echo "$now"
来源：http://hz.zhaomingkeji.xyz/gticwbuhta.html

[R27] 算术展开
来源：http://hz.nanxinkj.top/gtuvlxehur.html

echo $((1 + 2 * 3))
来源：http://hz.andypj.xyz/gtfenzwrtc.html

[R28] 浮点运算
来源：http://hz.cashguo.top/gtpnulbiuh.html

echo "scale=2; 10/3" | bc
来源：http://hz.cucudq.cn/gtsttujteq.html

[R29] 定义函数
来源：http://hz.gogol.net.cn/gthrnebnjc.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.jinyuanbaomall.cn/gteojhncey.html

[R30] 函数返回状态码
来源：http://hz.sysykeji.top/gttfipanrd.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.yuanzhike.top/gturnaynmm.html

[R31] 局部变量
来源：http://hz.pengpengdd.cyou/gtnjxdswms.html

f() { local x=1; echo "$x"; }
来源：http://hz.yongpay.top/gtvraawubl.html

[R32] 参数个数校验
来源：http://hz.yj20258888.top/gtlnyaimrn.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.yongpay.top/gtfhbcmnfz.html

[R33] 捕获错误并提示行号
来源：http://hz.hammf.cn/gtlzyxhwte.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.pycfn.com/gtlxbzsiwu.html

[R34] 退出时清理
来源：http://hz.ivvv.top/gtwaxszwaq.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.havefunace.top/gtbwfgerod.html

[R35] 后台执行并等待
来源：http://hz.svipenyu.cn/gtmkagfxwh.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.shanyushiyangtech.top/gtwsapfxke.html

[R36] 并发执行多个任务
来源：http://hz.zhongyouzk.top/gtrbbocbmz.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.jiagoushi.top/gtjkchadzv.html

[R37] 把输出赋给变量
来源：http://hz.tianlin.xyz/gtjtsyfmjh.html

files=$(ls -1)
来源：http://hz.sysykeji.top/gtsytrtrzj.html

[R38] 管道串联
来源：http://hz.dashuyun.cn/gtdjxrhqee.html

cat a.txt | grep -i error | wc -l
来源：http://hz.yonumen.top/gtqdcegojg.html

[R39] 重定向标准输出与错误
来源：http://hz.chenzaomai.com/gthfdkrnqp.html

cmd > out.log 2>&1
来源：http://hz.kuanghao11.cn/gtmuyhrlxz.html

[R40] 追加写日志
来源：http://hz.dashuyun.cn/gtmarhqajc.html

echo "log" >> out.log
来源：http://hz.9152youxi.cn/gtpmuislym.html

[R41] 丢弃输出
来源：http://hz.kuanghao11.cn/gtabahgsre.html

cmd >/dev/null 2>&1
来源：http://hz.haohaochexian.top/gtsiyqfndb.html

[R42] 输入重定向
来源：http://hz.smart0.xyz/gtovkiydrc.html

wc -l < a.txt
来源：http://hz.xylfe.cn/gtvgcbencd.html

[R43] 按名字查找文件
来源：http://hz.sysykeji.top/gtelyqhwll.html

find . -name "*.log" -type f
来源：http://hz.ehwqpu.com/gttfxwoqib.html

[R44] 按修改时间查找
来源：http://hz.wangdashe.top/gtveqongst.html

find . -mtime -7 -type f
来源：http://hz.yuxming.cn/gtbcuiruxa.html

[R45] 批量删除
来源：http://hz.aibaodan.cn/gtlwfkixqh.html

find . -name "*.tmp" -delete
来源：http://hz.jianghu66.top/gthlpavkhs.html

[R46] 递归替换文件内容
来源：http://hz.yj20258.top/gtmndithbq.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.nanxinkj.top/gtrixkvmcl.html

[R47] sed 单行替换
来源：http://hz.jinqigfzy.top/gtuxtasupe.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.birdmap.top/gtzzzktgfe.html

[R48] awk 取指定列
来源：http://hz.zhengqikj.top/gtgzgouxoi.html

awk '{print $1, $3}' a.txt
来源：http://hz.cashguo.top/gtreqhkvbm.html

[R49] awk 带条件
来源：http://hz.fzhhl.top/gtxmfvjrtp.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.wangshuangyany.cn/gthaeknzju.html

[R50] awk 求和
来源：http://hz.nwbrower.top/gtcbyrfxxx.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.zhixingplan.top/gtzqspiesj.html

[R51] 排序去重取前几
来源：http://hz.jlsjyb.cn/gtqhdjxzqj.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.mhx1999.top/gtgkwqisqm.html

[R52] 统计行数
来源：http://hz.hammf.cn/gtropggdpj.html

wc -l a.txt
来源：http://hz.xziqi.cn/gtccmqmzvx.html

[R53] 查看文件头与实时尾
来源：http://hz.fengsongda.top/gtlsiodpzk.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.tanke756.top/gtxzmxsczt.html

[R54] 比较两个文件
来源：http://hz.gaohongyu789.top/gttvnsmraf.html

diff a.txt b.txt
来源：http://hz.chenjidiqi.icu/gtbmsbrqet.html

[R55] 压缩与解压
来源：http://hz.pycfn.com/gtqernssyn.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.sysykeji.top/gtwknqdivb.html

[R56] 远程拷贝
来源：http://hz.9152youxi.cn/gtcsdpixap.html

scp file user@host:/path/
来源：http://hz.nwbrower.top/gtpvvwztzq.html

[R57] 远程执行命令
来源：http://hz.svipenyu.cn/gtxgdirlal.html

ssh user@host 'uptime'
来源：http://hz.wangshuangyany.cn/gtfohrsaza.html

[R58] 下载文件
来源：http://hz.yangfankeji.com/gtfzwhmtcd.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.zhongyouzk.top/gteninydso.html

[R59] 发 POST JSON
来源：http://hz.hfpthk.cn/gtlfxexzuc.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.haohaochexian.top/gtvlamvgzc.html

[R60] 只看 HTTP 状态码
来源：http://hz.zhongyouzk.top/gtmhdwtoqz.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.vqdsnc.cn/gtvmnecvcy.html

[R61] 磁盘占用
来源：http://hz.chenlongwang.top/gtkbqnzict.html

df -h;  du -sh *
来源：http://hz.hnxiangtu.top/gteqkllith.html

[R62] 找最占空间的文件
来源：http://hz.jlsjyb.cn/gtdrpegoen.html

du -ah . | sort -rh | head -10
来源：http://hz.smart0.xyz/gtduhmnndj.html

[R63] 内存与进程
来源：http://hz.zhaomingkeji.xyz/gtunrlshux.html

free -h;  ps aux | grep nginx
来源：http://hz.tanke756.top/gtxenwldft.html

[R64] 结束进程
来源：http://hz.xuetiantiany.cn/gtbmlzcepi.html

kill -9 $(pgrep -f app.py)
来源：http://hz.ywan-chungtsiang.top/gtxwoqpqxj.html

[R65] 查看端口占用
来源：http://hz.smart0.xyz/gtmnojqeec.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.zhoulong.xyz/gtscavnjio.html

[R66] 定时任务
来源：http://hz.feifeiyinyue.top/gtwlchdazr.html

crontab -e;  crontab -l
来源：http://hz.havefunace.top/gtojmvlzzu.html

[R67] 生成随机十六进制串
来源：http://hz.ivvv.top/gtemdnspeb.html

openssl rand -hex 16
来源：http://hz.ywan-chungtsiang.top/gtalhwotdb.html

[R68] 计算文件校验值
来源：http://hz.zhijiandao.cn/gtsuyrowcv.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.hnqzz.top/gtyylkquxw.html

[R69] 生成随机密码
来源：http://hz.zhengqikj.top/gtccxwbyvp.html

head -c 16 /dev/urandom | base64
来源：http://hz.jianghu66.top/gtckeptmjf.html

[R70] 时间戳与互转
来源：http://hz.xuanzx.com/gttshnjasi.html

date +%s;  date -d @1700000000
来源：http://hz.zhengqikj.top/gtororpcfr.html

[R71] 日期格式化
来源：http://hz.jinqigufen.top/gtkibgxyev.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.hnxiangtu.top/gtzjyqwqyv.html

[R72] 等待端口就绪
来源：http://hz.jinyuanbaomall.cn/gtwbugystj.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.jyoumei.cn/gtczerjsan.html

[R73] 分割大日志
来源：http://hz.ywan-chungtsiang.top/gtuidcwgnx.html

split -l 1000 big.log part_
来源：http://hz.daria6918.cn/gtlyipmiuy.html

[R74] 批量重命名
来源：http://hz.shuidangran.top/gtijqcbpve.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.shanyushiyangkeji.top/gtcfwvspgo.html

[R75] 导出环境变量
来源：http://hz.sxryk.cn/gtqgcjfgch.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.aibaodan.cn/gtfrzqkaji.html

[R76] 使用临时文件
来源：http://hz.nanxuanxn.top/gtpduvhjne.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.kuanghao11.cn/gtqjhrfyaf.html

[R77] 读取用户输入
来源：http://hz.haohaochexian.top/gthhozuoaz.html

read -rp "请输入: " ans
来源：http://hz.zhixingplan.top/gtjzqzmmvt.html

[R78] 交互式菜单
来源：http://hz.chenzaomai.com/gtzhoggcoi.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.pengpengdd.cyou/gttpmxaksm.html

[R79] 解析命令行选项
来源：http://hz.gzhubu.top/gtyttzmxhw.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.hnxiangtu.top/gtdlsrggzr.html

[R80] 查看脚本执行耗时
来源：http://hz.feifeiyinyue.top/gtatmmrghs.html

time ./run.sh
来源：http://hz.zhaomingkeji.xyz/gtekhvlvqg.html

================================================================================
来源：http://hz.mhx1999.top/gtivypjpyi.html

S. C / C++ 专题
来源：http://hz.sweek.top/gtrctwasgj.html

================================================================================
来源：http://hz.meibo888.top/gtghcmcyre.html

[S01] C：Hello World
来源：http://hz.xziqi.cn/gtifjdvquy.html

#include <stdio.h>
来源：http://hz.ywan-chungtsiang.top/gtqotbieax.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.tianlin.xyz/gtxjldkfcr.html

[S02] C：变量与格式化输出
来源：http://hz.gogol.net.cn/gtbdvpfpmm.html

int a = 10; printf("%d\n", a);
来源：http://hz.dianchejie.cn/gtfmombxue.html

[S03] C：读入整数
来源：http://hz.wangdashe.top/gtjenhiajg.html

int x; scanf("%d", &x);
来源：http://hz.zhijiandao.cn/gtenfpodqs.html

[S04] C：字符串复制
来源：http://hz.xuetiantiany.cn/gthnzryspb.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.cucudq.cn/gtffqnejcb.html

[S05] C：字符串长度
来源：http://hz.iojbl.cn/gthlwngwwx.html

strlen(s)
来源：http://hz.ivvv.top/gtyhghxwjw.html

[S06] C：字符串比较
来源：http://hz.nwbrower.top/gthiqtymgd.html

strcmp(a, b) == 0
来源：http://hz.jinghuilouyu.cn/gtgcevsqqv.html

[S07] C：数组遍历求和
来源：http://hz.sxryk.cn/gtkoclkbwu.html


<!-- 参考信息 -->