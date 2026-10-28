代发 wailian999

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.pycfn.com/gtsnzjqxrb.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.haohaochexian.top/gtqvzrkddx.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.guowangkeji.top/gtcaudoswe.html

[Q41] 多表连接
来源：http://hz.zhaomingkeji.xyz/gtaennwnfk.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.316326.xyz/gtprcyczkn.html

JOIN users u ON u.id = o.user_id
来源：http://hz.zdqjudy.top/gtciraupcy.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.cucudq.cn/gtrlelhqmp.html

[Q42] 连接条件附加过滤
来源：http://hz.yangfankeji.com/gtfogwwhxr.html

SELECT u.name, o.amount FROM users u
来源：http://hz.ivvv.top/gtknugzvzt.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.nanxinkj.top/gttzshvefn.html

[Q43] 标量子查询
来源：http://hz.daria6918.cn/gtpyudnqai.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.yueranfly.top/gtqlhkbeue.html

[Q44] IN 子查询
来源：http://hz.9152youxi.cn/gteyjjxdlb.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.gotoacloud.top/gtdlsnufgr.html

[Q45] EXISTS 判断存在
来源：http://hz.zycfv.cn/gtreswionw.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.shanyushiyangkeji.top/gtbrdkzbrl.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.xingfuxueyuan.xyz/gtiqzbfukp.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.tianlin.xyz/gtcqqpwppd.html

[Q47] 与平均值比较
来源：http://hz.mhx1999.top/gtyutpjmal.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.meibo888.top/gtxrgeptjg.html

[Q48] CTE 公用表表达式
来源：http://hz.hnxiangtu.top/gtegshhvyf.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.ivvv.top/gtzpubbsea.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.yongpay.top/gtbpykwjqv.html

[Q49] 更新单行
来源：http://hz.zdqjudy.top/gtxnsdwvad.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.redwolf501.top/gtvufycqfr.html

[Q50] 批量更新
来源：http://hz.xuanzx.com/gtcvvuaudb.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.aibaodan.cn/gtetpqnftc.html

[Q51] 用子查询更新
来源：http://hz.pengpengdd.cyou/gtpqbkswlj.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.nanxuanxn.top/gtzifdgjgd.html

[Q52] 删除指定行
来源：http://hz.chenlongwang.top/gtnanxuxks.html

DELETE FROM users WHERE id = 10;
来源：http://hz.ywan-chungtsiang.top/gtnihmjcfv.html

[Q53] 按条件删除
来源：http://hz.quarkkingdee.top/gtfbefomwa.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.shangyingyoupin.top/gtxbgatiim.html

[Q54] 清空表
来源：http://hz.jianghu66.top/gtmfuovdoo.html

TRUNCATE TABLE logs;
来源：http://hz.daxiang520.top/gteqcmnwkg.html

[Q55] 排名（并列占位）
来源：http://hz.tianlin.xyz/gtjwnrxhat.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.yj202588.top/gthsnjtgtj.html

[Q56] 密集排名（并列不占位）
来源：http://hz.dashuyun.cn/gtmfchpilu.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.hnqzz.top/gtdicpyuok.html

[Q57] 行号
来源：http://hz.yvedp.cn/gtqhmbxuxe.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.yj20258888.top/gtbryafxeg.html

[Q58] 累计求和
来源：http://hz.jinqigufen.top/gtkoyeblmy.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.mhx1999.top/gtwytqhtax.html

[Q59] 分组内累计
来源：http://hz.xziqi.cn/gtxcqdpxbm.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.quarkkingdee.top/gtkldmjlys.html

[Q60] 取上一行 / 下一行
来源：http://hz.fengsongda.top/gtawmthucm.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.shzxlz.cn/gtjsmjxdfh.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.zhoulong.xyz/gtaanhcwxl.html

[Q61] 移动平均
来源：http://hz.shanyushiyangtech.top/gtksdgwcky.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.xylfe.cn/gttstyijhx.html

[Q62] 分组占比
来源：http://hz.meibo888.top/gtqmneevix.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.jinqigfzy.top/gtjlgbvqmq.html

[Q63] 开启事务
来源：http://hz.cheryme.top/gtjzgcawfy.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.aizwys.cn/gtsnizrucb.html

[Q64] 提交事务
来源：http://hz.hnxiangtu.top/gtfpcovkls.html

COMMIT;
来源：http://hz.yj20258.top/gtbqtsjvbu.html

[Q65] 回滚事务
来源：http://hz.gzhubu.top/gtwtgjqfpy.html

ROLLBACK;
来源：http://hz.yj20258888.top/gtxrftnnhz.html

[Q66] 行锁查询
来源：http://hz.yongpay.top/gtmhuvekps.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.andypj.xyz/gtmfdytwec.html

[Q67] 设置隔离级别
来源：http://hz.zhengqikj.top/gtkxhhfefc.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.smart0.xyz/gtqngoylkg.html

[Q68] 保存点
来源：http://hz.zhaomingkeji.xyz/gtoidqaktb.html

SAVEPOINT sp1;
来源：http://hz.daxiang520.top/gtqbbqwdcn.html

ROLLBACK TO sp1;
来源：http://hz.shzxlz.cn/gtuynxadnu.html

[Q69] 查看执行计划
来源：http://hz.kuanghao11.cn/gtfybaojdy.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.daria6918.cn/gterwhpmxu.html

[Q70] 更新统计信息
来源：http://hz.gzhubu.top/gtgcibaujr.html

ANALYZE TABLE users;
来源：http://hz.zhiwuduotai.top/gtwurxrdqk.html

[Q71] 查看建表语句
来源：http://hz.mhx1999.top/gtasewtgdb.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.dashuyun.cn/gtireewote.html

[Q72] 查看索引
来源：http://hz.hywenlv.cn/gtnvzbrpce.html

SHOW INDEX FROM users;
来源：http://hz.kuanghao11.cn/gtfrpsnksq.html

[Q73] 查看表状态
来源：http://hz.chenzaomai.com/gtuvumzrbj.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.9152youxi.cn/gtvegpuksh.html

[Q74] 强制使用索引
来源：http://hz.shanyushiyangkeji.top/gtjcolqsdr.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.shanyushiyangkeji.top/gtlapareyk.html

[Q75] 日期格式化
来源：http://hz.c1oappe.top/gtxbpzbfnc.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.jqgufenzy.top/gtkzrzivpe.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.hnqzz.top/gtdsizfyfk.html

[Q76] 按天统计
来源：http://hz.tanke756.top/gtpzicyiec.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.daria6918.cn/gteajanjje.html

[Q77] 时间加减
来源：http://hz.hongshengwenyu.top/gteznckdgz.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.yj20258888.top/gtuysksnwt.html

[Q78] 当前时间
来源：http://hz.jinqigufen.top/gtjvzfgvfl.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.9152youxi.cn/gtgpcoxfeh.html

[Q79] 字符串拼接
来源：http://hz.shuidangran.top/gtayagvdmv.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.gogol.net.cn/gtlumrkaje.html

[Q80] 字符串截取
来源：http://hz.guannengcc.top/gtoczikerg.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.ybcxt.top/gtckvreuov.html

[Q81] 字符串替换
来源：http://hz.jqgfzy.top/gtgwiarqty.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.fzhhl.top/gtclhfcrdd.html

[Q82] 字符长度与字节长度
来源：http://hz.zhoulong.xyz/gtaqusozqm.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.guannengcc.top/gtujuncvdz.html

[Q83] 大小写转换
来源：http://hz.zhiwuduotai.top/gttlmcnohk.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.jqgufenzy.top/gtrqadciwl.html

[Q84] 去除首尾空格
来源：http://hz.zhengqikj.top/gtzrijocrx.html

SELECT TRIM(name) FROM users;
来源：http://hz.fzhhl.top/gtmngrdxuu.html

[Q85] 数值取整
来源：http://hz.smart0.xyz/gtzeslfocn.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.svipenyu.cn/gttgybptmx.html

[Q86] 读取 JSON 字段
来源：http://hz.yj20258.top/gtpowglgji.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.zhengqikj.top/gtnmelxdyk.html

[Q87] JSON 字段做条件
来源：http://hz.chenlongwang.top/gtipwfdspp.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.shzxlz.cn/gthjwzkqgu.html

[Q88] 行转列（条件聚合）
来源：http://hz.ybcxt.top/gtiwurzqlr.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.ydzc1.top/gtelakboae.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.smart0.xyz/gtzevtidaa.html

[Q89] 判断表是否存在
来源：http://hz.feifeiyinyue.top/gtvhfvrrwv.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.birdmap.top/gtlpjmqenu.html

[Q90] 生成序号列
来源：http://hz.hammf.cn/gtjnpmzfia.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.shangyingyoupin.top/gtbrbcfwvc.html

================================================================================
来源：http://hz.gzhubu.top/gtqpttdwpp.html

R. Bash 专题
来源：http://hz.chenjidiqi.icu/gtsdajpumy.html

================================================================================
来源：http://hz.meibo888.top/gtjsviyful.html

[R01] shebang 与严格模式
来源：http://hz.zhijiandao.cn/gtbtmlyoqe.html

#!/usr/bin/env bash
来源：http://hz.zhengqikj.top/gtmlsbjdml.html

set -euo pipefail
来源：http://hz.pengpengdd.cyou/gtlfouabxl.html

[R02] 变量赋值与使用
来源：http://hz.zhaomingkeji.xyz/gtzkhbpjvx.html

name="Tom"; echo "$name"
来源：http://hz.wangshuangyany.cn/gtfwrvkcmc.html

[R03] 只读变量
来源：http://hz.cashguo.top/gtbmdzmrhp.html

readonly PI=3.14
来源：http://hz.hammf.cn/gtugsrhinx.html

[R04] 位置参数
来源：http://hz.jqgufenzy.top/gtbltnjiqp.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.vqdsnc.cn/gtyaxnjyrg.html

[R05] 参数默认值
来源：http://hz.yj202588.top/gtivipxqtc.html

name="${1:-default}"
来源：http://hz.zhijiandao.cn/gtvpekhwac.html

[R06] 判断命令是否存在
来源：http://hz.52xcode.cn/gtfzyhhayw.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.xinyue.icu/gtpgverkwn.html

[R07] if 判断文件
来源：http://hz.aizwys.cn/gtbmjnscxg.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.zycfv.cn/gtpwpaicfi.html

[R08] 数值比较
来源：http://hz.gotoacloud.top/gthcqvpcnz.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.cheryme.top/gtkaivkmmn.html

[R09] 字符串比较
来源：http://hz.dashuyun.cn/gtcjwkiyuw.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.jiagoushi.top/gtnuquyshp.html

[R10] 正则匹配
来源：http://hz.cheryme.top/gtttbuqbqu.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.xylfe.cn/gtbrlzimga.html

[R11] case 多分支
来源：http://hz.yueranfly.top/gtjubspkhs.html

case "$1" in
来源：http://hz.shzxlz.cn/gtgwcscsrw.html

start) echo "启动" ;;
来源：http://hz.zhaomingkeji.xyz/gtchywvicl.html

stop)  echo "停止" ;;
来源：http://hz.yvedp.cn/gtkgwmbwqy.html

*)     echo "未知命令" ;;
来源：http://hz.ivvv.top/gtjqhhadbl.html

esac
来源：http://hz.9152youxi.cn/gtrfppfled.html

[R12] for 遍历文件
来源：http://hz.hammf.cn/gtwnutyroe.html

for f in *.txt; do echo "$f"; done
来源：http://hz.nanxinkj.top/gtztgljrav.html

[R13] for 计数循环
来源：http://hz.yj20258888.top/gtioovxxqa.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.nanxuanxn.top/gtjombnkmu.html

[R14] C 风格 for
来源：http://hz.havefunace.top/gtxwjneoqp.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.shanyushiyangkeji.top/gteemsosnt.html

[R15] while 逐行读文件
来源：http://hz.316326.xyz/gtfsicrmhe.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.sweek.top/gtudqgqted.html

[R16] until 等待条件
来源：http://hz.haohaochexian.top/gtuqcpgpkc.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.tanke756.top/gtbyqmtlgg.html

[R17] 数组定义与取值
来源：http://hz.ehwqpu.com/gtwnfoejbl.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.jinqigfzy.top/gtsnhrnvua.html

[R18] 遍历数组
来源：http://hz.zhaomingkeji.xyz/gtigsuzeeh.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.gaohongyu789.top/gtecskaycz.html

[R19] 数组长度
来源：http://hz.sufxvd.cn/gtfradkrzy.html

echo "${#arr[@]}"
来源：http://hz.yueranfly.top/gtldhtdvdx.html

[R20] 关联数组（字典）
来源：http://hz.wangshuangyany.cn/gtyksecgtz.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.shanyushiyangkeji.top/gtreppkdbn.html

[R21] 字符串长度
来源：http://hz.yongpay.top/gtqoieipbw.html

echo "${#s}"
来源：http://hz.aizwys.cn/gtsvaputzc.html

[R22] 截取子串
来源：http://hz.zhengqikj.top/gtjqjkomrk.html

echo "${s:0:5}"
来源：http://hz.0kj1m.cn/gtfupmsrkw.html

[R23] 字符串替换
来源：http://hz.zhoulong.xyz/gtrbzweudb.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.zhiwuduotai.top/gtbypmrkup.html

[R24] 大小写转换
来源：http://hz.xziqi.cn/gtzganoang.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.shuidangran.top/gtgislwujl.html

[R25] 去后缀 / 去前缀
来源：http://hz.yuxming.cn/gttkfwbkio.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.ydzc1.top/gtuoyfpdvr.html

[R26] 命令替换
来源：http://hz.ywan-chungtsiang.top/gtkvrviayp.html

now=$(date +%F); echo "$now"
来源：http://hz.jyoumei.cn/gtypquiddg.html

[R27] 算术展开
来源：http://hz.tian-w.cn/gtzmcucvul.html

echo $((1 + 2 * 3))
来源：http://hz.jinqigfzy.top/gtslvhtlzx.html

[R28] 浮点运算
来源：http://hz.aizwys.cn/gthfyvrikp.html

echo "scale=2; 10/3" | bc
来源：http://hz.yonumen.top/gtsrchzpox.html

[R29] 定义函数
来源：http://hz.xuanzx.com/gtgtvhpkzl.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.yj20258.top/gtpezliemg.html

[R30] 函数返回状态码
来源：http://hz.shanyushiyangtech.top/gttdinxqrx.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.guannengcc.top/gtekvlrmwk.html

[R31] 局部变量
来源：http://hz.iojbl.cn/gtzpsmrdvy.html

f() { local x=1; echo "$x"; }
来源：http://hz.wangdashe.top/gtiyxzpufy.html

[R32] 参数个数校验
来源：http://hz.c1oappe.top/gtwdthuvzw.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.zhixingplan.top/gtneyffaql.html

[R33] 捕获错误并提示行号
来源：http://hz.yvedp.cn/gtxifauput.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.chenzaomai.com/gtmkfaomur.html

[R34] 退出时清理
来源：http://hz.pycfn.com/gtegkzfzyi.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.yangfankeji.com/gtsodydtxs.html

[R35] 后台执行并等待
来源：http://hz.gzhubu.top/gtvrcgfjts.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.snrcjt.cn/gtlehbzorn.html

[R36] 并发执行多个任务
来源：http://hz.fzhhl.top/gthxkopsez.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.hywenlv.cn/gtnfptrikq.html

[R37] 把输出赋给变量
来源：http://hz.iojbl.cn/gttnrtuozu.html

files=$(ls -1)
来源：http://hz.ybcxt.top/gtxefhhkjr.html

[R38] 管道串联
来源：http://hz.zycfv.cn/gtqetgupmg.html

cat a.txt | grep -i error | wc -l
来源：http://hz.shanyushiyangtech.top/gtkvxggazh.html

[R39] 重定向标准输出与错误
来源：http://hz.jyoumei.cn/gtzfxydjab.html

cmd > out.log 2>&1
来源：http://hz.gotoacloud.top/gtwnipiuic.html

[R40] 追加写日志
来源：http://hz.sufxvd.cn/gtgsqcylit.html

echo "log" >> out.log
来源：http://hz.shzxlz.cn/gtavmsjbci.html

[R41] 丢弃输出
来源：http://hz.chenlongwang.top/gtyoilvnnq.html

cmd >/dev/null 2>&1
来源：http://hz.kuanghao11.cn/gtzmtvvkta.html

[R42] 输入重定向
来源：http://hz.snrcjt.cn/gtfaghxudy.html

wc -l < a.txt
来源：http://hz.jiagoushi.top/gtlyadffsk.html

[R43] 按名字查找文件
来源：http://hz.xuanzx.com/gtrvhjztsn.html

find . -name "*.log" -type f
来源：http://hz.hnxiangtu.top/gtidbtigva.html

[R44] 按修改时间查找
来源：http://hz.andypj.xyz/gtuaedoabh.html

find . -mtime -7 -type f
来源：http://hz.cdnleiting.top/gtjdudebub.html

[R45] 批量删除
来源：http://hz.jinqigfzy.top/gtatuuieml.html

find . -name "*.tmp" -delete
来源：http://hz.vqdsnc.cn/gtyrokndsr.html

[R46] 递归替换文件内容
来源：http://hz.yanxiufei.cn/gtixwxzhvf.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.hysaishi.cn/gttwfhkwij.html

[R47] sed 单行替换
来源：http://hz.nanxuanxn.top/gthainemag.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.hfpthk.cn/gtbudsjatu.html

[R48] awk 取指定列
来源：http://hz.nanxinkj.top/gtxvsysgqo.html

awk '{print $1, $3}' a.txt
来源：http://hz.cqqwz.cn/gtgnofzdpx.html

[R49] awk 带条件
来源：http://hz.gotoacloud.top/gtokbjxetu.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.yj20258.top/gtovghumlw.html

[R50] awk 求和
来源：http://hz.shanyushiyangkeji.top/gtnfxerymc.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.ybcxt.top/gttkxjjylm.html

[R51] 排序去重取前几
来源：http://hz.daria6918.cn/gtcmxqwlns.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.cucudq.cn/gtprnngdif.html

[R52] 统计行数
来源：http://hz.tian-w.cn/gtkwgwbfat.html

wc -l a.txt
来源：http://hz.fzhhl.top/gtzpvnyjke.html

[R53] 查看文件头与实时尾
来源：http://hz.gogol.net.cn/gtpohsddyg.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.chenzaomai.com/gthdrkqgkk.html

[R54] 比较两个文件
来源：http://hz.yvedp.cn/gtcvpeaxvq.html

diff a.txt b.txt
来源：http://hz.gaohongyu789.top/gtqrqclqyg.html

[R55] 压缩与解压
来源：http://hz.guannengcc.top/gtvjkfplcd.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.yonumen.top/gtjhgixypb.html

[R56] 远程拷贝
来源：http://hz.quarkkingdee.top/gtsbgvsswi.html

scp file user@host:/path/
来源：http://hz.fzhhl.top/gtrxlmxcxy.html

[R57] 远程执行命令
来源：http://hz.aizwys.cn/gtfsmddvqy.html

ssh user@host 'uptime'
来源：http://hz.tian-w.cn/gtzcjfbfhw.html

[R58] 下载文件
来源：http://hz.dashuyun.cn/gtcxsyueax.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.tanke756.top/gtohgzaksp.html

[R59] 发 POST JSON
来源：http://hz.pengpengdd.cyou/gtdvukohrv.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.sxryk.cn/gtikceismt.html

[R60] 只看 HTTP 状态码
来源：http://hz.ivvv.top/gtezksikia.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.ehwqpu.com/gtiewyxerf.html

[R61] 磁盘占用
来源：http://hz.daria6918.cn/gtnkjsvvfb.html

df -h;  du -sh *
来源：http://hz.xuetiantiany.cn/gtemtljagp.html

[R62] 找最占空间的文件
来源：http://hz.wangshuangyany.cn/gtmjmtpbdu.html

du -ah . | sort -rh | head -10
来源：http://hz.shangyingyoupin.top/gtqhpllrww.html

[R63] 内存与进程
来源：http://hz.zhixingplan.top/gtgaihdydi.html

free -h;  ps aux | grep nginx
来源：http://hz.yvedp.cn/gttngmrlss.html

[R64] 结束进程
来源：http://hz.feifeiyinyue.top/gtmooefzjf.html

kill -9 $(pgrep -f app.py)
来源：http://hz.cashguo.top/gteekxiwzg.html

[R65] 查看端口占用
来源：http://hz.smart0.xyz/gtnriwbxto.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.cashguo.top/gtqizloqge.html

[R66] 定时任务
来源：http://hz.xinyue.icu/gtyjzzihhn.html

crontab -e;  crontab -l
来源：http://hz.shanyushiyangkeji.top/gtbgtslpgc.html

[R67] 生成随机十六进制串
来源：http://hz.yanxiufei.cn/gtoeqkxbrc.html

openssl rand -hex 16
来源：http://hz.zhiwuduotai.top/gtgdwrbyma.html

[R68] 计算文件校验值
来源：http://hz.yuxming.cn/gtoqexpoex.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.sxryk.cn/gthmsbwrcg.html

[R69] 生成随机密码
来源：http://hz.wangshuangyany.cn/gtiyswiyvy.html

head -c 16 /dev/urandom | base64
来源：http://hz.zhongyouzk.top/gthzcjjhwz.html

[R70] 时间戳与互转
来源：http://hz.zhijiandao.cn/gtnbjouezi.html

date +%s;  date -d @1700000000
来源：http://hz.ybcxt.top/gtwjcorxfx.html

[R71] 日期格式化
来源：http://hz.c1oappe.top/gthesjcwxk.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.hfpthk.cn/gtwrswhrzt.html

[R72] 等待端口就绪
来源：http://hz.chenlongwang.top/gtrvaszcpv.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.cdnleiting.top/gtpuphvchh.html

[R73] 分割大日志
来源：http://hz.wangshuangyany.cn/gtadfamvjl.html

split -l 1000 big.log part_
来源：http://hz.chenzaomai.com/gtbgwfjbek.html

[R74] 批量重命名
来源：http://hz.xingfuxueyuan.xyz/gtbpihdaso.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.9152youxi.cn/gtqntkqiwi.html

[R75] 导出环境变量
来源：http://hz.wangdashe.top/gtetqyxncw.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.guowangkeji.top/gtclrjrxys.html

[R76] 使用临时文件
来源：http://hz.zhengqikj.top/gtvbpmqcts.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.iojbl.cn/gtvbgxggjn.html

[R77] 读取用户输入
来源：http://hz.ybcxt.top/gtufbjwbqt.html

read -rp "请输入: " ans
来源：http://hz.zhongyouzk.top/gtudesunml.html

[R78] 交互式菜单
来源：http://hz.guowangkeji.top/gtkxkdaijn.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.sweek.top/gtgmfrjiup.html

[R79] 解析命令行选项
来源：http://hz.zhengqikj.top/gtwgyhvchz.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.yj202588.top/gtuoxhwxiu.html

[R80] 查看脚本执行耗时
来源：http://hz.nanxuanxn.top/gtypvcfcxg.html

time ./run.sh
来源：http://hz.yj20258888.top/gtamhvpufc.html

================================================================================
来源：http://hz.yj20258888.top/gtqwhpiuxk.html

S. C / C++ 专题
来源：http://hz.ppjwa.cn/gtpkvegnxe.html

================================================================================
来源：http://hz.yangfankeji.com/gtaxqtituy.html

[S01] C：Hello World
来源：http://hz.hongshengwenyu.top/gtpuyyreye.html

#include <stdio.h>
来源：http://hz.cqqwz.cn/gthjwkycdu.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.zhijiandao.cn/gtgtwlhrsl.html

[S02] C：变量与格式化输出
来源：http://hz.quarkkingdee.top/gtvdnyaubd.html

int a = 10; printf("%d\n", a);
来源：http://hz.shanyushiyangtech.top/gtqtjhekls.html

[S03] C：读入整数
来源：http://hz.shzxlz.cn/gtvskkbrvi.html

int x; scanf("%d", &x);
来源：http://hz.gogol.net.cn/gtpzxwujdk.html

[S04] C：字符串复制
来源：http://hz.yongpay.top/gtzxrcbrhr.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.sweek.top/gtovjvvbsn.html

[S05] C：字符串长度
来源：http://hz.nanxuanxn.top/gtexpjituf.html

strlen(s)
来源：http://hz.bjfxy.top/gtxvqumyfh.html

[S06] C：字符串比较
来源：http://hz.sufxvd.cn/gtehmyttww.html

strcmp(a, b) == 0
来源：http://hz.smart0.xyz/gtohmgujtj.html

[S07] C：数组遍历求和
来源：http://hz.hammf.cn/gtmwqrlrmf.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.sufxvd.cn/gtlmfjmdxg.html

[S08] C：动态内存分配与释放
来源：http://hz.zdqjudy.top/gtyxdkdzzn.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.iojbl.cn/gtznbrlkfn.html

[S09] C：结构体定义与初始化
来源：http://hz.daxiang520.top/gtneftwbnr.html


<!-- 参考信息 -->