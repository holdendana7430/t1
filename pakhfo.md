代发 wailian999

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.hywenlv.cn/gtlhptacet.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.shangyingyoupin.top/gtoqyuzmxd.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.52xcode.cn/gtbskaektx.html

PHP:  if (empty($x)) {}
来源：http://hz.svipenyu.cn/gtlbwsodgk.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.sweek.top/gteodyhhoj.html

TS:   if (x == null) {}
来源：http://hz.shangyingyoupin.top/gtihxncxhx.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.yvedp.cn/gteudujnga.html

Go:   if x == nil {}
来源：http://hz.meibo888.top/gtzypnlaou.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.ydjk.org.cn/gticxeidhf.html

C#:   if (x is null) {}
来源：http://hz.tian-w.cn/gtmhcmrdxq.html

[P07] 防抖与节流
来源：http://hz.c1oappe.top/gtmnraxbjj.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.yuxming.cn/gtroirydwh.html

PHP:  // 手写时间戳比较
来源：http://hz.ppjwa.cn/gtfajfzswv.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yuxming.cn/gtrhwpviva.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zhiwuduotai.top/gtmulfbrbh.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.gogol.net.cn/gtlsrpmmpr.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.gotoacloud.top/gtnityzkmh.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.shanyushiyangtech.top/gtjrhkktsr.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.havefunace.top/gtqdcdrhwi.html

[P08] 处理浮点精度问题
来源：http://hz.chenlongwang.top/gtcupxsfym.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.pengpengdd.cyou/gtniwvrcxt.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.xylfe.cn/gtepmizbjs.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.redwolf501.top/gtgffmzgkb.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.ydjk.org.cn/gtzpmhbniz.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.shangyingyoupin.top/gttxthfepr.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.mhx1999.top/gteailpkvf.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.yj20258888.top/gtvvitwnjl.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.nanxinkj.top/gtxrjabvqg.html

================================================================================
来源：http://hz.jianghu66.top/gtlpsomspj.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.jinghuilouyu.cn/gtinqfepau.html

================================================================================
来源：http://hz.jqgufenzy.top/gtxkshjbbs.html

[Q01] 创建表
来源：http://hz.cqqwz.cn/gtvgwhoxyy.html

CREATE TABLE users (
来源：http://hz.chenzaomai.com/gtmwiecyfu.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yj202588.top/gtrmdrpwyf.html

name VARCHAR(50) NOT NULL,
来源：http://hz.yvedp.cn/gtjjlbnkht.html

email VARCHAR(100) UNIQUE,
来源：http://hz.cheryme.top/gtcmohplvw.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.xinyue.icu/gtqphukrmj.html

);
来源：http://hz.cheryme.top/gtltfrvtkw.html

[Q02] 创建带外键的表
来源：http://hz.jlsjyb.cn/gtxsasljhd.html

CREATE TABLE orders (
来源：http://hz.zhijiandao.cn/gtibszmyvd.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.hywenlv.cn/gtswxgdjca.html

user_id INT NOT NULL,
来源：http://hz.xylfe.cn/gtruerhkyj.html

amount DECIMAL(10, 2),
来源：http://hz.zycfv.cn/gteuguivcw.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.jinqigfzy.top/gtcvifviaz.html

);
来源：http://hz.hywenlv.cn/gtwggiyhgk.html

[Q03] 增加列
来源：http://hz.sweek.top/gtktamzous.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.yongpay.top/gtchdgrgwp.html

[Q04] 修改列类型
来源：http://hz.jlsjyb.cn/gtyqjcokjw.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.xylfe.cn/gtmhdzfktg.html

[Q05] 重命名列
来源：http://hz.gotoacloud.top/gthjwwgvwc.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.svipenyu.cn/gtrfykoolh.html

[Q06] 删除列
来源：http://hz.zhongyouzk.top/gtocaaiatr.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.ehwqpu.com/gtbgkcvjuo.html

[Q07] 删除表
来源：http://hz.cdnleiting.top/gtlebvaakn.html

DROP TABLE IF EXISTS orders;
来源：http://hz.cheryme.top/gtoninyftk.html

[Q08] 创建普通索引
来源：http://hz.yonumen.top/gtxvxtbngj.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.zycfv.cn/gtkhcaoapr.html

[Q09] 创建唯一索引
来源：http://hz.ehwqpu.com/gtaxbljdmh.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.nanxuanxn.top/gtzaxxkouk.html

[Q10] 插入单行
来源：http://hz.aibaodan.cn/gtnisiqdgc.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.snrcjt.cn/gtruzbrbth.html

[Q11] 一次插入多行
来源：http://hz.iojbl.cn/gtxcvxwphm.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.chenjidiqi.icu/gtguwocugc.html

[Q12] 插入后取自增 ID
来源：http://hz.jyoumei.cn/gtjmzqcnsn.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.yuanzhike.top/gtxmjlondt.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.jinqigufen.top/gtwcrrlepr.html

[Q13] 忽略重复插入
来源：http://hz.9152youxi.cn/gteifrxhql.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.ydjk.org.cn/gtuhnuoaos.html

[Q14] 存在则更新（upsert）
来源：http://hz.yuxming.cn/gtcsxwtcaq.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.52xcode.cn/gtxmtbsilf.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.vqdsnc.cn/gtlrixizly.html

[Q15] 查询全部
来源：http://hz.kuanghao11.cn/gtebgmqjmp.html

SELECT * FROM users;
来源：http://hz.cheryme.top/gtbdbcgvwz.html

[Q16] 查询指定列
来源：http://hz.gogol.net.cn/gtnekjnlmx.html

SELECT id, name FROM users;
来源：http://hz.ppjwa.cn/gtkbhvwqdj.html

[Q17] 条件查询
来源：http://hz.zhixingplan.top/gtivahoadf.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.zhaomingkeji.xyz/gtkpzdrnvk.html

[Q18] 模糊匹配
来源：http://hz.nanxinkj.top/gtuslssxgx.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.chenlongwang.top/gtcyqltqth.html

[Q19] 范围查询
来源：http://hz.meibo888.top/gtbhiltczm.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.jqgufenzy.top/gtqdogbzjz.html

[Q20] IN 列表
来源：http://hz.guannengcc.top/gtbjmdfpkn.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.jqgfzy.top/gtizuysyyx.html

[Q21] 空值判断
来源：http://hz.havefunace.top/gtqqqdwrxj.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.jyoumei.cn/gtsbjmzmdc.html

[Q22] 排序
来源：http://hz.jqgfzy.top/gtihviddtx.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.iojbl.cn/gtkjlwxwlw.html

[Q23] 分页
来源：http://hz.zhijiandao.cn/gtqwbfolms.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.ywan-chungtsiang.top/gtakpugylg.html

[Q24] 去重
来源：http://hz.zhixingplan.top/gtectctxcv.html

SELECT DISTINCT city FROM users;
来源：http://hz.zhiwuduotai.top/gtokdhnnyx.html

[Q25] 只取前 N 条
来源：http://hz.zhiwuduotai.top/gtkxekxglc.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.zycfv.cn/gtqwbhwxqv.html

[Q26] 计数
来源：http://hz.shanyushiyangkeji.top/gtuixdcwnb.html

SELECT COUNT(*) FROM users;
来源：http://hz.andypj.xyz/gtwgaczxpf.html

[Q27] 条件计数
来源：http://hz.chenzaomai.com/gtzingtpnp.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.havefunace.top/gtkbmgziwa.html

[Q28] 求和与平均
来源：http://hz.ydzc1.top/gtqzjfxwhz.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.yanxiufei.cn/gtjsiicgxv.html

[Q29] 最大最小值
来源：http://hz.pengpengdd.cyou/gtnzgigqeo.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.iojbl.cn/gtwimwbpwk.html

[Q30] 分组统计
来源：http://hz.fengsongda.top/gtbvzuhcjl.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.316326.xyz/gtxvzsgfkt.html

[Q31] 分组后过滤
来源：http://hz.zhoulong.xyz/gtmtvkcfex.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.yvedp.cn/gthcbdiege.html

[Q32] 分组拼接字符串
来源：http://hz.aibaodan.cn/gtzwhafwaf.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.sweek.top/gtpiexqodb.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.cdnleiting.top/gtsjbepwwp.html

[Q33] 多列分组
来源：http://hz.havefunace.top/gtxbdaxqtm.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.jiagoushi.top/gtzcyhjeux.html

[Q34] 每组取第一条
来源：http://hz.ivvv.top/gtsyserwgd.html

SELECT * FROM (
来源：http://hz.smart0.xyz/gtduwhjrle.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.zhongyouzk.top/gtkbmbayos.html

) t WHERE rn = 1;
来源：http://hz.hfpthk.cn/gtxjfzbohy.html

[Q35] 内连接
来源：http://hz.zhijiandao.cn/gtehsneihg.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.shuidangran.top/gtpmtihomv.html

[Q36] 左连接
来源：http://hz.zhoulong.xyz/gtfribmjtd.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.nwbrower.top/gtcwdapbyg.html

[Q37] 右连接
来源：http://hz.guowangkeji.top/gturpiprln.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.cqqwz.cn/gtacaufpkm.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.chenzaomai.com/gtgvvogltu.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.haohaochexian.top/gtgvciyxuy.html

[Q39] 自连接（查上下级）
来源：http://hz.ydzc1.top/gteqhnjdfr.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.cdnleiting.top/gthhwdejsv.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.yj20258.top/gthdglpfrc.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.wangshuangyany.cn/gtnizmpbvc.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.ydjk.org.cn/gtxahvrexf.html

[Q41] 多表连接
来源：http://hz.wangdashe.top/gttlnybtuc.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.shangyingyoupin.top/gtliqlhzvs.html

JOIN users u ON u.id = o.user_id
来源：http://hz.snrcjt.cn/gtnefjohbv.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.ivvv.top/gthbkcryur.html

[Q42] 连接条件附加过滤
来源：http://hz.sysykeji.top/gtfupjemxe.html

SELECT u.name, o.amount FROM users u
来源：http://hz.jiagoushi.top/gtrdwzfnzc.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.yj202588.top/gtiagtelmv.html

[Q43] 标量子查询
来源：http://hz.shuidangran.top/gtztbcidbo.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.shanyushiyangkeji.top/gtgkmgsxnw.html

[Q44] IN 子查询
来源：http://hz.jinyuanbaomall.cn/gtxlcnitkh.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.cdnleiting.top/gtispnupch.html

[Q45] EXISTS 判断存在
来源：http://hz.yj20258.top/gtgstmxnjg.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.hysaishi.cn/gtpamrafix.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.zhoulong.xyz/gtqomqmacx.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.shanyushiyangtech.top/gtzecfixnj.html

[Q47] 与平均值比较
来源：http://hz.sweek.top/gtzlnjerks.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.nanxinkj.top/gtmckoszaw.html

[Q48] CTE 公用表表达式
来源：http://hz.chenlongwang.top/gtbuilsatx.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.aizwys.cn/gtuicozqqf.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.yj20258888.top/gtgzibhbci.html

[Q49] 更新单行
来源：http://hz.tanke756.top/gtvklbvntd.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.jianghu66.top/gttkbzblta.html

[Q50] 批量更新
来源：http://hz.ppjwa.cn/gtqpbmbupv.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.hnqzz.top/gtgysqokno.html

[Q51] 用子查询更新
来源：http://hz.jqgufenzy.top/gtmbnsnaen.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.cashguo.top/gtpibmobwx.html

[Q52] 删除指定行
来源：http://hz.shanyushiyangtech.top/gtulehbhze.html

DELETE FROM users WHERE id = 10;
来源：http://hz.andypj.xyz/gtgfwtiuay.html

[Q53] 按条件删除
来源：http://hz.redwolf501.top/gtxigfttvm.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.tian-w.cn/gttezhkbsg.html

[Q54] 清空表
来源：http://hz.nanxinkj.top/gtunseewjx.html

TRUNCATE TABLE logs;
来源：http://hz.yonumen.top/gtaisanfxd.html

[Q55] 排名（并列占位）
来源：http://hz.jqgfzy.top/gtbdakjtxv.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.jyoumei.cn/gtkzgnknpg.html

[Q56] 密集排名（并列不占位）
来源：http://hz.haohaochexian.top/gtmdowjulq.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.xziqi.cn/gtmxfmodcc.html

[Q57] 行号
来源：http://hz.cashguo.top/gtlhcsdyrt.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.birdmap.top/gtbroizccc.html

[Q58] 累计求和
来源：http://hz.tian-w.cn/gthqmktzph.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.jinqigfzy.top/gtgjwvvlbc.html

[Q59] 分组内累计
来源：http://hz.gzhubu.top/gtulfzfwga.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.tian-w.cn/gtxtlpwevj.html

[Q60] 取上一行 / 下一行
来源：http://hz.dashuyun.cn/gtoousjliw.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.smart0.xyz/gtfhiwkthx.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.gotoacloud.top/gtfwafvfyp.html

[Q61] 移动平均
来源：http://hz.ywan-chungtsiang.top/gtojcpgckd.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.sufxvd.cn/gtztykdcti.html

[Q62] 分组占比
来源：http://hz.zhengqikj.top/gtyriobajr.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.yvedp.cn/gtfqpuzipb.html

[Q63] 开启事务
来源：http://hz.svipenyu.cn/gtcrkslmcr.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.feifeiyinyue.top/gtitwxrwdq.html

[Q64] 提交事务
来源：http://hz.jinqigufen.top/gtunxyvyys.html

COMMIT;
来源：http://hz.jinghuilouyu.cn/gtozigxmmh.html

[Q65] 回滚事务
来源：http://hz.cheryme.top/gtbmktyfjr.html

ROLLBACK;
来源：http://hz.zhijiandao.cn/gtcvfaycln.html

[Q66] 行锁查询
来源：http://hz.kuanghao11.cn/gtmbffvdjx.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.ivvv.top/gtdpahwyob.html

[Q67] 设置隔离级别
来源：http://hz.sufxvd.cn/gtnmrewlgl.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.hammf.cn/gtckfgavic.html

[Q68] 保存点
来源：http://hz.tanke756.top/gtslveanop.html

SAVEPOINT sp1;
来源：http://hz.feifeiyinyue.top/gteafpnhsd.html

ROLLBACK TO sp1;
来源：http://hz.gaohongyu789.top/gtrdnkwaoq.html

[Q69] 查看执行计划
来源：http://hz.redwolf501.top/gthaowhsut.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.hywenlv.cn/gtkgxjwvrp.html

[Q70] 更新统计信息
来源：http://hz.aibaodan.cn/gtqvxknyrn.html

ANALYZE TABLE users;
来源：http://hz.wangdashe.top/gtmshsxlpx.html

[Q71] 查看建表语句
来源：http://hz.ivvv.top/gtbpngjlzw.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.shuidangran.top/gtpiophvoj.html

[Q72] 查看索引
来源：http://hz.wangshuangyany.cn/gtilorrpvj.html

SHOW INDEX FROM users;
来源：http://hz.nanxuanxn.top/gtjecyjnqd.html

[Q73] 查看表状态
来源：http://hz.cucudq.cn/gtnrfvnhtn.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.ppjwa.cn/gttgnqiafn.html

[Q74] 强制使用索引
来源：http://hz.jinqigufen.top/gtkyljgkrj.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.yvedp.cn/gtgyurjjql.html

[Q75] 日期格式化
来源：http://hz.jinqigufen.top/gtwpcqncpd.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.yj20258.top/gtskhvldkr.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.kuanghao11.cn/gtppfojbyg.html

[Q76] 按天统计
来源：http://hz.cqqwz.cn/gthqskgkdt.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.zhongyouzk.top/gtgwmjvrdp.html

[Q77] 时间加减
来源：http://hz.hnxiangtu.top/gttqfppmtk.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.jinghuilouyu.cn/gtpfkenulk.html

[Q78] 当前时间
来源：http://hz.shangyingyoupin.top/gtdcxsjybj.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.wangshuangyany.cn/gteylwjdgh.html

[Q79] 字符串拼接
来源：http://hz.yueranfly.top/gtywoepjsj.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.shangyingyoupin.top/gtzvabbhet.html

[Q80] 字符串截取
来源：http://hz.svipenyu.cn/gthosagdgy.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.wangdashe.top/gtiqggchay.html

[Q81] 字符串替换
来源：http://hz.pycfn.com/gtyzlajlvl.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.jyoumei.cn/gtuntjwlsz.html

[Q82] 字符长度与字节长度
来源：http://hz.jyoumei.cn/gtdgbrmzwo.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.chenzaomai.com/gtyuvvflgs.html

[Q83] 大小写转换
来源：http://hz.yj20258888.top/gtodravucn.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.dianchejie.cn/gtkkpwfnsg.html

[Q84] 去除首尾空格
来源：http://hz.jinqigufen.top/gtrusvxjlw.html

SELECT TRIM(name) FROM users;
来源：http://hz.chenzaomai.com/gtjsrkoept.html

[Q85] 数值取整
来源：http://hz.zhiwuduotai.top/gtebdshnfn.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.shanyushiyangkeji.top/gtntwphlrq.html

[Q86] 读取 JSON 字段
来源：http://hz.chenlongwang.top/gtyfgptmwv.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.xinyue.icu/gtthumrriw.html

[Q87] JSON 字段做条件
来源：http://hz.ehwqpu.com/gtrutrguvx.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.hammf.cn/gtpjodvtgp.html

[Q88] 行转列（条件聚合）
来源：http://hz.mhx1999.top/gtyjtkhfea.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.wangdashe.top/gtpnbuihcw.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.hnqzz.top/gtgsjxbbpt.html

[Q89] 判断表是否存在
来源：http://hz.jqgfzy.top/gtifxtedhl.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.gzhubu.top/gtgehsfylr.html

[Q90] 生成序号列
来源：http://hz.zdqjudy.top/gtvwapimbd.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.iojbl.cn/gtoidelcak.html

================================================================================
来源：http://hz.jianghu66.top/gtsiiuiznl.html

R. Bash 专题
来源：http://hz.52xcode.cn/gtfvhhabgd.html

================================================================================
来源：http://hz.yj20258.top/gthtmeprtq.html

[R01] shebang 与严格模式
来源：http://hz.zhixingplan.top/gtuwsihorb.html

#!/usr/bin/env bash
来源：http://hz.birdmap.top/gtloygvcny.html

set -euo pipefail
来源：http://hz.kuanghao11.cn/gtkpfxiqxa.html

[R02] 变量赋值与使用
来源：http://hz.tanke756.top/gtrsahfjbd.html

name="Tom"; echo "$name"
来源：http://hz.zhaomingkeji.xyz/gtnagasjkt.html

[R03] 只读变量
来源：http://hz.tanke756.top/gtqrjtvocs.html

readonly PI=3.14
来源：http://hz.yj20258.top/gtvnzjzvlv.html

[R04] 位置参数
来源：http://hz.ywan-chungtsiang.top/gtinujxkws.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.chenlongwang.top/gtdxvjbgun.html

[R05] 参数默认值
来源：http://hz.ywan-chungtsiang.top/gttprhjzgk.html

name="${1:-default}"
来源：http://hz.xinyue.icu/gthgkyycbo.html

[R06] 判断命令是否存在
来源：http://hz.shangyingyoupin.top/gtbzvopmja.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.chenjidiqi.icu/gtagtdwqij.html

[R07] if 判断文件
来源：http://hz.xingfuxueyuan.xyz/gtiotmrgie.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.birdmap.top/gtvaemiyns.html

[R08] 数值比较
来源：http://hz.jianghu66.top/gtlzobnpww.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.kuanghao11.cn/gtfocwbsjq.html

[R09] 字符串比较
来源：http://hz.daxiang520.top/gtcudjobaq.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.guowangkeji.top/gterizgfij.html

[R10] 正则匹配
来源：http://hz.gaohongyu789.top/gtzpdlzizp.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.xziqi.cn/gtzjzgvzlo.html

[R11] case 多分支
来源：http://hz.quarkkingdee.top/gtafqsigli.html

case "$1" in
来源：http://hz.jianghu66.top/gtbhupmaqm.html

start) echo "启动" ;;
来源：http://hz.pycfn.com/gtxpmibqmi.html

stop)  echo "停止" ;;
来源：http://hz.redwolf501.top/gtoeakwsqv.html

*)     echo "未知命令" ;;
来源：http://hz.nanxinkj.top/gtlexuadna.html

esac
来源：http://hz.ehwqpu.com/gtievyffhr.html

[R12] for 遍历文件
来源：http://hz.hongshengwenyu.top/gtfjrvtqyj.html

for f in *.txt; do echo "$f"; done
来源：http://hz.haohaochexian.top/gtrzfyctqx.html

[R13] for 计数循环
来源：http://hz.hnxiangtu.top/gtewggvvxx.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.feifeiyinyue.top/gtggpbmnwy.html

[R14] C 风格 for
来源：http://hz.wangshuangyany.cn/gtrdesaumd.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.kuanghao11.cn/gtngcuchax.html

[R15] while 逐行读文件
来源：http://hz.nanxinkj.top/gtsshyzqdk.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.yuxming.cn/gtkpxlxyja.html

[R16] until 等待条件
来源：http://hz.nanxuanxn.top/gtlfrqudvn.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.dashuyun.cn/gtzxhdcxnd.html

[R17] 数组定义与取值
来源：http://hz.cdnleiting.top/gtgveymnit.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.xuetiantiany.cn/gtgrqyxncv.html

[R18] 遍历数组
来源：http://hz.shanyushiyangkeji.top/gtezgungah.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.jqgufenzy.top/gtwfrygcoo.html

[R19] 数组长度
来源：http://hz.xylfe.cn/gtqmirmuxz.html

echo "${#arr[@]}"
来源：http://hz.dianchejie.cn/gteqyovlpr.html

[R20] 关联数组（字典）
来源：http://hz.jinqigufen.top/gtbgfaadda.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.snrcjt.cn/gtfmaytosm.html

[R21] 字符串长度
来源：http://hz.jinqigufen.top/gtbkwqkbzw.html

echo "${#s}"
来源：http://hz.jinghuilouyu.cn/gtbwrsgbpj.html

[R22] 截取子串
来源：http://hz.svipenyu.cn/gtkcripmtc.html

echo "${s:0:5}"
来源：http://hz.zhongyouzk.top/gtjfpgmcln.html

[R23] 字符串替换
来源：http://hz.zhoulong.xyz/gtpxtgojbm.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.vqdsnc.cn/gtdfboxfvk.html

[R24] 大小写转换
来源：http://hz.zhiwuduotai.top/gtpuknhljd.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.fzhhl.top/gttnjwjhsv.html

[R25] 去后缀 / 去前缀
来源：http://hz.hnxiangtu.top/gtbmweosqk.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.aizwys.cn/gtodisgtmh.html

[R26] 命令替换
来源：http://hz.gaohongyu789.top/gtdintynvk.html

now=$(date +%F); echo "$now"
来源：http://hz.smart0.xyz/gtuyhkshwm.html

[R27] 算术展开
来源：http://hz.iojbl.cn/gtqsorxhok.html

echo $((1 + 2 * 3))
来源：http://hz.snrcjt.cn/gtijbzymbn.html

[R28] 浮点运算
来源：http://hz.jyoumei.cn/gtepidapzf.html

echo "scale=2; 10/3" | bc
来源：http://hz.zhixingplan.top/gtmliqpdxq.html

[R29] 定义函数
来源：http://hz.yueranfly.top/gtrxnmudpg.html


<!-- 参考信息 -->