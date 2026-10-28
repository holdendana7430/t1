代发 wailian999

[P01] 生成 UUID
来源：http://hz.jinqigufen.top/gtpglucbdt.html

Py:   str(uuid.uuid4())
来源：http://hz.316326.xyz/gtedgpbyqj.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.hysaishi.cn/gtlxdqqklg.html

JS:   crypto.randomUUID()
来源：http://hz.yj20258.top/gtnupxxgzh.html

TS:   crypto.randomUUID()
来源：http://hz.haohaochexian.top/gtkerybgwk.html

Java: UUID.randomUUID().toString()
来源：http://hz.gotoacloud.top/gtsaiybkui.html

Go:   // 用 github.com/google/uuid
来源：http://hz.sufxvd.cn/gtylwlknfi.html

Ruby: SecureRandom.uuid
来源：http://hz.jyoumei.cn/gtsbufvyjz.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.nanxinkj.top/gtvofomltv.html

[P02] MD5 / SHA256 摘要
来源：http://hz.xziqi.cn/gtbnhdmndn.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.yj20258.top/gtappvivyb.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.ivvv.top/gtiqyschzu.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.guowangkeji.top/gtibgfrlof.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.havefunace.top/gtkjzhndbo.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.smart0.xyz/gtvcxlhnbf.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.ybcxt.top/gtaaffnonn.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.gotoacloud.top/gtwvkiysds.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.cashguo.top/gteacvnizr.html

[P03] 生成短随机字符串
来源：http://hz.yuanzhike.top/gtxvtlxvmp.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.daria6918.cn/gtsczrmrrf.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.ydzc1.top/gtosvzdfmw.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.andypj.xyz/gtdsfcnjdd.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jinyuanbaomall.cn/gticgermvh.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.ehwqpu.com/gtfoejrubk.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.yj20258888.top/gtadfweezg.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.hnxiangtu.top/gtpbobulfo.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.gotoacloud.top/gtmhlobyvh.html

[P04] 求长度
来源：http://hz.aizwys.cn/gtwrrfndxq.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.daria6918.cn/gtibejunaz.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.gogol.net.cn/gtycsapvkt.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.hnqzz.top/gtqwrqwqwp.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.meibo888.top/gtqwswblip.html

Java: list.size();  map.size();  s.length()
来源：http://hz.jinyuanbaomall.cn/gtnmkzeipn.html

Go:   len(arr);  len(m)
来源：http://hz.fzhhl.top/gtsuvwlrcv.html

Ruby: x.length;  x.size
来源：http://hz.jqgfzy.top/gtdiqdfgno.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.aibaodan.cn/gtiqcqwamw.html

[P05] 判断两个对象内容是否相等
来源：http://hz.iojbl.cn/gtpeselqgr.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.yj20258888.top/gtibgbuaba.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.jinqigufen.top/gtvpfzhuci.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.ydjk.org.cn/gtewrrfxgm.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.hysaishi.cn/gtqqzzhmme.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.vqdsnc.cn/gtrjraxkif.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.0kj1m.cn/gtuqccfjdr.html

Ruby: a == b
来源：http://hz.sufxvd.cn/gtmobritdx.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.xylfe.cn/gtjyylqiln.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.yvedp.cn/gtpekwguju.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.9152youxi.cn/gtiyudjwnz.html

PHP:  if (empty($x)) {}
来源：http://hz.cheryme.top/gtznzumpdr.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.yj20258.top/gtzatrnjuo.html

TS:   if (x == null) {}
来源：http://hz.shangyingyoupin.top/gtyiczkonz.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.quarkkingdee.top/gtifmjjkls.html

Go:   if x == nil {}
来源：http://hz.sweek.top/gtfnarkslm.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.daxiang520.top/gtcscobeqq.html

C#:   if (x is null) {}
来源：http://hz.quarkkingdee.top/gtvgmxekdj.html

[P07] 防抖与节流
来源：http://hz.daria6918.cn/gtozyxrcrd.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.aibaodan.cn/gtqcgiezzp.html

PHP:  // 手写时间戳比较
来源：http://hz.sweek.top/gtvxulijov.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.chenlongwang.top/gtamnfcxtl.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.smart0.xyz/gtyqbirffl.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.cucudq.cn/gttkivbzyx.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.yuxming.cn/gtldpjivps.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.cqqwz.cn/gtuejgcpgf.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.tanke756.top/gtvnxxudbs.html

[P08] 处理浮点精度问题
来源：http://hz.chenlongwang.top/gtwxlrohcu.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.fengsongda.top/gtlokzyqfj.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.daxiang520.top/gtiadhearp.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.jiagoushi.top/gtdbsihvxx.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.vqdsnc.cn/gtunlbijex.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.zhijiandao.cn/gtealzpncc.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.havefunace.top/gtapldcqpn.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.cucudq.cn/gtcarkxeps.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.shuidangran.top/gteydadgus.html

================================================================================
来源：http://hz.xinyue.icu/gtzdfoppny.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.dianchejie.cn/gtzqvkjzpf.html

================================================================================
来源：http://hz.andypj.xyz/gtbfbjeujs.html

[Q01] 创建表
来源：http://hz.gotoacloud.top/gtkjyvfzmy.html

CREATE TABLE users (
来源：http://hz.guannengcc.top/gtmvtozgjo.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.guowangkeji.top/gthkxuuauu.html

name VARCHAR(50) NOT NULL,
来源：http://hz.zhaomingkeji.xyz/gtsntswadj.html

email VARCHAR(100) UNIQUE,
来源：http://hz.jianghu66.top/gtiaimnkfl.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.yj20258888.top/gtykxheepd.html

);
来源：http://hz.wangshuangyany.cn/gtyhjqjyjc.html

[Q02] 创建带外键的表
来源：http://hz.xuetiantiany.cn/gtfecekgxm.html

CREATE TABLE orders (
来源：http://hz.svipenyu.cn/gtsgxhtskz.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.nanxinkj.top/gtlqzrrfsc.html

user_id INT NOT NULL,
来源：http://hz.zdqjudy.top/gtxwrwrvpq.html

amount DECIMAL(10, 2),
来源：http://hz.guannengcc.top/gtaoymdaoe.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.zhijiandao.cn/gtilhifrqm.html

);
来源：http://hz.jqgufenzy.top/gtyfopxtru.html

[Q03] 增加列
来源：http://hz.xziqi.cn/gtirpygzfn.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.xuanzx.com/gtlxqxomtl.html

[Q04] 修改列类型
来源：http://hz.iojbl.cn/gtotqewudz.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.andypj.xyz/gtymmkrley.html

[Q05] 重命名列
来源：http://hz.zhiwuduotai.top/gtjxzrwcip.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.52xcode.cn/gtdnztllih.html

[Q06] 删除列
来源：http://hz.andypj.xyz/gtxapsnlkz.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.ydzc1.top/gtnkwfcjyf.html

[Q07] 删除表
来源：http://hz.haohaochexian.top/gtqoolhtqx.html

DROP TABLE IF EXISTS orders;
来源：http://hz.shanyushiyangtech.top/gtatsbuswk.html

[Q08] 创建普通索引
来源：http://hz.yj20258888.top/gtgxsubbmg.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.sweek.top/gtykrtlxiw.html

[Q09] 创建唯一索引
来源：http://hz.guannengcc.top/gtietetwyf.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.svipenyu.cn/gttxtbiner.html

[Q10] 插入单行
来源：http://hz.yangfankeji.com/gtbgkqlgki.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.andypj.xyz/gtlqgmebdf.html

[Q11] 一次插入多行
来源：http://hz.yonumen.top/gtzcwyqabp.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.xinyue.icu/gtxnyhougv.html

[Q12] 插入后取自增 ID
来源：http://hz.sweek.top/gtbigeuguy.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.dashuyun.cn/gtalgxqvyd.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.tianlin.xyz/gtbybnsbwu.html

[Q13] 忽略重复插入
来源：http://hz.mhx1999.top/gtirheawre.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.chenlongwang.top/gtcrxreykh.html

[Q14] 存在则更新（upsert）
来源：http://hz.shuidangran.top/gttpaanwtx.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.dianchejie.cn/gtzkzatugi.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.mhx1999.top/gtvyikckfo.html

[Q15] 查询全部
来源：http://hz.bjfxy.top/gtxqeszebc.html

SELECT * FROM users;
来源：http://hz.shanyushiyangkeji.top/gtwjtemajq.html

[Q16] 查询指定列
来源：http://hz.wangshuangyany.cn/gtozuvundj.html

SELECT id, name FROM users;
来源：http://hz.daria6918.cn/gtjjehedef.html

[Q17] 条件查询
来源：http://hz.yuanzhike.top/gtftzlythl.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.jinqigufen.top/gtsshnxmxu.html

[Q18] 模糊匹配
来源：http://hz.cdnleiting.top/gtnklfiosv.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.ybcxt.top/gtutelhftv.html

[Q19] 范围查询
来源：http://hz.aizwys.cn/gtrkutexdi.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.daxiang520.top/gthodxzplh.html

[Q20] IN 列表
来源：http://hz.yangfankeji.com/gtilyfhknr.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.haohaochexian.top/gtnuryedjl.html

[Q21] 空值判断
来源：http://hz.jinghuilouyu.cn/gtjedqhmhe.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.dianchejie.cn/gtatjpiebt.html

[Q22] 排序
来源：http://hz.hysaishi.cn/gtlkobdbcj.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.jinyuanbaomall.cn/gtvoqxnsnh.html

[Q23] 分页
来源：http://hz.hongshengwenyu.top/gtghazqvbz.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.smart0.xyz/gtjbwluuel.html

[Q24] 去重
来源：http://hz.ivvv.top/gtdzzdxutf.html

SELECT DISTINCT city FROM users;
来源：http://hz.ehwqpu.com/gtscynllgq.html

[Q25] 只取前 N 条
来源：http://hz.fzhhl.top/gtgsmgxsls.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.cashguo.top/gtfcfpektp.html

[Q26] 计数
来源：http://hz.snrcjt.cn/gtqmeotube.html

SELECT COUNT(*) FROM users;
来源：http://hz.hnqzz.top/gtegimtikg.html

[Q27] 条件计数
来源：http://hz.fengsongda.top/gtsrusoxoe.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.andypj.xyz/gtjrzmlngz.html

[Q28] 求和与平均
来源：http://hz.guannengcc.top/gtuqenukig.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.daria6918.cn/gtwdpftzla.html

[Q29] 最大最小值
来源：http://hz.guannengcc.top/gtffmfgycz.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.shuidangran.top/gtthfeafib.html

[Q30] 分组统计
来源：http://hz.cdnleiting.top/gtjnrtdxws.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.hammf.cn/gtlqynxtal.html

[Q31] 分组后过滤
来源：http://hz.shanyushiyangtech.top/gtdyqcddfc.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.jinghuilouyu.cn/gttbcyimva.html

[Q32] 分组拼接字符串
来源：http://hz.nanxinkj.top/gtnrxijaqh.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.zhengqikj.top/gtztliyyev.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.vqdsnc.cn/gttazeathz.html

[Q33] 多列分组
来源：http://hz.guowangkeji.top/gtbgeviype.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.jianghu66.top/gtqonwagnr.html

[Q34] 每组取第一条
来源：http://hz.jyoumei.cn/gtjilzpyla.html

SELECT * FROM (
来源：http://hz.xziqi.cn/gtrbsqdyek.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.nanxinkj.top/gtuhfjecoe.html

) t WHERE rn = 1;
来源：http://hz.yuanzhike.top/gtbainmpev.html

[Q35] 内连接
来源：http://hz.c1oappe.top/gteraketmk.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.c1oappe.top/gtcsmimytn.html

[Q36] 左连接
来源：http://hz.gogol.net.cn/gttviylrry.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.hysaishi.cn/gtsyuwxxic.html

[Q37] 右连接
来源：http://hz.yueranfly.top/gtnlrramke.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.zhengqikj.top/gtxsmjbcxa.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.xziqi.cn/gtcbthumln.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.havefunace.top/gtqndxqddw.html

[Q39] 自连接（查上下级）
来源：http://hz.ehwqpu.com/gtjznnftle.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.zhijiandao.cn/gtjjexexue.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.52xcode.cn/gtyvbprtjr.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.gogol.net.cn/gtlwrrznxc.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.jinghuilouyu.cn/gtqbbksvkx.html

[Q41] 多表连接
来源：http://hz.ywan-chungtsiang.top/gtpamkwzas.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.jiagoushi.top/gtohsavhwc.html

JOIN users u ON u.id = o.user_id
来源：http://hz.feifeiyinyue.top/gtpjwpjiwo.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.zhoulong.xyz/gtzypdhnfj.html

[Q42] 连接条件附加过滤
来源：http://hz.hnxiangtu.top/gttnsektnw.html

SELECT u.name, o.amount FROM users u
来源：http://hz.tianlin.xyz/gtwlutsudi.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.pycfn.com/gtipiuefyr.html

[Q43] 标量子查询
来源：http://hz.chenjidiqi.icu/gtlhkkfzie.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.jlsjyb.cn/gtmzmwrrgq.html

[Q44] IN 子查询
来源：http://hz.jyoumei.cn/gtjwffgghe.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.yangfankeji.com/gteiqfxljb.html

[Q45] EXISTS 判断存在
来源：http://hz.jqgufenzy.top/gtqxuhudaw.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jinghuilouyu.cn/gtqzfatlkk.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.cqqwz.cn/gtixqmiutb.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jinqigfzy.top/gtvphqxczo.html

[Q47] 与平均值比较
来源：http://hz.tanke756.top/gttxtlvwnr.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.jlsjyb.cn/gtdmjoytzt.html

[Q48] CTE 公用表表达式
来源：http://hz.sxryk.cn/gttaggcfkf.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.cashguo.top/gtjrtekmjm.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.xuetiantiany.cn/gtbrxunusi.html

[Q49] 更新单行
来源：http://hz.hnxiangtu.top/gthpsoohpp.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.cucudq.cn/gtvzlqegea.html

[Q50] 批量更新
来源：http://hz.yj20258.top/gtroscnjik.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.guowangkeji.top/gtnbllrozt.html

[Q51] 用子查询更新
来源：http://hz.shuidangran.top/gtcsherrly.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.0kj1m.cn/gtjjkiqbqi.html

[Q52] 删除指定行
来源：http://hz.xingfuxueyuan.xyz/gtohsitmjc.html

DELETE FROM users WHERE id = 10;
来源：http://hz.zycfv.cn/gtxmoiseij.html

[Q53] 按条件删除
来源：http://hz.tian-w.cn/gtwcmazznt.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.ydzc1.top/gtipjxbvjy.html

[Q54] 清空表
来源：http://hz.cashguo.top/gtrzxohyye.html

TRUNCATE TABLE logs;
来源：http://hz.gaohongyu789.top/gtulytsqgx.html

[Q55] 排名（并列占位）
来源：http://hz.yanxiufei.cn/gtphlbethf.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.nanxinkj.top/gtdqbnaque.html

[Q56] 密集排名（并列不占位）
来源：http://hz.birdmap.top/gtqptvuyhj.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.ywan-chungtsiang.top/gtffkiypds.html

[Q57] 行号
来源：http://hz.iojbl.cn/gtufzndjzc.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.pycfn.com/gtpfvfcaka.html

[Q58] 累计求和
来源：http://hz.chenlongwang.top/gtraiurtfk.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.havefunace.top/gtojbjjmlz.html

[Q59] 分组内累计
来源：http://hz.ydzc1.top/gtyycstywy.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.ydjk.org.cn/gttxnsxvis.html

[Q60] 取上一行 / 下一行
来源：http://hz.bjfxy.top/gtliptxsxh.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.aibaodan.cn/gtjzdywbcg.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.hammf.cn/gtxjgntvoa.html

[Q61] 移动平均
来源：http://hz.shuidangran.top/gtmljywijx.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.yj20258.top/gtujwvmpwc.html

[Q62] 分组占比
来源：http://hz.52xcode.cn/gtixixiqlj.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.hammf.cn/gtyreoodjz.html

[Q63] 开启事务
来源：http://hz.tanke756.top/gttblovaui.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.yj20258888.top/gttmoqkqol.html

[Q64] 提交事务
来源：http://hz.zhijiandao.cn/gthlazklxp.html

COMMIT;
来源：http://hz.yj202588.top/gtqlihswiw.html

[Q65] 回滚事务
来源：http://hz.316326.xyz/gtzdqicvrn.html

ROLLBACK;
来源：http://hz.yanxiufei.cn/gtwbthpqll.html

[Q66] 行锁查询
来源：http://hz.ybcxt.top/gtchdezeph.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.ivvv.top/gtjiomnfcn.html

[Q67] 设置隔离级别
来源：http://hz.cheryme.top/gtkrmtjpce.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.feifeiyinyue.top/gtyrximcvz.html

[Q68] 保存点
来源：http://hz.xuanzx.com/gtzrugjyal.html

SAVEPOINT sp1;
来源：http://hz.chenlongwang.top/gtfgemrfvp.html

ROLLBACK TO sp1;
来源：http://hz.zhengqikj.top/gtesjrjnbu.html

[Q69] 查看执行计划
来源：http://hz.dashuyun.cn/gtsxzpxqjn.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.chenlongwang.top/gtagmykeho.html

[Q70] 更新统计信息
来源：http://hz.yonumen.top/gtwzgtvlwn.html

ANALYZE TABLE users;
来源：http://hz.zhoulong.xyz/gtweijygig.html

[Q71] 查看建表语句
来源：http://hz.smart0.xyz/gtjriocthf.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.zhijiandao.cn/gtkjlljjfx.html

[Q72] 查看索引
来源：http://hz.hysaishi.cn/gtwamzopvo.html

SHOW INDEX FROM users;
来源：http://hz.cdnleiting.top/gthbuglvxh.html

[Q73] 查看表状态
来源：http://hz.svipenyu.cn/gtukqwjmdm.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.zhoulong.xyz/gtspcnfnbv.html

[Q74] 强制使用索引
来源：http://hz.yangfankeji.com/gtngdurezh.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.yj20258.top/gtlyfnybtx.html

[Q75] 日期格式化
来源：http://hz.zhixingplan.top/gteaoasscs.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.0kj1m.cn/gtsinhxkgk.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.havefunace.top/gttolkpcpl.html

[Q76] 按天统计
来源：http://hz.zdqjudy.top/gtaabumpub.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.cashguo.top/gtgsxpmcsb.html

[Q77] 时间加减
来源：http://hz.yongpay.top/gtrvonusyr.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.sweek.top/gtyiuxjkro.html

[Q78] 当前时间
来源：http://hz.xuetiantiany.cn/gtxvbidqft.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.vqdsnc.cn/gtiahaqrqw.html

[Q79] 字符串拼接
来源：http://hz.hammf.cn/gtpvfeblvn.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.andypj.xyz/gtyjzpddzr.html

[Q80] 字符串截取
来源：http://hz.yueranfly.top/gtkkwpmhdc.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.bjfxy.top/gtirhfxhtg.html

[Q81] 字符串替换
来源：http://hz.gzhubu.top/gtfudusgyj.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.chenlongwang.top/gtxxngupar.html

[Q82] 字符长度与字节长度
来源：http://hz.tianlin.xyz/gtpymagzwu.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.hnqzz.top/gtpiuaynpp.html

[Q83] 大小写转换
来源：http://hz.xingfuxueyuan.xyz/gtjqjbnlhv.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.cucudq.cn/gtplycksvc.html

[Q84] 去除首尾空格
来源：http://hz.jinqigufen.top/gtdzyxpvrq.html

SELECT TRIM(name) FROM users;
来源：http://hz.nwbrower.top/gtjodckqub.html

[Q85] 数值取整
来源：http://hz.zhiwuduotai.top/gtbcgwnfps.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.mhx1999.top/gtgqmdjjgb.html

[Q86] 读取 JSON 字段
来源：http://hz.fengsongda.top/gtegkoesyt.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.snrcjt.cn/gtvrpatumq.html

[Q87] JSON 字段做条件
来源：http://hz.yj202588.top/gtimpejxnr.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.shanyushiyangkeji.top/gtvarjfxix.html

[Q88] 行转列（条件聚合）
来源：http://hz.tian-w.cn/gtcmzjymqh.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.zhoulong.xyz/gtuiegnbvw.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.sxryk.cn/gtwomouihn.html

[Q89] 判断表是否存在
来源：http://hz.jqgufenzy.top/gtscubhxop.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.hongshengwenyu.top/gtxxkxdxat.html

[Q90] 生成序号列
来源：http://hz.smart0.xyz/gtytfzmbwp.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.jianghu66.top/gtvjqkuufb.html

================================================================================
来源：http://hz.shuidangran.top/gthfkosakb.html

R. Bash 专题
来源：http://hz.jianghu66.top/gtdapexfci.html

================================================================================
来源：http://hz.fzhhl.top/gtbbjbsfzb.html

[R01] shebang 与严格模式
来源：http://hz.iojbl.cn/gtffldogdo.html

#!/usr/bin/env bash
来源：http://hz.ydjk.org.cn/gtrunjatfp.html

set -euo pipefail
来源：http://hz.chenlongwang.top/gtevfijmdt.html

[R02] 变量赋值与使用
来源：http://hz.sweek.top/gtjlrvccss.html

name="Tom"; echo "$name"
来源：http://hz.hongshengwenyu.top/gtuiacelbg.html

[R03] 只读变量
来源：http://hz.hnxiangtu.top/gtvhkspqjm.html

readonly PI=3.14
来源：http://hz.yj20258888.top/gtqpybzajw.html

[R04] 位置参数
来源：http://hz.ivvv.top/gtbmmhemhl.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.yongpay.top/gthnrlolfs.html

[R05] 参数默认值
来源：http://hz.yonumen.top/gtpckcvsci.html

name="${1:-default}"
来源：http://hz.cashguo.top/gtjrtoxlgv.html

[R06] 判断命令是否存在
来源：http://hz.cashguo.top/gtxjyoivkn.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.zhijiandao.cn/gtvaofvbyp.html

[R07] if 判断文件
来源：http://hz.yanxiufei.cn/gtriewjjrw.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.ybcxt.top/gtlofijdes.html

[R08] 数值比较
来源：http://hz.cheryme.top/gtkdemtgvo.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.wangshuangyany.cn/gtwyigrxxr.html

[R09] 字符串比较
来源：http://hz.hywenlv.cn/gtbdgnowxs.html


<!-- 参考信息 -->