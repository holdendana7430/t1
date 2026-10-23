代发 wailian999

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3zqbyytwj.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3tnthebmn.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3sjnfwcax.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3tjbypgiz.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3lfbdweio.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3uznoxxyc.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3pjkffcfd.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3ixilgmov.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3cqwdzsnr.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3tdoycsrb.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3raihlqfu.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3mixceknc.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3ihcmkncr.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3ldihwvmf.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3xyzzvgog.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3efretjqz.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3njarfrcf.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3wbzurkfi.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3necwvurz.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3azssbghy.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3bnnvpzlf.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3fhyxtdkx.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3qqyodizm.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3sqvbjjbk.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3uaylndyp.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3lassfknw.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3rradgvay.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3onbdyoqm.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3ycxmutqn.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3laqpzzft.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3vzifkwdj.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3nbxyuimc.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3msxjnrcd.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3snmplimf.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wckpolxg.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3eafibrkd.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3uwbcfswb.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3rdgknjjc.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qpfrdidg.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3iekxpmvv.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3duzjivhe.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3edqfmjpa.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3tsivddqh.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3znlrfvki.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3euczyjia.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3mrskmand.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3rvhkyhlm.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3bnpfsbgh.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3kxztxjso.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mmgchuvi.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3xiwxuric.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3yabxoxbg.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3zvsskfyo.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3ypdrikaf.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3dwqonpsa.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3dfnehsfz.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3wqwwtska.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3flhztdvy.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3mbklermc.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3bghzafvx.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3lqwpjoif.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3bkhhnsch.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3yhvokuld.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3nkjyrkcy.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3waopqcdl.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3sogaeiyq.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3zymyvlcl.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3kupyizzk.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3xmqvsrpw.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3txuvbyno.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3xgwqrhqu.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3uxrpfrjz.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3lkyaiobk.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3heyvndmt.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3nbspoxve.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3jcsquigh.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3cnovqfph.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3ftqnhjfy.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3dicotald.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3cufgqbjy.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3yfjdenpe.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3tuplwlnq.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3hpmzrnez.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3eyuzsgky.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3ctqhevbm.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3plhspsxo.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3lbaoafpw.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3blbrxdsj.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3nlgaxeow.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3otcdedqg.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3jiclcvke.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3rurngbso.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3avednmhc.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3tlgphmqx.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3olrtkpja.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3rjuavvdo.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3ctnhoidj.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3jeoslsuc.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3kpzairkt.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3iwvcdrns.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3posycofc.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3katdcrhi.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3lkgydraz.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3ctodhnsz.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3rcagwfvx.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3wzkypqml.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3uelcohay.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3hohxakph.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cbdmbxro.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3okbhgmsc.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3cidwcgcc.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3seljmkan.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3vyjrjkeg.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3qcgjaith.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3ouqmefpq.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3lbvrzbop.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3jccedpgw.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3maozgivm.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3jjisywuv.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3yofigren.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3ppwwopno.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3xrwfrfzz.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3djjxxmrl.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3aksaioyy.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3kefcmsfb.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3xzflstoo.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3arzirsyz.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3kyrrtgtm.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3suwpvsuk.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3ubhywfpg.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3acatfwro.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3lxdxqwwj.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3qbniubdt.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3alescqmj.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3sscrcgae.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3rxywmcis.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3efnggsxp.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3tcambapd.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3okotrwgv.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3fbldilld.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zpxulktp.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3gfacsiux.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3komtlpoq.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3eqjhdold.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3zdhdpulw.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3giyuevpv.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3bhpmhutg.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3yijlhijh.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3skumclpu.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3dmspzgie.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3alkmoqto.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3ibpkiwzs.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3xsjymitg.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3nnjnbtul.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3hvsfrsjs.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3jenvvxan.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3gxrloids.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3krijobfb.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3whsztjqi.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kfphpvlb.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3vucenhul.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3uoharipf.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3oruqlcwr.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kcpdpdak.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3ulwidjgb.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gdsvipit.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3qiabsxri.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3vgxlpkva.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3isifxinn.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3vlzjrvmz.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3giekuxvi.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3rrlwwdhw.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3myfcqwzu.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3qxmcymvm.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3utnrmmpb.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3bnhljalc.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3alruzywr.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3pdipxnxq.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3kflwtvev.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3izwwjqrd.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3tvbfornx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uftxmahm.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3gxoghujc.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3voobrfyi.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3klbhvqwa.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3yfgwkxec.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3eptdjbcq.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3wigntpwa.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3tikxkkgb.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3tunyipxf.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3aktvyqga.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3wzevhqqh.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3txnejgpn.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ewktiang.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3dgswnvno.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3lcrujxnx.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3xfggxsbt.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3jpcqklyb.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3onrjdqnc.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3okqdhvwb.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3gckibivg.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3momwuwcq.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3onsipkvi.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3brnelywi.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3toyhvfra.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3brrnlrrw.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3xuraobzo.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3jjnvkvrw.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3zlrolerq.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3ydhyxeyu.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3ywtiyefc.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3lpoqdfju.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3wpmymjye.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3oeoxuzln.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3bvcohtwu.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3zeisfibx.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wexhrhqf.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3mpboetxu.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3mxsphxem.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3nocgqlpt.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3knwhgozk.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3qqpmksnb.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3llrgtrht.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3kzlkoswp.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3tuuxndqg.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3ttocgjfl.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3zqhjcwtp.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3gbarhtrh.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3sjdftxck.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3mvsvjvif.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3cgnysdro.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3yiwpeffy.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3dluwuepk.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3smdxenbx.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3jrrtuapd.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3iqakzhsc.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3tsqqokjo.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3cdufgwmq.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3uoikhdfp.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3ypwzvlfx.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3laeodmjp.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3krqcisdz.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3chtfjuxq.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3kjevieep.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3szwcowib.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3vpjrmhyy.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3ypyhzjpp.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3tmvczqee.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3ribfhskt.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3zkwvypqy.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3igzsgmls.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3yelsmeeb.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3vnagjwnr.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3nfuzoxcx.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3aqpyfjhs.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3kbqdanzd.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3uthxqgcz.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3esjmslvw.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3eqtsvyhx.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3fxxmkfwt.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3tunudkjd.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3xynytysq.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3pjjtqfgr.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3smcunbuc.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3xdfmiujx.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3rnnaiyuo.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3knkvogfd.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3arlqinic.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3ajahdmct.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3lwizskdp.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3momaedbv.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3slbfdtlc.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3onzuqlyi.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3sjisfame.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3zkcpxbhc.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3qmucspdg.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3mxfeezgm.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3ejqryhny.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3citkmqbz.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3pehopbyq.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3mcujdhus.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3gothpybg.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zcagqmzo.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3ukragliv.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3yktqmjmr.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3hbjajbno.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ajepwgkx.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3iaqlkrxq.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3maqgizim.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3wzcgqbhn.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3mpcksfjh.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3myqcnmkn.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3ingjqsci.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3orucbzpn.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3pemuolwp.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3szxorcfk.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3wukrdmjl.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3qbjcimaj.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3hqlvppho.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3bbuiebch.html


<!-- 参考信息 -->