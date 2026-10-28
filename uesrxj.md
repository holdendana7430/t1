代发 wailian999

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.yangfankeji.com/gtqgiuribe.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jinqigfzy.top/gtepbtvbxn.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.zdqjudy.top/gtnfwjstnh.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.gogol.net.cn/gtskiixmiz.html

Java: list.size();  map.size();  s.length()
来源：http://hz.guowangkeji.top/gtvoqdvcbp.html

Go:   len(arr);  len(m)
来源：http://hz.sxryk.cn/gtyiizlevm.html

Ruby: x.length;  x.size
来源：http://hz.9152youxi.cn/gtjrhhwvhg.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.ivvv.top/gtjhtpglnv.html

[P05] 判断两个对象内容是否相等
来源：http://hz.snrcjt.cn/gttwratgrt.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.xuanzx.com/gtwghfmlki.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.xuanzx.com/gtnybdifpx.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.tanke756.top/gtzbjzoynq.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.quarkkingdee.top/gtwbtphtvj.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.zhaomingkeji.xyz/gtpsupsecc.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.gzhubu.top/gtoctftajq.html

Ruby: a == b
来源：http://hz.zhaomingkeji.xyz/gtmhnaqnud.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.iojbl.cn/gtzyuupycu.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.jyoumei.cn/gtmnfwkulh.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.chenlongwang.top/gtypwmfnsk.html

PHP:  if (empty($x)) {}
来源：http://hz.52xcode.cn/gtjdyqlpii.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.316326.xyz/gtqxxlvzph.html

TS:   if (x == null) {}
来源：http://hz.xinyue.icu/gtikpsfjbw.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.sweek.top/gtjlpmvfek.html

Go:   if x == nil {}
来源：http://hz.pycfn.com/gtijkdaowj.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.ybcxt.top/gtruatsrpl.html

C#:   if (x is null) {}
来源：http://hz.smart0.xyz/gtxxgldniq.html

[P07] 防抖与节流
来源：http://hz.yangfankeji.com/gttnqshbwu.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.ydzc1.top/gtdohgsote.html

PHP:  // 手写时间戳比较
来源：http://hz.gotoacloud.top/gtttvdmgly.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.aizwys.cn/gttqtbupwz.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.redwolf501.top/gtqcechesz.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.tian-w.cn/gtpinjtpyr.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.sufxvd.cn/gtmbtnfstd.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.meibo888.top/gtcqcbgwfs.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.shanyushiyangkeji.top/gteeodunbt.html

[P08] 处理浮点精度问题
来源：http://hz.svipenyu.cn/gtfidddihg.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.yuxming.cn/gteczfwevp.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.cqqwz.cn/gtzhqcflwk.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.hnqzz.top/gtdgtsrdig.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.yj202588.top/gtbodqwrry.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.vqdsnc.cn/gtjshsppba.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.jlsjyb.cn/gtuzetyzcg.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.xuetiantiany.cn/gtobtikdbg.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.shanyushiyangkeji.top/gtrgkdueeq.html

================================================================================
来源：http://hz.ivvv.top/gtubcnkdts.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.chenlongwang.top/gtbzemezwb.html

================================================================================
来源：http://hz.zycfv.cn/gtwhrnaoqd.html

[Q01] 创建表
来源：http://hz.yongpay.top/gtkivathzt.html

CREATE TABLE users (
来源：http://hz.hnxiangtu.top/gtgmlqqxef.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.dianchejie.cn/gtyxbrcznn.html

name VARCHAR(50) NOT NULL,
来源：http://hz.jqgfzy.top/gtxidznphg.html

email VARCHAR(100) UNIQUE,
来源：http://hz.guannengcc.top/gtznsavoha.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.havefunace.top/gtmysnclhc.html

);
来源：http://hz.svipenyu.cn/gtlqnoxtxb.html

[Q02] 创建带外键的表
来源：http://hz.hfpthk.cn/gtnclbfstk.html

CREATE TABLE orders (
来源：http://hz.nwbrower.top/gtdyhowdez.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.tian-w.cn/gtebtnwumz.html

user_id INT NOT NULL,
来源：http://hz.ppjwa.cn/gtjcazmkby.html

amount DECIMAL(10, 2),
来源：http://hz.gogol.net.cn/gtbpfkufvq.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.cucudq.cn/gtfuqxrivd.html

);
来源：http://hz.zhiwuduotai.top/gtflkmtzdq.html

[Q03] 增加列
来源：http://hz.gogol.net.cn/gtrjxkmlnp.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.yongpay.top/gteoodvlwy.html

[Q04] 修改列类型
来源：http://hz.cashguo.top/gtzrkfqhao.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.52xcode.cn/gtfhomxgum.html

[Q05] 重命名列
来源：http://hz.jyoumei.cn/gtnqrrrbth.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.shanyushiyangtech.top/gtxnnzuubf.html

[Q06] 删除列
来源：http://hz.zycfv.cn/gtfsekorvi.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.smart0.xyz/gtgpwhjdck.html

[Q07] 删除表
来源：http://hz.316326.xyz/gtrpzdltpi.html

DROP TABLE IF EXISTS orders;
来源：http://hz.yangfankeji.com/gtmqrvhihw.html

[Q08] 创建普通索引
来源：http://hz.guannengcc.top/gtpngjbpwi.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.iojbl.cn/gtyrvbqifj.html

[Q09] 创建唯一索引
来源：http://hz.hfpthk.cn/gtrmunjmyq.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.chenzaomai.com/gtbutppxpa.html

[Q10] 插入单行
来源：http://hz.zhixingplan.top/gtdgeervhn.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.shuidangran.top/gtglilioho.html

[Q11] 一次插入多行
来源：http://hz.yanxiufei.cn/gttnnbuldy.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.gogol.net.cn/gttuzuqcth.html

[Q12] 插入后取自增 ID
来源：http://hz.yangfankeji.com/gtnyqnjmhc.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.meibo888.top/gtdhhfhfak.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.yueranfly.top/gtwuhqafdo.html

[Q13] 忽略重复插入
来源：http://hz.hnxiangtu.top/gtnhzdgjrx.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.aizwys.cn/gtbqbsgwxx.html

[Q14] 存在则更新（upsert）
来源：http://hz.gaohongyu789.top/gtduxpnxfa.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.zhixingplan.top/gthwsduswz.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.zhixingplan.top/gtkqzxudff.html

[Q15] 查询全部
来源：http://hz.cdnleiting.top/gtsyyazbhn.html

SELECT * FROM users;
来源：http://hz.daxiang520.top/gtlunozudt.html

[Q16] 查询指定列
来源：http://hz.hywenlv.cn/gtimehoyzx.html

SELECT id, name FROM users;
来源：http://hz.cashguo.top/gtzboymarr.html

[Q17] 条件查询
来源：http://hz.chenjidiqi.icu/gtlkrqfubi.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.xinyue.icu/gtgblawehw.html

[Q18] 模糊匹配
来源：http://hz.nanxuanxn.top/gtlclugslc.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.yangfankeji.com/gtwjiwohax.html

[Q19] 范围查询
来源：http://hz.iojbl.cn/gtykxuumnp.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.zhijiandao.cn/gtqssgbika.html

[Q20] IN 列表
来源：http://hz.daxiang520.top/gtqaiqvkoz.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.gzhubu.top/gtrdymaoto.html

[Q21] 空值判断
来源：http://hz.zhongyouzk.top/gtavtpvmrl.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.ivvv.top/gtutvmznit.html

[Q22] 排序
来源：http://hz.xingfuxueyuan.xyz/gtcsphadjw.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.jinqigfzy.top/gtkcegbqgt.html

[Q23] 分页
来源：http://hz.yuanzhike.top/gtdponrylz.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.dashuyun.cn/gtiwdgyyor.html

[Q24] 去重
来源：http://hz.zhaomingkeji.xyz/gtxuubisqk.html

SELECT DISTINCT city FROM users;
来源：http://hz.ybcxt.top/gtvqavhwru.html

[Q25] 只取前 N 条
来源：http://hz.shanyushiyangtech.top/gtigyqkkhy.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.gotoacloud.top/gtodmucuha.html

[Q26] 计数
来源：http://hz.hnqzz.top/gtmynxyzen.html

SELECT COUNT(*) FROM users;
来源：http://hz.ivvv.top/gtezfheqtv.html

[Q27] 条件计数
来源：http://hz.guannengcc.top/gtigslheow.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.jlsjyb.cn/gtselswjcd.html

[Q28] 求和与平均
来源：http://hz.zhaomingkeji.xyz/gtcoyvtgku.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.52xcode.cn/gtexiczwbd.html

[Q29] 最大最小值
来源：http://hz.c1oappe.top/gtlgsutrfl.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.hongshengwenyu.top/gtynqpcyqj.html

[Q30] 分组统计
来源：http://hz.hammf.cn/gteprhypea.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.hongshengwenyu.top/gtzsizawbk.html

[Q31] 分组后过滤
来源：http://hz.hongshengwenyu.top/gtpknexvcd.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.redwolf501.top/gtwrgeaipd.html

[Q32] 分组拼接字符串
来源：http://hz.zhaomingkeji.xyz/gtxzffbnio.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.tianlin.xyz/gtgrggmhla.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.tian-w.cn/gtmhwedfxt.html

[Q33] 多列分组
来源：http://hz.meibo888.top/gtieqqfhgw.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.zhongyouzk.top/gtaseuwpnn.html

[Q34] 每组取第一条
来源：http://hz.cucudq.cn/gthtooxdog.html

SELECT * FROM (
来源：http://hz.chenjidiqi.icu/gtynepaixk.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.sysykeji.top/gtdedvuxoi.html

) t WHERE rn = 1;
来源：http://hz.yangfankeji.com/gtcnnxibia.html

[Q35] 内连接
来源：http://hz.haohaochexian.top/gthdzzgnwg.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.jiagoushi.top/gtplyujakj.html

[Q36] 左连接
来源：http://hz.dianchejie.cn/gthvaskdso.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.hywenlv.cn/gtjwuixqbm.html

[Q37] 右连接
来源：http://hz.shanyushiyangkeji.top/gtrxfwfrjb.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.yj202588.top/gtwdnavvdt.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.cucudq.cn/gtioomodnb.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.ydjk.org.cn/gtrpzyceic.html

[Q39] 自连接（查上下级）
来源：http://hz.0kj1m.cn/gtwbbejfjg.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.zhoulong.xyz/gtxdtqngif.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.tanke756.top/gthexcubeq.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.daxiang520.top/gtzdscuyon.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.aibaodan.cn/gtnvjfjtbu.html

[Q41] 多表连接
来源：http://hz.aizwys.cn/gtwixmlfrd.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.redwolf501.top/gthvqdncth.html

JOIN users u ON u.id = o.user_id
来源：http://hz.xuanzx.com/gtnizwypud.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.nwbrower.top/gtjtyefxac.html

[Q42] 连接条件附加过滤
来源：http://hz.shuidangran.top/gtitsuerum.html

SELECT u.name, o.amount FROM users u
来源：http://hz.ydjk.org.cn/gtrsofrzae.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.wangshuangyany.cn/gtqafzwqkn.html

[Q43] 标量子查询
来源：http://hz.snrcjt.cn/gtgrfhpihw.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.zhijiandao.cn/gturjrbbzf.html

[Q44] IN 子查询
来源：http://hz.xziqi.cn/gtlytzwoso.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.xinyue.icu/gthgjunlxk.html

[Q45] EXISTS 判断存在
来源：http://hz.birdmap.top/gtecuuamjk.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.birdmap.top/gttqemrglo.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.yanxiufei.cn/gtscjiogkv.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.pengpengdd.cyou/gtuvgtrvvc.html

[Q47] 与平均值比较
来源：http://hz.yuanzhike.top/gtanongypi.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.shangyingyoupin.top/gtoxvbudvm.html

[Q48] CTE 公用表表达式
来源：http://hz.ydzc1.top/gtbusqksvw.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.jqgfzy.top/gtnoplgayx.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.zhongyouzk.top/gtgfalgmib.html

[Q49] 更新单行
来源：http://hz.gotoacloud.top/gtcjbtmyrr.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.quarkkingdee.top/gtjukyeypc.html

[Q50] 批量更新
来源：http://hz.chenlongwang.top/gteitdfmbo.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.zhiwuduotai.top/gtwjvdqajn.html

[Q51] 用子查询更新
来源：http://hz.chenlongwang.top/gtgjjyvoqt.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.yj20258.top/gtvoockfkc.html

[Q52] 删除指定行
来源：http://hz.yj202588.top/gtuovawobz.html

DELETE FROM users WHERE id = 10;
来源：http://hz.yangfankeji.com/gtenhapwra.html

[Q53] 按条件删除
来源：http://hz.tianlin.xyz/gtkeaotaha.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.meibo888.top/gtylodxkdy.html

[Q54] 清空表
来源：http://hz.shuidangran.top/gtblnungov.html

TRUNCATE TABLE logs;
来源：http://hz.hongshengwenyu.top/gttdqvlrsz.html

[Q55] 排名（并列占位）
来源：http://hz.nanxuanxn.top/gtmmdjmkcx.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.wangdashe.top/gtxdoieuvg.html

[Q56] 密集排名（并列不占位）
来源：http://hz.yangfankeji.com/gtlzcxkoec.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.xuanzx.com/gtyuydcnoq.html

[Q57] 行号
来源：http://hz.yuxming.cn/gtsmeedutx.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.jinqigfzy.top/gtkvvzilfh.html

[Q58] 累计求和
来源：http://hz.shzxlz.cn/gtavyufqor.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.snrcjt.cn/gthitoglum.html

[Q59] 分组内累计
来源：http://hz.andypj.xyz/gtulfezimg.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.jinghuilouyu.cn/gtkpduilxk.html

[Q60] 取上一行 / 下一行
来源：http://hz.zhoulong.xyz/gtguqaqznb.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.nanxinkj.top/gtbgoyasyc.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.hammf.cn/gtgxvbienv.html

[Q61] 移动平均
来源：http://hz.sufxvd.cn/gtcfozzziw.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.ppjwa.cn/gtvxxgfcps.html

[Q62] 分组占比
来源：http://hz.dashuyun.cn/gtgvavagde.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.yj20258.top/gtkcxsgolp.html

[Q63] 开启事务
来源：http://hz.zhaomingkeji.xyz/gtnxlgicuq.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.cqqwz.cn/gtxfmbrhrr.html

[Q64] 提交事务
来源：http://hz.wangdashe.top/gtwrtzbudg.html

COMMIT;
来源：http://hz.sufxvd.cn/gthcfyhygr.html

[Q65] 回滚事务
来源：http://hz.tian-w.cn/gtjujtmart.html

ROLLBACK;
来源：http://hz.mhx1999.top/gtddvspmkt.html

[Q66] 行锁查询
来源：http://hz.zycfv.cn/gtmhhqjwii.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.havefunace.top/gtrckroqwg.html

[Q67] 设置隔离级别
来源：http://hz.jqgufenzy.top/gtlzmalgfb.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.wangshuangyany.cn/gtmqfvtubj.html

[Q68] 保存点
来源：http://hz.tianlin.xyz/gtrdwqjpqa.html

SAVEPOINT sp1;
来源：http://hz.shanyushiyangtech.top/gtniwypyxf.html

ROLLBACK TO sp1;
来源：http://hz.hfpthk.cn/gtlhjpfufi.html

[Q69] 查看执行计划
来源：http://hz.daxiang520.top/gtqcoivicx.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.yongpay.top/gtigcdprvq.html

[Q70] 更新统计信息
来源：http://hz.zdqjudy.top/gtviqvwhrx.html

ANALYZE TABLE users;
来源：http://hz.yonumen.top/gtkswghsag.html

[Q71] 查看建表语句
来源：http://hz.jyoumei.cn/gtefnogwoj.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.xziqi.cn/gtoyyaqlmh.html

[Q72] 查看索引
来源：http://hz.jqgufenzy.top/gtbedhputc.html

SHOW INDEX FROM users;
来源：http://hz.chenzaomai.com/gtofkffflx.html

[Q73] 查看表状态
来源：http://hz.feifeiyinyue.top/gtkmflblll.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.hnqzz.top/gtiuyajrzj.html

[Q74] 强制使用索引
来源：http://hz.aibaodan.cn/gtizucieks.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.tian-w.cn/gtqojxuasg.html

[Q75] 日期格式化
来源：http://hz.tanke756.top/gtjwdvvrmf.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.sysykeji.top/gtwghfdvlu.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.yongpay.top/gtzhmobyme.html

[Q76] 按天统计
来源：http://hz.sweek.top/gtejcsfswg.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.kuanghao11.cn/gtxwajktnd.html

[Q77] 时间加减
来源：http://hz.chenjidiqi.icu/gtiilffjxi.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.hfpthk.cn/gtolsjwaxh.html

[Q78] 当前时间
来源：http://hz.yangfankeji.com/gtqzgfsnop.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.shuidangran.top/gtvmbsvkft.html

[Q79] 字符串拼接
来源：http://hz.gaohongyu789.top/gtirljpera.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.yanxiufei.cn/gthqohpbws.html

[Q80] 字符串截取
来源：http://hz.fzhhl.top/gtmndcdtoq.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.zhijiandao.cn/gtkeufiwoe.html

[Q81] 字符串替换
来源：http://hz.jyoumei.cn/gtczvybhsq.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.zhijiandao.cn/gtmolvawxc.html

[Q82] 字符长度与字节长度
来源：http://hz.aizwys.cn/gtjovnfrvz.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.shanyushiyangkeji.top/gtjbnllmgq.html

[Q83] 大小写转换
来源：http://hz.jinghuilouyu.cn/gthzepovfv.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.xinyue.icu/gtydfehnvu.html

[Q84] 去除首尾空格
来源：http://hz.shanyushiyangtech.top/gtpqtgjbuj.html

SELECT TRIM(name) FROM users;
来源：http://hz.cucudq.cn/gtmusnttiy.html

[Q85] 数值取整
来源：http://hz.ydjk.org.cn/gtiqjsgspt.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.chenlongwang.top/gteuuftqkz.html

[Q86] 读取 JSON 字段
来源：http://hz.zdqjudy.top/gtjcbbozfj.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.aizwys.cn/gtlgvacotw.html

[Q87] JSON 字段做条件
来源：http://hz.hysaishi.cn/gtmthmtikr.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.yueranfly.top/gtxaweitcw.html

[Q88] 行转列（条件聚合）
来源：http://hz.bjfxy.top/gtwosycplo.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.vqdsnc.cn/gtklbvltte.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.aibaodan.cn/gtwveorliq.html

[Q89] 判断表是否存在
来源：http://hz.dashuyun.cn/gtaxjbleze.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.haohaochexian.top/gtegkjocru.html

[Q90] 生成序号列
来源：http://hz.yj20258888.top/gtnasgmenm.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.shanyushiyangkeji.top/gtdjwhhquk.html

================================================================================
来源：http://hz.xziqi.cn/gtuyshrozc.html

R. Bash 专题
来源：http://hz.hysaishi.cn/gtdwunpnkl.html

================================================================================
来源：http://hz.chenzaomai.com/gtytrythpz.html

[R01] shebang 与严格模式
来源：http://hz.ydjk.org.cn/gtcywifwoy.html

#!/usr/bin/env bash
来源：http://hz.yvedp.cn/gtxhsltvvb.html

set -euo pipefail
来源：http://hz.jqgfzy.top/gtshevbnyx.html

[R02] 变量赋值与使用
来源：http://hz.meibo888.top/gtgofeveut.html

name="Tom"; echo "$name"
来源：http://hz.xuanzx.com/gtcxrrpspi.html

[R03] 只读变量
来源：http://hz.jinqigufen.top/gtzeqimuov.html

readonly PI=3.14
来源：http://hz.yj20258.top/gtwossxmty.html

[R04] 位置参数
来源：http://hz.9152youxi.cn/gtijtpeepc.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.gaohongyu789.top/gtfpkxdzdt.html

[R05] 参数默认值
来源：http://hz.hammf.cn/gtxwvyxkws.html

name="${1:-default}"
来源：http://hz.yj202588.top/gtturrklbl.html

[R06] 判断命令是否存在
来源：http://hz.yanxiufei.cn/gtlixbcfzp.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.pengpengdd.cyou/gtlcijyzsx.html

[R07] if 判断文件
来源：http://hz.sxryk.cn/gtmvtwsyps.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.hfpthk.cn/gtdoqdsfsj.html

[R08] 数值比较
来源：http://hz.kuanghao11.cn/gttcbpvemm.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.mhx1999.top/gtqrgkxlru.html

[R09] 字符串比较
来源：http://hz.ehwqpu.com/gtvvtzxlhi.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.dianchejie.cn/gtpcpteewx.html

[R10] 正则匹配
来源：http://hz.zhijiandao.cn/gtohzpvbmk.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.daria6918.cn/gtrvxazzcs.html

[R11] case 多分支
来源：http://hz.iojbl.cn/gtcfzmuhbl.html

case "$1" in
来源：http://hz.yj20258888.top/gtpmbewhkv.html

start) echo "启动" ;;
来源：http://hz.quarkkingdee.top/gtzdyesrbf.html

stop)  echo "停止" ;;
来源：http://hz.yj20258888.top/gtamzgwllf.html

*)     echo "未知命令" ;;
来源：http://hz.nanxinkj.top/gtnnxykyjm.html

esac
来源：http://hz.gaohongyu789.top/gtrasiaicb.html

[R12] for 遍历文件
来源：http://hz.yj20258888.top/gtvcdzrajm.html

for f in *.txt; do echo "$f"; done
来源：http://hz.ydjk.org.cn/gtagyepczf.html

[R13] for 计数循环
来源：http://hz.daxiang520.top/gtdhumiunt.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.jinghuilouyu.cn/gttxfwpbkw.html

[R14] C 风格 for
来源：http://hz.gaohongyu789.top/gtlkjbmzgi.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.zhixingplan.top/gthjhruvyq.html

[R15] while 逐行读文件
来源：http://hz.quarkkingdee.top/gtdfztgsao.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.nanxinkj.top/gtiejtuhtv.html

[R16] until 等待条件
来源：http://hz.andypj.xyz/gtoipwdfba.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.vqdsnc.cn/gtkygjvjql.html

[R17] 数组定义与取值
来源：http://hz.hnqzz.top/gtgntmazuh.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.feifeiyinyue.top/gtyhdctpkd.html

[R18] 遍历数组
来源：http://hz.tian-w.cn/gtilsfnuaj.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.bjfxy.top/gtfwdkbkso.html

[R19] 数组长度
来源：http://hz.yj20258.top/gttinqrqpa.html

echo "${#arr[@]}"
来源：http://hz.shuidangran.top/gtzcnbccyg.html

[R20] 关联数组（字典）
来源：http://hz.iojbl.cn/gtdgsbkhiw.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.haohaochexian.top/gtasxpcjfm.html

[R21] 字符串长度
来源：http://hz.havefunace.top/gtswvfhuet.html


<!-- 参考信息 -->