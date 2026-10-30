代发 wailian999

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.hesvh.cn/Article/details/grttmiiyc.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.fehbvm.com/Article/details/gvwgqliqp.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.fehbvm.com/Article/details/ggmtbwalz.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.zdbjq.cn/Article/details/gfuxggtlm.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.fehbvm.com/Article/details/gdjintakq.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.zdbjq.cn/Article/details/gtffgivov.sHtML

[Q43] 标量子查询
来源：http://m.share.fehbvm.com/Article/details/glitgxcqq.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.hesvh.cn/Article/details/gcjtoibpp.sHtML

[Q44] IN 子查询
来源：http://3g.zdbjq.cn/Article/details/gyjkspilf.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.fehbvm.com/Article/details/gknahqbgx.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.zdbjq.cn/Article/details/gwozxrmfh.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.hesvh.cn/Article/details/gypzulyxx.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.hesvh.cn/Article/details/gvspdmejx.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.hesvh.cn/Article/details/gyfekrxal.sHtML

[Q47] 与平均值比较
来源：http://read.share.zdbjq.cn/Article/details/giozhhpdq.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.zdbjq.cn/Article/details/gbihxhskv.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.hesvh.cn/Article/details/gycpoctlz.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.hesvh.cn/Article/details/givhshkpd.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.fehbvm.com/Article/details/ghstzwquz.sHtML

[Q49] 更新单行
来源：http://m.share.fehbvm.com/Article/details/givbbttog.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.fehbvm.com/Article/details/gkdsfzhrp.sHtML

[Q50] 批量更新
来源：http://blog.zdbjq.cn/Article/details/ggnuxalhm.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.fehbvm.com/Article/details/gackuxcok.sHtML

[Q51] 用子查询更新
来源：http://blog.hesvh.cn/Article/details/gwppcupuo.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.hesvh.cn/Article/details/gusumkpeb.sHtML

[Q52] 删除指定行
来源：http://blog.zdbjq.cn/Article/details/gmmxvjbqz.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.zdbjq.cn/Article/details/gclujvwmp.sHtML

[Q53] 按条件删除
来源：http://wap.zdbjq.cn/Article/details/gvmrvvlpu.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.hesvh.cn/Article/details/gechljxbt.sHtML

[Q54] 清空表
来源：http://mobile.fehbvm.com/Article/details/gqpgmzsnv.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.hesvh.cn/Article/details/gmzxywtik.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.zdbjq.cn/Article/details/gjlunzcrm.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.zdbjq.cn/Article/details/gecamkynu.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.hesvh.cn/Article/details/gdnlfmrra.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.zdbjq.cn/Article/details/ghrjdykso.sHtML

[Q57] 行号
来源：http://3g.fehbvm.com/Article/details/gqrhnhkov.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gpgufrekp.sHtML

[Q58] 累计求和
来源：http://www.share.zdbjq.cn/Article/details/ggqfizoon.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gvnlphfjp.sHtML

[Q59] 分组内累计
来源：http://www.m.share.zdbjq.cn/Article/details/griaglqyx.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gtildhyev.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.zdbjq.cn/Article/details/gwmjswhcf.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.hesvh.cn/Article/details/gymsknzbf.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gvpajeeag.sHtML

[Q61] 移动平均
来源：http://mobile.zdbjq.cn/Article/details/ggrtpmtuj.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.fehbvm.com/Article/details/gjvjxhyyg.sHtML

[Q62] 分组占比
来源：http://www.m.share.zdbjq.cn/Article/details/gmmajrpjt.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gbuqmiugg.sHtML

[Q63] 开启事务
来源：http://m.share.hesvh.cn/Article/details/gwebdshjc.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.hesvh.cn/Article/details/glpayayvs.sHtML

[Q64] 提交事务
来源：http://baike.zdbjq.cn/Article/details/gbkcyfuni.sHtML

COMMIT;
来源：http://blog.hesvh.cn/Article/details/gzsgjpopn.sHtML

[Q65] 回滚事务
来源：http://www.m.share.zdbjq.cn/Article/details/gaawwmdgi.sHtML

ROLLBACK;
来源：http://blog.hesvh.cn/Article/details/gkazxuxhu.sHtML

[Q66] 行锁查询
来源：http://m.share.zdbjq.cn/Article/details/gkqljjtkc.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.hesvh.cn/Article/details/gxfigzysv.sHtML

[Q67] 设置隔离级别
来源：http://blog.zdbjq.cn/Article/details/glddhdnhz.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.zdbjq.cn/Article/details/gexthpzup.sHtML

[Q68] 保存点
来源：http://wap.zdbjq.cn/Article/details/gzashezbx.sHtML

SAVEPOINT sp1;
来源：http://read.share.hesvh.cn/Article/details/ghebczzlq.sHtML

ROLLBACK TO sp1;
来源：http://www.share.hesvh.cn/Article/details/grzugttsh.sHtML

[Q69] 查看执行计划
来源：http://www.blog.zdbjq.cn/Article/details/gptiirmsh.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.hesvh.cn/Article/details/gnwcwzmrx.sHtML

[Q70] 更新统计信息
来源：http://mobile.fehbvm.com/Article/details/gnyskplpo.sHtML

ANALYZE TABLE users;
来源：http://baike.zdbjq.cn/Article/details/gzakbzpld.sHtML

[Q71] 查看建表语句
来源：http://baike.hesvh.cn/Article/details/gdyjvccld.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.zdbjq.cn/Article/details/gkkzupepr.sHtML

[Q72] 查看索引
来源：http://m.share.zdbjq.cn/Article/details/goigienkc.sHtML

SHOW INDEX FROM users;
来源：http://baike.fehbvm.com/Article/details/gfwevogki.sHtML

[Q73] 查看表状态
来源：http://3g.zdbjq.cn/Article/details/gujmznshy.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.hesvh.cn/Article/details/ggcooimas.sHtML

[Q74] 强制使用索引
来源：http://read.share.zdbjq.cn/Article/details/ghtrologl.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fehbvm.com/Article/details/gpiujfapj.sHtML

[Q75] 日期格式化
来源：http://read.share.hesvh.cn/Article/details/glecvjaul.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gpjwampud.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.hesvh.cn/Article/details/gvtlqzhxo.sHtML

[Q76] 按天统计
来源：http://3g.hesvh.cn/Article/details/grqusuqaa.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.fehbvm.com/Article/details/gqxsoobty.sHtML

[Q77] 时间加减
来源：http://www.m.share.zdbjq.cn/Article/details/gcqiiunia.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.zdbjq.cn/Article/details/gnvmcofzs.sHtML

[Q78] 当前时间
来源：http://read.share.fehbvm.com/Article/details/gdpqyodki.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.hesvh.cn/Article/details/gnvrobwbx.sHtML

[Q79] 字符串拼接
来源：http://blog.hesvh.cn/Article/details/gfervrzup.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.hesvh.cn/Article/details/gzxkonudk.sHtML

[Q80] 字符串截取
来源：http://baike.zdbjq.cn/Article/details/gsyoyikax.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.zdbjq.cn/Article/details/geppahgbi.sHtML

[Q81] 字符串替换
来源：http://www.blog.fehbvm.com/Article/details/gxkdslkbi.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.hesvh.cn/Article/details/gtoyfnipl.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.zdbjq.cn/Article/details/gqnxghrmq.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gbztimdtm.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fehbvm.com/Article/details/govmiunha.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gsdxxebiu.sHtML

[Q84] 去除首尾空格
来源：http://wap.zdbjq.cn/Article/details/gtvxflkap.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gdotfqwgd.sHtML

[Q85] 数值取整
来源：http://www.blog.hesvh.cn/Article/details/gwxckgqyz.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fehbvm.com/Article/details/gtdooxiwl.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.hesvh.cn/Article/details/gjbcdlnkk.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fehbvm.com/Article/details/gqshuccbz.sHtML

[Q87] JSON 字段做条件
来源：http://3g.hesvh.cn/Article/details/gwmqdzqbn.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.fehbvm.com/Article/details/gulvpdmsa.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.zdbjq.cn/Article/details/gqadbrdsw.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.hesvh.cn/Article/details/gvqsjkhju.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.hesvh.cn/Article/details/gptkielib.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fehbvm.com/Article/details/gqkokwgxa.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.hesvh.cn/Article/details/gajzdidlu.sHtML

[Q90] 生成序号列
来源：http://mobile.fehbvm.com/Article/details/gsrsgdfqk.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.hesvh.cn/Article/details/gbhupezyt.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gzqhqwxus.sHtML

R. Bash 专题
来源：http://baike.zdbjq.cn/Article/details/gqzijpfzv.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ghblodszf.sHtML

[R01] shebang 与严格模式
来源：http://3g.hesvh.cn/Article/details/gtvpiiiqb.sHtML

#!/usr/bin/env bash
来源：http://www.blog.zdbjq.cn/Article/details/gqgpstoba.sHtML

set -euo pipefail
来源：http://blog.hesvh.cn/Article/details/gznecrlxz.sHtML

[R02] 变量赋值与使用
来源：http://baike.zdbjq.cn/Article/details/ghmuyfpbe.sHtML

name="Tom"; echo "$name"
来源：http://blog.fehbvm.com/Article/details/gvemlzfin.sHtML

[R03] 只读变量
来源：http://wap.fehbvm.com/Article/details/gjuekkkhy.sHtML

readonly PI=3.14
来源：http://www.blog.hesvh.cn/Article/details/gyclfprbv.sHtML

[R04] 位置参数
来源：http://www.share.fehbvm.com/Article/details/gqqgbeggm.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.hesvh.cn/Article/details/gpcuaqnfp.sHtML

[R05] 参数默认值
来源：http://baike.hesvh.cn/Article/details/gbhehuqlz.sHtML

name="${1:-default}"
来源：http://m.share.fehbvm.com/Article/details/gvewbvpti.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fehbvm.com/Article/details/gugywriqm.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/gehwjarpf.sHtML

[R07] if 判断文件
来源：http://www.share.hesvh.cn/Article/details/gcjrrafpg.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fehbvm.com/Article/details/gfpjjoxkd.sHtML

[R08] 数值比较
来源：http://mobile.hesvh.cn/Article/details/gqbisnruv.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fehbvm.com/Article/details/gfqvctttt.sHtML

[R09] 字符串比较
来源：http://wap.fehbvm.com/Article/details/gatvmcokg.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.hesvh.cn/Article/details/gglqbhfro.sHtML

[R10] 正则匹配
来源：http://read.share.zdbjq.cn/Article/details/gfeacylwr.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.zdbjq.cn/Article/details/gblrewsst.sHtML

[R11] case 多分支
来源：http://read.share.zdbjq.cn/Article/details/gguemgvwk.sHtML

case "$1" in
来源：http://mobile.fehbvm.com/Article/details/gqgzvoiwo.sHtML

start) echo "启动" ;;
来源：http://mobile.fehbvm.com/Article/details/gfwuqzizy.sHtML

stop)  echo "停止" ;;
来源：http://wap.zdbjq.cn/Article/details/gfrrlbrsg.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fehbvm.com/Article/details/gwihmdoji.sHtML

esac
来源：http://wap.hesvh.cn/Article/details/giiyckizj.sHtML

[R12] for 遍历文件
来源：http://3g.zdbjq.cn/Article/details/goywfadyp.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.hesvh.cn/Article/details/gvtwodvri.sHtML

[R13] for 计数循环
来源：http://baike.hesvh.cn/Article/details/gadqwzblq.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fehbvm.com/Article/details/ggwqerfgo.sHtML

[R14] C 风格 for
来源：http://m.share.zdbjq.cn/Article/details/gupnflaws.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.hesvh.cn/Article/details/gwhqizclw.sHtML

[R15] while 逐行读文件
来源：http://baike.hesvh.cn/Article/details/gllfyltrv.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fehbvm.com/Article/details/gqvoqegfl.sHtML

[R16] until 等待条件
来源：http://3g.fehbvm.com/Article/details/gkzsaqdep.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.hesvh.cn/Article/details/gxjyzgdok.sHtML

[R17] 数组定义与取值
来源：http://blog.zdbjq.cn/Article/details/givzazhot.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fehbvm.com/Article/details/gnownagox.sHtML

[R18] 遍历数组
来源：http://www.m.share.zdbjq.cn/Article/details/gmcvyvrhb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.zdbjq.cn/Article/details/gfcbvotfy.sHtML

[R19] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/gmgkbelkh.sHtML

echo "${#arr[@]}"
来源：http://read.share.hesvh.cn/Article/details/gyhcwnprf.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fehbvm.com/Article/details/gocpcgzua.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.zdbjq.cn/Article/details/gtztiqpvo.sHtML

[R21] 字符串长度
来源：http://www.m.share.fehbvm.com/Article/details/ggoqxhiym.sHtML

echo "${#s}"
来源：http://www.share.fehbvm.com/Article/details/grneoofjc.sHtML

[R22] 截取子串
来源：http://www.m.share.hesvh.cn/Article/details/gtckqxlwq.sHtML

echo "${s:0:5}"
来源：http://3g.zdbjq.cn/Article/details/gmzxxqglr.sHtML

[R23] 字符串替换
来源：http://baike.zdbjq.cn/Article/details/gngozxmgg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.zdbjq.cn/Article/details/gjcyxzuje.sHtML

[R24] 大小写转换
来源：http://baike.zdbjq.cn/Article/details/gmfgumqoo.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fehbvm.com/Article/details/gqkmprrul.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.hesvh.cn/Article/details/gtgpnvdtd.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.hesvh.cn/Article/details/gmblrqrha.sHtML

[R26] 命令替换
来源：http://baike.zdbjq.cn/Article/details/grvhwvuhv.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.hesvh.cn/Article/details/gwrfwpemj.sHtML

[R27] 算术展开
来源：http://www.blog.zdbjq.cn/Article/details/gjigvafma.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fehbvm.com/Article/details/gnpwjpwvv.sHtML

[R28] 浮点运算
来源：http://blog.fehbvm.com/Article/details/giyoctivt.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.hesvh.cn/Article/details/gpdqjidmr.sHtML

[R29] 定义函数
来源：http://www.share.hesvh.cn/Article/details/ghzyrmcho.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.hesvh.cn/Article/details/gmjvxsknp.sHtML

[R30] 函数返回状态码
来源：http://wap.hesvh.cn/Article/details/gprbhqgvg.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.hesvh.cn/Article/details/goqvxirpr.sHtML

[R31] 局部变量
来源：http://3g.hesvh.cn/Article/details/gxezwmrqk.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.hesvh.cn/Article/details/gypexojfo.sHtML

[R32] 参数个数校验
来源：http://www.share.zdbjq.cn/Article/details/gomhczzhy.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.hesvh.cn/Article/details/glcfqdxxb.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fehbvm.com/Article/details/gtzievnud.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fehbvm.com/Article/details/grwxnxgec.sHtML

[R34] 退出时清理
来源：http://blog.fehbvm.com/Article/details/gyjvlcmtz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/glvbhvutd.sHtML

[R35] 后台执行并等待
来源：http://wap.zdbjq.cn/Article/details/gnzqfbwkp.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.zdbjq.cn/Article/details/gtajhgdet.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fehbvm.com/Article/details/gefsiqgxl.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.hesvh.cn/Article/details/glawtdnfa.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fehbvm.com/Article/details/gzmfnajre.sHtML

files=$(ls -1)
来源：http://mobile.hesvh.cn/Article/details/gofmhcqov.sHtML

[R38] 管道串联
来源：http://wap.zdbjq.cn/Article/details/gknnhfuny.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.zdbjq.cn/Article/details/gnzfeivyj.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fehbvm.com/Article/details/gufguxqyt.sHtML

cmd > out.log 2>&1
来源：http://read.share.fehbvm.com/Article/details/gqtezjvlg.sHtML

[R40] 追加写日志
来源：http://www.m.share.fehbvm.com/Article/details/giphgqpfa.sHtML

echo "log" >> out.log
来源：http://www.share.zdbjq.cn/Article/details/gmwvknoht.sHtML

[R41] 丢弃输出
来源：http://blog.fehbvm.com/Article/details/gbpvpmchd.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fehbvm.com/Article/details/gfjwppwuv.sHtML

[R42] 输入重定向
来源：http://www.m.share.fehbvm.com/Article/details/gpommcnjy.sHtML

wc -l < a.txt
来源：http://wap.fehbvm.com/Article/details/gesfowxoq.sHtML

[R43] 按名字查找文件
来源：http://blog.hesvh.cn/Article/details/gwcespvcf.sHtML

find . -name "*.log" -type f
来源：http://blog.hesvh.cn/Article/details/gcrbpahmc.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fehbvm.com/Article/details/gchlzhjdf.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.zdbjq.cn/Article/details/guemembfs.sHtML

[R45] 批量删除
来源：http://www.blog.hesvh.cn/Article/details/gtqvdyofb.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.hesvh.cn/Article/details/ghzhiwwgs.sHtML

[R46] 递归替换文件内容
来源：http://baike.fehbvm.com/Article/details/ghzivriwd.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fehbvm.com/Article/details/gcejyiudn.sHtML

[R47] sed 单行替换
来源：http://www.blog.zdbjq.cn/Article/details/geaznlmcl.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.hesvh.cn/Article/details/gazozvtck.sHtML

[R48] awk 取指定列
来源：http://mobile.hesvh.cn/Article/details/gwuihgtvh.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fehbvm.com/Article/details/gpylwwtpy.sHtML

[R49] awk 带条件
来源：http://read.share.zdbjq.cn/Article/details/gjlwatxsf.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.hesvh.cn/Article/details/gmnrrvena.sHtML

[R50] awk 求和
来源：http://www.m.share.hesvh.cn/Article/details/gymyswbek.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gnvuqbwbb.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.hesvh.cn/Article/details/gvfohghgd.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.zdbjq.cn/Article/details/gzpnfsacw.sHtML

[R52] 统计行数
来源：http://www.share.hesvh.cn/Article/details/gtrfskyjm.sHtML

wc -l a.txt
来源：http://m.share.fehbvm.com/Article/details/ghiuahxkl.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.zdbjq.cn/Article/details/garocbokl.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.zdbjq.cn/Article/details/ggvfaaxel.sHtML

[R54] 比较两个文件
来源：http://www.blog.hesvh.cn/Article/details/gnucykuhq.sHtML

diff a.txt b.txt
来源：http://www.share.hesvh.cn/Article/details/gbyakzemi.sHtML

[R55] 压缩与解压
来源：http://mobile.fehbvm.com/Article/details/gvuiaaozf.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.zdbjq.cn/Article/details/gdmzhrzmp.sHtML

[R56] 远程拷贝
来源：http://mobile.zdbjq.cn/Article/details/gvcyaxwiw.sHtML

scp file user@host:/path/
来源：http://www.m.share.hesvh.cn/Article/details/guonqnuut.sHtML

[R57] 远程执行命令
来源：http://blog.zdbjq.cn/Article/details/gzlaaumii.sHtML

ssh user@host 'uptime'
来源：http://wap.hesvh.cn/Article/details/gkpbnrtqh.sHtML

[R58] 下载文件
来源：http://www.share.fehbvm.com/Article/details/ggntjjnvn.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.zdbjq.cn/Article/details/glkxhdazp.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fehbvm.com/Article/details/gcgozbmuc.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.zdbjq.cn/Article/details/gqittelym.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fehbvm.com/Article/details/gbuqdjbyz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.zdbjq.cn/Article/details/gclqkobvw.sHtML

[R61] 磁盘占用
来源：http://3g.fehbvm.com/Article/details/gbqrvksit.sHtML

df -h;  du -sh *
来源：http://wap.zdbjq.cn/Article/details/gsjljjogd.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fehbvm.com/Article/details/gglmxiftz.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fehbvm.com/Article/details/gwnlzfptf.sHtML

[R63] 内存与进程
来源：http://read.share.zdbjq.cn/Article/details/gitpupdvj.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.zdbjq.cn/Article/details/ghnjfaevc.sHtML

[R64] 结束进程
来源：http://blog.zdbjq.cn/Article/details/gemnyocwy.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fehbvm.com/Article/details/gvewxesnv.sHtML

[R65] 查看端口占用
来源：http://mobile.hesvh.cn/Article/details/gdbznvtop.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.hesvh.cn/Article/details/gefzuoual.sHtML

[R66] 定时任务
来源：http://m.share.fehbvm.com/Article/details/grflzypsd.sHtML

crontab -e;  crontab -l
来源：http://mobile.fehbvm.com/Article/details/guwirjxjz.sHtML

[R67] 生成随机十六进制串
来源：http://blog.hesvh.cn/Article/details/gaxxzjhdn.sHtML

openssl rand -hex 16
来源：http://read.share.zdbjq.cn/Article/details/gtnzpjzyb.sHtML

[R68] 计算文件校验值
来源：http://blog.zdbjq.cn/Article/details/gqostydfl.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.zdbjq.cn/Article/details/gvpvydcsh.sHtML

[R69] 生成随机密码
来源：http://baike.fehbvm.com/Article/details/gtymegqrw.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.zdbjq.cn/Article/details/guttjcgjf.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.hesvh.cn/Article/details/gtgvebtmk.sHtML

date +%s;  date -d @1700000000
来源：http://blog.hesvh.cn/Article/details/gfwzobnbi.sHtML

[R71] 日期格式化
来源：http://baike.zdbjq.cn/Article/details/gxxyobthn.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.hesvh.cn/Article/details/gcafwxlka.sHtML

[R72] 等待端口就绪
来源：http://baike.fehbvm.com/Article/details/grjrchsja.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fehbvm.com/Article/details/gfuvgoyev.sHtML

[R73] 分割大日志
来源：http://m.share.hesvh.cn/Article/details/gslufitgh.sHtML

split -l 1000 big.log part_
来源：http://blog.fehbvm.com/Article/details/ghslovjzb.sHtML

[R74] 批量重命名
来源：http://3g.zdbjq.cn/Article/details/gztivlexb.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fehbvm.com/Article/details/gcepntcse.sHtML

[R75] 导出环境变量
来源：http://www.blog.hesvh.cn/Article/details/gecpdmvsv.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.zdbjq.cn/Article/details/gkdbnldcm.sHtML

[R76] 使用临时文件
来源：http://mobile.hesvh.cn/Article/details/gvicndfrr.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fehbvm.com/Article/details/gwcauifvc.sHtML

[R77] 读取用户输入
来源：http://www.share.fehbvm.com/Article/details/gpvitfzhx.sHtML

read -rp "请输入: " ans
来源：http://3g.hesvh.cn/Article/details/gjdbhdvgq.sHtML

[R78] 交互式菜单
来源：http://3g.fehbvm.com/Article/details/gpgshkfsc.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.hesvh.cn/Article/details/gtglmakru.sHtML

[R79] 解析命令行选项
来源：http://baike.zdbjq.cn/Article/details/geywajrel.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fehbvm.com/Article/details/gwyvplteg.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.hesvh.cn/Article/details/gawircvnz.sHtML

time ./run.sh
来源：http://blog.hesvh.cn/Article/details/gaotxzmhf.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gvhxcautb.sHtML

S. C / C++ 专题
来源：http://www.share.fehbvm.com/Article/details/gmakyeryu.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gngkkfzsu.sHtML

[S01] C：Hello World
来源：http://read.share.hesvh.cn/Article/details/gwoczysot.sHtML

#include <stdio.h>
来源：http://m.share.fehbvm.com/Article/details/glrqjxkiy.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.hesvh.cn/Article/details/gdkfgpihw.sHtML

[S02] C：变量与格式化输出
来源：http://blog.zdbjq.cn/Article/details/gakzsnmdk.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.zdbjq.cn/Article/details/ghujvjjtx.sHtML

[S03] C：读入整数
来源：http://m.share.zdbjq.cn/Article/details/gciorkfjm.sHtML

int x; scanf("%d", &x);
来源：http://baike.zdbjq.cn/Article/details/gkrmozild.sHtML

[S04] C：字符串复制
来源：http://www.m.share.hesvh.cn/Article/details/gynxclite.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.zdbjq.cn/Article/details/gkxvqdpzs.sHtML

[S05] C：字符串长度
来源：http://baike.zdbjq.cn/Article/details/gpkbmgcip.sHtML

strlen(s)
来源：http://mobile.zdbjq.cn/Article/details/gqdjojfwo.sHtML

[S06] C：字符串比较
来源：http://baike.zdbjq.cn/Article/details/gpqkbbmdk.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.zdbjq.cn/Article/details/gnqlttdhi.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fehbvm.com/Article/details/gtwnzzakg.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fehbvm.com/Article/details/gtiyutkck.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.hesvh.cn/Article/details/gwzyoxpoq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.zdbjq.cn/Article/details/gsikmebmp.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fehbvm.com/Article/details/gbjlclkwf.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.hesvh.cn/Article/details/gapyhpoku.sHtML

[S10] C：指针与解引用
来源：http://www.share.hesvh.cn/Article/details/gvozccoza.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fehbvm.com/Article/details/gbjndtwoh.sHtML

[S11] C：逐行读文件
来源：http://blog.fehbvm.com/Article/details/guxphsrcg.sHtML


<!-- 参考信息 -->