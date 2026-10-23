代发 wailian999

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3xduuggwt.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3dqqggulf.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3ttlttktg.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3avofnafa.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3jfszmlyb.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3qzqkfjqt.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3oevcfmqi.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3shfhynjf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lbrppfgn.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3cblgneuy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wpxqfxhk.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3svllyrak.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3jbrxiehh.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3rsywkspf.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3tkbhytvh.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3elvqcrru.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3nvtjuxae.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3yghpkpsh.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3egunpatc.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3ikrgjwew.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3puggehlm.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3xcbqucne.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3psptyltg.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3dgxmyaua.html

);
来源：http://www.52xcode.cn/Article/details/gt3ctmydpmd.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3fcnbfjsf.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3qzndqavd.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3dobtdzzw.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3wbjnlvaj.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3dlojfdfr.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3osevrtyd.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3eairmaix.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3lvcywkgt.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3mtiqqcok.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3oxuiigry.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3pgamhkfw.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3csgnceoc.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3ygbkfiyf.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3tyundcfq.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3kpbvrmou.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3bnxpyate.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3gjajknym.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3kfojkqmx.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3pclvptnp.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3xfvemuku.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3jpubpfwj.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3wlwdtear.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3dexzpafz.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3iawdfddm.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3vbkboqwq.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3kbhzjcez.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3osptjaet.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vwzkbrbg.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3ntzttcgm.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3sbnjbnaf.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3hmfiypuc.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3enjotsfq.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3zdhhhtxj.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3qeemtwrt.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3mckkhvjk.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3bxtmwxur.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3wmcfmbra.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3dihwcmcm.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3hvcmqfql.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3vvvmhsdp.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3domihelb.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3kqymigmz.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3hciutftt.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3mtkbhfwy.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3uepouqxb.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dhzcsqka.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3jbtjdjfu.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3zgynyfev.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3fbfguovf.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3uzprlfzo.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3zpcoctiu.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kosbtnbd.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3jnntvxnq.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3mizzzlxh.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3zxchinxw.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ftxagwiw.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3rbftxdnb.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3nalbngip.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3bpfhdlpb.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3tgkdqofz.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lfzodupm.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3fvhjxetu.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3aysqxufd.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3vruxvrpt.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3wcboyjhr.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3yeyggxgc.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3deutccjh.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3xkqjihdn.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3zrlbioux.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3dlqzxvei.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3fvovdcee.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3ecnzjvjk.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3beoekomz.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3zgzigrsc.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3wyhwrhid.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3kvphbjdr.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3gwocxajk.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3ahnybhnk.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3ovspnkmi.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3fcugruwx.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3zrhticig.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3gwfuxkns.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3cgezenos.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3mbhdgpaa.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3kxdxixfo.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3yeyoglgc.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3ithdtsbq.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3hiauxaec.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3prqirytc.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3yqrxkuuh.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3tchcibog.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3vwnerduv.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3yomgwuku.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3lvupconq.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3shraojtj.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3aewcvuek.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3rcliqxhm.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3wqllkkyj.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3ottkrhsi.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3xzujkbii.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3yirkzcsh.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3mbnaisqp.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3zxdapksu.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3fqjtmidx.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3foojvewk.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3ipiwneqa.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3czcrcsyg.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3eozguyno.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3aniyhajt.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3botxdtkh.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3lbsbejqu.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3ewbszrju.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3wgayyvne.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3bvstashl.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3msokecvc.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3ynuxosvf.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3xsqmtcpq.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3vimkzwiw.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3npbjiwwp.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tzgttoob.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3yvyamyum.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3qwoptwvd.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3crhhiqqi.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3yqjibffe.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3bmthofcv.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3wwadfvse.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ocncbdnn.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3dlxnzhif.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3comcwbma.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3wxyvquzf.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3cwrcjpfi.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3jieddxcn.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3ktlwutfj.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3zjmedmsp.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3ojlbwlcj.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3xtupnezw.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3lqwzfqqu.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3uzeykfsw.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3vqvqmlmd.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3ejugcxti.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3ubolliff.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3wtgoqjur.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3mjrxqwjq.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3dlspfmem.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3glumktlf.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3hjgmjdrr.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3bkrlcgon.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3lpjgplii.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3jyxyzgna.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3pnocjmxo.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3vgphtvdw.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bciuxtme.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3cuxywyzw.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3dnspgqdf.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3uklknnbb.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3jrzavjti.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3sovjtxug.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3nvuxxauk.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3ocqaqpcb.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3amlmzkaq.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3ptqfgvzl.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3hocceezi.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3swtyufsv.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3xfjhtkrz.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3xdvynscs.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3hjoaiefg.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3ruuogauh.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3txwtqpgd.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3efrixmif.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3okrqaksw.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3iiohycwx.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3fkvmkfqj.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jgxafkyb.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3sfuncvin.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3otnefezx.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3ufyfdlha.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ymeffnbv.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3ezwwbglg.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3bignajcp.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3seodrray.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3sichkddy.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3icrvjpbf.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3irawaiyx.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3ukkoiebr.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3nwmecuuf.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3scvqfows.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3tnczubyb.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3jhpnggmd.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3drbooxdr.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3miabtpbn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xhodrsum.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3hcissqtl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cgrfcujx.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3pipygxjv.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3qiyugpkm.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3utymqscn.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3ktkplhax.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3ezsoxqnn.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3mrlhmbla.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3sttmhamj.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3wksvmjoj.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3yuqkthtc.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3ehymykab.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3kyzmopwj.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3gpngzcwc.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3imecxcgi.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3crntznuq.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3ekzmqcil.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3nsytzaju.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3etvdujdm.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3gukkwbat.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3skktuynj.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3lqvyqxkk.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3upofvrmb.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3jeymapto.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3jhjmmcyt.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3xalrdafe.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3faqpgxpu.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3kkphtsaw.html

esac
来源：http://www.52xcode.cn/Article/details/gt3aekcdhmb.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3aclnwxhd.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3irelemks.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3eyxvvhii.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3rhbfmiga.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3eoxqmriq.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3dkoznttl.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3nhujtwex.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3vyadutuz.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3obcljzpw.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3skcjrapi.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3uxtvbdag.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3whrspmwf.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3wjhcjsir.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3bwoaskwq.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3oqczbcnc.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3dhwmsqoq.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3ivjmohyl.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3vwjrfvey.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3avfilcly.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3smaqqxtv.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3kgcwxeil.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3ezcovyqb.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3enshrira.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3dukzzpgj.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3uloxlvaj.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3oweawhpr.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3zwxqwskv.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3pcrmigwk.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3rxsstrma.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3onspvsae.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3brtsevgv.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3dclocznj.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3cvpjafdw.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3lzlrmyqm.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3bwwjkpqv.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3kdaiuoqp.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3fcosjpse.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3edverzhg.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3wmnsgjde.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hugdspeg.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3dawpythc.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3nrxuqlvs.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3oqgrloza.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3fbaxkuno.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3ofnnexki.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3fiqcwltf.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3kcfynbhc.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3sudmaruv.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3vazwixsr.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3xywtvqyp.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3xhungvau.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3ertnkekz.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3pcwuxqku.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3slfyuqen.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3eknzxtnb.html


<!-- 参考信息 -->