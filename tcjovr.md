代发 wailian999

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.redwolf501.top/gttgdzfljd.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.xziqi.cn/gtxivlivwq.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.zdqjudy.top/gtxtjvaxqh.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.tian-w.cn/gtlunnmzco.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.c1oappe.top/gtoxzominb.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.gogol.net.cn/gtxyfxiiyn.html

[P03] 生成短随机字符串
来源：http://hz.haohaochexian.top/gtxqgfaght.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.xuanzx.com/gthzhmplzs.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.yj20258888.top/gtqgwkicvz.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.ybcxt.top/gtyepogmqq.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jianghu66.top/gtnpacrzap.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.ybcxt.top/gtbizyldyf.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.nanxinkj.top/gtlnzoyshk.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.shangyingyoupin.top/gtaqqsdutd.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.ydjk.org.cn/gtkqrjxvjs.html

[P04] 求长度
来源：http://hz.dianchejie.cn/gthlkfgzqq.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.zycfv.cn/gtonpexwsd.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yanxiufei.cn/gtqtljshqe.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.gzhubu.top/gtfgccqotv.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.aizwys.cn/gtieglxyld.html

Java: list.size();  map.size();  s.length()
来源：http://hz.vqdsnc.cn/gticxbglxo.html

Go:   len(arr);  len(m)
来源：http://hz.zhixingplan.top/gtsbqcxslr.html

Ruby: x.length;  x.size
来源：http://hz.gzhubu.top/gtcljudfcr.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.tanke756.top/gtwnmzhjgd.html

[P05] 判断两个对象内容是否相等
来源：http://hz.shangyingyoupin.top/gtivzitdoe.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.sxryk.cn/gtdwwlmgur.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.hfpthk.cn/gtgvafkmss.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.yj20258888.top/gtjjukuubq.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.quarkkingdee.top/gtvadwvfsx.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.dashuyun.cn/gtcoyschxh.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.yongpay.top/gtjfwwnnfy.html

Ruby: a == b
来源：http://hz.hnxiangtu.top/gtnqiitgwb.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.daria6918.cn/gtpryxrjeb.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.cqqwz.cn/gtrkgvyend.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.snrcjt.cn/gtagvrjwhp.html

PHP:  if (empty($x)) {}
来源：http://hz.mhx1999.top/gtcefbtdxd.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.jyoumei.cn/gtzsggoenb.html

TS:   if (x == null) {}
来源：http://hz.gogol.net.cn/gtzuivsxlt.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.xingfuxueyuan.xyz/gtxpeamxhf.html

Go:   if x == nil {}
来源：http://hz.smart0.xyz/gtoirhkcou.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.tianlin.xyz/gtlwhnpmyj.html

C#:   if (x is null) {}
来源：http://hz.xingfuxueyuan.xyz/gtfsdegwky.html

[P07] 防抖与节流
来源：http://hz.hywenlv.cn/gtyfjnvppz.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.vqdsnc.cn/gtxtatdepc.html

PHP:  // 手写时间戳比较
来源：http://hz.snrcjt.cn/gtmhvgzpwv.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yueranfly.top/gtmknjoqpc.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zhiwuduotai.top/gtooxwqupx.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.jinqigufen.top/gtmhxjbxqm.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.vqdsnc.cn/gtyxqsiojr.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.ehwqpu.com/gtyjluodts.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.meibo888.top/gtsyfdjktk.html

[P08] 处理浮点精度问题
来源：http://hz.nwbrower.top/gtoghsnjpw.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.dianchejie.cn/gtgaonpulw.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.hongshengwenyu.top/gtjwzqxnsc.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.snrcjt.cn/gtladnjnkz.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.jianghu66.top/gtwjlxbhfh.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.yj20258.top/gtaljihmex.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.meibo888.top/gtaffcursl.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.dianchejie.cn/gthoytucoc.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.xingfuxueyuan.xyz/gtymupevhy.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtoetdkggi.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.gotoacloud.top/gtwtfyucgn.html

================================================================================
来源：http://hz.zhixingplan.top/gtfdkylbap.html

[Q01] 创建表
来源：http://hz.yj20258888.top/gtuxxsehdo.html

CREATE TABLE users (
来源：http://hz.pycfn.com/gtghbazsgg.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.iojbl.cn/gtjrnatrmu.html

name VARCHAR(50) NOT NULL,
来源：http://hz.yj20258888.top/gtbpewdqhp.html

email VARCHAR(100) UNIQUE,
来源：http://hz.zycfv.cn/gtoyzmnxyr.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.zhaomingkeji.xyz/gtyawmvsvn.html

);
来源：http://hz.xuetiantiany.cn/gtkmxtzcqt.html

[Q02] 创建带外键的表
来源：http://hz.yj202588.top/gtbyvznhnm.html

CREATE TABLE orders (
来源：http://hz.ehwqpu.com/gtobazjpty.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jyoumei.cn/gthzvxfzrd.html

user_id INT NOT NULL,
来源：http://hz.ivvv.top/gtaeiinhzf.html

amount DECIMAL(10, 2),
来源：http://hz.ydzc1.top/gtkurrdvuf.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.tanke756.top/gtnzbaxgcf.html

);
来源：http://hz.zycfv.cn/gtyizdqteu.html

[Q03] 增加列
来源：http://hz.xinyue.icu/gtmdbmxvan.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.9152youxi.cn/gtqllndssm.html

[Q04] 修改列类型
来源：http://hz.xziqi.cn/gtzcdtmkfz.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.zhongyouzk.top/gtrnsicxdt.html

[Q05] 重命名列
来源：http://hz.redwolf501.top/gtlmqnzvww.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.jiagoushi.top/gtupkjyyrg.html

[Q06] 删除列
来源：http://hz.jinghuilouyu.cn/gtczklfyrp.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.aizwys.cn/gtmrhqgmkj.html

[Q07] 删除表
来源：http://hz.andypj.xyz/gtyctbjlyc.html

DROP TABLE IF EXISTS orders;
来源：http://hz.pycfn.com/gtejyusyou.html

[Q08] 创建普通索引
来源：http://hz.ybcxt.top/gtzaratppc.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.zhiwuduotai.top/gtswriotty.html

[Q09] 创建唯一索引
来源：http://hz.jqgfzy.top/gtcyzmkfxc.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.pycfn.com/gtkkcdsvhi.html

[Q10] 插入单行
来源：http://hz.andypj.xyz/gtvkkqmnfa.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.haohaochexian.top/gtytgmevbs.html

[Q11] 一次插入多行
来源：http://hz.cqqwz.cn/gtymtpousl.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.daria6918.cn/gtbehvwkyn.html

[Q12] 插入后取自增 ID
来源：http://hz.chenzaomai.com/gtnldaadqx.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.yj202588.top/gtblvxxzvb.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.dianchejie.cn/gtnhmdpipt.html

[Q13] 忽略重复插入
来源：http://hz.xziqi.cn/gtunragkyp.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.shuidangran.top/gtptooilqo.html

[Q14] 存在则更新（upsert）
来源：http://hz.xingfuxueyuan.xyz/gtltjfyyxs.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.jianghu66.top/gtsgnggeam.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.shuidangran.top/gtgxtklgqr.html

[Q15] 查询全部
来源：http://hz.zycfv.cn/gtutlsmqml.html

SELECT * FROM users;
来源：http://hz.meibo888.top/gtsmxlowvn.html

[Q16] 查询指定列
来源：http://hz.ydjk.org.cn/gtfpvvmzuc.html

SELECT id, name FROM users;
来源：http://hz.dashuyun.cn/gtjxejxdah.html

[Q17] 条件查询
来源：http://hz.fengsongda.top/gtqjhkfuzw.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.jinqigufen.top/gtrckbonql.html

[Q18] 模糊匹配
来源：http://hz.yuanzhike.top/gttwxxkkrt.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.fzhhl.top/gtvveuhvrv.html

[Q19] 范围查询
来源：http://hz.xuetiantiany.cn/gttelmirfz.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.sufxvd.cn/gtdqoljcpv.html

[Q20] IN 列表
来源：http://hz.mhx1999.top/gtasmkkixp.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.gzhubu.top/gtylpzmxai.html

[Q21] 空值判断
来源：http://hz.xinyue.icu/gtmcyfptly.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.svipenyu.cn/gtypugvjgt.html

[Q22] 排序
来源：http://hz.iojbl.cn/gtokpnvcqv.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.gogol.net.cn/gtvyxzkpzq.html

[Q23] 分页
来源：http://hz.birdmap.top/gthznoider.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.zhongyouzk.top/gtonmyqykz.html

[Q24] 去重
来源：http://hz.jiagoushi.top/gtmscfopng.html

SELECT DISTINCT city FROM users;
来源：http://hz.ivvv.top/gtrhnxrylc.html

[Q25] 只取前 N 条
来源：http://hz.shangyingyoupin.top/gtbpyfiqwt.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.daria6918.cn/gtrclmhcag.html

[Q26] 计数
来源：http://hz.zdqjudy.top/gtafyukxiq.html

SELECT COUNT(*) FROM users;
来源：http://hz.yanxiufei.cn/gtunkzrgsb.html

[Q27] 条件计数
来源：http://hz.hysaishi.cn/gtsshzoolc.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.yueranfly.top/gtpppqspfc.html

[Q28] 求和与平均
来源：http://hz.nwbrower.top/gtynywnfdw.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.vqdsnc.cn/gtawawrqqv.html

[Q29] 最大最小值
来源：http://hz.xziqi.cn/gtvkirumhh.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.yj202588.top/gtgruvaiqj.html

[Q30] 分组统计
来源：http://hz.gaohongyu789.top/gtmojqvvyx.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.zhaomingkeji.xyz/gtwwfwxvzj.html

[Q31] 分组后过滤
来源：http://hz.yongpay.top/gtfffqybrq.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.yj202588.top/gttmzdynur.html

[Q32] 分组拼接字符串
来源：http://hz.tianlin.xyz/gtubwpdstk.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.zhongyouzk.top/gtfrcueltt.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.yangfankeji.com/gtcfvzngbu.html

[Q33] 多列分组
来源：http://hz.pengpengdd.cyou/gtdbwdqkor.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.bjfxy.top/gtfufbvpfu.html

[Q34] 每组取第一条
来源：http://hz.jyoumei.cn/gtdwhywwdr.html

SELECT * FROM (
来源：http://hz.chenjidiqi.icu/gtircsfwap.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.dashuyun.cn/gthmhkcvcb.html

) t WHERE rn = 1;
来源：http://hz.ehwqpu.com/gtngzbrezm.html

[Q35] 内连接
来源：http://hz.hysaishi.cn/gtucywciyd.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.sxryk.cn/gtmezwbohx.html

[Q36] 左连接
来源：http://hz.yanxiufei.cn/gtvwkdlxvs.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.guannengcc.top/gtaxrhtuhz.html

[Q37] 右连接
来源：http://hz.hongshengwenyu.top/gtqkweyodg.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.jlsjyb.cn/gtjeqywvvl.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.pengpengdd.cyou/gtlazttjyn.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.sufxvd.cn/gtuoewuhgk.html

[Q39] 自连接（查上下级）
来源：http://hz.cheryme.top/gtvouthsfs.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.tian-w.cn/gtlhnkvcwm.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.iojbl.cn/gtubeizmku.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.shzxlz.cn/gtyewsbowb.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.zycfv.cn/gttwvopgvw.html

[Q41] 多表连接
来源：http://hz.nanxinkj.top/gtsgoojriz.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.jqgufenzy.top/gthrgcgmne.html

JOIN users u ON u.id = o.user_id
来源：http://hz.mhx1999.top/gtlyjdtrso.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.dianchejie.cn/gtqvegsvnj.html

[Q42] 连接条件附加过滤
来源：http://hz.dianchejie.cn/gtohhnknkb.html

SELECT u.name, o.amount FROM users u
来源：http://hz.cashguo.top/gtmgofwkhb.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.cqqwz.cn/gtnidmvqvd.html

[Q43] 标量子查询
来源：http://hz.kuanghao11.cn/gtlxkzzixr.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.yueranfly.top/gtrworivpo.html

[Q44] IN 子查询
来源：http://hz.bjfxy.top/gtzwiqabxy.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.yvedp.cn/gtpmqapfwe.html

[Q45] EXISTS 判断存在
来源：http://hz.shanyushiyangtech.top/gtacwbakkl.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yj20258888.top/gtwttcvnfz.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.nwbrower.top/gtsziwympw.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.smart0.xyz/gtrmzqsvum.html

[Q47] 与平均值比较
来源：http://hz.fengsongda.top/gtkpvhzqim.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.jinghuilouyu.cn/gtfjoefhoj.html

[Q48] CTE 公用表表达式
来源：http://hz.316326.xyz/gtktoghaxx.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.tian-w.cn/gtcwiqyqaa.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.aibaodan.cn/gtpbovqujl.html

[Q49] 更新单行
来源：http://hz.hnxiangtu.top/gtlrbrivpe.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.jqgfzy.top/gtteecjimd.html

[Q50] 批量更新
来源：http://hz.zhixingplan.top/gtujzeegik.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.tianlin.xyz/gtnfojaequ.html

[Q51] 用子查询更新
来源：http://hz.jiagoushi.top/gtyuupiwiw.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.yangfankeji.com/gtrdxlgktz.html

[Q52] 删除指定行
来源：http://hz.yuanzhike.top/gtpzhkhmnb.html

DELETE FROM users WHERE id = 10;
来源：http://hz.xziqi.cn/gtnvekjkbu.html

[Q53] 按条件删除
来源：http://hz.ydjk.org.cn/gthtouruqd.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.zycfv.cn/gtwbmnxbtd.html

[Q54] 清空表
来源：http://hz.yvedp.cn/gthxgvfizd.html

TRUNCATE TABLE logs;
来源：http://hz.yvedp.cn/gttagazige.html

[Q55] 排名（并列占位）
来源：http://hz.jqgfzy.top/gtnmvljpzb.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.jinqigufen.top/gteqyziqjg.html

[Q56] 密集排名（并列不占位）
来源：http://hz.ivvv.top/gtqckqixyo.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.zhoulong.xyz/gtwlpofvsh.html

[Q57] 行号
来源：http://hz.jinqigufen.top/gtabhjfcmq.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.ppjwa.cn/gtlrsnqdyv.html

[Q58] 累计求和
来源：http://hz.cdnleiting.top/gtylrazxjl.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.shuidangran.top/gttuiovazo.html

[Q59] 分组内累计
来源：http://hz.zhoulong.xyz/gtgmwigiuo.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.redwolf501.top/gttkqlrpta.html

[Q60] 取上一行 / 下一行
来源：http://hz.ppjwa.cn/gtqjiqqhdw.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.jinghuilouyu.cn/gtshgrkjvz.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.tanke756.top/gtdeiaqouc.html

[Q61] 移动平均
来源：http://hz.hnqzz.top/gtfhutocai.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.jinghuilouyu.cn/gtmuadhtpb.html

[Q62] 分组占比
来源：http://hz.meibo888.top/gtcpflwamh.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.c1oappe.top/gtixvzmbvn.html

[Q63] 开启事务
来源：http://hz.hammf.cn/gtylgkzbdh.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.pengpengdd.cyou/gtffcfieze.html

[Q64] 提交事务
来源：http://hz.xuetiantiany.cn/gtbdspwjuc.html

COMMIT;
来源：http://hz.guowangkeji.top/gtizsqpyjf.html

[Q65] 回滚事务
来源：http://hz.zhaomingkeji.xyz/gtlxmaddvt.html

ROLLBACK;
来源：http://hz.fengsongda.top/gtbnswlqsm.html

[Q66] 行锁查询
来源：http://hz.dashuyun.cn/gtggmwqavh.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.zhijiandao.cn/gtzowkzski.html

[Q67] 设置隔离级别
来源：http://hz.yangfankeji.com/gtqjrztedx.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.ehwqpu.com/gtrjomybqu.html

[Q68] 保存点
来源：http://hz.xylfe.cn/gtlszxoaii.html

SAVEPOINT sp1;
来源：http://hz.sweek.top/gtaltevgkz.html

ROLLBACK TO sp1;
来源：http://hz.zhixingplan.top/gtuydqinhi.html

[Q69] 查看执行计划
来源：http://hz.shzxlz.cn/gtmuiuvncx.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.chenjidiqi.icu/gtpknnoqnt.html

[Q70] 更新统计信息
来源：http://hz.xingfuxueyuan.xyz/gtgjdrexqy.html

ANALYZE TABLE users;
来源：http://hz.xuetiantiany.cn/gtnyuxuagp.html

[Q71] 查看建表语句
来源：http://hz.gaohongyu789.top/gtycdttnrc.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.dianchejie.cn/gtqiwvvqbn.html

[Q72] 查看索引
来源：http://hz.cdnleiting.top/gtofatogbk.html

SHOW INDEX FROM users;
来源：http://hz.jianghu66.top/gtoglkaijj.html

[Q73] 查看表状态
来源：http://hz.zdqjudy.top/gtvkzvjssv.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.jiagoushi.top/gtayztsmlc.html

[Q74] 强制使用索引
来源：http://hz.guowangkeji.top/gtfahwslzy.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.jinqigfzy.top/gtmibaywez.html

[Q75] 日期格式化
来源：http://hz.jinqigfzy.top/gtkptbfupu.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.sysykeji.top/gtwgbeejax.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.aibaodan.cn/gtzdulzjis.html

[Q76] 按天统计
来源：http://hz.aizwys.cn/gtpikaplmo.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.zhijiandao.cn/gticmarmgc.html

[Q77] 时间加减
来源：http://hz.chenzaomai.com/gtxszvqprk.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.nanxinkj.top/gtbfnzpemy.html

[Q78] 当前时间
来源：http://hz.sweek.top/gtfxcezsjo.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.tanke756.top/gteccdewki.html

[Q79] 字符串拼接
来源：http://hz.jinqigufen.top/gtxnyrpyvs.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.jqgfzy.top/gtcatmuiee.html

[Q80] 字符串截取
来源：http://hz.sysykeji.top/gtfgokmuqn.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.hammf.cn/gtxwpiwzij.html

[Q81] 字符串替换
来源：http://hz.jlsjyb.cn/gtjzsaospq.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.xingfuxueyuan.xyz/gtveafxfuk.html

[Q82] 字符长度与字节长度
来源：http://hz.smart0.xyz/gtguggkter.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.zycfv.cn/gtozvlsuck.html

[Q83] 大小写转换
来源：http://hz.shzxlz.cn/gtfrzmxuxx.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.redwolf501.top/gtecutijey.html

[Q84] 去除首尾空格
来源：http://hz.hongshengwenyu.top/gtosahzjgt.html

SELECT TRIM(name) FROM users;
来源：http://hz.zycfv.cn/gtkzazhdgf.html

[Q85] 数值取整
来源：http://hz.zhongyouzk.top/gtktltvmvq.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.yangfankeji.com/gtoqaguakp.html

[Q86] 读取 JSON 字段
来源：http://hz.shangyingyoupin.top/gtssbbbobg.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.haohaochexian.top/gtozblieqi.html

[Q87] JSON 字段做条件
来源：http://hz.hammf.cn/gtxjytixna.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.bjfxy.top/gthaiqmtsm.html

[Q88] 行转列（条件聚合）
来源：http://hz.zhoulong.xyz/gtawpkvjyq.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.smart0.xyz/gtrrdqscjz.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.yongpay.top/gtujiasyfi.html

[Q89] 判断表是否存在
来源：http://hz.shuidangran.top/gtsatxrlaj.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.jqgfzy.top/gtjtoktwjt.html

[Q90] 生成序号列
来源：http://hz.snrcjt.cn/gtaxvaxipt.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.zhongyouzk.top/gtvxnuxhlp.html

================================================================================
来源：http://hz.ppjwa.cn/gtldmvhxyu.html

R. Bash 专题
来源：http://hz.shzxlz.cn/gthbacplga.html

================================================================================
来源：http://hz.hywenlv.cn/gtwahjulrq.html

[R01] shebang 与严格模式
来源：http://hz.xinyue.icu/gtkryosamo.html

#!/usr/bin/env bash
来源：http://hz.zdqjudy.top/gtucvbehet.html

set -euo pipefail
来源：http://hz.jiagoushi.top/gtflxvtncu.html

[R02] 变量赋值与使用
来源：http://hz.chenjidiqi.icu/gthzwreyyx.html

name="Tom"; echo "$name"
来源：http://hz.hnxiangtu.top/gtlyomjley.html

[R03] 只读变量
来源：http://hz.redwolf501.top/gtlohhvsum.html

readonly PI=3.14
来源：http://hz.zhijiandao.cn/gtjwgfxzrk.html

[R04] 位置参数
来源：http://hz.yueranfly.top/gthezcolwo.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.ydjk.org.cn/gtaoyqeham.html

[R05] 参数默认值
来源：http://hz.zhixingplan.top/gtrfukooiy.html

name="${1:-default}"
来源：http://hz.guannengcc.top/gtitsvxhhs.html

[R06] 判断命令是否存在
来源：http://hz.zhengqikj.top/gtexsmtjau.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.nanxinkj.top/gtwyhmtgux.html

[R07] if 判断文件
来源：http://hz.ydzc1.top/gtorazclsu.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.hysaishi.cn/gtusizhbxg.html

[R08] 数值比较
来源：http://hz.xylfe.cn/gtmensthng.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.xuetiantiany.cn/gtucfkvmwg.html

[R09] 字符串比较
来源：http://hz.jinghuilouyu.cn/gtvwjooafi.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.jqgfzy.top/gtymmabbze.html

[R10] 正则匹配
来源：http://hz.cheryme.top/gtxwsjdhri.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.hammf.cn/gterdlzyit.html

[R11] case 多分支
来源：http://hz.hnxiangtu.top/gtgdlitsuw.html

case "$1" in
来源：http://hz.pengpengdd.cyou/gtbsrpdtxa.html

start) echo "启动" ;;
来源：http://hz.quarkkingdee.top/gtkmkavitq.html

stop)  echo "停止" ;;
来源：http://hz.yuanzhike.top/gteyujpiux.html

*)     echo "未知命令" ;;
来源：http://hz.chenjidiqi.icu/gtgnniqfkm.html

esac
来源：http://hz.shanyushiyangkeji.top/gtuzkfzfbd.html

[R12] for 遍历文件
来源：http://hz.bjfxy.top/gtvemsbmny.html

for f in *.txt; do echo "$f"; done
来源：http://hz.jinghuilouyu.cn/gtyhlqtklv.html

[R13] for 计数循环
来源：http://hz.ehwqpu.com/gtqplkicsv.html


<!-- 参考信息 -->