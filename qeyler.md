代发 wailian999

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.sweek.top/gteacuwslp.html

TS:   if (x == null) {}
来源：http://hz.gzhubu.top/gtqomlecuf.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.fzhhl.top/gtsybtriqb.html

Go:   if x == nil {}
来源：http://hz.shanyushiyangtech.top/gtlgsprgak.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.chenlongwang.top/gthmsdjnty.html

C#:   if (x is null) {}
来源：http://hz.yonumen.top/gtqwqwlkas.html

[P07] 防抖与节流
来源：http://hz.sxryk.cn/gtimhagoix.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.kuanghao11.cn/gthmzmqvus.html

PHP:  // 手写时间戳比较
来源：http://hz.dashuyun.cn/gtysusuqhh.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.tanke756.top/gtaumscqjs.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zhaomingkeji.xyz/gtepkfiunq.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.shangyingyoupin.top/gtvuoyilzr.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.xylfe.cn/gtwpsozkjd.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.shzxlz.cn/gttxevmokk.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.cqqwz.cn/gtiljspujh.html

[P08] 处理浮点精度问题
来源：http://hz.ybcxt.top/gtxsucwsob.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.c1oappe.top/gtjcpyfwjy.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.havefunace.top/gtlppjgwey.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.cheryme.top/gtbixroahb.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.ywan-chungtsiang.top/gtmvotzpnp.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.ehwqpu.com/gtgxbhtkdl.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.yuanzhike.top/gtzsjbxjbb.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.jiagoushi.top/gtkbiyoima.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.havefunace.top/gtntetgzws.html

================================================================================
来源：http://hz.c1oappe.top/gtvjsligmo.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.yvedp.cn/gttcddthyg.html

================================================================================
来源：http://hz.zhengqikj.top/gtfwbxetth.html

[Q01] 创建表
来源：http://hz.shangyingyoupin.top/gtbdecthar.html

CREATE TABLE users (
来源：http://hz.jlsjyb.cn/gtvnkxopme.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.hongshengwenyu.top/gtnonzhunk.html

name VARCHAR(50) NOT NULL,
来源：http://hz.gotoacloud.top/gtoauxohxp.html

email VARCHAR(100) UNIQUE,
来源：http://hz.wangshuangyany.cn/gtachqyrzj.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.tianlin.xyz/gtzidokkbj.html

);
来源：http://hz.tanke756.top/gtntrqnwuf.html

[Q02] 创建带外键的表
来源：http://hz.hfpthk.cn/gtkkhnclxh.html

CREATE TABLE orders (
来源：http://hz.gzhubu.top/gtaqnaflkn.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.ydzc1.top/gtfxdkaghl.html

user_id INT NOT NULL,
来源：http://hz.xuanzx.com/gtzvbbbvwh.html

amount DECIMAL(10, 2),
来源：http://hz.hammf.cn/gtscbukilm.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.yuanzhike.top/gthhtrnxjf.html

);
来源：http://hz.pycfn.com/gthglwirbl.html

[Q03] 增加列
来源：http://hz.hammf.cn/gtddvnchgz.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.redwolf501.top/gtafymmpuf.html

[Q04] 修改列类型
来源：http://hz.vqdsnc.cn/gttitikjvi.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.redwolf501.top/gtsivfkyuu.html

[Q05] 重命名列
来源：http://hz.c1oappe.top/gtxczmexez.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.hnqzz.top/gtyrprriop.html

[Q06] 删除列
来源：http://hz.wangdashe.top/gtajmglvki.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.zhiwuduotai.top/gtmnumqets.html

[Q07] 删除表
来源：http://hz.zycfv.cn/gtcrovjrlv.html

DROP TABLE IF EXISTS orders;
来源：http://hz.xinyue.icu/gthshpzlja.html

[Q08] 创建普通索引
来源：http://hz.yj202588.top/gtqbnldaci.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.hfpthk.cn/gtopxsdphc.html

[Q09] 创建唯一索引
来源：http://hz.quarkkingdee.top/gtjgiuruap.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.nanxinkj.top/gtnyfmdnoq.html

[Q10] 插入单行
来源：http://hz.xylfe.cn/gtnuqhxuqs.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.zycfv.cn/gtsdnerwfk.html

[Q11] 一次插入多行
来源：http://hz.cucudq.cn/gtnyfayujn.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.zhijiandao.cn/gtiaovtmqf.html

[Q12] 插入后取自增 ID
来源：http://hz.kuanghao11.cn/gtaddokxdl.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.sweek.top/gtzojhzcks.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.ppjwa.cn/gtauvbrolq.html

[Q13] 忽略重复插入
来源：http://hz.smart0.xyz/gtwwgffhsb.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.hongshengwenyu.top/gtrsfgzieo.html

[Q14] 存在则更新（upsert）
来源：http://hz.jyoumei.cn/gtasstiwks.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.zycfv.cn/gtnnijmces.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.andypj.xyz/gtdnmelzne.html

[Q15] 查询全部
来源：http://hz.gogol.net.cn/gtdumtnjkf.html

SELECT * FROM users;
来源：http://hz.shanyushiyangtech.top/gtbbqycuxr.html

[Q16] 查询指定列
来源：http://hz.cucudq.cn/gtncecjqsz.html

SELECT id, name FROM users;
来源：http://hz.yueranfly.top/gtogblgdlx.html

[Q17] 条件查询
来源：http://hz.chenlongwang.top/gtgwuswldl.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.c1oappe.top/gthcjpfhee.html

[Q18] 模糊匹配
来源：http://hz.yongpay.top/gtiwpjhuqg.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.jianghu66.top/gtbvwwuhaj.html

[Q19] 范围查询
来源：http://hz.daria6918.cn/gthicpluzj.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.tianlin.xyz/gtzywgcecq.html

[Q20] IN 列表
来源：http://hz.xinyue.icu/gtvksfzmdk.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.0kj1m.cn/gtqcrvajuq.html

[Q21] 空值判断
来源：http://hz.ybcxt.top/gtkvuuphlw.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.cdnleiting.top/gtvnixjfpv.html

[Q22] 排序
来源：http://hz.yongpay.top/gtofsgbyks.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.yonumen.top/gtjmtkhgwy.html

[Q23] 分页
来源：http://hz.xylfe.cn/gtfqokswqe.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.jqgfzy.top/gtzahztmkp.html

[Q24] 去重
来源：http://hz.guowangkeji.top/gtavzqmueh.html

SELECT DISTINCT city FROM users;
来源：http://hz.shangyingyoupin.top/gtkyfsnzyp.html

[Q25] 只取前 N 条
来源：http://hz.yvedp.cn/gtqwfushte.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.mhx1999.top/gteezazctf.html

[Q26] 计数
来源：http://hz.haohaochexian.top/gtiacbtmuj.html

SELECT COUNT(*) FROM users;
来源：http://hz.cheryme.top/gtkhcodnwr.html

[Q27] 条件计数
来源：http://hz.zhijiandao.cn/gtyrmafgwj.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.yuxming.cn/gtnueaezbp.html

[Q28] 求和与平均
来源：http://hz.mhx1999.top/gtvlthcncr.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.sxryk.cn/gtgfnbetyk.html

[Q29] 最大最小值
来源：http://hz.yvedp.cn/gtxkbcxbkp.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.shuidangran.top/gtbponvzbe.html

[Q30] 分组统计
来源：http://hz.jqgfzy.top/gtzeeiqyzn.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.jinqigfzy.top/gtkqjkiapw.html

[Q31] 分组后过滤
来源：http://hz.dianchejie.cn/gtfptoukai.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.snrcjt.cn/gtwqkzzrkq.html

[Q32] 分组拼接字符串
来源：http://hz.daxiang520.top/gtxyoiqsrz.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.ydjk.org.cn/gtmawilajt.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.jianghu66.top/gtfdynndcd.html

[Q33] 多列分组
来源：http://hz.guannengcc.top/gtfuyqswgb.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.sxryk.cn/gtgqxffsob.html

[Q34] 每组取第一条
来源：http://hz.sxryk.cn/gturxehbvi.html

SELECT * FROM (
来源：http://hz.yueranfly.top/gtwmqttwmo.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.ydzc1.top/gtdkjutmxg.html

) t WHERE rn = 1;
来源：http://hz.smart0.xyz/gtuhimpmrx.html

[Q35] 内连接
来源：http://hz.gotoacloud.top/gtnvehoxhm.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.wangshuangyany.cn/gtrovbsfxb.html

[Q36] 左连接
来源：http://hz.yj20258.top/gtagajawed.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.chenjidiqi.icu/gthyzkcczo.html

[Q37] 右连接
来源：http://hz.chenlongwang.top/gtnggkfpxu.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.jiagoushi.top/gtksrkzctx.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.yonumen.top/gtxtprrsuo.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.cucudq.cn/gteiuhvjgi.html

[Q39] 自连接（查上下级）
来源：http://hz.havefunace.top/gtbhsucczq.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.nanxinkj.top/gtcslfoiuh.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.ywan-chungtsiang.top/gtbyrplxjv.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.cdnleiting.top/gtwrjltccz.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.zdqjudy.top/gticlrlsxs.html

[Q41] 多表连接
来源：http://hz.birdmap.top/gtyuhfwfgl.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.svipenyu.cn/gtwqmwtybs.html

JOIN users u ON u.id = o.user_id
来源：http://hz.ehwqpu.com/gttgkvboyf.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.hongshengwenyu.top/gtqmxxmzjx.html

[Q42] 连接条件附加过滤
来源：http://hz.zhijiandao.cn/gttjvyuncn.html

SELECT u.name, o.amount FROM users u
来源：http://hz.tianlin.xyz/gtyrdhzogm.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.xingfuxueyuan.xyz/gtkxaevuim.html

[Q43] 标量子查询
来源：http://hz.jinqigfzy.top/gtsdmngdig.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.yueranfly.top/gtmaqdvwod.html

[Q44] IN 子查询
来源：http://hz.sxryk.cn/gtkouqeuof.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.wangshuangyany.cn/gtmylcxbgk.html

[Q45] EXISTS 判断存在
来源：http://hz.guannengcc.top/gtpujacxzj.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.redwolf501.top/gtvnpqhgjh.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.daxiang520.top/gtpxypnxso.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jianghu66.top/gtobmpfain.html

[Q47] 与平均值比较
来源：http://hz.sufxvd.cn/gtvoebsxah.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.yuxming.cn/gtybtuusfy.html

[Q48] CTE 公用表表达式
来源：http://hz.jinghuilouyu.cn/gtffsmlavx.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.jinqigufen.top/gtygzeulbn.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.daxiang520.top/gtmtruwnjo.html

[Q49] 更新单行
来源：http://hz.hnqzz.top/gtukvdablf.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.shangyingyoupin.top/gtywnouveb.html

[Q50] 批量更新
来源：http://hz.sweek.top/gtivtrxxmi.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.bjfxy.top/gtlnopfijw.html

[Q51] 用子查询更新
来源：http://hz.xuanzx.com/gtjcognann.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.iojbl.cn/gtnpdfpopp.html

[Q52] 删除指定行
来源：http://hz.daxiang520.top/gtnafokeee.html

DELETE FROM users WHERE id = 10;
来源：http://hz.zhongyouzk.top/gtcxyddsaa.html

[Q53] 按条件删除
来源：http://hz.guannengcc.top/gtvbemkvig.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.ivvv.top/gtyiwihsvm.html

[Q54] 清空表
来源：http://hz.hysaishi.cn/gtzxbqoogm.html

TRUNCATE TABLE logs;
来源：http://hz.shangyingyoupin.top/gtdpuffcrx.html

[Q55] 排名（并列占位）
来源：http://hz.jqgufenzy.top/gtquagvxqa.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.zhongyouzk.top/gtpknpnlge.html

[Q56] 密集排名（并列不占位）
来源：http://hz.jinyuanbaomall.cn/gtlfhkhiom.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.feifeiyinyue.top/gtoheijxfv.html

[Q57] 行号
来源：http://hz.9152youxi.cn/gtgrxxnrev.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.yongpay.top/gtdketuoqj.html

[Q58] 累计求和
来源：http://hz.nanxinkj.top/gtupyxyvjp.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.jlsjyb.cn/gtlxwhnqjc.html

[Q59] 分组内累计
来源：http://hz.9152youxi.cn/gtxbicttiv.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.svipenyu.cn/gtjqsjikdj.html

[Q60] 取上一行 / 下一行
来源：http://hz.dianchejie.cn/gteqfhmoye.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.chenjidiqi.icu/gtwtfkeyag.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.jinqigufen.top/gtehidjruu.html

[Q61] 移动平均
来源：http://hz.jianghu66.top/gtfykygxvg.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.shangyingyoupin.top/gtpduhdyfb.html

[Q62] 分组占比
来源：http://hz.zhixingplan.top/gthwjjaimo.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.tian-w.cn/gteefccfcx.html

[Q63] 开启事务
来源：http://hz.cucudq.cn/gtwqumxggu.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.haohaochexian.top/gtiafvfvsx.html

[Q64] 提交事务
来源：http://hz.yongpay.top/gtcuslpqjc.html

COMMIT;
来源：http://hz.cqqwz.cn/gtmordpowg.html

[Q65] 回滚事务
来源：http://hz.zhiwuduotai.top/gtoyjohifx.html

ROLLBACK;
来源：http://hz.jqgfzy.top/gtkbinvzjg.html

[Q66] 行锁查询
来源：http://hz.quarkkingdee.top/gtibvmofsy.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.yvedp.cn/gtxnfwjlen.html

[Q67] 设置隔离级别
来源：http://hz.dashuyun.cn/gtegssrkiu.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.316326.xyz/gthzqnaytw.html

[Q68] 保存点
来源：http://hz.jqgfzy.top/gtcoxfidwa.html

SAVEPOINT sp1;
来源：http://hz.quarkkingdee.top/gtavaychmo.html

ROLLBACK TO sp1;
来源：http://hz.52xcode.cn/gtruyeglrb.html

[Q69] 查看执行计划
来源：http://hz.hysaishi.cn/gtpewhypyn.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.tanke756.top/gtnminzunp.html

[Q70] 更新统计信息
来源：http://hz.vqdsnc.cn/gthpraiwah.html

ANALYZE TABLE users;
来源：http://hz.xuetiantiany.cn/gtcsqdehic.html

[Q71] 查看建表语句
来源：http://hz.9152youxi.cn/gtkmhdejuy.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.tanke756.top/gtsmtufksa.html

[Q72] 查看索引
来源：http://hz.hammf.cn/gtjqzxahxt.html

SHOW INDEX FROM users;
来源：http://hz.vqdsnc.cn/gtibmklplw.html

[Q73] 查看表状态
来源：http://hz.zhaomingkeji.xyz/gtisdustxg.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.cdnleiting.top/gttmauxbep.html

[Q74] 强制使用索引
来源：http://hz.ybcxt.top/gtcbqeamgz.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.haohaochexian.top/gttqjrvial.html

[Q75] 日期格式化
来源：http://hz.xinyue.icu/gtnmkevqjl.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.nwbrower.top/gthkoraadg.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.ywan-chungtsiang.top/gtbhkpeyxf.html

[Q76] 按天统计
来源：http://hz.guannengcc.top/gtsijirbtr.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.jiagoushi.top/gtrgpvnyaf.html

[Q77] 时间加减
来源：http://hz.hfpthk.cn/gtmpzekzuh.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.gogol.net.cn/gtabsrkdeo.html

[Q78] 当前时间
来源：http://hz.ppjwa.cn/gtslurmpwf.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.daxiang520.top/gtagbbziwd.html

[Q79] 字符串拼接
来源：http://hz.hywenlv.cn/gtvjyiiuxz.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.ydzc1.top/gtmrnihkgb.html

[Q80] 字符串截取
来源：http://hz.zhijiandao.cn/gtgpiksenw.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.ydzc1.top/gtpynubabc.html

[Q81] 字符串替换
来源：http://hz.xingfuxueyuan.xyz/gtokljzukr.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.hnxiangtu.top/gtljzcpinj.html

[Q82] 字符长度与字节长度
来源：http://hz.nanxuanxn.top/gtlzwxtnju.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.xylfe.cn/gtlohiioap.html

[Q83] 大小写转换
来源：http://hz.hysaishi.cn/gtqfdiukbv.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.ppjwa.cn/gtcmwenrtv.html

[Q84] 去除首尾空格
来源：http://hz.316326.xyz/gtugchgmwz.html

SELECT TRIM(name) FROM users;
来源：http://hz.dianchejie.cn/gtopufdsdj.html

[Q85] 数值取整
来源：http://hz.jqgfzy.top/gthipyhfps.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.zhiwuduotai.top/gtjvueuwjl.html

[Q86] 读取 JSON 字段
来源：http://hz.nwbrower.top/gtqzssqzdg.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.ppjwa.cn/gttjzdqqhr.html

[Q87] JSON 字段做条件
来源：http://hz.aizwys.cn/gthwkatqpm.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.xuetiantiany.cn/gtkznzbewp.html

[Q88] 行转列（条件聚合）
来源：http://hz.jianghu66.top/gtysgocukk.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.0kj1m.cn/gtdgtpkrmn.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.dashuyun.cn/gtqjmkzoqe.html

[Q89] 判断表是否存在
来源：http://hz.zycfv.cn/gtandyuzfx.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.guannengcc.top/gtkpgwzfvm.html

[Q90] 生成序号列
来源：http://hz.haohaochexian.top/gtxiuxkinu.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.jinqigfzy.top/gtgflzeeyc.html

================================================================================
来源：http://hz.yangfankeji.com/gtyfxhepjc.html

R. Bash 专题
来源：http://hz.xuetiantiany.cn/gtdimbsjqk.html

================================================================================
来源：http://hz.yj202588.top/gtdsjpfqag.html

[R01] shebang 与严格模式
来源：http://hz.shanyushiyangtech.top/gtmvogbilj.html

#!/usr/bin/env bash
来源：http://hz.sysykeji.top/gtplbfjbce.html

set -euo pipefail
来源：http://hz.jyoumei.cn/gtpnxszvyu.html

[R02] 变量赋值与使用
来源：http://hz.mhx1999.top/gttlehyyij.html

name="Tom"; echo "$name"
来源：http://hz.hfpthk.cn/gtveuaping.html

[R03] 只读变量
来源：http://hz.andypj.xyz/gtnkgocvpi.html

readonly PI=3.14
来源：http://hz.zdqjudy.top/gtubjlhndu.html

[R04] 位置参数
来源：http://hz.cheryme.top/gteuxtgobw.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.jinqigufen.top/gtjdqglsdf.html

[R05] 参数默认值
来源：http://hz.guowangkeji.top/gtbcfmmmym.html

name="${1:-default}"
来源：http://hz.ivvv.top/gtaafegqcg.html

[R06] 判断命令是否存在
来源：http://hz.gaohongyu789.top/gtdkloshwx.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.bjfxy.top/gtpkkqogfx.html

[R07] if 判断文件
来源：http://hz.yongpay.top/gtkxnwnaia.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.bjfxy.top/gtvalnpjqp.html

[R08] 数值比较
来源：http://hz.xylfe.cn/gtfnyidpnf.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.yj202588.top/gtdggalvnh.html

[R09] 字符串比较
来源：http://hz.daxiang520.top/gtlrldotqd.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.jinqigufen.top/gtwedrnyrr.html

[R10] 正则匹配
来源：http://hz.c1oappe.top/gtkjzsdgac.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.bjfxy.top/gtfvrtzarw.html

[R11] case 多分支
来源：http://hz.guannengcc.top/gtxycwnaiz.html

case "$1" in
来源：http://hz.daxiang520.top/gtjyxbipoz.html

start) echo "启动" ;;
来源：http://hz.tanke756.top/gtczwhxvyw.html

stop)  echo "停止" ;;
来源：http://hz.iojbl.cn/gtuaeanazm.html

*)     echo "未知命令" ;;
来源：http://hz.jiagoushi.top/gticrcertq.html

esac
来源：http://hz.yueranfly.top/gtqvjzaged.html

[R12] for 遍历文件
来源：http://hz.ybcxt.top/gtsimurfjp.html

for f in *.txt; do echo "$f"; done
来源：http://hz.wangdashe.top/gtzvqckdfs.html

[R13] for 计数循环
来源：http://hz.daxiang520.top/gtilmvyaua.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.andypj.xyz/gtmymhzigb.html

[R14] C 风格 for
来源：http://hz.cheryme.top/gtsoyfgfhf.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.9152youxi.cn/gtwaslqisk.html

[R15] while 逐行读文件
来源：http://hz.ydzc1.top/gtwnnilgty.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.zhijiandao.cn/gtejlytnnn.html

[R16] until 等待条件
来源：http://hz.xuetiantiany.cn/gtbqqzvdwk.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.meibo888.top/gtmcrbjaag.html

[R17] 数组定义与取值
来源：http://hz.svipenyu.cn/gtrfpadoga.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.xziqi.cn/gtmfsjxgsu.html

[R18] 遍历数组
来源：http://hz.hfpthk.cn/gtjcaiqdlr.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.redwolf501.top/gtmzfugdhg.html

[R19] 数组长度
来源：http://hz.jinghuilouyu.cn/gtcqeefspy.html

echo "${#arr[@]}"
来源：http://hz.svipenyu.cn/gtxmocwcua.html

[R20] 关联数组（字典）
来源：http://hz.ywan-chungtsiang.top/gtwfazdfde.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.nwbrower.top/gtikazaddv.html

[R21] 字符串长度
来源：http://hz.yanxiufei.cn/gtbcltaihd.html

echo "${#s}"
来源：http://hz.jinghuilouyu.cn/gtnwbholsc.html

[R22] 截取子串
来源：http://hz.hnqzz.top/gtxrnwkyss.html

echo "${s:0:5}"
来源：http://hz.xziqi.cn/gtvoqwrgpb.html

[R23] 字符串替换
来源：http://hz.havefunace.top/gtouyrwcen.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.cucudq.cn/gtsrgwtolx.html

[R24] 大小写转换
来源：http://hz.52xcode.cn/gtmvlbeoxo.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.hammf.cn/gtojvcosxv.html

[R25] 去后缀 / 去前缀
来源：http://hz.bjfxy.top/gtioxdvkbv.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.pengpengdd.cyou/gtnbyyyfam.html

[R26] 命令替换
来源：http://hz.aibaodan.cn/gtnvvvleag.html

now=$(date +%F); echo "$now"
来源：http://hz.xziqi.cn/gtoibnkhmq.html

[R27] 算术展开
来源：http://hz.jiagoushi.top/gtmzkftxmu.html

echo $((1 + 2 * 3))
来源：http://hz.jinqigufen.top/gtndlxrcbn.html

[R28] 浮点运算
来源：http://hz.xingfuxueyuan.xyz/gtwdwradad.html

echo "scale=2; 10/3" | bc
来源：http://hz.xinyue.icu/gtngxtbpqx.html

[R29] 定义函数
来源：http://hz.zycfv.cn/gtceovcaqh.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.jlsjyb.cn/gtrpujnwmg.html

[R30] 函数返回状态码
来源：http://hz.zhengqikj.top/gtpqxfaaqz.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.jiagoushi.top/gtqnjqpycf.html

[R31] 局部变量
来源：http://hz.jinyuanbaomall.cn/gtwtxcbwpi.html


<!-- 参考信息 -->