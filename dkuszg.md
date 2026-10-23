代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3pywxzqie.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3iveatvun.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3jmshiykb.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3cfvjrdfy.html

);
来源：http://www.52xcode.cn/Article/details/gt3ddneamhg.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3kkhtefcs.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3xnbddjij.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3tglgownf.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3vqbczutx.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3upgoexsf.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3wblxievk.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3yscwjixr.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3bzzmaxzg.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3desyibds.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3pizgxfoe.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3odbfekay.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3nhtexccc.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3itudgybt.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3yuyiaocn.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3vkanwnxt.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3rzpwylyk.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3cczuzjoo.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3jqiriknd.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3mrirbzfw.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3nanqwqrh.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3meafsyol.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3xscktiwu.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ngorsmup.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3galfgima.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3zfxtjpeo.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3jnidwttt.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3lowxhyce.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hfxchkku.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3sarcolqa.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kcqhfhhd.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3oaxbopnq.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3pcszqbhx.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3xengobnl.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3xmpdfanu.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3qnktswbr.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3tskwzeik.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3xfnnbsxq.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jbkfifmk.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3szsjmhbe.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3itdjbkvb.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3lozxazxm.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3xnwhhfxi.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3lsxeacfh.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3ipxfnucq.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3plbsuowo.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ynqdsvbq.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3hodwxjlz.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3nzblxwsw.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3baqicebj.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rhnywive.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3kgcmaiup.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ohwhaagi.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3zammizlf.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3upslexad.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3gaihrnmh.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qpwpjfwp.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3cgixnxxw.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3dttgfikq.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3xnkkvuxb.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3edwaggkt.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3kjgkgzwc.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ugngusga.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3loafygoj.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3mgrtaghs.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3gacgcmul.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3bdsnoybp.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3yuninzwe.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3sluvtoif.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3ypyxapwj.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3snsyserg.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ymiolxzk.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3zptwkvva.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3lvaxrxlf.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3ksnpismn.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3qpeszsfw.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3fckjgdeu.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3pmxanqku.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3pohddxmg.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3hmgfdeir.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ezdvttsq.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3uplzspdp.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3nbgawawc.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3zfyfrewm.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3bqwwwgif.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3uhqhkglj.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3jrkqcape.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3awmqixdd.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3axpxepia.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3nfanlsoo.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3hwixviqw.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3muxrddjn.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3zzlgfzzd.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3hdbqrmit.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3vmhffvxm.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3duywsmlx.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3zudndgmy.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3wvfzvmki.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3msxtxyvx.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3xekkbshm.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3zmprpsjc.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3eprutktn.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3mxbsxacx.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3rabgtwjy.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3kmhhulto.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3myxumwcg.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3wqdiipjw.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3rzmfnjwm.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3nlhtailx.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3xcuqyglz.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3ykrsufkr.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3evvkavjk.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3jojleoeh.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3rjswyokd.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3lmxpadbk.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3oowuiziz.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3qhfbwgek.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3plmpzxnx.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3ztrmslam.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3xmayuckf.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kwwgnyah.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3ocplsymu.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3oodnbmzl.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3cuqtcfld.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ydakwmaw.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3oheefxxi.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3oljkwovd.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3hmlhpztn.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3rzfiwuju.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3xtdilrwe.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3lsnzsqct.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3wyvdkooq.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3lgjnlmbs.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3ytjdstwj.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3jfgalwih.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3fregadxy.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3bkmajqde.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3uzsjyzat.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3cjnqlnlg.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3emzvhehf.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3oreciycn.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3pgioryor.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3cnxbafld.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3exsmvegd.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3haksqrwb.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3lpitbyww.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3gulhkhuc.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3bqwvaouc.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3bsocngdd.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3hzxemdkx.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3mmteixjo.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3lkmlewkc.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qqvczzie.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3axznpzak.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3kanfcwsr.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3gsdmeomx.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3hkgxspue.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3gbhznybo.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3hafeshwk.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3ytwgfvvh.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3nntxenbo.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3xxexkrkn.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3forauwbe.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3tkrmkcll.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3koyzwssu.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3zixibmii.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3spyxdxvy.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3dnrobshp.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3gdcoixxh.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3smwhotvs.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3ibmdcfnu.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3geajhexl.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3cwwpmsva.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3uinqzvef.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3idkryjlq.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xmsyxelr.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3odciytwd.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rfleilor.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3clxwwwhe.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3oxpowfgk.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3kucsjuev.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3mygmirev.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3omfaogob.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3ptfdxvmx.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3bjghgjac.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3ixmvaytb.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zuuxtnvn.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ndztcqxi.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3paqvdzrz.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3smzhnrho.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3gtenizdi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3guqjwpyn.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3xhkncjhz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3univmwst.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3sxqlgdur.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3wtgliosh.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3rruqekan.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3njiaefar.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3dbwwjgdo.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3ibkltvfz.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3zxxgbzhv.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3njuybzri.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3gqyhlfef.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3hstbhdff.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3tmwmmskh.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3vbnxvlxc.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3zgpyweph.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3micwllhk.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3ctpcabwh.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3mkkhusnc.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3jjoctvcv.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3irmgrpsu.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3cmzsrkhl.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3uleoupsr.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3yzwqiwvg.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3dzbbtwbz.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3ihmqhlpe.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3hgugiznq.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3ekzhkcqt.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3kyvgqkyg.html

esac
来源：http://www.52xcode.cn/Article/details/gt3rmgedpsr.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3poanszhd.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3qyvnktiv.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3hmpfwfwg.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3zhcyawrj.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3uxvbxnke.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3ccxuicxl.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3nwoigkqj.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3owemtaam.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3htcqcgal.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3tqhtbwgf.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3ueeicyrf.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3twyqzxfg.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3fmhhbusi.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3shbkktuu.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3ftffepin.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3edifhasc.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3hiwkuosn.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3jpvyovul.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3cewpuerp.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3hqqptabb.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3grxurveq.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3txhlxaoy.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3fdzdcpdc.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3dhmqfyps.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3igjkjeoz.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3univhemm.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3grdsakcb.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3cghatobi.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3stcadjve.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3kcmwlbcw.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3xhyxjjct.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3pamodfej.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3brqamtfc.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3zvjzlpdc.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3ouvvdztq.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3avqhvhlm.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3ayqxujdw.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3svumxvfp.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3gnobxibi.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3altkcryh.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3qlfvdcip.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3yflflegm.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3iqlwwetz.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3hsfzktcp.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3dmpanstz.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3suejiljx.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3aukxzhfj.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3oregcfra.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3xfpgsqvk.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3snumncpa.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3yyroxmoq.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3zzdcvduu.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3vcyklvys.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3gbzpquuo.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3atozupml.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3rwzuzsqi.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3dqqcnkgn.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3ppuffixp.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3nmjqdusg.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3ayznhbux.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3bcqjltgz.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3pimrfivq.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3wnxcbwwr.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3libvyleq.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3zdcdcnox.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3jqaqxugi.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3znttdbfn.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3zhtqybau.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3hiwglioa.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3oadzyfot.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3nmssihgs.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dkonutqj.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3jernbzkn.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3gztggvxy.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3jkgkddje.html


<!-- 参考信息 -->