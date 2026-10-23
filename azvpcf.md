代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3yzaksqiu.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3jzqarhko.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3ifdlwrul.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3dhczilpp.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3omjnrwuj.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3fabtukem.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3yvuluhjq.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3kmijjbxq.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3hblyqefj.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3yxyhlnek.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kuhzgjyu.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3nejwejey.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3ditzrawz.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3twlfkabs.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3txypwmos.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3dsldqusb.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hopeumfo.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3aqtgsrnb.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3yquocxoh.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3jyopispk.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3oxjozxyz.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3eytnqvkh.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3ajyhcqcu.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3qwmmaspz.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3amwijazr.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3buyinqih.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3jeeaveko.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3iucweiyk.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3lulotrjd.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3xqejeyrn.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3njvoxsem.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3kkpisvfm.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3pzhccjhd.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ythlrzfb.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3pyqiogci.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3afcxehuj.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3zjeyfznl.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3hkzkyzut.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3wwyadpjg.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3guyggmnh.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3mqocqaqd.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3jbaentno.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3yjlbbynd.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3ebklkxim.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3fxkqjzgj.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3xxxvkydn.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3tzagtser.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3vtspmgas.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3gnwmzzul.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3jlnjlmrj.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3pgkbjeit.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3ugxhhotx.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3udckgotu.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3eamkfdzo.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3tguydepb.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3xtqtzbza.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3gbklqbco.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3bpnqnbrq.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3sugxgzar.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3rxanokzi.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3jhrgktfa.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3otvscdcr.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3aesiysvt.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3pxtmbyxg.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3iutlzoas.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3dpkjxjkp.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3qcvumvrq.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3qxfthtis.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3bqconlvy.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3wgoeifdy.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3ocqiddob.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3mqganjwc.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3wrxqicwv.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3onjreuja.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3lcuopokh.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3yskaankt.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3efzxsvcn.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3ewuayihf.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3inrygybj.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3ffikjfym.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3hbovrioy.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3dgyxbxgs.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3qojwkupb.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3thabrtsa.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ofjnldgj.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3griowrkm.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3roicacao.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3cnnpovlk.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3zuksunfz.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3yyyfzxjj.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3fvrmrebc.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3exoubafm.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3gdrneemp.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3trcygdcp.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3nybxqomp.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3pnbxrkdd.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3osjxluas.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3cfzpuxcd.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3yqpxuvim.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3twdhcdvk.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3jkqbziij.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3ciasixxp.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3attojdwi.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3ygvksczz.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3bzdgxbzz.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3gjucsnry.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3yxbaqjrg.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3oheondfm.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3wtlsitvk.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3tqeaffnz.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3betukbph.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3supmyuyn.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3xcvlpykw.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3vshevkar.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3iefqewkk.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3nnditnze.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zuizwdlc.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3zbjlsgpu.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3iooejoyy.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3enuiaufw.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3edwgajgl.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3leqfodke.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3kcpilfmo.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3pgiutizx.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3pdqukkwk.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3taxchhxr.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3qgsfntmg.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3apbhdgnh.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3bisrlmpp.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3aospfyqb.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3azjojvqt.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3omfjxnsk.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3gvfdszux.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vnassygn.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3qzctugvr.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wkgqaciw.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3mqvkmuyj.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wijbvvno.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3zgdhaned.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xpqpuywy.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3yjzxivzs.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3prvpfdee.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3cwpbjndl.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3pmdzilyt.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3ufvxquiv.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3otvukmdr.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3jdckmesg.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3ygaswbxo.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3vjcecznu.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3afktuiia.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bmpzexzc.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3kvgojkyr.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3rpjjwrub.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3noopbhqi.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3qgthayhg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3frimatas.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3fjcxjfbf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fhwtyyhq.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3foifksfe.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3vvoljrhq.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3atngqrog.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3dcpewkgi.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3wjghqacq.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3yfoydtzs.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3alzusctw.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3whqsjzto.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3vhrklfpq.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3zcmcoxro.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3efhdoykn.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3zadlhzzq.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3pztuypja.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3mmjpcqbm.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3biwtmshv.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3qvqkygzo.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3knjykwrm.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3xhxagiuu.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3xxlwcxuy.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3fovztdad.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3ctjigmog.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3xmvujukd.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3pajcizef.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3twzexmrf.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3tpsxsqvh.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3dodavjna.html

esac
来源：http://www.52xcode.cn/Article/details/gt3dpjlocnp.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3zvpwmjqo.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3fsgqzukx.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3cjzfupqx.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3pqbnfcul.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3ueqchhbb.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3uprrdplo.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3yaundnjy.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3davlhdbg.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3dfnvnvkq.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3vuzuwazg.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3yzdxrjot.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3vpglzrca.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3hjlcoflb.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3zsnbtccg.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3aiuzyhxd.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3xuzzspbq.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3dcnlhgce.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3bqgbvywo.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3fecrcarr.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3fvhicmzd.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3kedvodxv.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3odrqigrd.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3xkkvyief.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3nnpprgch.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ueilwqtv.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3gynqokuq.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3lmmrpokt.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3lckbmhdq.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3zzklepoi.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3rswtqieb.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3ssbavjha.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3odedzlgs.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3lhnrxpiz.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3dkvzebld.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3zowslgmn.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3klccxaas.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3zrhjfszu.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3hvvjiklc.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3teaosbhk.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3bklmhpra.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3caeprikf.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3abansrby.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3wgeqzzgf.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3dorzbkzg.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3nuwzrqdi.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3lykacfqf.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3vdqpzjib.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3syjjijld.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3tzdhjqdx.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3sqjchqvy.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3kfmsqofh.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3elulxjdw.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3fxsddtqi.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3ssmeykqs.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3gafatngn.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3dsjyavgi.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3ewcuqbch.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3wyszqhcb.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3lwxphzha.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3geviekkm.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3czsuqmhx.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3wgitzaqr.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3irtbtxca.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3zgeknwdl.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3cmnkxanw.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3jcsaytyq.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3zvqhuuge.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3jtctimvh.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3sesykott.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3vdipwwna.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3nhjlbmum.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fgrxwdpk.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3dqlykvvy.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3wrhyrqvr.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3zaaowpct.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3ufnfyvvl.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3pguopwov.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3phvtvyzf.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3legqrxpl.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3xvwugjwn.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3bdcuuvkn.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3uxefmdoq.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3auzmchua.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3sreidhrq.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3twawwidx.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mzktdxme.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3zywvdfgc.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3qjzozvaq.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3skfabdin.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3pajbldqs.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3rldumuyx.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3gkjnasok.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3mhvyjtcm.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3ohonctju.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3yrouzbcs.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3cvlaesri.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3xtvkgidr.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3ocahoeso.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3hczkppvx.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3plhpsbak.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3pyyvgxyv.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3arpmuwmi.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3yyitvucb.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3fsittnqc.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3pgletigx.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3qszkvuai.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3btkalcfu.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3iiiqoudl.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3pqhghtla.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3xuxoymwo.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3gmdpadri.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3qvqasnfn.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3lwfmhhds.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3tltnofpl.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3nbmtwekn.html


<!-- 参考信息 -->