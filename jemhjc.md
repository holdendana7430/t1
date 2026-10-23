代发 wailian999

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3mzwlfrxa.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3ddyuurfv.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3vibotwez.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3gfhtcamj.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3pozdsnzi.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3mbhazttl.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3glqjriyr.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3hjxtpyic.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3evxtoxkc.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3irdyqboc.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3iowbtiua.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3cfdclgpj.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3vcgzdtcu.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3pmpjykpn.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3dbeooouz.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3rjreyybx.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3gwzvaiym.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3tlmvziwz.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3dlghrjfx.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3saofzzfb.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3jrvjkqfl.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3flbcqeus.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3euedqqdt.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3yuaoatqa.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3ssexqmjd.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3zekudmnn.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3slqkotlg.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3oaqzmurm.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3lndsiesc.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3zczibube.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fhxlkqra.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3vxrjmcpp.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qkjokxhu.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3cygkgnur.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3vkldghyq.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3utuxgxvr.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3henkkgef.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3mnyanhie.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3zgniksub.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3iywleola.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3akifyryi.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3jqlttteu.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3yblwtbdb.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3wpombydl.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3ziszcrta.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3urayvssw.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3tkjdhokt.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3egtsjadt.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3cvnimpyk.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3tmsgkihp.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3cgvawsfu.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3eomocbqy.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3ftdtoqid.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3yexyloof.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3imujovwm.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3vmjcrmqb.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3ewowbxok.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3qrmmzkok.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3ivbffndo.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3xbcbqjsl.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3rkexrtzt.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3mzianboq.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3bvyfiaye.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3qqburbay.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3isgksncz.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3ngzyqpks.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3fkjuwrgo.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3wwuljbnr.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3fphbmyvw.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3ljwmbycj.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3izntzbgi.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3duzpzkld.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3zelzemza.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3sfweajwm.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3qnjjkqpr.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3qhvlkcmf.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3ermvtwcn.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3yukjqajz.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3pdxorlmg.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3zbgarnam.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3jwcxwzer.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3sxfrkrvj.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3mvmxzthm.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3ghqvwdtm.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3spihnykf.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3jqnhqdip.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3sdgazsnz.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3qtcmcuix.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3ynrempfj.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3casicuur.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3bqzvwcox.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3ggqaodjp.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3fekpnwqb.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3ieczyuac.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3iihgmxvw.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3ozmzwxpl.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3fgbaicxr.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3ugwyffwu.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3jmhzjqrx.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3ofxdccei.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dzfgdfcc.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3jgfojlcc.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3cgdjcdnb.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3npwufyxr.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3cemazsaw.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3btuwhrsz.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3ytlpqqig.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3mxnzschz.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3shynzegj.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3mbwrsxye.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3vytbzzys.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3aivrsiyp.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3yhrlpdwu.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3dpkefxje.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3xjmmsulv.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3lujjvnhz.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3vyhtdlpt.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3awidyqqy.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3qvujarjv.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3lczstwfx.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3ryozjvjg.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3ffbssxdk.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3nwhcoyce.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3liutykes.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3xusqztoj.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3eyjjvduu.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3fwuktjnc.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3ujpdctny.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3vjtfxyqj.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3krntudmp.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3ubvnxvxy.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3dhapovcl.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3faxpeaxa.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3yeewleiv.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3evgyrtll.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3jgfxtkoq.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3cuysyhui.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3yroxayhe.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wtvsuonm.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3umtginvr.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3whznpxet.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3jvnuvula.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3wmvgrtyx.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3gvgadwei.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3aesfskqt.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3etxiphbo.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3olnqolfb.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3gvfgwtpi.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3zgvhtkkl.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yrvygmho.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3fbjvwqvh.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ttobvtfk.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3thzsxwlo.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ydgigoby.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3gtnvskag.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3acuckqdm.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3tgoalzlt.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hmnojrpg.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3qpnvooyq.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3dshcwdxj.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3aoqbteqm.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3ykijjuqj.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3dyufmdjg.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3wjmkdmzh.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3nwwpovib.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3mfnheuee.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mgnxqfhx.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3rbqkgnns.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3lqyidohn.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3hngsmndx.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3hgugebsl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jsbnfuzz.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3vxquwrrq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uabqlrtk.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3gfvmbskg.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3vujwuror.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3ziksmeer.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3ozisycme.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3nxowxgas.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3rzjqovlp.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3cbdhsail.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3cajyxrzx.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3cwgsedtr.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3oiafyoft.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3orysphot.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3jzfzmezb.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3vgurdebe.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3ovuopnlj.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3kdpwqyuv.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3btegsxtc.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3mqsdtsyg.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3itpqwvvg.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3kmrqgoyd.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3rghoircg.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3dsuxnqhb.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3tyrtyenh.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3nhzcojzx.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3xadidwjm.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3vndbrdra.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3bvdtniks.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3rykkkwfg.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3gltjrrff.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3cybrqlxu.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3bghzrqcf.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3stbgsvri.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3yajjbhxc.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3qjfoqoij.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3bylnrega.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3pijgoqbs.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3buvqjyna.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3bdsyduuv.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3gvyirgft.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3akfsggri.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3vfdrabrt.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ltackyiy.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3eytwgncg.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3jphlrfvx.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3nrrazhza.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ffwtfeua.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3rofulvyu.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3kigkrrbs.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3yilfnppo.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3uonznlgs.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3euruvtyu.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3yqkugdcg.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3bvdengbl.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3ctfmqjiz.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3zfrpkwfu.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3pehkauwk.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3hfqyiiez.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3xhobkxkk.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3dkmdyurh.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3vqelqjgp.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3onkhvzsz.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3lrtniuqx.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3whryuwib.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3jmpmameq.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3lumcdngk.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3oghrpywv.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3thbfhzui.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3khlnpvea.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3uxuofxzy.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3bwqjuflu.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3naeaknzm.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3nskgddrl.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3htquvmum.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3rxpxxpvc.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3dbrthjxy.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3yxylfrfc.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3nbofrfny.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3auypscap.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3ltckaucs.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3zrnrucbz.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3qsmgjdvh.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3isgsubpc.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3nnngqidl.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3obwgyobp.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3tagemdoe.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3yvywkktt.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3ybylrlnv.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3jmmjxypt.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3hmdcpvwe.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3sryzdqal.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3oluvyhur.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3otbpcdss.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3gaeidgyz.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3nfxmuidg.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3pajkexcy.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3ekeluhgw.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3zerseaad.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3dmaiszod.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3dubqtmnm.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tvmjovqm.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3omipwlmf.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ipvkzley.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3kbxtzffa.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3taewrmis.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3zyjeozsm.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3fgngsuzz.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3jefwnhwx.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3qikisdtf.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3vbtvhznc.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3cicsvmlp.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3iuazamzf.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3pqpvyqja.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3ydxgbrzl.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fmdpmhqu.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3idibxeex.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3scckhyjk.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3pmxnexhu.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3vhatmfva.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3oqqqrwah.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3kxsyzuby.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3yfrgeapn.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3jjexlqnr.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3jijwjhse.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3znsmbzmb.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3zzingaad.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3eishzohq.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3stdvqyqu.html


<!-- 参考信息 -->