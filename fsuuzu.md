代发 wailian999

TS:   crypto.randomUUID()
来源：http://hz.xuetiantiany.cn/gtgfqziozd.html

Java: UUID.randomUUID().toString()
来源：http://hz.yj20258888.top/gtgxiqlmxj.html

Go:   // 用 github.com/google/uuid
来源：http://hz.jinyuanbaomall.cn/gtptpfesen.html

Ruby: SecureRandom.uuid
来源：http://hz.shuidangran.top/gteumejejs.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.yonumen.top/gtfucaxyhm.html

[P02] MD5 / SHA256 摘要
来源：http://hz.snrcjt.cn/gtfwfhieor.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.gogol.net.cn/gtnjhxzfmz.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.shanyushiyangkeji.top/gtenirdxxg.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.ybcxt.top/gtxppbjeex.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.fengsongda.top/gttzrdaazl.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.zhengqikj.top/gtwaksolko.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.jinghuilouyu.cn/gtdpwvbaae.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.feifeiyinyue.top/gtqogaqrfr.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.tianlin.xyz/gtidtdcdss.html

[P03] 生成短随机字符串
来源：http://hz.haohaochexian.top/gtxrsjqnwo.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.yueranfly.top/gtpccvgiys.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.dashuyun.cn/gtzxrjlypq.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.vqdsnc.cn/gtclbkvrdt.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jqgfzy.top/gtzxkszzhs.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.cucudq.cn/gtsztekiam.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.zdqjudy.top/gtnnwtgydz.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.xinyue.icu/gtzpaprcux.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.jyoumei.cn/gttodyzueo.html

[P04] 求长度
来源：http://hz.birdmap.top/gtyzqyvxod.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.havefunace.top/gtlkivopyq.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.dashuyun.cn/gtirkxkzux.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.chenlongwang.top/gtnbxynxco.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.tian-w.cn/gtaqcmicxz.html

Java: list.size();  map.size();  s.length()
来源：http://hz.jinghuilouyu.cn/gtzvleyxck.html

Go:   len(arr);  len(m)
来源：http://hz.zhengqikj.top/gtlqbfahif.html

Ruby: x.length;  x.size
来源：http://hz.daxiang520.top/gtexizvbpr.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.shanyushiyangtech.top/gtazsnkysr.html

[P05] 判断两个对象内容是否相等
来源：http://hz.zdqjudy.top/gttxoluhra.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.cucudq.cn/gtvxokapee.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.sweek.top/gtmqyhmxfe.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.yangfankeji.com/gtietobsva.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.hywenlv.cn/gtownasesj.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.jyoumei.cn/gtsinhksvn.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.jqgufenzy.top/gttcsgngib.html

Ruby: a == b
来源：http://hz.svipenyu.cn/gtoapmhlgw.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.xuanzx.com/gtvokyydrf.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.xuetiantiany.cn/gtdkykecwv.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.haohaochexian.top/gtyeiohbga.html

PHP:  if (empty($x)) {}
来源：http://hz.mhx1999.top/gtalhfiogl.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.xylfe.cn/gtydbghbyy.html

TS:   if (x == null) {}
来源：http://hz.9152youxi.cn/gtxkvesoqt.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.jlsjyb.cn/gtsznzpove.html

Go:   if x == nil {}
来源：http://hz.sxryk.cn/gtwqdfotdl.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.hysaishi.cn/gtqafdehoc.html

C#:   if (x is null) {}
来源：http://hz.quarkkingdee.top/gtwholuwoe.html

[P07] 防抖与节流
来源：http://hz.havefunace.top/gtkbvjbosa.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.sweek.top/gtlevgsabp.html

PHP:  // 手写时间戳比较
来源：http://hz.zhiwuduotai.top/gtwevodmco.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.tianlin.xyz/gteypqdbvt.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.shangyingyoupin.top/gtkyuxdlxo.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.wangdashe.top/gtzhnpqaen.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.yuanzhike.top/gtqmnkarof.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.cdnleiting.top/gtnvqpihip.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.yj20258888.top/gtodubkgnh.html

[P08] 处理浮点精度问题
来源：http://hz.snrcjt.cn/gtxobdtuiw.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.0kj1m.cn/gtiqsjtqta.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.hnxiangtu.top/gtpuwatvse.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.pycfn.com/gteiqowwtd.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.ivvv.top/gtsubcwtbb.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.cucudq.cn/gtozqasqam.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.aibaodan.cn/gtybaovhmf.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.ivvv.top/gtplvsqmlw.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.hfpthk.cn/gtrtihopqt.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtzwgfrnqa.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.yangfankeji.com/gthuhwnhrg.html

================================================================================
来源：http://hz.hammf.cn/gtmjeqyqkz.html

[Q01] 创建表
来源：http://hz.chenzaomai.com/gtaedwkszw.html

CREATE TABLE users (
来源：http://hz.jinghuilouyu.cn/gtxbhbezzv.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.ybcxt.top/gtizsjowyy.html

name VARCHAR(50) NOT NULL,
来源：http://hz.cqqwz.cn/gtgfvymsvz.html

email VARCHAR(100) UNIQUE,
来源：http://hz.jinqigfzy.top/gtlcfpczdc.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.yanxiufei.cn/gtivcrfveb.html

);
来源：http://hz.ybcxt.top/gtbhqfggmp.html

[Q02] 创建带外键的表
来源：http://hz.daria6918.cn/gtmaokxksa.html

CREATE TABLE orders (
来源：http://hz.tanke756.top/gtjssqhxsu.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yj20258.top/gtslyirbqx.html

user_id INT NOT NULL,
来源：http://hz.jlsjyb.cn/gtlaqfvinm.html

amount DECIMAL(10, 2),
来源：http://hz.ydjk.org.cn/gtlbqpnphj.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.gogol.net.cn/gtjvbhoztt.html

);
来源：http://hz.xuanzx.com/gtghmwyunw.html

[Q03] 增加列
来源：http://hz.tian-w.cn/gtdizolrxa.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.hammf.cn/gthbmphmyj.html

[Q04] 修改列类型
来源：http://hz.jqgufenzy.top/gtjncgrdol.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.aibaodan.cn/gtaqfhvmzp.html

[Q05] 重命名列
来源：http://hz.xziqi.cn/gtctqgmkrd.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.ydzc1.top/gtlpsbsnax.html

[Q06] 删除列
来源：http://hz.jinqigfzy.top/gtbjfubrut.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.yj20258888.top/gtcpcqqwee.html

[Q07] 删除表
来源：http://hz.tanke756.top/gtagjvzboy.html

DROP TABLE IF EXISTS orders;
来源：http://hz.yonumen.top/gtmzxncbsd.html

[Q08] 创建普通索引
来源：http://hz.bjfxy.top/gtruoaqftx.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.shangyingyoupin.top/gtahomogze.html

[Q09] 创建唯一索引
来源：http://hz.sweek.top/gtpppnnnmh.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.cashguo.top/gtvcnffywv.html

[Q10] 插入单行
来源：http://hz.ydjk.org.cn/gtszhpmsqz.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.sysykeji.top/gtvdscycxc.html

[Q11] 一次插入多行
来源：http://hz.pycfn.com/gtzrtxkkrj.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.feifeiyinyue.top/gtcpzwhixc.html

[Q12] 插入后取自增 ID
来源：http://hz.9152youxi.cn/gtidehjvje.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.hywenlv.cn/gtgwgbogae.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.tianlin.xyz/gtrmbsmkih.html

[Q13] 忽略重复插入
来源：http://hz.daxiang520.top/gtlucwhctd.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.haohaochexian.top/gtmjvboapj.html

[Q14] 存在则更新（upsert）
来源：http://hz.hysaishi.cn/gturbyiuue.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.daxiang520.top/gtseyzhdzi.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.zhaomingkeji.xyz/gtyajzehtl.html

[Q15] 查询全部
来源：http://hz.svipenyu.cn/gtguacjsfl.html

SELECT * FROM users;
来源：http://hz.0kj1m.cn/gtgvdmyvql.html

[Q16] 查询指定列
来源：http://hz.dianchejie.cn/gtcerllrdk.html

SELECT id, name FROM users;
来源：http://hz.xuanzx.com/gtwiwxynhr.html

[Q17] 条件查询
来源：http://hz.dashuyun.cn/gtvcykttxk.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.wangshuangyany.cn/gtgpsfkgzl.html

[Q18] 模糊匹配
来源：http://hz.chenzaomai.com/gtubfojxfe.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.jinqigufen.top/gtqtsrawlk.html

[Q19] 范围查询
来源：http://hz.zdqjudy.top/gthzsqfptb.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.cheryme.top/gtokadlaci.html

[Q20] IN 列表
来源：http://hz.wangshuangyany.cn/gtphoxnklk.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.cucudq.cn/gtohvicwnw.html

[Q21] 空值判断
来源：http://hz.hammf.cn/gtjmwckscu.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.cucudq.cn/gtvbdowmtr.html

[Q22] 排序
来源：http://hz.smart0.xyz/gtiliebrnm.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.yvedp.cn/gtzhgvuvmr.html

[Q23] 分页
来源：http://hz.jqgfzy.top/gtueiveymt.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.gogol.net.cn/gtjqcjihip.html

[Q24] 去重
来源：http://hz.yonumen.top/gtascabnmx.html

SELECT DISTINCT city FROM users;
来源：http://hz.dianchejie.cn/gtbxdpybjc.html

[Q25] 只取前 N 条
来源：http://hz.zhengqikj.top/gtfnselmcd.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.xziqi.cn/gtroipefxm.html

[Q26] 计数
来源：http://hz.guannengcc.top/gtatatytgd.html

SELECT COUNT(*) FROM users;
来源：http://hz.guowangkeji.top/gtqdnohsqy.html

[Q27] 条件计数
来源：http://hz.birdmap.top/gtktnpwqfx.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.vqdsnc.cn/gtiddltrqa.html

[Q28] 求和与平均
来源：http://hz.aizwys.cn/gtkkugrzrl.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.yongpay.top/gtetcpjejo.html

[Q29] 最大最小值
来源：http://hz.ehwqpu.com/gtrjrjikys.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.jlsjyb.cn/gtnijqfucf.html

[Q30] 分组统计
来源：http://hz.sysykeji.top/gtaaitmjvg.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.zhoulong.xyz/gtsnmgjiqm.html

[Q31] 分组后过滤
来源：http://hz.jqgfzy.top/gtachwvwxm.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.xuanzx.com/gtwyxcesnm.html

[Q32] 分组拼接字符串
来源：http://hz.shangyingyoupin.top/gtfukiandc.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.jinqigufen.top/gtvoueoluy.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.aibaodan.cn/gtlqasutub.html

[Q33] 多列分组
来源：http://hz.smart0.xyz/gtfnafjvjt.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.birdmap.top/gtqhuavewe.html

[Q34] 每组取第一条
来源：http://hz.shanyushiyangkeji.top/gtudphuqkb.html

SELECT * FROM (
来源：http://hz.hywenlv.cn/gtkhryrkuh.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.redwolf501.top/gtzjwrqhis.html

) t WHERE rn = 1;
来源：http://hz.jinyuanbaomall.cn/gtzhgtkncv.html

[Q35] 内连接
来源：http://hz.aizwys.cn/gtzmlbawvx.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.sysykeji.top/gttxamihwf.html

[Q36] 左连接
来源：http://hz.ydzc1.top/gtkpzuwzmr.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.ydjk.org.cn/gtpdpmmvlv.html

[Q37] 右连接
来源：http://hz.wangshuangyany.cn/gtqnywyzdu.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.shangyingyoupin.top/gtfydobuzv.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.chenzaomai.com/gtrvgwfojd.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.xinyue.icu/gttytwtrge.html

[Q39] 自连接（查上下级）
来源：http://hz.jqgfzy.top/gtdaluzmgd.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.shzxlz.cn/gtaaqtwnck.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.sysykeji.top/gtyhypbcgc.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.xylfe.cn/gtqkrsmnmx.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.yongpay.top/gtwvyiwabq.html

[Q41] 多表连接
来源：http://hz.jinghuilouyu.cn/gthsrtcqge.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.hywenlv.cn/gtxtwerldr.html

JOIN users u ON u.id = o.user_id
来源：http://hz.fzhhl.top/gtbfuituwt.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.tanke756.top/gtstxrwdwk.html

[Q42] 连接条件附加过滤
来源：http://hz.yuanzhike.top/gtoifwhzib.html

SELECT u.name, o.amount FROM users u
来源：http://hz.iojbl.cn/gtdfhykgtj.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.gzhubu.top/gtkqtilwwo.html

[Q43] 标量子查询
来源：http://hz.zhiwuduotai.top/gtgzxiietf.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.dianchejie.cn/gtwemnjnph.html

[Q44] IN 子查询
来源：http://hz.jianghu66.top/gtwxgmhvvp.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.zhaomingkeji.xyz/gtenegdaob.html

[Q45] EXISTS 判断存在
来源：http://hz.vqdsnc.cn/gtjkknjvwt.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yueranfly.top/gtrmgtsisv.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.yj202588.top/gtarxxgxae.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yangfankeji.com/gtvsdbiuwr.html

[Q47] 与平均值比较
来源：http://hz.chenzaomai.com/gtnhyevgow.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.hywenlv.cn/gtmvptzkle.html

[Q48] CTE 公用表表达式
来源：http://hz.chenjidiqi.icu/gthbitjozn.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.cheryme.top/gtwdqqxwxb.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.zhixingplan.top/gtoakirtac.html

[Q49] 更新单行
来源：http://hz.hysaishi.cn/gtggnppjrl.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.yongpay.top/gtpldnozok.html

[Q50] 批量更新
来源：http://hz.yj20258.top/gtggvljokb.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.316326.xyz/gthblzmgjh.html

[Q51] 用子查询更新
来源：http://hz.zhixingplan.top/gtlwszjwog.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.0kj1m.cn/gtwatjnowe.html

[Q52] 删除指定行
来源：http://hz.nanxinkj.top/gtoflmqidd.html

DELETE FROM users WHERE id = 10;
来源：http://hz.tian-w.cn/gtdvheepkg.html

[Q53] 按条件删除
来源：http://hz.zhixingplan.top/gtsjpdyhhp.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.c1oappe.top/gtpzcofxyv.html

[Q54] 清空表
来源：http://hz.jinyuanbaomall.cn/gtxtwhkwba.html

TRUNCATE TABLE logs;
来源：http://hz.hywenlv.cn/gtbueejnjh.html

[Q55] 排名（并列占位）
来源：http://hz.xuetiantiany.cn/gtxhmqiess.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.yonumen.top/gteeqkgrnz.html

[Q56] 密集排名（并列不占位）
来源：http://hz.kuanghao11.cn/gtiosyjivc.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.hysaishi.cn/gtdkxcqamv.html

[Q57] 行号
来源：http://hz.sxryk.cn/gtgrwloaqs.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.dianchejie.cn/gtxgatqzkz.html

[Q58] 累计求和
来源：http://hz.cqqwz.cn/gtfyatabmu.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.zdqjudy.top/gtomeowlwr.html

[Q59] 分组内累计
来源：http://hz.jinqigfzy.top/gtpufyigch.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.gaohongyu789.top/gtsaxecsyc.html

[Q60] 取上一行 / 下一行
来源：http://hz.feifeiyinyue.top/gtogilyexh.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.shanyushiyangtech.top/gtczcggnpw.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.hongshengwenyu.top/gtajxgvugq.html

[Q61] 移动平均
来源：http://hz.kuanghao11.cn/gtjejyzbfz.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.shangyingyoupin.top/gtojnnxsru.html

[Q62] 分组占比
来源：http://hz.zhaomingkeji.xyz/gtdreoouzs.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.smart0.xyz/gteomfluls.html

[Q63] 开启事务
来源：http://hz.tian-w.cn/gtnhesnmak.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.redwolf501.top/gtxnohfnro.html

[Q64] 提交事务
来源：http://hz.ydjk.org.cn/gthwvzrmyv.html

COMMIT;
来源：http://hz.chenlongwang.top/gtpzcjskkh.html

[Q65] 回滚事务
来源：http://hz.zdqjudy.top/gtbamrpsfj.html

ROLLBACK;
来源：http://hz.dianchejie.cn/gtdfcpuhhe.html

[Q66] 行锁查询
来源：http://hz.feifeiyinyue.top/gtniyoyfav.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.52xcode.cn/gtryvyilcq.html

[Q67] 设置隔离级别
来源：http://hz.jinyuanbaomall.cn/gtlfksvtmd.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.smart0.xyz/gttoyhybwm.html

[Q68] 保存点
来源：http://hz.hammf.cn/gturctxizs.html

SAVEPOINT sp1;
来源：http://hz.redwolf501.top/gtxbizqrau.html

ROLLBACK TO sp1;
来源：http://hz.jinqigfzy.top/gtrrpgfoms.html

[Q69] 查看执行计划
来源：http://hz.xziqi.cn/gtqslwhire.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.smart0.xyz/gtyltrptze.html

[Q70] 更新统计信息
来源：http://hz.yuanzhike.top/gtbxngceqq.html

ANALYZE TABLE users;
来源：http://hz.zhijiandao.cn/gtoturcgbd.html

[Q71] 查看建表语句
来源：http://hz.gaohongyu789.top/gtrauypjnr.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.pengpengdd.cyou/gtbpdvuzxd.html

[Q72] 查看索引
来源：http://hz.chenzaomai.com/gtaqzofuwc.html

SHOW INDEX FROM users;
来源：http://hz.ywan-chungtsiang.top/gtjyooufhx.html

[Q73] 查看表状态
来源：http://hz.hnqzz.top/gthdpzixeg.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.chenjidiqi.icu/gtssiocqbf.html

[Q74] 强制使用索引
来源：http://hz.guowangkeji.top/gterxqvgut.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.yuanzhike.top/gtwlabnyvf.html

[Q75] 日期格式化
来源：http://hz.zhiwuduotai.top/gtjgjmbxnv.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.hysaishi.cn/gtafhoupkr.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.nwbrower.top/gtpzzgjbys.html

[Q76] 按天统计
来源：http://hz.sysykeji.top/gtqvtanton.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.feifeiyinyue.top/gtdyfqscsx.html

[Q77] 时间加减
来源：http://hz.pycfn.com/gtktrvzmrv.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.xuetiantiany.cn/gtgltjwufh.html

[Q78] 当前时间
来源：http://hz.xylfe.cn/gtljbtpwqp.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.yvedp.cn/gtinqjexho.html

[Q79] 字符串拼接
来源：http://hz.pengpengdd.cyou/gtdzmllyqe.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.ydzc1.top/gtkxkndnez.html

[Q80] 字符串截取
来源：http://hz.bjfxy.top/gtryupsbzw.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.hnxiangtu.top/gttbttbhve.html

[Q81] 字符串替换
来源：http://hz.xylfe.cn/gtmbhndfmv.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.yueranfly.top/gtdrszhvup.html

[Q82] 字符长度与字节长度
来源：http://hz.zhijiandao.cn/gtfvghplsc.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.zhiwuduotai.top/gtudhharkg.html

[Q83] 大小写转换
来源：http://hz.daria6918.cn/gtkoivheoo.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.pengpengdd.cyou/gtosxqhvwf.html

[Q84] 去除首尾空格
来源：http://hz.cheryme.top/gtqhvfkrmj.html

SELECT TRIM(name) FROM users;
来源：http://hz.sysykeji.top/gtbpwkkaei.html

[Q85] 数值取整
来源：http://hz.jinyuanbaomall.cn/gtnpbjiazf.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.quarkkingdee.top/gtpkotdrcq.html

[Q86] 读取 JSON 字段
来源：http://hz.gogol.net.cn/gtyaniztdx.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.quarkkingdee.top/gtkhdejsnw.html

[Q87] JSON 字段做条件
来源：http://hz.zhengqikj.top/gtlhjhmpul.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.yangfankeji.com/gttmvspmfo.html

[Q88] 行转列（条件聚合）
来源：http://hz.dashuyun.cn/gtebifjicj.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.dashuyun.cn/gtzgmmigby.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.xuanzx.com/gtissacjux.html

[Q89] 判断表是否存在
来源：http://hz.zycfv.cn/gtpwslqkkd.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.aizwys.cn/gtltcpvqtt.html

[Q90] 生成序号列
来源：http://hz.zdqjudy.top/gtfolpzlqc.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.316326.xyz/gtndwmmyny.html

================================================================================
来源：http://hz.guannengcc.top/gtwmlehjxc.html

R. Bash 专题
来源：http://hz.hywenlv.cn/gtbkuzjcze.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtgxjdpgrl.html

[R01] shebang 与严格模式
来源：http://hz.hnxiangtu.top/gtrhefflbz.html

#!/usr/bin/env bash
来源：http://hz.kuanghao11.cn/gthiqlxlus.html

set -euo pipefail
来源：http://hz.hysaishi.cn/gtkbczrwbd.html

[R02] 变量赋值与使用
来源：http://hz.tanke756.top/gtlkhpjmvh.html

name="Tom"; echo "$name"
来源：http://hz.quarkkingdee.top/gthygbeoeu.html

[R03] 只读变量
来源：http://hz.jqgufenzy.top/gtudiwmtvw.html

readonly PI=3.14
来源：http://hz.kuanghao11.cn/gtufgoffeu.html

[R04] 位置参数
来源：http://hz.jianghu66.top/gtpzkohykb.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.xylfe.cn/gtkbqdqxdo.html

[R05] 参数默认值
来源：http://hz.tanke756.top/gtykzknlxx.html

name="${1:-default}"
来源：http://hz.iojbl.cn/gtcwhlbdqk.html

[R06] 判断命令是否存在
来源：http://hz.cdnleiting.top/gtbitzveef.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.gogol.net.cn/gtcopqikga.html

[R07] if 判断文件
来源：http://hz.cucudq.cn/gtjizyuntl.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.yueranfly.top/gtnyegnkiu.html

[R08] 数值比较
来源：http://hz.yuanzhike.top/gtfdozfygo.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.zycfv.cn/gtytvmcwbb.html

[R09] 字符串比较
来源：http://hz.yueranfly.top/gtccrpzduw.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.haohaochexian.top/gtlqvhsmyd.html

[R10] 正则匹配
来源：http://hz.zhiwuduotai.top/gtwiiphgvv.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.jqgfzy.top/gthqbjtteu.html

[R11] case 多分支
来源：http://hz.cucudq.cn/gtcywaingy.html


<!-- 参考信息 -->