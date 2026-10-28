代发 wailian999

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.yj20258888.top/gtzgslxkze.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.cheryme.top/gtufddhlze.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yuxming.cn/gtbdddkzgi.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.shanyushiyangtech.top/gtmoxcfscw.html

Java: list.size();  map.size();  s.length()
来源：http://hz.yangfankeji.com/gtynvkcwxr.html

Go:   len(arr);  len(m)
来源：http://hz.yuxming.cn/gtailwcyqq.html

Ruby: x.length;  x.size
来源：http://hz.hfpthk.cn/gtkylkwonl.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.316326.xyz/gtlrxcqilw.html

[P05] 判断两个对象内容是否相等
来源：http://hz.vqdsnc.cn/gtsbreepig.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.zhoulong.xyz/gtgfjscmkx.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.jinyuanbaomall.cn/gtfwwlwopv.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.xziqi.cn/gtkfjkmaiy.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.zdqjudy.top/gtfikuiwnn.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.yuanzhike.top/gtuokmttcv.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.shangyingyoupin.top/gtjvaeqfax.html

Ruby: a == b
来源：http://hz.tanke756.top/gtsvhljkti.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.hfpthk.cn/gtfcjgkbkx.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.sysykeji.top/gtedqkyygd.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.jiagoushi.top/gthkxvefdy.html

PHP:  if (empty($x)) {}
来源：http://hz.hnqzz.top/gtikirgaei.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.sxryk.cn/gtylqddqrf.html

TS:   if (x == null) {}
来源：http://hz.daria6918.cn/gtapvimhof.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.sufxvd.cn/gtnyagmvmb.html

Go:   if x == nil {}
来源：http://hz.chenlongwang.top/gtjmiulqpa.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.hammf.cn/gtejukxxfy.html

C#:   if (x is null) {}
来源：http://hz.tian-w.cn/gtucinfkew.html

[P07] 防抖与节流
来源：http://hz.guowangkeji.top/gtgdfekink.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.feifeiyinyue.top/gtzbhmnwug.html

PHP:  // 手写时间戳比较
来源：http://hz.zhongyouzk.top/gtezglsnlr.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.shangyingyoupin.top/gtbtjpeyvc.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.gotoacloud.top/gtiyrpcehs.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.hongshengwenyu.top/gtpvlgudrt.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.yj20258.top/gtgjvwmfih.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.zhoulong.xyz/gtltptdbtn.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.sufxvd.cn/gthazzumys.html

[P08] 处理浮点精度问题
来源：http://hz.daria6918.cn/gtrohzyygv.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.wangshuangyany.cn/gtucbkudsp.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.c1oappe.top/gtnsqvcckg.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.chenzaomai.com/gtkdzrcefv.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.jiagoushi.top/gtpvaewsxt.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.cashguo.top/gtmbiilgfw.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.cheryme.top/gtoyzubfej.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.cdnleiting.top/gtfwctqbme.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.tianlin.xyz/gtwmipexll.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtughwqdow.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.iojbl.cn/gtzxwkomlr.html

================================================================================
来源：http://hz.jqgfzy.top/gtfxutwbmn.html

[Q01] 创建表
来源：http://hz.havefunace.top/gtahwbikub.html

CREATE TABLE users (
来源：http://hz.redwolf501.top/gtwrogbyju.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.fengsongda.top/gtpxoygobq.html

name VARCHAR(50) NOT NULL,
来源：http://hz.dianchejie.cn/gtiuydbtdg.html

email VARCHAR(100) UNIQUE,
来源：http://hz.zhixingplan.top/gthqicwkpj.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.smart0.xyz/gtgpyqarwn.html

);
来源：http://hz.52xcode.cn/gtwjolhgnb.html

[Q02] 创建带外键的表
来源：http://hz.9152youxi.cn/gtvkatpflo.html

CREATE TABLE orders (
来源：http://hz.pengpengdd.cyou/gtyjnwqmqw.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.hnqzz.top/gtqlxekajb.html

user_id INT NOT NULL,
来源：http://hz.xziqi.cn/gtdhtgseym.html

amount DECIMAL(10, 2),
来源：http://hz.xylfe.cn/gtvdalqrej.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.xylfe.cn/gtwgwwbctf.html

);
来源：http://hz.gotoacloud.top/gtqxldrjsn.html

[Q03] 增加列
来源：http://hz.zhiwuduotai.top/gtjmtsakxc.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.bjfxy.top/gtdxhuflsq.html

[Q04] 修改列类型
来源：http://hz.haohaochexian.top/gtxmdjbavo.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.tanke756.top/gtnokrmwiq.html

[Q05] 重命名列
来源：http://hz.nanxinkj.top/gtrvlibipj.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.sysykeji.top/gtbeozvete.html

[Q06] 删除列
来源：http://hz.iojbl.cn/gtdqpvnhzk.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.xuanzx.com/gtqrtkghdo.html

[Q07] 删除表
来源：http://hz.fengsongda.top/gtqdovzxhz.html

DROP TABLE IF EXISTS orders;
来源：http://hz.xingfuxueyuan.xyz/gtdwdyirlz.html

[Q08] 创建普通索引
来源：http://hz.zhengqikj.top/gtktxmwiih.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.gogol.net.cn/gtzbkryuqr.html

[Q09] 创建唯一索引
来源：http://hz.ydzc1.top/gtfdaoxqoy.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.yongpay.top/gtahgypoof.html

[Q10] 插入单行
来源：http://hz.wangshuangyany.cn/gtsohxqlww.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.yj20258.top/gtfrlhqpag.html

[Q11] 一次插入多行
来源：http://hz.yonumen.top/gtfxfgqwcp.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.zhijiandao.cn/gtgangzrzo.html

[Q12] 插入后取自增 ID
来源：http://hz.tian-w.cn/gtsreyqrea.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.zycfv.cn/gtolgthfzs.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.yangfankeji.com/gtcbfygpbl.html

[Q13] 忽略重复插入
来源：http://hz.shzxlz.cn/gtakipvrad.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.tanke756.top/gtctbqfwtm.html

[Q14] 存在则更新（upsert）
来源：http://hz.wangshuangyany.cn/gthffujbjv.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.yj20258.top/gtxlpvjxzi.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.shuidangran.top/gtwrrkqfbg.html

[Q15] 查询全部
来源：http://hz.gogol.net.cn/gtpswhykei.html

SELECT * FROM users;
来源：http://hz.sxryk.cn/gtzwkjcwjv.html

[Q16] 查询指定列
来源：http://hz.yj20258888.top/gtsvuhgjxt.html

SELECT id, name FROM users;
来源：http://hz.9152youxi.cn/gtizfktzjz.html

[Q17] 条件查询
来源：http://hz.hnqzz.top/gtysiublhz.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.nwbrower.top/gtvyucltyg.html

[Q18] 模糊匹配
来源：http://hz.jyoumei.cn/gtakbxiuco.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.hnxiangtu.top/gtjnkaordz.html

[Q19] 范围查询
来源：http://hz.cucudq.cn/gtxmmvnfce.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.vqdsnc.cn/gtoufcfswx.html

[Q20] IN 列表
来源：http://hz.yongpay.top/gtykevnlbz.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.jlsjyb.cn/gtkdlxkmmv.html

[Q21] 空值判断
来源：http://hz.snrcjt.cn/gtwfwgslwx.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.shanyushiyangkeji.top/gtmaoywrnz.html

[Q22] 排序
来源：http://hz.shzxlz.cn/gtkvvuygmq.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.sufxvd.cn/gtgpiwndin.html

[Q23] 分页
来源：http://hz.dashuyun.cn/gtaahpuaia.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.316326.xyz/gtphoagesx.html

[Q24] 去重
来源：http://hz.nanxinkj.top/gtckasncyl.html

SELECT DISTINCT city FROM users;
来源：http://hz.gzhubu.top/gthlebknwf.html

[Q25] 只取前 N 条
来源：http://hz.yvedp.cn/gtqyodmnzo.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.ydzc1.top/gtcygpnpgm.html

[Q26] 计数
来源：http://hz.c1oappe.top/gtztxbtkwp.html

SELECT COUNT(*) FROM users;
来源：http://hz.pycfn.com/gtvjmjmhkd.html

[Q27] 条件计数
来源：http://hz.cheryme.top/gtdzmnauej.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.hnqzz.top/gtcysvefea.html

[Q28] 求和与平均
来源：http://hz.ydjk.org.cn/gtmmuhkbms.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.sysykeji.top/gtcczoexft.html

[Q29] 最大最小值
来源：http://hz.daria6918.cn/gtxpxwjeej.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.yj20258.top/gtegwoinau.html

[Q30] 分组统计
来源：http://hz.mhx1999.top/gtqyppocdj.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.cdnleiting.top/gtiwevuueq.html

[Q31] 分组后过滤
来源：http://hz.shanyushiyangtech.top/gtqgwubmvc.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.hysaishi.cn/gtmjnxgpre.html

[Q32] 分组拼接字符串
来源：http://hz.gzhubu.top/gtagnsnzqv.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.kuanghao11.cn/gtctumzzcl.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.c1oappe.top/gttnuxtncj.html

[Q33] 多列分组
来源：http://hz.jinqigufen.top/gtijhxdmqm.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.smart0.xyz/gtkzapfvql.html

[Q34] 每组取第一条
来源：http://hz.quarkkingdee.top/gtechhwfvc.html

SELECT * FROM (
来源：http://hz.jinyuanbaomall.cn/gtjhgmbfpv.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.9152youxi.cn/gtdjhohpcw.html

) t WHERE rn = 1;
来源：http://hz.haohaochexian.top/gtfxsvyjrs.html

[Q35] 内连接
来源：http://hz.cashguo.top/gtytmigbjb.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.gogol.net.cn/gtncexqrjl.html

[Q36] 左连接
来源：http://hz.xylfe.cn/gttkjxvzxd.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.svipenyu.cn/gtgfdcfzoj.html

[Q37] 右连接
来源：http://hz.jyoumei.cn/gtrzdwxwuw.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.hammf.cn/gtzzbmiwxh.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.aibaodan.cn/gtqxdvwchv.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.haohaochexian.top/gthilrwtge.html

[Q39] 自连接（查上下级）
来源：http://hz.hysaishi.cn/gtiacqtyxc.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.9152youxi.cn/gtxluxnlsf.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.ybcxt.top/gtnxyfbler.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.wangdashe.top/gtrzwsbobt.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.jinqigufen.top/gtyaiwnjjb.html

[Q41] 多表连接
来源：http://hz.jinghuilouyu.cn/gtzzidekuw.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.shuidangran.top/gtcowlptmf.html

JOIN users u ON u.id = o.user_id
来源：http://hz.meibo888.top/gtqycqjmzx.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.sysykeji.top/gtcrqcbswb.html

[Q42] 连接条件附加过滤
来源：http://hz.cheryme.top/gtmuzqujye.html

SELECT u.name, o.amount FROM users u
来源：http://hz.jinqigfzy.top/gtakwgmcep.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.9152youxi.cn/gtuwmolqah.html

[Q43] 标量子查询
来源：http://hz.tanke756.top/gtnafixmvq.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.xziqi.cn/gtegmtknjo.html

[Q44] IN 子查询
来源：http://hz.fengsongda.top/gtmpoafcga.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.hammf.cn/gtemhdnsks.html

[Q45] EXISTS 判断存在
来源：http://hz.aizwys.cn/gtvakacjza.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.hnxiangtu.top/gtogbbrsvm.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.ydjk.org.cn/gtxvykolzz.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.guowangkeji.top/gtvwkxyprl.html

[Q47] 与平均值比较
来源：http://hz.0kj1m.cn/gtfnyivueu.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.zhengqikj.top/gthecgvrco.html

[Q48] CTE 公用表表达式
来源：http://hz.jlsjyb.cn/gtpjlimaoi.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.nanxuanxn.top/gtuzihokxt.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.ywan-chungtsiang.top/gtdtdfasul.html

[Q49] 更新单行
来源：http://hz.yj20258.top/gtuoevnlrq.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.hfpthk.cn/gtxwwgrivn.html

[Q50] 批量更新
来源：http://hz.yvedp.cn/gtlvvnfrho.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.feifeiyinyue.top/gttpiqotdt.html

[Q51] 用子查询更新
来源：http://hz.yonumen.top/gtibmejnqj.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.ivvv.top/gtasnhiumu.html

[Q52] 删除指定行
来源：http://hz.chenzaomai.com/gtjwoepgak.html

DELETE FROM users WHERE id = 10;
来源：http://hz.yanxiufei.cn/gtotzdytvl.html

[Q53] 按条件删除
来源：http://hz.aizwys.cn/gtsrybwova.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.hnqzz.top/gtwqxzrjve.html

[Q54] 清空表
来源：http://hz.haohaochexian.top/gttwrjxckc.html

TRUNCATE TABLE logs;
来源：http://hz.jqgfzy.top/gtrdxvfwek.html

[Q55] 排名（并列占位）
来源：http://hz.gaohongyu789.top/gtpetbvtmo.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.cucudq.cn/gtqvverkdc.html

[Q56] 密集排名（并列不占位）
来源：http://hz.hywenlv.cn/gtbmzkxtaa.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.shuidangran.top/gtrywmaojx.html

[Q57] 行号
来源：http://hz.dianchejie.cn/gtxyrrdrda.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.shzxlz.cn/gtbthepvze.html

[Q58] 累计求和
来源：http://hz.jqgufenzy.top/gtlweftril.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.tanke756.top/gthshlnefp.html

[Q59] 分组内累计
来源：http://hz.sufxvd.cn/gtadbwjxsg.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.tian-w.cn/gtmzeoriwp.html

[Q60] 取上一行 / 下一行
来源：http://hz.dianchejie.cn/gtsaeawmvu.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.hnqzz.top/gttylawdqt.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.dianchejie.cn/gtsggzdlen.html

[Q61] 移动平均
来源：http://hz.jqgfzy.top/gtvaikpbfj.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.sufxvd.cn/gtzluitkwd.html

[Q62] 分组占比
来源：http://hz.svipenyu.cn/gtmntljhrh.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.zhijiandao.cn/gtfgvbveaf.html

[Q63] 开启事务
来源：http://hz.zycfv.cn/gtagsibwxn.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.yj20258.top/gtbrbodrlv.html

[Q64] 提交事务
来源：http://hz.hywenlv.cn/gtowrwbfdn.html

COMMIT;
来源：http://hz.daxiang520.top/gtraffyhqg.html

[Q65] 回滚事务
来源：http://hz.ydzc1.top/gtgtxfmkgo.html

ROLLBACK;
来源：http://hz.svipenyu.cn/gtozegohme.html

[Q66] 行锁查询
来源：http://hz.shzxlz.cn/gtjjpqohpl.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.ybcxt.top/gtlephhfrg.html

[Q67] 设置隔离级别
来源：http://hz.9152youxi.cn/gtqltehnbz.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.quarkkingdee.top/gtqviisqyw.html

[Q68] 保存点
来源：http://hz.hysaishi.cn/gtspjujyhh.html

SAVEPOINT sp1;
来源：http://hz.aibaodan.cn/gtykpqivyj.html

ROLLBACK TO sp1;
来源：http://hz.gaohongyu789.top/gtueiqcwny.html

[Q69] 查看执行计划
来源：http://hz.yuanzhike.top/gthczbwjsh.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.tanke756.top/gtuiifllxu.html

[Q70] 更新统计信息
来源：http://hz.yj20258.top/gthxbrghqg.html

ANALYZE TABLE users;
来源：http://hz.daria6918.cn/gtudllrbrm.html

[Q71] 查看建表语句
来源：http://hz.meibo888.top/gtjcyimtzh.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.fzhhl.top/gtynecvjbf.html

[Q72] 查看索引
来源：http://hz.fzhhl.top/gtvgstrcqr.html

SHOW INDEX FROM users;
来源：http://hz.aizwys.cn/gtpwmarxfa.html

[Q73] 查看表状态
来源：http://hz.sufxvd.cn/gtlwdlvnix.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.fengsongda.top/gtznsicdob.html

[Q74] 强制使用索引
来源：http://hz.yvedp.cn/gtpunncemf.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.chenjidiqi.icu/gtyihznogf.html

[Q75] 日期格式化
来源：http://hz.yvedp.cn/gtrepanezf.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.zhengqikj.top/gtqkrpyalh.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.gotoacloud.top/gttsxbhhgc.html

[Q76] 按天统计
来源：http://hz.yueranfly.top/gtqdcwiqfb.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.tanke756.top/gtjxvztnxt.html

[Q77] 时间加减
来源：http://hz.gzhubu.top/gtfglpqhoz.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.daxiang520.top/gtealfeeel.html

[Q78] 当前时间
来源：http://hz.tanke756.top/gtxdstckxz.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.ybcxt.top/gtykffbeym.html

[Q79] 字符串拼接
来源：http://hz.mhx1999.top/gtigvfbfxi.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.redwolf501.top/gtfhyusmoi.html

[Q80] 字符串截取
来源：http://hz.316326.xyz/gtzyoydugh.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.jyoumei.cn/gtegzkrtgx.html

[Q81] 字符串替换
来源：http://hz.316326.xyz/gtmfzuatts.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.yj202588.top/gtkdysozui.html

[Q82] 字符长度与字节长度
来源：http://hz.chenjidiqi.icu/gtksdrirpb.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.sxryk.cn/gtymnklnzk.html

[Q83] 大小写转换
来源：http://hz.snrcjt.cn/gtcoxubtju.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.yj20258.top/gtovzsakkt.html

[Q84] 去除首尾空格
来源：http://hz.pengpengdd.cyou/gtsrhzvhkt.html

SELECT TRIM(name) FROM users;
来源：http://hz.jinqigfzy.top/gtvfpozctk.html

[Q85] 数值取整
来源：http://hz.tianlin.xyz/gtgzjdhyty.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.yj20258888.top/gtyfvqdvll.html

[Q86] 读取 JSON 字段
来源：http://hz.wangdashe.top/gtoyxtpedh.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.zhiwuduotai.top/gtzisfqncn.html

[Q87] JSON 字段做条件
来源：http://hz.dashuyun.cn/gtmdwulwhy.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.yonumen.top/gtuopcwsea.html

[Q88] 行转列（条件聚合）
来源：http://hz.ehwqpu.com/gtozmqlnmr.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.nwbrower.top/gtsrytvjqf.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.gaohongyu789.top/gtheyuufrw.html

[Q89] 判断表是否存在
来源：http://hz.nwbrower.top/gtsvqyahlg.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.ybcxt.top/gtlvypephl.html

[Q90] 生成序号列
来源：http://hz.hammf.cn/gtvixripbn.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.jiagoushi.top/gtoyqlenig.html

================================================================================
来源：http://hz.snrcjt.cn/gthlzkdncb.html

R. Bash 专题
来源：http://hz.mhx1999.top/gtfscpopoy.html

================================================================================
来源：http://hz.xziqi.cn/gtshfczull.html

[R01] shebang 与严格模式
来源：http://hz.fengsongda.top/gtbapdldtu.html

#!/usr/bin/env bash
来源：http://hz.nanxinkj.top/gtsaghluls.html

set -euo pipefail
来源：http://hz.yonumen.top/gtzvhakvcl.html

[R02] 变量赋值与使用
来源：http://hz.zhiwuduotai.top/gtoepsfwul.html

name="Tom"; echo "$name"
来源：http://hz.ivvv.top/gtdmxztjal.html

[R03] 只读变量
来源：http://hz.svipenyu.cn/gtirlrabso.html

readonly PI=3.14
来源：http://hz.jlsjyb.cn/gtsgfpweli.html

[R04] 位置参数
来源：http://hz.hfpthk.cn/gtaetvxmxg.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.fengsongda.top/gtvbcbyjho.html

[R05] 参数默认值
来源：http://hz.quarkkingdee.top/gtdvxbhdby.html

name="${1:-default}"
来源：http://hz.chenlongwang.top/gtfhaltvzg.html

[R06] 判断命令是否存在
来源：http://hz.wangdashe.top/gtlzlzwskb.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.ydzc1.top/gtrkifrrem.html

[R07] if 判断文件
来源：http://hz.dianchejie.cn/gtbljwdvai.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.ywan-chungtsiang.top/gtwwgrfcvr.html

[R08] 数值比较
来源：http://hz.yuanzhike.top/gtlwycmkyd.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.xylfe.cn/gtzdximgyb.html

[R09] 字符串比较
来源：http://hz.zycfv.cn/gtcufbqlqf.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.zhiwuduotai.top/gtgoakhnvc.html

[R10] 正则匹配
来源：http://hz.0kj1m.cn/gttkquogrv.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.jyoumei.cn/gtkjhlwdht.html

[R11] case 多分支
来源：http://hz.meibo888.top/gtdnhshpwj.html

case "$1" in
来源：http://hz.daxiang520.top/gtdknqezxe.html

start) echo "启动" ;;
来源：http://hz.meibo888.top/gtgqzylzkl.html

stop)  echo "停止" ;;
来源：http://hz.fengsongda.top/gtwajazhnn.html

*)     echo "未知命令" ;;
来源：http://hz.iojbl.cn/gtmfrnpvzn.html

esac
来源：http://hz.fzhhl.top/gtznwgakyf.html

[R12] for 遍历文件
来源：http://hz.aibaodan.cn/gtjcutemaz.html

for f in *.txt; do echo "$f"; done
来源：http://hz.sysykeji.top/gtublmlotn.html

[R13] for 计数循环
来源：http://hz.birdmap.top/gtocucazzs.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.feifeiyinyue.top/gtyjwfymyg.html

[R14] C 风格 for
来源：http://hz.quarkkingdee.top/gtkfmqujqa.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.ppjwa.cn/gtgrtwspcx.html

[R15] while 逐行读文件
来源：http://hz.snrcjt.cn/gtjxezqxqn.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.jiagoushi.top/gtjlxuutxm.html

[R16] until 等待条件
来源：http://hz.ybcxt.top/gtpzifmztb.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.ydjk.org.cn/gtkizqniia.html

[R17] 数组定义与取值
来源：http://hz.tian-w.cn/gtccqnumpl.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.dashuyun.cn/gtjgsreooa.html

[R18] 遍历数组
来源：http://hz.nanxinkj.top/gtekmcarwq.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.tian-w.cn/gtgwnvxcti.html

[R19] 数组长度
来源：http://hz.jqgufenzy.top/gtkwrahkod.html

echo "${#arr[@]}"
来源：http://hz.zhengqikj.top/gtueqwzrhy.html

[R20] 关联数组（字典）
来源：http://hz.meibo888.top/gtyzzzrfis.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.52xcode.cn/gtxdvenztb.html

[R21] 字符串长度
来源：http://hz.jqgfzy.top/gtariehjqc.html


<!-- 参考信息 -->