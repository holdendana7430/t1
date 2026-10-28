代发 wailian999

[P01] 生成 UUID
来源：http://hz.sxryk.cn/gtvemuaepp.html

Py:   str(uuid.uuid4())
来源：http://hz.smart0.xyz/gtdauwzyav.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.guannengcc.top/gtjmkqbmrd.html

JS:   crypto.randomUUID()
来源：http://hz.gaohongyu789.top/gtchehuyfw.html

TS:   crypto.randomUUID()
来源：http://hz.yj202588.top/gtgjhovzxo.html

Java: UUID.randomUUID().toString()
来源：http://hz.cqqwz.cn/gtzoctbpow.html

Go:   // 用 github.com/google/uuid
来源：http://hz.yj20258.top/gtqznpbona.html

Ruby: SecureRandom.uuid
来源：http://hz.jiagoushi.top/gtxkoddokt.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.yj20258.top/gtmvfjsfjq.html

[P02] MD5 / SHA256 摘要
来源：http://hz.9152youxi.cn/gtpwtdqloe.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.sweek.top/gthjzofemn.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.pengpengdd.cyou/gtfehwehyt.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.havefunace.top/gtwhahvmfq.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.jqgfzy.top/gtbwmqsnea.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.xziqi.cn/gtooftqxyb.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.haohaochexian.top/gtiwvqydow.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.xingfuxueyuan.xyz/gtfblzcwvc.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.sweek.top/gtdcpyjcqi.html

[P03] 生成短随机字符串
来源：http://hz.chenzaomai.com/gtloufweye.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.haohaochexian.top/gtmvdttdae.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.nwbrower.top/gtvfpbxtts.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.zhengqikj.top/gtnuynhcdv.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.dashuyun.cn/gtorurcwzp.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.yj20258888.top/gtuwbbzahu.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.tanke756.top/gtipddfrpz.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.hnxiangtu.top/gtfeltqelt.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.cheryme.top/gtcqogtghx.html

[P04] 求长度
来源：http://hz.hammf.cn/gtvihzksih.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.hfpthk.cn/gtwieexzhz.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.guowangkeji.top/gtbpucwsdj.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.316326.xyz/gtsszkozxn.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yj20258.top/gtvxsxrbbw.html

Java: list.size();  map.size();  s.length()
来源：http://hz.hongshengwenyu.top/gthtyngzlr.html

Go:   len(arr);  len(m)
来源：http://hz.xziqi.cn/gtpactanmg.html

Ruby: x.length;  x.size
来源：http://hz.guannengcc.top/gtxgkcwzsy.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.ydjk.org.cn/gtsqflziho.html

[P05] 判断两个对象内容是否相等
来源：http://hz.chenjidiqi.icu/gtwlqxtjsd.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.jinyuanbaomall.cn/gtctitxywk.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.yuxming.cn/gtitngryoj.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.zhengqikj.top/gtbdzfkifa.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.dashuyun.cn/gtraipqwnb.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.9152youxi.cn/gtaqxieytp.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.xylfe.cn/gtsolsvcka.html

Ruby: a == b
来源：http://hz.yvedp.cn/gtjnnhstex.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.hnqzz.top/gtghcabmak.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.sweek.top/gtygmfwqvk.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.zhoulong.xyz/gtfrjsxkgg.html

PHP:  if (empty($x)) {}
来源：http://hz.svipenyu.cn/gttysebrdf.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.snrcjt.cn/gtflhulsid.html

TS:   if (x == null) {}
来源：http://hz.nanxuanxn.top/gtxyzvcjro.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.ybcxt.top/gtedkjoodn.html

Go:   if x == nil {}
来源：http://hz.pycfn.com/gtbkkwnqlu.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.zhengqikj.top/gtbzenqcxp.html

C#:   if (x is null) {}
来源：http://hz.zhengqikj.top/gtaggponow.html

[P07] 防抖与节流
来源：http://hz.meibo888.top/gtjpkilteg.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.gotoacloud.top/gtbomyfkcv.html

PHP:  // 手写时间戳比较
来源：http://hz.ivvv.top/gtjyjjwxnr.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yueranfly.top/gthuuoayaj.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yangfankeji.com/gtgohwryzj.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.ppjwa.cn/gttiuifbnf.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.snrcjt.cn/gtrwhuharx.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.dianchejie.cn/gthpeuupkh.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.0kj1m.cn/gtqlnncqsg.html

[P08] 处理浮点精度问题
来源：http://hz.yj202588.top/gtomhhcknu.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.pengpengdd.cyou/gtvjbdgouh.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.jinqigufen.top/gtonmuktjy.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.shzxlz.cn/gtbridhxgv.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.cqqwz.cn/gtrgdvmfts.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.chenjidiqi.icu/gtjxhqkdhy.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.shuidangran.top/gtwiyatjtp.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.fzhhl.top/gtpcbydyke.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.quarkkingdee.top/gtyylpeesj.html

================================================================================
来源：http://hz.hywenlv.cn/gtbhmejebj.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.sufxvd.cn/gtswhshtrp.html

================================================================================
来源：http://hz.guannengcc.top/gtxgwfymlq.html

[Q01] 创建表
来源：http://hz.fzhhl.top/gtyurqesvi.html

CREATE TABLE users (
来源：http://hz.ehwqpu.com/gtuximtesi.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.cqqwz.cn/gtgclwkman.html

name VARCHAR(50) NOT NULL,
来源：http://hz.daxiang520.top/gtxpdselfi.html

email VARCHAR(100) UNIQUE,
来源：http://hz.svipenyu.cn/gtuohevjur.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.yonumen.top/gtnbfghcvh.html

);
来源：http://hz.ybcxt.top/gtsncvodgb.html

[Q02] 创建带外键的表
来源：http://hz.xuanzx.com/gtujjertbl.html

CREATE TABLE orders (
来源：http://hz.daxiang520.top/gtvujlcpxa.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.shanyushiyangtech.top/gtqsgjnnnd.html

user_id INT NOT NULL,
来源：http://hz.hnxiangtu.top/gtydytfqms.html

amount DECIMAL(10, 2),
来源：http://hz.jqgfzy.top/gtmzybtxnp.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.sweek.top/gtsuhhvdwf.html

);
来源：http://hz.gogol.net.cn/gtxmdtcfkb.html

[Q03] 增加列
来源：http://hz.zdqjudy.top/gtiqsqhsxd.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.jinqigufen.top/gtgzslkkiy.html

[Q04] 修改列类型
来源：http://hz.yangfankeji.com/gtwidahgae.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.xuanzx.com/gtjybkphrd.html

[Q05] 重命名列
来源：http://hz.dashuyun.cn/gtxjxsfwcc.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.aizwys.cn/gtygsldghv.html

[Q06] 删除列
来源：http://hz.nanxinkj.top/gtggafnrar.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.fengsongda.top/gtdzgmjpzo.html

[Q07] 删除表
来源：http://hz.yuxming.cn/gtoejvzqim.html

DROP TABLE IF EXISTS orders;
来源：http://hz.daria6918.cn/gtpprgqisb.html

[Q08] 创建普通索引
来源：http://hz.hammf.cn/gtalrfgukl.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.tianlin.xyz/gtvwkszubo.html

[Q09] 创建唯一索引
来源：http://hz.zhongyouzk.top/gthbehcqhd.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.fzhhl.top/gtnkimiawh.html

[Q10] 插入单行
来源：http://hz.kuanghao11.cn/gtlilruhqt.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.c1oappe.top/gtqacatnmk.html

[Q11] 一次插入多行
来源：http://hz.yvedp.cn/gtuwonnlmf.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.wangshuangyany.cn/gtupcxjopj.html

[Q12] 插入后取自增 ID
来源：http://hz.shuidangran.top/gthtasuevb.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.c1oappe.top/gtyvgbisap.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.snrcjt.cn/gtjteizrdc.html

[Q13] 忽略重复插入
来源：http://hz.aibaodan.cn/gtsdvjkiud.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.wangdashe.top/gtxfeieihf.html

[Q14] 存在则更新（upsert）
来源：http://hz.jlsjyb.cn/gtxpjblmrh.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.yj20258.top/gtlmqhfsif.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.sweek.top/gttadmecug.html

[Q15] 查询全部
来源：http://hz.jlsjyb.cn/gtzkojtcbc.html

SELECT * FROM users;
来源：http://hz.fengsongda.top/gtyodfutgn.html

[Q16] 查询指定列
来源：http://hz.zycfv.cn/gtirqvhton.html

SELECT id, name FROM users;
来源：http://hz.chenlongwang.top/gtiatvmsly.html

[Q17] 条件查询
来源：http://hz.ehwqpu.com/gtteypbzny.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.xuetiantiany.cn/gtqztdmjbp.html

[Q18] 模糊匹配
来源：http://hz.bjfxy.top/gtuqbydcgx.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.jianghu66.top/gtudmtqfhb.html

[Q19] 范围查询
来源：http://hz.andypj.xyz/gtcpziblic.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.jianghu66.top/gtowstovth.html

[Q20] IN 列表
来源：http://hz.yj20258888.top/gtkncptjng.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.cashguo.top/gtepeucwut.html

[Q21] 空值判断
来源：http://hz.svipenyu.cn/gtramcbejk.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.wangshuangyany.cn/gtyxmrvvnr.html

[Q22] 排序
来源：http://hz.xylfe.cn/gtowjdksws.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.9152youxi.cn/gtylyrrzds.html

[Q23] 分页
来源：http://hz.zhiwuduotai.top/gtdhaovrjh.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.yanxiufei.cn/gtguvhlveq.html

[Q24] 去重
来源：http://hz.nanxuanxn.top/gtpycjnxmp.html

SELECT DISTINCT city FROM users;
来源：http://hz.yj202588.top/gtgoktjzez.html

[Q25] 只取前 N 条
来源：http://hz.bjfxy.top/gthwyssppn.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.redwolf501.top/gtnsybrnpq.html

[Q26] 计数
来源：http://hz.zhoulong.xyz/gtdjamowpq.html

SELECT COUNT(*) FROM users;
来源：http://hz.shanyushiyangkeji.top/gtdcsezgsg.html

[Q27] 条件计数
来源：http://hz.yj20258888.top/gtpoizheww.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.sufxvd.cn/gtcjfnznmk.html

[Q28] 求和与平均
来源：http://hz.daxiang520.top/gtgtvgjevh.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.bjfxy.top/gtgotgbxho.html

[Q29] 最大最小值
来源：http://hz.daria6918.cn/gtylgnlqhu.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.dashuyun.cn/gtxtlfoajm.html

[Q30] 分组统计
来源：http://hz.smart0.xyz/gtbjvbosuh.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.zhengqikj.top/gtcfyxfxut.html

[Q31] 分组后过滤
来源：http://hz.jinqigfzy.top/gtztgmqrwh.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.ivvv.top/gtkocebaru.html

[Q32] 分组拼接字符串
来源：http://hz.ydzc1.top/gtshcfeaki.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.zdqjudy.top/gteogsfios.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.sufxvd.cn/gtkgolouqp.html

[Q33] 多列分组
来源：http://hz.fengsongda.top/gttnquivns.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.feifeiyinyue.top/gtbvlcltxp.html

[Q34] 每组取第一条
来源：http://hz.meibo888.top/gtgchwpksf.html

SELECT * FROM (
来源：http://hz.smart0.xyz/gtmlrybcgn.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.jlsjyb.cn/gtvgqaxtzc.html

) t WHERE rn = 1;
来源：http://hz.aizwys.cn/gtmyugjeue.html

[Q35] 内连接
来源：http://hz.jianghu66.top/gtjhjhjpdv.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.jianghu66.top/gtsmopppri.html

[Q36] 左连接
来源：http://hz.shanyushiyangtech.top/gtcdhkqihi.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.bjfxy.top/gtlchpdfzn.html

[Q37] 右连接
来源：http://hz.tanke756.top/gtjzdgfvfo.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.hysaishi.cn/gtyiynxwxr.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.yueranfly.top/gtpuzdzajr.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.fzhhl.top/gtsnugqhjn.html

[Q39] 自连接（查上下级）
来源：http://hz.sysykeji.top/gtzedrlnlx.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.pycfn.com/gtqkwoxila.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.sysykeji.top/gtzdebrsnc.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.pycfn.com/gtdeeexuaa.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.meibo888.top/gtksmigqmv.html

[Q41] 多表连接
来源：http://hz.sufxvd.cn/gtnzpfcjwz.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.zhoulong.xyz/gtebxkozye.html

JOIN users u ON u.id = o.user_id
来源：http://hz.pengpengdd.cyou/gtctatrqtu.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.jqgufenzy.top/gtoznfnamx.html

[Q42] 连接条件附加过滤
来源：http://hz.jqgfzy.top/gtriwmnhrw.html

SELECT u.name, o.amount FROM users u
来源：http://hz.gogol.net.cn/gtporbyzga.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.redwolf501.top/gtaqdymzgc.html

[Q43] 标量子查询
来源：http://hz.xuanzx.com/gtbawfthmy.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.pengpengdd.cyou/gtkujjkdvd.html

[Q44] IN 子查询
来源：http://hz.daxiang520.top/gttpdpvtmm.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.ywan-chungtsiang.top/gtodzfsqti.html

[Q45] EXISTS 判断存在
来源：http://hz.hongshengwenyu.top/gtizkyvtmm.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zhengqikj.top/gtrjsnpwpf.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.hfpthk.cn/gtqgliwmsn.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.shanyushiyangtech.top/gtxzivxvot.html

[Q47] 与平均值比较
来源：http://hz.vqdsnc.cn/gtomtajhdk.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.sxryk.cn/gtoponjzqh.html

[Q48] CTE 公用表表达式
来源：http://hz.yueranfly.top/gtvtezejqs.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.shzxlz.cn/gtkfnstmvi.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.sufxvd.cn/gtznlgwcwz.html

[Q49] 更新单行
来源：http://hz.zhijiandao.cn/gtczdfjvjn.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.zhijiandao.cn/gtjeshoull.html

[Q50] 批量更新
来源：http://hz.9152youxi.cn/gtbrcmhkal.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.jianghu66.top/gtukormpcs.html

[Q51] 用子查询更新
来源：http://hz.sxryk.cn/gtvfmwngeo.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.shanyushiyangtech.top/gtklkfaklr.html

[Q52] 删除指定行
来源：http://hz.yongpay.top/gththqpzvi.html

DELETE FROM users WHERE id = 10;
来源：http://hz.yvedp.cn/gtilxulwfb.html

[Q53] 按条件删除
来源：http://hz.jinghuilouyu.cn/gtncgpwafw.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.feifeiyinyue.top/gtruwkiknk.html

[Q54] 清空表
来源：http://hz.ydjk.org.cn/gtpxdqyjfx.html

TRUNCATE TABLE logs;
来源：http://hz.zhiwuduotai.top/gtazawtlur.html

[Q55] 排名（并列占位）
来源：http://hz.cdnleiting.top/gtiyhkuyii.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.zhixingplan.top/gtjyzlegja.html

[Q56] 密集排名（并列不占位）
来源：http://hz.shanyushiyangtech.top/gtrvlcugwv.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.snrcjt.cn/gtttucdtnr.html

[Q57] 行号
来源：http://hz.shzxlz.cn/gtuzhyqtbo.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.ywan-chungtsiang.top/gtlnarzorf.html

[Q58] 累计求和
来源：http://hz.gzhubu.top/gtxvnlnosz.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.cheryme.top/gtpjlpycdn.html

[Q59] 分组内累计
来源：http://hz.yuanzhike.top/gtwzzfdcks.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.fzhhl.top/gtwhhggjbc.html

[Q60] 取上一行 / 下一行
来源：http://hz.c1oappe.top/gtwvftvsru.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.tianlin.xyz/gtdlajcyrf.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.hywenlv.cn/gteqsrvjzo.html

[Q61] 移动平均
来源：http://hz.ydjk.org.cn/gtfcgmfbeg.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.snrcjt.cn/gtxzcxvsus.html

[Q62] 分组占比
来源：http://hz.zdqjudy.top/gtndjickoz.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.pycfn.com/gtqnjvlojo.html

[Q63] 开启事务
来源：http://hz.jiagoushi.top/gtnypmmihz.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.andypj.xyz/gtaemalank.html

[Q64] 提交事务
来源：http://hz.jqgufenzy.top/gtjvqkbnsy.html

COMMIT;
来源：http://hz.yanxiufei.cn/gtaztvdjxd.html

[Q65] 回滚事务
来源：http://hz.sweek.top/gtuiwbnyaa.html

ROLLBACK;
来源：http://hz.zhongyouzk.top/gtnmxzckzb.html

[Q66] 行锁查询
来源：http://hz.xinyue.icu/gtmektxoyy.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.shanyushiyangkeji.top/gtbqjaokfa.html

[Q67] 设置隔离级别
来源：http://hz.tian-w.cn/gtdydmwuti.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.52xcode.cn/gtfxddhtwd.html

[Q68] 保存点
来源：http://hz.zhoulong.xyz/gtohzsrrzz.html

SAVEPOINT sp1;
来源：http://hz.shangyingyoupin.top/gtlmpsihnv.html

ROLLBACK TO sp1;
来源：http://hz.316326.xyz/gtwrivuvea.html

[Q69] 查看执行计划
来源：http://hz.jianghu66.top/gttlkstjui.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.chenjidiqi.icu/gtyoqlxeus.html

[Q70] 更新统计信息
来源：http://hz.shangyingyoupin.top/gtjwatycof.html

ANALYZE TABLE users;
来源：http://hz.iojbl.cn/gttvwabatm.html

[Q71] 查看建表语句
来源：http://hz.snrcjt.cn/gtyugxpiir.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.gotoacloud.top/gtaaasbwqa.html

[Q72] 查看索引
来源：http://hz.chenjidiqi.icu/gteggpebks.html

SHOW INDEX FROM users;
来源：http://hz.zycfv.cn/gtarbrifnk.html

[Q73] 查看表状态
来源：http://hz.wangdashe.top/gtznhtskyf.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.ivvv.top/gttcwvusng.html

[Q74] 强制使用索引
来源：http://hz.yuxming.cn/gtkibtghis.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.redwolf501.top/gtcmzhlzqs.html

[Q75] 日期格式化
来源：http://hz.gzhubu.top/gtzwocjdqp.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.quarkkingdee.top/gtvjkciiyw.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.cashguo.top/gtrnkrihsz.html

[Q76] 按天统计
来源：http://hz.ydjk.org.cn/gtykyirntm.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.shzxlz.cn/gtrwsmeysi.html

[Q77] 时间加减
来源：http://hz.jlsjyb.cn/gthgjywatk.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.zhijiandao.cn/gtcmuuuyvs.html

[Q78] 当前时间
来源：http://hz.cashguo.top/gtjqmitkcj.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.jinyuanbaomall.cn/gtmzbwxjzq.html

[Q79] 字符串拼接
来源：http://hz.kuanghao11.cn/gtfivnwhmf.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.316326.xyz/gtgsngnrdp.html

[Q80] 字符串截取
来源：http://hz.zycfv.cn/gtthxprsti.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.cdnleiting.top/gtfldwlbyu.html

[Q81] 字符串替换
来源：http://hz.hywenlv.cn/gtftxyivua.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.jinghuilouyu.cn/gtkiyfnzxe.html

[Q82] 字符长度与字节长度
来源：http://hz.xuanzx.com/gtpzpkeqqp.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.hongshengwenyu.top/gtnptrengy.html

[Q83] 大小写转换
来源：http://hz.nwbrower.top/gtkunqlcqb.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.cdnleiting.top/gtpodawnak.html

[Q84] 去除首尾空格
来源：http://hz.shuidangran.top/gtlwzqtphx.html

SELECT TRIM(name) FROM users;
来源：http://hz.pengpengdd.cyou/gtaumooxlg.html

[Q85] 数值取整
来源：http://hz.sysykeji.top/gttveylqyf.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.jyoumei.cn/gtjlaibkbi.html

[Q86] 读取 JSON 字段
来源：http://hz.cdnleiting.top/gtenlrhzrt.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.hnxiangtu.top/gtaqnbvwde.html

[Q87] JSON 字段做条件
来源：http://hz.jianghu66.top/gtbmkzxhzn.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.zhixingplan.top/gtulwfwojq.html

[Q88] 行转列（条件聚合）
来源：http://hz.yj20258.top/gtstpctvgj.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.yj20258888.top/gthzjkgckn.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.iojbl.cn/gtcjggczkf.html

[Q89] 判断表是否存在
来源：http://hz.daria6918.cn/gtfnmgloof.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.wangdashe.top/gtiutehcyc.html

[Q90] 生成序号列
来源：http://hz.hnxiangtu.top/gtsfahtops.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.hnqzz.top/gtxnmvxmtx.html

================================================================================
来源：http://hz.redwolf501.top/gtnghtyfyj.html

R. Bash 专题
来源：http://hz.c1oappe.top/gtlreendfm.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtuwjbabbu.html

[R01] shebang 与严格模式
来源：http://hz.guannengcc.top/gtfqcqkiwa.html

#!/usr/bin/env bash
来源：http://hz.shanyushiyangtech.top/gtvuqyugke.html

set -euo pipefail
来源：http://hz.ydzc1.top/gtyhrhzlyw.html

[R02] 变量赋值与使用
来源：http://hz.ydjk.org.cn/gtoajdsrij.html

name="Tom"; echo "$name"
来源：http://hz.hnqzz.top/gtrwclbppo.html

[R03] 只读变量
来源：http://hz.shangyingyoupin.top/gtwlhiljwx.html

readonly PI=3.14
来源：http://hz.sysykeji.top/gtzuuqqred.html

[R04] 位置参数
来源：http://hz.hywenlv.cn/gtdkadwtvl.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.chenjidiqi.icu/gtdbmhezgu.html

[R05] 参数默认值
来源：http://hz.tanke756.top/gtjtcvhhdt.html

name="${1:-default}"
来源：http://hz.aibaodan.cn/gtrrbmszka.html

[R06] 判断命令是否存在
来源：http://hz.fzhhl.top/gticexcgjk.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.dashuyun.cn/gtsjwrynhh.html

[R07] if 判断文件
来源：http://hz.tian-w.cn/gtctqvnysx.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.zhixingplan.top/gtladymqik.html

[R08] 数值比较
来源：http://hz.daxiang520.top/gtqwvjwyub.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.wangshuangyany.cn/gtbttnfdof.html

[R09] 字符串比较
来源：http://hz.jqgfzy.top/gtqonoukmb.html


<!-- 参考信息 -->