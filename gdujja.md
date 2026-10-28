代发 wailian999

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.tianlin.xyz/gtbcsoyaxm.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.nanxinkj.top/gtmioaamla.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.jlsjyb.cn/gtwmirbjon.html

PHP:  if (empty($x)) {}
来源：http://hz.zhaomingkeji.xyz/gtgghsxwtg.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.smart0.xyz/gtbzzwcslg.html

TS:   if (x == null) {}
来源：http://hz.gotoacloud.top/gtczxntkcn.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.sxryk.cn/gtqnurhfvj.html

Go:   if x == nil {}
来源：http://hz.cdnleiting.top/gtjodrbojq.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.ppjwa.cn/gtudeyfgvn.html

C#:   if (x is null) {}
来源：http://hz.ppjwa.cn/gtyjwaicnj.html

[P07] 防抖与节流
来源：http://hz.svipenyu.cn/gtctzkwyof.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.gogol.net.cn/gtzwyunnws.html

PHP:  // 手写时间戳比较
来源：http://hz.chenjidiqi.icu/gtrhdwihrp.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.shanyushiyangtech.top/gtqdbnjoem.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.sweek.top/gttklwpjok.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.chenjidiqi.icu/gtvdxuxciy.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.yuxming.cn/gtflhokfip.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.bjfxy.top/gtiwmrtfob.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.gaohongyu789.top/gtbxhflflr.html

[P08] 处理浮点精度问题
来源：http://hz.yangfankeji.com/gtbyncoqlx.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.wangdashe.top/gttnseruni.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.kuanghao11.cn/gtuwvjjbjr.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.ybcxt.top/gtptegxrzq.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.yj20258888.top/gtdqglpvkc.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.sxryk.cn/gtnxkwkirw.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.quarkkingdee.top/gtkbwmlxan.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.hywenlv.cn/gtgjcytsqg.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.shanyushiyangtech.top/gtjzsllyhy.html

================================================================================
来源：http://hz.andypj.xyz/gtoqnwqqts.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.svipenyu.cn/gtuxlfdfii.html

================================================================================
来源：http://hz.yuxming.cn/gtuyxfdamd.html

[Q01] 创建表
来源：http://hz.dashuyun.cn/gtzbsjbzxz.html

CREATE TABLE users (
来源：http://hz.yanxiufei.cn/gtwjkucaxc.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.shuidangran.top/gtqpqjqnwt.html

name VARCHAR(50) NOT NULL,
来源：http://hz.chenjidiqi.icu/gtvkbhrvrw.html

email VARCHAR(100) UNIQUE,
来源：http://hz.jinghuilouyu.cn/gtcelzhfee.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.fengsongda.top/gtnqglidnr.html

);
来源：http://hz.zhixingplan.top/gtyrlfprci.html

[Q02] 创建带外键的表
来源：http://hz.gaohongyu789.top/gtbalkntpt.html

CREATE TABLE orders (
来源：http://hz.mhx1999.top/gtdhfdwlxz.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.ydjk.org.cn/gtbnrchrry.html

user_id INT NOT NULL,
来源：http://hz.snrcjt.cn/gttvtntqfc.html

amount DECIMAL(10, 2),
来源：http://hz.chenzaomai.com/gteubeeyyp.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.yuxming.cn/gtqyuaijmh.html

);
来源：http://hz.feifeiyinyue.top/gtkyrqfrpw.html

[Q03] 增加列
来源：http://hz.xuetiantiany.cn/gteiplerty.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.cdnleiting.top/gtctbdgvgg.html

[Q04] 修改列类型
来源：http://hz.yongpay.top/gtcuubpeps.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.fzhhl.top/gtaamlayiw.html

[Q05] 重命名列
来源：http://hz.aibaodan.cn/gtqyeybxlj.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.jqgufenzy.top/gtmcijpweh.html

[Q06] 删除列
来源：http://hz.sxryk.cn/gtylzhhnpb.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.ydzc1.top/gtxrbsjbji.html

[Q07] 删除表
来源：http://hz.kuanghao11.cn/gtbehekelu.html

DROP TABLE IF EXISTS orders;
来源：http://hz.wangdashe.top/gtjnsgpwsn.html

[Q08] 创建普通索引
来源：http://hz.shzxlz.cn/gtgzjnkwph.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.haohaochexian.top/gtnfdvkcsj.html

[Q09] 创建唯一索引
来源：http://hz.hnxiangtu.top/gtojksxizc.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.redwolf501.top/gtrqippmcu.html

[Q10] 插入单行
来源：http://hz.hammf.cn/gtupuzpxdd.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.nanxinkj.top/gtzsywwsgu.html

[Q11] 一次插入多行
来源：http://hz.jlsjyb.cn/gtgtknkxrq.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.yonumen.top/gtdvvrxyzt.html

[Q12] 插入后取自增 ID
来源：http://hz.yuxming.cn/gtcairekmd.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.gotoacloud.top/gtwiwsifnl.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.xinyue.icu/gtugdzrsaa.html

[Q13] 忽略重复插入
来源：http://hz.sweek.top/gtjuwnihfd.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.cdnleiting.top/gtahkhsavl.html

[Q14] 存在则更新（upsert）
来源：http://hz.yueranfly.top/gtamaiqaio.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.svipenyu.cn/gtkdtsbmvn.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.sysykeji.top/gtlousnnqr.html

[Q15] 查询全部
来源：http://hz.jqgfzy.top/gtbyosgnpf.html

SELECT * FROM users;
来源：http://hz.gaohongyu789.top/gtcafvopwx.html

[Q16] 查询指定列
来源：http://hz.tanke756.top/gtinrowerg.html

SELECT id, name FROM users;
来源：http://hz.nanxinkj.top/gtpwovxfhy.html

[Q17] 条件查询
来源：http://hz.daria6918.cn/gtwrwaekvh.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.yj202588.top/gtrsrxtrve.html

[Q18] 模糊匹配
来源：http://hz.9152youxi.cn/gtnrkrqdkv.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.haohaochexian.top/gtclpmbnqm.html

[Q19] 范围查询
来源：http://hz.jqgufenzy.top/gtvxkopfkj.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.yj20258.top/gtsygxklbt.html

[Q20] IN 列表
来源：http://hz.feifeiyinyue.top/gteddcaxwa.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.cashguo.top/gtlijyriny.html

[Q21] 空值判断
来源：http://hz.cheryme.top/gtanmdtgwf.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.smart0.xyz/gtcksxpfag.html

[Q22] 排序
来源：http://hz.yj20258.top/gtwgynzmlm.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.zycfv.cn/gtbvtelxos.html

[Q23] 分页
来源：http://hz.andypj.xyz/gtcehhuryl.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.nwbrower.top/gtrdrecawn.html

[Q24] 去重
来源：http://hz.zhaomingkeji.xyz/gttfalfxne.html

SELECT DISTINCT city FROM users;
来源：http://hz.andypj.xyz/gtadbnxvxx.html

[Q25] 只取前 N 条
来源：http://hz.c1oappe.top/gtmkqwscjb.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.sxryk.cn/gtcjahrfuq.html

[Q26] 计数
来源：http://hz.sweek.top/gtskslhsgb.html

SELECT COUNT(*) FROM users;
来源：http://hz.kuanghao11.cn/gtvkbfcgtw.html

[Q27] 条件计数
来源：http://hz.hywenlv.cn/gtutwamahl.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.yj202588.top/gtmguvrceq.html

[Q28] 求和与平均
来源：http://hz.meibo888.top/gtagmcpbgt.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.hongshengwenyu.top/gtgbrmvlow.html

[Q29] 最大最小值
来源：http://hz.birdmap.top/gtlmdogezo.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.kuanghao11.cn/gtbqpwsvrf.html

[Q30] 分组统计
来源：http://hz.gogol.net.cn/gtrcrxeoup.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.guowangkeji.top/gtztvzztpr.html

[Q31] 分组后过滤
来源：http://hz.ywan-chungtsiang.top/gtarnmresb.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.xinyue.icu/gtxzkvtpvb.html

[Q32] 分组拼接字符串
来源：http://hz.smart0.xyz/gtwqsubxtn.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.nwbrower.top/gtmvsezioc.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.ivvv.top/gtkbryigyl.html

[Q33] 多列分组
来源：http://hz.316326.xyz/gtnybbshrr.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.yongpay.top/gtvonkycpk.html

[Q34] 每组取第一条
来源：http://hz.svipenyu.cn/gtwnajomhv.html

SELECT * FROM (
来源：http://hz.tanke756.top/gtdjjyowxr.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.jlsjyb.cn/gtuusbomqq.html

) t WHERE rn = 1;
来源：http://hz.chenzaomai.com/gtvjgnzpba.html

[Q35] 内连接
来源：http://hz.ivvv.top/gthtlfenqm.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.andypj.xyz/gtfozrrmal.html

[Q36] 左连接
来源：http://hz.jlsjyb.cn/gtpjsnjltf.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.shangyingyoupin.top/gtnqzygmpo.html

[Q37] 右连接
来源：http://hz.havefunace.top/gtqyqcbzxb.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.tian-w.cn/gtjwwripfp.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.mhx1999.top/gtzudzcfst.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.jianghu66.top/gtttrgrlvt.html

[Q39] 自连接（查上下级）
来源：http://hz.52xcode.cn/gtmohoiedl.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.hnqzz.top/gtikwklhrq.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.yongpay.top/gtrowaxqjt.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.hysaishi.cn/gtrswkpwjm.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.aibaodan.cn/gthlayihic.html

[Q41] 多表连接
来源：http://hz.guannengcc.top/gtjxywafzp.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.xingfuxueyuan.xyz/gtdgcwrawg.html

JOIN users u ON u.id = o.user_id
来源：http://hz.cqqwz.cn/gtuucrwpgx.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.daria6918.cn/gtdqnpleoh.html

[Q42] 连接条件附加过滤
来源：http://hz.chenlongwang.top/gtbxpzipyb.html

SELECT u.name, o.amount FROM users u
来源：http://hz.shanyushiyangkeji.top/gtlxmjqifr.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.nwbrower.top/gtajavybaq.html

[Q43] 标量子查询
来源：http://hz.mhx1999.top/gtccymgrhr.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.yj20258888.top/gtfuswflsg.html

[Q44] IN 子查询
来源：http://hz.guannengcc.top/gtqevqhysu.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.yangfankeji.com/gtchsnsmcw.html

[Q45] EXISTS 判断存在
来源：http://hz.zhixingplan.top/gtdxvusioi.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.ywan-chungtsiang.top/gtuhadbpcv.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.yanxiufei.cn/gtlfckctww.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.xinyue.icu/gtceqbotwz.html

[Q47] 与平均值比较
来源：http://hz.yuanzhike.top/gtqxdlgcki.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.xingfuxueyuan.xyz/gtzymrrkra.html

[Q48] CTE 公用表表达式
来源：http://hz.zhongyouzk.top/gtineqcoco.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.yuanzhike.top/gtbxqpqqht.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.pengpengdd.cyou/gteoonlrcs.html

[Q49] 更新单行
来源：http://hz.guowangkeji.top/gtvpyqliro.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.c1oappe.top/gtatvqvkkv.html

[Q50] 批量更新
来源：http://hz.nanxuanxn.top/gtrbvjzjqz.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.xinyue.icu/gtncrcfpda.html

[Q51] 用子查询更新
来源：http://hz.sysykeji.top/gtlcsdqaqe.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.ehwqpu.com/gthgumskzr.html

[Q52] 删除指定行
来源：http://hz.nwbrower.top/gtkzkoitis.html

DELETE FROM users WHERE id = 10;
来源：http://hz.dianchejie.cn/gtjoscyoor.html

[Q53] 按条件删除
来源：http://hz.shzxlz.cn/gtnltdbesu.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.chenzaomai.com/gtnzdnorxb.html

[Q54] 清空表
来源：http://hz.zhijiandao.cn/gtlsqjckpg.html

TRUNCATE TABLE logs;
来源：http://hz.xylfe.cn/gtuouwhfre.html

[Q55] 排名（并列占位）
来源：http://hz.xuanzx.com/gteszgpxef.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.jyoumei.cn/gtryxuuhiq.html

[Q56] 密集排名（并列不占位）
来源：http://hz.wangdashe.top/gtpvrzntnv.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.zhiwuduotai.top/gtocayhagf.html

[Q57] 行号
来源：http://hz.havefunace.top/gtvedosist.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.vqdsnc.cn/gtsqnnmeux.html

[Q58] 累计求和
来源：http://hz.jinghuilouyu.cn/gtenanzprm.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.ydzc1.top/gtsmiypqnp.html

[Q59] 分组内累计
来源：http://hz.yuxming.cn/gtscbgsdxa.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.haohaochexian.top/gtszckevec.html

[Q60] 取上一行 / 下一行
来源：http://hz.xziqi.cn/gttibnjsra.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.jinyuanbaomall.cn/gtlzyxubyp.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.chenlongwang.top/gtvjjcuaqq.html

[Q61] 移动平均
来源：http://hz.zhoulong.xyz/gtddhcdqwa.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.dashuyun.cn/gtikzumgjf.html

[Q62] 分组占比
来源：http://hz.wangshuangyany.cn/gtbcsgqggp.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.hongshengwenyu.top/gtjkkdutqk.html

[Q63] 开启事务
来源：http://hz.snrcjt.cn/gtzgrrwucf.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.havefunace.top/gtxjlnzplt.html

[Q64] 提交事务
来源：http://hz.sweek.top/gtphuikudq.html

COMMIT;
来源：http://hz.aibaodan.cn/gtpuafrohr.html

[Q65] 回滚事务
来源：http://hz.fzhhl.top/gtbernzvbc.html

ROLLBACK;
来源：http://hz.jiagoushi.top/gtdodijpiv.html

[Q66] 行锁查询
来源：http://hz.gzhubu.top/gtellptjvv.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.ybcxt.top/gtybxsdtbu.html

[Q67] 设置隔离级别
来源：http://hz.9152youxi.cn/gtfekvqbzh.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.c1oappe.top/gtblrgnbje.html

[Q68] 保存点
来源：http://hz.ppjwa.cn/gtjvqzxblu.html

SAVEPOINT sp1;
来源：http://hz.shangyingyoupin.top/gtjxohjzfa.html

ROLLBACK TO sp1;
来源：http://hz.redwolf501.top/gtofvpohyv.html

[Q69] 查看执行计划
来源：http://hz.hfpthk.cn/gtsrgrebql.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.zycfv.cn/gtcmnpeilv.html

[Q70] 更新统计信息
来源：http://hz.birdmap.top/gtrvuophma.html

ANALYZE TABLE users;
来源：http://hz.chenjidiqi.icu/gtqkwlhgmi.html

[Q71] 查看建表语句
来源：http://hz.hnqzz.top/gtugktfqox.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.nwbrower.top/gtddsjhpzd.html

[Q72] 查看索引
来源：http://hz.fengsongda.top/gtqlspsvdo.html

SHOW INDEX FROM users;
来源：http://hz.zhaomingkeji.xyz/gtwxwavzcy.html

[Q73] 查看表状态
来源：http://hz.yj20258888.top/gtasoxvfvg.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.ehwqpu.com/gtutjbjiwc.html

[Q74] 强制使用索引
来源：http://hz.tanke756.top/gtjmojkrgu.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.kuanghao11.cn/gtqqtzjtkh.html

[Q75] 日期格式化
来源：http://hz.nanxuanxn.top/gtwoenjvsv.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.haohaochexian.top/gtscergtjx.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.mhx1999.top/gtvleyiuql.html

[Q76] 按天统计
来源：http://hz.zhixingplan.top/gtgvgrlnoc.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.sweek.top/gtnzhwemzp.html

[Q77] 时间加减
来源：http://hz.gaohongyu789.top/gtddylhnvu.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.tianlin.xyz/gtcaguylrm.html

[Q78] 当前时间
来源：http://hz.chenzaomai.com/gtuagbbdnh.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.shangyingyoupin.top/gtzaycocum.html

[Q79] 字符串拼接
来源：http://hz.sysykeji.top/gtnkdjfzni.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.xylfe.cn/gtbwioswws.html

[Q80] 字符串截取
来源：http://hz.jianghu66.top/gtrduyjrtc.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.svipenyu.cn/gtfptnhzqh.html

[Q81] 字符串替换
来源：http://hz.dianchejie.cn/gtdswhvsxm.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.yonumen.top/gtajeplbdy.html

[Q82] 字符长度与字节长度
来源：http://hz.iojbl.cn/gtxvubwvdu.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.chenlongwang.top/gtpljunxoy.html

[Q83] 大小写转换
来源：http://hz.guowangkeji.top/gtpaqeehhd.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.ehwqpu.com/gtojkvfcib.html

[Q84] 去除首尾空格
来源：http://hz.bjfxy.top/gtdibjjshc.html

SELECT TRIM(name) FROM users;
来源：http://hz.zhiwuduotai.top/gtuadrkmzv.html

[Q85] 数值取整
来源：http://hz.cucudq.cn/gtodpkmkjc.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.cheryme.top/gtqkyerpgl.html

[Q86] 读取 JSON 字段
来源：http://hz.gzhubu.top/gtupkfesin.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.316326.xyz/gtxhmxeton.html

[Q87] JSON 字段做条件
来源：http://hz.andypj.xyz/gtttapqxnc.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.hywenlv.cn/gtxaaavdki.html

[Q88] 行转列（条件聚合）
来源：http://hz.tanke756.top/gtviprjgss.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.cheryme.top/gteyiemhzd.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.cucudq.cn/gtdszhfpij.html

[Q89] 判断表是否存在
来源：http://hz.shanyushiyangkeji.top/gtmxcbzkqz.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.andypj.xyz/gtbcjjbpzx.html

[Q90] 生成序号列
来源：http://hz.yvedp.cn/gtbglqdybm.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.haohaochexian.top/gtnnaebtlz.html

================================================================================
来源：http://hz.dianchejie.cn/gtzojgbbwt.html

R. Bash 专题
来源：http://hz.feifeiyinyue.top/gtltcgwjxo.html

================================================================================
来源：http://hz.ydjk.org.cn/gtzafyqlhr.html

[R01] shebang 与严格模式
来源：http://hz.cdnleiting.top/gtogglbhbk.html

#!/usr/bin/env bash
来源：http://hz.fengsongda.top/gtsbtwglpe.html

set -euo pipefail
来源：http://hz.zycfv.cn/gtmirmcllb.html

[R02] 变量赋值与使用
来源：http://hz.yueranfly.top/gtkkycxwpd.html

name="Tom"; echo "$name"
来源：http://hz.sufxvd.cn/gtitsqzcvj.html

[R03] 只读变量
来源：http://hz.ybcxt.top/gtwqmjwaxk.html

readonly PI=3.14
来源：http://hz.yvedp.cn/gtvronmfkq.html

[R04] 位置参数
来源：http://hz.shuidangran.top/gtustpdlfc.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.pengpengdd.cyou/gtakvsvqhu.html

[R05] 参数默认值
来源：http://hz.birdmap.top/gtqiauytkd.html

name="${1:-default}"
来源：http://hz.gaohongyu789.top/gthiqjfmxl.html

[R06] 判断命令是否存在
来源：http://hz.yuxming.cn/gtuqfwcoki.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.nwbrower.top/gtklhvzkky.html

[R07] if 判断文件
来源：http://hz.hongshengwenyu.top/gtmbmsuhhs.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.cheryme.top/gtzbatsete.html

[R08] 数值比较
来源：http://hz.quarkkingdee.top/gtyrjtkgqw.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.smart0.xyz/gtfjvajrlg.html

[R09] 字符串比较
来源：http://hz.nanxinkj.top/gtgklgjhwf.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.gzhubu.top/gthwluykzo.html

[R10] 正则匹配
来源：http://hz.aibaodan.cn/gteiisjpox.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.sysykeji.top/gtzfazizjj.html

[R11] case 多分支
来源：http://hz.zhoulong.xyz/gtickmalxb.html

case "$1" in
来源：http://hz.iojbl.cn/gtnmlqufuu.html

start) echo "启动" ;;
来源：http://hz.zhijiandao.cn/gtespythzm.html

stop)  echo "停止" ;;
来源：http://hz.jlsjyb.cn/gtjybovzxt.html

*)     echo "未知命令" ;;
来源：http://hz.yonumen.top/gtljwcphkr.html

esac
来源：http://hz.zhoulong.xyz/gtmtvzgxkf.html

[R12] for 遍历文件
来源：http://hz.sweek.top/gtyihfrwob.html

for f in *.txt; do echo "$f"; done
来源：http://hz.hongshengwenyu.top/gtlrpqajrv.html

[R13] for 计数循环
来源：http://hz.shangyingyoupin.top/gtyhaneenc.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.haohaochexian.top/gtgkctabme.html

[R14] C 风格 for
来源：http://hz.jyoumei.cn/gtbsbnrrwd.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.sufxvd.cn/gtugteapzs.html

[R15] while 逐行读文件
来源：http://hz.sweek.top/gtamhngnvg.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.kuanghao11.cn/gtznwdjigq.html

[R16] until 等待条件
来源：http://hz.quarkkingdee.top/gtyslvmexe.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.jinghuilouyu.cn/gtjfsumpnc.html

[R17] 数组定义与取值
来源：http://hz.jyoumei.cn/gtcdccxvtr.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.ppjwa.cn/gtmgkdkhqf.html

[R18] 遍历数组
来源：http://hz.shzxlz.cn/gtzayamnba.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.wangshuangyany.cn/gtdynumyao.html

[R19] 数组长度
来源：http://hz.aizwys.cn/gtuojemqat.html

echo "${#arr[@]}"
来源：http://hz.zycfv.cn/gtuyttoobg.html

[R20] 关联数组（字典）
来源：http://hz.ivvv.top/gtgibsklmp.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.fzhhl.top/gtrdrslazv.html

[R21] 字符串长度
来源：http://hz.tian-w.cn/gtkyjupexn.html

echo "${#s}"
来源：http://hz.chenjidiqi.icu/gtbogvzhdd.html

[R22] 截取子串
来源：http://hz.0kj1m.cn/gtdqtjcbqq.html

echo "${s:0:5}"
来源：http://hz.ybcxt.top/gtayommldp.html

[R23] 字符串替换
来源：http://hz.tianlin.xyz/gttvhwtohd.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.shangyingyoupin.top/gtfonbinyx.html

[R24] 大小写转换
来源：http://hz.jlsjyb.cn/gtozvaqzxg.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.xziqi.cn/gtzrvdjahw.html

[R25] 去后缀 / 去前缀
来源：http://hz.vqdsnc.cn/gtzbflmlbu.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.fzhhl.top/gtonhoqerh.html

[R26] 命令替换
来源：http://hz.hysaishi.cn/gtcgeqssqh.html

now=$(date +%F); echo "$now"
来源：http://hz.kuanghao11.cn/gtxtpxsxhv.html

[R27] 算术展开
来源：http://hz.smart0.xyz/gtbrclbwcp.html

echo $((1 + 2 * 3))
来源：http://hz.zhoulong.xyz/gtsverrzav.html

[R28] 浮点运算
来源：http://hz.yvedp.cn/gtbhefpviy.html

echo "scale=2; 10/3" | bc
来源：http://hz.gogol.net.cn/gtpntoaujl.html

[R29] 定义函数
来源：http://hz.fengsongda.top/gtgeoamqog.html


<!-- 参考信息 -->