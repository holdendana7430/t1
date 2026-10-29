代发 wailian999

[Q33] 多列分组
来源：http://blog.hesvh.cn/Article/details/gyzozjpgj.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.zdbjq.cn/Article/details/guxvmetad.sHtML

[Q34] 每组取第一条
来源：http://read.share.fehbvm.com/Article/details/ghuduebty.sHtML

SELECT * FROM (
来源：http://3g.hesvh.cn/Article/details/gcfccxnag.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.hesvh.cn/Article/details/gvunkmicg.sHtML

) t WHERE rn = 1;
来源：http://3g.fehbvm.com/Article/details/gqnnkynba.sHtML

[Q35] 内连接
来源：http://www.m.share.fehbvm.com/Article/details/gdvdevmma.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.hesvh.cn/Article/details/gmzazpsrs.sHtML

[Q36] 左连接
来源：http://read.share.hesvh.cn/Article/details/gudargswg.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fehbvm.com/Article/details/gzefxmyxj.sHtML

[Q37] 右连接
来源：http://3g.hesvh.cn/Article/details/ghzpgtdot.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fehbvm.com/Article/details/gbxeqhhvw.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.zdbjq.cn/Article/details/gtpgucxbc.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.fehbvm.com/Article/details/giyawmyys.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.hesvh.cn/Article/details/ggqpfawpo.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.fehbvm.com/Article/details/ganuwofkq.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.fehbvm.com/Article/details/gifldhhcp.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.hesvh.cn/Article/details/gwxbsimnm.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.fehbvm.com/Article/details/gphzrpqjv.sHtML

[Q41] 多表连接
来源：http://blog.zdbjq.cn/Article/details/gvywiyrof.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.zdbjq.cn/Article/details/glghqorgl.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.hesvh.cn/Article/details/gaszxgxvg.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.fehbvm.com/Article/details/goztswwzi.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.zdbjq.cn/Article/details/gwknxlqai.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.zdbjq.cn/Article/details/gifvzbbbq.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.fehbvm.com/Article/details/gxlhcdpxu.sHtML

[Q43] 标量子查询
来源：http://read.share.hesvh.cn/Article/details/gvuvqukfu.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.hesvh.cn/Article/details/gdlkvwqpg.sHtML

[Q44] IN 子查询
来源：http://www.blog.hesvh.cn/Article/details/gvlgaqddk.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.hesvh.cn/Article/details/gbapcygpa.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.hesvh.cn/Article/details/gpvgsjyys.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.hesvh.cn/Article/details/gmndzndvg.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.hesvh.cn/Article/details/gvtnauugc.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fehbvm.com/Article/details/gsiqcfcrm.sHtML

[Q47] 与平均值比较
来源：http://baike.hesvh.cn/Article/details/gtcqqrnqf.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.hesvh.cn/Article/details/gikijxqmt.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.hesvh.cn/Article/details/gkbgpjsbv.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.hesvh.cn/Article/details/gpoifybyr.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.fehbvm.com/Article/details/ghxpgdxez.sHtML

[Q49] 更新单行
来源：http://www.share.zdbjq.cn/Article/details/ggsbimkoq.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.hesvh.cn/Article/details/gwhvhaemd.sHtML

[Q50] 批量更新
来源：http://3g.fehbvm.com/Article/details/gypcqxamo.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.zdbjq.cn/Article/details/glhwbraqx.sHtML

[Q51] 用子查询更新
来源：http://m.share.hesvh.cn/Article/details/gllyzutqq.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.hesvh.cn/Article/details/gohaqobwj.sHtML

[Q52] 删除指定行
来源：http://www.share.hesvh.cn/Article/details/getymhhje.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.hesvh.cn/Article/details/ghnlxakhq.sHtML

[Q53] 按条件删除
来源：http://www.m.share.zdbjq.cn/Article/details/gjgygixeg.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fehbvm.com/Article/details/gkctwsssq.sHtML

[Q54] 清空表
来源：http://blog.fehbvm.com/Article/details/gnswplyas.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.fehbvm.com/Article/details/gpjnvvtmt.sHtML

[Q55] 排名（并列占位）
来源：http://baike.fehbvm.com/Article/details/gyxcwfyxd.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.zdbjq.cn/Article/details/gtviamxmk.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.fehbvm.com/Article/details/geaeruprv.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.fehbvm.com/Article/details/gytbrjisj.sHtML

[Q57] 行号
来源：http://read.share.zdbjq.cn/Article/details/gsjnewlmu.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.fehbvm.com/Article/details/gcoushqzh.sHtML

[Q58] 累计求和
来源：http://blog.fehbvm.com/Article/details/gifxpxwfw.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gbtxtpwpn.sHtML

[Q59] 分组内累计
来源：http://read.share.hesvh.cn/Article/details/gatszelad.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gyoxeygbu.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.zdbjq.cn/Article/details/gzjwhuwxu.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.zdbjq.cn/Article/details/gqlttmqwo.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.hesvh.cn/Article/details/gwqskqyra.sHtML

[Q61] 移动平均
来源：http://wap.hesvh.cn/Article/details/gewgsukaz.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gmuuzldjn.sHtML

[Q62] 分组占比
来源：http://www.share.fehbvm.com/Article/details/gntbzgnxz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gcslielrg.sHtML

[Q63] 开启事务
来源：http://mobile.hesvh.cn/Article/details/gzbpbmdjo.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fehbvm.com/Article/details/grqwkrvnx.sHtML

[Q64] 提交事务
来源：http://m.share.hesvh.cn/Article/details/glombeesg.sHtML

COMMIT;
来源：http://m.share.fehbvm.com/Article/details/gkhiqdnez.sHtML

[Q65] 回滚事务
来源：http://m.share.hesvh.cn/Article/details/gqzgfuhwf.sHtML

ROLLBACK;
来源：http://www.m.share.hesvh.cn/Article/details/gokseykyu.sHtML

[Q66] 行锁查询
来源：http://www.blog.hesvh.cn/Article/details/gxvjxbwkf.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.fehbvm.com/Article/details/ggqkleflo.sHtML

[Q67] 设置隔离级别
来源：http://read.share.hesvh.cn/Article/details/gsblbmato.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.fehbvm.com/Article/details/ggcidhsqd.sHtML

[Q68] 保存点
来源：http://mobile.fehbvm.com/Article/details/gqwqjjuez.sHtML

SAVEPOINT sp1;
来源：http://m.share.hesvh.cn/Article/details/geqyqbplh.sHtML

ROLLBACK TO sp1;
来源：http://mobile.hesvh.cn/Article/details/gtnabnvbh.sHtML

[Q69] 查看执行计划
来源：http://wap.fehbvm.com/Article/details/gqwzlnlrn.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fehbvm.com/Article/details/gpidhvatc.sHtML

[Q70] 更新统计信息
来源：http://www.blog.hesvh.cn/Article/details/gduhnzjkw.sHtML

ANALYZE TABLE users;
来源：http://m.share.zdbjq.cn/Article/details/gzgwrjkcu.sHtML

[Q71] 查看建表语句
来源：http://m.share.hesvh.cn/Article/details/gipkcbaxj.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.zdbjq.cn/Article/details/gydpmrbyw.sHtML

[Q72] 查看索引
来源：http://www.m.share.fehbvm.com/Article/details/gzpkbrlxv.sHtML

SHOW INDEX FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gqlmoekrs.sHtML

[Q73] 查看表状态
来源：http://baike.fehbvm.com/Article/details/gjcofehht.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.zdbjq.cn/Article/details/gqxnbtuoq.sHtML

[Q74] 强制使用索引
来源：http://baike.hesvh.cn/Article/details/gatdfphko.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.zdbjq.cn/Article/details/glbczkqpf.sHtML

[Q75] 日期格式化
来源：http://www.share.hesvh.cn/Article/details/gvyhkmecs.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fehbvm.com/Article/details/goccivebs.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fehbvm.com/Article/details/gdgnlwgfk.sHtML

[Q76] 按天统计
来源：http://baike.zdbjq.cn/Article/details/gjegymokc.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.fehbvm.com/Article/details/gokzfjzsh.sHtML

[Q77] 时间加减
来源：http://read.share.zdbjq.cn/Article/details/gobkgreup.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.zdbjq.cn/Article/details/gwnuyujju.sHtML

[Q78] 当前时间
来源：http://wap.fehbvm.com/Article/details/ganejjnke.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.hesvh.cn/Article/details/gpkxemuxy.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fehbvm.com/Article/details/gidddnhvt.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.zdbjq.cn/Article/details/giwbzxqwt.sHtML

[Q80] 字符串截取
来源：http://read.share.hesvh.cn/Article/details/gxanptrsx.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gzpoaqnel.sHtML

[Q81] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/gtwytoplc.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.fehbvm.com/Article/details/gkfmjment.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.hesvh.cn/Article/details/gukcnvgsi.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gqifkjcml.sHtML

[Q83] 大小写转换
来源：http://3g.hesvh.cn/Article/details/gknjumppp.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/grmiiesif.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.hesvh.cn/Article/details/gyzzcudyk.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gmfwcurim.sHtML

[Q85] 数值取整
来源：http://read.share.zdbjq.cn/Article/details/gquiiuole.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.zdbjq.cn/Article/details/gkgkmsgjh.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.fehbvm.com/Article/details/gigbpcdcr.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fehbvm.com/Article/details/ghlmkolpp.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.zdbjq.cn/Article/details/gihkwqdqb.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.zdbjq.cn/Article/details/gvqaooczn.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.zdbjq.cn/Article/details/gtvlnuhja.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fehbvm.com/Article/details/gqwqcqlww.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fehbvm.com/Article/details/gbftbmhoz.sHtML

[Q89] 判断表是否存在
来源：http://read.share.zdbjq.cn/Article/details/gyogspnoz.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.hesvh.cn/Article/details/gflntdkxv.sHtML

[Q90] 生成序号列
来源：http://baike.fehbvm.com/Article/details/gqhsrippq.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.hesvh.cn/Article/details/gnwvhagqm.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/getzjvptp.sHtML

R. Bash 专题
来源：http://wap.fehbvm.com/Article/details/gfbyddkvp.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/glpoxhkmm.sHtML

[R01] shebang 与严格模式
来源：http://3g.hesvh.cn/Article/details/gpwuwrywx.sHtML

#!/usr/bin/env bash
来源：http://m.share.hesvh.cn/Article/details/glvklgiyh.sHtML

set -euo pipefail
来源：http://m.share.zdbjq.cn/Article/details/gyuxttcvg.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.zdbjq.cn/Article/details/gyapogieb.sHtML

name="Tom"; echo "$name"
来源：http://wap.zdbjq.cn/Article/details/gedtalcjy.sHtML

[R03] 只读变量
来源：http://blog.zdbjq.cn/Article/details/geeirscdk.sHtML

readonly PI=3.14
来源：http://blog.fehbvm.com/Article/details/gdeqqgyof.sHtML

[R04] 位置参数
来源：http://www.share.fehbvm.com/Article/details/ghqvgmjky.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fehbvm.com/Article/details/gjyhvxwvb.sHtML

[R05] 参数默认值
来源：http://www.m.share.hesvh.cn/Article/details/gfkycbxjp.sHtML

name="${1:-default}"
来源：http://baike.hesvh.cn/Article/details/gyipsvxcm.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fehbvm.com/Article/details/ggwhvqybo.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fehbvm.com/Article/details/givhzzvma.sHtML

[R07] if 判断文件
来源：http://read.share.hesvh.cn/Article/details/gjfvlbspa.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.hesvh.cn/Article/details/goeneukxd.sHtML

[R08] 数值比较
来源：http://read.share.fehbvm.com/Article/details/glrwoxtot.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fehbvm.com/Article/details/gfpzqncru.sHtML

[R09] 字符串比较
来源：http://www.blog.hesvh.cn/Article/details/gkgmdmrip.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.hesvh.cn/Article/details/gkiqlhvtr.sHtML

[R10] 正则匹配
来源：http://baike.hesvh.cn/Article/details/grtigqydr.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fehbvm.com/Article/details/gfnkgbvlp.sHtML

[R11] case 多分支
来源：http://www.m.share.zdbjq.cn/Article/details/gpcygplwp.sHtML

case "$1" in
来源：http://baike.hesvh.cn/Article/details/ghopzqwsc.sHtML

start) echo "启动" ;;
来源：http://baike.fehbvm.com/Article/details/gdyzlwoab.sHtML

stop)  echo "停止" ;;
来源：http://3g.hesvh.cn/Article/details/gbczrwwwl.sHtML

*)     echo "未知命令" ;;
来源：http://3g.fehbvm.com/Article/details/gdhcgkbiu.sHtML

esac
来源：http://mobile.zdbjq.cn/Article/details/gbucebofk.sHtML

[R12] for 遍历文件
来源：http://www.m.share.hesvh.cn/Article/details/gbbeqagna.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.zdbjq.cn/Article/details/geadcavku.sHtML

[R13] for 计数循环
来源：http://mobile.hesvh.cn/Article/details/gbesmdppc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.zdbjq.cn/Article/details/gordcdrcc.sHtML

[R14] C 风格 for
来源：http://baike.fehbvm.com/Article/details/gbtdumaki.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fehbvm.com/Article/details/ghlaeauub.sHtML

[R15] while 逐行读文件
来源：http://3g.fehbvm.com/Article/details/gxhnlpfba.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.zdbjq.cn/Article/details/guxarrsdt.sHtML

[R16] until 等待条件
来源：http://blog.fehbvm.com/Article/details/gzrylwkwa.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.hesvh.cn/Article/details/gmbimiccp.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fehbvm.com/Article/details/gssegzbod.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.zdbjq.cn/Article/details/gtaaeilhm.sHtML

[R18] 遍历数组
来源：http://mobile.fehbvm.com/Article/details/gniflhgzd.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.hesvh.cn/Article/details/gfcklkzmq.sHtML

[R19] 数组长度
来源：http://mobile.hesvh.cn/Article/details/gqxrldgyq.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.hesvh.cn/Article/details/ghwkgpyxi.sHtML

[R20] 关联数组（字典）
来源：http://mobile.hesvh.cn/Article/details/gxqvrwevv.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fehbvm.com/Article/details/gbvrsqnnv.sHtML

[R21] 字符串长度
来源：http://read.share.zdbjq.cn/Article/details/gnawczpnd.sHtML

echo "${#s}"
来源：http://wap.hesvh.cn/Article/details/gkxhqwxvt.sHtML

[R22] 截取子串
来源：http://baike.zdbjq.cn/Article/details/gystbojxk.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fehbvm.com/Article/details/glrdoisqn.sHtML

[R23] 字符串替换
来源：http://baike.fehbvm.com/Article/details/gyefpzdja.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.zdbjq.cn/Article/details/gfabzrvyn.sHtML

[R24] 大小写转换
来源：http://wap.hesvh.cn/Article/details/gxpyvuemk.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.zdbjq.cn/Article/details/gysgpizar.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fehbvm.com/Article/details/gmcbzomqp.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.zdbjq.cn/Article/details/guvvulblf.sHtML

[R26] 命令替换
来源：http://m.share.zdbjq.cn/Article/details/gbdttxvvf.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fehbvm.com/Article/details/gcahayqzf.sHtML

[R27] 算术展开
来源：http://blog.hesvh.cn/Article/details/guwwhadgw.sHtML

echo $((1 + 2 * 3))
来源：http://baike.zdbjq.cn/Article/details/gzeykipzb.sHtML

[R28] 浮点运算
来源：http://www.blog.zdbjq.cn/Article/details/gwkmhuwtq.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fehbvm.com/Article/details/gqhatxvrl.sHtML

[R29] 定义函数
来源：http://blog.fehbvm.com/Article/details/gsldipucq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.zdbjq.cn/Article/details/gztrbnxvn.sHtML

[R30] 函数返回状态码
来源：http://www.blog.hesvh.cn/Article/details/gvndgqlkp.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fehbvm.com/Article/details/giahbmfvk.sHtML

[R31] 局部变量
来源：http://3g.zdbjq.cn/Article/details/gmblzfdwq.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fehbvm.com/Article/details/gwbivmlki.sHtML

[R32] 参数个数校验
来源：http://www.m.share.hesvh.cn/Article/details/gmrvtukpp.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.zdbjq.cn/Article/details/gkuseqcll.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.hesvh.cn/Article/details/glcjprpfm.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.hesvh.cn/Article/details/gtyhtssvk.sHtML

[R34] 退出时清理
来源：http://mobile.hesvh.cn/Article/details/gfklsnbgz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fehbvm.com/Article/details/gmyseredf.sHtML

[R35] 后台执行并等待
来源：http://wap.zdbjq.cn/Article/details/gptszezse.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.hesvh.cn/Article/details/gjilvmivq.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fehbvm.com/Article/details/gtjrqecwo.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.zdbjq.cn/Article/details/ggdyovsbs.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fehbvm.com/Article/details/govjndjdr.sHtML

files=$(ls -1)
来源：http://mobile.hesvh.cn/Article/details/gjygsenub.sHtML

[R38] 管道串联
来源：http://www.share.fehbvm.com/Article/details/gjptwnexj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fehbvm.com/Article/details/gwssgkcrh.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.hesvh.cn/Article/details/grcveqfum.sHtML

cmd > out.log 2>&1
来源：http://3g.fehbvm.com/Article/details/gqitzeqys.sHtML

[R40] 追加写日志
来源：http://baike.fehbvm.com/Article/details/gzgsxnvll.sHtML

echo "log" >> out.log
来源：http://3g.zdbjq.cn/Article/details/ggtpsslwo.sHtML

[R41] 丢弃输出
来源：http://3g.zdbjq.cn/Article/details/gcjcllbxp.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.zdbjq.cn/Article/details/gmpwdvdai.sHtML

[R42] 输入重定向
来源：http://m.share.zdbjq.cn/Article/details/gtkgrbtxv.sHtML

wc -l < a.txt
来源：http://baike.hesvh.cn/Article/details/gdhbfpxac.sHtML

[R43] 按名字查找文件
来源：http://wap.fehbvm.com/Article/details/gzkocqkkp.sHtML

find . -name "*.log" -type f
来源：http://3g.fehbvm.com/Article/details/gzuhcgicn.sHtML

[R44] 按修改时间查找
来源：http://baike.hesvh.cn/Article/details/giyopogav.sHtML

find . -mtime -7 -type f
来源：http://3g.hesvh.cn/Article/details/gbkeppxbs.sHtML

[R45] 批量删除
来源：http://www.blog.zdbjq.cn/Article/details/gvbrsyvfu.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.zdbjq.cn/Article/details/gztbpnexc.sHtML

[R46] 递归替换文件内容
来源：http://mobile.zdbjq.cn/Article/details/gsvmqyfnv.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.hesvh.cn/Article/details/gvkykswnu.sHtML

[R47] sed 单行替换
来源：http://www.blog.hesvh.cn/Article/details/gafwuksyi.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.hesvh.cn/Article/details/gxfkxqaxj.sHtML

[R48] awk 取指定列
来源：http://blog.hesvh.cn/Article/details/gluzksqnw.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fehbvm.com/Article/details/gzgdtlzlt.sHtML

[R49] awk 带条件
来源：http://wap.hesvh.cn/Article/details/gegsulbwq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fehbvm.com/Article/details/ggtqzmofn.sHtML

[R50] awk 求和
来源：http://www.m.share.zdbjq.cn/Article/details/gbjvovmjd.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.hesvh.cn/Article/details/gwhjsypyb.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fehbvm.com/Article/details/gyeaviuyo.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.hesvh.cn/Article/details/gjaplvech.sHtML

[R52] 统计行数
来源：http://www.m.share.fehbvm.com/Article/details/gyqcstyrt.sHtML

wc -l a.txt
来源：http://baike.fehbvm.com/Article/details/gqxplhpzc.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.hesvh.cn/Article/details/gykpifjge.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.hesvh.cn/Article/details/gvecwnsnf.sHtML

[R54] 比较两个文件
来源：http://blog.zdbjq.cn/Article/details/gttpyqqzw.sHtML

diff a.txt b.txt
来源：http://baike.hesvh.cn/Article/details/gdcwxbjhx.sHtML

[R55] 压缩与解压
来源：http://www.blog.zdbjq.cn/Article/details/grkspjuin.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.zdbjq.cn/Article/details/gmqwwtigf.sHtML

[R56] 远程拷贝
来源：http://wap.fehbvm.com/Article/details/gcusswbfk.sHtML

scp file user@host:/path/
来源：http://wap.zdbjq.cn/Article/details/gxmrllrwi.sHtML

[R57] 远程执行命令
来源：http://www.m.share.hesvh.cn/Article/details/gtkbewhgp.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.zdbjq.cn/Article/details/gotpesepo.sHtML

[R58] 下载文件
来源：http://3g.fehbvm.com/Article/details/giweqmxfk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.hesvh.cn/Article/details/ghcfyrryy.sHtML

[R59] 发 POST JSON
来源：http://www.blog.zdbjq.cn/Article/details/gyytzcemm.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.zdbjq.cn/Article/details/gbyajuvju.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.hesvh.cn/Article/details/gmdrbbwpx.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.zdbjq.cn/Article/details/giqpnxxzv.sHtML

[R61] 磁盘占用
来源：http://www.m.share.hesvh.cn/Article/details/gvokwepvg.sHtML

df -h;  du -sh *
来源：http://blog.hesvh.cn/Article/details/gpeidnvsu.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fehbvm.com/Article/details/gsvopthnq.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.hesvh.cn/Article/details/gjgdqlgum.sHtML

[R63] 内存与进程
来源：http://www.share.zdbjq.cn/Article/details/gimtodgzt.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.hesvh.cn/Article/details/gqurtkozl.sHtML

[R64] 结束进程
来源：http://wap.fehbvm.com/Article/details/glrurpzvl.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.zdbjq.cn/Article/details/gpqqfrexr.sHtML

[R65] 查看端口占用
来源：http://3g.hesvh.cn/Article/details/gicotqhcb.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fehbvm.com/Article/details/gficdibwv.sHtML

[R66] 定时任务
来源：http://wap.zdbjq.cn/Article/details/gdrhlqaxr.sHtML

crontab -e;  crontab -l
来源：http://m.share.hesvh.cn/Article/details/gbhxwwaze.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.hesvh.cn/Article/details/gsnbxwyim.sHtML

openssl rand -hex 16
来源：http://www.blog.fehbvm.com/Article/details/glfhwugfs.sHtML

[R68] 计算文件校验值
来源：http://wap.hesvh.cn/Article/details/gmumwlrnu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gaealnfoa.sHtML

[R69] 生成随机密码
来源：http://mobile.zdbjq.cn/Article/details/guiicjmhe.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.zdbjq.cn/Article/details/gjlorgldh.sHtML

[R70] 时间戳与互转
来源：http://blog.zdbjq.cn/Article/details/gonsonkya.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.zdbjq.cn/Article/details/gvazwtfbt.sHtML

[R71] 日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gqpyzwcqh.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.zdbjq.cn/Article/details/gfpybduin.sHtML

[R72] 等待端口就绪
来源：http://3g.fehbvm.com/Article/details/gttkxkcwr.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fehbvm.com/Article/details/ggkkcwmsw.sHtML

[R73] 分割大日志
来源：http://m.share.fehbvm.com/Article/details/grxnoltgz.sHtML

split -l 1000 big.log part_
来源：http://3g.fehbvm.com/Article/details/ggaqifhnw.sHtML

[R74] 批量重命名
来源：http://blog.zdbjq.cn/Article/details/glgaekoik.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.zdbjq.cn/Article/details/gowtzilyz.sHtML

[R75] 导出环境变量
来源：http://mobile.fehbvm.com/Article/details/gsniavdie.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.hesvh.cn/Article/details/gethkhzlk.sHtML

[R76] 使用临时文件
来源：http://www.share.hesvh.cn/Article/details/gbrzcuafj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.zdbjq.cn/Article/details/gitclthmd.sHtML

[R77] 读取用户输入
来源：http://read.share.zdbjq.cn/Article/details/gmsofvfxf.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fehbvm.com/Article/details/gvlmgvobh.sHtML

[R78] 交互式菜单
来源：http://read.share.hesvh.cn/Article/details/gvipavihe.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.zdbjq.cn/Article/details/gpkgsxydw.sHtML

[R79] 解析命令行选项
来源：http://www.share.fehbvm.com/Article/details/gvrwcwehw.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.hesvh.cn/Article/details/ghvoozaaf.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fehbvm.com/Article/details/ggopojzyf.sHtML

time ./run.sh
来源：http://www.m.share.fehbvm.com/Article/details/gnftdgedh.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gcyugwdjz.sHtML

S. C / C++ 专题
来源：http://www.share.hesvh.cn/Article/details/gvbywkhjq.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gmretcojn.sHtML

[S01] C：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gszatnbtq.sHtML

#include <stdio.h>
来源：http://www.m.share.hesvh.cn/Article/details/gvpighkib.sHtML


<!-- 参考信息 -->