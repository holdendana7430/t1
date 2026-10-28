代发 wailian999

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.jqgfzy.top/gtjygirxco.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.meibo888.top/gtosvmcirc.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.ehwqpu.com/gtczsmueji.html

PHP:  if (empty($x)) {}
来源：http://hz.hywenlv.cn/gtjchtfhyj.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.kuanghao11.cn/gtwnaqflku.html

TS:   if (x == null) {}
来源：http://hz.jinqigufen.top/gtlhlsiobz.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.havefunace.top/gtvjoaagsi.html

Go:   if x == nil {}
来源：http://hz.andypj.xyz/gtzkiyqmaq.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.aizwys.cn/gtsgudnins.html

C#:   if (x is null) {}
来源：http://hz.gzhubu.top/gtnnhszpcd.html

[P07] 防抖与节流
来源：http://hz.guannengcc.top/gtozdqizox.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.zhaomingkeji.xyz/gtajqmzqaa.html

PHP:  // 手写时间戳比较
来源：http://hz.jinqigfzy.top/gtjkljemsy.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.xylfe.cn/gteqmytmxf.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yj20258888.top/gtrozdvkbe.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.redwolf501.top/gtdixgnvdb.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.shanyushiyangtech.top/gtrbqnaucz.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.redwolf501.top/gtfbiqhnsi.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.xuanzx.com/gtdbshrhdz.html

[P08] 处理浮点精度问题
来源：http://hz.shuidangran.top/gtbqypbmiz.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.nanxinkj.top/gtokkcansa.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.yangfankeji.com/gtemubocag.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.wangdashe.top/gtbcohmudw.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.shanyushiyangkeji.top/gtaxtgemnm.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.hfpthk.cn/gtcplqwcfw.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.52xcode.cn/gtlonsivmq.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.nanxinkj.top/gttrqtjeke.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.hnqzz.top/gtwrmeqiij.html

================================================================================
来源：http://hz.cashguo.top/gtxpupzcyd.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.shanyushiyangtech.top/gtmxldiiqe.html

================================================================================
来源：http://hz.quarkkingdee.top/gtgjyaazyb.html

[Q01] 创建表
来源：http://hz.wangdashe.top/gtwqgvysgn.html

CREATE TABLE users (
来源：http://hz.daria6918.cn/gtsgjbibkx.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.sufxvd.cn/gtyqjmpejy.html

name VARCHAR(50) NOT NULL,
来源：http://hz.daria6918.cn/gtmikuxead.html

email VARCHAR(100) UNIQUE,
来源：http://hz.shangyingyoupin.top/gtbjdmswki.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.nanxinkj.top/gtngzkabdh.html

);
来源：http://hz.chenzaomai.com/gtyiqeeooa.html

[Q02] 创建带外键的表
来源：http://hz.yonumen.top/gthevrxvyw.html

CREATE TABLE orders (
来源：http://hz.sweek.top/gtiasgryrj.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.sufxvd.cn/gtftbyqmpd.html

user_id INT NOT NULL,
来源：http://hz.guannengcc.top/gtncriucde.html

amount DECIMAL(10, 2),
来源：http://hz.9152youxi.cn/gtbdinysws.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.shanyushiyangtech.top/gtucbnnpqa.html

);
来源：http://hz.gzhubu.top/gtxxdnltad.html

[Q03] 增加列
来源：http://hz.zhixingplan.top/gthyyvmtrm.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.zycfv.cn/gtcdymxihw.html

[Q04] 修改列类型
来源：http://hz.xinyue.icu/gtulxehyhv.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.ppjwa.cn/gtxxwfhdfq.html

[Q05] 重命名列
来源：http://hz.jianghu66.top/gttkxthigi.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.daxiang520.top/gtmjwbdymi.html

[Q06] 删除列
来源：http://hz.bjfxy.top/gtxrnevcvd.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.316326.xyz/gtrywraykf.html

[Q07] 删除表
来源：http://hz.chenzaomai.com/gtntwtjpcb.html

DROP TABLE IF EXISTS orders;
来源：http://hz.nanxuanxn.top/gtrobksucb.html

[Q08] 创建普通索引
来源：http://hz.hysaishi.cn/gtmxlcoudy.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.hywenlv.cn/gtmjuoeiox.html

[Q09] 创建唯一索引
来源：http://hz.dianchejie.cn/gtsjqyfzkm.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.birdmap.top/gtjxkjrnmn.html

[Q10] 插入单行
来源：http://hz.vqdsnc.cn/gtuiyriygx.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.yuanzhike.top/gtsmmckmir.html

[Q11] 一次插入多行
来源：http://hz.xingfuxueyuan.xyz/gthduixqtc.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.xylfe.cn/gtcgrxmonx.html

[Q12] 插入后取自增 ID
来源：http://hz.cdnleiting.top/gtoaxygqbv.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.yj202588.top/gttqhnfscx.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.gaohongyu789.top/gtyalaplzl.html

[Q13] 忽略重复插入
来源：http://hz.ppjwa.cn/gtvsxhnjce.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.52xcode.cn/gtiwsoxbyd.html

[Q14] 存在则更新（upsert）
来源：http://hz.sweek.top/gtssrnzgtw.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.316326.xyz/gtcqfaexvz.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.hnqzz.top/gthhdotoso.html

[Q15] 查询全部
来源：http://hz.cashguo.top/gtowymetqc.html

SELECT * FROM users;
来源：http://hz.yangfankeji.com/gtscszkygf.html

[Q16] 查询指定列
来源：http://hz.chenlongwang.top/gtojztactz.html

SELECT id, name FROM users;
来源：http://hz.0kj1m.cn/gttpeaayxr.html

[Q17] 条件查询
来源：http://hz.shanyushiyangkeji.top/gtuoafpdkt.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.hfpthk.cn/gtciomuznx.html

[Q18] 模糊匹配
来源：http://hz.yvedp.cn/gttvbpfesy.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.ppjwa.cn/gtdqnjkmhr.html

[Q19] 范围查询
来源：http://hz.guannengcc.top/gtdwhnpljf.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.shangyingyoupin.top/gtbvfzxxht.html

[Q20] IN 列表
来源：http://hz.hfpthk.cn/gtneagtswu.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.redwolf501.top/gtlbeqnbwp.html

[Q21] 空值判断
来源：http://hz.sufxvd.cn/gtnsnhqtas.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.svipenyu.cn/gtxnmquqeb.html

[Q22] 排序
来源：http://hz.dianchejie.cn/gtpknhkmzs.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.zhijiandao.cn/gtpiwfhvuv.html

[Q23] 分页
来源：http://hz.tanke756.top/gttoyloanz.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.chenlongwang.top/gtebsingco.html

[Q24] 去重
来源：http://hz.shzxlz.cn/gtwvkwavur.html

SELECT DISTINCT city FROM users;
来源：http://hz.yuanzhike.top/gtedenvwkl.html

[Q25] 只取前 N 条
来源：http://hz.xylfe.cn/gtmyjxcvsy.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.zdqjudy.top/gtqjnjuylm.html

[Q26] 计数
来源：http://hz.gogol.net.cn/gtkgwoeyjs.html

SELECT COUNT(*) FROM users;
来源：http://hz.shzxlz.cn/gtylodpnbd.html

[Q27] 条件计数
来源：http://hz.wangshuangyany.cn/gtcupkkhsq.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.gaohongyu789.top/gtbhrgqora.html

[Q28] 求和与平均
来源：http://hz.xylfe.cn/gtgufkjoqn.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.xuanzx.com/gtrwdvrpbs.html

[Q29] 最大最小值
来源：http://hz.yvedp.cn/gttvearrbv.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.xingfuxueyuan.xyz/gtvuxxyutm.html

[Q30] 分组统计
来源：http://hz.jlsjyb.cn/gtwbceprvy.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.kuanghao11.cn/gtcdtgzsqm.html

[Q31] 分组后过滤
来源：http://hz.nwbrower.top/gtojqlfxsb.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.redwolf501.top/gtjldcpzqp.html

[Q32] 分组拼接字符串
来源：http://hz.vqdsnc.cn/gtnukrujpb.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.pengpengdd.cyou/gtetmslpor.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.tian-w.cn/gtveylwtyk.html

[Q33] 多列分组
来源：http://hz.tanke756.top/gtqupvhfxk.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.havefunace.top/gtjduavqyh.html

[Q34] 每组取第一条
来源：http://hz.yuanzhike.top/gttmplbfjh.html

SELECT * FROM (
来源：http://hz.hysaishi.cn/gtpxxdkdzt.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.tian-w.cn/gtzrjlqcwy.html

) t WHERE rn = 1;
来源：http://hz.ydzc1.top/gtdtxpkxay.html

[Q35] 内连接
来源：http://hz.kuanghao11.cn/gtqptujbmt.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.fzhhl.top/gtiegaqzby.html

[Q36] 左连接
来源：http://hz.fengsongda.top/gttrxcqeqm.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.ywan-chungtsiang.top/gtrbcpduxr.html

[Q37] 右连接
来源：http://hz.zycfv.cn/gtdfouetvv.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.yueranfly.top/gtttotlzpz.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.sysykeji.top/gtzhasrdbe.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.cucudq.cn/gtabrmztus.html

[Q39] 自连接（查上下级）
来源：http://hz.jianghu66.top/gtinoneyur.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.birdmap.top/gtrhmskwpr.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.sysykeji.top/gtsuwvlfqs.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.gaohongyu789.top/gtyqttapmm.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.svipenyu.cn/gtmkqmfacu.html

[Q41] 多表连接
来源：http://hz.jyoumei.cn/gtkuydwixa.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.jinghuilouyu.cn/gtditjzmhk.html

JOIN users u ON u.id = o.user_id
来源：http://hz.daxiang520.top/gtozgfpgsy.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.mhx1999.top/gtguguotkb.html

[Q42] 连接条件附加过滤
来源：http://hz.jinqigufen.top/gtijkvgxxt.html

SELECT u.name, o.amount FROM users u
来源：http://hz.shuidangran.top/gtjjlqmkao.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.chenzaomai.com/gtgjiklifj.html

[Q43] 标量子查询
来源：http://hz.ydjk.org.cn/gtdudvqfgf.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.yonumen.top/gtzasilibo.html

[Q44] IN 子查询
来源：http://hz.smart0.xyz/gtjhbcryrk.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.tanke756.top/gtcnbyfsab.html

[Q45] EXISTS 判断存在
来源：http://hz.chenzaomai.com/gtgtscmiwv.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.ehwqpu.com/gtnvbdfnrt.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.aizwys.cn/gtqcdzmdwt.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.dashuyun.cn/gtyweevolk.html

[Q47] 与平均值比较
来源：http://hz.daria6918.cn/gtbpyfoacr.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.sufxvd.cn/gtyeplddkx.html

[Q48] CTE 公用表表达式
来源：http://hz.ybcxt.top/gtmychgeum.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.cqqwz.cn/gtigfqpvou.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.xingfuxueyuan.xyz/gtrcvzphdj.html

[Q49] 更新单行
来源：http://hz.meibo888.top/gtrzidgyzu.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.yanxiufei.cn/gtpxsfkrqv.html

[Q50] 批量更新
来源：http://hz.jinqigfzy.top/gtlgclbawz.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.gogol.net.cn/gtsrsfcimi.html

[Q51] 用子查询更新
来源：http://hz.yonumen.top/gthfksbina.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.quarkkingdee.top/gtxzosbsdv.html

[Q52] 删除指定行
来源：http://hz.zhiwuduotai.top/gtrkczuuwx.html

DELETE FROM users WHERE id = 10;
来源：http://hz.hongshengwenyu.top/gtayabsjdo.html

[Q53] 按条件删除
来源：http://hz.daria6918.cn/gtnuswogwe.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.ppjwa.cn/gtyzeigadz.html

[Q54] 清空表
来源：http://hz.hfpthk.cn/gtscwvbyxa.html

TRUNCATE TABLE logs;
来源：http://hz.pengpengdd.cyou/gtrbjvkkqk.html

[Q55] 排名（并列占位）
来源：http://hz.ydjk.org.cn/gteelamqwh.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.nwbrower.top/gtgkquieop.html

[Q56] 密集排名（并列不占位）
来源：http://hz.shangyingyoupin.top/gtfwlwkebn.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.jlsjyb.cn/gtibbwmkyc.html

[Q57] 行号
来源：http://hz.zhijiandao.cn/gtrhavbodd.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.52xcode.cn/gttdhqekjz.html

[Q58] 累计求和
来源：http://hz.yj20258888.top/gtxibkrkwu.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.iojbl.cn/gtwkucxrlh.html

[Q59] 分组内累计
来源：http://hz.shanyushiyangtech.top/gtxazdbfks.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.jinghuilouyu.cn/gtkfjydhwf.html

[Q60] 取上一行 / 下一行
来源：http://hz.zhaomingkeji.xyz/gtgihtheld.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.jianghu66.top/gtvlubgnzq.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.wangshuangyany.cn/gtracyliff.html

[Q61] 移动平均
来源：http://hz.aizwys.cn/gtmtiucxsi.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.ppjwa.cn/gtjtsgexus.html

[Q62] 分组占比
来源：http://hz.zdqjudy.top/gtubdztzoe.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.xingfuxueyuan.xyz/gtamndxlly.html

[Q63] 开启事务
来源：http://hz.zhongyouzk.top/gtrdsfpbud.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.xziqi.cn/gtxuaoyazc.html

[Q64] 提交事务
来源：http://hz.hnxiangtu.top/gtjketrmte.html

COMMIT;
来源：http://hz.yuanzhike.top/gtuviootal.html

[Q65] 回滚事务
来源：http://hz.cqqwz.cn/gtgyboqexm.html

ROLLBACK;
来源：http://hz.ppjwa.cn/gtuquzwaui.html

[Q66] 行锁查询
来源：http://hz.nwbrower.top/gtzscxuasj.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.vqdsnc.cn/gtvyhaqenb.html

[Q67] 设置隔离级别
来源：http://hz.zhixingplan.top/gthurmtuqi.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.hfpthk.cn/gtijihfmhh.html

[Q68] 保存点
来源：http://hz.nwbrower.top/gthkvayrqb.html

SAVEPOINT sp1;
来源：http://hz.yj20258888.top/gtoghsmalf.html

ROLLBACK TO sp1;
来源：http://hz.dianchejie.cn/gtvhvmnlsm.html

[Q69] 查看执行计划
来源：http://hz.guowangkeji.top/gtkbyvgzuq.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.jqgufenzy.top/gtndxpesnw.html

[Q70] 更新统计信息
来源：http://hz.bjfxy.top/gtsfwhkzuo.html

ANALYZE TABLE users;
来源：http://hz.yuanzhike.top/gthzghznsb.html

[Q71] 查看建表语句
来源：http://hz.aibaodan.cn/gtbrzwnafv.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.kuanghao11.cn/gttgwrzyca.html

[Q72] 查看索引
来源：http://hz.hfpthk.cn/gtsdeflesa.html

SHOW INDEX FROM users;
来源：http://hz.tianlin.xyz/gtewbakdka.html

[Q73] 查看表状态
来源：http://hz.jinyuanbaomall.cn/gtaxfoestc.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.xziqi.cn/gtmxuhpgls.html

[Q74] 强制使用索引
来源：http://hz.smart0.xyz/gthzambany.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.hnxiangtu.top/gtiuccushc.html

[Q75] 日期格式化
来源：http://hz.ydjk.org.cn/gtdzapbcqh.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.xinyue.icu/gtnlzaagdc.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.gogol.net.cn/gtgmeqbtoq.html

[Q76] 按天统计
来源：http://hz.wangshuangyany.cn/gtuclboaes.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.aizwys.cn/gtoarynoic.html

[Q77] 时间加减
来源：http://hz.tianlin.xyz/gtwailzmuk.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.jinghuilouyu.cn/gtcndnmzkj.html

[Q78] 当前时间
来源：http://hz.snrcjt.cn/gtsibfwnct.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.jinqigfzy.top/gtisxrilog.html

[Q79] 字符串拼接
来源：http://hz.xuetiantiany.cn/gtxdlxpxcu.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.c1oappe.top/gtfgskcbbx.html

[Q80] 字符串截取
来源：http://hz.nanxinkj.top/gtvjwqowgm.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.yuxming.cn/gtknkurtiy.html

[Q81] 字符串替换
来源：http://hz.nwbrower.top/gtrigzzcbx.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.mhx1999.top/gtlgtwzaqz.html

[Q82] 字符长度与字节长度
来源：http://hz.ybcxt.top/gtrgcxbeum.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.jinyuanbaomall.cn/gteqbsltcd.html

[Q83] 大小写转换
来源：http://hz.hfpthk.cn/gtoxrsvrsb.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.gzhubu.top/gtoohvelqr.html

[Q84] 去除首尾空格
来源：http://hz.xingfuxueyuan.xyz/gtznsauiln.html

SELECT TRIM(name) FROM users;
来源：http://hz.yueranfly.top/gtgvrlujcq.html

[Q85] 数值取整
来源：http://hz.mhx1999.top/gtkrjdsaxf.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.zhiwuduotai.top/gtxhxycqdr.html

[Q86] 读取 JSON 字段
来源：http://hz.ybcxt.top/gtvzmvjnrp.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.cheryme.top/gtrioykbpg.html

[Q87] JSON 字段做条件
来源：http://hz.yj20258.top/gtxjfzvzbp.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.yangfankeji.com/gtcrlzqkzn.html

[Q88] 行转列（条件聚合）
来源：http://hz.tanke756.top/gtanamwijt.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.hongshengwenyu.top/gtelyauhqc.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.jianghu66.top/gtbhwjekzb.html

[Q89] 判断表是否存在
来源：http://hz.cashguo.top/gthzeansbm.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.cqqwz.cn/gtkushcfjc.html

[Q90] 生成序号列
来源：http://hz.shanyushiyangtech.top/gtrxwygwim.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.wangdashe.top/gtcvtzhlka.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtwvcpotbl.html

R. Bash 专题
来源：http://hz.wangdashe.top/gtnnkxzphn.html

================================================================================
来源：http://hz.0kj1m.cn/gtvcoclglh.html

[R01] shebang 与严格模式
来源：http://hz.xziqi.cn/gtrxnadwqd.html

#!/usr/bin/env bash
来源：http://hz.ppjwa.cn/gtnosmmhhj.html

set -euo pipefail
来源：http://hz.aibaodan.cn/gtzntukqxr.html

[R02] 变量赋值与使用
来源：http://hz.zycfv.cn/gtvswiybcw.html

name="Tom"; echo "$name"
来源：http://hz.daxiang520.top/gtvczfkroo.html

[R03] 只读变量
来源：http://hz.ydjk.org.cn/gtejgmgemt.html

readonly PI=3.14
来源：http://hz.jinqigufen.top/gtmjhmxjue.html

[R04] 位置参数
来源：http://hz.cashguo.top/gtyfkyikxd.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.jqgufenzy.top/gtxkslvscf.html

[R05] 参数默认值
来源：http://hz.kuanghao11.cn/gtglcoohqv.html

name="${1:-default}"
来源：http://hz.ybcxt.top/gtdtrzsreq.html

[R06] 判断命令是否存在
来源：http://hz.jianghu66.top/gtkbmdlhnn.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.guowangkeji.top/gtrnbdnpey.html

[R07] if 判断文件
来源：http://hz.ybcxt.top/gtlaifrmme.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.fengsongda.top/gtjxtjojdr.html

[R08] 数值比较
来源：http://hz.smart0.xyz/gtmnmyhodx.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.guannengcc.top/gtnqlnncvj.html

[R09] 字符串比较
来源：http://hz.tianlin.xyz/gtbddogvop.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.hywenlv.cn/gtyysdbtzj.html

[R10] 正则匹配
来源：http://hz.wangdashe.top/gtuiizdwjh.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.wangdashe.top/gtfomabnjd.html

[R11] case 多分支
来源：http://hz.fzhhl.top/gtrmmpwhar.html

case "$1" in
来源：http://hz.fengsongda.top/gtbvcisluy.html

start) echo "启动" ;;
来源：http://hz.yj20258888.top/gtvpqfaggo.html

stop)  echo "停止" ;;
来源：http://hz.jinqigufen.top/gtsowlfplk.html

*)     echo "未知命令" ;;
来源：http://hz.sweek.top/gtbjkqfsvy.html

esac
来源：http://hz.smart0.xyz/gtqzvazqpz.html

[R12] for 遍历文件
来源：http://hz.zhijiandao.cn/gtsojkbqms.html

for f in *.txt; do echo "$f"; done
来源：http://hz.jianghu66.top/gtzzahkenr.html

[R13] for 计数循环
来源：http://hz.cqqwz.cn/gtercxubgo.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.meibo888.top/gtdsrfksvt.html

[R14] C 风格 for
来源：http://hz.yueranfly.top/gtpdnluntm.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.xylfe.cn/gtdflgmyhw.html

[R15] while 逐行读文件
来源：http://hz.nanxinkj.top/gtgzvjgfjp.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.yuanzhike.top/gtnzfdgngl.html

[R16] until 等待条件
来源：http://hz.daxiang520.top/gtpqqlpsbx.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.jianghu66.top/gtgsqhatdv.html

[R17] 数组定义与取值
来源：http://hz.shzxlz.cn/gtubgmbddr.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.shanyushiyangkeji.top/gttghkzves.html

[R18] 遍历数组
来源：http://hz.jlsjyb.cn/gtkrfzqfve.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.gogol.net.cn/gtfqmlkwjn.html

[R19] 数组长度
来源：http://hz.cqqwz.cn/gtsopsswmf.html

echo "${#arr[@]}"
来源：http://hz.ydzc1.top/gteahskuuc.html

[R20] 关联数组（字典）
来源：http://hz.xylfe.cn/gtoktqvchb.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.tianlin.xyz/gtsqfnwvcy.html

[R21] 字符串长度
来源：http://hz.iojbl.cn/gtvglnxydt.html

echo "${#s}"
来源：http://hz.9152youxi.cn/gtnciekbqi.html

[R22] 截取子串
来源：http://hz.yangfankeji.com/gtzorglgiy.html

echo "${s:0:5}"
来源：http://hz.xingfuxueyuan.xyz/gtniykeffj.html

[R23] 字符串替换
来源：http://hz.jianghu66.top/gtqhrpssqi.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.fengsongda.top/gtjreolscz.html

[R24] 大小写转换
来源：http://hz.guannengcc.top/gtmmjxwhed.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.pycfn.com/gtddkcliin.html

[R25] 去后缀 / 去前缀
来源：http://hz.yueranfly.top/gtiijecbhz.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.yuanzhike.top/gtkysesmqy.html

[R26] 命令替换
来源：http://hz.aizwys.cn/gttmhsjadj.html

now=$(date +%F); echo "$now"
来源：http://hz.daxiang520.top/gtafbzpwwa.html

[R27] 算术展开
来源：http://hz.yj202588.top/gtabdniapj.html

echo $((1 + 2 * 3))
来源：http://hz.9152youxi.cn/gtlrvuspkb.html

[R28] 浮点运算
来源：http://hz.shzxlz.cn/gtctktsaom.html

echo "scale=2; 10/3" | bc
来源：http://hz.zycfv.cn/gtknjyycpi.html

[R29] 定义函数
来源：http://hz.mhx1999.top/gthzzhozdi.html


<!-- 参考信息 -->