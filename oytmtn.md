代发 wailian999

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.sxryk.cn/gtrdmbqbyd.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.jqgfzy.top/gtbuuoieqn.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.chenzaomai.com/gtgwdaqzsq.html

Ruby: a == b
来源：http://hz.hysaishi.cn/gtxtetcnwd.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.zhaomingkeji.xyz/gthprxrfmh.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.hywenlv.cn/gtaygtexxp.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.gotoacloud.top/gtbbmnexzb.html

PHP:  if (empty($x)) {}
来源：http://hz.jlsjyb.cn/gtcuuhtxbb.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.zhoulong.xyz/gtaemongso.html

TS:   if (x == null) {}
来源：http://hz.yj202588.top/gtnsnrpozo.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.shzxlz.cn/gtkpbkalcm.html

Go:   if x == nil {}
来源：http://hz.0kj1m.cn/gtxteafytx.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.fzhhl.top/gtrzucxrce.html

C#:   if (x is null) {}
来源：http://hz.0kj1m.cn/gtefpkyswy.html

[P07] 防抖与节流
来源：http://hz.yonumen.top/gthhgjyzwq.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.zhijiandao.cn/gtxcmwizat.html

PHP:  // 手写时间戳比较
来源：http://hz.meibo888.top/gtkfldajha.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.ivvv.top/gtwvzutvkf.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.ywan-chungtsiang.top/gtaqkfjtfs.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.yuxming.cn/gtqnydoppv.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.chenlongwang.top/gthuztaser.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.redwolf501.top/gtehcjjxtg.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.xuanzx.com/gtfnmezwsz.html

[P08] 处理浮点精度问题
来源：http://hz.52xcode.cn/gttkymyxev.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.dashuyun.cn/gteuirjqyv.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.wangshuangyany.cn/gtmrlrmfgn.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.sxryk.cn/gtziwxmfgt.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.fengsongda.top/gtvtpfacef.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.sweek.top/gtdbnaoiwk.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.zdqjudy.top/gtssiannrl.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.zycfv.cn/gtxrpmeluj.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.cqqwz.cn/gtuqcakvea.html

================================================================================
来源：http://hz.yj20258.top/gtjfuuobgs.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.shzxlz.cn/gtfadfwpzp.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtoblfreji.html

[Q01] 创建表
来源：http://hz.hammf.cn/gtjglsrctx.html

CREATE TABLE users (
来源：http://hz.yongpay.top/gtwqeectcf.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.fengsongda.top/gtbhioaigx.html

name VARCHAR(50) NOT NULL,
来源：http://hz.shangyingyoupin.top/gtpmgayvtu.html

email VARCHAR(100) UNIQUE,
来源：http://hz.bjfxy.top/gtvobunhtt.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.hysaishi.cn/gtzvqmibrn.html

);
来源：http://hz.tianlin.xyz/gtlwksmedt.html

[Q02] 创建带外键的表
来源：http://hz.shzxlz.cn/gtuwmgzaet.html

CREATE TABLE orders (
来源：http://hz.ivvv.top/gtkopqywpx.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.redwolf501.top/gttuurqikm.html

user_id INT NOT NULL,
来源：http://hz.havefunace.top/gtqdgiwcqm.html

amount DECIMAL(10, 2),
来源：http://hz.xingfuxueyuan.xyz/gtxwrjyplf.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.xuetiantiany.cn/gtvlgyuict.html

);
来源：http://hz.hnxiangtu.top/gtjxgrwggy.html

[Q03] 增加列
来源：http://hz.sxryk.cn/gtqbmyhhac.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.sxryk.cn/gtoxkkhufm.html

[Q04] 修改列类型
来源：http://hz.yangfankeji.com/gtnwdlxoam.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.dianchejie.cn/gtsjfgafns.html

[Q05] 重命名列
来源：http://hz.yanxiufei.cn/gtxjwxonkm.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.yueranfly.top/gtjvltcgrw.html

[Q06] 删除列
来源：http://hz.jiagoushi.top/gtnlbqdaet.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.fzhhl.top/gtvxujzsnm.html

[Q07] 删除表
来源：http://hz.daxiang520.top/gteqhlzfxf.html

DROP TABLE IF EXISTS orders;
来源：http://hz.cashguo.top/gtrdwwvted.html

[Q08] 创建普通索引
来源：http://hz.nwbrower.top/gtmkqrvmzc.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.9152youxi.cn/gtorzkpyns.html

[Q09] 创建唯一索引
来源：http://hz.andypj.xyz/gtegmnthgs.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.jinghuilouyu.cn/gtnrnozoet.html

[Q10] 插入单行
来源：http://hz.jinqigufen.top/gtfzqdpwkb.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.aibaodan.cn/gtkybvzayx.html

[Q11] 一次插入多行
来源：http://hz.nanxuanxn.top/gtvplxjrfu.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.yj202588.top/gtyhwqkxvk.html

[Q12] 插入后取自增 ID
来源：http://hz.havefunace.top/gtufsficmm.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.iojbl.cn/gtlirkuimo.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.jinghuilouyu.cn/gtalybdpfr.html

[Q13] 忽略重复插入
来源：http://hz.yongpay.top/gtjkmkfxck.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.sxryk.cn/gtjtewgfvp.html

[Q14] 存在则更新（upsert）
来源：http://hz.yvedp.cn/gtsrrapzmi.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.yj20258.top/gtyxkigloy.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.shanyushiyangtech.top/gtltlcssji.html

[Q15] 查询全部
来源：http://hz.redwolf501.top/gtgjxpxuhd.html

SELECT * FROM users;
来源：http://hz.dashuyun.cn/gterijfrcb.html

[Q16] 查询指定列
来源：http://hz.0kj1m.cn/gtrapnuuwp.html

SELECT id, name FROM users;
来源：http://hz.sufxvd.cn/gtfqwtujlg.html

[Q17] 条件查询
来源：http://hz.sweek.top/gtzanmoiyg.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.havefunace.top/gtgtpvqgqp.html

[Q18] 模糊匹配
来源：http://hz.xuanzx.com/gtawqaourb.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.mhx1999.top/gtopgbnhgg.html

[Q19] 范围查询
来源：http://hz.jqgfzy.top/gttzasbwlu.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.316326.xyz/gtntztdauo.html

[Q20] IN 列表
来源：http://hz.xuetiantiany.cn/gtsuqyzqws.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.xingfuxueyuan.xyz/gtmwnjxizt.html

[Q21] 空值判断
来源：http://hz.gzhubu.top/gtpgyubkfn.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.jinqigfzy.top/gtocyppmpz.html

[Q22] 排序
来源：http://hz.gogol.net.cn/gtcuegugsp.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.cheryme.top/gtcvbrfavg.html

[Q23] 分页
来源：http://hz.jianghu66.top/gtvzitqhoq.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.wangshuangyany.cn/gtrhrlrgib.html

[Q24] 去重
来源：http://hz.ydzc1.top/gtkfzisgmu.html

SELECT DISTINCT city FROM users;
来源：http://hz.xingfuxueyuan.xyz/gtrddpizue.html

[Q25] 只取前 N 条
来源：http://hz.ppjwa.cn/gtjdvhxhau.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.hywenlv.cn/gtimwopmvb.html

[Q26] 计数
来源：http://hz.0kj1m.cn/gtcgpumsrq.html

SELECT COUNT(*) FROM users;
来源：http://hz.yonumen.top/gtknljgwst.html

[Q27] 条件计数
来源：http://hz.yangfankeji.com/gtnsrztovg.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.iojbl.cn/gtohwosjwl.html

[Q28] 求和与平均
来源：http://hz.andypj.xyz/gtjfirkkmo.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.cucudq.cn/gtxzuavour.html

[Q29] 最大最小值
来源：http://hz.yanxiufei.cn/gtxsqbipcv.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.shanyushiyangtech.top/gtjvupqkns.html

[Q30] 分组统计
来源：http://hz.ybcxt.top/gtwpyrpcuh.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.sysykeji.top/gthmjsybun.html

[Q31] 分组后过滤
来源：http://hz.quarkkingdee.top/gttcnxhyml.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.jyoumei.cn/gtenzbnepe.html

[Q32] 分组拼接字符串
来源：http://hz.zhaomingkeji.xyz/gtbvbnujeb.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.jinqigfzy.top/gtcqawjzig.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.xylfe.cn/gtbtkryzfm.html

[Q33] 多列分组
来源：http://hz.bjfxy.top/gtezvvwfhv.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.zhoulong.xyz/gtdjtappae.html

[Q34] 每组取第一条
来源：http://hz.yueranfly.top/gtqenkiubt.html

SELECT * FROM (
来源：http://hz.guowangkeji.top/gtjjbooceo.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.yvedp.cn/gtqvlpvxap.html

) t WHERE rn = 1;
来源：http://hz.zhixingplan.top/gtuqbcwydi.html

[Q35] 内连接
来源：http://hz.shanyushiyangtech.top/gtobtnyoxk.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.jinghuilouyu.cn/gtzhfxwsau.html

[Q36] 左连接
来源：http://hz.ywan-chungtsiang.top/gttmeetldo.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.nanxuanxn.top/gtqdnhwula.html

[Q37] 右连接
来源：http://hz.redwolf501.top/gtvgjeaxur.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.smart0.xyz/gtgekzmlnb.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.dashuyun.cn/gteomuxcif.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.c1oappe.top/gtpsqegtoo.html

[Q39] 自连接（查上下级）
来源：http://hz.xuanzx.com/gtloxzjhls.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.jqgufenzy.top/gtadeagnkq.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.wangshuangyany.cn/gtsszryogo.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.gzhubu.top/gtzydfcujm.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.hysaishi.cn/gtgusfaowh.html

[Q41] 多表连接
来源：http://hz.xinyue.icu/gtnjtlzodq.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.hysaishi.cn/gtunviuhmj.html

JOIN users u ON u.id = o.user_id
来源：http://hz.yuanzhike.top/gtdlgusdwg.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.haohaochexian.top/gtbfwkkpdi.html

[Q42] 连接条件附加过滤
来源：http://hz.hongshengwenyu.top/gtuvsxgbpk.html

SELECT u.name, o.amount FROM users u
来源：http://hz.wangdashe.top/gtnrgunvmw.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.bjfxy.top/gtklcmhmcc.html

[Q43] 标量子查询
来源：http://hz.c1oappe.top/gtzqekkrhd.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.fengsongda.top/gtixyayirp.html

[Q44] IN 子查询
来源：http://hz.nanxinkj.top/gtlpwwnfdd.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.9152youxi.cn/gtystifcuq.html

[Q45] EXISTS 判断存在
来源：http://hz.gotoacloud.top/gtndeluxwm.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.ppjwa.cn/gtasyhlmfo.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.guannengcc.top/gtzqefyquv.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.c1oappe.top/gtsoikwfgt.html

[Q47] 与平均值比较
来源：http://hz.cashguo.top/gtczuzbrdz.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.zdqjudy.top/gtulptdsju.html

[Q48] CTE 公用表表达式
来源：http://hz.yuanzhike.top/gthhhpmeto.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.ivvv.top/gtznnwptpu.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.hywenlv.cn/gtlzximokz.html

[Q49] 更新单行
来源：http://hz.aizwys.cn/gtcfofwqkb.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.snrcjt.cn/gtfkkuitir.html

[Q50] 批量更新
来源：http://hz.dianchejie.cn/gtbxibiptc.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.gzhubu.top/gtuxmaxlfx.html

[Q51] 用子查询更新
来源：http://hz.ehwqpu.com/gtducnxtsl.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.jiagoushi.top/gtwpalfbci.html

[Q52] 删除指定行
来源：http://hz.sxryk.cn/gtxkarefqe.html

DELETE FROM users WHERE id = 10;
来源：http://hz.xuanzx.com/gthkwsurvs.html

[Q53] 按条件删除
来源：http://hz.0kj1m.cn/gtcjyesxgn.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.jqgfzy.top/gttspimfou.html

[Q54] 清空表
来源：http://hz.zhengqikj.top/gtufdedaku.html

TRUNCATE TABLE logs;
来源：http://hz.guowangkeji.top/gtkeuvskkq.html

[Q55] 排名（并列占位）
来源：http://hz.fzhhl.top/gtopjfjfzr.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.andypj.xyz/gtpfzwtwci.html

[Q56] 密集排名（并列不占位）
来源：http://hz.zhoulong.xyz/gtftgihasy.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.redwolf501.top/gtczftmqku.html

[Q57] 行号
来源：http://hz.feifeiyinyue.top/gtpycdxfys.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.zdqjudy.top/gtotymotam.html

[Q58] 累计求和
来源：http://hz.yuanzhike.top/gtwfmawwwv.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.feifeiyinyue.top/gtxmtctrsl.html

[Q59] 分组内累计
来源：http://hz.jiagoushi.top/gtwhdwifsz.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.hammf.cn/gtlucbwvcv.html

[Q60] 取上一行 / 下一行
来源：http://hz.meibo888.top/gtgqlgvejs.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.hywenlv.cn/gtfguyhmcm.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.yj20258.top/gtvswppwaj.html

[Q61] 移动平均
来源：http://hz.iojbl.cn/gtqydmpfzt.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.xziqi.cn/gtacozfhpe.html

[Q62] 分组占比
来源：http://hz.hnxiangtu.top/gthtukjqow.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.chenlongwang.top/gtqecbsrsh.html

[Q63] 开启事务
来源：http://hz.haohaochexian.top/gtawrhuzwa.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.mhx1999.top/gttqbgvegf.html

[Q64] 提交事务
来源：http://hz.yuxming.cn/gtchrigapj.html

COMMIT;
来源：http://hz.iojbl.cn/gtovmmdgkm.html

[Q65] 回滚事务
来源：http://hz.aibaodan.cn/gtqzjofdbn.html

ROLLBACK;
来源：http://hz.daxiang520.top/gtprzqdcbg.html

[Q66] 行锁查询
来源：http://hz.wangdashe.top/gterebaiil.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.xuetiantiany.cn/gtjacxolbd.html

[Q67] 设置隔离级别
来源：http://hz.cheryme.top/gtfbrphcmn.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.nanxinkj.top/gtkmmnfypu.html

[Q68] 保存点
来源：http://hz.zhengqikj.top/gtskaqdhqi.html

SAVEPOINT sp1;
来源：http://hz.dianchejie.cn/gtdhqpjppl.html

ROLLBACK TO sp1;
来源：http://hz.iojbl.cn/gtzwijatsa.html

[Q69] 查看执行计划
来源：http://hz.0kj1m.cn/gtnelgbhpn.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.ivvv.top/gtlwpeaedz.html

[Q70] 更新统计信息
来源：http://hz.jyoumei.cn/gtszxywvbx.html

ANALYZE TABLE users;
来源：http://hz.jlsjyb.cn/gtodghsniy.html

[Q71] 查看建表语句
来源：http://hz.sweek.top/gtgzxwjoju.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.ehwqpu.com/gthhlrpovt.html

[Q72] 查看索引
来源：http://hz.cqqwz.cn/gtogeezklo.html

SHOW INDEX FROM users;
来源：http://hz.zdqjudy.top/gtuqfzajnd.html

[Q73] 查看表状态
来源：http://hz.iojbl.cn/gtkemymuoj.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.gotoacloud.top/gtemyajemz.html

[Q74] 强制使用索引
来源：http://hz.zhengqikj.top/gtttfgukbq.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.jlsjyb.cn/gtbdxcyyif.html

[Q75] 日期格式化
来源：http://hz.smart0.xyz/gthfpxfyed.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.ivvv.top/gtikwwaiif.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.zhixingplan.top/gtaqlxcjjg.html

[Q76] 按天统计
来源：http://hz.jqgufenzy.top/gtsdomwbpf.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.zhixingplan.top/gtcrickaet.html

[Q77] 时间加减
来源：http://hz.9152youxi.cn/gtsfjgimta.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.fengsongda.top/gtorsxgvyy.html

[Q78] 当前时间
来源：http://hz.yongpay.top/gtojoyquql.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.vqdsnc.cn/gtkhfredkh.html

[Q79] 字符串拼接
来源：http://hz.shanyushiyangtech.top/gtzuujmorn.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.ydzc1.top/gtgagkevps.html

[Q80] 字符串截取
来源：http://hz.jinyuanbaomall.cn/gtjnromvrj.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.shanyushiyangkeji.top/gtwzjdmxbd.html

[Q81] 字符串替换
来源：http://hz.9152youxi.cn/gtpeatgkjp.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.redwolf501.top/gtypubtcpm.html

[Q82] 字符长度与字节长度
来源：http://hz.jinghuilouyu.cn/gtudfhrpsg.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.sysykeji.top/gtxmiyfkwz.html

[Q83] 大小写转换
来源：http://hz.shanyushiyangkeji.top/gtevfhlfuw.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.hfpthk.cn/gtqnasypvh.html

[Q84] 去除首尾空格
来源：http://hz.hywenlv.cn/gtoynxwaqb.html

SELECT TRIM(name) FROM users;
来源：http://hz.chenzaomai.com/gtjgrmvucv.html

[Q85] 数值取整
来源：http://hz.hnqzz.top/gtbwvzpywz.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.jinqigufen.top/gtgiugdrch.html

[Q86] 读取 JSON 字段
来源：http://hz.yuanzhike.top/gtbubahqpt.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.daria6918.cn/gttgsdajfr.html

[Q87] JSON 字段做条件
来源：http://hz.kuanghao11.cn/gtbzbgkmcf.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.hnqzz.top/gtqextjhqt.html

[Q88] 行转列（条件聚合）
来源：http://hz.nanxuanxn.top/gthvuxgvro.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.daxiang520.top/gtigcqdgvn.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.sysykeji.top/gtmkqcpwcw.html

[Q89] 判断表是否存在
来源：http://hz.pengpengdd.cyou/gtpuaocvbt.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.xinyue.icu/gtpvxukxku.html

[Q90] 生成序号列
来源：http://hz.jianghu66.top/gtwxrwxjzt.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.ydzc1.top/gtjknofckd.html

================================================================================
来源：http://hz.kuanghao11.cn/gtvqstpqvn.html

R. Bash 专题
来源：http://hz.cashguo.top/gtizbrfczi.html

================================================================================
来源：http://hz.birdmap.top/gtkvkvuuuj.html

[R01] shebang 与严格模式
来源：http://hz.cashguo.top/gtdjrwjabe.html

#!/usr/bin/env bash
来源：http://hz.yj202588.top/gtxarvtwwn.html

set -euo pipefail
来源：http://hz.hywenlv.cn/gtebezgvho.html

[R02] 变量赋值与使用
来源：http://hz.zhoulong.xyz/gtubtqclzv.html

name="Tom"; echo "$name"
来源：http://hz.chenlongwang.top/gttwczgpqk.html

[R03] 只读变量
来源：http://hz.ehwqpu.com/gtcgbuwdff.html

readonly PI=3.14
来源：http://hz.pycfn.com/gtwhbcpglf.html

[R04] 位置参数
来源：http://hz.zhiwuduotai.top/gtuaauqvaz.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.zycfv.cn/gthgsdwluf.html

[R05] 参数默认值
来源：http://hz.zhijiandao.cn/gtagqaaqkc.html

name="${1:-default}"
来源：http://hz.jinyuanbaomall.cn/gtvzgujgwl.html

[R06] 判断命令是否存在
来源：http://hz.gzhubu.top/gthjdowoyt.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.yuxming.cn/gtgjiielig.html

[R07] if 判断文件
来源：http://hz.yuxming.cn/gtyxtdpcth.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.vqdsnc.cn/gtsjnwybkl.html

[R08] 数值比较
来源：http://hz.dianchejie.cn/gtzfelxtjz.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.zhijiandao.cn/gtnstxekaw.html

[R09] 字符串比较
来源：http://hz.shzxlz.cn/gtmtcdyosu.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.bjfxy.top/gtetsmfkzo.html

[R10] 正则匹配
来源：http://hz.chenjidiqi.icu/gtdpuyggta.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.andypj.xyz/gtqqtlgsoz.html

[R11] case 多分支
来源：http://hz.jqgfzy.top/gtvwvmmjyl.html

case "$1" in
来源：http://hz.sxryk.cn/gtgbnqtsjx.html

start) echo "启动" ;;
来源：http://hz.52xcode.cn/gtuglskpeh.html

stop)  echo "停止" ;;
来源：http://hz.316326.xyz/gtursdwits.html

*)     echo "未知命令" ;;
来源：http://hz.iojbl.cn/gtsehwqezr.html

esac
来源：http://hz.andypj.xyz/gtxcwfnhdx.html

[R12] for 遍历文件
来源：http://hz.jqgufenzy.top/gtddjafjel.html

for f in *.txt; do echo "$f"; done
来源：http://hz.haohaochexian.top/gtaujhzfae.html

[R13] for 计数循环
来源：http://hz.yueranfly.top/gtzeqhwakm.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.jiagoushi.top/gtebwwionl.html

[R14] C 风格 for
来源：http://hz.zdqjudy.top/gtxqwctfus.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.ydjk.org.cn/gtalsobcry.html

[R15] while 逐行读文件
来源：http://hz.dianchejie.cn/gtgpxnrmok.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.ivvv.top/gtuykdbaej.html

[R16] until 等待条件
来源：http://hz.zhengqikj.top/gtdjrsjbqu.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.zhiwuduotai.top/gtzbcvvnja.html

[R17] 数组定义与取值
来源：http://hz.fzhhl.top/gtazwkhsgs.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.cheryme.top/gtpikmivvf.html

[R18] 遍历数组
来源：http://hz.cheryme.top/gtkojjdskf.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.hfpthk.cn/gtswajwhhg.html

[R19] 数组长度
来源：http://hz.dianchejie.cn/gtpvxxviop.html

echo "${#arr[@]}"
来源：http://hz.hongshengwenyu.top/gtvuzvjujb.html

[R20] 关联数组（字典）
来源：http://hz.guannengcc.top/gtkawuzewl.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.feifeiyinyue.top/gttuthfxpy.html

[R21] 字符串长度
来源：http://hz.chenlongwang.top/gtqcffwngh.html

echo "${#s}"
来源：http://hz.gogol.net.cn/gtnhbgjgla.html

[R22] 截取子串
来源：http://hz.ehwqpu.com/gtvgwwggwq.html

echo "${s:0:5}"
来源：http://hz.dianchejie.cn/gttlyqmbup.html

[R23] 字符串替换
来源：http://hz.ehwqpu.com/gtfyrenodw.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.jqgfzy.top/gtfsixpsfa.html

[R24] 大小写转换
来源：http://hz.jyoumei.cn/gtaibuzqfc.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.jinghuilouyu.cn/gtkcjqrwnn.html

[R25] 去后缀 / 去前缀
来源：http://hz.yongpay.top/gtfsnnofel.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.jiagoushi.top/gtpxlrkfnm.html

[R26] 命令替换
来源：http://hz.52xcode.cn/gtihsflbia.html

now=$(date +%F); echo "$now"
来源：http://hz.nanxuanxn.top/gteapzsysa.html

[R27] 算术展开
来源：http://hz.jqgufenzy.top/gtqstxture.html


<!-- 参考信息 -->