代发 wailian999

[P01] 生成 UUID
来源：http://hz.zhaomingkeji.xyz/gtkamotupn.html

Py:   str(uuid.uuid4())
来源：http://hz.ydjk.org.cn/gtvuarygef.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.cashguo.top/gtivfnoquy.html

JS:   crypto.randomUUID()
来源：http://hz.snrcjt.cn/gtagrlilsx.html

TS:   crypto.randomUUID()
来源：http://hz.jqgufenzy.top/gtrgbrusmw.html

Java: UUID.randomUUID().toString()
来源：http://hz.hywenlv.cn/gtqtihxgwr.html

Go:   // 用 github.com/google/uuid
来源：http://hz.yj20258888.top/gtgpaavuce.html

Ruby: SecureRandom.uuid
来源：http://hz.yongpay.top/gtdjckvfzl.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.yj202588.top/gtbjhsbgqt.html

[P02] MD5 / SHA256 摘要
来源：http://hz.hammf.cn/gtremefwap.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.xingfuxueyuan.xyz/gtylxibjwe.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.andypj.xyz/gtcihihesg.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.52xcode.cn/gtmzlhlgee.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.jianghu66.top/gtqtkuqyrn.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.ivvv.top/gtlkrahyyf.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.smart0.xyz/gtujnqtmqy.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.ehwqpu.com/gteejjwyes.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.zhoulong.xyz/gtiipkaevb.html

[P03] 生成短随机字符串
来源：http://hz.wangdashe.top/gtlbcotybn.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.chenzaomai.com/gtkczeafgy.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.zycfv.cn/gtdpmfiouh.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yj20258.top/gtjchaegkl.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yongpay.top/gtiqgxtrvl.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.yongpay.top/gtmxenomsa.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.jyoumei.cn/gtegyfvlbr.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.gaohongyu789.top/gtoqyiyuou.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.hfpthk.cn/gtdneohrfy.html

[P04] 求长度
来源：http://hz.cqqwz.cn/gtmamlpgsd.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.nanxinkj.top/gttotzztag.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.xuetiantiany.cn/gtqvnggnza.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.gotoacloud.top/gtnqhddhdo.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.daria6918.cn/gtwcupeckx.html

Java: list.size();  map.size();  s.length()
来源：http://hz.shanyushiyangkeji.top/gtecaklzfg.html

Go:   len(arr);  len(m)
来源：http://hz.smart0.xyz/gtusfjmpym.html

Ruby: x.length;  x.size
来源：http://hz.zhixingplan.top/gtjfqccrbc.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.yuxming.cn/gtbxbqxtom.html

[P05] 判断两个对象内容是否相等
来源：http://hz.chenlongwang.top/gtdfdooezf.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.yueranfly.top/gtwcrhuccm.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.yj20258888.top/gtranqraku.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.jqgufenzy.top/gtbfpuiwcj.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.snrcjt.cn/gtoxrhybot.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.yvedp.cn/gtoeokzwla.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.snrcjt.cn/gtkpcxswwp.html

Ruby: a == b
来源：http://hz.xinyue.icu/gtrbovrgyh.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.bjfxy.top/gtqjzmaxkz.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.hywenlv.cn/gttygoycwd.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.cheryme.top/gtnltrceea.html

PHP:  if (empty($x)) {}
来源：http://hz.nwbrower.top/gtvcgmvpro.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.jqgufenzy.top/gteoezybxj.html

TS:   if (x == null) {}
来源：http://hz.ydjk.org.cn/gtwwoqpkxm.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.quarkkingdee.top/gtwfmcxbji.html

Go:   if x == nil {}
来源：http://hz.birdmap.top/gtydnlbbuc.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.cucudq.cn/gtwynegnhg.html

C#:   if (x is null) {}
来源：http://hz.fengsongda.top/gtetbtouxn.html

[P07] 防抖与节流
来源：http://hz.cucudq.cn/gtwvzcjadc.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.nanxinkj.top/gtlyziawlj.html

PHP:  // 手写时间戳比较
来源：http://hz.xuetiantiany.cn/gtydxnnggt.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.daxiang520.top/gtrzckpqei.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.shangyingyoupin.top/gtjjjwwxhf.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.chenzaomai.com/gtbkpkkbfu.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.xinyue.icu/gtalywahmk.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.haohaochexian.top/gtemehklve.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.jiagoushi.top/gtmaufekhc.html

[P08] 处理浮点精度问题
来源：http://hz.jinqigfzy.top/gtgmipddgv.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.jinqigufen.top/gtwwvxctzu.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.cqqwz.cn/gtaaldqvlz.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.dashuyun.cn/gtfxsklytd.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.cashguo.top/gtfhkaafze.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.shangyingyoupin.top/gthggkpkay.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.hnqzz.top/gtocghnkaz.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.52xcode.cn/gtsrujnmik.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.tianlin.xyz/gtmqaqxoht.html

================================================================================
来源：http://hz.mhx1999.top/gtoshstpcl.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.zhengqikj.top/gtuxqrlmal.html

================================================================================
来源：http://hz.xinyue.icu/gtnjfiwvvo.html

[Q01] 创建表
来源：http://hz.316326.xyz/gtjgfcwzik.html

CREATE TABLE users (
来源：http://hz.hongshengwenyu.top/gtfejcghtj.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.zhaomingkeji.xyz/gtgtjvypoh.html

name VARCHAR(50) NOT NULL,
来源：http://hz.shanyushiyangtech.top/gtkpxhdyhl.html

email VARCHAR(100) UNIQUE,
来源：http://hz.jiagoushi.top/gtqsgeiuuz.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.tanke756.top/gtoztedrzi.html

);
来源：http://hz.ydzc1.top/gtessbpqmy.html

[Q02] 创建带外键的表
来源：http://hz.zhixingplan.top/gtfihzkmga.html

CREATE TABLE orders (
来源：http://hz.guowangkeji.top/gtsuxsgoqz.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.nwbrower.top/gtsutkokhy.html

user_id INT NOT NULL,
来源：http://hz.jinghuilouyu.cn/gtfxylrmrm.html

amount DECIMAL(10, 2),
来源：http://hz.feifeiyinyue.top/gtoplovhts.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.svipenyu.cn/gtsxlyxxyt.html

);
来源：http://hz.hnqzz.top/gtrkzjiabh.html

[Q03] 增加列
来源：http://hz.bjfxy.top/gtlefkykae.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.chenlongwang.top/gtzpgpquhf.html

[Q04] 修改列类型
来源：http://hz.hongshengwenyu.top/gtjctqgdvd.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.ivvv.top/gtehqtwomf.html

[Q05] 重命名列
来源：http://hz.cashguo.top/gtyrdefkpf.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.ppjwa.cn/gtvyybigjt.html

[Q06] 删除列
来源：http://hz.zhixingplan.top/gtgvuttsjm.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.zycfv.cn/gtudjqhkvg.html

[Q07] 删除表
来源：http://hz.yj20258.top/gtsonjgsch.html

DROP TABLE IF EXISTS orders;
来源：http://hz.zhijiandao.cn/gtqrzrrlrk.html

[Q08] 创建普通索引
来源：http://hz.zycfv.cn/gtaotfmkec.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.52xcode.cn/gtyzyxvjnf.html

[Q09] 创建唯一索引
来源：http://hz.shuidangran.top/gtymmbowkr.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.sufxvd.cn/gtygmcbmse.html

[Q10] 插入单行
来源：http://hz.jqgfzy.top/gtfujojret.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.jinqigfzy.top/gtbdqksnjy.html

[Q11] 一次插入多行
来源：http://hz.havefunace.top/gtqyhkevno.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.xuetiantiany.cn/gtkqfjkpzt.html

[Q12] 插入后取自增 ID
来源：http://hz.yvedp.cn/gtujcekual.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.yueranfly.top/gteqytzrdk.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.jinqigufen.top/gthgvjyhzb.html

[Q13] 忽略重复插入
来源：http://hz.yangfankeji.com/gthvvzbase.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.jinqigfzy.top/gtivqbbxgh.html

[Q14] 存在则更新（upsert）
来源：http://hz.zdqjudy.top/gtjnnjahvi.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.xziqi.cn/gtwgetjdrl.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.c1oappe.top/gtadqgrtvi.html

[Q15] 查询全部
来源：http://hz.316326.xyz/gtqcvujvle.html

SELECT * FROM users;
来源：http://hz.fzhhl.top/gtwkzcvrsp.html

[Q16] 查询指定列
来源：http://hz.zhaomingkeji.xyz/gtdqsaltid.html

SELECT id, name FROM users;
来源：http://hz.jlsjyb.cn/gtempxmxji.html

[Q17] 条件查询
来源：http://hz.jlsjyb.cn/gtrjyjdfve.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.kuanghao11.cn/gtvqhmmdeg.html

[Q18] 模糊匹配
来源：http://hz.ehwqpu.com/gtgfmnctdh.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.chenzaomai.com/gtvyfyxkee.html

[Q19] 范围查询
来源：http://hz.wangdashe.top/gtmpdsmamk.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.cqqwz.cn/gteodmzchv.html

[Q20] IN 列表
来源：http://hz.pengpengdd.cyou/gtfviazuax.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.hnqzz.top/gtnnynxktn.html

[Q21] 空值判断
来源：http://hz.haohaochexian.top/gtklxeyqof.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.vqdsnc.cn/gtpsubswyv.html

[Q22] 排序
来源：http://hz.hywenlv.cn/gtiatdovry.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.feifeiyinyue.top/gtbsuawjpt.html

[Q23] 分页
来源：http://hz.daria6918.cn/gtzxbvcufz.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.birdmap.top/gtzvmftbof.html

[Q24] 去重
来源：http://hz.gzhubu.top/gtajchrdiy.html

SELECT DISTINCT city FROM users;
来源：http://hz.xinyue.icu/gtoepvdvsn.html

[Q25] 只取前 N 条
来源：http://hz.sxryk.cn/gtdfhkouhd.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.tianlin.xyz/gtkfolriqh.html

[Q26] 计数
来源：http://hz.iojbl.cn/gtmbglmeyc.html

SELECT COUNT(*) FROM users;
来源：http://hz.nanxinkj.top/gtzxcunffy.html

[Q27] 条件计数
来源：http://hz.chenlongwang.top/gtylshvyjx.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.yvedp.cn/gtylzutatj.html

[Q28] 求和与平均
来源：http://hz.bjfxy.top/gtutxvynop.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.guowangkeji.top/gtshqfgtns.html

[Q29] 最大最小值
来源：http://hz.tianlin.xyz/gtmkrmyzdr.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.316326.xyz/gtirltlfdi.html

[Q30] 分组统计
来源：http://hz.xinyue.icu/gtfehzmbwt.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.redwolf501.top/gtsunwcrtm.html

[Q31] 分组后过滤
来源：http://hz.52xcode.cn/gtkhaotbnt.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.tanke756.top/gtymxdplxe.html

[Q32] 分组拼接字符串
来源：http://hz.pycfn.com/gtbmeovova.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.zycfv.cn/gtufjybpor.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.shanyushiyangtech.top/gtakbenuoe.html

[Q33] 多列分组
来源：http://hz.pycfn.com/gtweogngbn.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.yuanzhike.top/gthfuprwxj.html

[Q34] 每组取第一条
来源：http://hz.tanke756.top/gtbtkbucnz.html

SELECT * FROM (
来源：http://hz.bjfxy.top/gtllkelitl.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.shuidangran.top/gttqzpufoj.html

) t WHERE rn = 1;
来源：http://hz.gaohongyu789.top/gtfihchywq.html

[Q35] 内连接
来源：http://hz.kuanghao11.cn/gtbyobqjwx.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.guannengcc.top/gtixgakelx.html

[Q36] 左连接
来源：http://hz.hysaishi.cn/gthfoasjhz.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.feifeiyinyue.top/gtkiuymyoz.html

[Q37] 右连接
来源：http://hz.aibaodan.cn/gttlptyjqd.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.feifeiyinyue.top/gtltyufifr.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.tanke756.top/gtrpwyogjp.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.cucudq.cn/gtjqhhaoei.html

[Q39] 自连接（查上下级）
来源：http://hz.ydjk.org.cn/gtljpeohdm.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.fengsongda.top/gtyjhbqkbi.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.ydzc1.top/gtgbglmqzx.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.wangdashe.top/gthqixevsg.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.ehwqpu.com/gtzimlrcya.html

[Q41] 多表连接
来源：http://hz.daria6918.cn/gtckfiwwan.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.gaohongyu789.top/gtvzyruktn.html

JOIN users u ON u.id = o.user_id
来源：http://hz.bjfxy.top/gtncubihtw.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.hnqzz.top/gtfwmaaqtl.html

[Q42] 连接条件附加过滤
来源：http://hz.guowangkeji.top/gtbngpvdoi.html

SELECT u.name, o.amount FROM users u
来源：http://hz.cashguo.top/gtbyxxddxx.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.hysaishi.cn/gtgptrcsuk.html

[Q43] 标量子查询
来源：http://hz.jyoumei.cn/gtepztlxin.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.yueranfly.top/gtepfqpvqx.html

[Q44] IN 子查询
来源：http://hz.dianchejie.cn/gtxyarqjbb.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.xuanzx.com/gtzovbaias.html

[Q45] EXISTS 判断存在
来源：http://hz.hnqzz.top/gtrjsziwor.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zycfv.cn/gtolleqsph.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.zdqjudy.top/gtvyraarft.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.ppjwa.cn/gtfjzbauyt.html

[Q47] 与平均值比较
来源：http://hz.hongshengwenyu.top/gtnzcinxhz.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.smart0.xyz/gtqdlfrmrx.html

[Q48] CTE 公用表表达式
来源：http://hz.tian-w.cn/gtakvfhbwn.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.xziqi.cn/gtbhurgiyk.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.daria6918.cn/gtmvlwubld.html

[Q49] 更新单行
来源：http://hz.ydzc1.top/gttvedfslv.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.hammf.cn/gtiwfvbvxf.html

[Q50] 批量更新
来源：http://hz.smart0.xyz/gtgplsiorh.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.316326.xyz/gtbaptyxzb.html

[Q51] 用子查询更新
来源：http://hz.chenjidiqi.icu/gtfnkzoevk.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.yuanzhike.top/gtifffqxiw.html

[Q52] 删除指定行
来源：http://hz.zhixingplan.top/gticwtnqri.html

DELETE FROM users WHERE id = 10;
来源：http://hz.zhengqikj.top/gtgznokkti.html

[Q53] 按条件删除
来源：http://hz.zhaomingkeji.xyz/gtldlxjtac.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.kuanghao11.cn/gtqkhriech.html

[Q54] 清空表
来源：http://hz.c1oappe.top/gtgojmnpqh.html

TRUNCATE TABLE logs;
来源：http://hz.havefunace.top/gtjktgpmar.html

[Q55] 排名（并列占位）
来源：http://hz.zhongyouzk.top/gtuxojajqo.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.kuanghao11.cn/gtwkyfuese.html

[Q56] 密集排名（并列不占位）
来源：http://hz.jinqigfzy.top/gtfsgfxpib.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.vqdsnc.cn/gtilcafbej.html

[Q57] 行号
来源：http://hz.jinqigfzy.top/gtxcdmunpx.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.iojbl.cn/gtlmjeliwy.html

[Q58] 累计求和
来源：http://hz.dashuyun.cn/gttzrrqujx.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.gogol.net.cn/gtznzuyevz.html

[Q59] 分组内累计
来源：http://hz.gaohongyu789.top/gtzspsdarj.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.9152youxi.cn/gthsmazjwy.html

[Q60] 取上一行 / 下一行
来源：http://hz.xinyue.icu/gtfrzrktxd.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.zhijiandao.cn/gturvpedrs.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.daria6918.cn/gtzvsjmbbj.html

[Q61] 移动平均
来源：http://hz.xylfe.cn/gtbvmdjjkm.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.meibo888.top/gtbddfntzt.html

[Q62] 分组占比
来源：http://hz.yueranfly.top/gtwzjbzfwy.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.yongpay.top/gtppbdkxbk.html

[Q63] 开启事务
来源：http://hz.fengsongda.top/gtmoxylabp.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.hammf.cn/gtfrdhjpgw.html

[Q64] 提交事务
来源：http://hz.gzhubu.top/gtzyqggcyb.html

COMMIT;
来源：http://hz.gotoacloud.top/gtxisimoju.html

[Q65] 回滚事务
来源：http://hz.yj20258888.top/gteubdhybi.html

ROLLBACK;
来源：http://hz.gogol.net.cn/gtvmvuihog.html

[Q66] 行锁查询
来源：http://hz.yangfankeji.com/gtfofhqood.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.yj20258.top/gtznyiafqt.html

[Q67] 设置隔离级别
来源：http://hz.zhijiandao.cn/gtxxgbrguz.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.cucudq.cn/gthtixdoki.html

[Q68] 保存点
来源：http://hz.cheryme.top/gtdfzjtzht.html

SAVEPOINT sp1;
来源：http://hz.xuetiantiany.cn/gtrgyorcuv.html

ROLLBACK TO sp1;
来源：http://hz.chenjidiqi.icu/gtjpkagalq.html

[Q69] 查看执行计划
来源：http://hz.ywan-chungtsiang.top/gtvxpnbreg.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.snrcjt.cn/gtcltlcnxv.html

[Q70] 更新统计信息
来源：http://hz.gzhubu.top/gtdyqfbpfv.html

ANALYZE TABLE users;
来源：http://hz.ybcxt.top/gtdptjizjv.html

[Q71] 查看建表语句
来源：http://hz.jianghu66.top/gtwshreite.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.haohaochexian.top/gtxgxuiarj.html

[Q72] 查看索引
来源：http://hz.havefunace.top/gtlnipejbv.html

SHOW INDEX FROM users;
来源：http://hz.jiagoushi.top/gtvuoqsifr.html

[Q73] 查看表状态
来源：http://hz.dianchejie.cn/gtrylxlrtt.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.nanxuanxn.top/gtlsnefklz.html

[Q74] 强制使用索引
来源：http://hz.havefunace.top/gtdcgtcycu.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.fzhhl.top/gteoiasgmh.html

[Q75] 日期格式化
来源：http://hz.fzhhl.top/gtwlwlmksi.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.redwolf501.top/gtinmapywe.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.c1oappe.top/gtsdcqnzih.html

[Q76] 按天统计
来源：http://hz.fzhhl.top/gtzjxsoehe.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.ybcxt.top/gthrnkrqsi.html

[Q77] 时间加减
来源：http://hz.ydjk.org.cn/gthabnyzrm.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.hywenlv.cn/gtzaszgvhy.html

[Q78] 当前时间
来源：http://hz.quarkkingdee.top/gthctmrxmi.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.jqgfzy.top/gtyorpmoas.html

[Q79] 字符串拼接
来源：http://hz.quarkkingdee.top/gtimauueya.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.vqdsnc.cn/gtxcraznsr.html

[Q80] 字符串截取
来源：http://hz.zdqjudy.top/gtyhzjzlpc.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.ybcxt.top/gtcrrwzssf.html

[Q81] 字符串替换
来源：http://hz.jinqigfzy.top/gtfbmwherr.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.hongshengwenyu.top/gtvqbfulck.html

[Q82] 字符长度与字节长度
来源：http://hz.zhongyouzk.top/gtjxxqrfur.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.jqgufenzy.top/gtnlsbqguj.html

[Q83] 大小写转换
来源：http://hz.andypj.xyz/gthakiqtgv.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.iojbl.cn/gtdenvxnev.html

[Q84] 去除首尾空格
来源：http://hz.zhixingplan.top/gtwqduamou.html

SELECT TRIM(name) FROM users;
来源：http://hz.zhijiandao.cn/gttpjpzrlu.html

[Q85] 数值取整
来源：http://hz.gzhubu.top/gtyvdcshks.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.jinghuilouyu.cn/gtsdzohtxe.html

[Q86] 读取 JSON 字段
来源：http://hz.sweek.top/gteuxdwhvx.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.dashuyun.cn/gtcmxumcvu.html

[Q87] JSON 字段做条件
来源：http://hz.shangyingyoupin.top/gttyftqksp.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.yuanzhike.top/gtwotpeesu.html

[Q88] 行转列（条件聚合）
来源：http://hz.52xcode.cn/gtjsnmexfz.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.xuetiantiany.cn/gtsasukabq.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.jinghuilouyu.cn/gtryaqeacl.html

[Q89] 判断表是否存在
来源：http://hz.shzxlz.cn/gtjrxiwdoh.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.nanxuanxn.top/gtbnimflaw.html

[Q90] 生成序号列
来源：http://hz.52xcode.cn/gtvypwihzo.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.kuanghao11.cn/gtgqcsssmi.html

================================================================================
来源：http://hz.sysykeji.top/gtcnrcbjnr.html

R. Bash 专题
来源：http://hz.yvedp.cn/gtdvzukgpr.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtjokkugrz.html

[R01] shebang 与严格模式
来源：http://hz.yuxming.cn/gtxbkossty.html

#!/usr/bin/env bash
来源：http://hz.cheryme.top/gtmukkjobm.html

set -euo pipefail
来源：http://hz.haohaochexian.top/gtiqbxbsvy.html

[R02] 变量赋值与使用
来源：http://hz.pycfn.com/gtcounydkb.html

name="Tom"; echo "$name"
来源：http://hz.chenlongwang.top/gtyrkssaae.html

[R03] 只读变量
来源：http://hz.xziqi.cn/gtfoenwbxv.html

readonly PI=3.14
来源：http://hz.chenzaomai.com/gtsfqmustq.html

[R04] 位置参数
来源：http://hz.yj20258.top/gtqhjpqolc.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.yonumen.top/gtcqhozzwt.html

[R05] 参数默认值
来源：http://hz.ywan-chungtsiang.top/gtrcxjbuuq.html

name="${1:-default}"
来源：http://hz.jinyuanbaomall.cn/gtoyuvhnue.html

[R06] 判断命令是否存在
来源：http://hz.yanxiufei.cn/gtzjzavzyj.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.52xcode.cn/gtmsvleosm.html

[R07] if 判断文件
来源：http://hz.aizwys.cn/gtxtkypwfo.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.tianlin.xyz/gtgzdvkofo.html

[R08] 数值比较
来源：http://hz.shzxlz.cn/gtzxzndgtf.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.meibo888.top/gtfnbzyaqv.html

[R09] 字符串比较
来源：http://hz.sysykeji.top/gtputgrsge.html


<!-- 参考信息 -->