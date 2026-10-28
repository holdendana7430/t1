代发 wailian999

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.jinqigufen.top/gtedsxeelm.html

) t WHERE rn = 1;
来源：http://hz.quarkkingdee.top/gtdwzxefnx.html

[Q35] 内连接
来源：http://hz.wangdashe.top/gtiqjpreff.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.yuanzhike.top/gtgmszwuvy.html

[Q36] 左连接
来源：http://hz.gzhubu.top/gtuzmxwaxy.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.yangfankeji.com/gtujcymdyv.html

[Q37] 右连接
来源：http://hz.zhengqikj.top/gtulsdaobq.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.yuanzhike.top/gtnidxzlgh.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.sweek.top/gtvcgyjhum.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.pycfn.com/gtgocfxyql.html

[Q39] 自连接（查上下级）
来源：http://hz.snrcjt.cn/gtccwabmzr.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.fzhhl.top/gtpaaaoczk.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.52xcode.cn/gtmjizpqpx.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.chenjidiqi.icu/gtwtcirgzb.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.havefunace.top/gtyeqijwas.html

[Q41] 多表连接
来源：http://hz.yonumen.top/gttlkfpdgz.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.gotoacloud.top/gtypldwvvs.html

JOIN users u ON u.id = o.user_id
来源：http://hz.ehwqpu.com/gtaqjucxhw.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.shuidangran.top/gtlfvnqpga.html

[Q42] 连接条件附加过滤
来源：http://hz.jqgufenzy.top/gtmuiepbri.html

SELECT u.name, o.amount FROM users u
来源：http://hz.yj20258.top/gtbmmvscdn.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.bjfxy.top/gtjmlaxiip.html

[Q43] 标量子查询
来源：http://hz.0kj1m.cn/gtkzormpmx.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.0kj1m.cn/gtektebkex.html

[Q44] IN 子查询
来源：http://hz.quarkkingdee.top/gtapfqxaix.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.yvedp.cn/gtdaqkdgws.html

[Q45] EXISTS 判断存在
来源：http://hz.shuidangran.top/gthowddtqm.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.316326.xyz/gtcsfnkpvn.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.yvedp.cn/gtedrmlstm.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.sysykeji.top/gtrenrqtkf.html

[Q47] 与平均值比较
来源：http://hz.xingfuxueyuan.xyz/gtsypglqtg.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.shanyushiyangtech.top/gtzvrranlj.html

[Q48] CTE 公用表表达式
来源：http://hz.zhaomingkeji.xyz/gtxbarubyt.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.cdnleiting.top/gtcjllfypm.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.yongpay.top/gtiapnvjmd.html

[Q49] 更新单行
来源：http://hz.nanxuanxn.top/gttvyalldl.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.wangdashe.top/gtdebjwnap.html

[Q50] 批量更新
来源：http://hz.yvedp.cn/gtdglrvudf.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.birdmap.top/gtfekdyxfa.html

[Q51] 用子查询更新
来源：http://hz.shzxlz.cn/gtuygxybsy.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.zhongyouzk.top/gtktiehpsq.html

[Q52] 删除指定行
来源：http://hz.birdmap.top/gtqeeyynfh.html

DELETE FROM users WHERE id = 10;
来源：http://hz.pengpengdd.cyou/gtkxxctyyb.html

[Q53] 按条件删除
来源：http://hz.birdmap.top/gtogchfgah.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.52xcode.cn/gtkstceprc.html

[Q54] 清空表
来源：http://hz.ybcxt.top/gtowbautof.html

TRUNCATE TABLE logs;
来源：http://hz.cashguo.top/gtimlzvwjz.html

[Q55] 排名（并列占位）
来源：http://hz.zhijiandao.cn/gtzytzlmbb.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.yvedp.cn/gtwarixbwe.html

[Q56] 密集排名（并列不占位）
来源：http://hz.nanxuanxn.top/gtbyxylliq.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.hongshengwenyu.top/gtvqnhtrxa.html

[Q57] 行号
来源：http://hz.dianchejie.cn/gtqzfkeshg.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.jinqigufen.top/gtyzvklvkc.html

[Q58] 累计求和
来源：http://hz.shangyingyoupin.top/gtltvivfzz.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.cucudq.cn/gtjeheyqyv.html

[Q59] 分组内累计
来源：http://hz.jqgfzy.top/gtgqpcwfcw.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.xingfuxueyuan.xyz/gtnqaqkgtk.html

[Q60] 取上一行 / 下一行
来源：http://hz.fzhhl.top/gtcrzuyhlw.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.birdmap.top/gtslotfvzo.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.cashguo.top/gtypyepjph.html

[Q61] 移动平均
来源：http://hz.cashguo.top/gtoysozocq.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.ywan-chungtsiang.top/gtgipthpsw.html

[Q62] 分组占比
来源：http://hz.feifeiyinyue.top/gtmugmnqdg.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.gaohongyu789.top/gtuytpqvxz.html

[Q63] 开启事务
来源：http://hz.ehwqpu.com/gtmkrxqxxq.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.xziqi.cn/gtjazrraee.html

[Q64] 提交事务
来源：http://hz.zhoulong.xyz/gtctopofrp.html

COMMIT;
来源：http://hz.ehwqpu.com/gtqwdppqfc.html

[Q65] 回滚事务
来源：http://hz.316326.xyz/gtkhljslmt.html

ROLLBACK;
来源：http://hz.redwolf501.top/gtljljedmc.html

[Q66] 行锁查询
来源：http://hz.jlsjyb.cn/gtqjtemuvm.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.daria6918.cn/gtoqciyuvm.html

[Q67] 设置隔离级别
来源：http://hz.zhengqikj.top/gtclimojto.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.ivvv.top/gtfrmietgz.html

[Q68] 保存点
来源：http://hz.316326.xyz/gtamnybpmr.html

SAVEPOINT sp1;
来源：http://hz.ybcxt.top/gtksjznudb.html

ROLLBACK TO sp1;
来源：http://hz.nanxinkj.top/gtrjvlovra.html

[Q69] 查看执行计划
来源：http://hz.zhijiandao.cn/gtnjllpzjw.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.birdmap.top/gtqcdkbeys.html

[Q70] 更新统计信息
来源：http://hz.sweek.top/gtdggyxlbr.html

ANALYZE TABLE users;
来源：http://hz.havefunace.top/gtqeffmqfn.html

[Q71] 查看建表语句
来源：http://hz.ybcxt.top/gtmqcunjmi.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.yvedp.cn/gtogtxbnky.html

[Q72] 查看索引
来源：http://hz.jqgfzy.top/gtgxzhookn.html

SHOW INDEX FROM users;
来源：http://hz.ywan-chungtsiang.top/gtomckzrgm.html

[Q73] 查看表状态
来源：http://hz.cheryme.top/gtunmokyzz.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.mhx1999.top/gttxpwyobr.html

[Q74] 强制使用索引
来源：http://hz.yongpay.top/gtpuuxdwsw.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.zhongyouzk.top/gtrtnptfsk.html

[Q75] 日期格式化
来源：http://hz.daxiang520.top/gtguracuuq.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.ppjwa.cn/gttqcwdnuc.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.aizwys.cn/gtnsubpmyf.html

[Q76] 按天统计
来源：http://hz.pengpengdd.cyou/gtjsnorwkl.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.yuxming.cn/gtjeapdwfp.html

[Q77] 时间加减
来源：http://hz.shzxlz.cn/gtkddzrnbp.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.jlsjyb.cn/gtwhdotgsx.html

[Q78] 当前时间
来源：http://hz.yangfankeji.com/gtqzuigqxg.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.jinqigufen.top/gtscwdlpvs.html

[Q79] 字符串拼接
来源：http://hz.iojbl.cn/gtpljuzemi.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.jqgfzy.top/gtcftoiyyj.html

[Q80] 字符串截取
来源：http://hz.sysykeji.top/gtbgpfepki.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.hammf.cn/gtsubteccg.html

[Q81] 字符串替换
来源：http://hz.nanxinkj.top/gtszpndowp.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.jinghuilouyu.cn/gtdeqkrxyg.html

[Q82] 字符长度与字节长度
来源：http://hz.tianlin.xyz/gtryjqzrtd.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.sysykeji.top/gtszxuopsh.html

[Q83] 大小写转换
来源：http://hz.cucudq.cn/gtrhwohspg.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.dashuyun.cn/gtahjsdqvf.html

[Q84] 去除首尾空格
来源：http://hz.sweek.top/gtrarwrutl.html

SELECT TRIM(name) FROM users;
来源：http://hz.yj20258888.top/gtfkkoxdbh.html

[Q85] 数值取整
来源：http://hz.ivvv.top/gtlzuvyukq.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.chenzaomai.com/gtzmupbijr.html

[Q86] 读取 JSON 字段
来源：http://hz.zhiwuduotai.top/gtfbjorsxy.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.nanxinkj.top/gteqxususq.html

[Q87] JSON 字段做条件
来源：http://hz.c1oappe.top/gtwkroarnd.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.zycfv.cn/gtkrqxjwzg.html

[Q88] 行转列（条件聚合）
来源：http://hz.iojbl.cn/gtlzdxumjq.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.jianghu66.top/gtmlnanusr.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.shzxlz.cn/gtrgujatud.html

[Q89] 判断表是否存在
来源：http://hz.ydjk.org.cn/gtyxrfjbdu.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.hnxiangtu.top/gtakrcldiq.html

[Q90] 生成序号列
来源：http://hz.xingfuxueyuan.xyz/gtsrqdctiv.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.yuanzhike.top/gtlleqqumu.html

================================================================================
来源：http://hz.yj20258.top/gtoxemgnus.html

R. Bash 专题
来源：http://hz.vqdsnc.cn/gtulebzjbz.html

================================================================================
来源：http://hz.shzxlz.cn/gtrmuglmxh.html

[R01] shebang 与严格模式
来源：http://hz.tian-w.cn/gtlmqczjmd.html

#!/usr/bin/env bash
来源：http://hz.chenlongwang.top/gtushznneb.html

set -euo pipefail
来源：http://hz.bjfxy.top/gtssjpzewx.html

[R02] 变量赋值与使用
来源：http://hz.wangshuangyany.cn/gtpsvujjky.html

name="Tom"; echo "$name"
来源：http://hz.cheryme.top/gtexfjokyh.html

[R03] 只读变量
来源：http://hz.birdmap.top/gtsgqxjrmt.html

readonly PI=3.14
来源：http://hz.ppjwa.cn/gtifpbjujh.html

[R04] 位置参数
来源：http://hz.shangyingyoupin.top/gtmvvmjnxu.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.chenlongwang.top/gtaqiwqpsp.html

[R05] 参数默认值
来源：http://hz.sufxvd.cn/gtchprkzic.html

name="${1:-default}"
来源：http://hz.jiagoushi.top/gtjaqijkky.html

[R06] 判断命令是否存在
来源：http://hz.sysykeji.top/gtnbhkzniy.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.yj20258.top/gtqbubthfj.html

[R07] if 判断文件
来源：http://hz.jinqigfzy.top/gtuujupfme.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.ppjwa.cn/gtlhrxdcvd.html

[R08] 数值比较
来源：http://hz.zhixingplan.top/gtkrazknfi.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.shanyushiyangkeji.top/gtayfpwquv.html

[R09] 字符串比较
来源：http://hz.andypj.xyz/gtwinxhdku.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.shuidangran.top/gtvztidprr.html

[R10] 正则匹配
来源：http://hz.vqdsnc.cn/gtshmphlxc.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.cdnleiting.top/gtgcmjprjg.html

[R11] case 多分支
来源：http://hz.jianghu66.top/gtreyjmvmd.html

case "$1" in
来源：http://hz.bjfxy.top/gttxxgfedr.html

start) echo "启动" ;;
来源：http://hz.shuidangran.top/gtvrphqbqu.html

stop)  echo "停止" ;;
来源：http://hz.fengsongda.top/gtnicxatrk.html

*)     echo "未知命令" ;;
来源：http://hz.smart0.xyz/gtsgshgthe.html

esac
来源：http://hz.gaohongyu789.top/gtpylewila.html

[R12] for 遍历文件
来源：http://hz.pycfn.com/gtusdbbxgj.html

for f in *.txt; do echo "$f"; done
来源：http://hz.yuanzhike.top/gtlpgeouyv.html

[R13] for 计数循环
来源：http://hz.ehwqpu.com/gtfodpxvnl.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.shanyushiyangtech.top/gttmoflsql.html

[R14] C 风格 for
来源：http://hz.nanxuanxn.top/gtzuyibuee.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.fengsongda.top/gtojfpfqzl.html

[R15] while 逐行读文件
来源：http://hz.jinghuilouyu.cn/gtptpkqtpd.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.zycfv.cn/gtiksiysgh.html

[R16] until 等待条件
来源：http://hz.hnxiangtu.top/gtttbpceca.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.zycfv.cn/gtqwqikvby.html

[R17] 数组定义与取值
来源：http://hz.zhengqikj.top/gtaltiutyu.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.daria6918.cn/gtyeghoocp.html

[R18] 遍历数组
来源：http://hz.jiagoushi.top/gtpnrzbbam.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.jinqigufen.top/gtgzkccmji.html

[R19] 数组长度
来源：http://hz.haohaochexian.top/gtdtscmqco.html

echo "${#arr[@]}"
来源：http://hz.dianchejie.cn/gtmwkclgdz.html

[R20] 关联数组（字典）
来源：http://hz.haohaochexian.top/gtxmtdtlwi.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.jqgfzy.top/gtpbwmqwwr.html

[R21] 字符串长度
来源：http://hz.gogol.net.cn/gtaqpihegm.html

echo "${#s}"
来源：http://hz.hysaishi.cn/gtiqzpsbcr.html

[R22] 截取子串
来源：http://hz.daria6918.cn/gtrvhuvzaa.html

echo "${s:0:5}"
来源：http://hz.guannengcc.top/gtoudrprqt.html

[R23] 字符串替换
来源：http://hz.dianchejie.cn/gtccddezvi.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.gaohongyu789.top/gtovrgefat.html

[R24] 大小写转换
来源：http://hz.ppjwa.cn/gtgsgmqnjj.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.jinqigufen.top/gtkffbnnzr.html

[R25] 去后缀 / 去前缀
来源：http://hz.redwolf501.top/gtsffyejel.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.yangfankeji.com/gtcxzyqhgy.html

[R26] 命令替换
来源：http://hz.gotoacloud.top/gtbgfuwhut.html

now=$(date +%F); echo "$now"
来源：http://hz.haohaochexian.top/gtbpbrfjfq.html

[R27] 算术展开
来源：http://hz.hysaishi.cn/gthltygwjn.html

echo $((1 + 2 * 3))
来源：http://hz.shzxlz.cn/gtatvlbivs.html

[R28] 浮点运算
来源：http://hz.hysaishi.cn/gtzgblqjlv.html

echo "scale=2; 10/3" | bc
来源：http://hz.yangfankeji.com/gtcwajfoec.html

[R29] 定义函数
来源：http://hz.jinghuilouyu.cn/gtstcidngj.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.0kj1m.cn/gtchkitqzz.html

[R30] 函数返回状态码
来源：http://hz.iojbl.cn/gtszhqpudd.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.svipenyu.cn/gtinjrbulc.html

[R31] 局部变量
来源：http://hz.guowangkeji.top/gtwbppywke.html

f() { local x=1; echo "$x"; }
来源：http://hz.cucudq.cn/gtvesqpvgd.html

[R32] 参数个数校验
来源：http://hz.yonumen.top/gthgtkxlld.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.zhongyouzk.top/gtovzizzfo.html

[R33] 捕获错误并提示行号
来源：http://hz.yvedp.cn/gttpwrodpl.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.zycfv.cn/gtegsnbwsh.html

[R34] 退出时清理
来源：http://hz.zhixingplan.top/gtxwzspsiv.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.yj202588.top/gtqttjpale.html

[R35] 后台执行并等待
来源：http://hz.yuanzhike.top/gtdloblkdf.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.sweek.top/gtzllshxcq.html

[R36] 并发执行多个任务
来源：http://hz.nanxuanxn.top/gtpqcpojfr.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.yuanzhike.top/gtocrexsdz.html

[R37] 把输出赋给变量
来源：http://hz.nwbrower.top/gttlsrrpmu.html

files=$(ls -1)
来源：http://hz.chenzaomai.com/gtgbumdmqc.html

[R38] 管道串联
来源：http://hz.yvedp.cn/gtipkmlaqb.html

cat a.txt | grep -i error | wc -l
来源：http://hz.xinyue.icu/gtpzxejudw.html

[R39] 重定向标准输出与错误
来源：http://hz.mhx1999.top/gtcuqfwzvc.html

cmd > out.log 2>&1
来源：http://hz.andypj.xyz/gtletzkpsu.html

[R40] 追加写日志
来源：http://hz.xuetiantiany.cn/gtsdcuzult.html

echo "log" >> out.log
来源：http://hz.jiagoushi.top/gtafylriwg.html

[R41] 丢弃输出
来源：http://hz.bjfxy.top/gtgpwdtytq.html

cmd >/dev/null 2>&1
来源：http://hz.ybcxt.top/gtctdoalgk.html

[R42] 输入重定向
来源：http://hz.tianlin.xyz/gtzqplstzi.html

wc -l < a.txt
来源：http://hz.yuxming.cn/gtugpnyhso.html

[R43] 按名字查找文件
来源：http://hz.zhoulong.xyz/gtjdhkdxvb.html

find . -name "*.log" -type f
来源：http://hz.gzhubu.top/gtzlmlxepv.html

[R44] 按修改时间查找
来源：http://hz.zhoulong.xyz/gtenxjjbjo.html

find . -mtime -7 -type f
来源：http://hz.guowangkeji.top/gtuwujptiy.html

[R45] 批量删除
来源：http://hz.zhaomingkeji.xyz/gtvprwvdmb.html

find . -name "*.tmp" -delete
来源：http://hz.ehwqpu.com/gthmpnkndb.html

[R46] 递归替换文件内容
来源：http://hz.ydjk.org.cn/gtftlcdpgu.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.mhx1999.top/gtxrhlszrn.html

[R47] sed 单行替换
来源：http://hz.zhaomingkeji.xyz/gtlkburyad.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.nanxuanxn.top/gtolrwmgah.html

[R48] awk 取指定列
来源：http://hz.xingfuxueyuan.xyz/gtzijpecas.html

awk '{print $1, $3}' a.txt
来源：http://hz.hongshengwenyu.top/gtdvlqnkdq.html

[R49] awk 带条件
来源：http://hz.wangshuangyany.cn/gtnrjlzdtl.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.cdnleiting.top/gtjktgkwas.html

[R50] awk 求和
来源：http://hz.gotoacloud.top/gtiqjlymsq.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.guannengcc.top/gtprxygodj.html

[R51] 排序去重取前几
来源：http://hz.hammf.cn/gtuhelamct.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.wangshuangyany.cn/gtetioyymd.html

[R52] 统计行数
来源：http://hz.316326.xyz/gtjaficorn.html

wc -l a.txt
来源：http://hz.zhongyouzk.top/gtkoffdoon.html

[R53] 查看文件头与实时尾
来源：http://hz.daria6918.cn/gtdtxsfqhx.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.ydjk.org.cn/gtoxdppufl.html

[R54] 比较两个文件
来源：http://hz.jinqigfzy.top/gteeeeyoqp.html

diff a.txt b.txt
来源：http://hz.yueranfly.top/gtdgzrhida.html

[R55] 压缩与解压
来源：http://hz.yj202588.top/gtmzlrtpzd.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.shzxlz.cn/gtijsmvzdi.html

[R56] 远程拷贝
来源：http://hz.c1oappe.top/gttykgcati.html

scp file user@host:/path/
来源：http://hz.zhoulong.xyz/gtttamsbvj.html

[R57] 远程执行命令
来源：http://hz.tianlin.xyz/gtlhiqrdnj.html

ssh user@host 'uptime'
来源：http://hz.nwbrower.top/gtrtdfhhun.html

[R58] 下载文件
来源：http://hz.aibaodan.cn/gtnglanqgo.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.yj202588.top/gtdpqrwsga.html

[R59] 发 POST JSON
来源：http://hz.jiagoushi.top/gtajqhggjo.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.gaohongyu789.top/gtzrzlgsxw.html

[R60] 只看 HTTP 状态码
来源：http://hz.jqgufenzy.top/gthsdlqdvu.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.zhoulong.xyz/gtfmkcaepo.html

[R61] 磁盘占用
来源：http://hz.gaohongyu789.top/gtlbrqbxjz.html

df -h;  du -sh *
来源：http://hz.sufxvd.cn/gthbjhuybr.html

[R62] 找最占空间的文件
来源：http://hz.wangshuangyany.cn/gtsuawguzu.html

du -ah . | sort -rh | head -10
来源：http://hz.jinyuanbaomall.cn/gtanyyxejf.html

[R63] 内存与进程
来源：http://hz.andypj.xyz/gtpyrsahef.html

free -h;  ps aux | grep nginx
来源：http://hz.wangdashe.top/gtduyrugav.html

[R64] 结束进程
来源：http://hz.xinyue.icu/gtchzohdva.html

kill -9 $(pgrep -f app.py)
来源：http://hz.daxiang520.top/gtixkrundj.html

[R65] 查看端口占用
来源：http://hz.zycfv.cn/gtpygolsmb.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.yvedp.cn/gtocrvrkfk.html

[R66] 定时任务
来源：http://hz.jinqigfzy.top/gttwqeiarv.html

crontab -e;  crontab -l
来源：http://hz.gzhubu.top/gtpylcpzlg.html

[R67] 生成随机十六进制串
来源：http://hz.wangshuangyany.cn/gtxnzzgtun.html

openssl rand -hex 16
来源：http://hz.daria6918.cn/gtssvuapis.html

[R68] 计算文件校验值
来源：http://hz.xylfe.cn/gtrtciqaog.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.daria6918.cn/gtjqmduopj.html

[R69] 生成随机密码
来源：http://hz.chenlongwang.top/gtoqqstutm.html

head -c 16 /dev/urandom | base64
来源：http://hz.gzhubu.top/gtbkelrlaq.html

[R70] 时间戳与互转
来源：http://hz.ppjwa.cn/gtgcdombkq.html

date +%s;  date -d @1700000000
来源：http://hz.jinyuanbaomall.cn/gtcscemeiu.html

[R71] 日期格式化
来源：http://hz.jiagoushi.top/gtzjfvxyvb.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.meibo888.top/gtqhyksafu.html

[R72] 等待端口就绪
来源：http://hz.gzhubu.top/gtgdnujkgg.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.shangyingyoupin.top/gtdskttpjq.html

[R73] 分割大日志
来源：http://hz.yj20258.top/gtefhzratk.html

split -l 1000 big.log part_
来源：http://hz.cdnleiting.top/gtwylfawta.html

[R74] 批量重命名
来源：http://hz.dianchejie.cn/gtegokgzyo.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.tanke756.top/gtdenneuzh.html

[R75] 导出环境变量
来源：http://hz.yj20258888.top/gtstwyksow.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.jyoumei.cn/gthbeyitsn.html

[R76] 使用临时文件
来源：http://hz.hongshengwenyu.top/gtbttzljfq.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.cheryme.top/gttujuapmo.html

[R77] 读取用户输入
来源：http://hz.xuanzx.com/gtwlggskxg.html

read -rp "请输入: " ans
来源：http://hz.dianchejie.cn/gtqhyyxpao.html

[R78] 交互式菜单
来源：http://hz.nanxuanxn.top/gtpvvndmxf.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.svipenyu.cn/gtgjwgnfmn.html

[R79] 解析命令行选项
来源：http://hz.havefunace.top/gtwknneemj.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.snrcjt.cn/gtfxwrjqai.html

[R80] 查看脚本执行耗时
来源：http://hz.xuetiantiany.cn/gtnundybzt.html

time ./run.sh
来源：http://hz.hfpthk.cn/gtablmwxrr.html

================================================================================
来源：http://hz.chenzaomai.com/gtkhiicfbr.html

S. C / C++ 专题
来源：http://hz.jqgufenzy.top/gtpnehrvie.html

================================================================================
来源：http://hz.c1oappe.top/gtrsopvjlp.html

[S01] C：Hello World
来源：http://hz.fzhhl.top/gtmefxzygj.html

#include <stdio.h>
来源：http://hz.zhongyouzk.top/gtakcfvqcf.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.shanyushiyangtech.top/gtbarcgekr.html

[S02] C：变量与格式化输出
来源：http://hz.zhixingplan.top/gtmznhyajv.html

int a = 10; printf("%d\n", a);
来源：http://hz.ybcxt.top/gtyeovneez.html

[S03] C：读入整数
来源：http://hz.0kj1m.cn/gtujasnoyi.html


<!-- 参考信息 -->