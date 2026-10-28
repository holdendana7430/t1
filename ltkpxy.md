代发 wailian999

Java: list.size();  map.size();  s.length()
来源：http://hz.quarkkingdee.top/gtlmqsvwfm.html

Go:   len(arr);  len(m)
来源：http://hz.birdmap.top/gtprqtsdyn.html

Ruby: x.length;  x.size
来源：http://hz.cucudq.cn/gtjaruhtrj.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.fengsongda.top/gtfhuxgutp.html

[P05] 判断两个对象内容是否相等
来源：http://hz.sysykeji.top/gtlhihkwbm.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.birdmap.top/gtcwvbcxmi.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.gzhubu.top/gthlwmffpy.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.yvedp.cn/gtziyaoyxl.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.cqqwz.cn/gtrqkibsnr.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.jiagoushi.top/gtvjvszkxo.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.kuanghao11.cn/gtylhrnrwp.html

Ruby: a == b
来源：http://hz.gotoacloud.top/gtkhubqhbi.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.jiagoushi.top/gtbwsozims.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.tian-w.cn/gtuaezplue.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.ydzc1.top/gtoedscqxf.html

PHP:  if (empty($x)) {}
来源：http://hz.feifeiyinyue.top/gtuvfrisjt.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.wangshuangyany.cn/gtqfgbbirx.html

TS:   if (x == null) {}
来源：http://hz.ybcxt.top/gttoapsxvd.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.guannengcc.top/gthrhtwxcv.html

Go:   if x == nil {}
来源：http://hz.yuxming.cn/gtdojrdyuv.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.shanyushiyangkeji.top/gtzbuewkop.html

C#:   if (x is null) {}
来源：http://hz.yongpay.top/gtpvqlnohq.html

[P07] 防抖与节流
来源：http://hz.haohaochexian.top/gthikfuwwl.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.hammf.cn/gtlhxdtjyk.html

PHP:  // 手写时间戳比较
来源：http://hz.birdmap.top/gtevcyeiqh.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.cdnleiting.top/gtqkhisdsy.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.ydzc1.top/gtjvshsmed.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.yonumen.top/gtyuorsnzr.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.yuxming.cn/gtsrcijugp.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.daria6918.cn/gtxbtwjfxj.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.hnxiangtu.top/gtfhszlmqz.html

[P08] 处理浮点精度问题
来源：http://hz.cucudq.cn/gtfelauqkw.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.yj20258.top/gtpjfgmcxh.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.nwbrower.top/gtzdjxdqcq.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.bjfxy.top/gtfuhwknjd.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.cashguo.top/gtmaqeiydh.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.hnqzz.top/gtlwckgeqe.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.hywenlv.cn/gtebkhwflr.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.shanyushiyangkeji.top/gtirbiyudi.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.cucudq.cn/gtqoimlrqs.html

================================================================================
来源：http://hz.aibaodan.cn/gtapsygkkg.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.52xcode.cn/gtnjqnvkfz.html

================================================================================
来源：http://hz.ydzc1.top/gtaadngrtz.html

[Q01] 创建表
来源：http://hz.0kj1m.cn/gtckfdrqfm.html

CREATE TABLE users (
来源：http://hz.svipenyu.cn/gtrzcwelta.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.shuidangran.top/gtjolfdfvp.html

name VARCHAR(50) NOT NULL,
来源：http://hz.mhx1999.top/gtqnesazoj.html

email VARCHAR(100) UNIQUE,
来源：http://hz.zhoulong.xyz/gtnwvdcgtd.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.shangyingyoupin.top/gtxywdopuf.html

);
来源：http://hz.hammf.cn/gtgrcrlcuc.html

[Q02] 创建带外键的表
来源：http://hz.iojbl.cn/gtrhtsagcj.html

CREATE TABLE orders (
来源：http://hz.ybcxt.top/gtggupdtyh.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.birdmap.top/gtusvkrtol.html

user_id INT NOT NULL,
来源：http://hz.jqgufenzy.top/gtbzuihiqu.html

amount DECIMAL(10, 2),
来源：http://hz.hysaishi.cn/gtuagcfzmo.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.316326.xyz/gtisvaansy.html

);
来源：http://hz.zhengqikj.top/gtmrymzgfq.html

[Q03] 增加列
来源：http://hz.ydzc1.top/gtmbqlmvsn.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.birdmap.top/gtsrywllkx.html

[Q04] 修改列类型
来源：http://hz.jinqigfzy.top/gtmdegzzsm.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.dashuyun.cn/gtwdrrjbcv.html

[Q05] 重命名列
来源：http://hz.snrcjt.cn/gtgefpblof.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.9152youxi.cn/gtsxbillgn.html

[Q06] 删除列
来源：http://hz.shanyushiyangtech.top/gtbcffqhab.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.cqqwz.cn/gtcybjpigu.html

[Q07] 删除表
来源：http://hz.cqqwz.cn/gtreqwlnkq.html

DROP TABLE IF EXISTS orders;
来源：http://hz.zhijiandao.cn/gtmmxnynpm.html

[Q08] 创建普通索引
来源：http://hz.svipenyu.cn/gtorbmznnj.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.andypj.xyz/gtjmlomzxz.html

[Q09] 创建唯一索引
来源：http://hz.daxiang520.top/gtbfmgeapu.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.redwolf501.top/gteupmspia.html

[Q10] 插入单行
来源：http://hz.guannengcc.top/gtknbpbthb.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.aibaodan.cn/gtjtyihtmk.html

[Q11] 一次插入多行
来源：http://hz.xziqi.cn/gtsmbopsql.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.iojbl.cn/gtkdokbqia.html

[Q12] 插入后取自增 ID
来源：http://hz.bjfxy.top/gtrfxfrter.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.hywenlv.cn/gtuybpoycf.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.redwolf501.top/gtadifqolt.html

[Q13] 忽略重复插入
来源：http://hz.fengsongda.top/gtlqdimkwz.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.gzhubu.top/gthakagtlq.html

[Q14] 存在则更新（upsert）
来源：http://hz.xuanzx.com/gtvjnkepku.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.hnxiangtu.top/gttrxpvamb.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.redwolf501.top/gtjqzelxcr.html

[Q15] 查询全部
来源：http://hz.xuetiantiany.cn/gtbhryopqo.html

SELECT * FROM users;
来源：http://hz.cqqwz.cn/gtwauukafu.html

[Q16] 查询指定列
来源：http://hz.chenjidiqi.icu/gtcdilzkkr.html

SELECT id, name FROM users;
来源：http://hz.yj202588.top/gtobujjswn.html

[Q17] 条件查询
来源：http://hz.sweek.top/gtxmlgbdvo.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.hongshengwenyu.top/gthfdsrive.html

[Q18] 模糊匹配
来源：http://hz.hnqzz.top/gthlbfxzww.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.jlsjyb.cn/gtzfxmzyoc.html

[Q19] 范围查询
来源：http://hz.jianghu66.top/gtykufowxj.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.nanxinkj.top/gthfrtplfc.html

[Q20] IN 列表
来源：http://hz.jinqigfzy.top/gtphdttdyq.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.hfpthk.cn/gtcwpnqspo.html

[Q21] 空值判断
来源：http://hz.hammf.cn/gtlrdejwcm.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.svipenyu.cn/gtckjkhlex.html

[Q22] 排序
来源：http://hz.yangfankeji.com/gtpyqonvan.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.yj20258.top/gtliugpzrw.html

[Q23] 分页
来源：http://hz.hongshengwenyu.top/gtzyhrpvkv.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.xuanzx.com/gtitynwtai.html

[Q24] 去重
来源：http://hz.yueranfly.top/gtpkanrzmf.html

SELECT DISTINCT city FROM users;
来源：http://hz.pengpengdd.cyou/gtxcsbhkgl.html

[Q25] 只取前 N 条
来源：http://hz.zhoulong.xyz/gtvifmydkz.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.gogol.net.cn/gtmrxxfjsz.html

[Q26] 计数
来源：http://hz.aibaodan.cn/gtrfjbqdjy.html

SELECT COUNT(*) FROM users;
来源：http://hz.yanxiufei.cn/gtjwewazfk.html

[Q27] 条件计数
来源：http://hz.quarkkingdee.top/gtbrbtfisx.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.aizwys.cn/gtkrcgmdde.html

[Q28] 求和与平均
来源：http://hz.jyoumei.cn/gtavwzelfd.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.jiagoushi.top/gtewcbhkdf.html

[Q29] 最大最小值
来源：http://hz.jinghuilouyu.cn/gtnateseek.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.nwbrower.top/gtokwyvusa.html

[Q30] 分组统计
来源：http://hz.zhongyouzk.top/gtyrooddni.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.gzhubu.top/gtyhhhvlxm.html

[Q31] 分组后过滤
来源：http://hz.jinqigufen.top/gttkusdwqc.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.gogol.net.cn/gtsezyoenh.html

[Q32] 分组拼接字符串
来源：http://hz.tianlin.xyz/gtrojevunj.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.jlsjyb.cn/gtjgartaom.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.dianchejie.cn/gtoxqxkkso.html

[Q33] 多列分组
来源：http://hz.daria6918.cn/gtrtwrqebq.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.daxiang520.top/gtagptpgjw.html

[Q34] 每组取第一条
来源：http://hz.daria6918.cn/gtllltpimf.html

SELECT * FROM (
来源：http://hz.feifeiyinyue.top/gtpsosoalt.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.52xcode.cn/gtrnbikiow.html

) t WHERE rn = 1;
来源：http://hz.chenlongwang.top/gtcvpfhxdm.html

[Q35] 内连接
来源：http://hz.chenlongwang.top/gtkugmjlzy.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.havefunace.top/gtyofszyuj.html

[Q36] 左连接
来源：http://hz.hammf.cn/gtkqegpqkh.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.nanxuanxn.top/gtetwwnhxc.html

[Q37] 右连接
来源：http://hz.cucudq.cn/gtmjzdbltn.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.zhoulong.xyz/gtwicctgil.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.andypj.xyz/gtgpdzuzlv.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.jinqigufen.top/gtpiwmhzub.html

[Q39] 自连接（查上下级）
来源：http://hz.svipenyu.cn/gtxrtjudrp.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.yueranfly.top/gtxczjnizn.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.hnqzz.top/gtsidqysdi.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.ehwqpu.com/gtskupkirl.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.ydjk.org.cn/gttsuxuxdl.html

[Q41] 多表连接
来源：http://hz.zhixingplan.top/gttdwbdjek.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.daxiang520.top/gtbikddyir.html

JOIN users u ON u.id = o.user_id
来源：http://hz.chenzaomai.com/gtbbmlbqzu.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.hfpthk.cn/gtuduwwgxz.html

[Q42] 连接条件附加过滤
来源：http://hz.haohaochexian.top/gtivjqgsfy.html

SELECT u.name, o.amount FROM users u
来源：http://hz.snrcjt.cn/gtjrznwtbh.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.svipenyu.cn/gtqhqmedmw.html

[Q43] 标量子查询
来源：http://hz.chenzaomai.com/gtvipuwwke.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.jinghuilouyu.cn/gtwndzdtzq.html

[Q44] IN 子查询
来源：http://hz.ivvv.top/gthgrbmblt.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.redwolf501.top/gtkbdllsiy.html

[Q45] EXISTS 判断存在
来源：http://hz.xinyue.icu/gthpmyztba.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.0kj1m.cn/gtzlmqivtk.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.jinqigufen.top/gtfdtxwltp.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.tianlin.xyz/gtlavnekhg.html

[Q47] 与平均值比较
来源：http://hz.guannengcc.top/gtzmlgdenl.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.pycfn.com/gteigshhsl.html

[Q48] CTE 公用表表达式
来源：http://hz.iojbl.cn/gtpqtdjjyj.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.snrcjt.cn/gtuibfuiof.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.svipenyu.cn/gtshgwitaq.html

[Q49] 更新单行
来源：http://hz.jlsjyb.cn/gtimseeyue.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.smart0.xyz/gtxouzbfjq.html

[Q50] 批量更新
来源：http://hz.yvedp.cn/gtcdqndivb.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.jinyuanbaomall.cn/gtpmfzoqsv.html

[Q51] 用子查询更新
来源：http://hz.yvedp.cn/gtsczttwbo.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.cucudq.cn/gtabjhuysb.html

[Q52] 删除指定行
来源：http://hz.jlsjyb.cn/gtrxebzgum.html

DELETE FROM users WHERE id = 10;
来源：http://hz.ppjwa.cn/gtenyjccyg.html

[Q53] 按条件删除
来源：http://hz.zycfv.cn/gtnqiyomuz.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.shanyushiyangtech.top/gturwisbtz.html

[Q54] 清空表
来源：http://hz.xylfe.cn/gtzuffbtna.html

TRUNCATE TABLE logs;
来源：http://hz.fzhhl.top/gtamrutbrn.html

[Q55] 排名（并列占位）
来源：http://hz.hywenlv.cn/gtyispnoqb.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.yuanzhike.top/gtwgkwhpix.html

[Q56] 密集排名（并列不占位）
来源：http://hz.svipenyu.cn/gtukjiwibs.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.sysykeji.top/gtkcsymwbf.html

[Q57] 行号
来源：http://hz.jiagoushi.top/gtcdlptzou.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.chenzaomai.com/gtqscsyniw.html

[Q58] 累计求和
来源：http://hz.kuanghao11.cn/gtptnxxbcc.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.feifeiyinyue.top/gtphxlmrpe.html

[Q59] 分组内累计
来源：http://hz.daxiang520.top/gtnkqmpmqb.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.guowangkeji.top/gtejlgkjgu.html

[Q60] 取上一行 / 下一行
来源：http://hz.316326.xyz/gtdfglnzjm.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.sweek.top/gtxkrtjogw.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.birdmap.top/gtuvqftebp.html

[Q61] 移动平均
来源：http://hz.guowangkeji.top/gtvylghzhg.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.sxryk.cn/gtijcmjpow.html

[Q62] 分组占比
来源：http://hz.ppjwa.cn/gtotzqhfqg.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.kuanghao11.cn/gtletspbih.html

[Q63] 开启事务
来源：http://hz.shuidangran.top/gtvmkfxupe.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.zycfv.cn/gttcvmfpqm.html

[Q64] 提交事务
来源：http://hz.wangshuangyany.cn/gtyfduagyf.html

COMMIT;
来源：http://hz.jianghu66.top/gtmnckgfst.html

[Q65] 回滚事务
来源：http://hz.jqgfzy.top/gtxzgtmzpn.html

ROLLBACK;
来源：http://hz.yj202588.top/gthoslacrt.html

[Q66] 行锁查询
来源：http://hz.redwolf501.top/gtevaokolv.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.feifeiyinyue.top/gtkenmmuhg.html

[Q67] 设置隔离级别
来源：http://hz.jyoumei.cn/gttkydqwen.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.aibaodan.cn/gtlohfawds.html

[Q68] 保存点
来源：http://hz.sysykeji.top/gttibwdgnu.html

SAVEPOINT sp1;
来源：http://hz.jinqigfzy.top/gtcsoltqkh.html

ROLLBACK TO sp1;
来源：http://hz.chenzaomai.com/gtoixdkqwh.html

[Q69] 查看执行计划
来源：http://hz.jyoumei.cn/gtqawgyuja.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.hywenlv.cn/gtsuzzpstv.html

[Q70] 更新统计信息
来源：http://hz.yj20258.top/gtmfsbegnl.html

ANALYZE TABLE users;
来源：http://hz.zhongyouzk.top/gtprggcrqr.html

[Q71] 查看建表语句
来源：http://hz.shangyingyoupin.top/gtpbgqfhjh.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.gzhubu.top/gtwccknmvu.html

[Q72] 查看索引
来源：http://hz.zhaomingkeji.xyz/gtpvnnxsbc.html

SHOW INDEX FROM users;
来源：http://hz.snrcjt.cn/gtlddlvzgn.html

[Q73] 查看表状态
来源：http://hz.c1oappe.top/gtothbutpo.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.xuetiantiany.cn/gtiywfwkte.html

[Q74] 强制使用索引
来源：http://hz.andypj.xyz/gtyvflldmt.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.nanxuanxn.top/gtzomsbhgw.html

[Q75] 日期格式化
来源：http://hz.zhixingplan.top/gtqgewtana.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.pycfn.com/gtdzoijhkg.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.c1oappe.top/gtpnhdryow.html

[Q76] 按天统计
来源：http://hz.tianlin.xyz/gtguksnqwq.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.yueranfly.top/gtxzytpmej.html

[Q77] 时间加减
来源：http://hz.tianlin.xyz/gtguhejrtk.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.zhixingplan.top/gtociqqjim.html

[Q78] 当前时间
来源：http://hz.cheryme.top/gtgjwrigfh.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.ydzc1.top/gtzdcrdshf.html

[Q79] 字符串拼接
来源：http://hz.hnqzz.top/gtjikzwtsu.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.guannengcc.top/gtseyhquho.html

[Q80] 字符串截取
来源：http://hz.wangshuangyany.cn/gtdcrgjfbu.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.andypj.xyz/gtpgeujojn.html

[Q81] 字符串替换
来源：http://hz.hysaishi.cn/gtbwmmtvnq.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.jinqigufen.top/gtigldxsbo.html

[Q82] 字符长度与字节长度
来源：http://hz.redwolf501.top/gtyveimatm.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.ywan-chungtsiang.top/gtpatngzcn.html

[Q83] 大小写转换
来源：http://hz.hywenlv.cn/gtqqopdjvh.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.tianlin.xyz/gtiotvcvgh.html

[Q84] 去除首尾空格
来源：http://hz.zdqjudy.top/gtmccrbqbh.html

SELECT TRIM(name) FROM users;
来源：http://hz.mhx1999.top/gtbosnwayu.html

[Q85] 数值取整
来源：http://hz.andypj.xyz/gtjjrtklzl.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.dashuyun.cn/gtgphwcqtv.html

[Q86] 读取 JSON 字段
来源：http://hz.iojbl.cn/gtdnkngavx.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.gogol.net.cn/gtgibmeobx.html

[Q87] JSON 字段做条件
来源：http://hz.yuxming.cn/gtqcwyzptr.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.sufxvd.cn/gtbttnzkiy.html

[Q88] 行转列（条件聚合）
来源：http://hz.zhoulong.xyz/gtzawlhcwt.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.jqgufenzy.top/gtizgrormt.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.shanyushiyangtech.top/gtlcbimufv.html

[Q89] 判断表是否存在
来源：http://hz.sxryk.cn/gtdzwpexdy.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.zycfv.cn/gtyiiseumm.html

[Q90] 生成序号列
来源：http://hz.chenjidiqi.icu/gtrubrbnwg.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.sufxvd.cn/gtzdqkzboa.html

================================================================================
来源：http://hz.chenlongwang.top/gthimhpqse.html

R. Bash 专题
来源：http://hz.cucudq.cn/gtihusmexs.html

================================================================================
来源：http://hz.gzhubu.top/gtorrrnutn.html

[R01] shebang 与严格模式
来源：http://hz.xingfuxueyuan.xyz/gtcmeeracp.html

#!/usr/bin/env bash
来源：http://hz.9152youxi.cn/gtpnzkspbd.html

set -euo pipefail
来源：http://hz.ivvv.top/gtmriptlqa.html

[R02] 变量赋值与使用
来源：http://hz.shanyushiyangkeji.top/gtvzwvakxi.html

name="Tom"; echo "$name"
来源：http://hz.kuanghao11.cn/gtawnsmcfq.html

[R03] 只读变量
来源：http://hz.cucudq.cn/gthqvzcqgm.html

readonly PI=3.14
来源：http://hz.haohaochexian.top/gtnakxuwwx.html

[R04] 位置参数
来源：http://hz.yonumen.top/gtiozfsaks.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.sysykeji.top/gttywejynn.html

[R05] 参数默认值
来源：http://hz.ybcxt.top/gtdgtpvwpk.html

name="${1:-default}"
来源：http://hz.c1oappe.top/gtncjchwqm.html

[R06] 判断命令是否存在
来源：http://hz.tianlin.xyz/gtqeoqqprc.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.vqdsnc.cn/gtwrhfekdi.html

[R07] if 判断文件
来源：http://hz.pycfn.com/gtvqptgjyh.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.bjfxy.top/gtqjzcavah.html

[R08] 数值比较
来源：http://hz.quarkkingdee.top/gtywqmiojc.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.jianghu66.top/gtefvvzeup.html

[R09] 字符串比较
来源：http://hz.meibo888.top/gtarwarvep.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.gogol.net.cn/gtcuuixqtq.html

[R10] 正则匹配
来源：http://hz.gzhubu.top/gtrcfaufdi.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.cdnleiting.top/gtrdhzaqng.html

[R11] case 多分支
来源：http://hz.shzxlz.cn/gtivpedxxs.html

case "$1" in
来源：http://hz.svipenyu.cn/gtdcrsokml.html

start) echo "启动" ;;
来源：http://hz.feifeiyinyue.top/gtgueqziuj.html

stop)  echo "停止" ;;
来源：http://hz.zhaomingkeji.xyz/gtvjkhdbct.html

*)     echo "未知命令" ;;
来源：http://hz.zhaomingkeji.xyz/gtxyskqrgt.html

esac
来源：http://hz.sysykeji.top/gtxyjmothc.html

[R12] for 遍历文件
来源：http://hz.52xcode.cn/gttycyahxf.html

for f in *.txt; do echo "$f"; done
来源：http://hz.jyoumei.cn/gtghfflknm.html

[R13] for 计数循环
来源：http://hz.yangfankeji.com/gtiprwliqa.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.xingfuxueyuan.xyz/gthpvwumgw.html

[R14] C 风格 for
来源：http://hz.haohaochexian.top/gthwtverdb.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.hfpthk.cn/gtcsuavhhe.html

[R15] while 逐行读文件
来源：http://hz.andypj.xyz/gtomysrmuq.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.zhiwuduotai.top/gtpdglzgvd.html

[R16] until 等待条件
来源：http://hz.hongshengwenyu.top/gtdxlzkkep.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.zhiwuduotai.top/gtdqljijwu.html

[R17] 数组定义与取值
来源：http://hz.jinqigufen.top/gtdfdormzz.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.shanyushiyangtech.top/gtzqmqygpk.html

[R18] 遍历数组
来源：http://hz.mhx1999.top/gtpawnwrys.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.hysaishi.cn/gtgzahfdow.html

[R19] 数组长度
来源：http://hz.316326.xyz/gtmiwzeirs.html

echo "${#arr[@]}"
来源：http://hz.hysaishi.cn/gtzhihdxuj.html

[R20] 关联数组（字典）
来源：http://hz.mhx1999.top/gtjrybegck.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.xylfe.cn/gtruoldbsl.html

[R21] 字符串长度
来源：http://hz.birdmap.top/gtkzjhijzf.html

echo "${#s}"
来源：http://hz.quarkkingdee.top/gtapogdnxw.html

[R22] 截取子串
来源：http://hz.zhoulong.xyz/gtstdxnzzb.html

echo "${s:0:5}"
来源：http://hz.shuidangran.top/gtqretqgfq.html

[R23] 字符串替换
来源：http://hz.yj20258.top/gtpyvjqrnx.html


<!-- 参考信息 -->