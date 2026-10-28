代发 wailian999

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.yangfankeji.com/gtnxqraqji.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.aizwys.cn/gtxsxdfrum.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.daria6918.cn/gtsyyyfpdo.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.tanke756.top/gteubywjza.html

Java: list.size();  map.size();  s.length()
来源：http://hz.sweek.top/gtqckkozct.html

Go:   len(arr);  len(m)
来源：http://hz.xylfe.cn/gtqyqrrdrq.html

Ruby: x.length;  x.size
来源：http://hz.xinyue.icu/gtcuktctei.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.yongpay.top/gtygqezmgo.html

[P05] 判断两个对象内容是否相等
来源：http://hz.ppjwa.cn/gtnamxaddk.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.jinyuanbaomall.cn/gtbsgdujuh.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.vqdsnc.cn/gtbqxhbqvt.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.xuanzx.com/gtccqzpvhm.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.jyoumei.cn/gtbnqonyjv.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.xinyue.icu/gtfdxlcavp.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.yueranfly.top/gtmjrwyfog.html

Ruby: a == b
来源：http://hz.ybcxt.top/gthnguruai.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.jqgfzy.top/gtjzpiskjl.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.yongpay.top/gtksaahklb.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.yj20258.top/gtszpgwxfu.html

PHP:  if (empty($x)) {}
来源：http://hz.hongshengwenyu.top/gtvfictbwd.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.jinqigfzy.top/gtmsersdmk.html

TS:   if (x == null) {}
来源：http://hz.xziqi.cn/gtjgabbxip.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.yuxming.cn/gtluoefmbk.html

Go:   if x == nil {}
来源：http://hz.yj20258888.top/gttxsaexet.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.yonumen.top/gtiitjppki.html

C#:   if (x is null) {}
来源：http://hz.aizwys.cn/gtrozguxse.html

[P07] 防抖与节流
来源：http://hz.tianlin.xyz/gtryyngvsw.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.cashguo.top/gtcwgedbvm.html

PHP:  // 手写时间戳比较
来源：http://hz.nwbrower.top/gtljvmbiff.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.mhx1999.top/gthvyhmrwg.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jqgfzy.top/gtqbyifuct.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.shanyushiyangtech.top/gtlmxoegyk.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.jinqigufen.top/gtnxcaotxy.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.pycfn.com/gtnellwmpy.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.xingfuxueyuan.xyz/gtrotyztlu.html

[P08] 处理浮点精度问题
来源：http://hz.guowangkeji.top/gtypmhpunu.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.havefunace.top/gtvjpqimgr.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.zdqjudy.top/gtwhsbeokc.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.hongshengwenyu.top/gtariyandm.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.xuetiantiany.cn/gtypfibpfn.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.tianlin.xyz/gttwxlreug.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.cucudq.cn/gtmiainyyz.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.dashuyun.cn/gtoopesugc.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.haohaochexian.top/gtohphmhst.html

================================================================================
来源：http://hz.xylfe.cn/gttmlqgenm.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.chenzaomai.com/gtepyzbwsv.html

================================================================================
来源：http://hz.jinqigfzy.top/gtlhaxmfbu.html

[Q01] 创建表
来源：http://hz.daria6918.cn/gthalvhfjb.html

CREATE TABLE users (
来源：http://hz.jyoumei.cn/gtzvxgchbv.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jyoumei.cn/gtwcjowjye.html

name VARCHAR(50) NOT NULL,
来源：http://hz.ydzc1.top/gtyvyhiyyk.html

email VARCHAR(100) UNIQUE,
来源：http://hz.jinyuanbaomall.cn/gtkgdgnriw.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.tanke756.top/gtjwtykwal.html

);
来源：http://hz.ydzc1.top/gttfxdoohq.html

[Q02] 创建带外键的表
来源：http://hz.sxryk.cn/gtpgsdflye.html

CREATE TABLE orders (
来源：http://hz.shanyushiyangtech.top/gtherkaikn.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.fengsongda.top/gtqojwmnbc.html

user_id INT NOT NULL,
来源：http://hz.xingfuxueyuan.xyz/gtdqprrkfi.html

amount DECIMAL(10, 2),
来源：http://hz.zhengqikj.top/gtwzgagwuh.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.yuanzhike.top/gtirhenwrc.html

);
来源：http://hz.hfpthk.cn/gtmligevmt.html

[Q03] 增加列
来源：http://hz.cucudq.cn/gtvigibsgv.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.shanyushiyangkeji.top/gteozpyubt.html

[Q04] 修改列类型
来源：http://hz.ydjk.org.cn/gthrwzgezq.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.jinqigufen.top/gticlrboms.html

[Q05] 重命名列
来源：http://hz.cucudq.cn/gtepklgjyi.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.zhixingplan.top/gtykjsyrxg.html

[Q06] 删除列
来源：http://hz.gogol.net.cn/gtzolmcplz.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.xuetiantiany.cn/gtviiifwcu.html

[Q07] 删除表
来源：http://hz.9152youxi.cn/gtxxvwress.html

DROP TABLE IF EXISTS orders;
来源：http://hz.gzhubu.top/gtsauggwer.html

[Q08] 创建普通索引
来源：http://hz.zhoulong.xyz/gtyqcfopla.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.smart0.xyz/gtrfihgsnb.html

[Q09] 创建唯一索引
来源：http://hz.jianghu66.top/gthhdewwhx.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.jqgufenzy.top/gtulqyvbcw.html

[Q10] 插入单行
来源：http://hz.cucudq.cn/gtkobmtpjv.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.yanxiufei.cn/gtgtxbxbno.html

[Q11] 一次插入多行
来源：http://hz.zhaomingkeji.xyz/gtmwjwrems.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.jiagoushi.top/gtczlizwsz.html

[Q12] 插入后取自增 ID
来源：http://hz.zhoulong.xyz/gtactgqmml.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.jinyuanbaomall.cn/gthpcmugmk.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.shzxlz.cn/gtnfkxgqsg.html

[Q13] 忽略重复插入
来源：http://hz.tian-w.cn/gtqkvzobtd.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.ppjwa.cn/gtdedrbbay.html

[Q14] 存在则更新（upsert）
来源：http://hz.yanxiufei.cn/gtglxaowmx.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.gaohongyu789.top/gtejzwfctv.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.chenzaomai.com/gtmnkooadh.html

[Q15] 查询全部
来源：http://hz.zhiwuduotai.top/gtujaompvs.html

SELECT * FROM users;
来源：http://hz.yuanzhike.top/gtpudawmzh.html

[Q16] 查询指定列
来源：http://hz.bjfxy.top/gtizkavphr.html

SELECT id, name FROM users;
来源：http://hz.andypj.xyz/gtwesqnjnn.html

[Q17] 条件查询
来源：http://hz.jinghuilouyu.cn/gtdqzyiidn.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.dashuyun.cn/gtcbzbvyhm.html

[Q18] 模糊匹配
来源：http://hz.ivvv.top/gtwnpdrdsh.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.cheryme.top/gtdmmifsld.html

[Q19] 范围查询
来源：http://hz.ehwqpu.com/gtklnyblce.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.svipenyu.cn/gthjywrkic.html

[Q20] IN 列表
来源：http://hz.0kj1m.cn/gtaqpgtcvi.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.9152youxi.cn/gttogemyte.html

[Q21] 空值判断
来源：http://hz.cqqwz.cn/gttrxmegjx.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.jyoumei.cn/gtpjbrbfat.html

[Q22] 排序
来源：http://hz.xziqi.cn/gtduujxywa.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.shanyushiyangtech.top/gtpdnkseft.html

[Q23] 分页
来源：http://hz.yueranfly.top/gtxppqewok.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.yvedp.cn/gtwetifndd.html

[Q24] 去重
来源：http://hz.xylfe.cn/gtijbovvfb.html

SELECT DISTINCT city FROM users;
来源：http://hz.chenzaomai.com/gtmwuwjfzt.html

[Q25] 只取前 N 条
来源：http://hz.nanxinkj.top/gtbcdhcxco.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.jlsjyb.cn/gtihmfqhfe.html

[Q26] 计数
来源：http://hz.ehwqpu.com/gtzaeckvqq.html

SELECT COUNT(*) FROM users;
来源：http://hz.gotoacloud.top/gtafnhygwy.html

[Q27] 条件计数
来源：http://hz.ydzc1.top/gtzxpfuoil.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.pycfn.com/gtbdjdcdok.html

[Q28] 求和与平均
来源：http://hz.ppjwa.cn/gtxbdmrjwy.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.zhijiandao.cn/gtgdboxllz.html

[Q29] 最大最小值
来源：http://hz.shanyushiyangtech.top/gtmvfsggck.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.dashuyun.cn/gtfalhaqss.html

[Q30] 分组统计
来源：http://hz.ppjwa.cn/gtapuaqlpa.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.vqdsnc.cn/gtfirkogct.html

[Q31] 分组后过滤
来源：http://hz.shzxlz.cn/gtdhtzkkfq.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.cdnleiting.top/gtppfwuqsp.html

[Q32] 分组拼接字符串
来源：http://hz.birdmap.top/gtjznazvpl.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.9152youxi.cn/gtslhppgvm.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.hysaishi.cn/gtxamlrwcp.html

[Q33] 多列分组
来源：http://hz.jinghuilouyu.cn/gtiwsmiynz.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.nanxinkj.top/gtkallmdqb.html

[Q34] 每组取第一条
来源：http://hz.chenlongwang.top/gtckzbatjs.html

SELECT * FROM (
来源：http://hz.jiagoushi.top/gtfudpgnao.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.quarkkingdee.top/gtfnzoyfti.html

) t WHERE rn = 1;
来源：http://hz.ivvv.top/gthkzctswn.html

[Q35] 内连接
来源：http://hz.bjfxy.top/gtehgjecqr.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.kuanghao11.cn/gtlcejhrsh.html

[Q36] 左连接
来源：http://hz.yangfankeji.com/gtlfgclmkw.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.gzhubu.top/gtrryvrclk.html

[Q37] 右连接
来源：http://hz.xuanzx.com/gtxqondzav.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.snrcjt.cn/gtforjrgsh.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.feifeiyinyue.top/gtuqelcyoi.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.daria6918.cn/gtjrmauein.html

[Q39] 自连接（查上下级）
来源：http://hz.hammf.cn/gtwfprbuql.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.nwbrower.top/gtbmrudnac.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.andypj.xyz/gtocztldjg.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.gzhubu.top/gtwylzauhs.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.yangfankeji.com/gtdtehziiv.html

[Q41] 多表连接
来源：http://hz.zhoulong.xyz/gthirmeaqi.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.shzxlz.cn/gtfqmyawid.html

JOIN users u ON u.id = o.user_id
来源：http://hz.cqqwz.cn/gttcfdsqtb.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.zhoulong.xyz/gtxuldbmvz.html

[Q42] 连接条件附加过滤
来源：http://hz.sysykeji.top/gttoibkstg.html

SELECT u.name, o.amount FROM users u
来源：http://hz.yanxiufei.cn/gtghzrbhuw.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.tanke756.top/gtzbcanbjk.html

[Q43] 标量子查询
来源：http://hz.hfpthk.cn/gtqthhjoiy.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.xylfe.cn/gtbfxecxrg.html

[Q44] IN 子查询
来源：http://hz.cashguo.top/gtydioqtqz.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.cucudq.cn/gtgtnfftzo.html

[Q45] EXISTS 判断存在
来源：http://hz.sysykeji.top/gtfkkogpkz.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jqgufenzy.top/gtdhgzgihh.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.shanyushiyangkeji.top/gtbswhxrtl.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yvedp.cn/gtrzhegvtw.html

[Q47] 与平均值比较
来源：http://hz.aizwys.cn/gtknelvegk.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.9152youxi.cn/gtbstrpmhm.html

[Q48] CTE 公用表表达式
来源：http://hz.redwolf501.top/gtrpadgbzx.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.yvedp.cn/gtjmgfyicj.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.pengpengdd.cyou/gtcnwjcuju.html

[Q49] 更新单行
来源：http://hz.jinyuanbaomall.cn/gtgbzrmjmt.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.jinqigufen.top/gtiwueemzq.html

[Q50] 批量更新
来源：http://hz.quarkkingdee.top/gthuxeqxep.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.jinghuilouyu.cn/gtbvhhmghl.html

[Q51] 用子查询更新
来源：http://hz.cheryme.top/gtczqirhxr.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.dashuyun.cn/gtsuxljsoe.html

[Q52] 删除指定行
来源：http://hz.guowangkeji.top/gteotcdnwk.html

DELETE FROM users WHERE id = 10;
来源：http://hz.yj20258888.top/gttcewhskb.html

[Q53] 按条件删除
来源：http://hz.zhoulong.xyz/gtdtceskzw.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.aibaodan.cn/gttiptlcwv.html

[Q54] 清空表
来源：http://hz.hywenlv.cn/gtukslkwet.html

TRUNCATE TABLE logs;
来源：http://hz.zdqjudy.top/gtjwojtnyd.html

[Q55] 排名（并列占位）
来源：http://hz.52xcode.cn/gthszdmbyt.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.hfpthk.cn/gtxghbszet.html

[Q56] 密集排名（并列不占位）
来源：http://hz.yj20258888.top/gtqvtyryzp.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.redwolf501.top/gtphfivfkt.html

[Q57] 行号
来源：http://hz.smart0.xyz/gtpushhpsj.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.xziqi.cn/gtaqgxvdea.html

[Q58] 累计求和
来源：http://hz.ehwqpu.com/gtaqtwoxsi.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.sweek.top/gthmrysvyu.html

[Q59] 分组内累计
来源：http://hz.c1oappe.top/gtnrvnbocw.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.shuidangran.top/gtntpirnlv.html

[Q60] 取上一行 / 下一行
来源：http://hz.yueranfly.top/gtlaaptdar.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.hfpthk.cn/gtkrafauxd.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.hammf.cn/gtwunidtmz.html

[Q61] 移动平均
来源：http://hz.zhongyouzk.top/gtgxdidigb.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.shanyushiyangtech.top/gtdaenhwrf.html

[Q62] 分组占比
来源：http://hz.ybcxt.top/gttppmjdtw.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.nwbrower.top/gtiymyikki.html

[Q63] 开启事务
来源：http://hz.tian-w.cn/gtefkxtgfi.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.ehwqpu.com/gtjzndqkag.html

[Q64] 提交事务
来源：http://hz.yuxming.cn/gtxieggzau.html

COMMIT;
来源：http://hz.cucudq.cn/gtkxmhssap.html

[Q65] 回滚事务
来源：http://hz.zhongyouzk.top/gtghlwqlpy.html

ROLLBACK;
来源：http://hz.svipenyu.cn/gtqikzxoyd.html

[Q66] 行锁查询
来源：http://hz.snrcjt.cn/gtosjfndtv.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.kuanghao11.cn/gtxtxtnyxm.html

[Q67] 设置隔离级别
来源：http://hz.zdqjudy.top/gtikzpcdzu.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.jyoumei.cn/gtphnbaupm.html

[Q68] 保存点
来源：http://hz.haohaochexian.top/gtggkpacdr.html

SAVEPOINT sp1;
来源：http://hz.c1oappe.top/gtsyxxtzuf.html

ROLLBACK TO sp1;
来源：http://hz.smart0.xyz/gtvafgtoki.html

[Q69] 查看执行计划
来源：http://hz.xylfe.cn/gtmqotjcgs.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.tanke756.top/gtlvylrvfb.html

[Q70] 更新统计信息
来源：http://hz.sufxvd.cn/gtudnepjor.html

ANALYZE TABLE users;
来源：http://hz.zhaomingkeji.xyz/gtmfwhnxjj.html

[Q71] 查看建表语句
来源：http://hz.aizwys.cn/gtfvzwvboc.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.fzhhl.top/gtnjgktqra.html

[Q72] 查看索引
来源：http://hz.ywan-chungtsiang.top/gtgrywlilo.html

SHOW INDEX FROM users;
来源：http://hz.nwbrower.top/gtjodtjiqj.html

[Q73] 查看表状态
来源：http://hz.hysaishi.cn/gtnxdricik.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.ehwqpu.com/gtqdfalbkf.html

[Q74] 强制使用索引
来源：http://hz.nanxinkj.top/gtqbaktyzk.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.dianchejie.cn/gtqrxptkxc.html

[Q75] 日期格式化
来源：http://hz.jqgfzy.top/gtkizyfunw.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.aizwys.cn/gtkqnkqluc.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.shanyushiyangkeji.top/gtdorelhff.html

[Q76] 按天统计
来源：http://hz.c1oappe.top/gtcvjdvnrs.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.feifeiyinyue.top/gtuzhyfxtg.html

[Q77] 时间加减
来源：http://hz.yanxiufei.cn/gtnshwrzmz.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.birdmap.top/gtvxhsqrpi.html

[Q78] 当前时间
来源：http://hz.feifeiyinyue.top/gtwtlpaefv.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.guannengcc.top/gthdvavmfl.html

[Q79] 字符串拼接
来源：http://hz.jqgufenzy.top/gtmqxtitvn.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.zhixingplan.top/gtwcafbfen.html

[Q80] 字符串截取
来源：http://hz.ybcxt.top/gtnbdokikw.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.nwbrower.top/gtczdperft.html

[Q81] 字符串替换
来源：http://hz.guannengcc.top/gtqoobeslc.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.chenjidiqi.icu/gtotocaakl.html

[Q82] 字符长度与字节长度
来源：http://hz.cqqwz.cn/gtbdfeucpr.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.dashuyun.cn/gtsvwagyfi.html

[Q83] 大小写转换
来源：http://hz.fzhhl.top/gtnckvzols.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.gotoacloud.top/gtuatipggo.html

[Q84] 去除首尾空格
来源：http://hz.shanyushiyangkeji.top/gtidttgoft.html

SELECT TRIM(name) FROM users;
来源：http://hz.meibo888.top/gtptscvywu.html

[Q85] 数值取整
来源：http://hz.jiagoushi.top/gtqcqnjrbe.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.wangshuangyany.cn/gtlfeaziza.html

[Q86] 读取 JSON 字段
来源：http://hz.dianchejie.cn/gtnxtpaxzs.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.c1oappe.top/gtkgvokfpo.html

[Q87] JSON 字段做条件
来源：http://hz.zhixingplan.top/gtnpnvgkaz.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.yj202588.top/gtleevtpdw.html

[Q88] 行转列（条件聚合）
来源：http://hz.hnqzz.top/gtvobogsse.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.xziqi.cn/gtjqdyopbc.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.cqqwz.cn/gtgwpgiyol.html

[Q89] 判断表是否存在
来源：http://hz.hysaishi.cn/gtvanjchlf.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.gotoacloud.top/gtulndgttu.html

[Q90] 生成序号列
来源：http://hz.sweek.top/gtjwwjtqbz.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.yuxming.cn/gtzsmtcvty.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtqloaubnt.html

R. Bash 专题
来源：http://hz.andypj.xyz/gtbpyaeezb.html

================================================================================
来源：http://hz.yangfankeji.com/gtfpivsxmh.html

[R01] shebang 与严格模式
来源：http://hz.zhengqikj.top/gtdtkocsdw.html

#!/usr/bin/env bash
来源：http://hz.cqqwz.cn/gtbnxrhinx.html

set -euo pipefail
来源：http://hz.havefunace.top/gtcyvzojds.html

[R02] 变量赋值与使用
来源：http://hz.bjfxy.top/gtuqehdmjs.html

name="Tom"; echo "$name"
来源：http://hz.tanke756.top/gtjwffzrfu.html

[R03] 只读变量
来源：http://hz.aizwys.cn/gtbycluumg.html

readonly PI=3.14
来源：http://hz.zdqjudy.top/gtrcjsudfd.html

[R04] 位置参数
来源：http://hz.ehwqpu.com/gtbghycrgl.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.yanxiufei.cn/gtlsymrkqq.html

[R05] 参数默认值
来源：http://hz.svipenyu.cn/gttnljrnhb.html

name="${1:-default}"
来源：http://hz.shanyushiyangkeji.top/gtzmdcvrzx.html

[R06] 判断命令是否存在
来源：http://hz.yueranfly.top/gtpucemcyq.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.zhongyouzk.top/gtdzflehcu.html

[R07] if 判断文件
来源：http://hz.zycfv.cn/gtxyltmump.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.yj202588.top/gtkgasqdko.html

[R08] 数值比较
来源：http://hz.ydjk.org.cn/gtanmtfmvl.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.tianlin.xyz/gtfkbtrnvb.html

[R09] 字符串比较
来源：http://hz.zhijiandao.cn/gtaqqclvhc.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.0kj1m.cn/gtvyhquaqw.html

[R10] 正则匹配
来源：http://hz.xylfe.cn/gtgzwlhrtf.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.jqgufenzy.top/gtbzdtmylb.html

[R11] case 多分支
来源：http://hz.9152youxi.cn/gtduhvejtg.html

case "$1" in
来源：http://hz.yongpay.top/gtpoiszqwy.html

start) echo "启动" ;;
来源：http://hz.hfpthk.cn/gtievrjbmh.html

stop)  echo "停止" ;;
来源：http://hz.sweek.top/gtbqdekfuw.html

*)     echo "未知命令" ;;
来源：http://hz.yj20258.top/gtjcrgucqr.html

esac
来源：http://hz.guannengcc.top/gtmccdrsln.html

[R12] for 遍历文件
来源：http://hz.bjfxy.top/gtumzpqxir.html

for f in *.txt; do echo "$f"; done
来源：http://hz.jinyuanbaomall.cn/gtammbbyoy.html

[R13] for 计数循环
来源：http://hz.jinqigufen.top/gtjfbwzfnz.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.xinyue.icu/gtpziypzsg.html

[R14] C 风格 for
来源：http://hz.andypj.xyz/gtmezyepvp.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.andypj.xyz/gtfnzghakz.html

[R15] while 逐行读文件
来源：http://hz.jinghuilouyu.cn/gtnrikjunx.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.jinqigfzy.top/gtgbvozmax.html

[R16] until 等待条件
来源：http://hz.chenjidiqi.icu/gttgpkayqi.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.sxryk.cn/gtngkojvve.html

[R17] 数组定义与取值
来源：http://hz.tanke756.top/gtjiuvnqga.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.xingfuxueyuan.xyz/gtmlyskluq.html

[R18] 遍历数组
来源：http://hz.kuanghao11.cn/gttmhnlxxf.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.guannengcc.top/gteydrnraw.html

[R19] 数组长度
来源：http://hz.tianlin.xyz/gtslsoxbog.html

echo "${#arr[@]}"
来源：http://hz.jiagoushi.top/gtvuuppidw.html

[R20] 关联数组（字典）
来源：http://hz.tanke756.top/gtdjjbqkze.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.sufxvd.cn/gtfntzmjqj.html

[R21] 字符串长度
来源：http://hz.0kj1m.cn/gtnugepdlo.html


<!-- 参考信息 -->