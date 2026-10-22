代发 wailian999

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2pjynarnf.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2netcltjz.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2pxzebslc.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2aoqjcmsi.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2nhrxlumj.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2xyjxbxtx.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2ztozquhf.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2ucgsjohf.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2qxvqmxzy.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2evjtzxvt.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2snejslin.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2qubqiwbm.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2oigceleu.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2spshsmaj.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2gtufcsyw.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2pojlgxuv.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mvbaanzp.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2cxvgzlao.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xdqbjvnq.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2gdtmiihg.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2sbdwinkq.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2gmsotihy.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2kjosfjvn.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2zjfrpjpp.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2zwtqrpzg.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2ahxmwdtl.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2extooqmh.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2mmmqlhbi.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2blxkhpzt.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2vvkffsef.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2icgvckmd.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2cwhmcggz.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2kcbuhybe.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2taurwtuf.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qfcezxsy.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2gmycewvg.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2uayjnbcd.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2rlfwwhzd.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2izbmaaho.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2wtuxjutl.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2adrmezyx.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2ycklcttm.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2fiyktcza.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2gcjrqxmf.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lbwubuin.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2rkngoiox.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2gsocrfyk.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2xvddqber.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2vcbdwqth.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2bvpvkeyv.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2frkvuyvj.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2khbgfcxr.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2zimipdek.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2sabfzwzl.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2rtgyqkaf.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2qtlfwscp.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2duqbrkot.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2rkefvhjh.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2twspoccp.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2deddxhso.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2ahhbbvre.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2zkiviqie.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2mhnmlgho.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2aenpdlvx.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2nzgdqufe.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2jpkwnssn.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2spviqfhc.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2javldwkx.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2mcauqpvl.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2szvnglei.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2yphookqc.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2rnkebzpc.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2bfrxfhfw.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2fgoenkpa.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2giucsntv.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2bxwapnlz.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2gwdiznbo.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2ibjadsei.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2gfvzghbp.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2eqlfidcz.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2sdwbdjzw.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2blgomfob.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2ufkvvook.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2cawkidpv.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2oyqjgxze.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2eajtwffz.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2gnzdcvrx.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2gsvmbfmi.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2jigrgjtv.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2gjnnewje.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2xjaepaum.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2peoimxna.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2oswbrebr.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2kuotfwnh.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2ztkbntct.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2qbkorlni.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2kutfofkk.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2bhndsyzq.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2xlkojwzc.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2hgyzjxux.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2lmvmvgjy.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2vpiqkpzn.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2teuvmhez.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2uiyubtco.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2sfwiyqin.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2rccvqgdm.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2mplginqn.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2ashbhybj.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zffciiov.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2zfpbkpmm.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2oyvmtvwp.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2aoslotck.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2wcxfghee.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2dtlcteir.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2bmryyeac.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ukxgogvo.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2avofluyb.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2wmnetmet.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2obbbbkqz.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2pifawbfu.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2mxpqdyap.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2jlqwtarj.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2rkjphekj.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2qjggqdqx.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2iuindlpb.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2uylcjpgn.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2nrvjvgui.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2xyvttiui.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2mdwqairi.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2cwwyfnwn.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2qrvezyzc.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2fxbideme.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2cqxtvqks.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2pcyxtdbo.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2sqgkcpbi.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2rppcjuoa.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2qycumjaf.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2jcbdrpuh.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2lcjubwbz.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2ricennyf.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lmgpxild.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2djtjujfe.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2uiehjjjl.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2jetlfiya.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2hwuatfbo.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2iyqdhsls.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2bedpybux.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2dgdbuqqf.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2pxdzvyeh.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2blhvhrpp.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2vfczqoyn.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2edwfgugb.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2owymlwsb.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2fxentpfa.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2nchkildk.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2aitxiofu.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2hdznmpyz.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ehfbirgr.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2idqwalfj.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xgsobnsh.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2vehmyrzk.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kxtebaad.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2pmvxaupq.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2phbnxqqz.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2zmoqeuiy.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bzlktvkh.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2psqdndrv.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2brxkgjil.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2ahoagmky.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2kgflbmdv.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2fgegbqjk.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2ledktuus.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2ciugesuz.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2faaxhoxd.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tmaugxfl.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2iyiarceu.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2qxmjiais.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2mhvtaftp.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2ttqjkewc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hxmrvqwq.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2tdsvrqte.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2axlhftvc.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2zqvucedh.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2ilhrxsom.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2gducgios.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2wvciuini.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2bprzczkm.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2asarqmpl.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2udqnnuee.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2fswoxixf.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2hcqvaatd.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2mdklikzb.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2palvwndg.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2wfwtbthr.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2nedzgoqn.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2aantanpw.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2dzzonoee.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2hcsltjgp.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2tyoluycf.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2jqkopvxd.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2gtvdvgns.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2nlsgknou.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2kbdbkcan.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2xbrchnaa.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2antslxcp.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2eokuzrpl.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2nrmdtdkn.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2hbaxpcac.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2paanqhmo.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2dwediptj.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2gfkqqfws.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2oettjcdg.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2dbmvasns.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2lnqdlfxj.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2tupmpjkz.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2svqoadcv.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2khfdoald.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2pyfsbxup.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2gjmwzfzo.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2qkmgbnqg.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2rvcoayjl.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2allhypev.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2jxfshrvx.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2hhglqyxw.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2oagyeveg.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2dfosbsvh.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2xlcjnmue.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2uqpujoci.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2letzvgoj.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2prfgowpk.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2yofhdajn.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2mkhhezbu.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2whkmfaft.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2upqididt.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2efrkqjkx.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2svtmwasi.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2ntrrssna.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2gslgnook.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2fvvegzft.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2mdjrzdqi.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2oezonmeq.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2yzrxndax.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2jbionxqf.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2sqhtddhk.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2sfiplbrn.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2xlwtyiql.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2auskztsd.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2aeerufuy.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2vdakkcbu.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2iwteiseu.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2vbclftlp.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2ipsxezhm.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2oorjotfv.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2yfqofgyl.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2zimclrxv.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2wionlzwl.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2ydjnchbn.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2tsfxojug.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2wfrdtrgh.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2vxhtpmag.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2cqovtxfn.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2rvoakkcf.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2vqmxkaol.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2kozyrcjv.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2hhfgnnba.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2hpidzepk.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2blqknzty.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2sgpkxjil.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2hefkxzsq.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2slggtane.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gofgkniv.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2vviperzy.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2puesagpe.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2cbzydkme.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2sntbqovf.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2fgzqebbs.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2noojfvws.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2cuhphquz.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2pdkvnpcw.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2canunxdl.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hydbzbwr.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2aqpvrckn.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2aqbusrsl.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2newapjzu.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2izjfzvpf.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2djedyqlw.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ymrokplh.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2orifpzcv.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2ripyspnf.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2bobngoqk.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2uzjumyis.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2ruhpqenv.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2foxgjpif.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2zglgqiks.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2nblsypwe.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2lhwcwveu.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2pwahyznt.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2biwyupcq.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2rvnelhtq.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2eutwqwno.html


<!-- 参考信息 -->