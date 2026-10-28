代发 wailian999

[P05] 判断两个对象内容是否相等
来源：http://hz.yanxiufei.cn/gtmeujdwvx.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.xziqi.cn/gtcykonqeg.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.yuxming.cn/gtfeevcdnp.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.kuanghao11.cn/gtzgnvcgqj.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.yangfankeji.com/gtdzsilbnw.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.sufxvd.cn/gtuxdmuski.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.tanke756.top/gtfwhvzwao.html

Ruby: a == b
来源：http://hz.sweek.top/gtpjhwdvqq.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.ywan-chungtsiang.top/gttminybpc.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.sweek.top/gtljtdbjdj.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.yuanzhike.top/gtupfmwlhh.html

PHP:  if (empty($x)) {}
来源：http://hz.ydjk.org.cn/gtnbebhonq.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.jinqigufen.top/gtvnvionyj.html

TS:   if (x == null) {}
来源：http://hz.chenlongwang.top/gtuuyxgekf.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.aizwys.cn/gtkzvebpkw.html

Go:   if x == nil {}
来源：http://hz.jinyuanbaomall.cn/gtdceionxv.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.cheryme.top/gteluonmwd.html

C#:   if (x is null) {}
来源：http://hz.tianlin.xyz/gtsgswgeay.html

[P07] 防抖与节流
来源：http://hz.guannengcc.top/gtxuhiierd.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.tian-w.cn/gthmbxgukw.html

PHP:  // 手写时间戳比较
来源：http://hz.aizwys.cn/gtvxxdgysw.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.9152youxi.cn/gtxazdevdi.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.shuidangran.top/gtrprxsltf.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.snrcjt.cn/gtppnarogt.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.svipenyu.cn/gtckpscmie.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.xinyue.icu/gttnxvdblh.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.jinyuanbaomall.cn/gtnzzwcmzx.html

[P08] 处理浮点精度问题
来源：http://hz.yangfankeji.com/gtsrzttviu.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.fengsongda.top/gtgrbxxomu.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.xuanzx.com/gteinsajha.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.jqgfzy.top/gtuwsgvfim.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.shuidangran.top/gttqiuscek.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.xingfuxueyuan.xyz/gtzptlotqx.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.gogol.net.cn/gtrqqmizhr.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.cqqwz.cn/gtombkqmzr.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.zhiwuduotai.top/gtmdntaavr.html

================================================================================
来源：http://hz.gotoacloud.top/gtwrggjcul.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.c1oappe.top/gttxetbhko.html

================================================================================
来源：http://hz.yangfankeji.com/gttlbsvzvk.html

[Q01] 创建表
来源：http://hz.jinqigufen.top/gtpdxfrrkj.html

CREATE TABLE users (
来源：http://hz.wangdashe.top/gtfyjceipi.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yanxiufei.cn/gtkilngbef.html

name VARCHAR(50) NOT NULL,
来源：http://hz.vqdsnc.cn/gtnqneusme.html

email VARCHAR(100) UNIQUE,
来源：http://hz.svipenyu.cn/gtdjiuytbs.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.andypj.xyz/gtbpnvnhnc.html

);
来源：http://hz.ehwqpu.com/gtsbeniqjy.html

[Q02] 创建带外键的表
来源：http://hz.shuidangran.top/gtyfkbagdm.html

CREATE TABLE orders (
来源：http://hz.daxiang520.top/gtufctnvum.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.xinyue.icu/gteipvyscd.html

user_id INT NOT NULL,
来源：http://hz.sufxvd.cn/gthchfnyhn.html

amount DECIMAL(10, 2),
来源：http://hz.jiagoushi.top/gtlumjohjo.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.shanyushiyangkeji.top/gtalyhwzmq.html

);
来源：http://hz.shangyingyoupin.top/gtbarropim.html

[Q03] 增加列
来源：http://hz.aibaodan.cn/gtaqtnbeck.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.pycfn.com/gtdtrocyar.html

[Q04] 修改列类型
来源：http://hz.havefunace.top/gtlvatkwkt.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.shuidangran.top/gthloodyfr.html

[Q05] 重命名列
来源：http://hz.zhengqikj.top/gttcamoyoy.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.havefunace.top/gtmsefkoik.html

[Q06] 删除列
来源：http://hz.shzxlz.cn/gtmcmdghcq.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.gogol.net.cn/gtxmhvujzo.html

[Q07] 删除表
来源：http://hz.cqqwz.cn/gtroqdctae.html

DROP TABLE IF EXISTS orders;
来源：http://hz.c1oappe.top/gtrxhssxih.html

[Q08] 创建普通索引
来源：http://hz.bjfxy.top/gtybgwjgmh.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.tian-w.cn/gtoemrnoco.html

[Q09] 创建唯一索引
来源：http://hz.shuidangran.top/gthuazgzov.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.hysaishi.cn/gtqrfokqpu.html

[Q10] 插入单行
来源：http://hz.sxryk.cn/gtwjeqthtd.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.ivvv.top/gtrrqneiur.html

[Q11] 一次插入多行
来源：http://hz.iojbl.cn/gtcyyfcypn.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.sysykeji.top/gtfuszctlv.html

[Q12] 插入后取自增 ID
来源：http://hz.zhiwuduotai.top/gtpbpmgtac.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.cucudq.cn/gtkoikntlb.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.haohaochexian.top/gtjgurbbjr.html

[Q13] 忽略重复插入
来源：http://hz.yongpay.top/gtgxldoufm.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.smart0.xyz/gtjirifkpp.html

[Q14] 存在则更新（upsert）
来源：http://hz.aibaodan.cn/gtvtwbeyqg.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.cheryme.top/gtiflnlntl.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.sweek.top/gtbtddfspc.html

[Q15] 查询全部
来源：http://hz.mhx1999.top/gtmoygdhgp.html

SELECT * FROM users;
来源：http://hz.shanyushiyangtech.top/gtuldzdhwm.html

[Q16] 查询指定列
来源：http://hz.nanxinkj.top/gtspwvczsl.html

SELECT id, name FROM users;
来源：http://hz.xziqi.cn/gtheabuory.html

[Q17] 条件查询
来源：http://hz.dashuyun.cn/gtpnqccsxz.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.dashuyun.cn/gtxijsmakn.html

[Q18] 模糊匹配
来源：http://hz.nwbrower.top/gtrcdmccpd.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.bjfxy.top/gtdznxwyyf.html

[Q19] 范围查询
来源：http://hz.nanxinkj.top/gtaolxlvqu.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.chenlongwang.top/gttojhirsw.html

[Q20] IN 列表
来源：http://hz.snrcjt.cn/gtgfwrsyvr.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.gaohongyu789.top/gtsbjwcygg.html

[Q21] 空值判断
来源：http://hz.yueranfly.top/gtilgawuhc.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.wangshuangyany.cn/gtvcpdtqls.html

[Q22] 排序
来源：http://hz.hnqzz.top/gttowjwyzo.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.jqgfzy.top/gtiysdvkmv.html

[Q23] 分页
来源：http://hz.fengsongda.top/gtbtgmklge.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.tian-w.cn/gtwrvpvixt.html

[Q24] 去重
来源：http://hz.zhaomingkeji.xyz/gtutlaluyl.html

SELECT DISTINCT city FROM users;
来源：http://hz.yueranfly.top/gtconhqcyy.html

[Q25] 只取前 N 条
来源：http://hz.xziqi.cn/gtenamilxi.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.cqqwz.cn/gtdhhkvikq.html

[Q26] 计数
来源：http://hz.daria6918.cn/gtropfqgwb.html

SELECT COUNT(*) FROM users;
来源：http://hz.gogol.net.cn/gtlrubwidq.html

[Q27] 条件计数
来源：http://hz.chenjidiqi.icu/gtbxszhyff.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.jianghu66.top/gtuegjmwju.html

[Q28] 求和与平均
来源：http://hz.nanxinkj.top/gtleubspue.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.aibaodan.cn/gtiuyucsew.html

[Q29] 最大最小值
来源：http://hz.ybcxt.top/gttsbwbrkc.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.xingfuxueyuan.xyz/gtmmfwbsze.html

[Q30] 分组统计
来源：http://hz.zhengqikj.top/gthhfbookp.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.yj202588.top/gtoukcgvfo.html

[Q31] 分组后过滤
来源：http://hz.sysykeji.top/gtsxypnxmx.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.bjfxy.top/gtkttqegdt.html

[Q32] 分组拼接字符串
来源：http://hz.yj20258888.top/gtfhqnkuyu.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.cucudq.cn/gtmwtjdviv.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.hnxiangtu.top/gtuycqzlmh.html

[Q33] 多列分组
来源：http://hz.guannengcc.top/gtqcttgodn.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.c1oappe.top/gtumvypxyg.html

[Q34] 每组取第一条
来源：http://hz.yueranfly.top/gtsjsfkrlj.html

SELECT * FROM (
来源：http://hz.ivvv.top/gtzgxofyzm.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.ivvv.top/gtsyfpvfwo.html

) t WHERE rn = 1;
来源：http://hz.jlsjyb.cn/gthfxcnifp.html

[Q35] 内连接
来源：http://hz.yueranfly.top/gtycdydnfs.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.hysaishi.cn/gttlezgkdz.html

[Q36] 左连接
来源：http://hz.jinghuilouyu.cn/gttxoikvye.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.guannengcc.top/gtvqlukrnp.html

[Q37] 右连接
来源：http://hz.guowangkeji.top/gtssrueimy.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.zhijiandao.cn/gtmnvlnfqg.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.fengsongda.top/gtirrwgjhx.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.zhongyouzk.top/gtzkgpglff.html

[Q39] 自连接（查上下级）
来源：http://hz.jiagoushi.top/gtjqvpanft.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.fengsongda.top/gtssdxuvpu.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.cashguo.top/gttmtshetp.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.hongshengwenyu.top/gtjkjotiav.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.cucudq.cn/gtjtuxsdmr.html

[Q41] 多表连接
来源：http://hz.daria6918.cn/gtqrpqiqxn.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.iojbl.cn/gtjqgrnniz.html

JOIN users u ON u.id = o.user_id
来源：http://hz.mhx1999.top/gtzjbqbqnm.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.nwbrower.top/gtsozikwrn.html

[Q42] 连接条件附加过滤
来源：http://hz.zhijiandao.cn/gtvlufikuh.html

SELECT u.name, o.amount FROM users u
来源：http://hz.52xcode.cn/gtecrxwopa.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.meibo888.top/gtommaphij.html

[Q43] 标量子查询
来源：http://hz.hammf.cn/gtgmoktgvo.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.sufxvd.cn/gtpqzycvit.html

[Q44] IN 子查询
来源：http://hz.316326.xyz/gtvchjqnsa.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.andypj.xyz/gtxprcijkf.html

[Q45] EXISTS 判断存在
来源：http://hz.zhengqikj.top/gtdlreudao.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.tianlin.xyz/gtzjwoslcp.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.cashguo.top/gttiiyvojr.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.bjfxy.top/gtpyhwjimt.html

[Q47] 与平均值比较
来源：http://hz.chenzaomai.com/gtznnyldwt.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.havefunace.top/gtzoeczedl.html

[Q48] CTE 公用表表达式
来源：http://hz.havefunace.top/gtikoiuzah.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.yj202588.top/gtzuxdzwiu.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.hammf.cn/gtdqliaozj.html

[Q49] 更新单行
来源：http://hz.xylfe.cn/gtalmpbtze.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.sysykeji.top/gtqirkftkn.html

[Q50] 批量更新
来源：http://hz.yonumen.top/gtxvwbwtsy.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.0kj1m.cn/gtdxjuauyd.html

[Q51] 用子查询更新
来源：http://hz.havefunace.top/gtccmrdeev.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.cqqwz.cn/gtlpnftibp.html

[Q52] 删除指定行
来源：http://hz.kuanghao11.cn/gtuunujnmx.html

DELETE FROM users WHERE id = 10;
来源：http://hz.kuanghao11.cn/gtbiqvlxaj.html

[Q53] 按条件删除
来源：http://hz.yvedp.cn/gtqkelbdpa.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.yuxming.cn/gtlhqvbsnh.html

[Q54] 清空表
来源：http://hz.hfpthk.cn/gtyuijyesh.html

TRUNCATE TABLE logs;
来源：http://hz.sysykeji.top/gtebwmvydu.html

[Q55] 排名（并列占位）
来源：http://hz.sufxvd.cn/gtsfovlgey.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.ywan-chungtsiang.top/gtgsqhvvvv.html

[Q56] 密集排名（并列不占位）
来源：http://hz.shuidangran.top/gtmhwiflgi.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.daxiang520.top/gttvewdquy.html

[Q57] 行号
来源：http://hz.ybcxt.top/gtfbviuhzz.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.hnxiangtu.top/gtceqrvrve.html

[Q58] 累计求和
来源：http://hz.tanke756.top/gtxbynhtky.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.shangyingyoupin.top/gttxjbgssx.html

[Q59] 分组内累计
来源：http://hz.shangyingyoupin.top/gtomfxjopd.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.jlsjyb.cn/gtvplamrny.html

[Q60] 取上一行 / 下一行
来源：http://hz.pengpengdd.cyou/gtxnbmbbhv.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.shuidangran.top/gtacponwly.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.nanxinkj.top/gtbwrwfejt.html

[Q61] 移动平均
来源：http://hz.cashguo.top/gtnmxfrwwm.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.yuxming.cn/gtvmsdybxr.html

[Q62] 分组占比
来源：http://hz.sysykeji.top/gtaxyvrcmq.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.ppjwa.cn/gtszgngcxk.html

[Q63] 开启事务
来源：http://hz.cqqwz.cn/gtdalkcsqe.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.guannengcc.top/gtwzspxcjt.html

[Q64] 提交事务
来源：http://hz.gaohongyu789.top/gtllzmvquw.html

COMMIT;
来源：http://hz.xylfe.cn/gtjnysjxdr.html

[Q65] 回滚事务
来源：http://hz.jqgfzy.top/gtfzohacyz.html

ROLLBACK;
来源：http://hz.yangfankeji.com/gtrwckpfmz.html

[Q66] 行锁查询
来源：http://hz.ppjwa.cn/gtugucfave.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.gzhubu.top/gtrriagwbt.html

[Q67] 设置隔离级别
来源：http://hz.yanxiufei.cn/gtfjhqvdli.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.ywan-chungtsiang.top/gtnwmistqw.html

[Q68] 保存点
来源：http://hz.kuanghao11.cn/gtfupwqadg.html

SAVEPOINT sp1;
来源：http://hz.0kj1m.cn/gttlajsqtz.html

ROLLBACK TO sp1;
来源：http://hz.yvedp.cn/gtlqubsvaf.html

[Q69] 查看执行计划
来源：http://hz.jiagoushi.top/gttsmrgnuh.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.fzhhl.top/gtekpnjumo.html

[Q70] 更新统计信息
来源：http://hz.yj202588.top/gtjuffsisn.html

ANALYZE TABLE users;
来源：http://hz.yangfankeji.com/gtyapyeqrb.html

[Q71] 查看建表语句
来源：http://hz.zhongyouzk.top/gtomwoyihc.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.gotoacloud.top/gtknbbecpm.html

[Q72] 查看索引
来源：http://hz.dianchejie.cn/gtzjvqorcp.html

SHOW INDEX FROM users;
来源：http://hz.xinyue.icu/gtrkfcsvot.html

[Q73] 查看表状态
来源：http://hz.yanxiufei.cn/gtwtoyfcgt.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.mhx1999.top/gtoiovutte.html

[Q74] 强制使用索引
来源：http://hz.shzxlz.cn/gtvcsbnjkz.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.iojbl.cn/gtsexvbcsd.html

[Q75] 日期格式化
来源：http://hz.jinqigfzy.top/gtabjkpspz.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.cheryme.top/gtdqzjizoq.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.jinghuilouyu.cn/gtgtxdgdan.html

[Q76] 按天统计
来源：http://hz.dashuyun.cn/gtozznmnqr.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.fengsongda.top/gtbnxdwmqw.html

[Q77] 时间加减
来源：http://hz.yueranfly.top/gtazyddxdn.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.hongshengwenyu.top/gtffbthumf.html

[Q78] 当前时间
来源：http://hz.jyoumei.cn/gtgfqoqoni.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.jiagoushi.top/gtjbblnzzl.html

[Q79] 字符串拼接
来源：http://hz.yj20258888.top/gtobtxcsvs.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.yj202588.top/gttuxxthdu.html

[Q80] 字符串截取
来源：http://hz.smart0.xyz/gtgpjfpoiv.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.yuxming.cn/gtfzhyvtwd.html

[Q81] 字符串替换
来源：http://hz.gzhubu.top/gtwafetjpa.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.zdqjudy.top/gtvzllzspv.html

[Q82] 字符长度与字节长度
来源：http://hz.yuanzhike.top/gtpbajicty.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.zycfv.cn/gtbxlgbrzd.html

[Q83] 大小写转换
来源：http://hz.jqgfzy.top/gtnmuikwwn.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.nanxinkj.top/gtobkwkviw.html

[Q84] 去除首尾空格
来源：http://hz.yanxiufei.cn/gttqkwhckf.html

SELECT TRIM(name) FROM users;
来源：http://hz.xziqi.cn/gtkbaeaxcg.html

[Q85] 数值取整
来源：http://hz.hnqzz.top/gtmqmsxptg.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.sxryk.cn/gtunsmltnz.html

[Q86] 读取 JSON 字段
来源：http://hz.sysykeji.top/gtbohkxxlx.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.nanxuanxn.top/gtmstjasmx.html

[Q87] JSON 字段做条件
来源：http://hz.zhoulong.xyz/gtnsikaqqa.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.jlsjyb.cn/gtvzcufmwh.html

[Q88] 行转列（条件聚合）
来源：http://hz.zycfv.cn/gtlmieiifm.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.fengsongda.top/gtkhdrqxyw.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.nwbrower.top/gtasalxchh.html

[Q89] 判断表是否存在
来源：http://hz.wangdashe.top/gtdwjjkrqm.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.tian-w.cn/gtvxlxfbzf.html

[Q90] 生成序号列
来源：http://hz.iojbl.cn/gtlvyipphk.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.hywenlv.cn/gtdbfujhob.html

================================================================================
来源：http://hz.ydjk.org.cn/gtezhdlqma.html

R. Bash 专题
来源：http://hz.aibaodan.cn/gttkrcqcyj.html

================================================================================
来源：http://hz.nwbrower.top/gtnhrdohyg.html

[R01] shebang 与严格模式
来源：http://hz.ywan-chungtsiang.top/gtntsrehak.html

#!/usr/bin/env bash
来源：http://hz.fengsongda.top/gtebzoksrj.html

set -euo pipefail
来源：http://hz.wangshuangyany.cn/gttflevqob.html

[R02] 变量赋值与使用
来源：http://hz.jinqigfzy.top/gtupobxdsd.html

name="Tom"; echo "$name"
来源：http://hz.fzhhl.top/gtqncvwvzn.html

[R03] 只读变量
来源：http://hz.c1oappe.top/gtrwgnwlqu.html

readonly PI=3.14
来源：http://hz.guannengcc.top/gtvzpshmvv.html

[R04] 位置参数
来源：http://hz.yj20258888.top/gtsepqwlve.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.hywenlv.cn/gtdshyxvjh.html

[R05] 参数默认值
来源：http://hz.pengpengdd.cyou/gtsjhgozzj.html

name="${1:-default}"
来源：http://hz.cucudq.cn/gtqbfjrwyk.html

[R06] 判断命令是否存在
来源：http://hz.gzhubu.top/gtpoxafhme.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.fzhhl.top/gtxspiabul.html

[R07] if 判断文件
来源：http://hz.zhaomingkeji.xyz/gtrtonzvli.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.yuanzhike.top/gtgwhijzip.html

[R08] 数值比较
来源：http://hz.zycfv.cn/gtxvhezdje.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.jlsjyb.cn/gteeukvzav.html

[R09] 字符串比较
来源：http://hz.kuanghao11.cn/gtljaaggad.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.shangyingyoupin.top/gtltcajbis.html

[R10] 正则匹配
来源：http://hz.cdnleiting.top/gtnqbnwjvb.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.yj20258.top/gtpjefyeuw.html

[R11] case 多分支
来源：http://hz.guannengcc.top/gtwzogukbl.html

case "$1" in
来源：http://hz.jianghu66.top/gtsrsosyok.html

start) echo "启动" ;;
来源：http://hz.aibaodan.cn/gttzxanmhw.html

stop)  echo "停止" ;;
来源：http://hz.shangyingyoupin.top/gttrkcackv.html

*)     echo "未知命令" ;;
来源：http://hz.shanyushiyangtech.top/gtvlvtrnza.html

esac
来源：http://hz.zdqjudy.top/gtbvxtxges.html

[R12] for 遍历文件
来源：http://hz.yj202588.top/gtygonhvqa.html

for f in *.txt; do echo "$f"; done
来源：http://hz.ywan-chungtsiang.top/gtieninerr.html

[R13] for 计数循环
来源：http://hz.andypj.xyz/gtqsnjilka.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.yj20258.top/gthiymryst.html

[R14] C 风格 for
来源：http://hz.yuxming.cn/gtfqkffyyt.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.gogol.net.cn/gtwoosrzlw.html

[R15] while 逐行读文件
来源：http://hz.aibaodan.cn/gtqpnftveu.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.hnxiangtu.top/gtqexqsont.html

[R16] until 等待条件
来源：http://hz.havefunace.top/gtxhdwycng.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.ppjwa.cn/gtcciuejfg.html

[R17] 数组定义与取值
来源：http://hz.guowangkeji.top/gtwufrmhie.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.shzxlz.cn/gtnylmptfm.html

[R18] 遍历数组
来源：http://hz.kuanghao11.cn/gtezwfcavm.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.zhengqikj.top/gtnzcfjust.html

[R19] 数组长度
来源：http://hz.cheryme.top/gtcioajpbp.html

echo "${#arr[@]}"
来源：http://hz.vqdsnc.cn/gtyuzslzgt.html

[R20] 关联数组（字典）
来源：http://hz.sxryk.cn/gtpvmimnav.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.havefunace.top/gtydkkqyzd.html

[R21] 字符串长度
来源：http://hz.aizwys.cn/gtznvfvtwu.html

echo "${#s}"
来源：http://hz.ywan-chungtsiang.top/gthjfiowgu.html

[R22] 截取子串
来源：http://hz.xziqi.cn/gtcvavmfvt.html

echo "${s:0:5}"
来源：http://hz.shzxlz.cn/gtvpeegelx.html

[R23] 字符串替换
来源：http://hz.jinqigfzy.top/gtmvwdshqi.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.svipenyu.cn/gtinklixww.html

[R24] 大小写转换
来源：http://hz.guannengcc.top/gtqthxlglg.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.meibo888.top/gtnkyluvwm.html

[R25] 去后缀 / 去前缀
来源：http://hz.chenlongwang.top/gteikefnzn.html


<!-- 参考信息 -->