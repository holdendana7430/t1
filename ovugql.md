代发 wailian999

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.xingfuxueyuan.xyz/gtvncsqtug.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.zhengqikj.top/gtghoaupmr.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.yueranfly.top/gthwbwmmdq.html

PHP:  if (empty($x)) {}
来源：http://hz.nanxinkj.top/gtwnsnirur.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.fzhhl.top/gtvlpzwrjq.html

TS:   if (x == null) {}
来源：http://hz.shuidangran.top/gtiuyfwmva.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.0kj1m.cn/gtixmkfypy.html

Go:   if x == nil {}
来源：http://hz.shuidangran.top/gtfsmorwbv.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.zhijiandao.cn/gtfhjmijiu.html

C#:   if (x is null) {}
来源：http://hz.jqgufenzy.top/gtmowmsvwr.html

[P07] 防抖与节流
来源：http://hz.shanyushiyangkeji.top/gtajtsrteh.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.xinyue.icu/gtijyoxfpw.html

PHP:  // 手写时间戳比较
来源：http://hz.yueranfly.top/gtqfuvxxts.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.gotoacloud.top/gtnzssrttd.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.shuidangran.top/gtyodldfym.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.aibaodan.cn/gtohpmswap.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.daxiang520.top/gtlfsdsaxj.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.yangfankeji.com/gtxyjczwdu.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.aizwys.cn/gtbfqfiarz.html

[P08] 处理浮点精度问题
来源：http://hz.guowangkeji.top/gtwnklpxzp.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.shangyingyoupin.top/gtfcvwpxct.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.xylfe.cn/gtgaqlglqu.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.zdqjudy.top/gtonarnxko.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.jqgufenzy.top/gtrkudxdfz.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.xinyue.icu/gtngludlnz.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.xingfuxueyuan.xyz/gtprybwhpx.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.zhaomingkeji.xyz/gtrgybtwnj.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.xuanzx.com/gtrevdjdou.html

================================================================================
来源：http://hz.jyoumei.cn/gttteoxohk.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.kuanghao11.cn/gtrpaaecro.html

================================================================================
来源：http://hz.zycfv.cn/gtyhdmgujt.html

[Q01] 创建表
来源：http://hz.feifeiyinyue.top/gtfsigwygf.html

CREATE TABLE users (
来源：http://hz.ivvv.top/gttluvbome.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jinghuilouyu.cn/gtmnkkjtsb.html

name VARCHAR(50) NOT NULL,
来源：http://hz.zhaomingkeji.xyz/gtgqgyzycc.html

email VARCHAR(100) UNIQUE,
来源：http://hz.zhoulong.xyz/gtxxruxgkx.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.aizwys.cn/gtbhjnnlta.html

);
来源：http://hz.gaohongyu789.top/gtloikezyl.html

[Q02] 创建带外键的表
来源：http://hz.shuidangran.top/gtxcrdykfg.html

CREATE TABLE orders (
来源：http://hz.316326.xyz/gtmiqwinpu.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.sufxvd.cn/gtlbaowffv.html

user_id INT NOT NULL,
来源：http://hz.chenjidiqi.icu/gttbziwgji.html

amount DECIMAL(10, 2),
来源：http://hz.shzxlz.cn/gtujndgozv.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.havefunace.top/gtkkatomuj.html

);
来源：http://hz.yj20258888.top/gtaeobjiji.html

[Q03] 增加列
来源：http://hz.vqdsnc.cn/gtzgrxwwve.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.hysaishi.cn/gtxbcchgoe.html

[Q04] 修改列类型
来源：http://hz.mhx1999.top/gtyhrovmfh.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.yj202588.top/gteorueous.html

[Q05] 重命名列
来源：http://hz.yongpay.top/gtprbiaafr.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.sxryk.cn/gtvkuwjsgi.html

[Q06] 删除列
来源：http://hz.gzhubu.top/gtbbdqowfz.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.ydzc1.top/gtdglxrxmk.html

[Q07] 删除表
来源：http://hz.xuanzx.com/gtgeduhiod.html

DROP TABLE IF EXISTS orders;
来源：http://hz.chenzaomai.com/gtubaipcrk.html

[Q08] 创建普通索引
来源：http://hz.nanxinkj.top/gtdrgyafki.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.yanxiufei.cn/gtlstmzxws.html

[Q09] 创建唯一索引
来源：http://hz.xziqi.cn/gtrsbuojhw.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.52xcode.cn/gtpcdafxwe.html

[Q10] 插入单行
来源：http://hz.ybcxt.top/gtnjqnyocc.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.zhoulong.xyz/gtkbzrmbiu.html

[Q11] 一次插入多行
来源：http://hz.meibo888.top/gtlywcxshp.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.xuanzx.com/gtauyqamwy.html

[Q12] 插入后取自增 ID
来源：http://hz.shanyushiyangkeji.top/gttqjkwzon.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.hnqzz.top/gtirpceoek.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.nwbrower.top/gtirgkxskb.html

[Q13] 忽略重复插入
来源：http://hz.aibaodan.cn/gteutadxhc.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.ppjwa.cn/gtzluardpv.html

[Q14] 存在则更新（upsert）
来源：http://hz.yangfankeji.com/gtftzmgwpp.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.svipenyu.cn/gtnuhaohiz.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.zdqjudy.top/gtuusewyoe.html

[Q15] 查询全部
来源：http://hz.shanyushiyangtech.top/gtswsnvjgz.html

SELECT * FROM users;
来源：http://hz.yonumen.top/gtjdwrywiu.html

[Q16] 查询指定列
来源：http://hz.snrcjt.cn/gtijgfjlzw.html

SELECT id, name FROM users;
来源：http://hz.fengsongda.top/gtgigyhjae.html

[Q17] 条件查询
来源：http://hz.jqgufenzy.top/gtwpkhxdgx.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.mhx1999.top/gtpbtvzwgm.html

[Q18] 模糊匹配
来源：http://hz.zhiwuduotai.top/gtdldesczn.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.tian-w.cn/gtlhxanqvo.html

[Q19] 范围查询
来源：http://hz.jinqigufen.top/gtaecwlbrg.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.yonumen.top/gtmjvumbrv.html

[Q20] IN 列表
来源：http://hz.nwbrower.top/gtcwfsrmgp.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.xuetiantiany.cn/gtukliihwu.html

[Q21] 空值判断
来源：http://hz.yj20258888.top/gtxdtmwdys.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.zdqjudy.top/gtddasghhp.html

[Q22] 排序
来源：http://hz.tanke756.top/gthdpuuuup.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.bjfxy.top/gtlraanzlr.html

[Q23] 分页
来源：http://hz.snrcjt.cn/gtvgtetdmd.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.quarkkingdee.top/gtosuwcadi.html

[Q24] 去重
来源：http://hz.aibaodan.cn/gtyghmyfzh.html

SELECT DISTINCT city FROM users;
来源：http://hz.cdnleiting.top/gtxedlwfdn.html

[Q25] 只取前 N 条
来源：http://hz.vqdsnc.cn/gthrfflmhd.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.xingfuxueyuan.xyz/gtejinvork.html

[Q26] 计数
来源：http://hz.daria6918.cn/gthnpjtxdn.html

SELECT COUNT(*) FROM users;
来源：http://hz.jianghu66.top/gtnysuuwkd.html

[Q27] 条件计数
来源：http://hz.xingfuxueyuan.xyz/gtscdwgosd.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.hywenlv.cn/gtxqbqqgua.html

[Q28] 求和与平均
来源：http://hz.wangdashe.top/gtbgenjcak.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.chenjidiqi.icu/gtcilnnnga.html

[Q29] 最大最小值
来源：http://hz.hongshengwenyu.top/gtxvndydws.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.aibaodan.cn/gtgjasdqlv.html

[Q30] 分组统计
来源：http://hz.wangdashe.top/gteaahildm.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.sysykeji.top/gtxbouvsld.html

[Q31] 分组后过滤
来源：http://hz.316326.xyz/gtyijwhdzv.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.c1oappe.top/gtinszjbmv.html

[Q32] 分组拼接字符串
来源：http://hz.hammf.cn/gtixiiixco.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.yangfankeji.com/gtzaarzmop.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.pengpengdd.cyou/gtzzkuezfu.html

[Q33] 多列分组
来源：http://hz.kuanghao11.cn/gtsidtyoeq.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.wangshuangyany.cn/gtkbgbpnrv.html

[Q34] 每组取第一条
来源：http://hz.nanxuanxn.top/gtgfdshlxw.html

SELECT * FROM (
来源：http://hz.xuanzx.com/gthwxrqhpc.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.tianlin.xyz/gtcocdfymy.html

) t WHERE rn = 1;
来源：http://hz.gaohongyu789.top/gtpsrzkppy.html

[Q35] 内连接
来源：http://hz.guannengcc.top/gtgarcjzcc.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.fzhhl.top/gtfbaflhvw.html

[Q36] 左连接
来源：http://hz.tianlin.xyz/gtlfhpphwd.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.svipenyu.cn/gtbfqizibr.html

[Q37] 右连接
来源：http://hz.aibaodan.cn/gttzdqocew.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.nwbrower.top/gtmyerkexs.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.xziqi.cn/gtthoqppzk.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.yvedp.cn/gtffhcihba.html

[Q39] 自连接（查上下级）
来源：http://hz.xuanzx.com/gtstqwgehw.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.ivvv.top/gtzqcqziei.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.yonumen.top/gtgnmmnggb.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.sysykeji.top/gtdjhjlsoh.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.xuanzx.com/gtejcjowqc.html

[Q41] 多表连接
来源：http://hz.fzhhl.top/gtvnjqhjbr.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.mhx1999.top/gtrhmcdkvv.html

JOIN users u ON u.id = o.user_id
来源：http://hz.zhoulong.xyz/gtahcwbodu.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.hammf.cn/gtrgvprpgl.html

[Q42] 连接条件附加过滤
来源：http://hz.sweek.top/gtnbdpwjhd.html

SELECT u.name, o.amount FROM users u
来源：http://hz.hnqzz.top/gtqzqrbaqo.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.ydzc1.top/gtswwzktjj.html

[Q43] 标量子查询
来源：http://hz.tian-w.cn/gtrvrslxtp.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.yj20258.top/gtuzvhpntw.html

[Q44] IN 子查询
来源：http://hz.smart0.xyz/gtdxdmctbk.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.tianlin.xyz/gtmxtijgcj.html

[Q45] EXISTS 判断存在
来源：http://hz.shanyushiyangkeji.top/gtyumaquht.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zdqjudy.top/gtlfdlyibq.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.guowangkeji.top/gtmfwgsepr.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zhixingplan.top/gtessbjrvl.html

[Q47] 与平均值比较
来源：http://hz.xuetiantiany.cn/gtteqncqyv.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.hfpthk.cn/gtaairfycv.html

[Q48] CTE 公用表表达式
来源：http://hz.chenzaomai.com/gtxpnxxkzy.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.zhijiandao.cn/gtzaldcywi.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.yuxming.cn/gtvcfjilqc.html

[Q49] 更新单行
来源：http://hz.guowangkeji.top/gtgpxotprp.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.ybcxt.top/gtjfuatluo.html

[Q50] 批量更新
来源：http://hz.ppjwa.cn/gtyhdsjwkq.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.gogol.net.cn/gtqpyprdur.html

[Q51] 用子查询更新
来源：http://hz.wangdashe.top/gtzdxqageg.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.bjfxy.top/gtrbyeiwoc.html

[Q52] 删除指定行
来源：http://hz.cashguo.top/gtfliybkai.html

DELETE FROM users WHERE id = 10;
来源：http://hz.wangdashe.top/gtkkyyqqjg.html

[Q53] 按条件删除
来源：http://hz.chenjidiqi.icu/gtwkayyhnl.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.ydzc1.top/gtxczzqgwh.html

[Q54] 清空表
来源：http://hz.yueranfly.top/gtbzluxpli.html

TRUNCATE TABLE logs;
来源：http://hz.sufxvd.cn/gtsjuanbph.html

[Q55] 排名（并列占位）
来源：http://hz.redwolf501.top/gtguaopatw.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.svipenyu.cn/gtoyppuukv.html

[Q56] 密集排名（并列不占位）
来源：http://hz.jianghu66.top/gthwdfztgd.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.nwbrower.top/gtykvpbtwh.html

[Q57] 行号
来源：http://hz.gaohongyu789.top/gtfagznrau.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.xziqi.cn/gtepyezyyh.html

[Q58] 累计求和
来源：http://hz.hnqzz.top/gttxmrukvs.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.yvedp.cn/gtjxfbqova.html

[Q59] 分组内累计
来源：http://hz.pengpengdd.cyou/gtmhuhbvbm.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.yonumen.top/gtabheblkk.html

[Q60] 取上一行 / 下一行
来源：http://hz.jiagoushi.top/gtpyikjpho.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.ydzc1.top/gtbijyjifs.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.xuetiantiany.cn/gtjbvwbimm.html

[Q61] 移动平均
来源：http://hz.snrcjt.cn/gtukdskpqf.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.xuetiantiany.cn/gtjwvxtkvc.html

[Q62] 分组占比
来源：http://hz.pycfn.com/gtwoibpgla.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.meibo888.top/gtcxrxziut.html

[Q63] 开启事务
来源：http://hz.aizwys.cn/gtycgmftkl.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.tianlin.xyz/gtysfqnbpg.html

[Q64] 提交事务
来源：http://hz.yvedp.cn/gtjqdozsix.html

COMMIT;
来源：http://hz.jinqigfzy.top/gtbiezrizs.html

[Q65] 回滚事务
来源：http://hz.gaohongyu789.top/gtpmueqanm.html

ROLLBACK;
来源：http://hz.jianghu66.top/gtgergoock.html

[Q66] 行锁查询
来源：http://hz.yj202588.top/gtvnhaujjg.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.tian-w.cn/gtnkbujswl.html

[Q67] 设置隔离级别
来源：http://hz.xylfe.cn/gtzkplzsom.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.wangshuangyany.cn/gtyfheekxy.html

[Q68] 保存点
来源：http://hz.yueranfly.top/gthemxeaot.html

SAVEPOINT sp1;
来源：http://hz.bjfxy.top/gtlrsbvymm.html

ROLLBACK TO sp1;
来源：http://hz.ywan-chungtsiang.top/gtkbvtsqxk.html

[Q69] 查看执行计划
来源：http://hz.fengsongda.top/gtwmwazxuq.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.yongpay.top/gtatujdzji.html

[Q70] 更新统计信息
来源：http://hz.meibo888.top/gtldztaxqg.html

ANALYZE TABLE users;
来源：http://hz.aibaodan.cn/gtmddcgbgw.html

[Q71] 查看建表语句
来源：http://hz.hnxiangtu.top/gtlmqbckka.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.meibo888.top/gtsnsydoiy.html

[Q72] 查看索引
来源：http://hz.9152youxi.cn/gtilwpvovn.html

SHOW INDEX FROM users;
来源：http://hz.jianghu66.top/gtbvofywhu.html

[Q73] 查看表状态
来源：http://hz.ywan-chungtsiang.top/gtmermvmjs.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.yanxiufei.cn/gtkysahfnw.html

[Q74] 强制使用索引
来源：http://hz.jinqigfzy.top/gtlfdtbyhg.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.jinqigufen.top/gtkrhwfjkc.html

[Q75] 日期格式化
来源：http://hz.jinghuilouyu.cn/gtdussncvz.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.haohaochexian.top/gtfsqfcczi.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.316326.xyz/gtwmwivvzx.html

[Q76] 按天统计
来源：http://hz.ywan-chungtsiang.top/gtabpshpka.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.ivvv.top/gtbszexaob.html

[Q77] 时间加减
来源：http://hz.hnqzz.top/gtrepqgzvq.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.hysaishi.cn/gtofztdotp.html

[Q78] 当前时间
来源：http://hz.yj20258888.top/gtyfemhnyi.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.yuxming.cn/gtroopfgwx.html

[Q79] 字符串拼接
来源：http://hz.jqgufenzy.top/gtisuvzdfc.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.jqgfzy.top/gtyjiyyymo.html

[Q80] 字符串截取
来源：http://hz.xingfuxueyuan.xyz/gtuzlxsxou.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.snrcjt.cn/gtrkltnwlv.html

[Q81] 字符串替换
来源：http://hz.ppjwa.cn/gtkrdjelpi.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.yueranfly.top/gtyppsfcdx.html

[Q82] 字符长度与字节长度
来源：http://hz.316326.xyz/gtkoexhbbh.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.ppjwa.cn/gticbscyxd.html

[Q83] 大小写转换
来源：http://hz.havefunace.top/gtmlwrjokw.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.gotoacloud.top/gtldbaqptx.html

[Q84] 去除首尾空格
来源：http://hz.sysykeji.top/gtjctwrdjo.html

SELECT TRIM(name) FROM users;
来源：http://hz.bjfxy.top/gtcfnebtvv.html

[Q85] 数值取整
来源：http://hz.kuanghao11.cn/gtyfbecvwb.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.gaohongyu789.top/gtxagkpggu.html

[Q86] 读取 JSON 字段
来源：http://hz.fzhhl.top/gtbafcsqei.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.zhongyouzk.top/gtrtearfem.html

[Q87] JSON 字段做条件
来源：http://hz.shanyushiyangkeji.top/gtvhliplvu.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.9152youxi.cn/gtdxtupjqj.html

[Q88] 行转列（条件聚合）
来源：http://hz.zhiwuduotai.top/gtpdpqyjmf.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.cucudq.cn/gtupodvgkd.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.zhijiandao.cn/gtbjpjripr.html

[Q89] 判断表是否存在
来源：http://hz.jqgfzy.top/gtztyynsum.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.meibo888.top/gtyxdlhcnk.html

[Q90] 生成序号列
来源：http://hz.yuxming.cn/gtkswuiwdn.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.jianghu66.top/gtsbwdtvni.html

================================================================================
来源：http://hz.fengsongda.top/gtcouypkgx.html

R. Bash 专题
来源：http://hz.jinyuanbaomall.cn/gtepzqtkgt.html

================================================================================
来源：http://hz.nanxinkj.top/gtqxwimbuu.html

[R01] shebang 与严格模式
来源：http://hz.jianghu66.top/gtxykcxgcz.html

#!/usr/bin/env bash
来源：http://hz.xylfe.cn/gtiwbfzdvg.html

set -euo pipefail
来源：http://hz.hywenlv.cn/gtdvvcmbwh.html

[R02] 变量赋值与使用
来源：http://hz.0kj1m.cn/gtlroskryz.html

name="Tom"; echo "$name"
来源：http://hz.hnxiangtu.top/gtshxhfrek.html

[R03] 只读变量
来源：http://hz.cashguo.top/gtwpgukwrt.html

readonly PI=3.14
来源：http://hz.xziqi.cn/gtzljkrubj.html

[R04] 位置参数
来源：http://hz.yanxiufei.cn/gtwpjcavvx.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.hnxiangtu.top/gtoevciltl.html

[R05] 参数默认值
来源：http://hz.xuetiantiany.cn/gttgrfxbpl.html

name="${1:-default}"
来源：http://hz.yonumen.top/gtezqrafwd.html

[R06] 判断命令是否存在
来源：http://hz.xylfe.cn/gthhxfoxaz.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.xziqi.cn/gtgkhtzroy.html

[R07] if 判断文件
来源：http://hz.zdqjudy.top/gtoxqhojtz.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.wangdashe.top/gtzlbenkxu.html

[R08] 数值比较
来源：http://hz.hnxiangtu.top/gtzaswcmhl.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.wangshuangyany.cn/gtyjxwtvcy.html

[R09] 字符串比较
来源：http://hz.wangdashe.top/gtbcgioogg.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.hfpthk.cn/gteitzrrey.html

[R10] 正则匹配
来源：http://hz.52xcode.cn/gtiuxbdbif.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.aizwys.cn/gtfddftgnp.html

[R11] case 多分支
来源：http://hz.yj20258888.top/gtzvqxpdfs.html

case "$1" in
来源：http://hz.gogol.net.cn/gtdkyryamm.html

start) echo "启动" ;;
来源：http://hz.wangshuangyany.cn/gtkmmwyice.html

stop)  echo "停止" ;;
来源：http://hz.jinqigfzy.top/gtyagbkvuh.html

*)     echo "未知命令" ;;
来源：http://hz.meibo888.top/gtjwoqopri.html

esac
来源：http://hz.zhiwuduotai.top/gtixsmtuvh.html

[R12] for 遍历文件
来源：http://hz.jinqigufen.top/gtvpnsgird.html

for f in *.txt; do echo "$f"; done
来源：http://hz.hnxiangtu.top/gtpkflcyvs.html

[R13] for 计数循环
来源：http://hz.ydzc1.top/gtwuzmslwl.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.haohaochexian.top/gtcovtqxca.html

[R14] C 风格 for
来源：http://hz.tianlin.xyz/gtowsjjhdl.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.svipenyu.cn/gtupobrtii.html

[R15] while 逐行读文件
来源：http://hz.hnqzz.top/gtksbzzmaq.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.jinqigfzy.top/gtiuoiyjhz.html

[R16] until 等待条件
来源：http://hz.aizwys.cn/gtdptbxssf.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.jinqigufen.top/gtvbmspols.html

[R17] 数组定义与取值
来源：http://hz.hfpthk.cn/gtnykpbnze.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.hywenlv.cn/gtjhuuoaht.html

[R18] 遍历数组
来源：http://hz.birdmap.top/gtcilkcwbx.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.jinqigufen.top/gtzmnlgdzh.html

[R19] 数组长度
来源：http://hz.hnqzz.top/gtyyeqqvzy.html

echo "${#arr[@]}"
来源：http://hz.chenjidiqi.icu/gtqdyrpudl.html

[R20] 关联数组（字典）
来源：http://hz.jinqigufen.top/gtzfkhmujk.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.dashuyun.cn/gtfxejqzdl.html

[R21] 字符串长度
来源：http://hz.yvedp.cn/gtxlphdrug.html

echo "${#s}"
来源：http://hz.xuanzx.com/gttylcwvwf.html

[R22] 截取子串
来源：http://hz.jianghu66.top/gtcvvgnfrj.html

echo "${s:0:5}"
来源：http://hz.cheryme.top/gttdazdmoq.html

[R23] 字符串替换
来源：http://hz.zhengqikj.top/gtcyuponjg.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.wangshuangyany.cn/gtauxlklbn.html

[R24] 大小写转换
来源：http://hz.sxryk.cn/gtnireekex.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.nwbrower.top/gthedtazsg.html

[R25] 去后缀 / 去前缀
来源：http://hz.nanxuanxn.top/gttnqxcmkg.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.chenzaomai.com/gtckrddxpn.html

[R26] 命令替换
来源：http://hz.nanxinkj.top/gtuprrpbxp.html

now=$(date +%F); echo "$now"
来源：http://hz.yanxiufei.cn/gtqikygxik.html

[R27] 算术展开
来源：http://hz.yangfankeji.com/gthkjgpvzj.html

echo $((1 + 2 * 3))
来源：http://hz.gaohongyu789.top/gtwftadteh.html

[R28] 浮点运算
来源：http://hz.gaohongyu789.top/gttbptzljs.html

echo "scale=2; 10/3" | bc
来源：http://hz.52xcode.cn/gtcubuokov.html

[R29] 定义函数
来源：http://hz.jyoumei.cn/gtcuupnkoa.html


<!-- 参考信息 -->