代发 wailian999

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.vqdsnc.cn/gtvsdkgpoe.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.dashuyun.cn/gtjpucpcci.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.quarkkingdee.top/gtvcdriqkr.html

Ruby: a == b
来源：http://hz.guowangkeji.top/gtmtflavks.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.yongpay.top/gtqrjnyool.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.dianchejie.cn/gtedtypewb.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.jqgfzy.top/gtummgaslk.html

PHP:  if (empty($x)) {}
来源：http://hz.jinghuilouyu.cn/gthkngikhl.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.chenzaomai.com/gtipppdpzu.html

TS:   if (x == null) {}
来源：http://hz.feifeiyinyue.top/gthhmpxlzc.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.jinqigfzy.top/gtltrnyenu.html

Go:   if x == nil {}
来源：http://hz.cqqwz.cn/gtrdgtjeqb.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.9152youxi.cn/gttpqchngy.html

C#:   if (x is null) {}
来源：http://hz.sweek.top/gtovredzaj.html

[P07] 防抖与节流
来源：http://hz.pycfn.com/gtbfxcllov.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.gotoacloud.top/gtxywvfeqw.html

PHP:  // 手写时间戳比较
来源：http://hz.cqqwz.cn/gtljlpuvgd.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.aibaodan.cn/gtzcowktnc.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.cashguo.top/gtxatwklzf.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.tian-w.cn/gtlmbmoous.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.jqgufenzy.top/gtfuypaopp.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.yj20258.top/gtwebrcvde.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.sufxvd.cn/gttpzhzstn.html

[P08] 处理浮点精度问题
来源：http://hz.jinghuilouyu.cn/gtdvyaudod.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.hywenlv.cn/gtmxqvcgos.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.feifeiyinyue.top/gtwajdjxpx.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.mhx1999.top/gtqhjzdwwr.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.fzhhl.top/gtpponcwbn.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.xuanzx.com/gtcycerbif.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.gaohongyu789.top/gtiynbvnuy.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.smart0.xyz/gtixrduiie.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.jlsjyb.cn/gtjmipgomt.html

================================================================================
来源：http://hz.smart0.xyz/gtneeolbbj.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.0kj1m.cn/gtprseugxt.html

================================================================================
来源：http://hz.gotoacloud.top/gtgjpdbcke.html

[Q01] 创建表
来源：http://hz.dashuyun.cn/gtjctmqrjp.html

CREATE TABLE users (
来源：http://hz.zhaomingkeji.xyz/gtbzfirrpi.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jinqigfzy.top/gtmrbtywqv.html

name VARCHAR(50) NOT NULL,
来源：http://hz.iojbl.cn/gtklizlpau.html

email VARCHAR(100) UNIQUE,
来源：http://hz.xylfe.cn/gtoagfmzeg.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.haohaochexian.top/gtapxrwutp.html

);
来源：http://hz.jinghuilouyu.cn/gtqazisxfz.html

[Q02] 创建带外键的表
来源：http://hz.vqdsnc.cn/gtgswqador.html

CREATE TABLE orders (
来源：http://hz.mhx1999.top/gtgohiohrl.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.hnxiangtu.top/gtzqmwogbn.html

user_id INT NOT NULL,
来源：http://hz.xylfe.cn/gtoawohsyv.html

amount DECIMAL(10, 2),
来源：http://hz.zhiwuduotai.top/gtxrssrigw.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.snrcjt.cn/gtqeprysjt.html

);
来源：http://hz.cashguo.top/gtzqifkjiv.html

[Q03] 增加列
来源：http://hz.gogol.net.cn/gttaesisuw.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.yj20258.top/gtwrabbiky.html

[Q04] 修改列类型
来源：http://hz.ywan-chungtsiang.top/gtlmhnyisi.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.tianlin.xyz/gtarabwyht.html

[Q05] 重命名列
来源：http://hz.yongpay.top/gtcptwuvzz.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.hongshengwenyu.top/gtwrqjssfb.html

[Q06] 删除列
来源：http://hz.zdqjudy.top/gtsogbwfrn.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.vqdsnc.cn/gthjjhuhpa.html

[Q07] 删除表
来源：http://hz.snrcjt.cn/gteacybmsw.html

DROP TABLE IF EXISTS orders;
来源：http://hz.cdnleiting.top/gtzfmqhraf.html

[Q08] 创建普通索引
来源：http://hz.havefunace.top/gtknqhhgqa.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.jlsjyb.cn/gtkrjjacto.html

[Q09] 创建唯一索引
来源：http://hz.sufxvd.cn/gtfoktgpwv.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.yuxming.cn/gtcufnmorl.html

[Q10] 插入单行
来源：http://hz.hywenlv.cn/gtrlkkrgju.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.fzhhl.top/gtnjwrsdhx.html

[Q11] 一次插入多行
来源：http://hz.hysaishi.cn/gtopdjpggf.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.xziqi.cn/gtznmlvbpd.html

[Q12] 插入后取自增 ID
来源：http://hz.sxryk.cn/gtutovjrjd.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.zhixingplan.top/gtalpfiykm.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.xuanzx.com/gtrxkwzmtm.html

[Q13] 忽略重复插入
来源：http://hz.zhiwuduotai.top/gtrzbhmqun.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.316326.xyz/gtmueqsuzt.html

[Q14] 存在则更新（upsert）
来源：http://hz.jlsjyb.cn/gtrvlefosb.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.mhx1999.top/gtehghripo.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.redwolf501.top/gtdegdpbqf.html

[Q15] 查询全部
来源：http://hz.jinqigufen.top/gteelmnmue.html

SELECT * FROM users;
来源：http://hz.pengpengdd.cyou/gtfjctjfjr.html

[Q16] 查询指定列
来源：http://hz.hnqzz.top/gttzthxuds.html

SELECT id, name FROM users;
来源：http://hz.aizwys.cn/gteamgqxxj.html

[Q17] 条件查询
来源：http://hz.gogol.net.cn/gtaxtrgxai.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.mhx1999.top/gtrapkwgcq.html

[Q18] 模糊匹配
来源：http://hz.wangdashe.top/gtydrndtnh.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.yj202588.top/gtlkbtxlax.html

[Q19] 范围查询
来源：http://hz.dashuyun.cn/gtwxoxwoil.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.xziqi.cn/gtkwhjvbht.html

[Q20] IN 列表
来源：http://hz.jianghu66.top/gtdtwcleec.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.snrcjt.cn/gtyuiyjjqb.html

[Q21] 空值判断
来源：http://hz.zhiwuduotai.top/gteoymyfxi.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.cheryme.top/gtnqsjbnst.html

[Q22] 排序
来源：http://hz.smart0.xyz/gthrqdlxwu.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.smart0.xyz/gtubkkvszm.html

[Q23] 分页
来源：http://hz.yj20258888.top/gtlmveheos.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.zhijiandao.cn/gtfstyawhq.html

[Q24] 去重
来源：http://hz.chenzaomai.com/gtfzfoyvcy.html

SELECT DISTINCT city FROM users;
来源：http://hz.yvedp.cn/gtbbtjtplv.html

[Q25] 只取前 N 条
来源：http://hz.gzhubu.top/gtxgesklhp.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.cheryme.top/gtsjzisxwt.html

[Q26] 计数
来源：http://hz.quarkkingdee.top/gtlvijxruo.html

SELECT COUNT(*) FROM users;
来源：http://hz.gaohongyu789.top/gtleappybw.html

[Q27] 条件计数
来源：http://hz.meibo888.top/gtsbwcoosw.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.yuxming.cn/gtyydbczrv.html

[Q28] 求和与平均
来源：http://hz.chenjidiqi.icu/gtoumhzwiz.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.316326.xyz/gtqmytkgxs.html

[Q29] 最大最小值
来源：http://hz.redwolf501.top/gtfkzwbysi.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.zhaomingkeji.xyz/gtserjezqc.html

[Q30] 分组统计
来源：http://hz.jinqigufen.top/gtwcguodze.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.ybcxt.top/gtgklljbgk.html

[Q31] 分组后过滤
来源：http://hz.svipenyu.cn/gtdlhcryxf.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.ydzc1.top/gtfsuxojxi.html

[Q32] 分组拼接字符串
来源：http://hz.9152youxi.cn/gtntonuqef.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.cucudq.cn/gtykrtlzfm.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.gogol.net.cn/gtmdjqdyaj.html

[Q33] 多列分组
来源：http://hz.jinyuanbaomall.cn/gtdmcmozaf.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.zycfv.cn/gtmeidxrjp.html

[Q34] 每组取第一条
来源：http://hz.tianlin.xyz/gtyxgatkub.html

SELECT * FROM (
来源：http://hz.chenjidiqi.icu/gtthfwvffo.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.hywenlv.cn/gtibllwzoz.html

) t WHERE rn = 1;
来源：http://hz.tian-w.cn/gtjysjptlc.html

[Q35] 内连接
来源：http://hz.jiagoushi.top/gtxmxqpkac.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.chenlongwang.top/gtecxaoggk.html

[Q36] 左连接
来源：http://hz.gzhubu.top/gtulivblcd.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.redwolf501.top/gtgyidezps.html

[Q37] 右连接
来源：http://hz.yj20258888.top/gtadgjowto.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.pycfn.com/gtunucfrak.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.jinghuilouyu.cn/gtyhewjakg.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.yuxming.cn/gttmqnvszk.html

[Q39] 自连接（查上下级）
来源：http://hz.zhixingplan.top/gtuaxujeej.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.yj20258888.top/gtxeqzqzip.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.guannengcc.top/gtqldymxcq.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.chenjidiqi.icu/gtroapdhax.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.dianchejie.cn/gtpasmxttv.html

[Q41] 多表连接
来源：http://hz.hnqzz.top/gtwxwxmtni.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.yanxiufei.cn/gtkbytrvlk.html

JOIN users u ON u.id = o.user_id
来源：http://hz.cucudq.cn/gteignlbuc.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.shanyushiyangtech.top/gtlrqvwqvq.html

[Q42] 连接条件附加过滤
来源：http://hz.dianchejie.cn/gtnzeonike.html

SELECT u.name, o.amount FROM users u
来源：http://hz.jiagoushi.top/gtdawizlrb.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.zhiwuduotai.top/gtjihxfoai.html

[Q43] 标量子查询
来源：http://hz.shuidangran.top/gtobjuldzp.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.tian-w.cn/gtuffqitnn.html

[Q44] IN 子查询
来源：http://hz.daxiang520.top/gtyffjacpj.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.smart0.xyz/gttbrbdiny.html

[Q45] EXISTS 判断存在
来源：http://hz.sweek.top/gtgzuguovf.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.sysykeji.top/gtjdqihwmg.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.haohaochexian.top/gtzrtmrdkh.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.xinyue.icu/gtcqtghozi.html

[Q47] 与平均值比较
来源：http://hz.redwolf501.top/gtskxwwzqx.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.52xcode.cn/gtgppxnnzq.html

[Q48] CTE 公用表表达式
来源：http://hz.c1oappe.top/gtsepqmxrk.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.ivvv.top/gtascrgljo.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.ivvv.top/gtievkkadp.html

[Q49] 更新单行
来源：http://hz.yj202588.top/gtbisyqgil.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.zycfv.cn/gtojbdaeky.html

[Q50] 批量更新
来源：http://hz.andypj.xyz/gttlniqnnt.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.wangdashe.top/gteyjklsij.html

[Q51] 用子查询更新
来源：http://hz.cheryme.top/gtmfxnsixl.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.haohaochexian.top/gtcrutxpwu.html

[Q52] 删除指定行
来源：http://hz.tian-w.cn/gtbutrpfew.html

DELETE FROM users WHERE id = 10;
来源：http://hz.sysykeji.top/gthopvwapi.html

[Q53] 按条件删除
来源：http://hz.havefunace.top/gtdxjqfcxh.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.9152youxi.cn/gtfvvzuqwk.html

[Q54] 清空表
来源：http://hz.svipenyu.cn/gtqwvotrwr.html

TRUNCATE TABLE logs;
来源：http://hz.yvedp.cn/gtiarajamb.html

[Q55] 排名（并列占位）
来源：http://hz.fengsongda.top/gtatbasdbr.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.iojbl.cn/gtmfgvzulx.html

[Q56] 密集排名（并列不占位）
来源：http://hz.wangshuangyany.cn/gtmnmqcnfg.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.zhoulong.xyz/gtsanwhkte.html

[Q57] 行号
来源：http://hz.shanyushiyangkeji.top/gtmueulfnz.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.xuetiantiany.cn/gtgzsnrzqt.html

[Q58] 累计求和
来源：http://hz.yj20258.top/gtjhxmored.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.cdnleiting.top/gthblylxzk.html

[Q59] 分组内累计
来源：http://hz.wangdashe.top/gtmjkezogp.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.xuanzx.com/gtwokbouhw.html

[Q60] 取上一行 / 下一行
来源：http://hz.ydjk.org.cn/gtbbdavpcc.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.hfpthk.cn/gteameuvqy.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.shzxlz.cn/gtpcyixnmx.html

[Q61] 移动平均
来源：http://hz.zycfv.cn/gtgzsvqgjc.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.aibaodan.cn/gtdyphxptl.html

[Q62] 分组占比
来源：http://hz.redwolf501.top/gtbbmbxpfz.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.316326.xyz/gtgyiqvzmx.html

[Q63] 开启事务
来源：http://hz.daria6918.cn/gtilcskevl.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.52xcode.cn/gteguvtxzw.html

[Q64] 提交事务
来源：http://hz.jinqigfzy.top/gtfvrgimme.html

COMMIT;
来源：http://hz.xziqi.cn/gtegcxqfsp.html

[Q65] 回滚事务
来源：http://hz.sweek.top/gtlccyyxgo.html

ROLLBACK;
来源：http://hz.zdqjudy.top/gthcjvvich.html

[Q66] 行锁查询
来源：http://hz.hnqzz.top/gtegjknqib.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.jqgufenzy.top/gtaisgiqrq.html

[Q67] 设置隔离级别
来源：http://hz.tanke756.top/gtexhoifuq.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.shangyingyoupin.top/gtzsoimzzq.html

[Q68] 保存点
来源：http://hz.shzxlz.cn/gtnhsxugnr.html

SAVEPOINT sp1;
来源：http://hz.xziqi.cn/gtodtsdflz.html

ROLLBACK TO sp1;
来源：http://hz.gaohongyu789.top/gtsmtlyiuz.html

[Q69] 查看执行计划
来源：http://hz.yueranfly.top/gtkvhyluxq.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.hfpthk.cn/gtitsthxqx.html

[Q70] 更新统计信息
来源：http://hz.dianchejie.cn/gtfjlxljzx.html

ANALYZE TABLE users;
来源：http://hz.zhijiandao.cn/gtzdimtalg.html

[Q71] 查看建表语句
来源：http://hz.sufxvd.cn/gthlzviwaj.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.ivvv.top/gtdhivbaxb.html

[Q72] 查看索引
来源：http://hz.aibaodan.cn/gttzeegdpw.html

SHOW INDEX FROM users;
来源：http://hz.xingfuxueyuan.xyz/gtcstsrgqm.html

[Q73] 查看表状态
来源：http://hz.yj20258.top/gtvitzcxcm.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.dashuyun.cn/gtkojirzzo.html

[Q74] 强制使用索引
来源：http://hz.daxiang520.top/gtzgmiipbu.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.hongshengwenyu.top/gtpihdnqhu.html

[Q75] 日期格式化
来源：http://hz.shanyushiyangkeji.top/gtxyixzqwx.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.pengpengdd.cyou/gtfchlvttx.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.nanxinkj.top/gtrnhfctlf.html

[Q76] 按天统计
来源：http://hz.yanxiufei.cn/gtszojavwn.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.tanke756.top/gtsiupbsry.html

[Q77] 时间加减
来源：http://hz.dianchejie.cn/gtobxbluwi.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.nanxinkj.top/gtvnzmdxhv.html

[Q78] 当前时间
来源：http://hz.smart0.xyz/gtmkmceqqw.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.andypj.xyz/gttdraeyjm.html

[Q79] 字符串拼接
来源：http://hz.cdnleiting.top/gtsvyfzfli.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.nwbrower.top/gtabfexfqx.html

[Q80] 字符串截取
来源：http://hz.jiagoushi.top/gtmejzuqul.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.chenjidiqi.icu/gtevokgkpi.html

[Q81] 字符串替换
来源：http://hz.sweek.top/gtroxttjaj.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.hnxiangtu.top/gtfhxznvxy.html

[Q82] 字符长度与字节长度
来源：http://hz.hysaishi.cn/gtqroebghw.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.chenzaomai.com/gtxmffmqre.html

[Q83] 大小写转换
来源：http://hz.xuanzx.com/gtcxrhixho.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.sufxvd.cn/gtyfhqbqac.html

[Q84] 去除首尾空格
来源：http://hz.ppjwa.cn/gtdqxqugmm.html

SELECT TRIM(name) FROM users;
来源：http://hz.svipenyu.cn/gtrnhltfwq.html

[Q85] 数值取整
来源：http://hz.xuetiantiany.cn/gtuzqymdlx.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.zycfv.cn/gtukqxmzmo.html

[Q86] 读取 JSON 字段
来源：http://hz.hfpthk.cn/gtvrmptbca.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.jqgfzy.top/gtezeorfuj.html

[Q87] JSON 字段做条件
来源：http://hz.nanxuanxn.top/gtcofsdrtz.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.zhijiandao.cn/gtzpvrafur.html

[Q88] 行转列（条件聚合）
来源：http://hz.zhiwuduotai.top/gtbhtvtcml.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.zhiwuduotai.top/gtwnkitibt.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.yvedp.cn/gtfosuczou.html

[Q89] 判断表是否存在
来源：http://hz.yonumen.top/gtbgyznwfb.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.jiagoushi.top/gtcixkbuif.html

[Q90] 生成序号列
来源：http://hz.fengsongda.top/gtmrzmcybl.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.shangyingyoupin.top/gtwydguxzt.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtvfktqjen.html

R. Bash 专题
来源：http://hz.chenjidiqi.icu/gtvmwwtgot.html

================================================================================
来源：http://hz.ydjk.org.cn/gtbqhgdokw.html

[R01] shebang 与严格模式
来源：http://hz.zhixingplan.top/gtxlilkgzs.html

#!/usr/bin/env bash
来源：http://hz.cdnleiting.top/gtouocmgvz.html

set -euo pipefail
来源：http://hz.vqdsnc.cn/gtvkdhuotq.html

[R02] 变量赋值与使用
来源：http://hz.jqgufenzy.top/gtkcjsqgsl.html

name="Tom"; echo "$name"
来源：http://hz.jinqigfzy.top/gtgiawuxtg.html

[R03] 只读变量
来源：http://hz.jyoumei.cn/gtnotdngjz.html

readonly PI=3.14
来源：http://hz.cucudq.cn/gtnezehgqu.html

[R04] 位置参数
来源：http://hz.kuanghao11.cn/gtndunjhgg.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.cheryme.top/gtswqfuznu.html

[R05] 参数默认值
来源：http://hz.zhijiandao.cn/gtwlhvespo.html

name="${1:-default}"
来源：http://hz.jinyuanbaomall.cn/gtowlyglpu.html

[R06] 判断命令是否存在
来源：http://hz.hammf.cn/gtqtnklnff.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.hywenlv.cn/gtychthlec.html

[R07] if 判断文件
来源：http://hz.gotoacloud.top/gtrewszndj.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.yj20258888.top/gtrykhnxro.html

[R08] 数值比较
来源：http://hz.shuidangran.top/gteycoexfm.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.zdqjudy.top/gtzwduertu.html

[R09] 字符串比较
来源：http://hz.jqgfzy.top/gtfgzpoztg.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.zhoulong.xyz/gtwrveekdk.html

[R10] 正则匹配
来源：http://hz.ydzc1.top/gtgwyxkpoy.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.gaohongyu789.top/gtzsnutkhd.html

[R11] case 多分支
来源：http://hz.aibaodan.cn/gtftyvyjco.html

case "$1" in
来源：http://hz.zhengqikj.top/gtnervvege.html

start) echo "启动" ;;
来源：http://hz.dashuyun.cn/gtzqymjtnw.html

stop)  echo "停止" ;;
来源：http://hz.guannengcc.top/gtixeyxztu.html

*)     echo "未知命令" ;;
来源：http://hz.sufxvd.cn/gtyrcumviu.html

esac
来源：http://hz.nanxinkj.top/gtcvymulsz.html

[R12] for 遍历文件
来源：http://hz.hywenlv.cn/gtypxcmsmw.html

for f in *.txt; do echo "$f"; done
来源：http://hz.chenlongwang.top/gtzesshprk.html

[R13] for 计数循环
来源：http://hz.jinyuanbaomall.cn/gtibfhjecx.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.pengpengdd.cyou/gtbawfpahj.html

[R14] C 风格 for
来源：http://hz.dashuyun.cn/gtonfishvt.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.hammf.cn/gtheecpbqm.html

[R15] while 逐行读文件
来源：http://hz.cdnleiting.top/gtnxouuxue.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.hammf.cn/gtwqedlfue.html

[R16] until 等待条件
来源：http://hz.yj20258.top/gtphldehxw.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.guannengcc.top/gtlwbivjmp.html

[R17] 数组定义与取值
来源：http://hz.0kj1m.cn/gtpckgammb.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.cashguo.top/gtwmvgjnex.html

[R18] 遍历数组
来源：http://hz.fengsongda.top/gtdxpxshxu.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.xuanzx.com/gtwejrixkm.html

[R19] 数组长度
来源：http://hz.hywenlv.cn/gtmrdrxrdw.html

echo "${#arr[@]}"
来源：http://hz.svipenyu.cn/gtomanzhip.html

[R20] 关联数组（字典）
来源：http://hz.zhoulong.xyz/gtrzxrjues.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.shangyingyoupin.top/gtizppgzrp.html

[R21] 字符串长度
来源：http://hz.0kj1m.cn/gtpvjounmb.html

echo "${#s}"
来源：http://hz.kuanghao11.cn/gtdjjpoxus.html

[R22] 截取子串
来源：http://hz.haohaochexian.top/gtqrksqall.html

echo "${s:0:5}"
来源：http://hz.sysykeji.top/gtuwxezxtj.html

[R23] 字符串替换
来源：http://hz.jianghu66.top/gttdirlibn.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.hammf.cn/gtvskfledj.html

[R24] 大小写转换
来源：http://hz.wangdashe.top/gtoegrfecw.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.0kj1m.cn/gtrtnggpfl.html

[R25] 去后缀 / 去前缀
来源：http://hz.dashuyun.cn/gtcdghqrhr.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.kuanghao11.cn/gteipcogoz.html

[R26] 命令替换
来源：http://hz.aizwys.cn/gtervldzee.html

now=$(date +%F); echo "$now"
来源：http://hz.hammf.cn/gtbmjfrnje.html

[R27] 算术展开
来源：http://hz.wangdashe.top/gtokchnbii.html


<!-- 参考信息 -->