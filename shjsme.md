代发 wailian999

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.jlsjyb.cn/gtatnxeuao.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.jianghu66.top/gtcpertmum.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.chenzaomai.com/gtffvqtwtx.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.ydzc1.top/gtynqkjvbg.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.jlsjyb.cn/gtqxvrckzw.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.cqqwz.cn/gtvardqiuj.html

[P03] 生成短随机字符串
来源：http://hz.xinyue.icu/gtexqmsjdm.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.zhixingplan.top/gtbevjfdmb.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.dashuyun.cn/gtwxlrqqdb.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yongpay.top/gtuhfvsabu.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.hysaishi.cn/gtzjfzuldl.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.0kj1m.cn/gtmltladzf.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.cdnleiting.top/gtvbodtxgz.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.jqgufenzy.top/gtgzrzookn.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.chenlongwang.top/gtlhtfefhk.html

[P04] 求长度
来源：http://hz.jlsjyb.cn/gtywmgriaj.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.zhongyouzk.top/gtlbroiacq.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zhijiandao.cn/gtlbexwxby.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.aibaodan.cn/gtitgtyphk.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.ybcxt.top/gtdyxqwzwt.html

Java: list.size();  map.size();  s.length()
来源：http://hz.sweek.top/gtzrxbyvwi.html

Go:   len(arr);  len(m)
来源：http://hz.chenzaomai.com/gteaijhgkb.html

Ruby: x.length;  x.size
来源：http://hz.smart0.xyz/gtftjrkzum.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.daxiang520.top/gttenypzfv.html

[P05] 判断两个对象内容是否相等
来源：http://hz.xziqi.cn/gtrqtzuqzj.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.gotoacloud.top/gteckszjfr.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.bjfxy.top/gtybwpaqcy.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.jianghu66.top/gtcdfvphcp.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.gotoacloud.top/gtpcvdxngd.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.ehwqpu.com/gtihglrtto.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.kuanghao11.cn/gtchbmdaol.html

Ruby: a == b
来源：http://hz.daxiang520.top/gttssnupcv.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.0kj1m.cn/gtqgdbruhc.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.yj20258888.top/gtnginmsvk.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.yongpay.top/gtbarbcmfw.html

PHP:  if (empty($x)) {}
来源：http://hz.yj20258.top/gtypjcrmob.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.zhijiandao.cn/gtdcbtzlmg.html

TS:   if (x == null) {}
来源：http://hz.meibo888.top/gtnicjdgjl.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.zycfv.cn/gtmyxrnkoo.html

Go:   if x == nil {}
来源：http://hz.xingfuxueyuan.xyz/gtfgibujsn.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.hammf.cn/gtdqcwlkqb.html

C#:   if (x is null) {}
来源：http://hz.yvedp.cn/gtghmwhrhc.html

[P07] 防抖与节流
来源：http://hz.cucudq.cn/gttwpwnsfm.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.jyoumei.cn/gtqfnwgccr.html

PHP:  // 手写时间戳比较
来源：http://hz.guannengcc.top/gtfsbjapfm.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.hnxiangtu.top/gtxegjkynv.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.svipenyu.cn/gtxnxolplz.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.zhaomingkeji.xyz/gttiukobna.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.chenjidiqi.icu/gtvwcpaobr.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.shzxlz.cn/gtyyjhctug.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.c1oappe.top/gtynmxzgch.html

[P08] 处理浮点精度问题
来源：http://hz.jqgufenzy.top/gtanlgyvzk.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.ydjk.org.cn/gtlemculka.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.aibaodan.cn/gthibjgieh.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.xylfe.cn/gtxnjakmcn.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.tian-w.cn/gtslqwqlja.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.sxryk.cn/gtavicaafh.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.yvedp.cn/gthivpgecx.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.zhongyouzk.top/gtuijtdrax.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.snrcjt.cn/gtgtgqlhat.html

================================================================================
来源：http://hz.hammf.cn/gtsfaeklbl.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.jyoumei.cn/gttaibjedi.html

================================================================================
来源：http://hz.yuxming.cn/gtsgyvwkdj.html

[Q01] 创建表
来源：http://hz.xuetiantiany.cn/gtekxkdknk.html

CREATE TABLE users (
来源：http://hz.zhoulong.xyz/gtjuvydfcw.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.gogol.net.cn/gtcmbedclg.html

name VARCHAR(50) NOT NULL,
来源：http://hz.xylfe.cn/gtschsyohh.html

email VARCHAR(100) UNIQUE,
来源：http://hz.sxryk.cn/gthtexxumb.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.jinyuanbaomall.cn/gtklbbjzur.html

);
来源：http://hz.pycfn.com/gtokulmtuz.html

[Q02] 创建带外键的表
来源：http://hz.hywenlv.cn/gtufsmaxvb.html

CREATE TABLE orders (
来源：http://hz.aibaodan.cn/gtischbyiw.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.pengpengdd.cyou/gtjsnfedws.html

user_id INT NOT NULL,
来源：http://hz.yangfankeji.com/gtrdrgzedy.html

amount DECIMAL(10, 2),
来源：http://hz.sysykeji.top/gtbkfpabjs.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.havefunace.top/gtpovwuodq.html

);
来源：http://hz.fengsongda.top/gtazxbqfmo.html

[Q03] 增加列
来源：http://hz.316326.xyz/gtoszxntax.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.yangfankeji.com/gtmbsztlzn.html

[Q04] 修改列类型
来源：http://hz.shanyushiyangkeji.top/gtrjfngrrz.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.yanxiufei.cn/gthjadpbtw.html

[Q05] 重命名列
来源：http://hz.shanyushiyangkeji.top/gtloehrpbc.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.yangfankeji.com/gtwivmrxsg.html

[Q06] 删除列
来源：http://hz.yuanzhike.top/gtrkwmoujs.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.ivvv.top/gtmtpyxpby.html

[Q07] 删除表
来源：http://hz.gogol.net.cn/gtmmpwzqhx.html

DROP TABLE IF EXISTS orders;
来源：http://hz.cdnleiting.top/gtfvdeogij.html

[Q08] 创建普通索引
来源：http://hz.yangfankeji.com/gtvsqhemfo.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.zhijiandao.cn/gtowcddizq.html

[Q09] 创建唯一索引
来源：http://hz.jyoumei.cn/gtxelsysyj.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.cdnleiting.top/gtqusiaguy.html

[Q10] 插入单行
来源：http://hz.ehwqpu.com/gtxkyklcwd.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.yanxiufei.cn/gtjumbausl.html

[Q11] 一次插入多行
来源：http://hz.cheryme.top/gtectwaidm.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.nwbrower.top/gtbejxtfic.html

[Q12] 插入后取自增 ID
来源：http://hz.yj20258888.top/gtajngcuvb.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.ivvv.top/gtuygawjef.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.zhongyouzk.top/gtoabycpri.html

[Q13] 忽略重复插入
来源：http://hz.shangyingyoupin.top/gtrorwqxxw.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.zhoulong.xyz/gtbxxzxyfc.html

[Q14] 存在则更新（upsert）
来源：http://hz.yuanzhike.top/gtxvtygwdi.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.jinqigufen.top/gtanoxkpju.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.pengpengdd.cyou/gtkvgsclch.html

[Q15] 查询全部
来源：http://hz.dianchejie.cn/gtgjxvryxt.html

SELECT * FROM users;
来源：http://hz.chenzaomai.com/gtykkeilen.html

[Q16] 查询指定列
来源：http://hz.52xcode.cn/gtsphybvks.html

SELECT id, name FROM users;
来源：http://hz.dianchejie.cn/gtqylvilaa.html

[Q17] 条件查询
来源：http://hz.c1oappe.top/gtlsamzicf.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.hfpthk.cn/gtdqwlawqz.html

[Q18] 模糊匹配
来源：http://hz.yueranfly.top/gtyoxamvne.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.guowangkeji.top/gtkzkgdbut.html

[Q19] 范围查询
来源：http://hz.chenzaomai.com/gtrmkmnlgj.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.xziqi.cn/gtnoggbtwx.html

[Q20] IN 列表
来源：http://hz.shanyushiyangtech.top/gtyfshnwyo.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.tanke756.top/gtenauapfj.html

[Q21] 空值判断
来源：http://hz.ydzc1.top/gtmssvjfej.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.yuanzhike.top/gttrliwkct.html

[Q22] 排序
来源：http://hz.hnxiangtu.top/gtbiqyhuvg.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.zhaomingkeji.xyz/gtigrhfvbh.html

[Q23] 分页
来源：http://hz.hnxiangtu.top/gtzohfgvfd.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.svipenyu.cn/gtpwrkkyux.html

[Q24] 去重
来源：http://hz.fzhhl.top/gtmlpjlvko.html

SELECT DISTINCT city FROM users;
来源：http://hz.yuxming.cn/gtkkbzlflm.html

[Q25] 只取前 N 条
来源：http://hz.pengpengdd.cyou/gtluicufgb.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.jinghuilouyu.cn/gthutodcew.html

[Q26] 计数
来源：http://hz.zhiwuduotai.top/gtfjicfrbu.html

SELECT COUNT(*) FROM users;
来源：http://hz.ydzc1.top/gtfcgeesgv.html

[Q27] 条件计数
来源：http://hz.ydjk.org.cn/gtesrxcvfq.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.ywan-chungtsiang.top/gtvqdsvxsc.html

[Q28] 求和与平均
来源：http://hz.hnxiangtu.top/gtsekxprmt.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.yanxiufei.cn/gtlmclouzc.html

[Q29] 最大最小值
来源：http://hz.yanxiufei.cn/gtccqykwau.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.svipenyu.cn/gtpvfiaxkd.html

[Q30] 分组统计
来源：http://hz.hfpthk.cn/gthflxtiqv.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.vqdsnc.cn/gtcxafcvia.html

[Q31] 分组后过滤
来源：http://hz.svipenyu.cn/gtdwersvxe.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.ehwqpu.com/gtlzbcmbgl.html

[Q32] 分组拼接字符串
来源：http://hz.pengpengdd.cyou/gtjjbgbsbq.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.shanyushiyangkeji.top/gtzyidptmc.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.cashguo.top/gthqwazmnw.html

[Q33] 多列分组
来源：http://hz.svipenyu.cn/gtitzorhio.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.cucudq.cn/gthqdyguok.html

[Q34] 每组取第一条
来源：http://hz.hnxiangtu.top/gtcpmdryrr.html

SELECT * FROM (
来源：http://hz.zhaomingkeji.xyz/gtaykzuzan.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.gogol.net.cn/gtgxtwmznu.html

) t WHERE rn = 1;
来源：http://hz.sufxvd.cn/gtfxuymahp.html

[Q35] 内连接
来源：http://hz.0kj1m.cn/gtjvngkmdr.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.ywan-chungtsiang.top/gtirpuatpr.html

[Q36] 左连接
来源：http://hz.yanxiufei.cn/gtjymqistv.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.sysykeji.top/gtizlawhud.html

[Q37] 右连接
来源：http://hz.iojbl.cn/gtavgiohxe.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.316326.xyz/gtfjaymhoh.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.ybcxt.top/gtlzpabiqs.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.havefunace.top/gtrvrcrizv.html

[Q39] 自连接（查上下级）
来源：http://hz.dashuyun.cn/gtcrqpnakn.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.sufxvd.cn/gtxdgwqrnd.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.tianlin.xyz/gtaryrilgb.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.zhengqikj.top/gtfghextfq.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.jinghuilouyu.cn/gtlbhtnwbt.html

[Q41] 多表连接
来源：http://hz.jinqigfzy.top/gtlehuwbjz.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.gaohongyu789.top/gtfsraumfe.html

JOIN users u ON u.id = o.user_id
来源：http://hz.daxiang520.top/gtuvihxkod.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.nwbrower.top/gtxiilwqlr.html

[Q42] 连接条件附加过滤
来源：http://hz.wangdashe.top/gtctugmnln.html

SELECT u.name, o.amount FROM users u
来源：http://hz.zhiwuduotai.top/gtlovwtpxj.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.aibaodan.cn/gtkzwuipbd.html

[Q43] 标量子查询
来源：http://hz.feifeiyinyue.top/gtadelzuti.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.guowangkeji.top/gtiumtcufy.html

[Q44] IN 子查询
来源：http://hz.yj20258.top/gtyiobtqoi.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.zhongyouzk.top/gttqpklnfd.html

[Q45] EXISTS 判断存在
来源：http://hz.zhixingplan.top/gthppjaoat.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.xylfe.cn/gtrxqouatu.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.gaohongyu789.top/gtqljtaabp.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.c1oappe.top/gtilbokozs.html

[Q47] 与平均值比较
来源：http://hz.tian-w.cn/gtvdtbwogp.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.yj202588.top/gttffmqbfu.html

[Q48] CTE 公用表表达式
来源：http://hz.tian-w.cn/gtuypmzrlz.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.jqgfzy.top/gtlnrtzrdy.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.316326.xyz/gtuapfzbfe.html

[Q49] 更新单行
来源：http://hz.shzxlz.cn/gtbhycfwzf.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.pengpengdd.cyou/gtnofvgwyy.html

[Q50] 批量更新
来源：http://hz.xziqi.cn/gtsjpbdpfm.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.ppjwa.cn/gtjsjzqblx.html

[Q51] 用子查询更新
来源：http://hz.daria6918.cn/gtnvsrfuqk.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.ywan-chungtsiang.top/gtbhscoprl.html

[Q52] 删除指定行
来源：http://hz.havefunace.top/gtrfekflio.html

DELETE FROM users WHERE id = 10;
来源：http://hz.daxiang520.top/gtcbefurjr.html

[Q53] 按条件删除
来源：http://hz.c1oappe.top/gtynswkmxh.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.tianlin.xyz/gtaazkagpk.html

[Q54] 清空表
来源：http://hz.jyoumei.cn/gtkbuolfvx.html

TRUNCATE TABLE logs;
来源：http://hz.daxiang520.top/gttnedeqzy.html

[Q55] 排名（并列占位）
来源：http://hz.xuanzx.com/gtckpczrsm.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.0kj1m.cn/gtnryzxrwy.html

[Q56] 密集排名（并列不占位）
来源：http://hz.pengpengdd.cyou/gtpabyeoze.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.kuanghao11.cn/gtjevhtarv.html

[Q57] 行号
来源：http://hz.xylfe.cn/gtzckjwlwj.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.yj202588.top/gtrqgydbqb.html

[Q58] 累计求和
来源：http://hz.jyoumei.cn/gtgebbgrfp.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.guowangkeji.top/gtxqlhvwmv.html

[Q59] 分组内累计
来源：http://hz.cashguo.top/gtlhqdlxwf.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.guowangkeji.top/gtwukhtgvu.html

[Q60] 取上一行 / 下一行
来源：http://hz.chenjidiqi.icu/gtdyfyfscy.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.bjfxy.top/gtelbhpsuk.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.quarkkingdee.top/gtzpemjwlq.html

[Q61] 移动平均
来源：http://hz.jlsjyb.cn/gtxcpfxoxt.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.nanxuanxn.top/gtgetjkkby.html

[Q62] 分组占比
来源：http://hz.yvedp.cn/gtjpbfwzmd.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.jqgfzy.top/gtrznfdmwc.html

[Q63] 开启事务
来源：http://hz.birdmap.top/gtophvbtaz.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.jyoumei.cn/gtmgegtfwf.html

[Q64] 提交事务
来源：http://hz.yvedp.cn/gtmhzgeifq.html

COMMIT;
来源：http://hz.xuetiantiany.cn/gtnzrddfwc.html

[Q65] 回滚事务
来源：http://hz.zhongyouzk.top/gtkazlcrvy.html

ROLLBACK;
来源：http://hz.aibaodan.cn/gtqoyzakwo.html

[Q66] 行锁查询
来源：http://hz.hnqzz.top/gtxyjeyjwx.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.dashuyun.cn/gthedxfkjd.html

[Q67] 设置隔离级别
来源：http://hz.jiagoushi.top/gtrnyhyjna.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.aibaodan.cn/gtewgmzvcl.html

[Q68] 保存点
来源：http://hz.tian-w.cn/gtqydcauvc.html

SAVEPOINT sp1;
来源：http://hz.jqgufenzy.top/gtyalzhmeh.html

ROLLBACK TO sp1;
来源：http://hz.gotoacloud.top/gtbxnjiwvn.html

[Q69] 查看执行计划
来源：http://hz.hfpthk.cn/gtzrmxnvph.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.yangfankeji.com/gtammgycrd.html

[Q70] 更新统计信息
来源：http://hz.ybcxt.top/gtinvmgytt.html

ANALYZE TABLE users;
来源：http://hz.jinyuanbaomall.cn/gtuingcwvt.html

[Q71] 查看建表语句
来源：http://hz.zhixingplan.top/gteqkszpfw.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.gotoacloud.top/gtkiajjnmy.html

[Q72] 查看索引
来源：http://hz.jqgfzy.top/gtmftghxvr.html

SHOW INDEX FROM users;
来源：http://hz.gogol.net.cn/gtrwowmmpk.html

[Q73] 查看表状态
来源：http://hz.dashuyun.cn/gtsalbdrew.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.hammf.cn/gtccbfcjbq.html

[Q74] 强制使用索引
来源：http://hz.0kj1m.cn/gtbziezyod.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.sysykeji.top/gtzskqzoiv.html

[Q75] 日期格式化
来源：http://hz.xinyue.icu/gtdwamwzyg.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.sysykeji.top/gtehdbqemx.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.zycfv.cn/gtjapxdkal.html

[Q76] 按天统计
来源：http://hz.shzxlz.cn/gtzrmsxnjb.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.yueranfly.top/gtqxhpxtoz.html

[Q77] 时间加减
来源：http://hz.haohaochexian.top/gthrinehni.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.wangshuangyany.cn/gtwejypfqg.html

[Q78] 当前时间
来源：http://hz.jqgfzy.top/gtzjgppzui.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.gzhubu.top/gttjmomghr.html

[Q79] 字符串拼接
来源：http://hz.dianchejie.cn/gtjkctxqvs.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.jqgfzy.top/gtrfpjnkwz.html

[Q80] 字符串截取
来源：http://hz.9152youxi.cn/gtipcqzgwp.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.meibo888.top/gtodrhdwpc.html

[Q81] 字符串替换
来源：http://hz.ydzc1.top/gtxhyoriyu.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.zdqjudy.top/gtsflgltjk.html

[Q82] 字符长度与字节长度
来源：http://hz.52xcode.cn/gtfhlbviwu.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.jiagoushi.top/gtjzboozlm.html

[Q83] 大小写转换
来源：http://hz.mhx1999.top/gtkqjpkroh.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.gogol.net.cn/gtljkarvhl.html

[Q84] 去除首尾空格
来源：http://hz.nanxuanxn.top/gtxsejbiou.html

SELECT TRIM(name) FROM users;
来源：http://hz.nwbrower.top/gtcajpxyed.html

[Q85] 数值取整
来源：http://hz.zhengqikj.top/gtkzsjdcxz.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.ybcxt.top/gtlboaowkl.html

[Q86] 读取 JSON 字段
来源：http://hz.ppjwa.cn/gtrnxjvejl.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.zhijiandao.cn/gtnmztyydh.html

[Q87] JSON 字段做条件
来源：http://hz.sxryk.cn/gtgijceloh.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.wangshuangyany.cn/gtkllwhdty.html

[Q88] 行转列（条件聚合）
来源：http://hz.daria6918.cn/gtocqqnuzx.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.sysykeji.top/gtkvyoxoqq.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.kuanghao11.cn/gtralhyxep.html

[Q89] 判断表是否存在
来源：http://hz.ivvv.top/gtkuwnpcvy.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.fengsongda.top/gtezmbausz.html

[Q90] 生成序号列
来源：http://hz.zhijiandao.cn/gtvlzlvfmn.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.cashguo.top/gtmshdwgnj.html

================================================================================
来源：http://hz.xuanzx.com/gtfgdyqsii.html

R. Bash 专题
来源：http://hz.sxryk.cn/gtevkvgfpq.html

================================================================================
来源：http://hz.meibo888.top/gtgjreeund.html

[R01] shebang 与严格模式
来源：http://hz.meibo888.top/gteslhejjg.html

#!/usr/bin/env bash
来源：http://hz.shuidangran.top/gtjgkvngpk.html

set -euo pipefail
来源：http://hz.gaohongyu789.top/gtbcnvdfee.html

[R02] 变量赋值与使用
来源：http://hz.gogol.net.cn/gtrqvdypkn.html

name="Tom"; echo "$name"
来源：http://hz.jyoumei.cn/gtblhlmlbk.html

[R03] 只读变量
来源：http://hz.meibo888.top/gtkhblyqvr.html

readonly PI=3.14
来源：http://hz.dashuyun.cn/gturmpqowj.html

[R04] 位置参数
来源：http://hz.feifeiyinyue.top/gtovzddney.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.shanyushiyangtech.top/gtkflgsprv.html

[R05] 参数默认值
来源：http://hz.daxiang520.top/gthofddrmc.html

name="${1:-default}"
来源：http://hz.yongpay.top/gtvyzhsaxi.html

[R06] 判断命令是否存在
来源：http://hz.yj20258888.top/gtjterybye.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.hammf.cn/gtuvlrmbdr.html

[R07] if 判断文件
来源：http://hz.sysykeji.top/gtfvggcypv.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.jlsjyb.cn/gtwzjzutxa.html

[R08] 数值比较
来源：http://hz.yonumen.top/gtvrgtsnus.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.xuetiantiany.cn/gtspihcupf.html

[R09] 字符串比较
来源：http://hz.cheryme.top/gtjvjyegjc.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.fzhhl.top/gtlsnelloh.html

[R10] 正则匹配
来源：http://hz.daxiang520.top/gtqichixya.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.316326.xyz/gtjsdwelin.html

[R11] case 多分支
来源：http://hz.yuxming.cn/gtcgdszkve.html

case "$1" in
来源：http://hz.gogol.net.cn/gtslfsddpz.html

start) echo "启动" ;;
来源：http://hz.jinyuanbaomall.cn/gtwtpulxlh.html

stop)  echo "停止" ;;
来源：http://hz.ppjwa.cn/gtjbeyojrz.html

*)     echo "未知命令" ;;
来源：http://hz.jianghu66.top/gtxampyxev.html

esac
来源：http://hz.zhiwuduotai.top/gtoicisppf.html

[R12] for 遍历文件
来源：http://hz.yanxiufei.cn/gtknqpujtz.html

for f in *.txt; do echo "$f"; done
来源：http://hz.xylfe.cn/gtqhmogtyi.html

[R13] for 计数循环
来源：http://hz.shangyingyoupin.top/gtkvpglxxb.html


<!-- 参考信息 -->