代发 wailian999

[P05] 判断两个对象内容是否相等
来源：http://hz.chenzaomai.com/gtaldjaejp.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.hywenlv.cn/gtnbhzhvct.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.ydjk.org.cn/gtfodbrqap.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.smart0.xyz/gtypbkqohy.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.nwbrower.top/gtsqlfpxxz.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.sxryk.cn/gtydhakzdp.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.shanyushiyangtech.top/gtmjypkpjz.html

Ruby: a == b
来源：http://hz.yuanzhike.top/gtzixjibvg.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.ehwqpu.com/gtmjzytvbv.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.chenzaomai.com/gtupyiisma.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.vqdsnc.cn/gthmumkarz.html

PHP:  if (empty($x)) {}
来源：http://hz.bjfxy.top/gtjhhrevlf.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.pengpengdd.cyou/gtwnypievx.html

TS:   if (x == null) {}
来源：http://hz.hongshengwenyu.top/gtrhbuqghx.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.zhijiandao.cn/gtnfezuhqy.html

Go:   if x == nil {}
来源：http://hz.shuidangran.top/gtknwgizsc.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.chenzaomai.com/gtdfiidudp.html

C#:   if (x is null) {}
来源：http://hz.jiagoushi.top/gtylnqydlp.html

[P07] 防抖与节流
来源：http://hz.gaohongyu789.top/gtwjdpbfym.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.wangdashe.top/gtyrydgtqr.html

PHP:  // 手写时间戳比较
来源：http://hz.cheryme.top/gtyfmugstw.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.chenzaomai.com/gtjckctdvr.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.chenlongwang.top/gtpdzvphpt.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.dashuyun.cn/gtmyudxytp.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.316326.xyz/gtotfddtxj.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.shzxlz.cn/gtwevcibok.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.zhixingplan.top/gtjliahkoh.html

[P08] 处理浮点精度问题
来源：http://hz.iojbl.cn/gteegozawp.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.zhijiandao.cn/gtmcptpesm.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.yueranfly.top/gtnplwqwld.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.xuanzx.com/gtwtpextom.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.yuxming.cn/gtqklhxetn.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.jqgfzy.top/gtyhuactjk.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.zhaomingkeji.xyz/gtpknairpi.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.zhongyouzk.top/gtttpcmenq.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.ehwqpu.com/gttjzqdhmq.html

================================================================================
来源：http://hz.zhengqikj.top/gtpthtzrif.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.fzhhl.top/gtafpifelq.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtmvwmkelv.html

[Q01] 创建表
来源：http://hz.ivvv.top/gtmvqfjyje.html

CREATE TABLE users (
来源：http://hz.chenlongwang.top/gtelawafie.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.52xcode.cn/gtuqgaeniq.html

name VARCHAR(50) NOT NULL,
来源：http://hz.jinqigufen.top/gtcwxescsi.html

email VARCHAR(100) UNIQUE,
来源：http://hz.guannengcc.top/gtwjfeobpu.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.nanxuanxn.top/gtitjqoqdv.html

);
来源：http://hz.xinyue.icu/gtnsdkxezg.html

[Q02] 创建带外键的表
来源：http://hz.tianlin.xyz/gtejycfuqy.html

CREATE TABLE orders (
来源：http://hz.xinyue.icu/gtbfigxnyq.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.cashguo.top/gtiqllfrss.html

user_id INT NOT NULL,
来源：http://hz.tian-w.cn/gtlldrntfw.html

amount DECIMAL(10, 2),
来源：http://hz.ybcxt.top/gtqdgmhewo.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.cashguo.top/gtthrvforx.html

);
来源：http://hz.quarkkingdee.top/gthnehubem.html

[Q03] 增加列
来源：http://hz.hongshengwenyu.top/gtupkaluer.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.sweek.top/gttjhgfxpa.html

[Q04] 修改列类型
来源：http://hz.fengsongda.top/gtvvwgumva.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.jinqigufen.top/gtnqyanhvm.html

[Q05] 重命名列
来源：http://hz.wangshuangyany.cn/gtibqqtqib.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.cheryme.top/gthppxaxpy.html

[Q06] 删除列
来源：http://hz.zhixingplan.top/gtzhlggbqd.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.snrcjt.cn/gtchxiebmk.html

[Q07] 删除表
来源：http://hz.andypj.xyz/gtcizinfwt.html

DROP TABLE IF EXISTS orders;
来源：http://hz.kuanghao11.cn/gtalkkeveb.html

[Q08] 创建普通索引
来源：http://hz.jianghu66.top/gtkunlluoi.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.fzhhl.top/gtrxuosefo.html

[Q09] 创建唯一索引
来源：http://hz.ivvv.top/gtemztrdwj.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.wangdashe.top/gtottaxrbx.html

[Q10] 插入单行
来源：http://hz.sufxvd.cn/gtnzpetvhv.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.jyoumei.cn/gtoyequfqe.html

[Q11] 一次插入多行
来源：http://hz.zhiwuduotai.top/gtwjjhalkl.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.feifeiyinyue.top/gtctknvjhf.html

[Q12] 插入后取自增 ID
来源：http://hz.hysaishi.cn/gtyicuwszn.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.mhx1999.top/gtwyvkoagm.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.wangshuangyany.cn/gtgpxuubrj.html

[Q13] 忽略重复插入
来源：http://hz.52xcode.cn/gtxbfgroat.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.daxiang520.top/gtukwgipfp.html

[Q14] 存在则更新（upsert）
来源：http://hz.jyoumei.cn/gtvmkqaiin.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.wangdashe.top/gtgxfswnkq.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.jiagoushi.top/gtgdujrykf.html

[Q15] 查询全部
来源：http://hz.tanke756.top/gtepsxbgok.html

SELECT * FROM users;
来源：http://hz.yanxiufei.cn/gtlpcjpitg.html

[Q16] 查询指定列
来源：http://hz.xinyue.icu/gtuizgjoxz.html

SELECT id, name FROM users;
来源：http://hz.ppjwa.cn/gtkkmagbmy.html

[Q17] 条件查询
来源：http://hz.cdnleiting.top/gtzjdlrxnh.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.316326.xyz/gtryiiaqeu.html

[Q18] 模糊匹配
来源：http://hz.pengpengdd.cyou/gtuxtngzgn.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.zhaomingkeji.xyz/gttwsodjgp.html

[Q19] 范围查询
来源：http://hz.sxryk.cn/gtfzcqltwk.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.ywan-chungtsiang.top/gtxxnrqeka.html

[Q20] IN 列表
来源：http://hz.316326.xyz/gtazuhbwws.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.hfpthk.cn/gttilcjdqd.html

[Q21] 空值判断
来源：http://hz.jlsjyb.cn/gteyujbvqh.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.316326.xyz/gtqxagnxxd.html

[Q22] 排序
来源：http://hz.ppjwa.cn/gtdhnoplmi.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.ybcxt.top/gttqwwssqs.html

[Q23] 分页
来源：http://hz.zhengqikj.top/gtmbazyhpq.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.shuidangran.top/gteoxiludz.html

[Q24] 去重
来源：http://hz.hywenlv.cn/gtdjgluxvy.html

SELECT DISTINCT city FROM users;
来源：http://hz.aizwys.cn/gtltcdzsve.html

[Q25] 只取前 N 条
来源：http://hz.shanyushiyangkeji.top/gtbfwmvmtr.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.aizwys.cn/gtrmbzvevp.html

[Q26] 计数
来源：http://hz.yueranfly.top/gtqibsvohd.html

SELECT COUNT(*) FROM users;
来源：http://hz.yuanzhike.top/gtawlbrlfj.html

[Q27] 条件计数
来源：http://hz.pengpengdd.cyou/gtnkvelzbj.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.hammf.cn/gtuyqhetwa.html

[Q28] 求和与平均
来源：http://hz.jqgfzy.top/gtdabpvgph.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.zhengqikj.top/gtrrpocnme.html

[Q29] 最大最小值
来源：http://hz.chenzaomai.com/gtkqkzymsf.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.iojbl.cn/gtjsgzmrwj.html

[Q30] 分组统计
来源：http://hz.yongpay.top/gtbdskjdqp.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.cheryme.top/gtooqhatej.html

[Q31] 分组后过滤
来源：http://hz.kuanghao11.cn/gtltvvfxpb.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.chenjidiqi.icu/gtyxsebuhm.html

[Q32] 分组拼接字符串
来源：http://hz.pycfn.com/gtszqxojwf.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.hfpthk.cn/gtmmlykyjc.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.yanxiufei.cn/gtslphrnhk.html

[Q33] 多列分组
来源：http://hz.ivvv.top/gtbzgjzzdd.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.pengpengdd.cyou/gtgpdrusqy.html

[Q34] 每组取第一条
来源：http://hz.meibo888.top/gtkmcutnmg.html

SELECT * FROM (
来源：http://hz.jlsjyb.cn/gtekmeqywb.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.smart0.xyz/gtomidyefe.html

) t WHERE rn = 1;
来源：http://hz.shuidangran.top/gtecmkuidy.html

[Q35] 内连接
来源：http://hz.jlsjyb.cn/gtyiqtzjkh.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.0kj1m.cn/gtemwgsvot.html

[Q36] 左连接
来源：http://hz.vqdsnc.cn/gtpcpsfwul.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.gotoacloud.top/gtklvhtkpt.html

[Q37] 右连接
来源：http://hz.jqgfzy.top/gtfihjlclt.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.wangshuangyany.cn/gtfedilqlk.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.gogol.net.cn/gtfuzqbzqv.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.sweek.top/gtvapccast.html

[Q39] 自连接（查上下级）
来源：http://hz.shangyingyoupin.top/gtzboajexm.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.dashuyun.cn/gtmqlavxll.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.yj202588.top/gtznwtjtfv.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.chenlongwang.top/gtxrekyele.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.gotoacloud.top/gtdhotaanb.html

[Q41] 多表连接
来源：http://hz.yj202588.top/gtdiyaiyrv.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.zycfv.cn/gtvynfykae.html

JOIN users u ON u.id = o.user_id
来源：http://hz.chenzaomai.com/gtpqxzbhnq.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.hnxiangtu.top/gtdrwlcxhm.html

[Q42] 连接条件附加过滤
来源：http://hz.gzhubu.top/gtkwjkqimf.html

SELECT u.name, o.amount FROM users u
来源：http://hz.shanyushiyangtech.top/gttqrxzqjw.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.shanyushiyangtech.top/gtymgovkzr.html

[Q43] 标量子查询
来源：http://hz.xuetiantiany.cn/gtydpffnux.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.kuanghao11.cn/gtcvlpptck.html

[Q44] IN 子查询
来源：http://hz.hywenlv.cn/gtvagerual.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.jinqigufen.top/gtfezxjzdj.html

[Q45] EXISTS 判断存在
来源：http://hz.ivvv.top/gtpkzjlgcc.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.havefunace.top/gthaugtwsi.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.jianghu66.top/gtupquxxjk.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.havefunace.top/gtxvbrtoeh.html

[Q47] 与平均值比较
来源：http://hz.birdmap.top/gtpdgilwfe.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.meibo888.top/gtxqijxnta.html

[Q48] CTE 公用表表达式
来源：http://hz.nwbrower.top/gtcdhmeqmj.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.wangdashe.top/gtvspvljcv.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.sxryk.cn/gtatrlvlwq.html

[Q49] 更新单行
来源：http://hz.sweek.top/gtnoemorsi.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.c1oappe.top/gtujjezdhp.html

[Q50] 批量更新
来源：http://hz.zhengqikj.top/gtkknwddxl.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.gzhubu.top/gtoytdktbw.html

[Q51] 用子查询更新
来源：http://hz.daxiang520.top/gtllopxdiw.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.zhongyouzk.top/gtdkcqddqz.html

[Q52] 删除指定行
来源：http://hz.316326.xyz/gtblgwousu.html

DELETE FROM users WHERE id = 10;
来源：http://hz.haohaochexian.top/gtllpiwfer.html

[Q53] 按条件删除
来源：http://hz.gotoacloud.top/gtrnudptdo.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.snrcjt.cn/gtwdwijsts.html

[Q54] 清空表
来源：http://hz.chenzaomai.com/gtzuajzmoy.html

TRUNCATE TABLE logs;
来源：http://hz.nwbrower.top/gtixszfqeb.html

[Q55] 排名（并列占位）
来源：http://hz.jlsjyb.cn/gtvipphvls.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.zhengqikj.top/gtpkjwgjlq.html

[Q56] 密集排名（并列不占位）
来源：http://hz.vqdsnc.cn/gtqvlihkjf.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.ywan-chungtsiang.top/gtcaardazq.html

[Q57] 行号
来源：http://hz.chenjidiqi.icu/gttcggrygw.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.cheryme.top/gtefeffibe.html

[Q58] 累计求和
来源：http://hz.zhongyouzk.top/gtvepfkodd.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.wangdashe.top/gtnupiocgt.html

[Q59] 分组内累计
来源：http://hz.ybcxt.top/gtrptixpqh.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.yonumen.top/gtvzpwrihn.html

[Q60] 取上一行 / 下一行
来源：http://hz.yongpay.top/gtczlexzys.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.yj20258888.top/gtadyfjvzg.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.gzhubu.top/gtkkkwevbx.html

[Q61] 移动平均
来源：http://hz.ybcxt.top/gtsqwderhs.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.jlsjyb.cn/gtgsloiyxr.html

[Q62] 分组占比
来源：http://hz.zhijiandao.cn/gtlpdcvnii.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.pycfn.com/gtgnnebieg.html

[Q63] 开启事务
来源：http://hz.yonumen.top/gtzsbthtbq.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.quarkkingdee.top/gtmrqgnquu.html

[Q64] 提交事务
来源：http://hz.jiagoushi.top/gtanptivip.html

COMMIT;
来源：http://hz.gaohongyu789.top/gtnxppcoeu.html

[Q65] 回滚事务
来源：http://hz.ywan-chungtsiang.top/gtdnztakme.html

ROLLBACK;
来源：http://hz.guannengcc.top/gtoqzniykh.html

[Q66] 行锁查询
来源：http://hz.xylfe.cn/gtzjfkymmj.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.havefunace.top/gtxcmeeweh.html

[Q67] 设置隔离级别
来源：http://hz.yj202588.top/gtcwclouyx.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.dashuyun.cn/gtqcbdjexe.html

[Q68] 保存点
来源：http://hz.xylfe.cn/gtikcljgrv.html

SAVEPOINT sp1;
来源：http://hz.daxiang520.top/gtqxuqmifw.html

ROLLBACK TO sp1;
来源：http://hz.zhiwuduotai.top/gtnzznadls.html

[Q69] 查看执行计划
来源：http://hz.zhaomingkeji.xyz/gteennmiix.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.c1oappe.top/gtwrqyekcz.html

[Q70] 更新统计信息
来源：http://hz.gogol.net.cn/gtxyqplzfs.html

ANALYZE TABLE users;
来源：http://hz.zhoulong.xyz/gtzuzqmbod.html

[Q71] 查看建表语句
来源：http://hz.haohaochexian.top/gtcjdgkltj.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.tian-w.cn/gtdueqdrmw.html

[Q72] 查看索引
来源：http://hz.pengpengdd.cyou/gtwohfxwom.html

SHOW INDEX FROM users;
来源：http://hz.quarkkingdee.top/gtqlgzjxld.html

[Q73] 查看表状态
来源：http://hz.sysykeji.top/gtjcctuywj.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.dashuyun.cn/gtdbfghfgd.html

[Q74] 强制使用索引
来源：http://hz.yvedp.cn/gtyapuqxun.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.nanxinkj.top/gtizmzxmli.html

[Q75] 日期格式化
来源：http://hz.yj202588.top/gtzmvjjucj.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.guowangkeji.top/gtzggjgzjb.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.yj20258.top/gtbupgdwjt.html

[Q76] 按天统计
来源：http://hz.9152youxi.cn/gtskvatdou.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.daria6918.cn/gtwkdysgvl.html

[Q77] 时间加减
来源：http://hz.ywan-chungtsiang.top/gtpekcddpa.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.shuidangran.top/gtlzlcunkn.html

[Q78] 当前时间
来源：http://hz.havefunace.top/gtcekkszsf.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.ywan-chungtsiang.top/gtaxfedpth.html

[Q79] 字符串拼接
来源：http://hz.chenjidiqi.icu/gtsitoqvjp.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.jianghu66.top/gtbuyehyzc.html

[Q80] 字符串截取
来源：http://hz.yongpay.top/gthccplzgn.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.havefunace.top/gtwzdagrnx.html

[Q81] 字符串替换
来源：http://hz.cheryme.top/gtwexpfcgw.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.tanke756.top/gtjnbypglg.html

[Q82] 字符长度与字节长度
来源：http://hz.ivvv.top/gtoqmwazkz.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.tanke756.top/gtrzekseuk.html

[Q83] 大小写转换
来源：http://hz.aibaodan.cn/gthsqzympe.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.shanyushiyangkeji.top/gtlfbjmcge.html

[Q84] 去除首尾空格
来源：http://hz.cqqwz.cn/gtaxowfxnh.html

SELECT TRIM(name) FROM users;
来源：http://hz.gzhubu.top/gtaxekojgf.html

[Q85] 数值取整
来源：http://hz.hnqzz.top/gtuambzpgs.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.svipenyu.cn/gtpbtkbefk.html

[Q86] 读取 JSON 字段
来源：http://hz.hywenlv.cn/gtcdqvyelh.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.c1oappe.top/gttrhdxtbz.html

[Q87] JSON 字段做条件
来源：http://hz.316326.xyz/gtusrzfuzw.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.snrcjt.cn/gtxxviiots.html

[Q88] 行转列（条件聚合）
来源：http://hz.xingfuxueyuan.xyz/gttsnjorhr.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.ehwqpu.com/gtuavrtbnn.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.yvedp.cn/gtjibyzpha.html

[Q89] 判断表是否存在
来源：http://hz.zycfv.cn/gtalabsrlc.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.hfpthk.cn/gtgzsfptba.html

[Q90] 生成序号列
来源：http://hz.dashuyun.cn/gtfaxuyqom.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.zhoulong.xyz/gtgphamuir.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtubbiirev.html

R. Bash 专题
来源：http://hz.zhengqikj.top/gtxjnlhzzg.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtsbvfxkqr.html

[R01] shebang 与严格模式
来源：http://hz.hnxiangtu.top/gtutqqrwfy.html

#!/usr/bin/env bash
来源：http://hz.meibo888.top/gtlltbfzyx.html

set -euo pipefail
来源：http://hz.xylfe.cn/gtfidnsrzo.html

[R02] 变量赋值与使用
来源：http://hz.tanke756.top/gttxyuwywb.html

name="Tom"; echo "$name"
来源：http://hz.yuxming.cn/gtntsbptwy.html

[R03] 只读变量
来源：http://hz.zhaomingkeji.xyz/gtcdwhnbzo.html

readonly PI=3.14
来源：http://hz.bjfxy.top/gtvuikkxff.html

[R04] 位置参数
来源：http://hz.sxryk.cn/gtepsxqpgd.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.yuanzhike.top/gtuqnnbage.html

[R05] 参数默认值
来源：http://hz.ivvv.top/gtgpascqpf.html

name="${1:-default}"
来源：http://hz.9152youxi.cn/gtddxcbdlm.html

[R06] 判断命令是否存在
来源：http://hz.xylfe.cn/gtvgftamcv.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.zdqjudy.top/gtoyqasyus.html

[R07] if 判断文件
来源：http://hz.chenjidiqi.icu/gtioijqowi.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.mhx1999.top/gtztcubxfu.html

[R08] 数值比较
来源：http://hz.smart0.xyz/gtyijgnaiq.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.ydjk.org.cn/gtvvvdmzbn.html

[R09] 字符串比较
来源：http://hz.iojbl.cn/gtgbsugppx.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.yj20258888.top/gtubpxfpuf.html

[R10] 正则匹配
来源：http://hz.gotoacloud.top/gtwttfrpxn.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.hfpthk.cn/gtkufdnnth.html

[R11] case 多分支
来源：http://hz.ywan-chungtsiang.top/gtfhgeiszt.html

case "$1" in
来源：http://hz.aizwys.cn/gtnystjzpx.html

start) echo "启动" ;;
来源：http://hz.nwbrower.top/gtryvhatxq.html

stop)  echo "停止" ;;
来源：http://hz.shanyushiyangkeji.top/gtisjmoqdd.html

*)     echo "未知命令" ;;
来源：http://hz.daxiang520.top/gtgafmrhrb.html

esac
来源：http://hz.fzhhl.top/gtscnkjbjm.html

[R12] for 遍历文件
来源：http://hz.guannengcc.top/gtsfejewlw.html

for f in *.txt; do echo "$f"; done
来源：http://hz.zhaomingkeji.xyz/gtjwohdnkd.html

[R13] for 计数循环
来源：http://hz.zhengqikj.top/gtzxhsbzvo.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.jqgufenzy.top/gtqcxlksym.html

[R14] C 风格 for
来源：http://hz.aizwys.cn/gtlqfqodlh.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.havefunace.top/gtqvxulsva.html

[R15] while 逐行读文件
来源：http://hz.cdnleiting.top/gteztmlqaa.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.dianchejie.cn/gtoczxyxaj.html

[R16] until 等待条件
来源：http://hz.cashguo.top/gtjbdfdatq.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.gotoacloud.top/gtftntrxmx.html

[R17] 数组定义与取值
来源：http://hz.yanxiufei.cn/gtmdqxigqm.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.jqgfzy.top/gtudcrhxiz.html

[R18] 遍历数组
来源：http://hz.52xcode.cn/gtkqadvmoe.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.xziqi.cn/gtpnoscxwu.html

[R19] 数组长度
来源：http://hz.yuanzhike.top/gtfhztqwtq.html

echo "${#arr[@]}"
来源：http://hz.yj20258.top/gthhqbgjyx.html

[R20] 关联数组（字典）
来源：http://hz.meibo888.top/gtivltfdvt.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.snrcjt.cn/gtmlqiqzjx.html

[R21] 字符串长度
来源：http://hz.daria6918.cn/gtptnluvpd.html

echo "${#s}"
来源：http://hz.guannengcc.top/gtgkjokvxn.html

[R22] 截取子串
来源：http://hz.nwbrower.top/gtfsnjabqg.html

echo "${s:0:5}"
来源：http://hz.hnqzz.top/gtilychmvz.html

[R23] 字符串替换
来源：http://hz.hammf.cn/gtifezehsf.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.9152youxi.cn/gtpilkzuqq.html

[R24] 大小写转换
来源：http://hz.yj20258.top/gtviiemlfe.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.hnqzz.top/gtcfewcoju.html

[R25] 去后缀 / 去前缀
来源：http://hz.quarkkingdee.top/gtgduqzliz.html


<!-- 参考信息 -->