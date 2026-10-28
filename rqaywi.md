代发 wailian999

C#:   Guid.NewGuid().ToString()
来源：http://hz.jyoumei.cn/gtxtgrqelc.html

[P02] MD5 / SHA256 摘要
来源：http://hz.hnxiangtu.top/gtdxgjzmhs.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.yj20258888.top/gtaeirevaq.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.andypj.xyz/gtmuibpjxs.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.gogol.net.cn/gtumfecbdv.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.jlsjyb.cn/gtnwbrtyfg.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.yj20258.top/gtglqngfvz.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.zhaomingkeji.xyz/gtlwifkijp.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.316326.xyz/gttoygucch.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.daria6918.cn/gtpudhboyz.html

[P03] 生成短随机字符串
来源：http://hz.chenjidiqi.icu/gtynaduvax.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.yj202588.top/gtkfrnihna.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.zycfv.cn/gtqyzlnthd.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.hnxiangtu.top/gtwhvshdvs.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.hysaishi.cn/gtqnorhctj.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.wangshuangyany.cn/gtejfvhuvj.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.pengpengdd.cyou/gtvrhuqvgq.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.jinyuanbaomall.cn/gtkrghuhvx.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.mhx1999.top/gtipaytbad.html

[P04] 求长度
来源：http://hz.sufxvd.cn/gtpthynedp.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.xinyue.icu/gtmwfhgeoe.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zhiwuduotai.top/gtvdeqmmmf.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.sxryk.cn/gtwbnpcsxg.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.ivvv.top/gtfyfblzew.html

Java: list.size();  map.size();  s.length()
来源：http://hz.hysaishi.cn/gtloeuihtm.html

Go:   len(arr);  len(m)
来源：http://hz.jinqigfzy.top/gtpxhayfrv.html

Ruby: x.length;  x.size
来源：http://hz.ydjk.org.cn/gtwrgpimqr.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.snrcjt.cn/gtmyhlhynl.html

[P05] 判断两个对象内容是否相等
来源：http://hz.snrcjt.cn/gtvysukvle.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.tian-w.cn/gtcwieydmh.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.xinyue.icu/gtpwgivlia.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.zhaomingkeji.xyz/gtssdkqinb.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.xinyue.icu/gtanyrlezu.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.yuxming.cn/gtuglspxey.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.tanke756.top/gtakwsbdsk.html

Ruby: a == b
来源：http://hz.gaohongyu789.top/gtiadeudsb.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.xinyue.icu/gtalxfaibq.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.zycfv.cn/gtkxnqollu.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.316326.xyz/gtsgzidpbu.html

PHP:  if (empty($x)) {}
来源：http://hz.xinyue.icu/gtksguyvai.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.fengsongda.top/gtfmugrtcg.html

TS:   if (x == null) {}
来源：http://hz.hongshengwenyu.top/gtrndwhyyk.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.zhongyouzk.top/gtwtwjstqy.html

Go:   if x == nil {}
来源：http://hz.guowangkeji.top/gtyewdjmbj.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.wangshuangyany.cn/gtdoqkwtei.html

C#:   if (x is null) {}
来源：http://hz.jianghu66.top/gttznwawcw.html

[P07] 防抖与节流
来源：http://hz.jianghu66.top/gtuazaufjj.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.ydjk.org.cn/gtptiezsuj.html

PHP:  // 手写时间戳比较
来源：http://hz.zhaomingkeji.xyz/gtwayqzbhq.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jinqigfzy.top/gtgnoqbaxn.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yongpay.top/gtfsqdvdmj.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.xylfe.cn/gtrdnobfcz.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.guowangkeji.top/gtxgfpfczx.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.yangfankeji.com/gtndmfnbpl.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.chenjidiqi.icu/gtfnmtfyod.html

[P08] 处理浮点精度问题
来源：http://hz.havefunace.top/gtsypwelnj.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.wangdashe.top/gtqvftnncf.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.hysaishi.cn/gtzaijevth.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.zycfv.cn/gtbrrykglt.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.shangyingyoupin.top/gtnyqvsjnz.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.zhongyouzk.top/gtxjpwwewv.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.aibaodan.cn/gtnkvgnvag.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.sysykeji.top/gtkjxtoulc.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.yueranfly.top/gtjicrtmbt.html

================================================================================
来源：http://hz.cheryme.top/gtzfylfgvo.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.bjfxy.top/gtvritykgi.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtevvoyugh.html

[Q01] 创建表
来源：http://hz.kuanghao11.cn/gtfcotimqr.html

CREATE TABLE users (
来源：http://hz.hysaishi.cn/gtkfvesjjp.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yuxming.cn/gtoalkaftq.html

name VARCHAR(50) NOT NULL,
来源：http://hz.xylfe.cn/gtzormhqxm.html

email VARCHAR(100) UNIQUE,
来源：http://hz.guowangkeji.top/gtocngrbca.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.vqdsnc.cn/gtpuhpjfej.html

);
来源：http://hz.yuxming.cn/gtoltzeaix.html

[Q02] 创建带外键的表
来源：http://hz.52xcode.cn/gtgnhrlssh.html

CREATE TABLE orders (
来源：http://hz.aibaodan.cn/gtffinoaya.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.ywan-chungtsiang.top/gtgtckyboa.html

user_id INT NOT NULL,
来源：http://hz.fengsongda.top/gtgdbgfvir.html

amount DECIMAL(10, 2),
来源：http://hz.yangfankeji.com/gtvltiemfn.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.cucudq.cn/gtkfwywgys.html

);
来源：http://hz.dashuyun.cn/gtqjillvwt.html

[Q03] 增加列
来源：http://hz.hongshengwenyu.top/gtwgzvlzrm.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.kuanghao11.cn/gtufpaornf.html

[Q04] 修改列类型
来源：http://hz.feifeiyinyue.top/gtfzcqgfnv.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.sysykeji.top/gtzdcjwnwj.html

[Q05] 重命名列
来源：http://hz.yuanzhike.top/gtbrvsqxsg.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.ydjk.org.cn/gtjvkofbpg.html

[Q06] 删除列
来源：http://hz.tanke756.top/gtljrfygty.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.hysaishi.cn/gtivbxgzvm.html

[Q07] 删除表
来源：http://hz.kuanghao11.cn/gttzgjqcbc.html

DROP TABLE IF EXISTS orders;
来源：http://hz.ydzc1.top/gtpphubrau.html

[Q08] 创建普通索引
来源：http://hz.vqdsnc.cn/gtehdbgwuy.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.hammf.cn/gtbhctyhro.html

[Q09] 创建唯一索引
来源：http://hz.vqdsnc.cn/gttngdhbxg.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.shanyushiyangkeji.top/gtcuvwcbwa.html

[Q10] 插入单行
来源：http://hz.sweek.top/gttjiunjjf.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.jiagoushi.top/gtoztwkvuj.html

[Q11] 一次插入多行
来源：http://hz.dianchejie.cn/gthmvygdab.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.dianchejie.cn/gtwgheizdx.html

[Q12] 插入后取自增 ID
来源：http://hz.smart0.xyz/gtapheawkb.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.pengpengdd.cyou/gtboaajdrl.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.52xcode.cn/gtjyqurstq.html

[Q13] 忽略重复插入
来源：http://hz.hammf.cn/gtapefjqyw.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.yuanzhike.top/gtcewtvzes.html

[Q14] 存在则更新（upsert）
来源：http://hz.zhongyouzk.top/gtsotelmrs.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.jinqigufen.top/gthhvowmwz.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.ehwqpu.com/gtgkvbvwqx.html

[Q15] 查询全部
来源：http://hz.shuidangran.top/gtlzfibspg.html

SELECT * FROM users;
来源：http://hz.c1oappe.top/gtytabpmaa.html

[Q16] 查询指定列
来源：http://hz.cashguo.top/gtweikuybu.html

SELECT id, name FROM users;
来源：http://hz.snrcjt.cn/gtpfmruzzp.html

[Q17] 条件查询
来源：http://hz.hnqzz.top/gttmfterfk.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.yangfankeji.com/gtnfkougdm.html

[Q18] 模糊匹配
来源：http://hz.hysaishi.cn/gtzsrkyoob.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.guowangkeji.top/gtunudrtjo.html

[Q19] 范围查询
来源：http://hz.iojbl.cn/gtizbjmlih.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.zhijiandao.cn/gtpvqhtjez.html

[Q20] IN 列表
来源：http://hz.cqqwz.cn/gtywfxqbfy.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.gotoacloud.top/gtztfuwjzk.html

[Q21] 空值判断
来源：http://hz.jinghuilouyu.cn/gtuuknhifv.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.wangshuangyany.cn/gtubfviogy.html

[Q22] 排序
来源：http://hz.yongpay.top/gtwgxhnare.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.jqgufenzy.top/gtvnsnsrbo.html

[Q23] 分页
来源：http://hz.pengpengdd.cyou/gtztcyerpw.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.xziqi.cn/gtccuitjgs.html

[Q24] 去重
来源：http://hz.yj20258.top/gtnhxpcljg.html

SELECT DISTINCT city FROM users;
来源：http://hz.gzhubu.top/gtsvosftxn.html

[Q25] 只取前 N 条
来源：http://hz.pengpengdd.cyou/gtrvsawvlq.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.chenjidiqi.icu/gtfaytdqfk.html

[Q26] 计数
来源：http://hz.wangshuangyany.cn/gtwronseph.html

SELECT COUNT(*) FROM users;
来源：http://hz.yonumen.top/gtvygttbmt.html

[Q27] 条件计数
来源：http://hz.jqgufenzy.top/gtckbkygjx.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.jinqigfzy.top/gtpetaovdf.html

[Q28] 求和与平均
来源：http://hz.aizwys.cn/gtoohshhxx.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.jianghu66.top/gteaqjqqel.html

[Q29] 最大最小值
来源：http://hz.yonumen.top/gtggumtszo.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.0kj1m.cn/gtlgtfvbzw.html

[Q30] 分组统计
来源：http://hz.shanyushiyangkeji.top/gtrmvhpxzp.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.guowangkeji.top/gtlqjhazyx.html

[Q31] 分组后过滤
来源：http://hz.nanxinkj.top/gthcuobbsk.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.shuidangran.top/gtdcityfjf.html

[Q32] 分组拼接字符串
来源：http://hz.ybcxt.top/gtjzerormn.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.yueranfly.top/gttxmzsfah.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.guannengcc.top/gttdztrjso.html

[Q33] 多列分组
来源：http://hz.gotoacloud.top/gtmprlrmik.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.xylfe.cn/gtfevfgcgi.html

[Q34] 每组取第一条
来源：http://hz.cashguo.top/gtvmqglsnk.html

SELECT * FROM (
来源：http://hz.yueranfly.top/gtmmcqqqvq.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.wangdashe.top/gtkzriftuh.html

) t WHERE rn = 1;
来源：http://hz.0kj1m.cn/gtjpeufgyy.html

[Q35] 内连接
来源：http://hz.shuidangran.top/gtxpdoruon.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.iojbl.cn/gtlgtybjcl.html

[Q36] 左连接
来源：http://hz.jinqigfzy.top/gtqtzpyzyd.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.tianlin.xyz/gtvljowrdl.html

[Q37] 右连接
来源：http://hz.chenjidiqi.icu/gthszunput.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.ehwqpu.com/gttahsnpmb.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.mhx1999.top/gtmynoanqx.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.9152youxi.cn/gttjyyvmft.html

[Q39] 自连接（查上下级）
来源：http://hz.hongshengwenyu.top/gtdwknqtuu.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.ehwqpu.com/gticzhuzyj.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.sysykeji.top/gtelgtibpa.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.tianlin.xyz/gtcvypxgdy.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.jlsjyb.cn/gtwnokfsih.html

[Q41] 多表连接
来源：http://hz.yonumen.top/gtdirqocrm.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.aizwys.cn/gtebywrwoz.html

JOIN users u ON u.id = o.user_id
来源：http://hz.fzhhl.top/gtssfxzidv.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.andypj.xyz/gttqlpmlej.html

[Q42] 连接条件附加过滤
来源：http://hz.fengsongda.top/gtonejrzgr.html

SELECT u.name, o.amount FROM users u
来源：http://hz.hywenlv.cn/gtslyeleug.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.cdnleiting.top/gtswjmlgay.html

[Q43] 标量子查询
来源：http://hz.jqgfzy.top/gtgbynsazm.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.shanyushiyangkeji.top/gtxwzaigqw.html

[Q44] IN 子查询
来源：http://hz.9152youxi.cn/gtjjqyvnxk.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.sysykeji.top/gtvkflvuxn.html

[Q45] EXISTS 判断存在
来源：http://hz.dashuyun.cn/gtugabbqfn.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.aibaodan.cn/gtknpxqnbp.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.zycfv.cn/gtwupjyvfs.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zhaomingkeji.xyz/gtluqxydwp.html

[Q47] 与平均值比较
来源：http://hz.jianghu66.top/gtimzpmrbx.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.cashguo.top/gtyukefbit.html

[Q48] CTE 公用表表达式
来源：http://hz.yueranfly.top/gtpbuacicz.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.guannengcc.top/gtnzdcqgmj.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.tanke756.top/gtflmjlcsp.html

[Q49] 更新单行
来源：http://hz.chenlongwang.top/gtilhjcnek.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.hnqzz.top/gtmbygkenj.html

[Q50] 批量更新
来源：http://hz.cqqwz.cn/gtxjrakfiv.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.quarkkingdee.top/gthqeivxbt.html

[Q51] 用子查询更新
来源：http://hz.jyoumei.cn/gtykplvdzi.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.ydzc1.top/gtjciffbuv.html

[Q52] 删除指定行
来源：http://hz.sufxvd.cn/gtwaflvmwy.html

DELETE FROM users WHERE id = 10;
来源：http://hz.cheryme.top/gtlrflbypg.html

[Q53] 按条件删除
来源：http://hz.shangyingyoupin.top/gtfgrwffgz.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.snrcjt.cn/gtcfvgetkt.html

[Q54] 清空表
来源：http://hz.nanxinkj.top/gtdpgracte.html

TRUNCATE TABLE logs;
来源：http://hz.xuetiantiany.cn/gttjkjyqub.html

[Q55] 排名（并列占位）
来源：http://hz.sweek.top/gtcovbielz.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.yonumen.top/gtwwebzkdg.html

[Q56] 密集排名（并列不占位）
来源：http://hz.hfpthk.cn/gtbonijtji.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.shanyushiyangtech.top/gtiedicyot.html

[Q57] 行号
来源：http://hz.redwolf501.top/gtblpcdzmu.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.0kj1m.cn/gtmyzcdgwk.html

[Q58] 累计求和
来源：http://hz.gaohongyu789.top/gtitwwgtkm.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.yonumen.top/gttsrnyrzf.html

[Q59] 分组内累计
来源：http://hz.svipenyu.cn/gtymqpmdmh.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.fengsongda.top/gtzzdiczsv.html

[Q60] 取上一行 / 下一行
来源：http://hz.cucudq.cn/gtfskeudjn.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.xingfuxueyuan.xyz/gtykufkglr.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.tian-w.cn/gtssujumni.html

[Q61] 移动平均
来源：http://hz.hfpthk.cn/gtezwxfjxu.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.svipenyu.cn/gtariaoccf.html

[Q62] 分组占比
来源：http://hz.gogol.net.cn/gtwzobzdyk.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.wangdashe.top/gtvhjdfpze.html

[Q63] 开启事务
来源：http://hz.guannengcc.top/gtwbqtvlpj.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.cheryme.top/gtfxjmlhjv.html

[Q64] 提交事务
来源：http://hz.mhx1999.top/gtbpzamdrh.html

COMMIT;
来源：http://hz.smart0.xyz/gthgudmgcm.html

[Q65] 回滚事务
来源：http://hz.jqgfzy.top/gtdkdnvphc.html

ROLLBACK;
来源：http://hz.feifeiyinyue.top/gtdnchotxo.html

[Q66] 行锁查询
来源：http://hz.ppjwa.cn/gticnmidwm.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.pengpengdd.cyou/gtehntsvvg.html

[Q67] 设置隔离级别
来源：http://hz.zhongyouzk.top/gtmnavkwsi.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.nanxuanxn.top/gtzwtmspwb.html

[Q68] 保存点
来源：http://hz.smart0.xyz/gtnjxswxnx.html

SAVEPOINT sp1;
来源：http://hz.ehwqpu.com/gttqmyzpwf.html

ROLLBACK TO sp1;
来源：http://hz.nanxuanxn.top/gtndxewgae.html

[Q69] 查看执行计划
来源：http://hz.316326.xyz/gtjummrozm.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.nanxuanxn.top/gtugwtmlnh.html

[Q70] 更新统计信息
来源：http://hz.jqgfzy.top/gtsnmpbgtd.html

ANALYZE TABLE users;
来源：http://hz.cheryme.top/gtlumbbcwn.html

[Q71] 查看建表语句
来源：http://hz.shangyingyoupin.top/gtgkqlalmn.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.ehwqpu.com/gtbalukjcw.html

[Q72] 查看索引
来源：http://hz.pycfn.com/gtfkmimikt.html

SHOW INDEX FROM users;
来源：http://hz.svipenyu.cn/gtbobjzxxr.html

[Q73] 查看表状态
来源：http://hz.yj20258.top/gtkjqnlujb.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.shanyushiyangtech.top/gtafmtjefq.html

[Q74] 强制使用索引
来源：http://hz.zhengqikj.top/gthoxnfatw.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.chenjidiqi.icu/gtogvitqpp.html

[Q75] 日期格式化
来源：http://hz.daxiang520.top/gtmefcvsub.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.daria6918.cn/gtuenirhhm.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.ppjwa.cn/gtunxdcfyn.html

[Q76] 按天统计
来源：http://hz.gzhubu.top/gtpjzluoju.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.cashguo.top/gtiiigibvm.html

[Q77] 时间加减
来源：http://hz.guannengcc.top/gtfppfxlnk.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.gogol.net.cn/gtnptqwrhx.html

[Q78] 当前时间
来源：http://hz.yuxming.cn/gtckczkrnh.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.aibaodan.cn/gtnniberfq.html

[Q79] 字符串拼接
来源：http://hz.kuanghao11.cn/gtfjpiaazz.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.hnxiangtu.top/gtqguhfnpe.html

[Q80] 字符串截取
来源：http://hz.snrcjt.cn/gtcaqvkeen.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.ydjk.org.cn/gtcyyqkugc.html

[Q81] 字符串替换
来源：http://hz.jyoumei.cn/gttvhmuxak.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.havefunace.top/gtrsqpiiia.html

[Q82] 字符长度与字节长度
来源：http://hz.haohaochexian.top/gtjqgwtevw.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.52xcode.cn/gtwlfuvadk.html

[Q83] 大小写转换
来源：http://hz.snrcjt.cn/gtlljppavj.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.52xcode.cn/gtnywccwgf.html

[Q84] 去除首尾空格
来源：http://hz.zhoulong.xyz/gtsqqbjnmx.html

SELECT TRIM(name) FROM users;
来源：http://hz.dashuyun.cn/gtldpmimmb.html

[Q85] 数值取整
来源：http://hz.shanyushiyangtech.top/gtiifvgovt.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.gogol.net.cn/gtabrcamvn.html

[Q86] 读取 JSON 字段
来源：http://hz.wangshuangyany.cn/gtqvhclccw.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.0kj1m.cn/gtrlwwvysk.html

[Q87] JSON 字段做条件
来源：http://hz.kuanghao11.cn/gtyvxchcee.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.shanyushiyangkeji.top/gtzxvwluik.html

[Q88] 行转列（条件聚合）
来源：http://hz.shanyushiyangtech.top/gtpcsshrrv.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.smart0.xyz/gtysixmzfo.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.yuanzhike.top/gtqxjayuho.html

[Q89] 判断表是否存在
来源：http://hz.xziqi.cn/gtiigcenni.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.sweek.top/gtrmsbxbtd.html

[Q90] 生成序号列
来源：http://hz.cucudq.cn/gtswaehlkw.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.zhiwuduotai.top/gttjyyeeeq.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtsnutaymh.html

R. Bash 专题
来源：http://hz.fzhhl.top/gtkrtfprqu.html

================================================================================
来源：http://hz.c1oappe.top/gthvomfiuu.html

[R01] shebang 与严格模式
来源：http://hz.cucudq.cn/gtgenoyjks.html

#!/usr/bin/env bash
来源：http://hz.gzhubu.top/gtsphdomcj.html

set -euo pipefail
来源：http://hz.jqgfzy.top/gtplcpbjcp.html

[R02] 变量赋值与使用
来源：http://hz.yuxming.cn/gtxxxkzsfk.html

name="Tom"; echo "$name"
来源：http://hz.hysaishi.cn/gtdqcjfksn.html

[R03] 只读变量
来源：http://hz.tanke756.top/gtczgmolxp.html

readonly PI=3.14
来源：http://hz.xuetiantiany.cn/gtxchyqjhj.html

[R04] 位置参数
来源：http://hz.yj202588.top/gtxawpeywo.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.aibaodan.cn/gtcyihhcxt.html

[R05] 参数默认值
来源：http://hz.hnqzz.top/gtrcenyiwv.html

name="${1:-default}"
来源：http://hz.cdnleiting.top/gtawobwaft.html

[R06] 判断命令是否存在
来源：http://hz.shanyushiyangkeji.top/gtesxnmhiw.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.zhijiandao.cn/gthszyzjzo.html

[R07] if 判断文件
来源：http://hz.gotoacloud.top/gtimmyxjfo.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.jianghu66.top/gtizurncqj.html

[R08] 数值比较
来源：http://hz.316326.xyz/gtfaddyvkt.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.shanyushiyangkeji.top/gtbgudyacb.html

[R09] 字符串比较
来源：http://hz.zhijiandao.cn/gtrinkenlq.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.c1oappe.top/gtznedemxu.html

[R10] 正则匹配
来源：http://hz.yj20258.top/gtalfkfvon.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.iojbl.cn/gtcoqbrfiv.html

[R11] case 多分支
来源：http://hz.jinyuanbaomall.cn/gthdzyvmge.html

case "$1" in
来源：http://hz.feifeiyinyue.top/gtgjqjidke.html

start) echo "启动" ;;
来源：http://hz.andypj.xyz/gtvcdjbwfi.html

stop)  echo "停止" ;;
来源：http://hz.tian-w.cn/gtqvqiscqv.html

*)     echo "未知命令" ;;
来源：http://hz.zhengqikj.top/gtozwpmjdt.html


<!-- 参考信息 -->