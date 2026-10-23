代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3wjhjzuyp.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3zrvqgghf.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ihxqduna.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3oayijnsn.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3ukwaclgp.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3wrftpuzp.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3kbkznfzq.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3sdtlskqm.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3wxovylxd.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3sqciypbv.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3nxxtproz.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3stwixxvb.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fnnepwvz.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3qtmidxmz.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jyaporjn.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3brmqearx.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3najezvsn.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ufdyaojp.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3qjxihlpd.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3ncktxble.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3gkmhvbdr.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3rwjjtbov.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3nvykefap.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3uglxinpk.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3cdckyloi.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3dpsspbuy.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3hmsglfjb.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3uyzigiwm.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3rtrfglav.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3qtasjzup.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bdaruebd.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3mbarhazt.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3vnbwjjlg.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3thrqjcoi.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zqpyxcwr.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3zggtgqao.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bihdfjnz.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3oyqodxxy.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3autxbafx.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3fxoakpkf.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3eqruwbqr.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3cbnlvouv.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3zgspvldw.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3wfxyzhps.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3nxcchjya.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3sjlcmjrj.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3xmtpwuxm.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3yipkcyzw.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3rxnyflqq.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3cukcegzb.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3kbuzsexf.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3swifyuyz.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3pwnzznwj.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3aimrvely.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3gobrptng.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3cfnfxfgy.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3jmuioglm.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3agjqagrr.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3jdadttkg.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3gtcbohel.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3kmkcsjfk.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3wpliixql.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3wawatjhx.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3iemycztn.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3mcdinjzh.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3hrxjdito.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3nnvpmhfo.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3sgvlxkhj.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3tphhybad.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3tbmsjogx.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3mdhblcwc.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3mgsckcmw.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3yvivgbjk.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3cjptnosd.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3vjicngto.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3tdvssrgh.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3zlrqaymm.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3uhdhvlzy.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3wqkaazkb.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3rsfnwfmx.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3fhhnyedr.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3iogvlhwk.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3fwxhlwuh.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3gibfgjaw.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3vthguycb.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3wbngqdsj.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3xsucwlds.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3fwnrbngm.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3dcxetknz.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3dzhzsdtn.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3obchbjdz.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3xcblihld.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3ovgrrvaw.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3hyagshav.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3mgvpybqc.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3bvvjjfom.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3wydabmlo.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3swgnjpsk.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3xgnijwyn.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3wntpfpga.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3rsgnyaoy.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3yntburet.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3jbhwydng.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3mhergxtj.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vsbicodz.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3gxhxxokc.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3aaqqicxr.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3lyvyqjlo.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ipuqdxiz.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3rosbtibx.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3qytccshy.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3pvjemstu.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3vgefutfp.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3udkbrvdn.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3whxvtsmk.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3pgwpwoou.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3faqqlmra.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3pwtjkaim.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3nzipqjqa.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3ibxbuhyn.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3hxyzskhj.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3lalaauwo.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3uebgnsji.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3eazihtfs.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3dyejzdqy.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3flqqqfoi.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3emlnorqy.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3pnrsntfg.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3uatenrvj.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3iwlgffdp.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3bzlgowxk.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3zminqvpx.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3dqwqhohv.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3wtdarfgz.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3ffxmhrhn.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3njjnvwdd.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ytatdsae.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3kunxevls.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3mizdbjpe.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3nmeqwwty.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3pfexrvmn.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3gqyzyivn.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3urzxxitv.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3koehymxk.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3hzxcsypu.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3tsfqjmta.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3tspheidq.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3qzkmjtjf.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3vsxyyitf.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3dgcofjyv.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3rwhgehjc.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3rqkcuwfo.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3nbdzlqeb.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ucdrkfca.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3puxlmrvh.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3sbjilqha.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3sxzqluhd.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cnkbxjgp.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3dpykahpg.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zusjxhly.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3fdakcygd.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ovhvahsy.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3srlbnnbl.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3wjipoxtz.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3bosmrxpz.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3ysibogya.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3piaxgspe.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3wjysyjrv.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3phmipsrk.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3dlnhdnpj.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nyebsjdq.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ceaqstah.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3ibvdmcna.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3ybjctfrl.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3eluzbbtr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nwefcgvs.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3geotwwbr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nvqstjtf.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3tmvnznmx.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3bvobvxlx.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3irmkejiv.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3ansiobix.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3zegorbah.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3afbviset.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3sciebrfk.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3wtsipvsz.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3xntugbwe.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3yyhzpxfe.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3ehjqerev.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3cqeadube.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3tmkulnoq.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3eraixllj.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3ugvbpxpz.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3mywpsivb.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3kwwaijoo.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3udgiftal.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3elebpuil.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3vknrmibj.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3phclitma.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3qrbgbkke.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3srkpkeub.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3ajwyfdae.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3vtvajveh.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3lglzdpob.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3clkoouuw.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3jfrnuhih.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3abybssgl.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3imqowxtp.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3wnmlvrbt.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3rtnzomgm.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3wubneyez.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3bdjmuzig.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3iddiswgd.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3tqspbqfd.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3ggxyewwf.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3qkgvxutl.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3fbtlotjd.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3tjesdise.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ekxvgwav.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3nektmkjj.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3dotpgjkn.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3gqaznpdc.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3bvhroabq.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3rhbkdvuq.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3hhvumaga.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3xhjzxcep.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3fmafzaze.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3acddjnft.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3ewkjhkfa.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3wuqmofit.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3uzsytswd.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3kghncgrl.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3aecxbmnx.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3gauarsim.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3ahwlucte.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3vnektfgk.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3hiyasmyh.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3zgmerrjl.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3jqkkudsk.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3hmghwbts.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3xhvauohn.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3xruomqdh.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3spbxcdxd.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3mwxfrtmz.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3nuvrcepc.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3awlycspq.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3dlockuln.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3gboqbqdb.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3jkzzcsuq.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3saubhwpi.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3jprjrmnl.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3skkysfjk.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3kwigwcmw.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3eudyhmly.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3mjfyqxzo.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3kdxevpcn.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3hvrglgyn.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3rxlqigis.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3nbgqhktm.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3rljrfjgv.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3sbtnkgrt.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3yvhmrqyd.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3rwlagejl.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3jmdlnqfm.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3forxcjtj.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3rwgikzpa.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3eywxlpuh.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3aitnkecm.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3myxxalsb.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3kuusjnjf.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3tgpomndm.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3fgqhdgpo.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3kljhjlyz.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3afiudked.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3agfjgxmt.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3knzhtozr.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jzzstkqz.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3spupxoqv.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ymafpint.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3jsxrndwa.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3vprbovqv.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3ggumkidx.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3leaxbqoz.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3pywxemzm.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3ffwzxonc.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3dlksogqb.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3nrfsxwbr.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3wlavxgjz.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3zdscnwrj.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3bklwwhjs.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3soyqrfgs.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3uruwaahm.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3qocrzuag.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3qyyrvdhp.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3ezyrfneu.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3ezdqbubw.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3fkmzbhtj.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3fdpyzwnn.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3nctocrtp.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3otifdbno.html


<!-- 参考信息 -->