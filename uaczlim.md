代发 wailian999

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gcraoigbr.sHtML

[Q30] 分组统计
来源：http://baike.hesvh.cn/Article/details/gekencwkz.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gzmuafgcg.sHtML

[Q31] 分组后过滤
来源：http://blog.hesvh.cn/Article/details/guxyibhfc.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.hesvh.cn/Article/details/gkvputyyg.sHtML

[Q32] 分组拼接字符串
来源：http://wap.fehbvm.com/Article/details/gvllzfpnk.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/gridowxdg.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.zdbjq.cn/Article/details/grdfxfffg.sHtML

[Q33] 多列分组
来源：http://3g.zdbjq.cn/Article/details/gxqkwzcbw.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.hesvh.cn/Article/details/gmhsoggqv.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.fehbvm.com/Article/details/gucqbmfjz.sHtML

SELECT * FROM (
来源：http://mobile.zdbjq.cn/Article/details/gayisagit.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.zdbjq.cn/Article/details/gdjtuxpze.sHtML

) t WHERE rn = 1;
来源：http://baike.fehbvm.com/Article/details/glydoivll.sHtML

[Q35] 内连接
来源：http://read.share.zdbjq.cn/Article/details/gleqwrqhk.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fehbvm.com/Article/details/gdmjurwur.sHtML

[Q36] 左连接
来源：http://m.share.fehbvm.com/Article/details/gylnflgqy.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/gaegvjxjf.sHtML

[Q37] 右连接
来源：http://m.share.fehbvm.com/Article/details/ggdwyjvaw.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.fehbvm.com/Article/details/goyuhkqtw.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.hesvh.cn/Article/details/gqtiyppjc.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.zdbjq.cn/Article/details/gmebrwxzs.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.fehbvm.com/Article/details/guogkuyfz.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.fehbvm.com/Article/details/gsiwdlxvs.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.hesvh.cn/Article/details/gkxjgubrn.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.zdbjq.cn/Article/details/gbpztdxqk.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.hesvh.cn/Article/details/gntmclzzq.sHtML

[Q41] 多表连接
来源：http://www.share.zdbjq.cn/Article/details/gdtibiwbe.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.hesvh.cn/Article/details/gpqwyrrql.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.zdbjq.cn/Article/details/gtqdfunzm.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.fehbvm.com/Article/details/gnahcevgj.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.hesvh.cn/Article/details/gzwipxrlc.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.fehbvm.com/Article/details/gtyuxdrpa.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.zdbjq.cn/Article/details/gvzhsoemz.sHtML

[Q43] 标量子查询
来源：http://blog.hesvh.cn/Article/details/gsmlexlky.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.fehbvm.com/Article/details/gcnezpxur.sHtML

[Q44] IN 子查询
来源：http://m.share.hesvh.cn/Article/details/ggiiylhys.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.fehbvm.com/Article/details/gibaccyrj.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.hesvh.cn/Article/details/ggbenycxb.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.hesvh.cn/Article/details/gxkryuvnm.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.zdbjq.cn/Article/details/gvqsxzznx.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.hesvh.cn/Article/details/gucwvkvkg.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.zdbjq.cn/Article/details/ghlokicih.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.zdbjq.cn/Article/details/gcleceyxa.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.fehbvm.com/Article/details/gcwglpmlx.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.zdbjq.cn/Article/details/gfuljkice.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.hesvh.cn/Article/details/gqijehptm.sHtML

[Q49] 更新单行
来源：http://m.share.zdbjq.cn/Article/details/gxctihmvf.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.hesvh.cn/Article/details/gnknyfjhq.sHtML

[Q50] 批量更新
来源：http://blog.zdbjq.cn/Article/details/grmxcuyio.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.zdbjq.cn/Article/details/gxlguifbe.sHtML

[Q51] 用子查询更新
来源：http://blog.hesvh.cn/Article/details/glhbcjrsy.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.hesvh.cn/Article/details/gefrwyzjp.sHtML

[Q52] 删除指定行
来源：http://mobile.hesvh.cn/Article/details/gapqoaokm.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.fehbvm.com/Article/details/gzuqjwjch.sHtML

[Q53] 按条件删除
来源：http://www.m.share.fehbvm.com/Article/details/gjbupvycm.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.hesvh.cn/Article/details/gbqgnjjyl.sHtML

[Q54] 清空表
来源：http://wap.hesvh.cn/Article/details/gyasfjrux.sHtML

TRUNCATE TABLE logs;
来源：http://3g.fehbvm.com/Article/details/gwdhjkgsy.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.fehbvm.com/Article/details/gahasnwwt.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.zdbjq.cn/Article/details/gkgkdrdrq.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.zdbjq.cn/Article/details/gvbfsuebp.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.hesvh.cn/Article/details/gpaqlipqz.sHtML

[Q57] 行号
来源：http://www.blog.fehbvm.com/Article/details/gqupfqinj.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.hesvh.cn/Article/details/gtlbwhtki.sHtML

[Q58] 累计求和
来源：http://read.share.hesvh.cn/Article/details/gqzelfwfn.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gungwqgll.sHtML

[Q59] 分组内累计
来源：http://m.share.hesvh.cn/Article/details/ghbzngkhe.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.fehbvm.com/Article/details/gdhiwkkkq.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.zdbjq.cn/Article/details/grcjeovwh.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.hesvh.cn/Article/details/grxuupfqq.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.fehbvm.com/Article/details/gtlljmpwm.sHtML

[Q61] 移动平均
来源：http://3g.fehbvm.com/Article/details/gtghkboau.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/ghzridrpz.sHtML

[Q62] 分组占比
来源：http://www.m.share.hesvh.cn/Article/details/gptguyggp.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gioubtelh.sHtML

[Q63] 开启事务
来源：http://www.blog.fehbvm.com/Article/details/gpthinfmv.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.fehbvm.com/Article/details/gffndifau.sHtML

[Q64] 提交事务
来源：http://m.share.zdbjq.cn/Article/details/glxzzyrdq.sHtML

COMMIT;
来源：http://wap.hesvh.cn/Article/details/ggbouldyu.sHtML

[Q65] 回滚事务
来源：http://read.share.zdbjq.cn/Article/details/gptashwbl.sHtML

ROLLBACK;
来源：http://3g.fehbvm.com/Article/details/gkpxtwnpr.sHtML

[Q66] 行锁查询
来源：http://mobile.hesvh.cn/Article/details/gidvqsmks.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.hesvh.cn/Article/details/gqqtmzywc.sHtML

[Q67] 设置隔离级别
来源：http://blog.zdbjq.cn/Article/details/ghcdoryri.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.zdbjq.cn/Article/details/gbicyvwdl.sHtML

[Q68] 保存点
来源：http://baike.fehbvm.com/Article/details/gvssxoyvc.sHtML

SAVEPOINT sp1;
来源：http://baike.fehbvm.com/Article/details/gwllmysfz.sHtML

ROLLBACK TO sp1;
来源：http://blog.hesvh.cn/Article/details/gnswyyize.sHtML

[Q69] 查看执行计划
来源：http://mobile.fehbvm.com/Article/details/gnmkhmekp.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.hesvh.cn/Article/details/ghchwxmiv.sHtML

[Q70] 更新统计信息
来源：http://www.blog.hesvh.cn/Article/details/gjgtrzpli.sHtML

ANALYZE TABLE users;
来源：http://www.blog.hesvh.cn/Article/details/grxtjrdri.sHtML

[Q71] 查看建表语句
来源：http://m.share.hesvh.cn/Article/details/gvzlyjajx.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.zdbjq.cn/Article/details/guojinryz.sHtML

[Q72] 查看索引
来源：http://read.share.hesvh.cn/Article/details/ggcfaycjf.sHtML

SHOW INDEX FROM users;
来源：http://wap.zdbjq.cn/Article/details/gnoxnvbln.sHtML

[Q73] 查看表状态
来源：http://mobile.hesvh.cn/Article/details/ggabyzhiu.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.zdbjq.cn/Article/details/gpxvotmzp.sHtML

[Q74] 强制使用索引
来源：http://m.share.hesvh.cn/Article/details/gncwwobwz.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fehbvm.com/Article/details/gjknrdnhl.sHtML

[Q75] 日期格式化
来源：http://3g.hesvh.cn/Article/details/gljcjilgp.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.zdbjq.cn/Article/details/glreepczo.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.zdbjq.cn/Article/details/gfrdvksly.sHtML

[Q76] 按天统计
来源：http://mobile.zdbjq.cn/Article/details/gxwkqqlyq.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.fehbvm.com/Article/details/gzxlreobr.sHtML

[Q77] 时间加减
来源：http://www.blog.fehbvm.com/Article/details/gpxmklcqx.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.zdbjq.cn/Article/details/gdyfqnteh.sHtML

[Q78] 当前时间
来源：http://mobile.zdbjq.cn/Article/details/gzckplaia.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.zdbjq.cn/Article/details/gxmqrhoti.sHtML

[Q79] 字符串拼接
来源：http://mobile.hesvh.cn/Article/details/gosfmowcl.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.hesvh.cn/Article/details/gjrbvyahs.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fehbvm.com/Article/details/gimfqgiwa.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.zdbjq.cn/Article/details/geyctubve.sHtML

[Q81] 字符串替换
来源：http://3g.fehbvm.com/Article/details/gpigpraty.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.fehbvm.com/Article/details/gcuperllm.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.zdbjq.cn/Article/details/gjnlulvhf.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/gokhabfzh.sHtML

[Q83] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/gdjwucqkq.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gzcdlcbyu.sHtML

[Q84] 去除首尾空格
来源：http://read.share.hesvh.cn/Article/details/gjizjfxfy.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gopxayypo.sHtML

[Q85] 数值取整
来源：http://m.share.hesvh.cn/Article/details/gkqjrfwjf.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.zdbjq.cn/Article/details/gdorzkrhs.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.hesvh.cn/Article/details/gggqvstif.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.hesvh.cn/Article/details/gdyamtpzn.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fehbvm.com/Article/details/gjyfbmosm.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.zdbjq.cn/Article/details/gihfnuzpv.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.zdbjq.cn/Article/details/gxzcmvjqm.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.hesvh.cn/Article/details/growlbber.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fehbvm.com/Article/details/goayaokdp.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fehbvm.com/Article/details/gphuwdqbv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.zdbjq.cn/Article/details/geddljxma.sHtML

[Q90] 生成序号列
来源：http://m.share.fehbvm.com/Article/details/glbexfcem.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.hesvh.cn/Article/details/gjonnesih.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gxorzjpss.sHtML

R. Bash 专题
来源：http://www.m.share.hesvh.cn/Article/details/gwuychrzr.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gfqgvwjzl.sHtML

[R01] shebang 与严格模式
来源：http://baike.fehbvm.com/Article/details/gygfgwfui.sHtML

#!/usr/bin/env bash
来源：http://m.share.zdbjq.cn/Article/details/gvtjjxwic.sHtML

set -euo pipefail
来源：http://m.share.zdbjq.cn/Article/details/gclnxnfwp.sHtML

[R02] 变量赋值与使用
来源：http://3g.zdbjq.cn/Article/details/gcxiwrcso.sHtML

name="Tom"; echo "$name"
来源：http://blog.hesvh.cn/Article/details/gcepjxufk.sHtML

[R03] 只读变量
来源：http://www.blog.fehbvm.com/Article/details/gjtecbhfu.sHtML

readonly PI=3.14
来源：http://baike.fehbvm.com/Article/details/gufclefaw.sHtML

[R04] 位置参数
来源：http://wap.hesvh.cn/Article/details/gknezbfbz.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.zdbjq.cn/Article/details/glimigyrn.sHtML

[R05] 参数默认值
来源：http://baike.fehbvm.com/Article/details/grgmhivbp.sHtML

name="${1:-default}"
来源：http://m.share.zdbjq.cn/Article/details/ggdhsrzjv.sHtML

[R06] 判断命令是否存在
来源：http://mobile.hesvh.cn/Article/details/gwxtpiebq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fehbvm.com/Article/details/gwaknuzcp.sHtML

[R07] if 判断文件
来源：http://baike.zdbjq.cn/Article/details/gcgpxaiep.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fehbvm.com/Article/details/gnrbnujkb.sHtML

[R08] 数值比较
来源：http://wap.hesvh.cn/Article/details/gexmqprex.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.hesvh.cn/Article/details/geqtfniko.sHtML

[R09] 字符串比较
来源：http://3g.zdbjq.cn/Article/details/gqoedsawk.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.zdbjq.cn/Article/details/gzyhoiovs.sHtML

[R10] 正则匹配
来源：http://blog.hesvh.cn/Article/details/ghcsqycni.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fehbvm.com/Article/details/gbypnpioz.sHtML

[R11] case 多分支
来源：http://baike.zdbjq.cn/Article/details/gfavpvpim.sHtML

case "$1" in
来源：http://blog.hesvh.cn/Article/details/gukljzdcc.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gmeaiyvyg.sHtML

stop)  echo "停止" ;;
来源：http://baike.zdbjq.cn/Article/details/gkauajmye.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.zdbjq.cn/Article/details/gngqwmrqi.sHtML

esac
来源：http://read.share.fehbvm.com/Article/details/gigzinshu.sHtML

[R12] for 遍历文件
来源：http://www.share.hesvh.cn/Article/details/gllxxsjio.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fehbvm.com/Article/details/giklggyor.sHtML

[R13] for 计数循环
来源：http://www.m.share.hesvh.cn/Article/details/gzxekhigz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.hesvh.cn/Article/details/gaejwtzjt.sHtML

[R14] C 风格 for
来源：http://www.m.share.fehbvm.com/Article/details/gjipphayi.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/gnpvpgwqe.sHtML

[R15] while 逐行读文件
来源：http://blog.fehbvm.com/Article/details/gprjokcbv.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.zdbjq.cn/Article/details/gbrebazna.sHtML

[R16] until 等待条件
来源：http://mobile.fehbvm.com/Article/details/gcugbswgm.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.hesvh.cn/Article/details/govkpwyaq.sHtML

[R17] 数组定义与取值
来源：http://m.share.hesvh.cn/Article/details/ghjufolux.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fehbvm.com/Article/details/gjahucdhn.sHtML

[R18] 遍历数组
来源：http://m.share.fehbvm.com/Article/details/gnqpsddry.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fehbvm.com/Article/details/gslxwmfoe.sHtML

[R19] 数组长度
来源：http://read.share.zdbjq.cn/Article/details/ghwpxcsnd.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.hesvh.cn/Article/details/gzimfrxag.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.hesvh.cn/Article/details/gvtudevwu.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fehbvm.com/Article/details/guuyndxdr.sHtML

[R21] 字符串长度
来源：http://mobile.fehbvm.com/Article/details/gxebyltum.sHtML

echo "${#s}"
来源：http://read.share.hesvh.cn/Article/details/ggfpvmrmu.sHtML

[R22] 截取子串
来源：http://m.share.zdbjq.cn/Article/details/gzhuhxtnz.sHtML

echo "${s:0:5}"
来源：http://www.share.hesvh.cn/Article/details/grlfiumti.sHtML

[R23] 字符串替换
来源：http://baike.zdbjq.cn/Article/details/grhezmvxk.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.zdbjq.cn/Article/details/gfzyuopnj.sHtML

[R24] 大小写转换
来源：http://www.m.share.fehbvm.com/Article/details/gkyqiyngw.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fehbvm.com/Article/details/gjzxknomf.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.zdbjq.cn/Article/details/gzavxoebe.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.hesvh.cn/Article/details/gyuykvqoa.sHtML

[R26] 命令替换
来源：http://mobile.zdbjq.cn/Article/details/gfbmmiiqk.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fehbvm.com/Article/details/gdvsjagly.sHtML

[R27] 算术展开
来源：http://blog.zdbjq.cn/Article/details/gcbawwios.sHtML

echo $((1 + 2 * 3))
来源：http://wap.zdbjq.cn/Article/details/grqnsubzj.sHtML

[R28] 浮点运算
来源：http://mobile.hesvh.cn/Article/details/gvijbvfrw.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fehbvm.com/Article/details/gzknpthab.sHtML

[R29] 定义函数
来源：http://blog.zdbjq.cn/Article/details/gzozasgnd.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.zdbjq.cn/Article/details/ghglmzdgb.sHtML

[R30] 函数返回状态码
来源：http://baike.hesvh.cn/Article/details/ggheuuebm.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fehbvm.com/Article/details/gpihudkyo.sHtML

[R31] 局部变量
来源：http://www.blog.hesvh.cn/Article/details/ggijfjfzy.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.zdbjq.cn/Article/details/ghdnmjrzd.sHtML

[R32] 参数个数校验
来源：http://read.share.hesvh.cn/Article/details/guqoqchmc.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.zdbjq.cn/Article/details/gfptjsubp.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.hesvh.cn/Article/details/gayqwobsr.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.zdbjq.cn/Article/details/glkydpikc.sHtML

[R34] 退出时清理
来源：http://www.m.share.zdbjq.cn/Article/details/gcuwlfzey.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fehbvm.com/Article/details/gymwnrmow.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fehbvm.com/Article/details/gycibbbvy.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fehbvm.com/Article/details/gsdcxgioa.sHtML

[R36] 并发执行多个任务
来源：http://wap.zdbjq.cn/Article/details/galsmqkrz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fehbvm.com/Article/details/gawfmyxeo.sHtML

[R37] 把输出赋给变量
来源：http://blog.fehbvm.com/Article/details/gvvcnvdjw.sHtML

files=$(ls -1)
来源：http://www.share.zdbjq.cn/Article/details/gbsztfggg.sHtML

[R38] 管道串联
来源：http://3g.hesvh.cn/Article/details/gnjugrwea.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.zdbjq.cn/Article/details/gqbjvwdsn.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.zdbjq.cn/Article/details/gyuqiojrc.sHtML

cmd > out.log 2>&1
来源：http://read.share.hesvh.cn/Article/details/gamgjfsat.sHtML

[R40] 追加写日志
来源：http://www.m.share.zdbjq.cn/Article/details/gdjtvogkl.sHtML

echo "log" >> out.log
来源：http://www.share.zdbjq.cn/Article/details/ghalofzec.sHtML

[R41] 丢弃输出
来源：http://m.share.zdbjq.cn/Article/details/gftxfbjtq.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.hesvh.cn/Article/details/gwqnwijsm.sHtML

[R42] 输入重定向
来源：http://read.share.fehbvm.com/Article/details/gbmjwiccr.sHtML

wc -l < a.txt
来源：http://3g.fehbvm.com/Article/details/gbyopgwun.sHtML

[R43] 按名字查找文件
来源：http://3g.zdbjq.cn/Article/details/glvdypsch.sHtML

find . -name "*.log" -type f
来源：http://baike.fehbvm.com/Article/details/gwxkawtad.sHtML

[R44] 按修改时间查找
来源：http://www.share.zdbjq.cn/Article/details/gnxidjwqh.sHtML

find . -mtime -7 -type f
来源：http://wap.fehbvm.com/Article/details/greflwxny.sHtML

[R45] 批量删除
来源：http://www.share.hesvh.cn/Article/details/gbuuvcpnc.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.zdbjq.cn/Article/details/gpdseilxs.sHtML

[R46] 递归替换文件内容
来源：http://www.share.hesvh.cn/Article/details/gfrxogsdt.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.zdbjq.cn/Article/details/ghbzakqwg.sHtML

[R47] sed 单行替换
来源：http://read.share.zdbjq.cn/Article/details/gxufczjsg.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fehbvm.com/Article/details/gsxqzptqi.sHtML

[R48] awk 取指定列
来源：http://read.share.fehbvm.com/Article/details/gtlozkccx.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gbqccovow.sHtML

[R49] awk 带条件
来源：http://www.m.share.zdbjq.cn/Article/details/gxacsqsab.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.zdbjq.cn/Article/details/gtqvwwwtc.sHtML

[R50] awk 求和
来源：http://www.m.share.hesvh.cn/Article/details/gbnukuswr.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.hesvh.cn/Article/details/ggdnmqvib.sHtML

[R51] 排序去重取前几
来源：http://wap.fehbvm.com/Article/details/gehdtyewp.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.zdbjq.cn/Article/details/gbcjohtsc.sHtML

[R52] 统计行数
来源：http://www.m.share.zdbjq.cn/Article/details/gunkecisj.sHtML

wc -l a.txt
来源：http://baike.zdbjq.cn/Article/details/gegbgyjbb.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fehbvm.com/Article/details/gkfuzvstq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fehbvm.com/Article/details/gknofiohw.sHtML

[R54] 比较两个文件
来源：http://read.share.hesvh.cn/Article/details/gnikhtlej.sHtML

diff a.txt b.txt
来源：http://m.share.hesvh.cn/Article/details/glvecdxrx.sHtML

[R55] 压缩与解压
来源：http://read.share.hesvh.cn/Article/details/gxkybyyfe.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fehbvm.com/Article/details/gghztjwof.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gfxnpkvld.sHtML

scp file user@host:/path/
来源：http://blog.fehbvm.com/Article/details/gaggjztsm.sHtML

[R57] 远程执行命令
来源：http://wap.zdbjq.cn/Article/details/gqumtounl.sHtML

ssh user@host 'uptime'
来源：http://www.blog.zdbjq.cn/Article/details/gttmwaqcs.sHtML

[R58] 下载文件
来源：http://wap.hesvh.cn/Article/details/gfacumzns.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fehbvm.com/Article/details/gmmklpybw.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.hesvh.cn/Article/details/ggqxjydkc.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.zdbjq.cn/Article/details/ghidouzib.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.hesvh.cn/Article/details/gelmfagow.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.zdbjq.cn/Article/details/gabnwomop.sHtML

[R61] 磁盘占用
来源：http://mobile.zdbjq.cn/Article/details/gzwikxfqc.sHtML

df -h;  du -sh *
来源：http://read.share.hesvh.cn/Article/details/gftcekkwb.sHtML

[R62] 找最占空间的文件
来源：http://read.share.zdbjq.cn/Article/details/goexyflka.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.hesvh.cn/Article/details/gnkdvtixq.sHtML

[R63] 内存与进程
来源：http://www.m.share.hesvh.cn/Article/details/gkrvzbnvw.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.hesvh.cn/Article/details/gqvlgkxux.sHtML

[R64] 结束进程
来源：http://blog.zdbjq.cn/Article/details/ggvlzxopo.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fehbvm.com/Article/details/gpiklhymn.sHtML

[R65] 查看端口占用
来源：http://www.blog.hesvh.cn/Article/details/ggvqubmek.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.zdbjq.cn/Article/details/gokwxqqfb.sHtML

[R66] 定时任务
来源：http://www.m.share.fehbvm.com/Article/details/glcfemisr.sHtML

crontab -e;  crontab -l
来源：http://3g.hesvh.cn/Article/details/gdlwjfbtv.sHtML

[R67] 生成随机十六进制串
来源：http://blog.hesvh.cn/Article/details/gpifqkjlr.sHtML

openssl rand -hex 16
来源：http://www.share.zdbjq.cn/Article/details/giratofqa.sHtML

[R68] 计算文件校验值
来源：http://m.share.hesvh.cn/Article/details/gxxbrqocp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fehbvm.com/Article/details/gjqluymwq.sHtML

[R69] 生成随机密码
来源：http://blog.zdbjq.cn/Article/details/grydgtnzp.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fehbvm.com/Article/details/gxinnhawh.sHtML

[R70] 时间戳与互转
来源：http://www.share.fehbvm.com/Article/details/gpxfsyamy.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fehbvm.com/Article/details/gzgvgslwl.sHtML

[R71] 日期格式化
来源：http://m.share.fehbvm.com/Article/details/gttzexhkv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fehbvm.com/Article/details/gyttycvtm.sHtML

[R72] 等待端口就绪
来源：http://wap.hesvh.cn/Article/details/gqjoddzmo.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.hesvh.cn/Article/details/gojvxobrc.sHtML

[R73] 分割大日志
来源：http://read.share.fehbvm.com/Article/details/gelquvdff.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.hesvh.cn/Article/details/gkqfqmrcs.sHtML

[R74] 批量重命名
来源：http://mobile.fehbvm.com/Article/details/gvpgnfazj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.hesvh.cn/Article/details/gbfxvhxpp.sHtML

[R75] 导出环境变量
来源：http://wap.zdbjq.cn/Article/details/gsqvejziq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fehbvm.com/Article/details/gyrejlgzx.sHtML

[R76] 使用临时文件
来源：http://www.m.share.hesvh.cn/Article/details/gwuagiqsu.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fehbvm.com/Article/details/gzomcipvj.sHtML

[R77] 读取用户输入
来源：http://www.blog.fehbvm.com/Article/details/ggcuoqdlf.sHtML

read -rp "请输入: " ans
来源：http://blog.fehbvm.com/Article/details/gfschbcsu.sHtML

[R78] 交互式菜单
来源：http://m.share.fehbvm.com/Article/details/gppcpvhoa.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.hesvh.cn/Article/details/ggptauvic.sHtML

[R79] 解析命令行选项
来源：http://blog.zdbjq.cn/Article/details/gyqmqmaia.sHtML


<!-- 参考信息 -->