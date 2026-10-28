代发 wailian999

[P05] 判断两个对象内容是否相等
来源：http://hz.9152youxi.cn/gtkhvoeuhu.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.guannengcc.top/gtudthhxgv.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.sxryk.cn/gtpphuasil.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.fzhhl.top/gtuqhlycoa.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.ppjwa.cn/gtdjwqpota.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.jqgfzy.top/gtrgeowwfz.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.daria6918.cn/gtegtfjslx.html

Ruby: a == b
来源：http://hz.yuxming.cn/gtbgkymenw.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.shzxlz.cn/gtvsbqclud.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.meibo888.top/gtlibexipu.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.ydzc1.top/gtlrgceiig.html

PHP:  if (empty($x)) {}
来源：http://hz.hywenlv.cn/gtqakvsfxl.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.shuidangran.top/gtnjbmmeun.html

TS:   if (x == null) {}
来源：http://hz.jqgfzy.top/gtzwarlpza.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.yj20258888.top/gtpsynrcdn.html

Go:   if x == nil {}
来源：http://hz.zhongyouzk.top/gthjoyhuuy.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.yonumen.top/gtylaizuuf.html

C#:   if (x is null) {}
来源：http://hz.hongshengwenyu.top/gtueqcehxd.html

[P07] 防抖与节流
来源：http://hz.zhoulong.xyz/gtghktwcac.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.jinqigufen.top/gtbqqqsrmq.html

PHP:  // 手写时间戳比较
来源：http://hz.fzhhl.top/gtrxwxkwez.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.tianlin.xyz/gtljwyhspu.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.xingfuxueyuan.xyz/gthpaabpoa.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.shzxlz.cn/gteghditjq.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.yangfankeji.com/gtvxbdqste.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.52xcode.cn/gtwfnuyxri.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.yj20258.top/gtnbootatv.html

[P08] 处理浮点精度问题
来源：http://hz.dashuyun.cn/gtncuuhzwh.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.ehwqpu.com/gtdlnucqlj.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.52xcode.cn/gttgupwbde.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.daria6918.cn/gtztysbhwb.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.sufxvd.cn/gtdrncqehl.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.shuidangran.top/gtdjeldukv.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.shangyingyoupin.top/gtxdimmcss.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.nanxinkj.top/gtdtokiyun.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.chenzaomai.com/gttxsamekf.html

================================================================================
来源：http://hz.jqgfzy.top/gtsgaxsmxs.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.ehwqpu.com/gtlssfmyme.html

================================================================================
来源：http://hz.jqgfzy.top/gtneiuajvo.html

[Q01] 创建表
来源：http://hz.ybcxt.top/gtaehxonmt.html

CREATE TABLE users (
来源：http://hz.pycfn.com/gtbmshxgmh.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.52xcode.cn/gtgkszldwv.html

name VARCHAR(50) NOT NULL,
来源：http://hz.hammf.cn/gtivyxzxhv.html

email VARCHAR(100) UNIQUE,
来源：http://hz.ydzc1.top/gtmixsazny.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.shzxlz.cn/gthqukrlfx.html

);
来源：http://hz.jqgufenzy.top/gtaairmvyk.html

[Q02] 创建带外键的表
来源：http://hz.dashuyun.cn/gtolegacnd.html

CREATE TABLE orders (
来源：http://hz.vqdsnc.cn/gtlxdbygxj.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.shanyushiyangtech.top/gtxzwvjghb.html

user_id INT NOT NULL,
来源：http://hz.gzhubu.top/gtsliqoxiw.html

amount DECIMAL(10, 2),
来源：http://hz.gzhubu.top/gtkoomygfi.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.mhx1999.top/gtfwwijplj.html

);
来源：http://hz.xinyue.icu/gtmqxgkonw.html

[Q03] 增加列
来源：http://hz.shanyushiyangkeji.top/gtlygbujfd.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.xylfe.cn/gtuysbddjv.html

[Q04] 修改列类型
来源：http://hz.nwbrower.top/gtcyhwhwmp.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.fzhhl.top/gtcnjlefqq.html

[Q05] 重命名列
来源：http://hz.cqqwz.cn/gtrozjwgxl.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.cqqwz.cn/gtzqlhbjal.html

[Q06] 删除列
来源：http://hz.zhijiandao.cn/gtmzgslymo.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.zhixingplan.top/gtikkyrhxr.html

[Q07] 删除表
来源：http://hz.ybcxt.top/gtqphfisdh.html

DROP TABLE IF EXISTS orders;
来源：http://hz.sweek.top/gtpdttqfoi.html

[Q08] 创建普通索引
来源：http://hz.zhijiandao.cn/gtysgbtaep.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.yangfankeji.com/gtxlwsroqj.html

[Q09] 创建唯一索引
来源：http://hz.kuanghao11.cn/gtvhihuhhq.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.c1oappe.top/gtqjybmrtc.html

[Q10] 插入单行
来源：http://hz.yanxiufei.cn/gtqpqfwoxe.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.yongpay.top/gttdwshixz.html

[Q11] 一次插入多行
来源：http://hz.zhijiandao.cn/gtstukkhow.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.zhijiandao.cn/gtpgslklix.html

[Q12] 插入后取自增 ID
来源：http://hz.aibaodan.cn/gtvquzsbuu.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.aizwys.cn/gtrszdxaye.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.yueranfly.top/gtkltxqlva.html

[Q13] 忽略重复插入
来源：http://hz.nanxinkj.top/gtplkjmqrd.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.chenjidiqi.icu/gtynhgckqa.html

[Q14] 存在则更新（upsert）
来源：http://hz.nanxuanxn.top/gtryzkqdgh.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.yvedp.cn/gtqtuovcuz.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.jyoumei.cn/gtnijseaoc.html

[Q15] 查询全部
来源：http://hz.haohaochexian.top/gtdjthaoee.html

SELECT * FROM users;
来源：http://hz.chenzaomai.com/gtjfpgehgb.html

[Q16] 查询指定列
来源：http://hz.hywenlv.cn/gtiwzfagll.html

SELECT id, name FROM users;
来源：http://hz.jiagoushi.top/gtoxzlffeo.html

[Q17] 条件查询
来源：http://hz.jinyuanbaomall.cn/gtykjcnjbu.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.nanxinkj.top/gtltewzwoy.html

[Q18] 模糊匹配
来源：http://hz.zhengqikj.top/gtrjvyrsqb.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.pycfn.com/gtxhdemzlx.html

[Q19] 范围查询
来源：http://hz.jinqigufen.top/gtovcuaroa.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.birdmap.top/gtxzdzbdip.html

[Q20] IN 列表
来源：http://hz.52xcode.cn/gtujkwzfol.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.nwbrower.top/gtgqqzzzhg.html

[Q21] 空值判断
来源：http://hz.jianghu66.top/gtuxmgevmc.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.tian-w.cn/gtfunlphza.html

[Q22] 排序
来源：http://hz.yj20258.top/gtwmuvlnfg.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.wangshuangyany.cn/gtzeililqj.html

[Q23] 分页
来源：http://hz.fengsongda.top/gtnrtiuzhs.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.xingfuxueyuan.xyz/gtynkshwxn.html

[Q24] 去重
来源：http://hz.zdqjudy.top/gtwkvyucgj.html

SELECT DISTINCT city FROM users;
来源：http://hz.sweek.top/gtiailffof.html

[Q25] 只取前 N 条
来源：http://hz.feifeiyinyue.top/gtcqayxapn.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.aizwys.cn/gtvakojkpe.html

[Q26] 计数
来源：http://hz.gzhubu.top/gtzwtrtgzt.html

SELECT COUNT(*) FROM users;
来源：http://hz.yonumen.top/gtcwvuaajb.html

[Q27] 条件计数
来源：http://hz.nwbrower.top/gtoozdifco.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.daxiang520.top/gtkpnximzj.html

[Q28] 求和与平均
来源：http://hz.xziqi.cn/gtlwkhfyzu.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.hnxiangtu.top/gtpklcafro.html

[Q29] 最大最小值
来源：http://hz.zhaomingkeji.xyz/gtfwqzivep.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.kuanghao11.cn/gtlttahhqb.html

[Q30] 分组统计
来源：http://hz.jyoumei.cn/gtclsccdda.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.52xcode.cn/gtpfyplrnu.html

[Q31] 分组后过滤
来源：http://hz.cdnleiting.top/gtmeiktvzl.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.52xcode.cn/gtzetodjbr.html

[Q32] 分组拼接字符串
来源：http://hz.yongpay.top/gtzmiassst.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.sxryk.cn/gtveoeqpqm.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.sufxvd.cn/gtjpgprfln.html

[Q33] 多列分组
来源：http://hz.zhixingplan.top/gtfkibggdb.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.dianchejie.cn/gthxznnack.html

[Q34] 每组取第一条
来源：http://hz.nwbrower.top/gtodkfqedy.html

SELECT * FROM (
来源：http://hz.shuidangran.top/gtnhktmlhs.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.havefunace.top/gtjpkqcosh.html

) t WHERE rn = 1;
来源：http://hz.haohaochexian.top/gtdvoxkkmv.html

[Q35] 内连接
来源：http://hz.guannengcc.top/gtjyjmlgsk.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.aizwys.cn/gttfjgesio.html

[Q36] 左连接
来源：http://hz.tian-w.cn/gtfxqjmnpw.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.yanxiufei.cn/gtzgwxznau.html

[Q37] 右连接
来源：http://hz.jiagoushi.top/gtmhbvapbj.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.pengpengdd.cyou/gtexpzobll.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.wangdashe.top/gtixgpzffe.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.wangshuangyany.cn/gtuwulhpyv.html

[Q39] 自连接（查上下级）
来源：http://hz.jqgufenzy.top/gtovrgygvp.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.ydzc1.top/gtvbiqegiu.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.snrcjt.cn/gtbiioawba.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.cashguo.top/gtwoxhnipu.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.nwbrower.top/gtqougqgnm.html

[Q41] 多表连接
来源：http://hz.smart0.xyz/gtvpxvausz.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.yanxiufei.cn/gtszfhcvns.html

JOIN users u ON u.id = o.user_id
来源：http://hz.ybcxt.top/gtyymtuumf.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.sufxvd.cn/gtzdrqpfmg.html

[Q42] 连接条件附加过滤
来源：http://hz.jinqigfzy.top/gtqnhbffhi.html

SELECT u.name, o.amount FROM users u
来源：http://hz.ydzc1.top/gtxkfpuerq.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.jinqigfzy.top/gtafjibkpk.html

[Q43] 标量子查询
来源：http://hz.ydzc1.top/gtfzwufdtx.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.kuanghao11.cn/gtyucwqlsr.html

[Q44] IN 子查询
来源：http://hz.hnxiangtu.top/gtmnaawucn.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.quarkkingdee.top/gtfxsziqft.html

[Q45] EXISTS 判断存在
来源：http://hz.tian-w.cn/gtpbvnzgmf.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.dashuyun.cn/gtnxdgtjmg.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.havefunace.top/gtvcuyuaja.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.9152youxi.cn/gtycozdqgl.html

[Q47] 与平均值比较
来源：http://hz.sufxvd.cn/gtqaoopfjj.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.mhx1999.top/gtjriljmty.html

[Q48] CTE 公用表表达式
来源：http://hz.ybcxt.top/gtgnfcnqbb.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.0kj1m.cn/gtlmqmtjku.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.yueranfly.top/gtymlqtmly.html

[Q49] 更新单行
来源：http://hz.cheryme.top/gtornqxktj.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.dianchejie.cn/gtjmqzdvia.html

[Q50] 批量更新
来源：http://hz.cucudq.cn/gtzoulxerm.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.yuanzhike.top/gtgudgbetk.html

[Q51] 用子查询更新
来源：http://hz.guowangkeji.top/gtkyteutdv.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.yueranfly.top/gtpimyvtof.html

[Q52] 删除指定行
来源：http://hz.yuanzhike.top/gtwbafehkm.html

DELETE FROM users WHERE id = 10;
来源：http://hz.ppjwa.cn/gtyeqjqtox.html

[Q53] 按条件删除
来源：http://hz.zhaomingkeji.xyz/gttoberqjk.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.bjfxy.top/gttkldenbp.html

[Q54] 清空表
来源：http://hz.ppjwa.cn/gtpevsbjue.html

TRUNCATE TABLE logs;
来源：http://hz.aizwys.cn/gtuswvsotz.html

[Q55] 排名（并列占位）
来源：http://hz.yonumen.top/gtbeyjynlx.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.andypj.xyz/gtvbcisqkr.html

[Q56] 密集排名（并列不占位）
来源：http://hz.xylfe.cn/gtbiwmuthq.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.xylfe.cn/gtmnkqxmwk.html

[Q57] 行号
来源：http://hz.shanyushiyangkeji.top/gtpuepxlvw.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.wangshuangyany.cn/gtmzbxpgzq.html

[Q58] 累计求和
来源：http://hz.yj20258.top/gtwerfcxsk.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.xuetiantiany.cn/gtryvfneww.html

[Q59] 分组内累计
来源：http://hz.hongshengwenyu.top/gtkkzovrnn.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.tanke756.top/gtpibgyqgg.html

[Q60] 取上一行 / 下一行
来源：http://hz.birdmap.top/gtjxsmfdmq.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.jqgfzy.top/gtqgrfgzau.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.hongshengwenyu.top/gtssczmqsv.html

[Q61] 移动平均
来源：http://hz.gaohongyu789.top/gtqsedjapi.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.zhiwuduotai.top/gtpvvsvisd.html

[Q62] 分组占比
来源：http://hz.cashguo.top/gteqvkymdd.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.jinqigufen.top/gtolwnoity.html

[Q63] 开启事务
来源：http://hz.yj20258888.top/gtmngzcvhz.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.pycfn.com/gtdiailosf.html

[Q64] 提交事务
来源：http://hz.hysaishi.cn/gtpvrvdvlf.html

COMMIT;
来源：http://hz.yueranfly.top/gticfwwdqk.html

[Q65] 回滚事务
来源：http://hz.nanxuanxn.top/gtqvydpjzh.html

ROLLBACK;
来源：http://hz.jqgfzy.top/gtxwxeaipl.html

[Q66] 行锁查询
来源：http://hz.hongshengwenyu.top/gtotppwhoz.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.jinqigufen.top/gtnwiibmxh.html

[Q67] 设置隔离级别
来源：http://hz.jinqigfzy.top/gthrpukjat.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.nanxinkj.top/gtavuiknlm.html

[Q68] 保存点
来源：http://hz.xinyue.icu/gtoqjdpidu.html

SAVEPOINT sp1;
来源：http://hz.jinqigfzy.top/gtcvrceymn.html

ROLLBACK TO sp1;
来源：http://hz.jianghu66.top/gtiqwqcrxl.html

[Q69] 查看执行计划
来源：http://hz.jinqigufen.top/gtfymkkxse.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.tian-w.cn/gtnqwrpvyl.html

[Q70] 更新统计信息
来源：http://hz.ydzc1.top/gtdffkvids.html

ANALYZE TABLE users;
来源：http://hz.quarkkingdee.top/gteaihmpjw.html

[Q71] 查看建表语句
来源：http://hz.ydzc1.top/gtsfvmngmc.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.kuanghao11.cn/gtxlyhrgjj.html

[Q72] 查看索引
来源：http://hz.iojbl.cn/gtfsmwvybb.html

SHOW INDEX FROM users;
来源：http://hz.feifeiyinyue.top/gtrczrtpxk.html

[Q73] 查看表状态
来源：http://hz.daria6918.cn/gtcnhzursw.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.jyoumei.cn/gtnmrsmivd.html

[Q74] 强制使用索引
来源：http://hz.sweek.top/gtpeeudtfw.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.dianchejie.cn/gtoqztpsdk.html

[Q75] 日期格式化
来源：http://hz.bjfxy.top/gtnwzvsvnn.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.bjfxy.top/gtujyyigdg.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.pycfn.com/gtnffurwci.html

[Q76] 按天统计
来源：http://hz.tianlin.xyz/gtpcpzzgac.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.bjfxy.top/gtxvoievyt.html

[Q77] 时间加减
来源：http://hz.daxiang520.top/gtgfrwrnmz.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.yanxiufei.cn/gtfxocjhtj.html

[Q78] 当前时间
来源：http://hz.snrcjt.cn/gtyumzfike.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.birdmap.top/gtmwkilsam.html

[Q79] 字符串拼接
来源：http://hz.zhaomingkeji.xyz/gtkoxrymng.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.chenjidiqi.icu/gtlbdjfshe.html

[Q80] 字符串截取
来源：http://hz.guowangkeji.top/gtwuhdsdhj.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.aibaodan.cn/gtlruthywk.html

[Q81] 字符串替换
来源：http://hz.zhoulong.xyz/gtqosiiylu.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.c1oappe.top/gthkqwgrpq.html

[Q82] 字符长度与字节长度
来源：http://hz.feifeiyinyue.top/gtwzbnuawt.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.nanxuanxn.top/gtqpqfomut.html

[Q83] 大小写转换
来源：http://hz.kuanghao11.cn/gtgbaitchk.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.quarkkingdee.top/gtekpeslkx.html

[Q84] 去除首尾空格
来源：http://hz.birdmap.top/gttgbvshav.html

SELECT TRIM(name) FROM users;
来源：http://hz.jinyuanbaomall.cn/gtuopwesru.html

[Q85] 数值取整
来源：http://hz.ywan-chungtsiang.top/gtneznprio.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.jqgfzy.top/gtckroyenn.html

[Q86] 读取 JSON 字段
来源：http://hz.yanxiufei.cn/gtfytsusah.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.quarkkingdee.top/gtkeukmqny.html

[Q87] JSON 字段做条件
来源：http://hz.zhijiandao.cn/gtzouqwudq.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.hysaishi.cn/gtkppimsls.html

[Q88] 行转列（条件聚合）
来源：http://hz.dashuyun.cn/gtcynsfenf.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.yvedp.cn/gtfpwrmzcx.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.nwbrower.top/gtdfrxcfqb.html

[Q89] 判断表是否存在
来源：http://hz.nanxuanxn.top/gtzbutktpz.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.quarkkingdee.top/gtvlnncnby.html

[Q90] 生成序号列
来源：http://hz.redwolf501.top/gtiweczchr.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.havefunace.top/gttwmasvsg.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtwukbramj.html

R. Bash 专题
来源：http://hz.hysaishi.cn/gtpalpvkcf.html

================================================================================
来源：http://hz.ydzc1.top/gtpckxhjsq.html

[R01] shebang 与严格模式
来源：http://hz.nanxinkj.top/gtkmomqkbh.html

#!/usr/bin/env bash
来源：http://hz.aibaodan.cn/gtzmrdihdp.html

set -euo pipefail
来源：http://hz.jinyuanbaomall.cn/gtiytazidm.html

[R02] 变量赋值与使用
来源：http://hz.gzhubu.top/gtxccmisdg.html

name="Tom"; echo "$name"
来源：http://hz.shangyingyoupin.top/gtlwmqakds.html

[R03] 只读变量
来源：http://hz.fzhhl.top/gtzivcnhll.html

readonly PI=3.14
来源：http://hz.shangyingyoupin.top/gtwbsblgmz.html

[R04] 位置参数
来源：http://hz.zhijiandao.cn/gtsiumacum.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.havefunace.top/gthjlgeath.html

[R05] 参数默认值
来源：http://hz.jinyuanbaomall.cn/gtzgknizxd.html

name="${1:-default}"
来源：http://hz.tianlin.xyz/gtonqawpjh.html

[R06] 判断命令是否存在
来源：http://hz.andypj.xyz/gttlfitxuo.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.hywenlv.cn/gtryifnxsv.html

[R07] if 判断文件
来源：http://hz.mhx1999.top/gtsmthjjpt.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.hywenlv.cn/gtdjrzgzxy.html

[R08] 数值比较
来源：http://hz.ydjk.org.cn/gttaxyoxww.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.sweek.top/gttrabeusd.html

[R09] 字符串比较
来源：http://hz.ppjwa.cn/gttkbiinil.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.chenjidiqi.icu/gteqpempkw.html

[R10] 正则匹配
来源：http://hz.52xcode.cn/gtyuxbwgpg.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.pengpengdd.cyou/gtrhshzrhj.html

[R11] case 多分支
来源：http://hz.pycfn.com/gtrvecxcue.html

case "$1" in
来源：http://hz.shanyushiyangkeji.top/gtjvdnkung.html

start) echo "启动" ;;
来源：http://hz.daxiang520.top/gtjlwtrfyu.html

stop)  echo "停止" ;;
来源：http://hz.hfpthk.cn/gtdvfpajnl.html

*)     echo "未知命令" ;;
来源：http://hz.hammf.cn/gtrsggjsqs.html

esac
来源：http://hz.quarkkingdee.top/gtnmhenfxe.html

[R12] for 遍历文件
来源：http://hz.meibo888.top/gtrvcgbjtk.html

for f in *.txt; do echo "$f"; done
来源：http://hz.cashguo.top/gtivgoglxg.html

[R13] for 计数循环
来源：http://hz.hongshengwenyu.top/gtyofgnjqw.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.tanke756.top/gtlllbxzux.html

[R14] C 风格 for
来源：http://hz.dianchejie.cn/gtgubeulsr.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.hywenlv.cn/gtbrtytlop.html

[R15] while 逐行读文件
来源：http://hz.zycfv.cn/gtxzssuqmx.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.chenjidiqi.icu/gtektbsgta.html

[R16] until 等待条件
来源：http://hz.daxiang520.top/gtepwoinwt.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.andypj.xyz/gtjsbscdkm.html

[R17] 数组定义与取值
来源：http://hz.yueranfly.top/gtfjufkkya.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.gaohongyu789.top/gtqwaywojf.html

[R18] 遍历数组
来源：http://hz.ybcxt.top/gtbimtqiln.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.jyoumei.cn/gtwegycjzm.html

[R19] 数组长度
来源：http://hz.jyoumei.cn/gtpetnxlxm.html

echo "${#arr[@]}"
来源：http://hz.shanyushiyangtech.top/gtwnpcoabr.html

[R20] 关联数组（字典）
来源：http://hz.guannengcc.top/gtoaswnkqc.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.xinyue.icu/gtoamislkg.html

[R21] 字符串长度
来源：http://hz.daria6918.cn/gtoytfianb.html

echo "${#s}"
来源：http://hz.aibaodan.cn/gtgiyxktjz.html

[R22] 截取子串
来源：http://hz.9152youxi.cn/gtfbuxhpys.html

echo "${s:0:5}"
来源：http://hz.birdmap.top/gtxoqfkceh.html

[R23] 字符串替换
来源：http://hz.chenlongwang.top/gtfcruzvxa.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.jinqigfzy.top/gtbceuybqh.html

[R24] 大小写转换
来源：http://hz.ehwqpu.com/gtjcbyzbqz.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.yonumen.top/gtqwomtitz.html

[R25] 去后缀 / 去前缀
来源：http://hz.316326.xyz/gtmvkwvghf.html


<!-- 参考信息 -->