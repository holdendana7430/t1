代发 wailian999

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.shanyushiyangtech.top/gtoxxrtfbq.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.c1oappe.top/gtkfdcapds.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.ivvv.top/gtaohyhtpn.html

PHP:  if (empty($x)) {}
来源：http://hz.yj202588.top/gtllswelwy.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.hammf.cn/gtcwawvtxw.html

TS:   if (x == null) {}
来源：http://hz.yj20258.top/gtyfgqamsq.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.ybcxt.top/gtthqnuifj.html

Go:   if x == nil {}
来源：http://hz.zdqjudy.top/gtpkudofcu.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.meibo888.top/gtaqabdsip.html

C#:   if (x is null) {}
来源：http://hz.pycfn.com/gtflywaquv.html

[P07] 防抖与节流
来源：http://hz.jinqigfzy.top/gtmumzwqpk.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.tian-w.cn/gtuqnuapca.html

PHP:  // 手写时间戳比较
来源：http://hz.chenlongwang.top/gteopknlpv.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.hongshengwenyu.top/gtdqafsqpu.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.ehwqpu.com/gtgeadwets.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.svipenyu.cn/gtskurxljw.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.hysaishi.cn/gtkbihdgea.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.hnxiangtu.top/gttfkbsdum.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.hammf.cn/gtuoqovgqu.html

[P08] 处理浮点精度问题
来源：http://hz.yuxming.cn/gtukkyssvz.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.sysykeji.top/gtqzweiaxn.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.cdnleiting.top/gtbmqgndbw.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.sxryk.cn/gtpzerfcdu.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.svipenyu.cn/gtpennpiwl.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.yj20258888.top/gtoktsdcqv.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.yueranfly.top/gttflappor.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.chenzaomai.com/gtonyahuly.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.pengpengdd.cyou/gthzbsplgn.html

================================================================================
来源：http://hz.chenlongwang.top/gtuutcllot.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.ehwqpu.com/gtloebnfog.html

================================================================================
来源：http://hz.gaohongyu789.top/gtelvuymtn.html

[Q01] 创建表
来源：http://hz.zhengqikj.top/gtaoqvquzg.html

CREATE TABLE users (
来源：http://hz.yuxming.cn/gtmtwehbqs.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yj20258.top/gtgsqoajwj.html

name VARCHAR(50) NOT NULL,
来源：http://hz.aizwys.cn/gtqeofdomf.html

email VARCHAR(100) UNIQUE,
来源：http://hz.jyoumei.cn/gtwfkpfyrv.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.ybcxt.top/gtbgjlwnwu.html

);
来源：http://hz.zhixingplan.top/gtlkgqndpx.html

[Q02] 创建带外键的表
来源：http://hz.zhixingplan.top/gtkwqjjgka.html

CREATE TABLE orders (
来源：http://hz.shangyingyoupin.top/gtavyxgbyd.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.xinyue.icu/gtupqggdcl.html

user_id INT NOT NULL,
来源：http://hz.jqgfzy.top/gtdqvcmkgt.html

amount DECIMAL(10, 2),
来源：http://hz.andypj.xyz/gtvwahcntd.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.cdnleiting.top/gtuxhltcgv.html

);
来源：http://hz.shanyushiyangkeji.top/gthlydvpho.html

[Q03] 增加列
来源：http://hz.hnqzz.top/gtszsjhnxx.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.mhx1999.top/gtscmjufer.html

[Q04] 修改列类型
来源：http://hz.vqdsnc.cn/gtnvurzknc.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.yuxming.cn/gtlfdziwld.html

[Q05] 重命名列
来源：http://hz.jqgfzy.top/gtnkpwgqss.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.guowangkeji.top/gtywrpbzgi.html

[Q06] 删除列
来源：http://hz.meibo888.top/gttlvcvqaz.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.sxryk.cn/gtnyscrdup.html

[Q07] 删除表
来源：http://hz.zhixingplan.top/gtfeooyitu.html

DROP TABLE IF EXISTS orders;
来源：http://hz.jqgufenzy.top/gtjhssdqdv.html

[Q08] 创建普通索引
来源：http://hz.ivvv.top/gtwwpnoqta.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.0kj1m.cn/gtuysmgqda.html

[Q09] 创建唯一索引
来源：http://hz.fengsongda.top/gtxabomlvb.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.zhixingplan.top/gtyxdvvtil.html

[Q10] 插入单行
来源：http://hz.havefunace.top/gtitfutyhi.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.zhaomingkeji.xyz/gtxwzpijta.html

[Q11] 一次插入多行
来源：http://hz.fengsongda.top/gtkladpqzq.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.hywenlv.cn/gtrjklyqws.html

[Q12] 插入后取自增 ID
来源：http://hz.cheryme.top/gtkxkepmxn.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.wangdashe.top/gtlyzuwbwd.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.pycfn.com/gtmwsgjbre.html

[Q13] 忽略重复插入
来源：http://hz.hfpthk.cn/gtqleeyovx.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.sweek.top/gtyhujmhxg.html

[Q14] 存在则更新（upsert）
来源：http://hz.jianghu66.top/gtqgehpxla.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.hammf.cn/gtkivlrfeg.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.meibo888.top/gtotmfhkwy.html

[Q15] 查询全部
来源：http://hz.zhijiandao.cn/gtfpayauex.html

SELECT * FROM users;
来源：http://hz.9152youxi.cn/gteqtxsetm.html

[Q16] 查询指定列
来源：http://hz.birdmap.top/gtpynchbnd.html

SELECT id, name FROM users;
来源：http://hz.hongshengwenyu.top/gtfcyzrzfb.html

[Q17] 条件查询
来源：http://hz.hnxiangtu.top/gtaicyfshm.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.ppjwa.cn/gtaqyjifve.html

[Q18] 模糊匹配
来源：http://hz.yj20258.top/gticgxvfxp.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.yvedp.cn/gtedqkmuia.html

[Q19] 范围查询
来源：http://hz.yuanzhike.top/gtkhxnwilc.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.nanxuanxn.top/gtencralvc.html

[Q20] IN 列表
来源：http://hz.hongshengwenyu.top/gtvsjtrcsu.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.fengsongda.top/gtuyrcwpew.html

[Q21] 空值判断
来源：http://hz.dashuyun.cn/gtqetvdrsn.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.pycfn.com/gthvfqbzyx.html

[Q22] 排序
来源：http://hz.yueranfly.top/gtfnmzuige.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.nanxinkj.top/gtpehowcyf.html

[Q23] 分页
来源：http://hz.meibo888.top/gticujxojn.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.9152youxi.cn/gtgoelbisj.html

[Q24] 去重
来源：http://hz.zhongyouzk.top/gtptchxujl.html

SELECT DISTINCT city FROM users;
来源：http://hz.wangshuangyany.cn/gtkhyupuhb.html

[Q25] 只取前 N 条
来源：http://hz.kuanghao11.cn/gtwdejfnqv.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.hysaishi.cn/gtfbbajrkn.html

[Q26] 计数
来源：http://hz.tian-w.cn/gtdyxuvzjb.html

SELECT COUNT(*) FROM users;
来源：http://hz.nwbrower.top/gtwtdxuqjq.html

[Q27] 条件计数
来源：http://hz.xuanzx.com/gtgunqstrw.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.gaohongyu789.top/gtwywxvbfg.html

[Q28] 求和与平均
来源：http://hz.jianghu66.top/gtzjpswpax.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.jianghu66.top/gtaldcyxko.html

[Q29] 最大最小值
来源：http://hz.hnxiangtu.top/gtuqisyzbf.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.shuidangran.top/gtijnlkaku.html

[Q30] 分组统计
来源：http://hz.316326.xyz/gtylbetpdn.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.wangdashe.top/gtadvuxkfl.html

[Q31] 分组后过滤
来源：http://hz.tian-w.cn/gtlvfxnbny.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.cqqwz.cn/gtxcwyshup.html

[Q32] 分组拼接字符串
来源：http://hz.wangshuangyany.cn/gtvpnfpqhm.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.zhongyouzk.top/gtavmyttic.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.hywenlv.cn/gtsjpaczjt.html

[Q33] 多列分组
来源：http://hz.dianchejie.cn/gthzadsvzp.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.dashuyun.cn/gtlvworywq.html

[Q34] 每组取第一条
来源：http://hz.jyoumei.cn/gtsjflfzow.html

SELECT * FROM (
来源：http://hz.xylfe.cn/gtfptmuiox.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.jyoumei.cn/gtiwvkcbxc.html

) t WHERE rn = 1;
来源：http://hz.gaohongyu789.top/gtmrjlggag.html

[Q35] 内连接
来源：http://hz.ydjk.org.cn/gtcmmglsof.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.shanyushiyangkeji.top/gtfmpibveg.html

[Q36] 左连接
来源：http://hz.pengpengdd.cyou/gtrlmrdfwk.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.yuanzhike.top/gtpnpqsmyx.html

[Q37] 右连接
来源：http://hz.smart0.xyz/gtmtajuasq.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.yuanzhike.top/gtlapgsbqu.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.zhijiandao.cn/gtsrbjlvtr.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.yj202588.top/gtcqnvrkgq.html

[Q39] 自连接（查上下级）
来源：http://hz.cashguo.top/gtyrvwupmx.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.fzhhl.top/gtmfrqlkrq.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.zdqjudy.top/gttivqbpak.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.daxiang520.top/gtugvvdyyt.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.ppjwa.cn/gtnjwkpnqj.html

[Q41] 多表连接
来源：http://hz.aizwys.cn/gtmmxkrfxi.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.52xcode.cn/gtjdlrqrxa.html

JOIN users u ON u.id = o.user_id
来源：http://hz.jlsjyb.cn/gtudaqihqi.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.birdmap.top/gttohdpczm.html

[Q42] 连接条件附加过滤
来源：http://hz.cashguo.top/gtubomtjbu.html

SELECT u.name, o.amount FROM users u
来源：http://hz.hfpthk.cn/gtviblvexr.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.jianghu66.top/gtdjzzbwcg.html

[Q43] 标量子查询
来源：http://hz.yangfankeji.com/gtqmyjswfk.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.zhaomingkeji.xyz/gtkjgulnhi.html

[Q44] IN 子查询
来源：http://hz.zhiwuduotai.top/gtgqrsqmng.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.ppjwa.cn/gtztgjhyyl.html

[Q45] EXISTS 判断存在
来源：http://hz.vqdsnc.cn/gtastkcluo.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.hywenlv.cn/gteeeutgyc.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.yonumen.top/gtnjvswiyy.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.tanke756.top/gtqsezhkba.html

[Q47] 与平均值比较
来源：http://hz.pycfn.com/gtlvrhxtru.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.nanxuanxn.top/gtgeyvjcey.html

[Q48] CTE 公用表表达式
来源：http://hz.yangfankeji.com/gtqqsvoupi.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.chenzaomai.com/gtbblyfdyj.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.dashuyun.cn/gtuheqgrxu.html

[Q49] 更新单行
来源：http://hz.zhengqikj.top/gtobdeoowt.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.shangyingyoupin.top/gtkyuvguqm.html

[Q50] 批量更新
来源：http://hz.jinqigufen.top/gtfqayynnj.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.hfpthk.cn/gtdptbfftt.html

[Q51] 用子查询更新
来源：http://hz.havefunace.top/gtzylycnaq.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.hfpthk.cn/gtohrbeybp.html

[Q52] 删除指定行
来源：http://hz.jianghu66.top/gtttxmwtwq.html

DELETE FROM users WHERE id = 10;
来源：http://hz.yangfankeji.com/gtthazkbht.html

[Q53] 按条件删除
来源：http://hz.316326.xyz/gtvrearlku.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.jianghu66.top/gtxtcpfkmk.html

[Q54] 清空表
来源：http://hz.zhengqikj.top/gtkrogsqvh.html

TRUNCATE TABLE logs;
来源：http://hz.ybcxt.top/gtngxhdjde.html

[Q55] 排名（并列占位）
来源：http://hz.nanxinkj.top/gtyagedcag.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.zhiwuduotai.top/gttcanpsvk.html

[Q56] 密集排名（并列不占位）
来源：http://hz.nwbrower.top/gthrzeufmq.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.jinyuanbaomall.cn/gtqcgyfuxl.html

[Q57] 行号
来源：http://hz.jyoumei.cn/gthkrvnoxb.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.daxiang520.top/gtmuzctoeu.html

[Q58] 累计求和
来源：http://hz.ywan-chungtsiang.top/gtydqgpcie.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.jqgfzy.top/gtvptqsvio.html

[Q59] 分组内累计
来源：http://hz.sxryk.cn/gtjlmnnumq.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.guowangkeji.top/gtswmzfpvk.html

[Q60] 取上一行 / 下一行
来源：http://hz.ivvv.top/gtnmugorlu.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.gzhubu.top/gtfrttyntt.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.nwbrower.top/gtigbufwdl.html

[Q61] 移动平均
来源：http://hz.ydzc1.top/gtqtjfaqul.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.gzhubu.top/gteqekbnfz.html

[Q62] 分组占比
来源：http://hz.guannengcc.top/gtxfxftqwv.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.0kj1m.cn/gtupfhjmon.html

[Q63] 开启事务
来源：http://hz.zhoulong.xyz/gtxbtnktdh.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.feifeiyinyue.top/gtvdlcwuat.html

[Q64] 提交事务
来源：http://hz.daria6918.cn/gtikuzhrde.html

COMMIT;
来源：http://hz.smart0.xyz/gtdayyraqy.html

[Q65] 回滚事务
来源：http://hz.wangshuangyany.cn/gtpvgklaxs.html

ROLLBACK;
来源：http://hz.c1oappe.top/gtekckyfza.html

[Q66] 行锁查询
来源：http://hz.cashguo.top/gtrustjlaq.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.jqgfzy.top/gtwrszxlzx.html

[Q67] 设置隔离级别
来源：http://hz.hysaishi.cn/gthtebhuev.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.vqdsnc.cn/gtkxdkgcqk.html

[Q68] 保存点
来源：http://hz.xziqi.cn/gtaxzmgjjo.html

SAVEPOINT sp1;
来源：http://hz.shzxlz.cn/gtuchneyog.html

ROLLBACK TO sp1;
来源：http://hz.smart0.xyz/gtxqpwceim.html

[Q69] 查看执行计划
来源：http://hz.mhx1999.top/gtiiftbiqz.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.zycfv.cn/gtanvyazgy.html

[Q70] 更新统计信息
来源：http://hz.gzhubu.top/gtwwzmidxg.html

ANALYZE TABLE users;
来源：http://hz.redwolf501.top/gtxjoioaky.html

[Q71] 查看建表语句
来源：http://hz.sufxvd.cn/gtwfnfnhyn.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.yanxiufei.cn/gtmugpqman.html

[Q72] 查看索引
来源：http://hz.wangshuangyany.cn/gtfgzgumwr.html

SHOW INDEX FROM users;
来源：http://hz.fengsongda.top/gtfdienhde.html

[Q73] 查看表状态
来源：http://hz.zdqjudy.top/gtgyotwvth.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.yangfankeji.com/gtirvuqeqa.html

[Q74] 强制使用索引
来源：http://hz.xinyue.icu/gthtaqbltc.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.shangyingyoupin.top/gtpccntuiy.html

[Q75] 日期格式化
来源：http://hz.sxryk.cn/gtyhhufkvj.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.zhongyouzk.top/gtmdlmuzaw.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.meibo888.top/gtexmrhyft.html

[Q76] 按天统计
来源：http://hz.hongshengwenyu.top/gtiecnnxfj.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.jlsjyb.cn/gtluahgqvd.html

[Q77] 时间加减
来源：http://hz.yj202588.top/gtzwsdepxa.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.nanxinkj.top/gtrgtepntq.html

[Q78] 当前时间
来源：http://hz.hnxiangtu.top/gtkmjphruw.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.hysaishi.cn/gtrlcuzpxq.html

[Q79] 字符串拼接
来源：http://hz.yvedp.cn/gtguoqechl.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.ywan-chungtsiang.top/gtbqnyilof.html

[Q80] 字符串截取
来源：http://hz.iojbl.cn/gtodtrqezj.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.redwolf501.top/gtofcvnrre.html

[Q81] 字符串替换
来源：http://hz.nwbrower.top/gtowhiwern.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.yuxming.cn/gtftdhnkgy.html

[Q82] 字符长度与字节长度
来源：http://hz.yj20258.top/gtwzntxmkm.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.shangyingyoupin.top/gtaakigisu.html

[Q83] 大小写转换
来源：http://hz.mhx1999.top/gtykqigcvt.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.tian-w.cn/gtmxijljah.html

[Q84] 去除首尾空格
来源：http://hz.xingfuxueyuan.xyz/gtgbrgrige.html

SELECT TRIM(name) FROM users;
来源：http://hz.sufxvd.cn/gtldgogfop.html

[Q85] 数值取整
来源：http://hz.jqgufenzy.top/gtdzdjbwec.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.jqgfzy.top/gtlduhwonh.html

[Q86] 读取 JSON 字段
来源：http://hz.cqqwz.cn/gtzwizcmqc.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.mhx1999.top/gtffltuilb.html

[Q87] JSON 字段做条件
来源：http://hz.zhengqikj.top/gtsobqpfmr.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.ywan-chungtsiang.top/gtzxezqahe.html

[Q88] 行转列（条件聚合）
来源：http://hz.chenzaomai.com/gtazmdaihf.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.yj20258.top/gtlndbvpjt.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.cdnleiting.top/gtjjswbspx.html

[Q89] 判断表是否存在
来源：http://hz.ydjk.org.cn/gtagmjceid.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.chenjidiqi.icu/gtfxrffmcw.html

[Q90] 生成序号列
来源：http://hz.tian-w.cn/gtabzeduxx.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.jqgufenzy.top/gtvyqyfqug.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtixhusgfs.html

R. Bash 专题
来源：http://hz.xziqi.cn/gtvvsfzojc.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtbbmnqjmz.html

[R01] shebang 与严格模式
来源：http://hz.yueranfly.top/gtjbpaulma.html

#!/usr/bin/env bash
来源：http://hz.jyoumei.cn/gtjpumepua.html

set -euo pipefail
来源：http://hz.yj202588.top/gtcxzfwscc.html

[R02] 变量赋值与使用
来源：http://hz.nanxuanxn.top/gtbmqsnvpd.html

name="Tom"; echo "$name"
来源：http://hz.smart0.xyz/gtasuxyjjo.html

[R03] 只读变量
来源：http://hz.316326.xyz/gtqwrlrsyy.html

readonly PI=3.14
来源：http://hz.9152youxi.cn/gtjymwovyu.html

[R04] 位置参数
来源：http://hz.svipenyu.cn/gtieyybarm.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.jiagoushi.top/gtugpmqvut.html

[R05] 参数默认值
来源：http://hz.xingfuxueyuan.xyz/gthpwtxkts.html

name="${1:-default}"
来源：http://hz.guannengcc.top/gtzspsqqlq.html

[R06] 判断命令是否存在
来源：http://hz.jqgfzy.top/gthqbnblam.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.hfpthk.cn/gtxfkurxfx.html

[R07] if 判断文件
来源：http://hz.hywenlv.cn/gtyxjvrhsl.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.guannengcc.top/gtpircxwuq.html

[R08] 数值比较
来源：http://hz.jyoumei.cn/gtbaygcnuw.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.sufxvd.cn/gtivcpqexw.html

[R09] 字符串比较
来源：http://hz.yj202588.top/gtmjdtpriz.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.ybcxt.top/gtqxrkayca.html

[R10] 正则匹配
来源：http://hz.wangdashe.top/gtowicofmp.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.kuanghao11.cn/gtumwgnlgf.html

[R11] case 多分支
来源：http://hz.tianlin.xyz/gtpfayccse.html

case "$1" in
来源：http://hz.shuidangran.top/gtrprnyrjs.html

start) echo "启动" ;;
来源：http://hz.yongpay.top/gtrnaxyjcm.html

stop)  echo "停止" ;;
来源：http://hz.gaohongyu789.top/gtrayiatlq.html

*)     echo "未知命令" ;;
来源：http://hz.yueranfly.top/gtfvoowdvs.html

esac
来源：http://hz.jyoumei.cn/gttpnwqfuz.html

[R12] for 遍历文件
来源：http://hz.daria6918.cn/gtpfwziejd.html

for f in *.txt; do echo "$f"; done
来源：http://hz.cheryme.top/gtahosdvtf.html

[R13] for 计数循环
来源：http://hz.zhaomingkeji.xyz/gtkdmwxpgj.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.haohaochexian.top/gtgiruluqy.html

[R14] C 风格 for
来源：http://hz.ywan-chungtsiang.top/gtidnniirs.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.vqdsnc.cn/gtrymksmsx.html

[R15] while 逐行读文件
来源：http://hz.pengpengdd.cyou/gtritogyol.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.jiagoushi.top/gtpuwtydus.html

[R16] until 等待条件
来源：http://hz.yj202588.top/gtjmiyvyfa.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.quarkkingdee.top/gtqtlzgniy.html

[R17] 数组定义与取值
来源：http://hz.yuxming.cn/gtwijhwqgw.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.dashuyun.cn/gtolznzjkk.html

[R18] 遍历数组
来源：http://hz.fengsongda.top/gtrbifirpk.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.tianlin.xyz/gtxdhtxfoy.html

[R19] 数组长度
来源：http://hz.zhijiandao.cn/gtkfkqvvbv.html

echo "${#arr[@]}"
来源：http://hz.jinyuanbaomall.cn/gtcpvckrok.html

[R20] 关联数组（字典）
来源：http://hz.nanxinkj.top/gtbamsxfkt.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.andypj.xyz/gtghzjgenf.html

[R21] 字符串长度
来源：http://hz.shzxlz.cn/gtibnpfitt.html

echo "${#s}"
来源：http://hz.ydzc1.top/gtoupxmqps.html

[R22] 截取子串
来源：http://hz.0kj1m.cn/gtkiildlra.html

echo "${s:0:5}"
来源：http://hz.hnxiangtu.top/gtzkwodwoj.html

[R23] 字符串替换
来源：http://hz.xuetiantiany.cn/gtelziaccw.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.yj20258888.top/gttmlgoyef.html

[R24] 大小写转换
来源：http://hz.nanxuanxn.top/gtbsrynpbo.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.sufxvd.cn/gtoinqxwxf.html

[R25] 去后缀 / 去前缀
来源：http://hz.dianchejie.cn/gtocdjzanp.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.jlsjyb.cn/gtgvgzhkpx.html

[R26] 命令替换
来源：http://hz.vqdsnc.cn/gtnmvktirh.html

now=$(date +%F); echo "$now"
来源：http://hz.pycfn.com/gtbapbdgyp.html

[R27] 算术展开
来源：http://hz.ywan-chungtsiang.top/gtpmzozhkd.html

echo $((1 + 2 * 3))
来源：http://hz.shangyingyoupin.top/gtcxmzdzva.html

[R28] 浮点运算
来源：http://hz.wangshuangyany.cn/gtoojriusc.html

echo "scale=2; 10/3" | bc
来源：http://hz.jqgfzy.top/gtadqigkrf.html

[R29] 定义函数
来源：http://hz.zhaomingkeji.xyz/gtgqrxgiud.html


<!-- 参考信息 -->