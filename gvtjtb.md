代发 wailian999

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.wangshuangyany.cn/gthgzhflma.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.pycfn.com/gthpyznkll.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.shanyushiyangkeji.top/gtogxrzrct.html

[P08] 处理浮点精度问题
来源：http://hz.hfpthk.cn/gtjyqncnop.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.cashguo.top/gtjkgepmnr.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.mhx1999.top/gtgdbiygvc.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.kuanghao11.cn/gtwbbgbbmo.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.vqdsnc.cn/gtggstuzud.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.jqgfzy.top/gtdhdnlqrk.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.sweek.top/gthnbytszp.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.nwbrower.top/gtxvtrsxez.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.ppjwa.cn/gtsujcuhns.html

================================================================================
来源：http://hz.hywenlv.cn/gtgcodftsf.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.yuanzhike.top/gtzhwlzmvx.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtxdjcvkma.html

[Q01] 创建表
来源：http://hz.xinyue.icu/gtffniqrzq.html

CREATE TABLE users (
来源：http://hz.yj20258.top/gtynzqiimu.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jqgfzy.top/gtghxrbugz.html

name VARCHAR(50) NOT NULL,
来源：http://hz.yj20258.top/gtkbacpssl.html

email VARCHAR(100) UNIQUE,
来源：http://hz.52xcode.cn/gtgpiqfqwj.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.yj20258888.top/gtotmbjucc.html

);
来源：http://hz.tanke756.top/gtxvlaaydu.html

[Q02] 创建带外键的表
来源：http://hz.ivvv.top/gtyimdmqnu.html

CREATE TABLE orders (
来源：http://hz.nanxuanxn.top/gtdggespye.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.wangshuangyany.cn/gttashfaso.html

user_id INT NOT NULL,
来源：http://hz.aizwys.cn/gtzsvgykgg.html

amount DECIMAL(10, 2),
来源：http://hz.shangyingyoupin.top/gtwisqijzf.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.yongpay.top/gtjbwebash.html

);
来源：http://hz.hongshengwenyu.top/gtcucoaayg.html

[Q03] 增加列
来源：http://hz.shangyingyoupin.top/gtsnhfhtox.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.ivvv.top/gtllksgkre.html

[Q04] 修改列类型
来源：http://hz.sweek.top/gtlznvvehi.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.zhongyouzk.top/gtnydoxdlg.html

[Q05] 重命名列
来源：http://hz.zhengqikj.top/gtuptkrkih.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.birdmap.top/gtsvrhhjjj.html

[Q06] 删除列
来源：http://hz.feifeiyinyue.top/gtuqnxkzpr.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.zhengqikj.top/gtinbjluxx.html

[Q07] 删除表
来源：http://hz.hfpthk.cn/gthoxkoqui.html

DROP TABLE IF EXISTS orders;
来源：http://hz.yuanzhike.top/gtekyexnze.html

[Q08] 创建普通索引
来源：http://hz.zhaomingkeji.xyz/gtblgraofr.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.sysykeji.top/gtogrlxbsf.html

[Q09] 创建唯一索引
来源：http://hz.yj202588.top/gtulghvvri.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.chenzaomai.com/gtolpwrufk.html

[Q10] 插入单行
来源：http://hz.nanxinkj.top/gtcupjaxki.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.jinqigufen.top/gtvzzcloqf.html

[Q11] 一次插入多行
来源：http://hz.zhixingplan.top/gtbbtitanc.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.iojbl.cn/gtbgqmxzcs.html

[Q12] 插入后取自增 ID
来源：http://hz.zhengqikj.top/gtouiocfzf.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.yonumen.top/gtxknjvujo.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.ehwqpu.com/gtnmgfqbsj.html

[Q13] 忽略重复插入
来源：http://hz.sxryk.cn/gtgpqipopx.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.zhongyouzk.top/gtmrxbythb.html

[Q14] 存在则更新（upsert）
来源：http://hz.yj202588.top/gtrtsgfdsr.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.gzhubu.top/gtdtjayokz.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.hfpthk.cn/gtanhfnazf.html

[Q15] 查询全部
来源：http://hz.xuetiantiany.cn/gtokuqsgyb.html

SELECT * FROM users;
来源：http://hz.zhongyouzk.top/gtabuepjuq.html

[Q16] 查询指定列
来源：http://hz.fengsongda.top/gtxvtwtnfh.html

SELECT id, name FROM users;
来源：http://hz.gaohongyu789.top/gttzonvpux.html

[Q17] 条件查询
来源：http://hz.yueranfly.top/gtthnnsbcc.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.haohaochexian.top/gtazqwpcjk.html

[Q18] 模糊匹配
来源：http://hz.xylfe.cn/gtgzdaqqiy.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.xinyue.icu/gtaefwzjmo.html

[Q19] 范围查询
来源：http://hz.hammf.cn/gtexngohit.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.jinqigfzy.top/gtcpqtjzee.html

[Q20] IN 列表
来源：http://hz.c1oappe.top/gtixocszfa.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.ybcxt.top/gtivldhsva.html

[Q21] 空值判断
来源：http://hz.nwbrower.top/gtoclllerl.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.tianlin.xyz/gtzynlxzuo.html

[Q22] 排序
来源：http://hz.gzhubu.top/gtyfxihqbg.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.ehwqpu.com/gtohqisnzg.html

[Q23] 分页
来源：http://hz.yanxiufei.cn/gtnitadsif.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.wangdashe.top/gtubgmirnk.html

[Q24] 去重
来源：http://hz.zhaomingkeji.xyz/gtpsmtflvn.html

SELECT DISTINCT city FROM users;
来源：http://hz.guowangkeji.top/gtimsznpxv.html

[Q25] 只取前 N 条
来源：http://hz.redwolf501.top/gtsufpzibb.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.feifeiyinyue.top/gtevymomyw.html

[Q26] 计数
来源：http://hz.hnxiangtu.top/gtgwrsmmab.html

SELECT COUNT(*) FROM users;
来源：http://hz.shanyushiyangtech.top/gtlfxilgvc.html

[Q27] 条件计数
来源：http://hz.sweek.top/gthckzlses.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.yj20258888.top/gtmsfwkuil.html

[Q28] 求和与平均
来源：http://hz.shzxlz.cn/gtdjzdffzh.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.hysaishi.cn/gtgyfilcdl.html

[Q29] 最大最小值
来源：http://hz.tanke756.top/gtrshorzss.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.aizwys.cn/gtdmuggkar.html

[Q30] 分组统计
来源：http://hz.shangyingyoupin.top/gtoygnqdwa.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.cqqwz.cn/gthxueheqd.html

[Q31] 分组后过滤
来源：http://hz.sysykeji.top/gtlncuqbie.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.dashuyun.cn/gtpclrgbrq.html

[Q32] 分组拼接字符串
来源：http://hz.daxiang520.top/gtmfkblkmu.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.jinyuanbaomall.cn/gteogglbrf.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.chenjidiqi.icu/gtmoqqrbmc.html

[Q33] 多列分组
来源：http://hz.yanxiufei.cn/gtskivhlim.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.xuetiantiany.cn/gtnbygczok.html

[Q34] 每组取第一条
来源：http://hz.yongpay.top/gtsdaxwdmu.html

SELECT * FROM (
来源：http://hz.zhaomingkeji.xyz/gtahrphtvt.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.0kj1m.cn/gtvlqqlink.html

) t WHERE rn = 1;
来源：http://hz.iojbl.cn/gtvpgprdam.html

[Q35] 内连接
来源：http://hz.ivvv.top/gtdvnlhkfu.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.chenjidiqi.icu/gtqnjqyyfa.html

[Q36] 左连接
来源：http://hz.tian-w.cn/gtldehimjo.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.yangfankeji.com/gtkvampksv.html

[Q37] 右连接
来源：http://hz.redwolf501.top/gtndgdeutc.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.shuidangran.top/gtagbdmqal.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.yj20258888.top/gtztxkbxqd.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.yvedp.cn/gteedhmdkx.html

[Q39] 自连接（查上下级）
来源：http://hz.feifeiyinyue.top/gtpaojieti.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.yj20258.top/gtkxvzzmiq.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.jinghuilouyu.cn/gtqjfjqzru.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.nanxuanxn.top/gthltfbokd.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.chenzaomai.com/gtlepbdapj.html

[Q41] 多表连接
来源：http://hz.gotoacloud.top/gtrjtbkthm.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.guannengcc.top/gtanzufzoy.html

JOIN users u ON u.id = o.user_id
来源：http://hz.zhaomingkeji.xyz/gtccbnylfx.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.pycfn.com/gtxyufifui.html

[Q42] 连接条件附加过滤
来源：http://hz.zhiwuduotai.top/gtezxfkwni.html

SELECT u.name, o.amount FROM users u
来源：http://hz.daxiang520.top/gtfljzscgn.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.jinqigfzy.top/gteakddmuj.html

[Q43] 标量子查询
来源：http://hz.gzhubu.top/gtrvifyqgr.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.316326.xyz/gtljidaari.html

[Q44] IN 子查询
来源：http://hz.yj20258.top/gtcfzwhpld.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.hammf.cn/gtuzophpgw.html

[Q45] EXISTS 判断存在
来源：http://hz.yongpay.top/gtlrkhiifv.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.xuanzx.com/gtltxfsdbs.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.gogol.net.cn/gthofbxkjl.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.fzhhl.top/gtvohjfeqo.html

[Q47] 与平均值比较
来源：http://hz.zhiwuduotai.top/gtkdoezpmi.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.cheryme.top/gthbfdgcwz.html

[Q48] CTE 公用表表达式
来源：http://hz.0kj1m.cn/gtfyqbxobq.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.jinqigufen.top/gtrmweatzc.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.snrcjt.cn/gtxiqitbfz.html

[Q49] 更新单行
来源：http://hz.yanxiufei.cn/gthiqeruuo.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.jlsjyb.cn/gtgxhescun.html

[Q50] 批量更新
来源：http://hz.sufxvd.cn/gtuuqsnxpt.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.yj20258.top/gtzigywyev.html

[Q51] 用子查询更新
来源：http://hz.guannengcc.top/gtxxrychbw.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.yongpay.top/gtktaeumyb.html

[Q52] 删除指定行
来源：http://hz.xuetiantiany.cn/gtiobkqwio.html

DELETE FROM users WHERE id = 10;
来源：http://hz.aizwys.cn/gthnpzmerq.html

[Q53] 按条件删除
来源：http://hz.yj20258.top/gtvdpneamo.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.hammf.cn/gtsviykjyq.html

[Q54] 清空表
来源：http://hz.meibo888.top/gtwcagcdnz.html

TRUNCATE TABLE logs;
来源：http://hz.shanyushiyangkeji.top/gtrqudjnbs.html

[Q55] 排名（并列占位）
来源：http://hz.jinyuanbaomall.cn/gtecihjoks.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.mhx1999.top/gtpdqgyafl.html

[Q56] 密集排名（并列不占位）
来源：http://hz.hywenlv.cn/gtcxwganrt.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.dianchejie.cn/gtqbznukkr.html

[Q57] 行号
来源：http://hz.xuanzx.com/gtutgfkidf.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.gaohongyu789.top/gtytxxrksi.html

[Q58] 累计求和
来源：http://hz.cheryme.top/gtobjzwnkk.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.svipenyu.cn/gtewcrkszx.html

[Q59] 分组内累计
来源：http://hz.52xcode.cn/gtxtqmsgbl.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.andypj.xyz/gtcpqphuam.html

[Q60] 取上一行 / 下一行
来源：http://hz.xuanzx.com/gtnebfuqwx.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.cqqwz.cn/gtkfmhkxhy.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.fzhhl.top/gtyhgtrmqk.html

[Q61] 移动平均
来源：http://hz.ivvv.top/gtsdldwfys.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.cdnleiting.top/gtdddfkxyo.html

[Q62] 分组占比
来源：http://hz.ppjwa.cn/gtxtxnqizh.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.yongpay.top/gtnjjykrub.html

[Q63] 开启事务
来源：http://hz.ivvv.top/gturnhkxsj.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.ivvv.top/gtrpkvmaxo.html

[Q64] 提交事务
来源：http://hz.ydjk.org.cn/gtwaqhugtw.html

COMMIT;
来源：http://hz.aizwys.cn/gtmfkktrme.html

[Q65] 回滚事务
来源：http://hz.shangyingyoupin.top/gtwygjvylm.html

ROLLBACK;
来源：http://hz.ppjwa.cn/gtysvdvmav.html

[Q66] 行锁查询
来源：http://hz.chenlongwang.top/gtccdeixvf.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.zycfv.cn/gtynaushoh.html

[Q67] 设置隔离级别
来源：http://hz.tanke756.top/gtvdtdeuei.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.shangyingyoupin.top/gtqcbsmacw.html

[Q68] 保存点
来源：http://hz.ydzc1.top/gtjsfxhnvo.html

SAVEPOINT sp1;
来源：http://hz.c1oappe.top/gtaojvhxzg.html

ROLLBACK TO sp1;
来源：http://hz.chenlongwang.top/gtqlnlevep.html

[Q69] 查看执行计划
来源：http://hz.zhongyouzk.top/gtrcznwdiv.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.xylfe.cn/gtjoidxgtb.html

[Q70] 更新统计信息
来源：http://hz.redwolf501.top/gtoavootgl.html

ANALYZE TABLE users;
来源：http://hz.fengsongda.top/gticfliltq.html

[Q71] 查看建表语句
来源：http://hz.yj20258.top/gtajqhmhki.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.yongpay.top/gtvttstqqk.html

[Q72] 查看索引
来源：http://hz.jiagoushi.top/gtandzetfa.html

SHOW INDEX FROM users;
来源：http://hz.316326.xyz/gttfvazgyv.html

[Q73] 查看表状态
来源：http://hz.andypj.xyz/gtuyzyqgfd.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.yj20258.top/gtvcfndean.html

[Q74] 强制使用索引
来源：http://hz.andypj.xyz/gtapxawgyl.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.dashuyun.cn/gtommdcdie.html

[Q75] 日期格式化
来源：http://hz.jinqigfzy.top/gtzghzqutj.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.vqdsnc.cn/gtnhqgwdtf.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.0kj1m.cn/gtjjwinrqb.html

[Q76] 按天统计
来源：http://hz.aibaodan.cn/gtadkqxnjn.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.tianlin.xyz/gtejkaudts.html

[Q77] 时间加减
来源：http://hz.jinyuanbaomall.cn/gtncbnwsui.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.hnxiangtu.top/gtotpsdjfr.html

[Q78] 当前时间
来源：http://hz.haohaochexian.top/gtqcgsenln.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.zhiwuduotai.top/gtvwqvkenu.html

[Q79] 字符串拼接
来源：http://hz.meibo888.top/gtxonlyzki.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.ivvv.top/gtxwkxdtmz.html

[Q80] 字符串截取
来源：http://hz.redwolf501.top/gtjsiygghn.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.smart0.xyz/gtzlaiierg.html

[Q81] 字符串替换
来源：http://hz.xingfuxueyuan.xyz/gtcgzgrmzf.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.chenzaomai.com/gtesbkbfvb.html

[Q82] 字符长度与字节长度
来源：http://hz.birdmap.top/gtybfwvmpm.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.zdqjudy.top/gtcxzewfhb.html

[Q83] 大小写转换
来源：http://hz.hywenlv.cn/gtbxfijkjt.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.xuetiantiany.cn/gtzdxrdmfs.html

[Q84] 去除首尾空格
来源：http://hz.ydjk.org.cn/gtrfujphzv.html

SELECT TRIM(name) FROM users;
来源：http://hz.sxryk.cn/gtppwbxmsx.html

[Q85] 数值取整
来源：http://hz.0kj1m.cn/gtkzukmksf.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.yanxiufei.cn/gtltkbeswd.html

[Q86] 读取 JSON 字段
来源：http://hz.quarkkingdee.top/gtjlfzflbf.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.xuetiantiany.cn/gtcswvrmtm.html

[Q87] JSON 字段做条件
来源：http://hz.yj202588.top/gtnhwyrali.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.jqgufenzy.top/gttqffiyjn.html

[Q88] 行转列（条件聚合）
来源：http://hz.ydjk.org.cn/gtvctzhnas.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.jiagoushi.top/gtvozdptco.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.chenzaomai.com/gtnnsyizvf.html

[Q89] 判断表是否存在
来源：http://hz.shzxlz.cn/gtlkfmetih.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.redwolf501.top/gtfylzrlhk.html

[Q90] 生成序号列
来源：http://hz.cqqwz.cn/gtejvpbrbp.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.xziqi.cn/gtggczjovl.html

================================================================================
来源：http://hz.nanxinkj.top/gttzugpwqt.html

R. Bash 专题
来源：http://hz.jlsjyb.cn/gtsiqtrjvl.html

================================================================================
来源：http://hz.jqgfzy.top/gtxszyrekb.html

[R01] shebang 与严格模式
来源：http://hz.zhengqikj.top/gtqwaeaokm.html

#!/usr/bin/env bash
来源：http://hz.ywan-chungtsiang.top/gtyllhuerv.html

set -euo pipefail
来源：http://hz.yj20258.top/gtfsakzdtv.html

[R02] 变量赋值与使用
来源：http://hz.ivvv.top/gtzkjprrlg.html

name="Tom"; echo "$name"
来源：http://hz.pycfn.com/gtculbbjtc.html

[R03] 只读变量
来源：http://hz.snrcjt.cn/gtwqiiqlmq.html

readonly PI=3.14
来源：http://hz.pycfn.com/gtatzqbrsq.html

[R04] 位置参数
来源：http://hz.gotoacloud.top/gteveotccu.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.jinghuilouyu.cn/gtlknoptjs.html

[R05] 参数默认值
来源：http://hz.redwolf501.top/gtqpblmsne.html

name="${1:-default}"
来源：http://hz.zhixingplan.top/gtwrezbwbq.html

[R06] 判断命令是否存在
来源：http://hz.guannengcc.top/gtbxswtfmb.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.yuanzhike.top/gtrlrennwb.html

[R07] if 判断文件
来源：http://hz.sxryk.cn/gtbmvfxmry.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.andypj.xyz/gtyzybgajf.html

[R08] 数值比较
来源：http://hz.yongpay.top/gthghpfhom.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.dashuyun.cn/gtlfjfnanb.html

[R09] 字符串比较
来源：http://hz.aizwys.cn/gtzxexnhgm.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.jinyuanbaomall.cn/gtnxggldcx.html

[R10] 正则匹配
来源：http://hz.guowangkeji.top/gtvujihbya.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.fzhhl.top/gtmnccqpsy.html

[R11] case 多分支
来源：http://hz.jinqigufen.top/gtrbmmfxpw.html

case "$1" in
来源：http://hz.9152youxi.cn/gtqaimlzaw.html

start) echo "启动" ;;
来源：http://hz.feifeiyinyue.top/gtuyftmmjx.html

stop)  echo "停止" ;;
来源：http://hz.gzhubu.top/gtbtfyqibe.html

*)     echo "未知命令" ;;
来源：http://hz.quarkkingdee.top/gtmwsdibun.html

esac
来源：http://hz.xylfe.cn/gtrtzgphth.html

[R12] for 遍历文件
来源：http://hz.ybcxt.top/gtfwnddhog.html

for f in *.txt; do echo "$f"; done
来源：http://hz.cucudq.cn/gtijbacczs.html

[R13] for 计数循环
来源：http://hz.birdmap.top/gtvysjdkog.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.tian-w.cn/gtxvxvtgyf.html

[R14] C 风格 for
来源：http://hz.xziqi.cn/gtcyzkdqas.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.ywan-chungtsiang.top/gtmxfoxqhz.html

[R15] while 逐行读文件
来源：http://hz.hywenlv.cn/gtmrccfqzm.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.mhx1999.top/gtvwpmdytr.html

[R16] until 等待条件
来源：http://hz.gzhubu.top/gtsjyibgyg.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.hysaishi.cn/gtccygylot.html

[R17] 数组定义与取值
来源：http://hz.cheryme.top/gttmwerwle.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.316326.xyz/gtlhpwqeas.html

[R18] 遍历数组
来源：http://hz.chenzaomai.com/gtyetmitwi.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.birdmap.top/gtwmdikuob.html

[R19] 数组长度
来源：http://hz.redwolf501.top/gtrkdpwzdf.html

echo "${#arr[@]}"
来源：http://hz.hywenlv.cn/gtkwnbrfsx.html

[R20] 关联数组（字典）
来源：http://hz.nanxuanxn.top/gtsavsffvh.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.yvedp.cn/gtoigrtcgp.html

[R21] 字符串长度
来源：http://hz.xuetiantiany.cn/gtwqthypoy.html

echo "${#s}"
来源：http://hz.shzxlz.cn/gtjzrwxuoj.html

[R22] 截取子串
来源：http://hz.gaohongyu789.top/gthxggplik.html

echo "${s:0:5}"
来源：http://hz.jlsjyb.cn/gtwcrimvjx.html

[R23] 字符串替换
来源：http://hz.zhixingplan.top/gtlmyahhmw.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.jyoumei.cn/gtowbsfddr.html

[R24] 大小写转换
来源：http://hz.fengsongda.top/gtlxofympj.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.daria6918.cn/gtslzamnzm.html

[R25] 去后缀 / 去前缀
来源：http://hz.shuidangran.top/gtjzryrhft.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.nwbrower.top/gtkykxmhqu.html

[R26] 命令替换
来源：http://hz.jqgfzy.top/gtnoypqpxx.html

now=$(date +%F); echo "$now"
来源：http://hz.shangyingyoupin.top/gtnmabyxzf.html

[R27] 算术展开
来源：http://hz.daria6918.cn/gtqdwawjsc.html

echo $((1 + 2 * 3))
来源：http://hz.xinyue.icu/gtklyflakz.html

[R28] 浮点运算
来源：http://hz.iojbl.cn/gteholbxqg.html

echo "scale=2; 10/3" | bc
来源：http://hz.dianchejie.cn/gtwzztjluy.html

[R29] 定义函数
来源：http://hz.shanyushiyangkeji.top/gtwtbfgrez.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.xinyue.icu/gtfwbenrjo.html

[R30] 函数返回状态码
来源：http://hz.bjfxy.top/gtqdixdprq.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.daria6918.cn/gtmqqbrxoa.html

[R31] 局部变量
来源：http://hz.yuanzhike.top/gtvljirmnz.html

f() { local x=1; echo "$x"; }
来源：http://hz.snrcjt.cn/gtpuvyjwye.html

[R32] 参数个数校验
来源：http://hz.gogol.net.cn/gtbdljxjip.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.guannengcc.top/gtpdinifin.html

[R33] 捕获错误并提示行号
来源：http://hz.hnqzz.top/gtesvqpjpr.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.nanxinkj.top/gtofchdrki.html

[R34] 退出时清理
来源：http://hz.shanyushiyangtech.top/gterrejtsp.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.shanyushiyangtech.top/gtphhmgvjh.html

[R35] 后台执行并等待
来源：http://hz.cucudq.cn/gtroselxvv.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.cashguo.top/gtiozhyzmm.html

[R36] 并发执行多个任务
来源：http://hz.daxiang520.top/gtmceumjvk.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.hysaishi.cn/gtahgrpsyw.html

[R37] 把输出赋给变量
来源：http://hz.52xcode.cn/gtbvwsdehm.html


<!-- 参考信息 -->