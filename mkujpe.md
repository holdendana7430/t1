代发 wailian999

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.nanxinkj.top/gtopnueprp.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.zhiwuduotai.top/gtuzaukznp.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.cdnleiting.top/gtypsgetvb.html

Ruby: a == b
来源：http://hz.smart0.xyz/gtgejlvpfb.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.zdqjudy.top/gtpkauanie.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.yuxming.cn/gtqtzlleko.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.cucudq.cn/gttqilkjhx.html

PHP:  if (empty($x)) {}
来源：http://hz.feifeiyinyue.top/gtywbqisvy.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.shanyushiyangkeji.top/gtymypqadw.html

TS:   if (x == null) {}
来源：http://hz.wangshuangyany.cn/gtuwzmnbno.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.zhengqikj.top/gtrzpxusjo.html

Go:   if x == nil {}
来源：http://hz.xuetiantiany.cn/gtrzlbcshq.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.mhx1999.top/gtllaikapr.html

C#:   if (x is null) {}
来源：http://hz.chenjidiqi.icu/gtnxucflbv.html

[P07] 防抖与节流
来源：http://hz.ywan-chungtsiang.top/gtujlxqxwa.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.dianchejie.cn/gtiszqnpcp.html

PHP:  // 手写时间戳比较
来源：http://hz.nwbrower.top/gtuhuinjte.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.chenlongwang.top/gtztcmwrdw.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yj202588.top/gtmakyobru.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.sweek.top/gtzwzzbgaz.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.chenzaomai.com/gtppfuirlw.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.shanyushiyangtech.top/gtajcqdyxa.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.wangshuangyany.cn/gtnbvdsdkw.html

[P08] 处理浮点精度问题
来源：http://hz.daxiang520.top/gtesjljixo.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.pycfn.com/gtmcntygnk.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.sysykeji.top/gtcyfzcate.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.chenlongwang.top/gtqyoqxswx.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.yj20258888.top/gtqrbmtxuv.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.aibaodan.cn/gtbxgzqfkr.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.yj202588.top/gtobypfhmg.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.jlsjyb.cn/gtikcqcybq.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.hammf.cn/gttquipskt.html

================================================================================
来源：http://hz.ydjk.org.cn/gtoirqvcxk.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.aibaodan.cn/gtyjaxrebh.html

================================================================================
来源：http://hz.yongpay.top/gtdxhofeww.html

[Q01] 创建表
来源：http://hz.zhoulong.xyz/gthpaopxdw.html

CREATE TABLE users (
来源：http://hz.hywenlv.cn/gtaulrqcgx.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.hongshengwenyu.top/gtazczttnl.html

name VARCHAR(50) NOT NULL,
来源：http://hz.cashguo.top/gtcdvzlstv.html

email VARCHAR(100) UNIQUE,
来源：http://hz.ppjwa.cn/gtqbpupbyo.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.cucudq.cn/gtptyocnin.html

);
来源：http://hz.zhixingplan.top/gtijhdtomt.html

[Q02] 创建带外键的表
来源：http://hz.sysykeji.top/gttlpatkpm.html

CREATE TABLE orders (
来源：http://hz.316326.xyz/gtaptrixsj.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.wangdashe.top/gtftdanbmx.html

user_id INT NOT NULL,
来源：http://hz.jinqigufen.top/gtnsurwrns.html

amount DECIMAL(10, 2),
来源：http://hz.gaohongyu789.top/gtogtkdzib.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.nanxuanxn.top/gtcnibwhjy.html

);
来源：http://hz.fzhhl.top/gthzkpkkfr.html

[Q03] 增加列
来源：http://hz.shzxlz.cn/gtvxzbtdqz.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.guowangkeji.top/gtqwpqtwdf.html

[Q04] 修改列类型
来源：http://hz.guannengcc.top/gtcqczcpns.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.kuanghao11.cn/gtoepezcdv.html

[Q05] 重命名列
来源：http://hz.daxiang520.top/gtjsaepmpj.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.nanxinkj.top/gtkfxjoeam.html

[Q06] 删除列
来源：http://hz.sweek.top/gtyqbjoplv.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.chenjidiqi.icu/gtlqoagfiw.html

[Q07] 删除表
来源：http://hz.fengsongda.top/gtgjdeuldt.html

DROP TABLE IF EXISTS orders;
来源：http://hz.shanyushiyangkeji.top/gtsepygxhq.html

[Q08] 创建普通索引
来源：http://hz.gzhubu.top/gthanfrabi.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.cheryme.top/gtalaghgjo.html

[Q09] 创建唯一索引
来源：http://hz.hongshengwenyu.top/gtnmchhycf.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.pengpengdd.cyou/gtwkxadumr.html

[Q10] 插入单行
来源：http://hz.sweek.top/gttnwaletp.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.cucudq.cn/gtnugfazps.html

[Q11] 一次插入多行
来源：http://hz.nanxinkj.top/gtstnfyvgi.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.shanyushiyangtech.top/gtnxnpferx.html

[Q12] 插入后取自增 ID
来源：http://hz.c1oappe.top/gtrnqcxcao.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.vqdsnc.cn/gtcqhfmncy.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.yuanzhike.top/gtqerykgaq.html

[Q13] 忽略重复插入
来源：http://hz.52xcode.cn/gtulzjptwe.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.yj202588.top/gtzsmnjgdn.html

[Q14] 存在则更新（upsert）
来源：http://hz.aizwys.cn/gtifjzokkn.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.nanxinkj.top/gtwtchhbia.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.9152youxi.cn/gtqbrrrjge.html

[Q15] 查询全部
来源：http://hz.snrcjt.cn/gtbjksqyyd.html

SELECT * FROM users;
来源：http://hz.c1oappe.top/gtarpgkujp.html

[Q16] 查询指定列
来源：http://hz.dianchejie.cn/gtdwixumlp.html

SELECT id, name FROM users;
来源：http://hz.tianlin.xyz/gtqvgvezxj.html

[Q17] 条件查询
来源：http://hz.sufxvd.cn/gtyivxoctx.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.sysykeji.top/gtxsvrrmdl.html

[Q18] 模糊匹配
来源：http://hz.guannengcc.top/gtdcwweime.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.haohaochexian.top/gtkfrebqqp.html

[Q19] 范围查询
来源：http://hz.vqdsnc.cn/gttrgbsnyh.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.guannengcc.top/gtzsnbbzcq.html

[Q20] IN 列表
来源：http://hz.chenzaomai.com/gtgfbpmxxd.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.zdqjudy.top/gtfbumwulh.html

[Q21] 空值判断
来源：http://hz.havefunace.top/gtiekhvdee.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.c1oappe.top/gtpymezvsu.html

[Q22] 排序
来源：http://hz.tanke756.top/gtqbxqlcvz.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.c1oappe.top/gtejhizozs.html

[Q23] 分页
来源：http://hz.yuanzhike.top/gtsaxnmkza.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.jianghu66.top/gthaigyest.html

[Q24] 去重
来源：http://hz.pycfn.com/gtglishkko.html

SELECT DISTINCT city FROM users;
来源：http://hz.ydzc1.top/gttwxviygq.html

[Q25] 只取前 N 条
来源：http://hz.pengpengdd.cyou/gtnuixdmhx.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.bjfxy.top/gtcgtpcgki.html

[Q26] 计数
来源：http://hz.shanyushiyangtech.top/gtjudbyrvn.html

SELECT COUNT(*) FROM users;
来源：http://hz.mhx1999.top/gtyfxipook.html

[Q27] 条件计数
来源：http://hz.jqgufenzy.top/gtbdtrflgw.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.yj202588.top/gtchpqbcii.html

[Q28] 求和与平均
来源：http://hz.hammf.cn/gtebsqeolj.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.kuanghao11.cn/gttrfetrfr.html

[Q29] 最大最小值
来源：http://hz.cdnleiting.top/gtbghbpkcu.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.smart0.xyz/gtujgnzgky.html

[Q30] 分组统计
来源：http://hz.feifeiyinyue.top/gtzrzkgntl.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.tanke756.top/gtcybjquyr.html

[Q31] 分组后过滤
来源：http://hz.xuetiantiany.cn/gtyiuetlld.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.ivvv.top/gtpuualqpb.html

[Q32] 分组拼接字符串
来源：http://hz.zhiwuduotai.top/gtkwmkbnir.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.yj20258888.top/gtizonnaxm.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.xingfuxueyuan.xyz/gtyebtbksx.html

[Q33] 多列分组
来源：http://hz.shuidangran.top/gtjtvouodl.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.xziqi.cn/gtdjcgkhup.html

[Q34] 每组取第一条
来源：http://hz.vqdsnc.cn/gtbssrwfgt.html

SELECT * FROM (
来源：http://hz.nanxinkj.top/gttxvxfmre.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.guannengcc.top/gtleipxjbi.html

) t WHERE rn = 1;
来源：http://hz.yj202588.top/gtkjzfdcvs.html

[Q35] 内连接
来源：http://hz.wangshuangyany.cn/gtqpuatimf.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.yvedp.cn/gteogvcsrd.html

[Q36] 左连接
来源：http://hz.nanxinkj.top/gtngffjtvi.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.yvedp.cn/gtcpgcgrvv.html

[Q37] 右连接
来源：http://hz.vqdsnc.cn/gtdpxqoikb.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.jiagoushi.top/gtvhhxmwso.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.smart0.xyz/gtqnghwlci.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.tian-w.cn/gtbrjrbbsl.html

[Q39] 自连接（查上下级）
来源：http://hz.meibo888.top/gtyiyzvlik.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.wangshuangyany.cn/gtpgelpufj.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.yuxming.cn/gtpogejqzd.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.dianchejie.cn/gtwnywojmm.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.shzxlz.cn/gtgfxagekq.html

[Q41] 多表连接
来源：http://hz.shanyushiyangtech.top/gtzdqbiykg.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.xuetiantiany.cn/gtsyrqqanv.html

JOIN users u ON u.id = o.user_id
来源：http://hz.52xcode.cn/gtvejhirqy.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.daxiang520.top/gtzahtpenk.html

[Q42] 连接条件附加过滤
来源：http://hz.yangfankeji.com/gtlliqllcc.html

SELECT u.name, o.amount FROM users u
来源：http://hz.birdmap.top/gtqcyaasxr.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.iojbl.cn/gtafjtmnro.html

[Q43] 标量子查询
来源：http://hz.gogol.net.cn/gtjfywenvp.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.ppjwa.cn/gtvsfrsasa.html

[Q44] IN 子查询
来源：http://hz.yuanzhike.top/gtibpqefrx.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.smart0.xyz/gthuwkaiwa.html

[Q45] EXISTS 判断存在
来源：http://hz.haohaochexian.top/gthpnbuacr.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jinqigufen.top/gtklwlarov.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.fzhhl.top/gthrmkminx.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.dianchejie.cn/gtzlzywpvp.html

[Q47] 与平均值比较
来源：http://hz.wangdashe.top/gtmyvnbszy.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.chenjidiqi.icu/gtkeviliix.html

[Q48] CTE 公用表表达式
来源：http://hz.shangyingyoupin.top/gtpxeuojed.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.mhx1999.top/gtqpvcfrki.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.ehwqpu.com/gtoxkvbzar.html

[Q49] 更新单行
来源：http://hz.jianghu66.top/gtcpumoccn.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.jyoumei.cn/gtichulhda.html

[Q50] 批量更新
来源：http://hz.ybcxt.top/gtnnsowfza.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.andypj.xyz/gtivdyxnsb.html

[Q51] 用子查询更新
来源：http://hz.316326.xyz/gtagxqskpq.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.nwbrower.top/gtaempzxzo.html

[Q52] 删除指定行
来源：http://hz.zycfv.cn/gtebvslboe.html

DELETE FROM users WHERE id = 10;
来源：http://hz.hywenlv.cn/gtvqrhslyq.html

[Q53] 按条件删除
来源：http://hz.havefunace.top/gtrdgaowsq.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.zhongyouzk.top/gtjtpzwcrz.html

[Q54] 清空表
来源：http://hz.sysykeji.top/gtfmtxepod.html

TRUNCATE TABLE logs;
来源：http://hz.zhoulong.xyz/gtwamcspcl.html

[Q55] 排名（并列占位）
来源：http://hz.hnqzz.top/gtiwrgpudd.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.dianchejie.cn/gtjouvvfih.html

[Q56] 密集排名（并列不占位）
来源：http://hz.sweek.top/gtsdvzcdjv.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.svipenyu.cn/gtnmypfwps.html

[Q57] 行号
来源：http://hz.ydjk.org.cn/gttfpukqhu.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.zhaomingkeji.xyz/gtnzcpvior.html

[Q58] 累计求和
来源：http://hz.0kj1m.cn/gtevkczljw.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.chenjidiqi.icu/gthmqiwoxd.html

[Q59] 分组内累计
来源：http://hz.aizwys.cn/gtcouyhljc.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.jinghuilouyu.cn/gtqjkkatki.html

[Q60] 取上一行 / 下一行
来源：http://hz.snrcjt.cn/gtxzrxuqik.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.zhiwuduotai.top/gtubfopozh.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.quarkkingdee.top/gtmouaathj.html

[Q61] 移动平均
来源：http://hz.zhiwuduotai.top/gtxcbnkike.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.hnqzz.top/gtawfjqhzx.html

[Q62] 分组占比
来源：http://hz.yanxiufei.cn/gtcfcwfufq.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.sxryk.cn/gtgtvphxsj.html

[Q63] 开启事务
来源：http://hz.guowangkeji.top/gtrahxmcnw.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.316326.xyz/gtcmcqpyvb.html

[Q64] 提交事务
来源：http://hz.chenzaomai.com/gtwcrrkrqg.html

COMMIT;
来源：http://hz.yj202588.top/gtsszndrlf.html

[Q65] 回滚事务
来源：http://hz.hywenlv.cn/gtjrnazuup.html

ROLLBACK;
来源：http://hz.pengpengdd.cyou/gtgyqnfsav.html

[Q66] 行锁查询
来源：http://hz.yueranfly.top/gtgcztjsyh.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.havefunace.top/gtcdahwjjr.html

[Q67] 设置隔离级别
来源：http://hz.tian-w.cn/gtexhgogki.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.daxiang520.top/gtqbcyguob.html

[Q68] 保存点
来源：http://hz.yangfankeji.com/gtffijfrey.html

SAVEPOINT sp1;
来源：http://hz.jinqigufen.top/gtsiftjnur.html

ROLLBACK TO sp1;
来源：http://hz.jlsjyb.cn/gtzelpofky.html

[Q69] 查看执行计划
来源：http://hz.zycfv.cn/gtfgmjwlgw.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.zhixingplan.top/gtwxqfiyup.html

[Q70] 更新统计信息
来源：http://hz.hywenlv.cn/gtxvdhprae.html

ANALYZE TABLE users;
来源：http://hz.dashuyun.cn/gtucisjutq.html

[Q71] 查看建表语句
来源：http://hz.gaohongyu789.top/gtvagzears.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.daxiang520.top/gtuljjzyjh.html

[Q72] 查看索引
来源：http://hz.quarkkingdee.top/gtxrnjynww.html

SHOW INDEX FROM users;
来源：http://hz.iojbl.cn/gteqpqmiok.html

[Q73] 查看表状态
来源：http://hz.c1oappe.top/gtlrnqnrmw.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.fzhhl.top/gtpabaaedi.html

[Q74] 强制使用索引
来源：http://hz.jianghu66.top/gtxvwutkhg.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.yj202588.top/gtpfofquyx.html

[Q75] 日期格式化
来源：http://hz.sweek.top/gtuxzxpqll.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.cheryme.top/gtwivdrflo.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.andypj.xyz/gtlytrxgve.html

[Q76] 按天统计
来源：http://hz.nanxuanxn.top/gtxvswjgld.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.wangdashe.top/gtxoclicwx.html

[Q77] 时间加减
来源：http://hz.pycfn.com/gtpfigscqu.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.jqgfzy.top/gtienqqeuo.html

[Q78] 当前时间
来源：http://hz.jianghu66.top/gtszllyyve.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.vqdsnc.cn/gtpixtxhaf.html

[Q79] 字符串拼接
来源：http://hz.dashuyun.cn/gtkmeksxnw.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.0kj1m.cn/gtwraxwrxh.html

[Q80] 字符串截取
来源：http://hz.gaohongyu789.top/gthwchpxgs.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.vqdsnc.cn/gtqgisyuop.html

[Q81] 字符串替换
来源：http://hz.316326.xyz/gtmdllihgf.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.guannengcc.top/gtoobhabnm.html

[Q82] 字符长度与字节长度
来源：http://hz.cashguo.top/gtgskrbfvs.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.sysykeji.top/gtjalvvjtg.html

[Q83] 大小写转换
来源：http://hz.shanyushiyangtech.top/gtnqhvajpa.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.hysaishi.cn/gtydlmtxah.html

[Q84] 去除首尾空格
来源：http://hz.sysykeji.top/gtiignlivb.html

SELECT TRIM(name) FROM users;
来源：http://hz.zhixingplan.top/gtykyluxmb.html

[Q85] 数值取整
来源：http://hz.iojbl.cn/gtqwgxnyhi.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.tianlin.xyz/gtvjtpnrtt.html

[Q86] 读取 JSON 字段
来源：http://hz.dianchejie.cn/gtunriusaj.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.svipenyu.cn/gtbxfhgvgk.html

[Q87] JSON 字段做条件
来源：http://hz.guannengcc.top/gtgyqaooxk.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.tianlin.xyz/gtuufsbbmm.html

[Q88] 行转列（条件聚合）
来源：http://hz.tianlin.xyz/gtecpkqcvf.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.zhengqikj.top/gtjmykfnfu.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.yvedp.cn/gtofinzeye.html

[Q89] 判断表是否存在
来源：http://hz.nanxinkj.top/gtpeushdnf.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.guowangkeji.top/gtwalblqqe.html

[Q90] 生成序号列
来源：http://hz.jyoumei.cn/gtvabcjaxv.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.nanxuanxn.top/gtsjmqyman.html

================================================================================
来源：http://hz.yueranfly.top/gtkqcbokak.html

R. Bash 专题
来源：http://hz.ppjwa.cn/gtjpaxpxxj.html

================================================================================
来源：http://hz.316326.xyz/gtlkcnieaj.html

[R01] shebang 与严格模式
来源：http://hz.meibo888.top/gtsrnrrkid.html

#!/usr/bin/env bash
来源：http://hz.zhiwuduotai.top/gtljbamjgq.html

set -euo pipefail
来源：http://hz.xingfuxueyuan.xyz/gtrmrrmxwu.html

[R02] 变量赋值与使用
来源：http://hz.aizwys.cn/gtejhjjcvo.html

name="Tom"; echo "$name"
来源：http://hz.zhengqikj.top/gtlwelyiii.html

[R03] 只读变量
来源：http://hz.cheryme.top/gtxrfkfgil.html

readonly PI=3.14
来源：http://hz.gogol.net.cn/gtgeqvgqqr.html

[R04] 位置参数
来源：http://hz.sxryk.cn/gtttvzkdxb.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.zhaomingkeji.xyz/gthzgmcitn.html

[R05] 参数默认值
来源：http://hz.bjfxy.top/gtelrcmcva.html

name="${1:-default}"
来源：http://hz.smart0.xyz/gtyjcuhatb.html

[R06] 判断命令是否存在
来源：http://hz.c1oappe.top/gtmaizwxsf.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.ydjk.org.cn/gtcxgbnyzc.html

[R07] if 判断文件
来源：http://hz.andypj.xyz/gtgylegviq.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.zhiwuduotai.top/gtjoafhcwu.html

[R08] 数值比较
来源：http://hz.kuanghao11.cn/gtkkgdqazt.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.dianchejie.cn/gtmrijpkex.html

[R09] 字符串比较
来源：http://hz.shanyushiyangtech.top/gtimlfcgaa.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.9152youxi.cn/gtjtuumqzd.html

[R10] 正则匹配
来源：http://hz.andypj.xyz/gtezixqdta.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.dashuyun.cn/gtslzdoqya.html

[R11] case 多分支
来源：http://hz.cqqwz.cn/gtupaifdlm.html

case "$1" in
来源：http://hz.fengsongda.top/gtxzypzvtx.html

start) echo "启动" ;;
来源：http://hz.hnqzz.top/gtilwmugeo.html

stop)  echo "停止" ;;
来源：http://hz.dashuyun.cn/gtdxcxquia.html

*)     echo "未知命令" ;;
来源：http://hz.wangdashe.top/gtqfzqxses.html

esac
来源：http://hz.jqgfzy.top/gtrdeobclo.html

[R12] for 遍历文件
来源：http://hz.guannengcc.top/gtujwgqgyh.html

for f in *.txt; do echo "$f"; done
来源：http://hz.tianlin.xyz/gtycmmgcod.html

[R13] for 计数循环
来源：http://hz.sweek.top/gtywgkocta.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.meibo888.top/gtmxtratdi.html

[R14] C 风格 for
来源：http://hz.yj20258888.top/gtxyqgwkjf.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.c1oappe.top/gtwfwgxfkq.html

[R15] while 逐行读文件
来源：http://hz.yj202588.top/gtdyjluosh.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.meibo888.top/gtrmvtylzu.html

[R16] until 等待条件
来源：http://hz.gaohongyu789.top/gtllwjewbj.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.cqqwz.cn/gtofbhrmyh.html

[R17] 数组定义与取值
来源：http://hz.jianghu66.top/gtkrrxxtwd.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.mhx1999.top/gtkkftutuz.html

[R18] 遍历数组
来源：http://hz.shuidangran.top/gtpxoqclug.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.tian-w.cn/gtcxhskoaj.html

[R19] 数组长度
来源：http://hz.jqgfzy.top/gtwwnxzilk.html

echo "${#arr[@]}"
来源：http://hz.tian-w.cn/gtejjanaiz.html

[R20] 关联数组（字典）
来源：http://hz.daria6918.cn/gttupxrwpq.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.pengpengdd.cyou/gtflrngghk.html

[R21] 字符串长度
来源：http://hz.yongpay.top/gtiiiqkbhm.html

echo "${#s}"
来源：http://hz.chenlongwang.top/gtkrqkojlr.html

[R22] 截取子串
来源：http://hz.gogol.net.cn/gtcpidxapf.html

echo "${s:0:5}"
来源：http://hz.shzxlz.cn/gtwckszufs.html

[R23] 字符串替换
来源：http://hz.yj20258.top/gthkyyxajk.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.jinyuanbaomall.cn/gtujskkpbs.html

[R24] 大小写转换
来源：http://hz.haohaochexian.top/gthjcczufd.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.jlsjyb.cn/gtferugbcq.html

[R25] 去后缀 / 去前缀
来源：http://hz.cdnleiting.top/gtqzatcenr.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.bjfxy.top/gtucwsciga.html

[R26] 命令替换
来源：http://hz.jinghuilouyu.cn/gtwffwajat.html

now=$(date +%F); echo "$now"
来源：http://hz.xingfuxueyuan.xyz/gthyvqjhlh.html

[R27] 算术展开
来源：http://hz.guowangkeji.top/gttduessmj.html


<!-- 参考信息 -->