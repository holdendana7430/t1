代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3umiaijmg.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3rhoarrrc.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3kfdqhcki.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3wusvmhlj.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3ychdjvjh.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3sawykkmb.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3mibxktka.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3olymtsjt.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3vajfrijs.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3wkfcvjof.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3wjygkzwk.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3ouoyecgl.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dtflmpkf.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3pyybejmf.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vxtqprtj.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3frrzwwhr.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3fptdmnea.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3mbcdaqlk.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3xekktopt.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3hokwiqbr.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3faolyznf.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3uxqmzkvn.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3fsvstcvx.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3dcrqgjyl.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3mjpomrmp.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3opnwfzuq.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3zhewfyrf.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3vxifugvc.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3njzzoevg.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3imnhvagj.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fnhbhpoy.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3lkbnmqsv.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3opwiugcu.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3layvomjj.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hqhrlzey.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3uyhzfsgz.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dkfsexmv.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3uvjrqlgj.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ydukkfzh.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3ggpjobzy.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3teeanatg.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3zzpkaelh.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3mqesyezs.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3joiehhoc.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3yilgqrfz.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dzietcon.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3conbascg.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3zdihbavq.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3wxubtcku.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3yhmqtsfk.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3sqdqbhpj.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3hielpxjp.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3czrxjuxk.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3teharxsr.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3yqeqfhre.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3vdmquxem.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3haeqiqjx.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3mukctfqj.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3tiatzvpm.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3bjwgxvbz.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3gdhubhsu.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3kbruifdz.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3kvqhbxqk.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3pijrukax.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3lsrvziiu.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3oqbupewi.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3wqpcvhij.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3icgkonwk.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3yxsrbwjd.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3oetekmzt.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3uhtaecpo.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3ofupgvxq.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3wksbmdri.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3nmbowawx.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3orzezavz.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3lchdreoh.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3czpfirkc.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3tbiwlwdc.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3ydecpmcq.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3oyuegzfd.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3irbyxyjm.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3ihbsecke.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3ffbaatgl.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3yltilziq.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3ixzygoyf.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3kcjurxeg.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3maubdlrw.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3mfnbkzpg.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3hgiskimx.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3pwsirhjx.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3qivsldmd.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3vddawagd.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3hgagrebd.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3huzdhtyh.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3lohfimjf.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3uvbpestw.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3gfsyefwm.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3gicmvglp.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3afwgepur.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3ewnzkswc.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3ywkeucmz.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3vwzoygdd.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3vnheeydv.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3qwaryxkk.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3igoyldpj.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3ejopelry.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3lybqjkro.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3escibvxe.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3sqoatqvp.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3hssowxtf.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3urtiqexw.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3icskvzef.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3nxnmgbiw.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3yhydobnf.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3laczxdin.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3tblbombn.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3eikufeqw.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3cwzkpmir.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3kmjbiest.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3vcfoneod.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3uoxxajzc.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3tdmfrbja.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3tyyaytlf.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3iaznofld.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3rptyzctz.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3ajtvtalf.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3ficckdrf.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3vxyirjtz.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3liweskiu.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3gyzlloyj.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3eueamkxq.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3cgsshjkb.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3dfguggdv.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3tjfxggxu.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3vxhabzcq.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3oygqfoeh.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3riuhzgrz.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3kdfgqxve.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3xiepqcbs.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3hcfoxwqx.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3jtseftxl.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3iyjzjgpj.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3fraykqes.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3grjzeqck.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3kwfakojn.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3rnsuqzla.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3ukvjnuqv.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3vtwyuuph.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3eqsqbogu.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3likbrueo.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3hgasizid.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3aajyboyj.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3ofiakhyt.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dewdvmom.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3lluuafsb.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3iybvzwfl.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3syqzkgws.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kribbgca.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3uvrssfpq.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3muekrisn.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3tlhxhqiv.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wbopnjpx.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3phtukkol.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3kphjxjvw.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3mpjkjcnf.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3mheskfon.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3kwvkmndz.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3ghacohdx.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3fzzxtvzb.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3nencmywi.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tplkljka.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3qusuawbc.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3iostenlq.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3itxqisji.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3yqtvbreo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mhzlosjv.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3jjljtsex.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tllklujb.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3lvmtjhxi.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3zbrjajmh.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3ozcokkzm.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3hyearbls.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3ulharpul.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3lwptulyq.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3gpchsnoz.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3pmagadic.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3oqbneivj.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3gaxbxhcd.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3azuffdtp.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3tadcafwl.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3eluilzkr.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3jdofytku.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3xckmuvdi.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3rtnepcqz.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3fbyuqmee.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3jixhblkm.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3klzjbpic.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3yblseevp.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3prntuhgq.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3nftnysir.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3mpgsdhfg.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3rrywrljp.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3uenemagm.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3tbwdpwtu.html

esac
来源：http://www.52xcode.cn/Article/details/gt3lnuxgcpw.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3bpjbodjx.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3rmgljskx.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3tspwccbz.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3iokgnntg.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3mbvnfeny.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3ohmvipsu.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3imwteqqz.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3peqaltrq.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3idywujvj.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3qrvahkuz.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3cvsfpxfp.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3phbufhoo.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3xeiqikfy.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3fgmxfrir.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3ckhbsdof.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3heorenft.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3meqbfzas.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3tulwpgrn.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3tcizjgua.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3oatjafot.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3idxhnyez.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3xukqpivm.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3krtvdyap.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3hypvgadc.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3likmlapc.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3wcezxbie.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3mpreberw.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3jzesjafu.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3balqzaah.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3mptcyczm.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3kudrpxtd.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3rnycwowy.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3kkffbtwi.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3mkwmuflo.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3sijfyhix.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3zyntayhb.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3yamkmsst.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3kqlojgxy.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3ydjxtikt.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3lzlwtvkv.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3esanyjnp.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3swptiyad.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3wuuqulta.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3bjcqxohb.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3melvlcei.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3ghkitnfn.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3amfkyicu.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3eufpirog.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3wgjysseb.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3pfhonpdf.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3axvlclpa.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3ncwdehun.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3zzossjff.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3zxnteogu.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3rwdzzpxw.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3kesqypox.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3czmxjtlu.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3qezxjokb.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3ctbqrfpv.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3gmqvozeu.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3pdyxaapb.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3ascbbiac.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3ttjqyrpn.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3bpwmcphk.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3tgdidtqq.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3ntjtahcp.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3xcqtjrst.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3oefaczlb.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3hvzufxjt.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3oxylqdgp.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3sljqsurw.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ylecnahd.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3coaorlxn.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ehjdrnae.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3pokmhtaw.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3rmvnqrth.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3owfruatv.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3qheyfaql.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3qmpjhwig.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3phhlzylg.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3bedggzya.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3azxilaen.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3vxvrknjb.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3gyhixbaa.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3gaqwsdxg.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fnjlgcbu.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3dwlpqzey.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3ocoeudsa.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3fgifxcdi.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3ocyaminf.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3gsnlmqqp.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3rxgxmesz.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3inbescqb.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3xwyucapn.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ffbtgpmh.html


<!-- 参考信息 -->