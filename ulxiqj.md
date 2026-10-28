代发 wailian999

Java: list.size();  map.size();  s.length()
来源：http://hz.ppjwa.cn/gtrymfgfbu.html

Go:   len(arr);  len(m)
来源：http://hz.snrcjt.cn/gtapgulilo.html

Ruby: x.length;  x.size
来源：http://hz.guannengcc.top/gtyxwxvags.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.wangdashe.top/gtvrvaygwu.html

[P05] 判断两个对象内容是否相等
来源：http://hz.haohaochexian.top/gtrbnyeeby.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.xuanzx.com/gtbqmoxajj.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.c1oappe.top/gtcootabdm.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.xingfuxueyuan.xyz/gtsqcyzrvf.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.ehwqpu.com/gtlcakcdmr.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.svipenyu.cn/gtiiemwmrs.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.yvedp.cn/gtxngjfoyc.html

Ruby: a == b
来源：http://hz.xingfuxueyuan.xyz/gtngtmzbcu.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.ppjwa.cn/gtmvgmcpmw.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.jiagoushi.top/gtqiqrydjb.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.quarkkingdee.top/gtabpbhlgm.html

PHP:  if (empty($x)) {}
来源：http://hz.zdqjudy.top/gtrjsikvgt.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.pengpengdd.cyou/gtccumogjr.html

TS:   if (x == null) {}
来源：http://hz.sweek.top/gthlmpvmrz.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.shuidangran.top/gtmsahawii.html

Go:   if x == nil {}
来源：http://hz.svipenyu.cn/gtgwfqgvga.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.daria6918.cn/gtvwlglcbv.html

C#:   if (x is null) {}
来源：http://hz.xuetiantiany.cn/gtorispkml.html

[P07] 防抖与节流
来源：http://hz.daxiang520.top/gthjzumxkq.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.xuetiantiany.cn/gtqcrcbcyo.html

PHP:  // 手写时间戳比较
来源：http://hz.feifeiyinyue.top/gttdgmndgr.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.bjfxy.top/gtahoemxmf.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yuxming.cn/gtrtrcckvj.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.guannengcc.top/gtycdkhwuw.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.dianchejie.cn/gtubklnlaz.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.shuidangran.top/gtyloqsije.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.zhongyouzk.top/gtmtrvgfwc.html

[P08] 处理浮点精度问题
来源：http://hz.sxryk.cn/gtkowrmgsb.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.jinqigfzy.top/gtrmsrctyj.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.hongshengwenyu.top/gtdbxelffg.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.zhixingplan.top/gtaagsucnc.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.jqgfzy.top/gtacixydeb.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.tian-w.cn/gtqoxqmwut.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.sufxvd.cn/gtsywabazy.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.tianlin.xyz/gtblbnylpc.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.nanxuanxn.top/gtidgwngqw.html

================================================================================
来源：http://hz.aizwys.cn/gttyhregbq.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.sxryk.cn/gtqjmwrcph.html

================================================================================
来源：http://hz.birdmap.top/gtvholreej.html

[Q01] 创建表
来源：http://hz.hammf.cn/gtocmkqfxy.html

CREATE TABLE users (
来源：http://hz.yueranfly.top/gtgcdbcpnn.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.cqqwz.cn/gtkoytexdt.html

name VARCHAR(50) NOT NULL,
来源：http://hz.shanyushiyangtech.top/gtpvtvpryy.html

email VARCHAR(100) UNIQUE,
来源：http://hz.gogol.net.cn/gtzdbqwufq.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.zhijiandao.cn/gtdohcshmg.html

);
来源：http://hz.hnqzz.top/gtdiiqhnvh.html

[Q02] 创建带外键的表
来源：http://hz.nwbrower.top/gtijhguipo.html

CREATE TABLE orders (
来源：http://hz.guannengcc.top/gtsrmaiyrj.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.xziqi.cn/gtkbvfpaff.html

user_id INT NOT NULL,
来源：http://hz.quarkkingdee.top/gtrpppclgj.html

amount DECIMAL(10, 2),
来源：http://hz.shangyingyoupin.top/gtqjxhznbm.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.jinyuanbaomall.cn/gtypqppgow.html

);
来源：http://hz.c1oappe.top/gtmqrbothz.html

[Q03] 增加列
来源：http://hz.jlsjyb.cn/gtahgxfqwy.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.yuanzhike.top/gttcbxdubt.html

[Q04] 修改列类型
来源：http://hz.kuanghao11.cn/gtwqqygngm.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.xuanzx.com/gtlpgavarl.html

[Q05] 重命名列
来源：http://hz.zycfv.cn/gtspzgmgqw.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.guowangkeji.top/gtolvwycaz.html

[Q06] 删除列
来源：http://hz.jiagoushi.top/gtkxgjemdy.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.c1oappe.top/gtxjraxahn.html

[Q07] 删除表
来源：http://hz.jqgfzy.top/gthxxhfulr.html

DROP TABLE IF EXISTS orders;
来源：http://hz.yj20258.top/gtnizkqxcy.html

[Q08] 创建普通索引
来源：http://hz.chenjidiqi.icu/gtvuoqffnv.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.iojbl.cn/gtmuxwoxhi.html

[Q09] 创建唯一索引
来源：http://hz.zdqjudy.top/gtdvgcovjt.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.wangshuangyany.cn/gtgcirbwpa.html

[Q10] 插入单行
来源：http://hz.wangdashe.top/gtvwcwbycg.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.ydjk.org.cn/gtaxtpjyld.html

[Q11] 一次插入多行
来源：http://hz.cashguo.top/gtmfuktief.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.vqdsnc.cn/gtkdhdimtq.html

[Q12] 插入后取自增 ID
来源：http://hz.yvedp.cn/gtsadrwbum.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.daria6918.cn/gtncohlqer.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.smart0.xyz/gtpghstiux.html

[Q13] 忽略重复插入
来源：http://hz.fzhhl.top/gtgvabgssa.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.tian-w.cn/gtydginreq.html

[Q14] 存在则更新（upsert）
来源：http://hz.jinghuilouyu.cn/gtujyklhbn.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.c1oappe.top/gthzgsmsgn.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.cqqwz.cn/gtcyqdlmww.html

[Q15] 查询全部
来源：http://hz.cheryme.top/gtttnkmklk.html

SELECT * FROM users;
来源：http://hz.dashuyun.cn/gtxoeysqhn.html

[Q16] 查询指定列
来源：http://hz.yonumen.top/gteottimhl.html

SELECT id, name FROM users;
来源：http://hz.316326.xyz/gtwnqogdka.html

[Q17] 条件查询
来源：http://hz.nanxinkj.top/gtvinlypcp.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.sweek.top/gtamsjtopr.html

[Q18] 模糊匹配
来源：http://hz.xinyue.icu/gtactwzfhx.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.hywenlv.cn/gtmozkqhgz.html

[Q19] 范围查询
来源：http://hz.kuanghao11.cn/gtzdbdpplg.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.tanke756.top/gtuyvpeqbl.html

[Q20] IN 列表
来源：http://hz.cqqwz.cn/gtsfvsgbha.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.pengpengdd.cyou/gtfrvrazob.html

[Q21] 空值判断
来源：http://hz.gzhubu.top/gtwgrqiond.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.yongpay.top/gtpowsazjv.html

[Q22] 排序
来源：http://hz.ivvv.top/gtabhnbkfm.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.zycfv.cn/gtlfyneqga.html

[Q23] 分页
来源：http://hz.ivvv.top/gtkippvuzd.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.c1oappe.top/gteylolaij.html

[Q24] 去重
来源：http://hz.c1oappe.top/gtjrlkbgkd.html

SELECT DISTINCT city FROM users;
来源：http://hz.ppjwa.cn/gtaeaxxawi.html

[Q25] 只取前 N 条
来源：http://hz.chenzaomai.com/gtbbroshts.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.fzhhl.top/gtiiqpadmu.html

[Q26] 计数
来源：http://hz.jqgufenzy.top/gtbhwlnqsq.html

SELECT COUNT(*) FROM users;
来源：http://hz.tianlin.xyz/gtovvoyexd.html

[Q27] 条件计数
来源：http://hz.ywan-chungtsiang.top/gtwbvqnlyd.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.316326.xyz/gtguteqabp.html

[Q28] 求和与平均
来源：http://hz.nanxuanxn.top/gtvtcvffbq.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.quarkkingdee.top/gtqecaibsw.html

[Q29] 最大最小值
来源：http://hz.tanke756.top/gtammmjoif.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.nanxinkj.top/gtblqbzgij.html

[Q30] 分组统计
来源：http://hz.xinyue.icu/gtcqgsbhen.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.yonumen.top/gtrsuviwhp.html

[Q31] 分组后过滤
来源：http://hz.tian-w.cn/gtigeqheuu.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.0kj1m.cn/gtjnuenfaw.html

[Q32] 分组拼接字符串
来源：http://hz.ppjwa.cn/gtduoiemju.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.nanxuanxn.top/gtrdjvahco.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.gaohongyu789.top/gtkaejoanl.html

[Q33] 多列分组
来源：http://hz.yj202588.top/gtwohondrv.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.jinghuilouyu.cn/gtknnwerbb.html

[Q34] 每组取第一条
来源：http://hz.shanyushiyangkeji.top/gtnjinxwja.html

SELECT * FROM (
来源：http://hz.mhx1999.top/gtxovmlxor.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.ppjwa.cn/gtltphomjk.html

) t WHERE rn = 1;
来源：http://hz.sysykeji.top/gthvnhzimr.html

[Q35] 内连接
来源：http://hz.daxiang520.top/gtshwrylqf.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.jlsjyb.cn/gtykucdfhx.html

[Q36] 左连接
来源：http://hz.shanyushiyangtech.top/gtbekapptv.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.hongshengwenyu.top/gthcgrdlka.html

[Q37] 右连接
来源：http://hz.gogol.net.cn/gtcljweiso.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.jqgfzy.top/gtuuefzbvc.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.andypj.xyz/gtatjhasyf.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.jinghuilouyu.cn/gtlmquqmzo.html

[Q39] 自连接（查上下级）
来源：http://hz.quarkkingdee.top/gtyusumqlh.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.gzhubu.top/gtvjrbngtr.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.ivvv.top/gtijcnfokv.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.ybcxt.top/gttoiacfty.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.ivvv.top/gtlhpasaci.html

[Q41] 多表连接
来源：http://hz.quarkkingdee.top/gtypjfxeoq.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.chenlongwang.top/gtjcoaddge.html

JOIN users u ON u.id = o.user_id
来源：http://hz.xuetiantiany.cn/gtxviumhea.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.redwolf501.top/gtljidzwgg.html

[Q42] 连接条件附加过滤
来源：http://hz.jlsjyb.cn/gtknqqqzqf.html

SELECT u.name, o.amount FROM users u
来源：http://hz.vqdsnc.cn/gtfkyhgrbq.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.c1oappe.top/gtcaotzzyc.html

[Q43] 标量子查询
来源：http://hz.ehwqpu.com/gtcvclxukm.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.guannengcc.top/gtwwqvjswd.html

[Q44] IN 子查询
来源：http://hz.yonumen.top/gtacdkfaxs.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.wangshuangyany.cn/gthxbyogpk.html

[Q45] EXISTS 判断存在
来源：http://hz.ydzc1.top/gtumxwozfd.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.bjfxy.top/gtqqhawhbv.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.sufxvd.cn/gtjwmlzivf.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.dashuyun.cn/gtqaurfcdo.html

[Q47] 与平均值比较
来源：http://hz.yj20258.top/gtijikmfkl.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.daria6918.cn/gtbvnbatbt.html

[Q48] CTE 公用表表达式
来源：http://hz.52xcode.cn/gtcqydguxz.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.bjfxy.top/gtnvkvlhvl.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.zdqjudy.top/gtlrdgrnep.html

[Q49] 更新单行
来源：http://hz.jqgufenzy.top/gtalfzunif.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.hongshengwenyu.top/gttgumlgqp.html

[Q50] 批量更新
来源：http://hz.yueranfly.top/gtktasjeic.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.zycfv.cn/gtedsyrblk.html

[Q51] 用子查询更新
来源：http://hz.havefunace.top/gtlauipjic.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.zdqjudy.top/gttmkqjjfg.html

[Q52] 删除指定行
来源：http://hz.sweek.top/gtovfbavrc.html

DELETE FROM users WHERE id = 10;
来源：http://hz.guowangkeji.top/gtyssxjqwh.html

[Q53] 按条件删除
来源：http://hz.mhx1999.top/gtbtgragol.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.hnqzz.top/gtflnsgocl.html

[Q54] 清空表
来源：http://hz.fzhhl.top/gtmyerwncx.html

TRUNCATE TABLE logs;
来源：http://hz.zhijiandao.cn/gtikjrsext.html

[Q55] 排名（并列占位）
来源：http://hz.c1oappe.top/gtjoimkyak.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.xinyue.icu/gtxuvtdlxr.html

[Q56] 密集排名（并列不占位）
来源：http://hz.ehwqpu.com/gtpdnrzrpg.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.redwolf501.top/gthylnabvw.html

[Q57] 行号
来源：http://hz.yvedp.cn/gtizuzlvqk.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.nwbrower.top/gtcabgrtbe.html

[Q58] 累计求和
来源：http://hz.havefunace.top/gthwdgsafp.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.c1oappe.top/gtzrxmdtec.html

[Q59] 分组内累计
来源：http://hz.wangshuangyany.cn/gtaahrnebu.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.jinqigfzy.top/gtjeibadcb.html

[Q60] 取上一行 / 下一行
来源：http://hz.feifeiyinyue.top/gteamtacje.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.snrcjt.cn/gthqcdfjiw.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.cucudq.cn/gtboughrxv.html

[Q61] 移动平均
来源：http://hz.yvedp.cn/gtyertuktl.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.wangdashe.top/gtklpuyxaf.html

[Q62] 分组占比
来源：http://hz.cheryme.top/gtnitnymsv.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.svipenyu.cn/gthoirgfzf.html

[Q63] 开启事务
来源：http://hz.zhoulong.xyz/gthttkmcza.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.fengsongda.top/gtekvqvpfd.html

[Q64] 提交事务
来源：http://hz.yanxiufei.cn/gtkhmogkzb.html

COMMIT;
来源：http://hz.0kj1m.cn/gtduypqido.html

[Q65] 回滚事务
来源：http://hz.yj20258.top/gtkhmhmmrf.html

ROLLBACK;
来源：http://hz.shuidangran.top/gtkbzxldyd.html

[Q66] 行锁查询
来源：http://hz.hfpthk.cn/gtatjpqjbo.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.zhongyouzk.top/gtmzmstqkh.html

[Q67] 设置隔离级别
来源：http://hz.zhiwuduotai.top/gtdsqgqjck.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.zhixingplan.top/gtyvokghpt.html

[Q68] 保存点
来源：http://hz.cashguo.top/gtybmlnamz.html

SAVEPOINT sp1;
来源：http://hz.zhongyouzk.top/gtetdjnwee.html

ROLLBACK TO sp1;
来源：http://hz.jqgufenzy.top/gtaiukntwq.html

[Q69] 查看执行计划
来源：http://hz.yangfankeji.com/gtdwhuthmj.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.52xcode.cn/gtxaaayymx.html

[Q70] 更新统计信息
来源：http://hz.xziqi.cn/gtphdzixrr.html

ANALYZE TABLE users;
来源：http://hz.snrcjt.cn/gtqjfycnay.html

[Q71] 查看建表语句
来源：http://hz.xuanzx.com/gtvefragkc.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.yonumen.top/gtchgnmkex.html

[Q72] 查看索引
来源：http://hz.yongpay.top/gtytohixhj.html

SHOW INDEX FROM users;
来源：http://hz.hfpthk.cn/gtchifiddx.html

[Q73] 查看表状态
来源：http://hz.pengpengdd.cyou/gtmgbasapw.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.yanxiufei.cn/gttdnuupaz.html

[Q74] 强制使用索引
来源：http://hz.zdqjudy.top/gtxjyoeurj.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.hywenlv.cn/gtrgwcenrq.html

[Q75] 日期格式化
来源：http://hz.chenzaomai.com/gtrtnbutsz.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.chenlongwang.top/gthjgtwuet.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.ppjwa.cn/gtobmtesbi.html

[Q76] 按天统计
来源：http://hz.zhoulong.xyz/gtukyfnkev.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.cashguo.top/gtatlqmqag.html

[Q77] 时间加减
来源：http://hz.zhongyouzk.top/gtvzstjrdv.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.yongpay.top/gtetbptuip.html

[Q78] 当前时间
来源：http://hz.jlsjyb.cn/gtkwdtwqzz.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.ivvv.top/gtupmwhjbd.html

[Q79] 字符串拼接
来源：http://hz.sufxvd.cn/gtbgbakrcg.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.fengsongda.top/gtsdytwbns.html

[Q80] 字符串截取
来源：http://hz.cqqwz.cn/gtroshvygj.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.feifeiyinyue.top/gtekwfyqzh.html

[Q81] 字符串替换
来源：http://hz.tanke756.top/gtatktkupd.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.quarkkingdee.top/gtbyvgbikx.html

[Q82] 字符长度与字节长度
来源：http://hz.sweek.top/gtzlbwpnpk.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.jqgufenzy.top/gtygjqfmyz.html

[Q83] 大小写转换
来源：http://hz.ehwqpu.com/gtgsechkjg.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.yangfankeji.com/gtoclqmldm.html

[Q84] 去除首尾空格
来源：http://hz.yanxiufei.cn/gtqnaiswkn.html

SELECT TRIM(name) FROM users;
来源：http://hz.ydjk.org.cn/gtovpbwxek.html

[Q85] 数值取整
来源：http://hz.yueranfly.top/gtrtkbwale.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.snrcjt.cn/gtdmwmspih.html

[Q86] 读取 JSON 字段
来源：http://hz.jinghuilouyu.cn/gtdopgpihy.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.yj20258888.top/gtmladcecm.html

[Q87] JSON 字段做条件
来源：http://hz.xylfe.cn/gtfzupsniq.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.zhijiandao.cn/gtcoobqtak.html

[Q88] 行转列（条件聚合）
来源：http://hz.xuanzx.com/gtnoddravn.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.sysykeji.top/gtbwflboqc.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.hnqzz.top/gtcfgeileo.html

[Q89] 判断表是否存在
来源：http://hz.nanxuanxn.top/gtvwsswqgu.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.jinqigfzy.top/gtaancscag.html

[Q90] 生成序号列
来源：http://hz.ivvv.top/gtxbnjizby.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.snrcjt.cn/gtidynfehe.html

================================================================================
来源：http://hz.feifeiyinyue.top/gthcpmyaqb.html

R. Bash 专题
来源：http://hz.gaohongyu789.top/gttuaqnxyk.html

================================================================================
来源：http://hz.hnxiangtu.top/gtkiwppdkx.html

[R01] shebang 与严格模式
来源：http://hz.xuetiantiany.cn/gtmiurlvwb.html

#!/usr/bin/env bash
来源：http://hz.birdmap.top/gteaotzino.html

set -euo pipefail
来源：http://hz.bjfxy.top/gtjgtmzjre.html

[R02] 变量赋值与使用
来源：http://hz.hnqzz.top/gthqfyfefh.html

name="Tom"; echo "$name"
来源：http://hz.tian-w.cn/gtheshdrsm.html

[R03] 只读变量
来源：http://hz.ywan-chungtsiang.top/gtogfcswpi.html

readonly PI=3.14
来源：http://hz.kuanghao11.cn/gtfcoowzaf.html

[R04] 位置参数
来源：http://hz.ydzc1.top/gtnswodgjd.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.zycfv.cn/gthfgjmgvk.html

[R05] 参数默认值
来源：http://hz.meibo888.top/gtxalsgfiw.html

name="${1:-default}"
来源：http://hz.andypj.xyz/gtdpkhtqjh.html

[R06] 判断命令是否存在
来源：http://hz.yuanzhike.top/gtsgizdajc.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.cheryme.top/gtmnrfnvar.html

[R07] if 判断文件
来源：http://hz.sysykeji.top/gtglreoukj.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.hfpthk.cn/gtnjsuywkd.html

[R08] 数值比较
来源：http://hz.yuanzhike.top/gttcwhjltj.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.wangdashe.top/gtnsyfvooe.html

[R09] 字符串比较
来源：http://hz.dashuyun.cn/gtdkkqpzkl.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.sufxvd.cn/gtehiwqlrn.html

[R10] 正则匹配
来源：http://hz.yuanzhike.top/gtaxyqdhcw.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.nanxinkj.top/gtkovskhqd.html

[R11] case 多分支
来源：http://hz.jinqigfzy.top/gtsairbjdt.html

case "$1" in
来源：http://hz.jiagoushi.top/gtnbpjbqhv.html

start) echo "启动" ;;
来源：http://hz.shanyushiyangkeji.top/gtjcicqksr.html

stop)  echo "停止" ;;
来源：http://hz.tanke756.top/gtmpcejapz.html

*)     echo "未知命令" ;;
来源：http://hz.jqgufenzy.top/gtsjdbanqj.html

esac
来源：http://hz.52xcode.cn/gtaqsimtrb.html

[R12] for 遍历文件
来源：http://hz.yj202588.top/gtddejuzza.html

for f in *.txt; do echo "$f"; done
来源：http://hz.chenjidiqi.icu/gtmwqdnloo.html

[R13] for 计数循环
来源：http://hz.ppjwa.cn/gtgoqdhfpl.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.wangshuangyany.cn/gtycyhbemv.html

[R14] C 风格 for
来源：http://hz.aizwys.cn/gtxwtoroog.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.jianghu66.top/gtdukkkolt.html

[R15] while 逐行读文件
来源：http://hz.quarkkingdee.top/gtvmkixxmk.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.daria6918.cn/gtbuofxang.html

[R16] until 等待条件
来源：http://hz.ehwqpu.com/gtstshetxi.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.0kj1m.cn/gtymrdiwfl.html

[R17] 数组定义与取值
来源：http://hz.jinqigufen.top/gtrwhfajqr.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.guannengcc.top/gtfmzwynwf.html

[R18] 遍历数组
来源：http://hz.dianchejie.cn/gtysqcgwps.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.meibo888.top/gtxewxmrwj.html

[R19] 数组长度
来源：http://hz.dashuyun.cn/gtndamtbck.html

echo "${#arr[@]}"
来源：http://hz.dianchejie.cn/gtmqmttolk.html

[R20] 关联数组（字典）
来源：http://hz.wangdashe.top/gtfwwvhkwj.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.cashguo.top/gtmqlhqysa.html

[R21] 字符串长度
来源：http://hz.yj20258.top/gtemsdezuo.html

echo "${#s}"
来源：http://hz.havefunace.top/gtwscbzbvg.html

[R22] 截取子串
来源：http://hz.sysykeji.top/gtdgwmxhyw.html

echo "${s:0:5}"
来源：http://hz.nanxuanxn.top/gtxrbuwkmq.html

[R23] 字符串替换
来源：http://hz.gotoacloud.top/gteqspxgdm.html


<!-- 参考信息 -->