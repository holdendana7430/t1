代发 wailian999

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2hkzutdtr.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2cieilzwv.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2alivuexy.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2mdpwdhoc.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2diofyhcp.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2pabbwjsa.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2znecffry.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2pnnjdzcc.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2criehasl.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2rfmbpjip.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2nzkebavr.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2hsqrhiln.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2ruxcyxdx.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2acyxqefe.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2hgbvfobq.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2jstfyvix.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kbadiuvb.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2gcpsvyoj.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tcxbtbbd.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2hitpxvpz.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2mqbvkyjw.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2pzgrvaap.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2kiijdhzv.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2bulfqxtd.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2wfdofqoi.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2lupjkpij.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2ymsmammu.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2wbeczwgt.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2lwxajoyk.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2sudcodhz.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2kteojflf.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2tgkrtdwi.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2flbnzsbe.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2jbvdkpoz.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qqdxwooa.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2qiyrchum.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2tegnhkfn.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2pxwrhpcx.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pffdjrke.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2avykoxuo.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dszerwao.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2mhznivke.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2bxxvsnal.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2qjyhccfq.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2matchvme.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2qniuzxko.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2jyhtawax.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2qfpdcnny.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2tifkcedq.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dsablvrq.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2uocwcwwk.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2ilfvwwma.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2mpaomtlo.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2oecrwxrq.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2iaylvdaj.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2fsgbosuv.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2vtieibem.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2ukqnrwno.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2qgyomvgc.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2hrrfxeqy.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2oqllfrfs.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2blxrbewc.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2zrzsuelg.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2vvzzlsar.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2nymyjumw.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2yvbkkngn.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2qufrtyya.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2ucgyqxjz.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2xilcniov.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2tizjnrpt.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2nqblrekc.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2wlpchgkk.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2pfazkkae.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2dalyrfyp.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2xqtgknus.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2acipguai.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2vwivotlt.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2mwqshjdp.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2mljctgox.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2osfkukoo.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2frgahtng.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2jpolmcup.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2atoxquxt.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2ebuglyqv.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2dmlchbru.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2mgnrarlr.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2vhyipwnh.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2vmverqgb.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2qvudpgzy.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2nzvglupn.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2qrafczxd.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2vdqnmstr.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2kubigqbf.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2xxtbgxaq.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2ffiawqyx.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2bocfzcon.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2xmgtguzm.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2lxsvosde.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2uzihsxpy.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2kmlzneeh.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2qfzbsghl.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2fwuyassq.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2iudlcfsv.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2vkzqdsdj.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2jgkssuin.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2vpoivbsu.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2gbvmacqt.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2kkghuyqd.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mppfbfjh.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2ygsoiqmd.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2bgaspavp.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2kimriztd.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2yxrhepfg.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2dzktukfr.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2lmpwjsxe.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2fzuwtuzo.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2dzgtxqpo.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2huxlzubl.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2exskagjj.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2yvaxpsxi.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2gesmnlub.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2mecxvxpo.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2wgdqasqz.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2vujcirtr.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2iitdarff.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2ptodoegu.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2qkhwuasz.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2qstykvaq.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2duhxgvrr.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2fmvcquwq.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2wingxbqi.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2evotbsfq.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2glgruyfu.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2zyuvameu.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2ygmlncgo.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2cdglxmcr.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2cscrrznr.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2cblzuduk.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2xlryvahw.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2vszlqhxl.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2aivkipdz.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2vyoatuan.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2cwxkyfke.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2hdxxgazw.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2hoecmwdj.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2xoxoypvv.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2jeawkbvk.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2zkbxqzpo.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2huqqjhzi.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2yuudtzrz.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2lkgrthlm.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2fsbridnv.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2hndqmjhm.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2bcmxspwy.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2vgcavljy.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2denqnabx.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2csiopjxs.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ukzwwcow.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2emwmytmw.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dkuozpdw.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2vlxosgxn.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cggwdvoy.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2nvzohxel.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2seznqkfu.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2dsyapqbc.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2epekjqim.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2pzimabmb.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2rxebdjkd.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2rnzcljno.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2xxmiupyf.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2sgevdhhh.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2bjfdsxch.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2xqmqyykh.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2prshlafn.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ekajupyx.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2mgbzeydx.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2zxgnxxlo.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2gkboffnd.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2lrzsfevp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vevdanlj.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2focudiin.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2trljswwe.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2lypovrkb.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2lprcxhuw.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2zzvzgnkf.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2imkakdng.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2loxzjbkl.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2cydyghbk.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2cbdjtxcr.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2sydevwyk.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2pfccisdt.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2zuyzistk.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2bvrnbcuy.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2gkkbjflt.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2nmsnoshu.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2gntwjxeh.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2dxmkffgx.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2hyxaxbrh.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2spbfjaxd.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2lpvakfyk.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2oxiyukax.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2vhirdtim.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2wziadevk.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2oqafdxjh.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2fmzafpsw.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2uoitncah.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2mbvhvwwr.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2zmfbskkh.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2imxlyvek.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2rnkbwqet.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2jjgeozvw.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2qrzpanqp.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2pepiuyla.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2ptaafeqo.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2buhrpfbg.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2jhiucdpu.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2uhyskvgk.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2kwdhioiq.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2mdqtmimc.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2fcguluhb.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2bvgbxpmh.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2atldattq.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2jyuzijct.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2qtpkpedm.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2hvfjqvqs.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2myqamdss.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2omctnluw.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2civpjnzf.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2sciouyvc.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2aqjyiodc.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2oqqeglfa.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2smoqfpbf.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2zuiibtxz.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2nwjqnjgv.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2mrgoabdq.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2cdcwoqvi.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2curykmec.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2befesuno.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2putsihjo.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2iihhlpjl.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2awyhwmoh.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2geoouxwl.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2hzgdgvti.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2osrrkkdl.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2atjgrzeq.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2jjnczxzj.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2ptnbouyj.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2bpszgkzq.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zgdpqmmv.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2noavskkg.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2myfitoag.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2fgwsxawm.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2xmteyqre.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2fionbwux.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2cxqhgatn.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2ykdhxisr.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2rcbnyjcm.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2yofrbfdi.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2gngljjwy.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2xnhzfwdm.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2goxpeizh.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2olxtraid.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2zxtxhuqm.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2cmgoysbf.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2dgbzyccv.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2xvvfbxpk.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2hudenevt.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2rhblsojj.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2yxtlhqbz.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2piwqpknw.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2vfgxheer.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2kmfzbqsb.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2lltkfuax.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2gowbitxm.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2hhthknrd.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2rwgksjyb.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2hmpddfxn.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2ntaulpzg.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2jjilizov.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2bwhiaedq.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wgkpmnoo.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2gnfqqbtg.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2jrddahoi.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2fxjfpzqn.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2qmbbbogw.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2hydpksbn.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2yqelckaq.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2rratvfhz.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2srwnuytm.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2fpuomtpe.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2oqfpjzos.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2msiknmri.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2nnrkfpfn.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2tdpuohjq.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2oqpuvahv.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2rnefekyk.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2zlptbqkk.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2zibdejjy.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2ikuvyngv.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2pxvwjauj.html


<!-- 参考信息 -->