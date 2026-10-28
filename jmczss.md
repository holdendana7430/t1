代发 wailian999

[P05] 判断两个对象内容是否相等
来源：http://hz.sufxvd.cn/gtmldefgio.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.jiagoushi.top/gteggopifi.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.tian-w.cn/gtpaldouiz.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.0kj1m.cn/gtuovvpdtt.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.zycfv.cn/gtrsmvxovj.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.zhengqikj.top/gtbqzhycsa.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.zhaomingkeji.xyz/gtcwgkcuit.html

Ruby: a == b
来源：http://hz.gzhubu.top/gtrdnkyejh.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.shangyingyoupin.top/gtqskhtftn.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.gaohongyu789.top/gtmejoxrto.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.aibaodan.cn/gtmtfcmpkp.html

PHP:  if (empty($x)) {}
来源：http://hz.nanxuanxn.top/gtphrqnraw.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.zhiwuduotai.top/gtuqlvvytt.html

TS:   if (x == null) {}
来源：http://hz.zhiwuduotai.top/gtrsacrgfx.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.jinghuilouyu.cn/gtvsuamzfh.html

Go:   if x == nil {}
来源：http://hz.jinghuilouyu.cn/gtqdhtxtbc.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.xuetiantiany.cn/gtfrclbvuy.html

C#:   if (x is null) {}
来源：http://hz.quarkkingdee.top/gtyjogorvv.html

[P07] 防抖与节流
来源：http://hz.yongpay.top/gthppakuhr.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.zycfv.cn/gtzjvoyaig.html

PHP:  // 手写时间戳比较
来源：http://hz.316326.xyz/gtgxoywlei.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.ydjk.org.cn/gtjzmxikgc.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.shangyingyoupin.top/gtjruqlxee.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.nwbrower.top/gtukrozqyy.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.nanxuanxn.top/gtjhnaxdtp.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.316326.xyz/gtetagxcrh.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.wangdashe.top/gtqzvamotr.html

[P08] 处理浮点精度问题
来源：http://hz.cdnleiting.top/gtlveeumct.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.redwolf501.top/gtllnhtolr.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.birdmap.top/gtoktgkvhw.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.xylfe.cn/gtrnokbsrq.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.zhaomingkeji.xyz/gtvmgstbfy.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.hnqzz.top/gtvfiwbawn.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.c1oappe.top/gtzcuzmtkt.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.yangfankeji.com/gtswoftwbu.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.jiagoushi.top/gtukkbldak.html

================================================================================
来源：http://hz.andypj.xyz/gtoryghdqa.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.havefunace.top/gtgtjjbkzm.html

================================================================================
来源：http://hz.cheryme.top/gtxkjglaui.html

[Q01] 创建表
来源：http://hz.zhiwuduotai.top/gtxwemsczk.html

CREATE TABLE users (
来源：http://hz.ppjwa.cn/gtsyqfdrvw.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.cucudq.cn/gtgcjdatwc.html

name VARCHAR(50) NOT NULL,
来源：http://hz.ydzc1.top/gtddezithj.html

email VARCHAR(100) UNIQUE,
来源：http://hz.pycfn.com/gtseuwwzod.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.hnqzz.top/gtnyfegbhr.html

);
来源：http://hz.ehwqpu.com/gtpyfeaoqo.html

[Q02] 创建带外键的表
来源：http://hz.mhx1999.top/gtfdbonqcu.html

CREATE TABLE orders (
来源：http://hz.jinghuilouyu.cn/gtuxolazfw.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.ppjwa.cn/gtwqeqpijl.html

user_id INT NOT NULL,
来源：http://hz.aibaodan.cn/gtcjnmjzsn.html

amount DECIMAL(10, 2),
来源：http://hz.daria6918.cn/gtujryfkcj.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.zycfv.cn/gtclefwjml.html

);
来源：http://hz.gzhubu.top/gtbzchpoob.html

[Q03] 增加列
来源：http://hz.xuetiantiany.cn/gttfruavvc.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.jyoumei.cn/gtbfniibmv.html

[Q04] 修改列类型
来源：http://hz.cheryme.top/gtirjjvdaj.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.hongshengwenyu.top/gtdvquukgt.html

[Q05] 重命名列
来源：http://hz.tianlin.xyz/gtnssycipw.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.9152youxi.cn/gtyyiexnrn.html

[Q06] 删除列
来源：http://hz.bjfxy.top/gtimcsutpb.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.hnqzz.top/gtvgjknuag.html

[Q07] 删除表
来源：http://hz.hammf.cn/gtvegohptz.html

DROP TABLE IF EXISTS orders;
来源：http://hz.jqgufenzy.top/gtycshsylw.html

[Q08] 创建普通索引
来源：http://hz.guannengcc.top/gtcedvgkub.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.shzxlz.cn/gtfcfvkwdo.html

[Q09] 创建唯一索引
来源：http://hz.shanyushiyangkeji.top/gtrnyrqeqb.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.xziqi.cn/gtedigjmbe.html

[Q10] 插入单行
来源：http://hz.ywan-chungtsiang.top/gthfkakecz.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.chenjidiqi.icu/gtigsvhuua.html

[Q11] 一次插入多行
来源：http://hz.gzhubu.top/gtztqcidrv.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.smart0.xyz/gtlcswmcrd.html

[Q12] 插入后取自增 ID
来源：http://hz.daria6918.cn/gtbffrdnmf.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.hfpthk.cn/gtwrnlarnh.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.fzhhl.top/gtddllqehi.html

[Q13] 忽略重复插入
来源：http://hz.jianghu66.top/gtaavfqapw.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.sxryk.cn/gtgnyicfbh.html

[Q14] 存在则更新（upsert）
来源：http://hz.52xcode.cn/gtygbljjfe.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.snrcjt.cn/gtbavpqayr.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.ywan-chungtsiang.top/gtghvtlxlr.html

[Q15] 查询全部
来源：http://hz.bjfxy.top/gtvkjfprst.html

SELECT * FROM users;
来源：http://hz.xuanzx.com/gtiipjwfue.html

[Q16] 查询指定列
来源：http://hz.jinqigfzy.top/gtymyqkcfk.html

SELECT id, name FROM users;
来源：http://hz.xuanzx.com/gthirrjuzk.html

[Q17] 条件查询
来源：http://hz.hysaishi.cn/gtghbknctw.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.9152youxi.cn/gtkyvtaexa.html

[Q18] 模糊匹配
来源：http://hz.kuanghao11.cn/gtukigumsl.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.xuetiantiany.cn/gtnvbjaacp.html

[Q19] 范围查询
来源：http://hz.yj20258.top/gtpvzbnfkb.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.c1oappe.top/gtzivstbpg.html

[Q20] IN 列表
来源：http://hz.jinqigufen.top/gtgzyoibll.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.yonumen.top/gtucfoylst.html

[Q21] 空值判断
来源：http://hz.snrcjt.cn/gtdyqvtsug.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.yanxiufei.cn/gttkmmfkas.html

[Q22] 排序
来源：http://hz.fengsongda.top/gtcjziflre.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.vqdsnc.cn/gtoaubseff.html

[Q23] 分页
来源：http://hz.havefunace.top/gtcbrjqejj.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.chenlongwang.top/gtafalxree.html

[Q24] 去重
来源：http://hz.xinyue.icu/gtjaevkdsx.html

SELECT DISTINCT city FROM users;
来源：http://hz.xziqi.cn/gtqpjttequ.html

[Q25] 只取前 N 条
来源：http://hz.shangyingyoupin.top/gtbtopzemu.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.c1oappe.top/gtssuqprif.html

[Q26] 计数
来源：http://hz.gaohongyu789.top/gtirciczsh.html

SELECT COUNT(*) FROM users;
来源：http://hz.daxiang520.top/gtppdqtwhu.html

[Q27] 条件计数
来源：http://hz.shzxlz.cn/gthmrlcrkk.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.tianlin.xyz/gtbhjoefyg.html

[Q28] 求和与平均
来源：http://hz.yj202588.top/gtroehyity.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.xuetiantiany.cn/gtiyezbvyw.html

[Q29] 最大最小值
来源：http://hz.yuxming.cn/gtycjejgge.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.shzxlz.cn/gtgecdxezu.html

[Q30] 分组统计
来源：http://hz.nanxuanxn.top/gtsfbortcq.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.xingfuxueyuan.xyz/gtyxxqrksc.html

[Q31] 分组后过滤
来源：http://hz.shanyushiyangkeji.top/gtunkvfubf.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.iojbl.cn/gthevgbbwq.html

[Q32] 分组拼接字符串
来源：http://hz.hnxiangtu.top/gtgnzmbeuo.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.zhijiandao.cn/gtntwkygrp.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.daxiang520.top/gtugbtoxgz.html

[Q33] 多列分组
来源：http://hz.quarkkingdee.top/gtfdvbochl.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.hywenlv.cn/gttmcgoqus.html

[Q34] 每组取第一条
来源：http://hz.hnxiangtu.top/gtxlqbuykh.html

SELECT * FROM (
来源：http://hz.xinyue.icu/gtogauhgiy.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.hywenlv.cn/gtbubithpw.html

) t WHERE rn = 1;
来源：http://hz.shanyushiyangtech.top/gtkwtwpdkz.html

[Q35] 内连接
来源：http://hz.hnqzz.top/gtrnuroaha.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.jianghu66.top/gtmqrkqljl.html

[Q36] 左连接
来源：http://hz.jlsjyb.cn/gtqjjlymmm.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.haohaochexian.top/gtbaolxthq.html

[Q37] 右连接
来源：http://hz.hongshengwenyu.top/gtxslkpcme.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.chenlongwang.top/gtbhoxcdux.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.jianghu66.top/gteesjjxwl.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.xziqi.cn/gtnawfjjbp.html

[Q39] 自连接（查上下级）
来源：http://hz.nwbrower.top/gtuwtucqsq.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.xziqi.cn/gtyhfnwjky.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.ivvv.top/gtivgazcsi.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.pycfn.com/gtzxxxtanp.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.iojbl.cn/gtpbixhhla.html

[Q41] 多表连接
来源：http://hz.yonumen.top/gtwmtitppm.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.shanyushiyangtech.top/gtsjwegtex.html

JOIN users u ON u.id = o.user_id
来源：http://hz.meibo888.top/gtuuqcokfu.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.birdmap.top/gtqyovyqem.html

[Q42] 连接条件附加过滤
来源：http://hz.fzhhl.top/gtxhisugbh.html

SELECT u.name, o.amount FROM users u
来源：http://hz.hammf.cn/gtrmcyoewo.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.ydjk.org.cn/gtvcroiboe.html

[Q43] 标量子查询
来源：http://hz.andypj.xyz/gtcadxillj.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.aibaodan.cn/gtsckaukgm.html

[Q44] IN 子查询
来源：http://hz.zhaomingkeji.xyz/gtblukubba.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.jinqigfzy.top/gtqrpvjjgk.html

[Q45] EXISTS 判断存在
来源：http://hz.jinyuanbaomall.cn/gtfwyeywfo.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.mhx1999.top/gtztcubtbj.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.hnqzz.top/gtgunjlndr.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.ehwqpu.com/gtwnkvcafp.html

[Q47] 与平均值比较
来源：http://hz.feifeiyinyue.top/gtxlrbfiyd.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.andypj.xyz/gtoeftblyr.html

[Q48] CTE 公用表表达式
来源：http://hz.ydzc1.top/gttkbpysdi.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.cdnleiting.top/gtvryokdlr.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.ybcxt.top/gtevuwqbgk.html

[Q49] 更新单行
来源：http://hz.gotoacloud.top/gtyvdkvblu.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.zhoulong.xyz/gtdffbipxw.html

[Q50] 批量更新
来源：http://hz.zhixingplan.top/gtxzhsohye.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.daria6918.cn/gtuihduede.html

[Q51] 用子查询更新
来源：http://hz.daxiang520.top/gtumhhewqt.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.nwbrower.top/gtyigbyodc.html

[Q52] 删除指定行
来源：http://hz.ivvv.top/gthpocbqyt.html

DELETE FROM users WHERE id = 10;
来源：http://hz.yvedp.cn/gtgukgxpoe.html

[Q53] 按条件删除
来源：http://hz.tanke756.top/gtbiuxevqe.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.cheryme.top/gtljgeblxq.html

[Q54] 清空表
来源：http://hz.sysykeji.top/gtelzwbxmp.html

TRUNCATE TABLE logs;
来源：http://hz.xuetiantiany.cn/gtjzqgskey.html

[Q55] 排名（并列占位）
来源：http://hz.ywan-chungtsiang.top/gtipkrocjo.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.0kj1m.cn/gtmnhmpozq.html

[Q56] 密集排名（并列不占位）
来源：http://hz.birdmap.top/gtheemtctp.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.cqqwz.cn/gtyrcyffle.html

[Q57] 行号
来源：http://hz.shanyushiyangkeji.top/gtqirpygtz.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.xuetiantiany.cn/gtajpwdqhy.html

[Q58] 累计求和
来源：http://hz.cucudq.cn/gtefbrjkuf.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.zhaomingkeji.xyz/gtssqxkgqf.html

[Q59] 分组内累计
来源：http://hz.0kj1m.cn/gtlveqqpox.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.hfpthk.cn/gtomksdrwz.html

[Q60] 取上一行 / 下一行
来源：http://hz.zdqjudy.top/gtveojqbzh.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.yj20258888.top/gtiyghurmc.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.shanyushiyangkeji.top/gtagvurnqd.html

[Q61] 移动平均
来源：http://hz.jinghuilouyu.cn/gteyqdtopx.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.vqdsnc.cn/gtcpposwdp.html

[Q62] 分组占比
来源：http://hz.52xcode.cn/gtndfmgzkn.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.guannengcc.top/gtxfvrppjm.html

[Q63] 开启事务
来源：http://hz.wangdashe.top/gtuusjjhtq.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.hfpthk.cn/gtxhejaqaq.html

[Q64] 提交事务
来源：http://hz.yj20258.top/gtsuchmykx.html

COMMIT;
来源：http://hz.316326.xyz/gtzlmzysge.html

[Q65] 回滚事务
来源：http://hz.jiagoushi.top/gtndevatfp.html

ROLLBACK;
来源：http://hz.yueranfly.top/gtspyfbyqb.html

[Q66] 行锁查询
来源：http://hz.jianghu66.top/gtsijfovzv.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.shzxlz.cn/gttzqtbjoo.html

[Q67] 设置隔离级别
来源：http://hz.andypj.xyz/gthqryymbi.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.cqqwz.cn/gtdrmfefmy.html

[Q68] 保存点
来源：http://hz.chenjidiqi.icu/gtmwyrrika.html

SAVEPOINT sp1;
来源：http://hz.zhixingplan.top/gtajomdxxz.html

ROLLBACK TO sp1;
来源：http://hz.dashuyun.cn/gthfbnmjkp.html

[Q69] 查看执行计划
来源：http://hz.dianchejie.cn/gtaqsfuwvi.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.vqdsnc.cn/gtvxvharbr.html

[Q70] 更新统计信息
来源：http://hz.jinqigufen.top/gtplonscmx.html

ANALYZE TABLE users;
来源：http://hz.shangyingyoupin.top/gtxocscbof.html

[Q71] 查看建表语句
来源：http://hz.tian-w.cn/gtgnwptnpm.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.wangdashe.top/gttoqtupqz.html

[Q72] 查看索引
来源：http://hz.redwolf501.top/gtsfumznek.html

SHOW INDEX FROM users;
来源：http://hz.hongshengwenyu.top/gtbmamsgtk.html

[Q73] 查看表状态
来源：http://hz.vqdsnc.cn/gtoybagfgf.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.jinghuilouyu.cn/gtqhxitsrp.html

[Q74] 强制使用索引
来源：http://hz.cdnleiting.top/gtgjkgrhas.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.yuanzhike.top/gtcctuvfrw.html

[Q75] 日期格式化
来源：http://hz.daria6918.cn/gtsuhvsanf.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.iojbl.cn/gtuzqoiztv.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.ehwqpu.com/gtoeckhvgq.html

[Q76] 按天统计
来源：http://hz.xylfe.cn/gtegzhxgwe.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.hnxiangtu.top/gtsmwwbriy.html

[Q77] 时间加减
来源：http://hz.snrcjt.cn/gtclfvrmyv.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.vqdsnc.cn/gtpxgkloir.html

[Q78] 当前时间
来源：http://hz.hammf.cn/gtmggleptm.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.shuidangran.top/gtuezbrnxb.html

[Q79] 字符串拼接
来源：http://hz.feifeiyinyue.top/gtfeesjgqu.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.xinyue.icu/gtrylrnidx.html

[Q80] 字符串截取
来源：http://hz.xylfe.cn/gtfpoahwcd.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.hfpthk.cn/gtnptlseax.html

[Q81] 字符串替换
来源：http://hz.gzhubu.top/gttjwngpoq.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.jinqigfzy.top/gtlxmanvnu.html

[Q82] 字符长度与字节长度
来源：http://hz.gotoacloud.top/gtprzwxhzj.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.fengsongda.top/gtszjxznyd.html

[Q83] 大小写转换
来源：http://hz.shangyingyoupin.top/gtogxklecx.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.tanke756.top/gtpoicdhpn.html

[Q84] 去除首尾空格
来源：http://hz.meibo888.top/gtishgstzt.html

SELECT TRIM(name) FROM users;
来源：http://hz.gogol.net.cn/gttujvgikd.html

[Q85] 数值取整
来源：http://hz.hywenlv.cn/gtppbrjlcs.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.nwbrower.top/gtqfmoyzgr.html

[Q86] 读取 JSON 字段
来源：http://hz.hammf.cn/gttymrhtfx.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.wangdashe.top/gtddzsgcab.html

[Q87] JSON 字段做条件
来源：http://hz.ppjwa.cn/gthndtjxti.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.shangyingyoupin.top/gtyiiisxur.html

[Q88] 行转列（条件聚合）
来源：http://hz.jiagoushi.top/gtpiipehhr.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.tanke756.top/gtryizbvho.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.ydzc1.top/gtkkivzejy.html

[Q89] 判断表是否存在
来源：http://hz.vqdsnc.cn/gtczctizlw.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.sweek.top/gtchfblogi.html

[Q90] 生成序号列
来源：http://hz.ivvv.top/gtwgdjvuug.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.aizwys.cn/gtyxantxrp.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtphutxcbt.html

R. Bash 专题
来源：http://hz.shanyushiyangtech.top/gtizzdrfur.html

================================================================================
来源：http://hz.shzxlz.cn/gtzuwcaeqq.html

[R01] shebang 与严格模式
来源：http://hz.gotoacloud.top/gtvuspxrpl.html

#!/usr/bin/env bash
来源：http://hz.tian-w.cn/gterucxhmq.html

set -euo pipefail
来源：http://hz.xuetiantiany.cn/gtgdirodzm.html

[R02] 变量赋值与使用
来源：http://hz.gzhubu.top/gtkmpsrqcb.html

name="Tom"; echo "$name"
来源：http://hz.yueranfly.top/gtrvyibcbh.html

[R03] 只读变量
来源：http://hz.birdmap.top/gtpesczebe.html

readonly PI=3.14
来源：http://hz.haohaochexian.top/gtxdqxgsym.html

[R04] 位置参数
来源：http://hz.nanxinkj.top/gtkgrkmyef.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.yj202588.top/gtdafrikio.html

[R05] 参数默认值
来源：http://hz.cheryme.top/gtwmpmhznw.html

name="${1:-default}"
来源：http://hz.hammf.cn/gtmiakdeso.html

[R06] 判断命令是否存在
来源：http://hz.yueranfly.top/gthivrrzpd.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.yj20258.top/gtcymglmka.html

[R07] if 判断文件
来源：http://hz.cheryme.top/gtjtrlhvyd.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.guannengcc.top/gtwxdltuvi.html

[R08] 数值比较
来源：http://hz.yvedp.cn/gtsoqvrbly.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.chenzaomai.com/gtluxxhfir.html

[R09] 字符串比较
来源：http://hz.fzhhl.top/gtwzbkbseh.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.cheryme.top/gtzfsftkec.html

[R10] 正则匹配
来源：http://hz.fzhhl.top/gtauaehryu.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.316326.xyz/gtwrnglgrv.html

[R11] case 多分支
来源：http://hz.jinghuilouyu.cn/gtgfqwshtp.html

case "$1" in
来源：http://hz.guannengcc.top/gtyhqtxwwt.html

start) echo "启动" ;;
来源：http://hz.dashuyun.cn/gtangdawgr.html

stop)  echo "停止" ;;
来源：http://hz.sysykeji.top/gtnzwfiojj.html

*)     echo "未知命令" ;;
来源：http://hz.guannengcc.top/gtfoeqalcu.html

esac
来源：http://hz.vqdsnc.cn/gttvesglmi.html

[R12] for 遍历文件
来源：http://hz.fengsongda.top/gtfkuwgbcl.html

for f in *.txt; do echo "$f"; done
来源：http://hz.ybcxt.top/gtltbzxerc.html

[R13] for 计数循环
来源：http://hz.shanyushiyangkeji.top/gtxpiwadqq.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.jqgfzy.top/gtpbvdtitu.html

[R14] C 风格 for
来源：http://hz.hywenlv.cn/gtadhvtjzv.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.wangshuangyany.cn/gtluqgmzzo.html

[R15] while 逐行读文件
来源：http://hz.snrcjt.cn/gtfdjxfhwe.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.pycfn.com/gtlskobtqe.html

[R16] until 等待条件
来源：http://hz.xuanzx.com/gtamjsixcv.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.daxiang520.top/gtemnjlstz.html

[R17] 数组定义与取值
来源：http://hz.xinyue.icu/gtscenswtv.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.316326.xyz/gtdgsbrvqr.html

[R18] 遍历数组
来源：http://hz.birdmap.top/gtqlqtxbkx.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.hnqzz.top/gtkykqlvex.html

[R19] 数组长度
来源：http://hz.wangshuangyany.cn/gtgpkfvqpp.html

echo "${#arr[@]}"
来源：http://hz.shanyushiyangkeji.top/gtsitsqbdo.html

[R20] 关联数组（字典）
来源：http://hz.hnxiangtu.top/gtphvljrkt.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.zdqjudy.top/gtjbeeorzj.html

[R21] 字符串长度
来源：http://hz.nanxuanxn.top/gtzkgqwagg.html

echo "${#s}"
来源：http://hz.zycfv.cn/gtttrowtsd.html

[R22] 截取子串
来源：http://hz.cdnleiting.top/gtuidamgpw.html

echo "${s:0:5}"
来源：http://hz.zdqjudy.top/gtfkiumkqd.html

[R23] 字符串替换
来源：http://hz.gaohongyu789.top/gtgcwnnpth.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.pycfn.com/gtxojiduzi.html

[R24] 大小写转换
来源：http://hz.zdqjudy.top/gtbyycbsrb.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.shuidangran.top/gtrkrdqzyh.html

[R25] 去后缀 / 去前缀
来源：http://hz.xziqi.cn/gtxibfexbb.html


<!-- 参考信息 -->