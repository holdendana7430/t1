代发 wailian999

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.sweek.top/gtyxykzndk.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.yanxiufei.cn/gtwwxethkt.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.haohaochexian.top/gtpqcunfyg.html

Ruby: a == b
来源：http://hz.ywan-chungtsiang.top/gtubzzrbrb.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.hywenlv.cn/gtstvxugfs.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.shanyushiyangkeji.top/gtgjzztjhg.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.zhengqikj.top/gtyyqroxob.html

PHP:  if (empty($x)) {}
来源：http://hz.316326.xyz/gtaarkjonq.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.gotoacloud.top/gtovajijlm.html

TS:   if (x == null) {}
来源：http://hz.zhiwuduotai.top/gtrtfaeuxl.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.tianlin.xyz/gtcghsjaeh.html

Go:   if x == nil {}
来源：http://hz.zhijiandao.cn/gtntidnmfv.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.0kj1m.cn/gthzyquaig.html

C#:   if (x is null) {}
来源：http://hz.ehwqpu.com/gtizjynqex.html

[P07] 防抖与节流
来源：http://hz.daxiang520.top/gtjojlzanw.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.jinqigufen.top/gtpkafzfqx.html

PHP:  // 手写时间戳比较
来源：http://hz.hysaishi.cn/gtfegnpxic.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zycfv.cn/gtvpustkcu.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.52xcode.cn/gtmklvsgob.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.sufxvd.cn/gtealkjvrn.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.gzhubu.top/gtmnsdqpjt.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.nwbrower.top/gtkwozbmpk.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.jianghu66.top/gtuozgvobn.html

[P08] 处理浮点精度问题
来源：http://hz.ybcxt.top/gtzmedotaz.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.nwbrower.top/gtauxpgzyw.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.zhoulong.xyz/gtjyxczikg.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.ybcxt.top/gtxsethezb.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.yuxming.cn/gtohegegmx.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.dianchejie.cn/gtfzjuyykf.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.0kj1m.cn/gtxtzdmkur.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.tian-w.cn/gtldcmtkgl.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.smart0.xyz/gtgkvpgpbh.html

================================================================================
来源：http://hz.ydzc1.top/gtoepapnmm.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.bjfxy.top/gtgsknxbqs.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtgbaqchay.html

[Q01] 创建表
来源：http://hz.ybcxt.top/gtuserforc.html

CREATE TABLE users (
来源：http://hz.zhoulong.xyz/gtgherqsrb.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.xuetiantiany.cn/gtnvryxzld.html

name VARCHAR(50) NOT NULL,
来源：http://hz.zhengqikj.top/gtwgppaffq.html

email VARCHAR(100) UNIQUE,
来源：http://hz.tian-w.cn/gtyrhcrfyh.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.smart0.xyz/gtjfrgsczt.html

);
来源：http://hz.xuetiantiany.cn/gtqdxkudca.html

[Q02] 创建带外键的表
来源：http://hz.xuetiantiany.cn/gterdovefo.html

CREATE TABLE orders (
来源：http://hz.xuetiantiany.cn/gtowynbhaa.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.sysykeji.top/gteeanrkxe.html

user_id INT NOT NULL,
来源：http://hz.sufxvd.cn/gtarrtvqlk.html

amount DECIMAL(10, 2),
来源：http://hz.dashuyun.cn/gtmqkgbtjs.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.jinqigfzy.top/gtkhvjxwss.html

);
来源：http://hz.birdmap.top/gtjrudhzph.html

[Q03] 增加列
来源：http://hz.yuxming.cn/gtkfptxiim.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.aizwys.cn/gtzxirffnj.html

[Q04] 修改列类型
来源：http://hz.zhongyouzk.top/gtwkjwhszu.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.jinghuilouyu.cn/gtidlizicp.html

[Q05] 重命名列
来源：http://hz.tian-w.cn/gtucmknnsr.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.zhengqikj.top/gtdqnfohsf.html

[Q06] 删除列
来源：http://hz.chenzaomai.com/gtiagedwyx.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.ydzc1.top/gtaqakipwc.html

[Q07] 删除表
来源：http://hz.sufxvd.cn/gtdvkhpdmk.html

DROP TABLE IF EXISTS orders;
来源：http://hz.vqdsnc.cn/gtlskhpxot.html

[Q08] 创建普通索引
来源：http://hz.ybcxt.top/gthlzijwzs.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.daria6918.cn/gtutqyzcqh.html

[Q09] 创建唯一索引
来源：http://hz.wangshuangyany.cn/gttlrohzqf.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.wangshuangyany.cn/gtvojnqmfz.html

[Q10] 插入单行
来源：http://hz.wangdashe.top/gtonuthbnq.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.pycfn.com/gtbrqzxyyu.html

[Q11] 一次插入多行
来源：http://hz.jlsjyb.cn/gtsezugcbm.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.pengpengdd.cyou/gtvkgdsxjp.html

[Q12] 插入后取自增 ID
来源：http://hz.meibo888.top/gtjihabbet.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.gzhubu.top/gthlmowggi.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.yanxiufei.cn/gthyxnhlds.html

[Q13] 忽略重复插入
来源：http://hz.wangshuangyany.cn/gtsqogfoca.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.xylfe.cn/gtqeieeqep.html

[Q14] 存在则更新（upsert）
来源：http://hz.yuanzhike.top/gtnxdwtwdw.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.jlsjyb.cn/gtusmdqpfi.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.jinqigfzy.top/gtszbotzvl.html

[Q15] 查询全部
来源：http://hz.yangfankeji.com/gtrglyxryo.html

SELECT * FROM users;
来源：http://hz.xziqi.cn/gtnjxiubbk.html

[Q16] 查询指定列
来源：http://hz.wangshuangyany.cn/gtfbhaugrb.html

SELECT id, name FROM users;
来源：http://hz.redwolf501.top/gtmrjvsocg.html

[Q17] 条件查询
来源：http://hz.ybcxt.top/gtgesotuqp.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.smart0.xyz/gtwzmnchsg.html

[Q18] 模糊匹配
来源：http://hz.yj20258.top/gtwpndhuax.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.dashuyun.cn/gteqfhaouy.html

[Q19] 范围查询
来源：http://hz.gzhubu.top/gtxzgxkxme.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.jqgufenzy.top/gtsivlecnz.html

[Q20] IN 列表
来源：http://hz.9152youxi.cn/gtodimmmzo.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.smart0.xyz/gtsnsqxlmk.html

[Q21] 空值判断
来源：http://hz.hnqzz.top/gtkjcuamsz.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.tian-w.cn/gtgiarnokb.html

[Q22] 排序
来源：http://hz.svipenyu.cn/gtdfyszgeb.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.zhaomingkeji.xyz/gtykesiowq.html

[Q23] 分页
来源：http://hz.chenlongwang.top/gtvimygayd.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.dashuyun.cn/gtedtzrdzs.html

[Q24] 去重
来源：http://hz.jinyuanbaomall.cn/gteoizqqke.html

SELECT DISTINCT city FROM users;
来源：http://hz.yuxming.cn/gtoyjpqbtc.html

[Q25] 只取前 N 条
来源：http://hz.zhengqikj.top/gtgojptwtx.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.yueranfly.top/gtvwyyicop.html

[Q26] 计数
来源：http://hz.gaohongyu789.top/gtiumowfhs.html

SELECT COUNT(*) FROM users;
来源：http://hz.xziqi.cn/gtywlaqtmx.html

[Q27] 条件计数
来源：http://hz.chenlongwang.top/gtukqijzdn.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.yuxming.cn/gtmkqnjpvx.html

[Q28] 求和与平均
来源：http://hz.chenjidiqi.icu/gtbbfgnlom.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.zhoulong.xyz/gtpsrgkwfl.html

[Q29] 最大最小值
来源：http://hz.meibo888.top/gtolayhvje.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.shanyushiyangkeji.top/gtdlbuvoru.html

[Q30] 分组统计
来源：http://hz.zhixingplan.top/gtqsdnxmas.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.9152youxi.cn/gthdvkobfj.html

[Q31] 分组后过滤
来源：http://hz.birdmap.top/gtfhgugkdt.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.nwbrower.top/gtyqnavokt.html

[Q32] 分组拼接字符串
来源：http://hz.daxiang520.top/gtvnltiqgc.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.sxryk.cn/gtzhlguxfo.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.cdnleiting.top/gtqqrgxrjh.html

[Q33] 多列分组
来源：http://hz.mhx1999.top/gtrkralhas.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.kuanghao11.cn/gtmzoxtbtu.html

[Q34] 每组取第一条
来源：http://hz.bjfxy.top/gtlhwashrg.html

SELECT * FROM (
来源：http://hz.hnqzz.top/gtpohdaeln.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.yonumen.top/gtifuyvbmd.html

) t WHERE rn = 1;
来源：http://hz.yanxiufei.cn/gtjreocwip.html

[Q35] 内连接
来源：http://hz.0kj1m.cn/gtzjgvpdrf.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.sufxvd.cn/gtdikjyhlc.html

[Q36] 左连接
来源：http://hz.ywan-chungtsiang.top/gtzjbsiwyv.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.fzhhl.top/gtoeqbktci.html

[Q37] 右连接
来源：http://hz.hysaishi.cn/gtvuzmozbv.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.wangdashe.top/gtzpvptacy.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.vqdsnc.cn/gtbmbrwvgf.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.316326.xyz/gtnujmzwtf.html

[Q39] 自连接（查上下级）
来源：http://hz.jianghu66.top/gtvavhqpbs.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.shanyushiyangtech.top/gtebqkihtt.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.daxiang520.top/gtkoseztej.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.wangdashe.top/gtelyahxjr.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.meibo888.top/gtzojjfjvt.html

[Q41] 多表连接
来源：http://hz.feifeiyinyue.top/gtqoqrmpgd.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.ehwqpu.com/gtafbklfgx.html

JOIN users u ON u.id = o.user_id
来源：http://hz.xinyue.icu/gtmsitrmvs.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.aibaodan.cn/gtbziydmmu.html

[Q42] 连接条件附加过滤
来源：http://hz.jinqigufen.top/gtoqnmfxwv.html

SELECT u.name, o.amount FROM users u
来源：http://hz.tanke756.top/gtdmkfpvhq.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.hongshengwenyu.top/gtaceofhgl.html

[Q43] 标量子查询
来源：http://hz.jyoumei.cn/gtsfqabbmn.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.sysykeji.top/gtetrbeblp.html

[Q44] IN 子查询
来源：http://hz.haohaochexian.top/gtyvuvmkbx.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.wangdashe.top/gtvyefidgd.html

[Q45] EXISTS 判断存在
来源：http://hz.jinghuilouyu.cn/gtrqcvslzl.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.havefunace.top/gtakhqpdxu.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.chenlongwang.top/gthqxegbwt.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yongpay.top/gtonhtxpap.html

[Q47] 与平均值比较
来源：http://hz.snrcjt.cn/gtvltqlecs.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.c1oappe.top/gteefdbrau.html

[Q48] CTE 公用表表达式
来源：http://hz.gzhubu.top/gttcvqwzms.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.gotoacloud.top/gtyqbxxzmk.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.zhijiandao.cn/gtwevwncpj.html

[Q49] 更新单行
来源：http://hz.xziqi.cn/gtktoltzbq.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.yvedp.cn/gtgkwnpfjl.html

[Q50] 批量更新
来源：http://hz.yangfankeji.com/gtpyehovlh.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.xuetiantiany.cn/gtayfobpoy.html

[Q51] 用子查询更新
来源：http://hz.gogol.net.cn/gtbxfqvjfu.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.jinqigufen.top/gtcssiahji.html

[Q52] 删除指定行
来源：http://hz.redwolf501.top/gtmktzklfu.html

DELETE FROM users WHERE id = 10;
来源：http://hz.jianghu66.top/gtyajbwlup.html

[Q53] 按条件删除
来源：http://hz.chenlongwang.top/gtrhvdryem.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.c1oappe.top/gtokqbwhgf.html

[Q54] 清空表
来源：http://hz.meibo888.top/gtgxudrhtl.html

TRUNCATE TABLE logs;
来源：http://hz.yongpay.top/gthoponkqr.html

[Q55] 排名（并列占位）
来源：http://hz.andypj.xyz/gtlwhxjbas.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.c1oappe.top/gtkabusyzc.html

[Q56] 密集排名（并列不占位）
来源：http://hz.zhaomingkeji.xyz/gtfiyowupg.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.52xcode.cn/gtmbjdkwlh.html

[Q57] 行号
来源：http://hz.gzhubu.top/gtztxjunko.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.wangdashe.top/gtplzfvuul.html

[Q58] 累计求和
来源：http://hz.havefunace.top/gthtwwymld.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.ivvv.top/gtutjthbnp.html

[Q59] 分组内累计
来源：http://hz.shuidangran.top/gtwfapinct.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.quarkkingdee.top/gthwuxnghx.html

[Q60] 取上一行 / 下一行
来源：http://hz.aibaodan.cn/gtexmidjjj.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.meibo888.top/gteimlyvqp.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.jinyuanbaomall.cn/gtxqgrtsca.html

[Q61] 移动平均
来源：http://hz.daria6918.cn/gtuabsngaj.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.yongpay.top/gtabevspzw.html

[Q62] 分组占比
来源：http://hz.zhengqikj.top/gtlrlcvioh.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.feifeiyinyue.top/gtqtjpluvg.html

[Q63] 开启事务
来源：http://hz.ydjk.org.cn/gtcjoafkbf.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.tianlin.xyz/gtfgxazjlu.html

[Q64] 提交事务
来源：http://hz.tian-w.cn/gteoidoytg.html

COMMIT;
来源：http://hz.nanxinkj.top/gtblxqruju.html

[Q65] 回滚事务
来源：http://hz.xingfuxueyuan.xyz/gtewbtiexh.html

ROLLBACK;
来源：http://hz.0kj1m.cn/gttnlazvsx.html

[Q66] 行锁查询
来源：http://hz.xinyue.icu/gtbccalsql.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.sxryk.cn/gtvpxkmqft.html

[Q67] 设置隔离级别
来源：http://hz.bjfxy.top/gthzpdmuwy.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.ybcxt.top/gtkxzxkgcc.html

[Q68] 保存点
来源：http://hz.redwolf501.top/gtzukstnwt.html

SAVEPOINT sp1;
来源：http://hz.hywenlv.cn/gtruxuyuaa.html

ROLLBACK TO sp1;
来源：http://hz.jinqigufen.top/gtqysoabzs.html

[Q69] 查看执行计划
来源：http://hz.cdnleiting.top/gtjgxvumas.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.yvedp.cn/gtcciufscm.html

[Q70] 更新统计信息
来源：http://hz.yueranfly.top/gtcqngtspn.html

ANALYZE TABLE users;
来源：http://hz.zhaomingkeji.xyz/gtkwsbozsg.html

[Q71] 查看建表语句
来源：http://hz.wangshuangyany.cn/gtejgiavbo.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.iojbl.cn/gtcjgqrckr.html

[Q72] 查看索引
来源：http://hz.xingfuxueyuan.xyz/gtbgzqzint.html

SHOW INDEX FROM users;
来源：http://hz.sxryk.cn/gtepvgmoaj.html

[Q73] 查看表状态
来源：http://hz.snrcjt.cn/gtjctfhzsw.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.jinqigfzy.top/gtvvstxqxn.html

[Q74] 强制使用索引
来源：http://hz.yongpay.top/gtvjqgqyzt.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.zycfv.cn/gtekcbdckq.html

[Q75] 日期格式化
来源：http://hz.pengpengdd.cyou/gtxxypyict.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.andypj.xyz/gtwxuocfnh.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.jlsjyb.cn/gtmisiaoba.html

[Q76] 按天统计
来源：http://hz.ydzc1.top/gtfogdemlx.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.hfpthk.cn/gtlnvirekb.html

[Q77] 时间加减
来源：http://hz.sxryk.cn/gtgjelnuww.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.cashguo.top/gtreceqhwq.html

[Q78] 当前时间
来源：http://hz.nwbrower.top/gtsrhktnyn.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.gzhubu.top/gtwxbensvf.html

[Q79] 字符串拼接
来源：http://hz.pycfn.com/gtrkzwrtso.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.yuxming.cn/gterakoolq.html

[Q80] 字符串截取
来源：http://hz.aibaodan.cn/gtfytsawie.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.chenzaomai.com/gtmusglmnj.html

[Q81] 字符串替换
来源：http://hz.zhengqikj.top/gtgrezzllr.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.cheryme.top/gtwlrnkxwk.html

[Q82] 字符长度与字节长度
来源：http://hz.52xcode.cn/gtkbysprdt.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.hysaishi.cn/gtnbmubskg.html

[Q83] 大小写转换
来源：http://hz.hammf.cn/gtdpxzoyth.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.bjfxy.top/gtzhtbjzjv.html

[Q84] 去除首尾空格
来源：http://hz.yongpay.top/gtcklltmsg.html

SELECT TRIM(name) FROM users;
来源：http://hz.jqgfzy.top/gtdkuhamiu.html

[Q85] 数值取整
来源：http://hz.guowangkeji.top/gtitutwzyb.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.wangdashe.top/gtgxqleiof.html

[Q86] 读取 JSON 字段
来源：http://hz.cqqwz.cn/gtqwwzpjmj.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.cucudq.cn/gtyqrwqivz.html

[Q87] JSON 字段做条件
来源：http://hz.yj20258.top/gtrpdqcyzs.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.xinyue.icu/gtzkmrsvkr.html

[Q88] 行转列（条件聚合）
来源：http://hz.yangfankeji.com/gtwtvvhdnh.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.jinghuilouyu.cn/gtudhtvagw.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.fzhhl.top/gtmmpsljxm.html

[Q89] 判断表是否存在
来源：http://hz.jiagoushi.top/gteyhgazkl.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.tianlin.xyz/gtewwwucde.html

[Q90] 生成序号列
来源：http://hz.tanke756.top/gttlzdctzz.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.daxiang520.top/gtdpwheyca.html

================================================================================
来源：http://hz.ppjwa.cn/gtlgxytbjd.html

R. Bash 专题
来源：http://hz.wangdashe.top/gtqrgoecss.html

================================================================================
来源：http://hz.ybcxt.top/gtuszyzsye.html

[R01] shebang 与严格模式
来源：http://hz.zhiwuduotai.top/gtasksodqy.html

#!/usr/bin/env bash
来源：http://hz.bjfxy.top/gtfytfuxtm.html

set -euo pipefail
来源：http://hz.yj20258.top/gtdxldnmrf.html

[R02] 变量赋值与使用
来源：http://hz.gzhubu.top/gtktyepvul.html

name="Tom"; echo "$name"
来源：http://hz.zhoulong.xyz/gtikchbvgm.html

[R03] 只读变量
来源：http://hz.jinyuanbaomall.cn/gtbjjadacn.html

readonly PI=3.14
来源：http://hz.zhaomingkeji.xyz/gtsoxdlppx.html

[R04] 位置参数
来源：http://hz.zhijiandao.cn/gtgquvqbij.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.cashguo.top/gtyxnpkpef.html

[R05] 参数默认值
来源：http://hz.wangshuangyany.cn/gtqyweuyhz.html

name="${1:-default}"
来源：http://hz.svipenyu.cn/gtoxxhtjrn.html

[R06] 判断命令是否存在
来源：http://hz.havefunace.top/gtykxsrhpc.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.kuanghao11.cn/gtskwbmmmh.html

[R07] if 判断文件
来源：http://hz.gogol.net.cn/gtzrzbmbkm.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.guannengcc.top/gttybjlofd.html

[R08] 数值比较
来源：http://hz.cashguo.top/gtxymzgftf.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.ydjk.org.cn/gtfaermtkl.html

[R09] 字符串比较
来源：http://hz.feifeiyinyue.top/gtobxiusmn.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.cucudq.cn/gtnecqdeku.html

[R10] 正则匹配
来源：http://hz.zhixingplan.top/gtyuoyhiiw.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.sweek.top/gtzwjejsma.html

[R11] case 多分支
来源：http://hz.pengpengdd.cyou/gtvrelpkkw.html

case "$1" in
来源：http://hz.meibo888.top/gtnynewrou.html

start) echo "启动" ;;
来源：http://hz.xuanzx.com/gttjnfgirz.html

stop)  echo "停止" ;;
来源：http://hz.yangfankeji.com/gtvidjzmyu.html

*)     echo "未知命令" ;;
来源：http://hz.shangyingyoupin.top/gtbktrallh.html

esac
来源：http://hz.ehwqpu.com/gtxcvbofze.html

[R12] for 遍历文件
来源：http://hz.ehwqpu.com/gtumhisjdv.html

for f in *.txt; do echo "$f"; done
来源：http://hz.nanxuanxn.top/gtntleyhhc.html

[R13] for 计数循环
来源：http://hz.hfpthk.cn/gtqltwmpat.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.dashuyun.cn/gtfcwdawpn.html

[R14] C 风格 for
来源：http://hz.yj20258888.top/gtvkcjxhix.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.hywenlv.cn/gtgdibkeyh.html

[R15] while 逐行读文件
来源：http://hz.jyoumei.cn/gtiqyvixhs.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.ehwqpu.com/gtqdhxulky.html

[R16] until 等待条件
来源：http://hz.fzhhl.top/gtyyoarkpn.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.jiagoushi.top/gtmkjftnlh.html

[R17] 数组定义与取值
来源：http://hz.jyoumei.cn/gtnewtvowt.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.zhaomingkeji.xyz/gttztdjpbd.html

[R18] 遍历数组
来源：http://hz.jinqigfzy.top/gthbkxzaik.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.zhongyouzk.top/gtxdsdjsrk.html

[R19] 数组长度
来源：http://hz.tanke756.top/gtewdqxlzo.html

echo "${#arr[@]}"
来源：http://hz.chenzaomai.com/gthatpdmes.html

[R20] 关联数组（字典）
来源：http://hz.jinqigfzy.top/gtjeidhqkv.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.hfpthk.cn/gtkvtvpsgk.html

[R21] 字符串长度
来源：http://hz.ppjwa.cn/gtabvozosx.html

echo "${#s}"
来源：http://hz.cheryme.top/gtihyefmxr.html

[R22] 截取子串
来源：http://hz.nwbrower.top/gtxxrjsupr.html

echo "${s:0:5}"
来源：http://hz.zhengqikj.top/gtsizigtjj.html

[R23] 字符串替换
来源：http://hz.jinyuanbaomall.cn/gtwlyjioyc.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.jinqigfzy.top/gtdlhzfaki.html

[R24] 大小写转换
来源：http://hz.sufxvd.cn/gtlaoygxyv.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.hywenlv.cn/gtyqnjlzgq.html

[R25] 去后缀 / 去前缀
来源：http://hz.hysaishi.cn/gtslsxkcfb.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.yangfankeji.com/gtzdejscqg.html

[R26] 命令替换
来源：http://hz.hysaishi.cn/gtafvmsebe.html

now=$(date +%F); echo "$now"
来源：http://hz.tanke756.top/gtqxdkwguj.html

[R27] 算术展开
来源：http://hz.yj202588.top/gtzfzmhpwv.html


<!-- 参考信息 -->