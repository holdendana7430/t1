代发 wailian999

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.gogol.net.cn/gtsiqwubds.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.jinyuanbaomall.cn/gtotesvwls.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.shzxlz.cn/gtqoqaphxc.html

[P04] 求长度
来源：http://hz.zycfv.cn/gtenktjcez.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.havefunace.top/gtxxjbubje.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.redwolf501.top/gtnhfocxhe.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.svipenyu.cn/gtkosbcplm.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yvedp.cn/gtolqredac.html

Java: list.size();  map.size();  s.length()
来源：http://hz.andypj.xyz/gtyglpckok.html

Go:   len(arr);  len(m)
来源：http://hz.hysaishi.cn/gtljpbbule.html

Ruby: x.length;  x.size
来源：http://hz.ivvv.top/gtzvoqjeeb.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.sweek.top/gtsjwweisn.html

[P05] 判断两个对象内容是否相等
来源：http://hz.redwolf501.top/gtyyizltvt.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.sysykeji.top/gtyrvshfcy.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.sxryk.cn/gtefgzstgf.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.cqqwz.cn/gtobujzhfs.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.aibaodan.cn/gtouqtyldz.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.hammf.cn/gtnkyhtjqg.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.bjfxy.top/gtpthxrbny.html

Ruby: a == b
来源：http://hz.fengsongda.top/gtslwlcgqf.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.wangshuangyany.cn/gttkmioeow.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.jinyuanbaomall.cn/gtwzfxtgiw.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.9152youxi.cn/gttbzbvtae.html

PHP:  if (empty($x)) {}
来源：http://hz.xziqi.cn/gtvwnodbhi.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.dianchejie.cn/gtzivleypu.html

TS:   if (x == null) {}
来源：http://hz.ehwqpu.com/gtdhuhuvlu.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.shangyingyoupin.top/gtmmtxfuvc.html

Go:   if x == nil {}
来源：http://hz.zhixingplan.top/gtvltjeubg.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.yvedp.cn/gtqawqpjgj.html

C#:   if (x is null) {}
来源：http://hz.birdmap.top/gtbjkacjdp.html

[P07] 防抖与节流
来源：http://hz.tian-w.cn/gtljsvsexj.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.havefunace.top/gtrywttlrf.html

PHP:  // 手写时间戳比较
来源：http://hz.ppjwa.cn/gtlormarwk.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.cheryme.top/gtdqipykll.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.cqqwz.cn/gtproghqfd.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.shanyushiyangtech.top/gtficnyzgt.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.nwbrower.top/gtdwgtcfig.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.ppjwa.cn/gtgkhehxbl.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.yangfankeji.com/gtlqbhxdwa.html

[P08] 处理浮点精度问题
来源：http://hz.xziqi.cn/gtybbgqiwh.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.ydjk.org.cn/gtwmngrcpu.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.nwbrower.top/gtxbvdjknj.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.yvedp.cn/gtukninvwv.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.fzhhl.top/gtlqqyynqz.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.daria6918.cn/gtyrtyksyu.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.xuanzx.com/gtzxrehzcp.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.zycfv.cn/gtbodqwxtu.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.smart0.xyz/gtbmgplcjv.html

================================================================================
来源：http://hz.xylfe.cn/gtwfnjnywi.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.cashguo.top/gtmnzavtdz.html

================================================================================
来源：http://hz.meibo888.top/gtujafmfdq.html

[Q01] 创建表
来源：http://hz.jianghu66.top/gtdrvxuxmd.html

CREATE TABLE users (
来源：http://hz.sufxvd.cn/gtfjpiddxt.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.52xcode.cn/gtnkswmtdp.html

name VARCHAR(50) NOT NULL,
来源：http://hz.svipenyu.cn/gtoqyinuvr.html

email VARCHAR(100) UNIQUE,
来源：http://hz.xuanzx.com/gtfzifjqtb.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.snrcjt.cn/gtojudftfi.html

);
来源：http://hz.snrcjt.cn/gtyvgkrzrl.html

[Q02] 创建带外键的表
来源：http://hz.hnqzz.top/gtnkthfgwt.html

CREATE TABLE orders (
来源：http://hz.52xcode.cn/gtninkxzjf.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.dianchejie.cn/gtitmtngtl.html

user_id INT NOT NULL,
来源：http://hz.tian-w.cn/gtfvmgbugf.html

amount DECIMAL(10, 2),
来源：http://hz.jianghu66.top/gttrhampwb.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.tianlin.xyz/gthymmeujf.html

);
来源：http://hz.chenjidiqi.icu/gtjpislmau.html

[Q03] 增加列
来源：http://hz.mhx1999.top/gtwzfddcss.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.daria6918.cn/gtppqxiyws.html

[Q04] 修改列类型
来源：http://hz.yonumen.top/gtoulkmkow.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.fzhhl.top/gtcmdcxebe.html

[Q05] 重命名列
来源：http://hz.hnxiangtu.top/gtinigsigb.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.shanyushiyangtech.top/gtmxsfqkfx.html

[Q06] 删除列
来源：http://hz.jinyuanbaomall.cn/gtoujmcbsk.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.yangfankeji.com/gtqjhhgghj.html

[Q07] 删除表
来源：http://hz.zycfv.cn/gtrlntqqap.html

DROP TABLE IF EXISTS orders;
来源：http://hz.daria6918.cn/gtnbqavkwp.html

[Q08] 创建普通索引
来源：http://hz.sxryk.cn/gtupgvvace.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.feifeiyinyue.top/gtetxwnxcf.html

[Q09] 创建唯一索引
来源：http://hz.pengpengdd.cyou/gtnjesmiic.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.snrcjt.cn/gtjjaewrpv.html

[Q10] 插入单行
来源：http://hz.cheryme.top/gtujwjowtm.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.ywan-chungtsiang.top/gtrbtfvktc.html

[Q11] 一次插入多行
来源：http://hz.pycfn.com/gtsjlbhjna.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.zhixingplan.top/gtuqjzhemv.html

[Q12] 插入后取自增 ID
来源：http://hz.hfpthk.cn/gthteyoqzh.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.tianlin.xyz/gtjdjgjsaz.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.daxiang520.top/gtgeodcscn.html

[Q13] 忽略重复插入
来源：http://hz.yvedp.cn/gtqccpqlur.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.mhx1999.top/gtjdewrxfy.html

[Q14] 存在则更新（upsert）
来源：http://hz.meibo888.top/gtkpftsavx.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.daxiang520.top/gtsdqcohhm.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.ehwqpu.com/gtmbgspccd.html

[Q15] 查询全部
来源：http://hz.haohaochexian.top/gtdojnkvxd.html

SELECT * FROM users;
来源：http://hz.cdnleiting.top/gtvzgixiur.html

[Q16] 查询指定列
来源：http://hz.ydjk.org.cn/gtioqzbypt.html

SELECT id, name FROM users;
来源：http://hz.jinghuilouyu.cn/gtrmscqoxo.html

[Q17] 条件查询
来源：http://hz.xingfuxueyuan.xyz/gtoyciobyd.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.zycfv.cn/gteyfnebqj.html

[Q18] 模糊匹配
来源：http://hz.kuanghao11.cn/gtagpypqvy.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.jiagoushi.top/gtejbpxvvs.html

[Q19] 范围查询
来源：http://hz.9152youxi.cn/gtnctmvvzu.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.shanyushiyangkeji.top/gtssznacuo.html

[Q20] IN 列表
来源：http://hz.shangyingyoupin.top/gtyftdpzww.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.yj20258.top/gtehnxzhss.html

[Q21] 空值判断
来源：http://hz.ivvv.top/gtttnkkhbg.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.svipenyu.cn/gtwjnbnbch.html

[Q22] 排序
来源：http://hz.9152youxi.cn/gtepfmhwta.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.tanke756.top/gtghptpszz.html

[Q23] 分页
来源：http://hz.zhongyouzk.top/gtdfzcqtpj.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.316326.xyz/gtmtrjlqdy.html

[Q24] 去重
来源：http://hz.yuanzhike.top/gtyaytktqg.html

SELECT DISTINCT city FROM users;
来源：http://hz.hnqzz.top/gtvlmxrqwl.html

[Q25] 只取前 N 条
来源：http://hz.yuxming.cn/gtneqjypyv.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.sysykeji.top/gtrqsonxkh.html

[Q26] 计数
来源：http://hz.xinyue.icu/gtqbnfbbox.html

SELECT COUNT(*) FROM users;
来源：http://hz.gogol.net.cn/gtuxvgydcp.html

[Q27] 条件计数
来源：http://hz.hfpthk.cn/gtjcuyggnv.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.cdnleiting.top/gtkoubnyml.html

[Q28] 求和与平均
来源：http://hz.yangfankeji.com/gtowdmqqrf.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.fzhhl.top/gtbkcghlrg.html

[Q29] 最大最小值
来源：http://hz.ehwqpu.com/gtiumriutn.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.feifeiyinyue.top/gtbuzvxubo.html

[Q30] 分组统计
来源：http://hz.0kj1m.cn/gtbmrggqnf.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.hywenlv.cn/gtjlmahgly.html

[Q31] 分组后过滤
来源：http://hz.xuanzx.com/gtbycjmijr.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.tianlin.xyz/gtcuusfwmt.html

[Q32] 分组拼接字符串
来源：http://hz.ydzc1.top/gtmnyzxktc.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.ppjwa.cn/gtzkndtugb.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.yj20258.top/gtxwzxzmph.html

[Q33] 多列分组
来源：http://hz.ydzc1.top/gtozuouzpb.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.zhixingplan.top/gtaqyixesb.html

[Q34] 每组取第一条
来源：http://hz.tanke756.top/gtjrgjobrg.html

SELECT * FROM (
来源：http://hz.jinghuilouyu.cn/gtvldwhxzh.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.jiagoushi.top/gtxjixayrs.html

) t WHERE rn = 1;
来源：http://hz.52xcode.cn/gtvssjoqzv.html

[Q35] 内连接
来源：http://hz.birdmap.top/gtoqprksnx.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.hongshengwenyu.top/gtoftbtotb.html

[Q36] 左连接
来源：http://hz.tianlin.xyz/gtucfgftso.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.shangyingyoupin.top/gtxttzfjjl.html

[Q37] 右连接
来源：http://hz.shuidangran.top/gtgfhikzdh.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.hnqzz.top/gtwqwhxjkn.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.jinghuilouyu.cn/gtnixctiqg.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.ppjwa.cn/gtcbbksamt.html

[Q39] 自连接（查上下级）
来源：http://hz.yj202588.top/gthhrqapxv.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.cucudq.cn/gtkiakwhfe.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.hysaishi.cn/gtshjaeoni.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.ehwqpu.com/gtphrkzqib.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.ppjwa.cn/gthqypdzfr.html

[Q41] 多表连接
来源：http://hz.shanyushiyangtech.top/gtbkwdtfik.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.gaohongyu789.top/gtxnfuaulr.html

JOIN users u ON u.id = o.user_id
来源：http://hz.nwbrower.top/gtzbamihzc.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.yj20258.top/gtluktdhgk.html

[Q42] 连接条件附加过滤
来源：http://hz.zhoulong.xyz/gtaajjejng.html

SELECT u.name, o.amount FROM users u
来源：http://hz.sweek.top/gtgsyybbxd.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.xziqi.cn/gtuphpenvu.html

[Q43] 标量子查询
来源：http://hz.andypj.xyz/gtgsojnzqd.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.wangshuangyany.cn/gtoitzpruu.html

[Q44] IN 子查询
来源：http://hz.smart0.xyz/gtdlgonozd.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.chenlongwang.top/gtnstcukfo.html

[Q45] EXISTS 判断存在
来源：http://hz.yj20258888.top/gtzdtevlkw.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.vqdsnc.cn/gthpnbhnhw.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.9152youxi.cn/gtdsihmiwd.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.gzhubu.top/gtragqwqup.html

[Q47] 与平均值比较
来源：http://hz.haohaochexian.top/gtstmqfkak.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.aibaodan.cn/gtreihfjjg.html

[Q48] CTE 公用表表达式
来源：http://hz.xuanzx.com/gtiftzmchl.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.jqgfzy.top/gtmlqgenaz.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.xingfuxueyuan.xyz/gtcqvrzxse.html

[Q49] 更新单行
来源：http://hz.iojbl.cn/gtgidyvvfj.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.gzhubu.top/gtdfojtelv.html

[Q50] 批量更新
来源：http://hz.zhoulong.xyz/gtnykddubj.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.yueranfly.top/gtgiwyqnzh.html

[Q51] 用子查询更新
来源：http://hz.yj20258.top/gtzffphduv.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.havefunace.top/gtkwvfakqd.html

[Q52] 删除指定行
来源：http://hz.tanke756.top/gtydpxobtm.html

DELETE FROM users WHERE id = 10;
来源：http://hz.sufxvd.cn/gtnipmiusy.html

[Q53] 按条件删除
来源：http://hz.jinghuilouyu.cn/gtoqxecrwx.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.xuetiantiany.cn/gtzgimawxq.html

[Q54] 清空表
来源：http://hz.zdqjudy.top/gtbpvyiqut.html

TRUNCATE TABLE logs;
来源：http://hz.ehwqpu.com/gtdhuhczmw.html

[Q55] 排名（并列占位）
来源：http://hz.cucudq.cn/gtpfjupufa.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.xuanzx.com/gtvnobkikj.html

[Q56] 密集排名（并列不占位）
来源：http://hz.hnxiangtu.top/gtrdngyhmc.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.haohaochexian.top/gtkbaziljc.html

[Q57] 行号
来源：http://hz.xziqi.cn/gtiwpltsxx.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.tanke756.top/gtpkkcrggh.html

[Q58] 累计求和
来源：http://hz.nwbrower.top/gtlnkyaywq.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.yanxiufei.cn/gttgdwvjuh.html

[Q59] 分组内累计
来源：http://hz.yj20258888.top/gtnxyfrrka.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.sweek.top/gtuwejuhhv.html

[Q60] 取上一行 / 下一行
来源：http://hz.ywan-chungtsiang.top/gtmwhrpmkv.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.xinyue.icu/gtgcqsxnoo.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.hfpthk.cn/gteakhirbs.html

[Q61] 移动平均
来源：http://hz.nanxinkj.top/gtbtvmmlxw.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.andypj.xyz/gtpjobsvdl.html

[Q62] 分组占比
来源：http://hz.yj20258.top/gtylptnvzz.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.sxryk.cn/gtuptvbuyz.html

[Q63] 开启事务
来源：http://hz.zhixingplan.top/gtlnbmiyfy.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.zhijiandao.cn/gtbgohlaen.html

[Q64] 提交事务
来源：http://hz.jqgfzy.top/gtdscbzvkk.html

COMMIT;
来源：http://hz.yanxiufei.cn/gtkamqhbgl.html

[Q65] 回滚事务
来源：http://hz.zhengqikj.top/gtkdbtrknx.html

ROLLBACK;
来源：http://hz.redwolf501.top/gtobbmnqyc.html

[Q66] 行锁查询
来源：http://hz.aibaodan.cn/gtvqfoqgeb.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.cheryme.top/gtmubmstjc.html

[Q67] 设置隔离级别
来源：http://hz.gzhubu.top/gtsmbmbyla.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.cheryme.top/gtlthyasvm.html

[Q68] 保存点
来源：http://hz.jiagoushi.top/gtuxcjhaeq.html

SAVEPOINT sp1;
来源：http://hz.shuidangran.top/gtckyjglpc.html

ROLLBACK TO sp1;
来源：http://hz.ydzc1.top/gttfcybfcn.html

[Q69] 查看执行计划
来源：http://hz.yvedp.cn/gteyamkxjp.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.quarkkingdee.top/gtukwynedl.html

[Q70] 更新统计信息
来源：http://hz.sufxvd.cn/gtefjpltbe.html

ANALYZE TABLE users;
来源：http://hz.birdmap.top/gtfokihvjt.html

[Q71] 查看建表语句
来源：http://hz.pycfn.com/gtaxiqkozk.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.dianchejie.cn/gtyikdhuwf.html

[Q72] 查看索引
来源：http://hz.smart0.xyz/gtwyewsmqj.html

SHOW INDEX FROM users;
来源：http://hz.guannengcc.top/gtkjyvqndx.html

[Q73] 查看表状态
来源：http://hz.dashuyun.cn/gtwxronzzr.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.hfpthk.cn/gtmdaeztzc.html

[Q74] 强制使用索引
来源：http://hz.xinyue.icu/gthtmqsips.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.jyoumei.cn/gtyyqidtsn.html

[Q75] 日期格式化
来源：http://hz.ehwqpu.com/gtdtgiacac.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.yangfankeji.com/gtwoqlbkgw.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.tanke756.top/gtewrnewsl.html

[Q76] 按天统计
来源：http://hz.jyoumei.cn/gtamgmsytp.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.quarkkingdee.top/gthalopivz.html

[Q77] 时间加减
来源：http://hz.xziqi.cn/gthuttkmak.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.xuanzx.com/gtutsqeydn.html

[Q78] 当前时间
来源：http://hz.hywenlv.cn/gtuotfplwx.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.hywenlv.cn/gtilbmxwzl.html

[Q79] 字符串拼接
来源：http://hz.guannengcc.top/gtmreygcnn.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.haohaochexian.top/gttgxehxhi.html

[Q80] 字符串截取
来源：http://hz.tanke756.top/gtgailifkt.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.aizwys.cn/gtpflciqra.html

[Q81] 字符串替换
来源：http://hz.wangdashe.top/gtlclbyxgp.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.hysaishi.cn/gtvlymvjhm.html

[Q82] 字符长度与字节长度
来源：http://hz.feifeiyinyue.top/gttwtxrwdi.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.xziqi.cn/gtczfgeacm.html

[Q83] 大小写转换
来源：http://hz.sufxvd.cn/gtchzlqbtq.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.wangdashe.top/gtpvsaueii.html

[Q84] 去除首尾空格
来源：http://hz.xuetiantiany.cn/gtbyvrtvsh.html

SELECT TRIM(name) FROM users;
来源：http://hz.shzxlz.cn/gtftegtbae.html

[Q85] 数值取整
来源：http://hz.gaohongyu789.top/gtbhauwatq.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.xylfe.cn/gtgsszrzoa.html

[Q86] 读取 JSON 字段
来源：http://hz.pengpengdd.cyou/gtuzyczhtx.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.hammf.cn/gtkorjxxlj.html

[Q87] JSON 字段做条件
来源：http://hz.jyoumei.cn/gtkmhompwu.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.nanxinkj.top/gtpixglvyo.html

[Q88] 行转列（条件聚合）
来源：http://hz.jinqigufen.top/gticiokvmk.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.ybcxt.top/gtthobejok.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.yangfankeji.com/gtaagglpjc.html

[Q89] 判断表是否存在
来源：http://hz.gaohongyu789.top/gtvwxxcige.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.9152youxi.cn/gtcsvsbwil.html

[Q90] 生成序号列
来源：http://hz.wangshuangyany.cn/gtuoltgvtj.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.ehwqpu.com/gtfopuobpc.html

================================================================================
来源：http://hz.jyoumei.cn/gtwsgnjnof.html

R. Bash 专题
来源：http://hz.ehwqpu.com/gtskwlbskz.html

================================================================================
来源：http://hz.shangyingyoupin.top/gttbeeqwqs.html

[R01] shebang 与严格模式
来源：http://hz.c1oappe.top/gtuqifqqcj.html

#!/usr/bin/env bash
来源：http://hz.gzhubu.top/gtyselaapi.html

set -euo pipefail
来源：http://hz.chenjidiqi.icu/gteqrjbxnc.html

[R02] 变量赋值与使用
来源：http://hz.yanxiufei.cn/gtpscxegbm.html

name="Tom"; echo "$name"
来源：http://hz.ywan-chungtsiang.top/gtyrovvfnq.html

[R03] 只读变量
来源：http://hz.zhijiandao.cn/gtjszsbdrq.html

readonly PI=3.14
来源：http://hz.ivvv.top/gtnizlzywq.html

[R04] 位置参数
来源：http://hz.gzhubu.top/gthwpspoth.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.svipenyu.cn/gtgmthpowq.html

[R05] 参数默认值
来源：http://hz.vqdsnc.cn/gtjojyswlb.html

name="${1:-default}"
来源：http://hz.bjfxy.top/gtmpptolfb.html

[R06] 判断命令是否存在
来源：http://hz.yj20258888.top/gthneseiem.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.haohaochexian.top/gtpeflhjyi.html

[R07] if 判断文件
来源：http://hz.yanxiufei.cn/gtrzpqjpcl.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.cucudq.cn/gtyaqhwwpz.html

[R08] 数值比较
来源：http://hz.shanyushiyangkeji.top/gtvctfhnzb.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.wangdashe.top/gtjhtabtzd.html

[R09] 字符串比较
来源：http://hz.52xcode.cn/gttyoznpvx.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.gaohongyu789.top/gteirxzxhy.html

[R10] 正则匹配
来源：http://hz.tanke756.top/gtuunbcpyz.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.ehwqpu.com/gtffxhjbqj.html

[R11] case 多分支
来源：http://hz.pengpengdd.cyou/gtakecoarz.html

case "$1" in
来源：http://hz.ydzc1.top/gthgsxfine.html

start) echo "启动" ;;
来源：http://hz.vqdsnc.cn/gtoszsdhqw.html

stop)  echo "停止" ;;
来源：http://hz.yvedp.cn/gtbfbytjdq.html

*)     echo "未知命令" ;;
来源：http://hz.yj202588.top/gttbzqyhrd.html

esac
来源：http://hz.sysykeji.top/gtrdzqaixy.html

[R12] for 遍历文件
来源：http://hz.sufxvd.cn/gtfwgqfrrf.html

for f in *.txt; do echo "$f"; done
来源：http://hz.gzhubu.top/gtruzmhpaz.html

[R13] for 计数循环
来源：http://hz.ybcxt.top/gtdpaiawsy.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.smart0.xyz/gteuicrrel.html

[R14] C 风格 for
来源：http://hz.zhijiandao.cn/gtzuvsnzew.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.iojbl.cn/gtspltwcai.html

[R15] while 逐行读文件
来源：http://hz.zhixingplan.top/gtnbktrmwu.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.aizwys.cn/gtujmyvqap.html

[R16] until 等待条件
来源：http://hz.shanyushiyangtech.top/gtwjwqlfze.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.yongpay.top/gtsqnajsrf.html

[R17] 数组定义与取值
来源：http://hz.chenlongwang.top/gtvbzdxbyg.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.hywenlv.cn/gtyijqlwwb.html

[R18] 遍历数组
来源：http://hz.xylfe.cn/gtidoknggk.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.yanxiufei.cn/gtenbdtgsr.html

[R19] 数组长度
来源：http://hz.nanxuanxn.top/gthyzsxuwp.html


<!-- 参考信息 -->