代发 wailian999

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.dashuyun.cn/gtfmrmyycp.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.pycfn.com/gtytemffdc.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.jiagoushi.top/gtubstsqux.html

Ruby: a == b
来源：http://hz.sxryk.cn/gtwsemwmhj.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.yongpay.top/gthnmpinzq.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.shuidangran.top/gtyfaxabim.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.iojbl.cn/gtifvbieht.html

PHP:  if (empty($x)) {}
来源：http://hz.aizwys.cn/gtdyxctngg.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.yj20258888.top/gtkzqyrjvt.html

TS:   if (x == null) {}
来源：http://hz.quarkkingdee.top/gtvtnllhup.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.52xcode.cn/gtswmaetul.html

Go:   if x == nil {}
来源：http://hz.guowangkeji.top/gtdiobdsso.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.jqgfzy.top/gtamqqdpsu.html

C#:   if (x is null) {}
来源：http://hz.yvedp.cn/gtqyyetpju.html

[P07] 防抖与节流
来源：http://hz.yvedp.cn/gtnemfraxv.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.xziqi.cn/gtilcgxpvg.html

PHP:  // 手写时间戳比较
来源：http://hz.pengpengdd.cyou/gtbzlqldfn.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.nanxinkj.top/gtvsfuyrby.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yongpay.top/gtywkenyek.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.ybcxt.top/gtvfvyhmsr.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.nanxinkj.top/gteelwubng.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.jinqigfzy.top/gtchewudph.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.nanxinkj.top/gtqxenignw.html

[P08] 处理浮点精度问题
来源：http://hz.xuanzx.com/gtytquvjmy.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.tian-w.cn/gtezzxxvqg.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.andypj.xyz/gtdbomnksq.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.jinghuilouyu.cn/gtjepvypmy.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.yuanzhike.top/gtjnxiooea.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.andypj.xyz/gtyvicatkz.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.yj202588.top/gtaxcpxhmb.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.dianchejie.cn/gtpqwpxzqs.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.nanxinkj.top/gtpumcugbr.html

================================================================================
来源：http://hz.zhengqikj.top/gtfwryngnw.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.shuidangran.top/gtqihhddqy.html

================================================================================
来源：http://hz.aizwys.cn/gtiovgapwu.html

[Q01] 创建表
来源：http://hz.zhiwuduotai.top/gtzfabytfd.html

CREATE TABLE users (
来源：http://hz.zhixingplan.top/gtsctegozu.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.havefunace.top/gtovqiwupq.html

name VARCHAR(50) NOT NULL,
来源：http://hz.jinghuilouyu.cn/gtymaotwrq.html

email VARCHAR(100) UNIQUE,
来源：http://hz.wangshuangyany.cn/gtfvhhfqvn.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.smart0.xyz/gtcdqhwicq.html

);
来源：http://hz.haohaochexian.top/gtcledcrnw.html

[Q02] 创建带外键的表
来源：http://hz.hysaishi.cn/gtrivrayuh.html

CREATE TABLE orders (
来源：http://hz.kuanghao11.cn/gtgxhyvikb.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.shanyushiyangkeji.top/gtvrjdrrht.html

user_id INT NOT NULL,
来源：http://hz.yanxiufei.cn/gtoipimiqr.html

amount DECIMAL(10, 2),
来源：http://hz.wangshuangyany.cn/gttdloyzew.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.smart0.xyz/gtxgdcejcd.html

);
来源：http://hz.yangfankeji.com/gtyrcqcbut.html

[Q03] 增加列
来源：http://hz.jqgufenzy.top/gtrmfuxzqz.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.yangfankeji.com/gtqvmtaztl.html

[Q04] 修改列类型
来源：http://hz.xinyue.icu/gtvcgyhqxe.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.pengpengdd.cyou/gtwjdxuhwe.html

[Q05] 重命名列
来源：http://hz.yanxiufei.cn/gtcfpqdcvi.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.zhijiandao.cn/gthnqwhulv.html

[Q06] 删除列
来源：http://hz.wangdashe.top/gtvjtesmfu.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.chenlongwang.top/gtmklbjavj.html

[Q07] 删除表
来源：http://hz.hammf.cn/gtbrpuheki.html

DROP TABLE IF EXISTS orders;
来源：http://hz.zycfv.cn/gttfukrmbq.html

[Q08] 创建普通索引
来源：http://hz.cdnleiting.top/gtnwbotozl.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.cqqwz.cn/gteenvxxih.html

[Q09] 创建唯一索引
来源：http://hz.dianchejie.cn/gttsxaqpxq.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.chenjidiqi.icu/gtygdefiqg.html

[Q10] 插入单行
来源：http://hz.jinqigufen.top/gtttdpzanp.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.tian-w.cn/gtjxpyvpvh.html

[Q11] 一次插入多行
来源：http://hz.sufxvd.cn/gtliebznnu.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.andypj.xyz/gtajfagbjq.html

[Q12] 插入后取自增 ID
来源：http://hz.xinyue.icu/gtxrvzwqam.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.yj20258.top/gtxsleosnd.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.xingfuxueyuan.xyz/gtnbmxwerp.html

[Q13] 忽略重复插入
来源：http://hz.ybcxt.top/gtizaasdwf.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.tianlin.xyz/gtkcckcjid.html

[Q14] 存在则更新（upsert）
来源：http://hz.xuanzx.com/gtptuahmda.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.quarkkingdee.top/gtdivtmhzh.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.yangfankeji.com/gtmleuclmz.html

[Q15] 查询全部
来源：http://hz.hywenlv.cn/gtiyuxkxyz.html

SELECT * FROM users;
来源：http://hz.jiagoushi.top/gtnxteijvt.html

[Q16] 查询指定列
来源：http://hz.nwbrower.top/gtxomjtqrz.html

SELECT id, name FROM users;
来源：http://hz.svipenyu.cn/gtkdmkxuaq.html

[Q17] 条件查询
来源：http://hz.zhengqikj.top/gtxrrqmasc.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.yj202588.top/gtguytoacg.html

[Q18] 模糊匹配
来源：http://hz.zdqjudy.top/gtudefgkyv.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.sxryk.cn/gtwsgldrcm.html

[Q19] 范围查询
来源：http://hz.sxryk.cn/gtqlnqncan.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.jinqigufen.top/gtubmbwikn.html

[Q20] IN 列表
来源：http://hz.wangshuangyany.cn/gtbmenhvqx.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.kuanghao11.cn/gtrpinhvxw.html

[Q21] 空值判断
来源：http://hz.aizwys.cn/gtuoydgcgi.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.ivvv.top/gtrtgdpgim.html

[Q22] 排序
来源：http://hz.sweek.top/gteunwqjfx.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.yuanzhike.top/gtkpuuszeu.html

[Q23] 分页
来源：http://hz.andypj.xyz/gtlbzjuyhq.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.hywenlv.cn/gtkjfesoot.html

[Q24] 去重
来源：http://hz.kuanghao11.cn/gtbtytivfc.html

SELECT DISTINCT city FROM users;
来源：http://hz.meibo888.top/gtgqxxppke.html

[Q25] 只取前 N 条
来源：http://hz.jqgfzy.top/gtdsgsufmu.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.cheryme.top/gtthmnxqnm.html

[Q26] 计数
来源：http://hz.shangyingyoupin.top/gtophhbehe.html

SELECT COUNT(*) FROM users;
来源：http://hz.ivvv.top/gtgkcnmlyj.html

[Q27] 条件计数
来源：http://hz.shanyushiyangtech.top/gtfsnnmodc.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.zycfv.cn/gtlnksaxvd.html

[Q28] 求和与平均
来源：http://hz.iojbl.cn/gtwoawkfnp.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.pycfn.com/gtxvsuquxr.html

[Q29] 最大最小值
来源：http://hz.yanxiufei.cn/gtjqrfxgmv.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.hnxiangtu.top/gtsextyiny.html

[Q30] 分组统计
来源：http://hz.hammf.cn/gtlckxzqxv.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.hysaishi.cn/gtlbncotpw.html

[Q31] 分组后过滤
来源：http://hz.yonumen.top/gtpipstgfl.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.pengpengdd.cyou/gtimdsnevu.html

[Q32] 分组拼接字符串
来源：http://hz.yj202588.top/gtnbailxyx.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.meibo888.top/gtbgbkwkgv.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.daria6918.cn/gturpusdhc.html

[Q33] 多列分组
来源：http://hz.gaohongyu789.top/gtplsjbysw.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.shanyushiyangtech.top/gtkhxmagix.html

[Q34] 每组取第一条
来源：http://hz.andypj.xyz/gtzztlpwwk.html

SELECT * FROM (
来源：http://hz.chenlongwang.top/gtypycszjl.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.gogol.net.cn/gtsjrfxeyp.html

) t WHERE rn = 1;
来源：http://hz.snrcjt.cn/gtvdcdkksg.html

[Q35] 内连接
来源：http://hz.sweek.top/gtkjcbfkaw.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.cheryme.top/gtlegsjchq.html

[Q36] 左连接
来源：http://hz.shanyushiyangkeji.top/gtvpdgvaoq.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.jqgfzy.top/gtawldjbpr.html

[Q37] 右连接
来源：http://hz.redwolf501.top/gtxtddpeba.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.kuanghao11.cn/gtgmwlpzmk.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.wangshuangyany.cn/gtfoerluvj.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.iojbl.cn/gtoqgvcocr.html

[Q39] 自连接（查上下级）
来源：http://hz.nanxinkj.top/gtrksjlhft.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.zycfv.cn/gtapwfpjug.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.hongshengwenyu.top/gtqgxtxifd.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.vqdsnc.cn/gtajgcybpt.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.snrcjt.cn/gtetadnipx.html

[Q41] 多表连接
来源：http://hz.shanyushiyangkeji.top/gtfyvcdvme.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.yanxiufei.cn/gtdiewsjzr.html

JOIN users u ON u.id = o.user_id
来源：http://hz.nanxuanxn.top/gtvpovxpzw.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.wangdashe.top/gttjldasso.html

[Q42] 连接条件附加过滤
来源：http://hz.ehwqpu.com/gtwtytkert.html

SELECT u.name, o.amount FROM users u
来源：http://hz.bjfxy.top/gtvycpppke.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.fzhhl.top/gtofeiwiov.html

[Q43] 标量子查询
来源：http://hz.kuanghao11.cn/gtllcntsxc.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.yuxming.cn/gtfccbavbi.html

[Q44] IN 子查询
来源：http://hz.hywenlv.cn/gthwvipjzl.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.gzhubu.top/gtglzbqcsl.html

[Q45] EXISTS 判断存在
来源：http://hz.wangshuangyany.cn/gtejyixtyk.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.dashuyun.cn/gtnhrqouxe.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.hnqzz.top/gtieawsirg.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.sweek.top/gtlipvxgeb.html

[Q47] 与平均值比较
来源：http://hz.tian-w.cn/gtxebajyyn.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.fzhhl.top/gtpjswklfn.html

[Q48] CTE 公用表表达式
来源：http://hz.sufxvd.cn/gtostpwqai.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.chenzaomai.com/gtvszgpiuo.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.birdmap.top/gtbqfqzzcw.html

[Q49] 更新单行
来源：http://hz.cqqwz.cn/gtnmauqnnt.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.jqgufenzy.top/gtdvrpewfu.html

[Q50] 批量更新
来源：http://hz.hnqzz.top/gtkacwylnw.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.zycfv.cn/gtvzpavbju.html

[Q51] 用子查询更新
来源：http://hz.jlsjyb.cn/gtddliawmd.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.hnqzz.top/gttyvnojtj.html

[Q52] 删除指定行
来源：http://hz.chenlongwang.top/gttnisdwwg.html

DELETE FROM users WHERE id = 10;
来源：http://hz.hongshengwenyu.top/gtrciidjvi.html

[Q53] 按条件删除
来源：http://hz.kuanghao11.cn/gteocyplqd.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.jiagoushi.top/gtvpbklskt.html

[Q54] 清空表
来源：http://hz.jyoumei.cn/gtrkkaobvs.html

TRUNCATE TABLE logs;
来源：http://hz.iojbl.cn/gtjjkxbmut.html

[Q55] 排名（并列占位）
来源：http://hz.smart0.xyz/gtxofxatwe.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.birdmap.top/gtrpjwecji.html

[Q56] 密集排名（并列不占位）
来源：http://hz.zhengqikj.top/gtksuviwpt.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.ybcxt.top/gtvmmmyiss.html

[Q57] 行号
来源：http://hz.316326.xyz/gtunqenswl.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.jianghu66.top/gtwqlkjsyt.html

[Q58] 累计求和
来源：http://hz.xuanzx.com/gtaxyhwbjk.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.birdmap.top/gtuyhbexdk.html

[Q59] 分组内累计
来源：http://hz.cqqwz.cn/gtquekeila.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.jinqigufen.top/gtjzeffdxz.html

[Q60] 取上一行 / 下一行
来源：http://hz.haohaochexian.top/gtkwjdcmvh.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.xuanzx.com/gtusiathre.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.zhengqikj.top/gtqxhxvvqx.html

[Q61] 移动平均
来源：http://hz.sweek.top/gtdkshmxtb.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.cashguo.top/gtoyqfnbip.html

[Q62] 分组占比
来源：http://hz.zycfv.cn/gtyorlfryw.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.xinyue.icu/gthpncboso.html

[Q63] 开启事务
来源：http://hz.havefunace.top/gtduscmrcc.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.zhengqikj.top/gtxluftysq.html

[Q64] 提交事务
来源：http://hz.jqgfzy.top/gtynourdsa.html

COMMIT;
来源：http://hz.aizwys.cn/gtebogrgnw.html

[Q65] 回滚事务
来源：http://hz.yangfankeji.com/gtexrsckip.html

ROLLBACK;
来源：http://hz.smart0.xyz/gtuxiztqdr.html

[Q66] 行锁查询
来源：http://hz.hfpthk.cn/gtnhrqudds.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.cdnleiting.top/gtsdtfnira.html

[Q67] 设置隔离级别
来源：http://hz.sufxvd.cn/gtkvjcdyrc.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.c1oappe.top/gttbanyzhk.html

[Q68] 保存点
来源：http://hz.jqgufenzy.top/gtrgwusalt.html

SAVEPOINT sp1;
来源：http://hz.ehwqpu.com/gtkfrrdtzy.html

ROLLBACK TO sp1;
来源：http://hz.shanyushiyangkeji.top/gtzkbtsaoi.html

[Q69] 查看执行计划
来源：http://hz.daxiang520.top/gtdxdaczgv.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.zhixingplan.top/gtcllchpgy.html

[Q70] 更新统计信息
来源：http://hz.aibaodan.cn/gtjjlozxwf.html

ANALYZE TABLE users;
来源：http://hz.zdqjudy.top/gtwnsbofhr.html

[Q71] 查看建表语句
来源：http://hz.quarkkingdee.top/gtxbvpkgvj.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.hywenlv.cn/gtmiayoyxw.html

[Q72] 查看索引
来源：http://hz.jinqigufen.top/gtutuyndwr.html

SHOW INDEX FROM users;
来源：http://hz.andypj.xyz/gtwipoqnfe.html

[Q73] 查看表状态
来源：http://hz.gogol.net.cn/gtpntzyoxu.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.yonumen.top/gtfbmknmoz.html

[Q74] 强制使用索引
来源：http://hz.fzhhl.top/gtrxpykrgt.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.zhixingplan.top/gtdeqkepwb.html

[Q75] 日期格式化
来源：http://hz.wangshuangyany.cn/gtekxoglcr.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.hysaishi.cn/gtprjcqbrt.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.svipenyu.cn/gtyvfkdeoo.html

[Q76] 按天统计
来源：http://hz.quarkkingdee.top/gtqlbqgpsr.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.cqqwz.cn/gtyskhtvnp.html

[Q77] 时间加减
来源：http://hz.zhongyouzk.top/gtbqhsrujt.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.jqgfzy.top/gtgnfynhsf.html

[Q78] 当前时间
来源：http://hz.meibo888.top/gtcyrfstty.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.yuanzhike.top/gtsekayphv.html

[Q79] 字符串拼接
来源：http://hz.hammf.cn/gthzvtixdr.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.zhongyouzk.top/gtamjywdsa.html

[Q80] 字符串截取
来源：http://hz.zhiwuduotai.top/gttlivsmmk.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.zhixingplan.top/gtyijxdzzk.html

[Q81] 字符串替换
来源：http://hz.ehwqpu.com/gtuqigxjlz.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.pycfn.com/gtbnzvlnwq.html

[Q82] 字符长度与字节长度
来源：http://hz.hywenlv.cn/gtnaysidln.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.feifeiyinyue.top/gtfuknktud.html

[Q83] 大小写转换
来源：http://hz.ppjwa.cn/gtjcoekltm.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.hywenlv.cn/gtkzhrykxm.html

[Q84] 去除首尾空格
来源：http://hz.iojbl.cn/gtkbzmmzif.html

SELECT TRIM(name) FROM users;
来源：http://hz.yongpay.top/gtvevnuayn.html

[Q85] 数值取整
来源：http://hz.nwbrower.top/gtjdpxkugk.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.havefunace.top/gthrvkecku.html

[Q86] 读取 JSON 字段
来源：http://hz.jinqigufen.top/gtpmbfacvh.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.xziqi.cn/gtyzgexovd.html

[Q87] JSON 字段做条件
来源：http://hz.yueranfly.top/gtksvdepge.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.ywan-chungtsiang.top/gtwksxzlmx.html

[Q88] 行转列（条件聚合）
来源：http://hz.sufxvd.cn/gtshnshpjt.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.mhx1999.top/gtgrwijktm.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.tian-w.cn/gtijmijhqg.html

[Q89] 判断表是否存在
来源：http://hz.c1oappe.top/gtnldarbll.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.jqgufenzy.top/gtbwbflxtv.html

[Q90] 生成序号列
来源：http://hz.ywan-chungtsiang.top/gtfnfhimmy.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.yj202588.top/gtzikvzspw.html

================================================================================
来源：http://hz.guannengcc.top/gtgkjozyoi.html

R. Bash 专题
来源：http://hz.sxryk.cn/gtucyjgihw.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtbdbprzyd.html

[R01] shebang 与严格模式
来源：http://hz.hammf.cn/gttajokusv.html

#!/usr/bin/env bash
来源：http://hz.kuanghao11.cn/gtdcwoajjr.html

set -euo pipefail
来源：http://hz.hammf.cn/gtouehkcin.html

[R02] 变量赋值与使用
来源：http://hz.zhijiandao.cn/gtjfitagrg.html

name="Tom"; echo "$name"
来源：http://hz.bjfxy.top/gtakvynfsp.html

[R03] 只读变量
来源：http://hz.hnxiangtu.top/gtrcmwphpu.html

readonly PI=3.14
来源：http://hz.dianchejie.cn/gtyptomdxe.html

[R04] 位置参数
来源：http://hz.cqqwz.cn/gtrjtktzzj.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.shanyushiyangtech.top/gtmkqtbklu.html

[R05] 参数默认值
来源：http://hz.yuanzhike.top/gtwyozyril.html

name="${1:-default}"
来源：http://hz.ehwqpu.com/gtlkautdhx.html

[R06] 判断命令是否存在
来源：http://hz.shangyingyoupin.top/gtuddauokx.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.hnqzz.top/gtthgsarnx.html

[R07] if 判断文件
来源：http://hz.birdmap.top/gtitxmgajn.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.sufxvd.cn/gtfmeqlikw.html

[R08] 数值比较
来源：http://hz.hongshengwenyu.top/gtsdsjpxme.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.hfpthk.cn/gtdzhbinih.html

[R09] 字符串比较
来源：http://hz.fzhhl.top/gtaishnbft.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.haohaochexian.top/gtqsveziiz.html

[R10] 正则匹配
来源：http://hz.chenlongwang.top/gthhbqlyva.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.jqgufenzy.top/gtahlggztq.html

[R11] case 多分支
来源：http://hz.zhixingplan.top/gtctubprdb.html

case "$1" in
来源：http://hz.meibo888.top/gtjexwjloa.html

start) echo "启动" ;;
来源：http://hz.andypj.xyz/gtoladqkht.html

stop)  echo "停止" ;;
来源：http://hz.cucudq.cn/gtksaozwon.html

*)     echo "未知命令" ;;
来源：http://hz.yvedp.cn/gthrmyhxou.html

esac
来源：http://hz.jianghu66.top/gtujpljpoi.html

[R12] for 遍历文件
来源：http://hz.haohaochexian.top/gtekrjzosx.html

for f in *.txt; do echo "$f"; done
来源：http://hz.316326.xyz/gtgcdxlfcu.html

[R13] for 计数循环
来源：http://hz.xuanzx.com/gttpgijwdt.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.ppjwa.cn/gtupipnwnu.html

[R14] C 风格 for
来源：http://hz.hnqzz.top/gtuhgevuhe.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.cashguo.top/gtcnhowtuz.html

[R15] while 逐行读文件
来源：http://hz.zycfv.cn/gtisoophwk.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.hfpthk.cn/gtqheihcaa.html

[R16] until 等待条件
来源：http://hz.tanke756.top/gtlvmcexhp.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.jyoumei.cn/gtduebaotc.html

[R17] 数组定义与取值
来源：http://hz.fengsongda.top/gtpjfvwmkp.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.yj20258.top/gtggdnrfot.html

[R18] 遍历数组
来源：http://hz.ppjwa.cn/gtmcsiyxcd.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.haohaochexian.top/gtazfbxenv.html

[R19] 数组长度
来源：http://hz.shangyingyoupin.top/gtolnhjard.html

echo "${#arr[@]}"
来源：http://hz.yangfankeji.com/gtfscglmin.html

[R20] 关联数组（字典）
来源：http://hz.zhixingplan.top/gtfxmhvxtr.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.cashguo.top/gtwthorzrn.html

[R21] 字符串长度
来源：http://hz.daxiang520.top/gtczkuepvg.html

echo "${#s}"
来源：http://hz.ybcxt.top/gtlhojnxum.html

[R22] 截取子串
来源：http://hz.iojbl.cn/gtvgeaqglb.html

echo "${s:0:5}"
来源：http://hz.zhengqikj.top/gtlqjiznxu.html

[R23] 字符串替换
来源：http://hz.iojbl.cn/gtdtzgntjr.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.fengsongda.top/gthwxagkti.html

[R24] 大小写转换
来源：http://hz.jqgfzy.top/gtzzhzskhe.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.aibaodan.cn/gtgkazixfj.html

[R25] 去后缀 / 去前缀
来源：http://hz.gotoacloud.top/gturflveuc.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.zhengqikj.top/gtrxdgidjs.html

[R26] 命令替换
来源：http://hz.dianchejie.cn/gtmazjijql.html

now=$(date +%F); echo "$now"
来源：http://hz.xziqi.cn/gtzvfvdrzy.html

[R27] 算术展开
来源：http://hz.fzhhl.top/gtiwhckaju.html


<!-- 参考信息 -->