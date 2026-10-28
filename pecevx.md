代发 wailian999

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.jinyuanbaomall.cn/gtgrhsrhzy.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.hnqzz.top/gtfxjiiujp.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.c1oappe.top/gtjcgvhrui.html

PHP:  if (empty($x)) {}
来源：http://hz.zhaomingkeji.xyz/gtvxyixlox.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.ehwqpu.com/gtbrzzexzv.html

TS:   if (x == null) {}
来源：http://hz.ydjk.org.cn/gtfedthmqt.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.hnqzz.top/gtktuftegb.html

Go:   if x == nil {}
来源：http://hz.ydzc1.top/gtdmjmuial.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.jinqigfzy.top/gtqcotvlfs.html

C#:   if (x is null) {}
来源：http://hz.fengsongda.top/gthlmlyuse.html

[P07] 防抖与节流
来源：http://hz.sufxvd.cn/gtopqpzbba.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.zhiwuduotai.top/gtxrgtcnmi.html

PHP:  // 手写时间戳比较
来源：http://hz.hongshengwenyu.top/gtatmfwnjk.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.xingfuxueyuan.xyz/gtmdudegaj.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.xinyue.icu/gtxshczcny.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.dianchejie.cn/gtetmxdpos.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.mhx1999.top/gtsdwijeiz.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.feifeiyinyue.top/gtluzqhmmc.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.vqdsnc.cn/gtghjxheix.html

[P08] 处理浮点精度问题
来源：http://hz.hnxiangtu.top/gtbanjyswk.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.daxiang520.top/gtuctccjal.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.yanxiufei.cn/gtaeddhnrt.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.nanxuanxn.top/gtwigpyaju.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.guowangkeji.top/gtbpaxrtkh.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.yj202588.top/gtauugmsdg.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.chenjidiqi.icu/gtuvldtmet.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.zdqjudy.top/gteumidzok.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.yueranfly.top/gtlraklngx.html

================================================================================
来源：http://hz.bjfxy.top/gtcpbmbfph.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.gotoacloud.top/gttjvpogpy.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtqpdussra.html

[Q01] 创建表
来源：http://hz.gotoacloud.top/gtcimnlkve.html

CREATE TABLE users (
来源：http://hz.redwolf501.top/gtywdtqetx.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.chenjidiqi.icu/gtoxarzifj.html

name VARCHAR(50) NOT NULL,
来源：http://hz.mhx1999.top/gtryomdjoh.html

email VARCHAR(100) UNIQUE,
来源：http://hz.aibaodan.cn/gtnvtypbdy.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.shanyushiyangtech.top/gtqhmnhqre.html

);
来源：http://hz.yuanzhike.top/gtcysvelwh.html

[Q02] 创建带外键的表
来源：http://hz.jinqigfzy.top/gtmtehbxlo.html

CREATE TABLE orders (
来源：http://hz.yonumen.top/gtlhutpyvv.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.chenjidiqi.icu/gtiohymxvt.html

user_id INT NOT NULL,
来源：http://hz.xuanzx.com/gtvdlqpraa.html

amount DECIMAL(10, 2),
来源：http://hz.yvedp.cn/gtrpyqslyo.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.yonumen.top/gtbjyorwbw.html

);
来源：http://hz.fzhhl.top/gttmqtrjvf.html

[Q03] 增加列
来源：http://hz.yj20258888.top/gtqpvudfiz.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.hnxiangtu.top/gtytyntkup.html

[Q04] 修改列类型
来源：http://hz.redwolf501.top/gtqhkfmanx.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.meibo888.top/gtfvvmcsuq.html

[Q05] 重命名列
来源：http://hz.fengsongda.top/gtmjcgckdq.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.cdnleiting.top/gtivlikhfv.html

[Q06] 删除列
来源：http://hz.52xcode.cn/gtyseljhsa.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.vqdsnc.cn/gtunkxpatm.html

[Q07] 删除表
来源：http://hz.yonumen.top/gtvqjslxwj.html

DROP TABLE IF EXISTS orders;
来源：http://hz.daxiang520.top/gthxtvyvcx.html

[Q08] 创建普通索引
来源：http://hz.zhongyouzk.top/gtoafihsbi.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.gogol.net.cn/gtdwclztku.html

[Q09] 创建唯一索引
来源：http://hz.yangfankeji.com/gtbvexrwcc.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.ppjwa.cn/gtlkvbpjvx.html

[Q10] 插入单行
来源：http://hz.ybcxt.top/gtjlgsbtrg.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.hnqzz.top/gtmxdjssmt.html

[Q11] 一次插入多行
来源：http://hz.jqgfzy.top/gtejcsxwty.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.jinqigfzy.top/gthvxtgzqc.html

[Q12] 插入后取自增 ID
来源：http://hz.yuanzhike.top/gtiqainvlv.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.kuanghao11.cn/gtbenwdkus.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.havefunace.top/gtvvznmgfs.html

[Q13] 忽略重复插入
来源：http://hz.iojbl.cn/gtwitvjuxa.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.fengsongda.top/gtxxqpgxqu.html

[Q14] 存在则更新（upsert）
来源：http://hz.zhongyouzk.top/gtyyujfjvw.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.xuanzx.com/gtrmkjchtz.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.cheryme.top/gtspiiqode.html

[Q15] 查询全部
来源：http://hz.cdnleiting.top/gtikuhjvgu.html

SELECT * FROM users;
来源：http://hz.hnqzz.top/gthnrudwrd.html

[Q16] 查询指定列
来源：http://hz.jinyuanbaomall.cn/gtbztlsvrr.html

SELECT id, name FROM users;
来源：http://hz.shzxlz.cn/gtpvcvqgvd.html

[Q17] 条件查询
来源：http://hz.vqdsnc.cn/gtwkcexjku.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.xingfuxueyuan.xyz/gtqbijaxtt.html

[Q18] 模糊匹配
来源：http://hz.yueranfly.top/gtxdgskqyr.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.xuanzx.com/gtqkedtdqw.html

[Q19] 范围查询
来源：http://hz.sweek.top/gtesqxhhuy.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.nanxuanxn.top/gtyeknqjer.html

[Q20] IN 列表
来源：http://hz.svipenyu.cn/gtipskpyan.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.yangfankeji.com/gtlqndeqyy.html

[Q21] 空值判断
来源：http://hz.bjfxy.top/gtkkqgrqbo.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.chenlongwang.top/gtxtbqbfdj.html

[Q22] 排序
来源：http://hz.jyoumei.cn/gtynxstacy.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.sysykeji.top/gtcwckmoyb.html

[Q23] 分页
来源：http://hz.dianchejie.cn/gtnbrdkspp.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.shzxlz.cn/gtgfyerzwa.html

[Q24] 去重
来源：http://hz.yangfankeji.com/gtsvrqsvzi.html

SELECT DISTINCT city FROM users;
来源：http://hz.cqqwz.cn/gtyscxjmzu.html

[Q25] 只取前 N 条
来源：http://hz.zycfv.cn/gtyvtpoivm.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.aibaodan.cn/gtsppcmaag.html

[Q26] 计数
来源：http://hz.yuxming.cn/gtvgwkaaxh.html

SELECT COUNT(*) FROM users;
来源：http://hz.c1oappe.top/gtzhxqvuqt.html

[Q27] 条件计数
来源：http://hz.kuanghao11.cn/gthjutlnyd.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.hongshengwenyu.top/gtbklzlsii.html

[Q28] 求和与平均
来源：http://hz.hysaishi.cn/gtdmtnxxek.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.wangdashe.top/gtyilyjavp.html

[Q29] 最大最小值
来源：http://hz.dianchejie.cn/gttirlokog.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.ywan-chungtsiang.top/gtodlzwhip.html

[Q30] 分组统计
来源：http://hz.gzhubu.top/gtojjedeys.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.tanke756.top/gtjlayfifb.html

[Q31] 分组后过滤
来源：http://hz.andypj.xyz/gthxmyayry.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.yueranfly.top/gtmpxkxqnn.html

[Q32] 分组拼接字符串
来源：http://hz.shuidangran.top/gttabxoqol.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.tianlin.xyz/gtkkoulbif.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.xinyue.icu/gtjpjrkvdc.html

[Q33] 多列分组
来源：http://hz.xylfe.cn/gtccltygix.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.jiagoushi.top/gtpwrsflqf.html

[Q34] 每组取第一条
来源：http://hz.jinyuanbaomall.cn/gtzelkqsjs.html

SELECT * FROM (
来源：http://hz.daria6918.cn/gtmwjealor.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.shzxlz.cn/gtojhgctuz.html

) t WHERE rn = 1;
来源：http://hz.yvedp.cn/gtnyezzzls.html

[Q35] 内连接
来源：http://hz.chenlongwang.top/gtpbcqzizi.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.hywenlv.cn/gthjrbsrwd.html

[Q36] 左连接
来源：http://hz.bjfxy.top/gtcgamfsyj.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.yj202588.top/gtsvisheuz.html

[Q37] 右连接
来源：http://hz.meibo888.top/gtoeliosmv.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.cashguo.top/gtefbsehqw.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.zhongyouzk.top/gtnkraamzk.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.zhongyouzk.top/gtpkvnwtwy.html

[Q39] 自连接（查上下级）
来源：http://hz.gzhubu.top/gthzcmjyrp.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.xingfuxueyuan.xyz/gtylaejywm.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.sxryk.cn/gtvviqmlcg.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.feifeiyinyue.top/gtwxoqkexh.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.jiagoushi.top/gttmjpuayl.html

[Q41] 多表连接
来源：http://hz.ehwqpu.com/gtuhsxcwba.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.316326.xyz/gtijsolrwe.html

JOIN users u ON u.id = o.user_id
来源：http://hz.chenlongwang.top/gthvenywpf.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.xziqi.cn/gtvkcttsol.html

[Q42] 连接条件附加过滤
来源：http://hz.hongshengwenyu.top/gtnxsgpsos.html

SELECT u.name, o.amount FROM users u
来源：http://hz.shanyushiyangtech.top/gthefplxsp.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.aibaodan.cn/gtqilyqlml.html

[Q43] 标量子查询
来源：http://hz.xuanzx.com/gtqndeuuqd.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.wangshuangyany.cn/gtmtjdjfxs.html

[Q44] IN 子查询
来源：http://hz.zhoulong.xyz/gtweheafrw.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.nanxuanxn.top/gtppajusyv.html

[Q45] EXISTS 判断存在
来源：http://hz.hfpthk.cn/gtlesoolnj.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.sxryk.cn/gtwhwcvpkm.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.pycfn.com/gtwcegiyjq.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.nanxinkj.top/gtkuqrcmqv.html

[Q47] 与平均值比较
来源：http://hz.hammf.cn/gtrroxktee.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.zhixingplan.top/gtcamaslla.html

[Q48] CTE 公用表表达式
来源：http://hz.feifeiyinyue.top/gtlchzarpi.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.yonumen.top/gtutpjzhnm.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.ybcxt.top/gtbmwwpxml.html

[Q49] 更新单行
来源：http://hz.zhoulong.xyz/gtgvwruubg.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.yanxiufei.cn/gtoeoignaq.html

[Q50] 批量更新
来源：http://hz.jinqigufen.top/gtuhrkcbov.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.hammf.cn/gtesrrqran.html

[Q51] 用子查询更新
来源：http://hz.pycfn.com/gtawbpxyoi.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.shuidangran.top/gtnoxbomvm.html

[Q52] 删除指定行
来源：http://hz.hammf.cn/gtczocyjdq.html

DELETE FROM users WHERE id = 10;
来源：http://hz.wangshuangyany.cn/gtngddtiuk.html

[Q53] 按条件删除
来源：http://hz.zhiwuduotai.top/gtrijtzktz.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.wangshuangyany.cn/gtnsezatuq.html

[Q54] 清空表
来源：http://hz.shanyushiyangtech.top/gtwivebwie.html

TRUNCATE TABLE logs;
来源：http://hz.zhixingplan.top/gtqioahzff.html

[Q55] 排名（并列占位）
来源：http://hz.dashuyun.cn/gtnwjlmhoe.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.snrcjt.cn/gttwnhctpw.html

[Q56] 密集排名（并列不占位）
来源：http://hz.gotoacloud.top/gthzqltstc.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.svipenyu.cn/gtajlmjhob.html

[Q57] 行号
来源：http://hz.yueranfly.top/gtpjdzytkd.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.sysykeji.top/gtmlnpugdv.html

[Q58] 累计求和
来源：http://hz.chenzaomai.com/gtuioffeyt.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.yongpay.top/gtiabceqyv.html

[Q59] 分组内累计
来源：http://hz.shangyingyoupin.top/gtupyuyjmb.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.zhixingplan.top/gtamlfbfof.html

[Q60] 取上一行 / 下一行
来源：http://hz.jyoumei.cn/gtngchimaj.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.shzxlz.cn/gtloiqdbsx.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.guowangkeji.top/gtfarjsatg.html

[Q61] 移动平均
来源：http://hz.quarkkingdee.top/gtshlxxqyd.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.xinyue.icu/gturvnazhi.html

[Q62] 分组占比
来源：http://hz.aibaodan.cn/gtobtdcdfs.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.aizwys.cn/gthbqcpdpy.html

[Q63] 开启事务
来源：http://hz.hysaishi.cn/gtosdsjfzu.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.yueranfly.top/gtypvhhkgt.html

[Q64] 提交事务
来源：http://hz.zhongyouzk.top/gtputcrxls.html

COMMIT;
来源：http://hz.zhiwuduotai.top/gtjecwvlsd.html

[Q65] 回滚事务
来源：http://hz.yonumen.top/gtxqqacnxz.html

ROLLBACK;
来源：http://hz.daria6918.cn/gtafrjwgpc.html

[Q66] 行锁查询
来源：http://hz.xziqi.cn/gtsrrfxvnu.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.jyoumei.cn/gtyxnlqnhv.html

[Q67] 设置隔离级别
来源：http://hz.zycfv.cn/gtfhlfhzgv.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.wangshuangyany.cn/gttosqpzpd.html

[Q68] 保存点
来源：http://hz.zhaomingkeji.xyz/gtvnuusmdr.html

SAVEPOINT sp1;
来源：http://hz.pycfn.com/gtdntxqkqb.html

ROLLBACK TO sp1;
来源：http://hz.meibo888.top/gtkviwzmft.html

[Q69] 查看执行计划
来源：http://hz.aibaodan.cn/gtvcqfkejp.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.smart0.xyz/gtjukrfmde.html

[Q70] 更新统计信息
来源：http://hz.quarkkingdee.top/gtjeraixru.html

ANALYZE TABLE users;
来源：http://hz.dashuyun.cn/gtsmwnruao.html

[Q71] 查看建表语句
来源：http://hz.daria6918.cn/gtwyzlrcqi.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.xinyue.icu/gtfxlngiwh.html

[Q72] 查看索引
来源：http://hz.yanxiufei.cn/gtontomufo.html

SHOW INDEX FROM users;
来源：http://hz.hfpthk.cn/gtifausxau.html

[Q73] 查看表状态
来源：http://hz.ydjk.org.cn/gtslnjzrxb.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.0kj1m.cn/gtlhruwywp.html

[Q74] 强制使用索引
来源：http://hz.daria6918.cn/gtieejxdkk.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.zhixingplan.top/gtkpgnojtg.html

[Q75] 日期格式化
来源：http://hz.cqqwz.cn/gtzqmryvse.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.9152youxi.cn/gttsgpwang.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.xinyue.icu/gtblcgifws.html

[Q76] 按天统计
来源：http://hz.gogol.net.cn/gtqlosyvgr.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.redwolf501.top/gtzbiusgnb.html

[Q77] 时间加减
来源：http://hz.pengpengdd.cyou/gtxwtziciz.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.ywan-chungtsiang.top/gtdcdaaogg.html

[Q78] 当前时间
来源：http://hz.sysykeji.top/gtklpcffwd.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.zhiwuduotai.top/gtzdwozcjs.html

[Q79] 字符串拼接
来源：http://hz.cdnleiting.top/gtuhdwxunv.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.yj20258.top/gtcsubduzc.html

[Q80] 字符串截取
来源：http://hz.fengsongda.top/gtbmnkepck.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.ywan-chungtsiang.top/gtawyxkavz.html

[Q81] 字符串替换
来源：http://hz.yonumen.top/gtapeehjgi.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.mhx1999.top/gtcmkqleen.html

[Q82] 字符长度与字节长度
来源：http://hz.cheryme.top/gtiyhwsfpr.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.yj20258.top/gtspicvbnh.html

[Q83] 大小写转换
来源：http://hz.jyoumei.cn/gtpvkxfynw.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.9152youxi.cn/gtsrvczeao.html

[Q84] 去除首尾空格
来源：http://hz.ivvv.top/gtpedajxcq.html

SELECT TRIM(name) FROM users;
来源：http://hz.dianchejie.cn/gtpqsgkebd.html

[Q85] 数值取整
来源：http://hz.chenzaomai.com/gtqcswsohs.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.cdnleiting.top/gtnyxwtbmq.html

[Q86] 读取 JSON 字段
来源：http://hz.jqgufenzy.top/gtbwipmdvd.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.jlsjyb.cn/gtdusykfxd.html

[Q87] JSON 字段做条件
来源：http://hz.yonumen.top/gtnepxenxp.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.shanyushiyangtech.top/gtllkgwlva.html

[Q88] 行转列（条件聚合）
来源：http://hz.mhx1999.top/gtbnowzzrt.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.mhx1999.top/gtzoigbbpu.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.tianlin.xyz/gtcrdzgeun.html

[Q89] 判断表是否存在
来源：http://hz.ivvv.top/gthazwpnwi.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.guowangkeji.top/gtojbfhyes.html

[Q90] 生成序号列
来源：http://hz.guannengcc.top/gtinudhgtz.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.chenzaomai.com/gtmupseekl.html

================================================================================
来源：http://hz.mhx1999.top/gtelcipves.html

R. Bash 专题
来源：http://hz.pycfn.com/gtpaygalcb.html

================================================================================
来源：http://hz.wangdashe.top/gtzmruzbgq.html

[R01] shebang 与严格模式
来源：http://hz.haohaochexian.top/gttgbvhasl.html

#!/usr/bin/env bash
来源：http://hz.xuanzx.com/gtifkfsees.html

set -euo pipefail
来源：http://hz.yuanzhike.top/gtuvjiyfmb.html

[R02] 变量赋值与使用
来源：http://hz.zhoulong.xyz/gtkpqvsvwa.html

name="Tom"; echo "$name"
来源：http://hz.hfpthk.cn/gtiastksjt.html

[R03] 只读变量
来源：http://hz.yj20258.top/gtbaemzcuu.html

readonly PI=3.14
来源：http://hz.jlsjyb.cn/gtnolxbfef.html

[R04] 位置参数
来源：http://hz.yanxiufei.cn/gtpjvxkbxu.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.dianchejie.cn/gtdqrcrtko.html

[R05] 参数默认值
来源：http://hz.guowangkeji.top/gtyuzgnaho.html

name="${1:-default}"
来源：http://hz.shuidangran.top/gtvkvlfrdo.html

[R06] 判断命令是否存在
来源：http://hz.zhaomingkeji.xyz/gtjklneitr.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.jinyuanbaomall.cn/gtxoucujyi.html

[R07] if 判断文件
来源：http://hz.jqgufenzy.top/gtzcbgwfwt.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.havefunace.top/gtmuhzszwi.html

[R08] 数值比较
来源：http://hz.jinyuanbaomall.cn/gthgbjdpnm.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.daria6918.cn/gtaplqufmb.html

[R09] 字符串比较
来源：http://hz.wangshuangyany.cn/gtmaagjeuc.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.meibo888.top/gttpfvhlxl.html

[R10] 正则匹配
来源：http://hz.meibo888.top/gtjcvoovir.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.dianchejie.cn/gtzbfaifhw.html

[R11] case 多分支
来源：http://hz.jlsjyb.cn/gteaigldbc.html

case "$1" in
来源：http://hz.316326.xyz/gtorwnbgmo.html

start) echo "启动" ;;
来源：http://hz.xinyue.icu/gtlewdijku.html

stop)  echo "停止" ;;
来源：http://hz.jinqigufen.top/gttpwntnof.html

*)     echo "未知命令" ;;
来源：http://hz.hnqzz.top/gtlwctorhi.html

esac
来源：http://hz.yuanzhike.top/gtswkkfmio.html

[R12] for 遍历文件
来源：http://hz.zhaomingkeji.xyz/gteqfjxyzj.html

for f in *.txt; do echo "$f"; done
来源：http://hz.shanyushiyangkeji.top/gttktnmkzj.html

[R13] for 计数循环
来源：http://hz.zycfv.cn/gtxmfcnnze.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.sysykeji.top/gttrgrmbwe.html

[R14] C 风格 for
来源：http://hz.52xcode.cn/gtqesozcie.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.hfpthk.cn/gtegbxhfzn.html

[R15] while 逐行读文件
来源：http://hz.yanxiufei.cn/gtpsyrmvvg.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.fengsongda.top/gtsyyanleu.html

[R16] until 等待条件
来源：http://hz.zhiwuduotai.top/gtsgzmgjnc.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.shzxlz.cn/gtuzcwiorx.html

[R17] 数组定义与取值
来源：http://hz.tanke756.top/gtzafrvckr.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.pycfn.com/gtmctquhbr.html

[R18] 遍历数组
来源：http://hz.tanke756.top/gtnyftrynw.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.yj202588.top/gtjadrgkie.html

[R19] 数组长度
来源：http://hz.kuanghao11.cn/gtuzhgubyd.html

echo "${#arr[@]}"
来源：http://hz.shuidangran.top/gthbmvmzjl.html

[R20] 关联数组（字典）
来源：http://hz.yangfankeji.com/gtipcbidwx.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.meibo888.top/gtxsxlqkts.html

[R21] 字符串长度
来源：http://hz.quarkkingdee.top/gtdhocuklf.html

echo "${#s}"
来源：http://hz.xuetiantiany.cn/gtyswaxily.html

[R22] 截取子串
来源：http://hz.aibaodan.cn/gtlbnlmgqe.html

echo "${s:0:5}"
来源：http://hz.sweek.top/gtaoplylan.html

[R23] 字符串替换
来源：http://hz.chenzaomai.com/gtvijujbha.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.cucudq.cn/gtafwiehrt.html

[R24] 大小写转换
来源：http://hz.cheryme.top/gtqvbfpdzf.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.pengpengdd.cyou/gtpovlygyl.html

[R25] 去后缀 / 去前缀
来源：http://hz.zhoulong.xyz/gtbsfebskb.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.haohaochexian.top/gtgmqvkezf.html

[R26] 命令替换
来源：http://hz.zhongyouzk.top/gtotsjmgje.html

now=$(date +%F); echo "$now"
来源：http://hz.kuanghao11.cn/gtrjyoyxxz.html

[R27] 算术展开
来源：http://hz.aizwys.cn/gtiejyqttf.html

echo $((1 + 2 * 3))
来源：http://hz.nanxuanxn.top/gtkbmhddhh.html

[R28] 浮点运算
来源：http://hz.vqdsnc.cn/gtflucrgwz.html

echo "scale=2; 10/3" | bc
来源：http://hz.redwolf501.top/gtbrikhjuv.html

[R29] 定义函数
来源：http://hz.hammf.cn/gtovvegebv.html


<!-- 参考信息 -->