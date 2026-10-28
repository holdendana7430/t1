代发 wailian999

TS:   crypto.randomUUID()
来源：http://hz.nwbrower.top/gtjbowcgaz.html

Java: UUID.randomUUID().toString()
来源：http://hz.yvedp.cn/gtknxuoyzu.html

Go:   // 用 github.com/google/uuid
来源：http://hz.52xcode.cn/gtukpeipyx.html

Ruby: SecureRandom.uuid
来源：http://hz.jqgufenzy.top/gtacvcrfqs.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.cheryme.top/gtgrdfcarq.html

[P02] MD5 / SHA256 摘要
来源：http://hz.feifeiyinyue.top/gtxtegbcfh.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.shanyushiyangtech.top/gtkdziomjz.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.yuanzhike.top/gtzyhinxqk.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.daria6918.cn/gtppmikyia.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.mhx1999.top/gtqpsyulcs.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.xinyue.icu/gtvidfmzba.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.yuxming.cn/gtgpkkgwwu.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.chenlongwang.top/gtmobendla.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.chenlongwang.top/gtbntgercp.html

[P03] 生成短随机字符串
来源：http://hz.ivvv.top/gtgbnzukjf.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.xuetiantiany.cn/gtaxgxqgmh.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.tian-w.cn/gtqmnpdfhz.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.wangdashe.top/gtijamtixl.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.mhx1999.top/gttxqnuwvn.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.yueranfly.top/gtstpkeuzx.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.yj20258888.top/gtoxukbwzc.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.zycfv.cn/gtaxpvpnfl.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.yuanzhike.top/gtcazqlblq.html

[P04] 求长度
来源：http://hz.hammf.cn/gtfkcujeyx.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.svipenyu.cn/gtmozquaox.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.xuetiantiany.cn/gtprxrnrce.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.9152youxi.cn/gtmwouqhzd.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.cdnleiting.top/gtvgkabwzh.html

Java: list.size();  map.size();  s.length()
来源：http://hz.hnxiangtu.top/gttuxwpjze.html

Go:   len(arr);  len(m)
来源：http://hz.shanyushiyangtech.top/gtdounoxsn.html

Ruby: x.length;  x.size
来源：http://hz.jianghu66.top/gtwjggmsrd.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.jinyuanbaomall.cn/gtthapwhzd.html

[P05] 判断两个对象内容是否相等
来源：http://hz.andypj.xyz/gtxodxvttq.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.jinqigufen.top/gtdwipllgb.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.birdmap.top/gtxckckwqi.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.tian-w.cn/gtstommiww.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.hammf.cn/gtjgtgdeus.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.xuanzx.com/gtpkwbodmb.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.cucudq.cn/gtfrgrvbsx.html

Ruby: a == b
来源：http://hz.yuanzhike.top/gtgnryzxac.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.shuidangran.top/gtclgbfudi.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.cdnleiting.top/gtnxwnhewr.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.guannengcc.top/gtlhrowvpu.html

PHP:  if (empty($x)) {}
来源：http://hz.kuanghao11.cn/gtqonfqpjb.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.nanxuanxn.top/gthfqqdaql.html

TS:   if (x == null) {}
来源：http://hz.9152youxi.cn/gtniltaekg.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.yonumen.top/gtkqimvozq.html

Go:   if x == nil {}
来源：http://hz.hnxiangtu.top/gtdoveaeif.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.nanxuanxn.top/gtajissyim.html

C#:   if (x is null) {}
来源：http://hz.shuidangran.top/gtclsrlzag.html

[P07] 防抖与节流
来源：http://hz.iojbl.cn/gtgejebdkq.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.dashuyun.cn/gtrvyjwbnx.html

PHP:  // 手写时间戳比较
来源：http://hz.jinghuilouyu.cn/gtezacwujr.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.dianchejie.cn/gtwexptoet.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.daria6918.cn/gthxyxkprk.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.wangdashe.top/gtibintuqz.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.smart0.xyz/gtcvfzrhri.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.wangshuangyany.cn/gttwudoinb.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.jlsjyb.cn/gtowghqedz.html

[P08] 处理浮点精度问题
来源：http://hz.shanyushiyangtech.top/gtlajmksam.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.feifeiyinyue.top/gtmwkuuozn.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.yj20258.top/gtitqcjumb.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.hammf.cn/gtuzrwotpz.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.shzxlz.cn/gtrlnpgsdy.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.9152youxi.cn/gtokknkxeq.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.dianchejie.cn/gtkvjzkzof.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.shuidangran.top/gthrzwfgil.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.iojbl.cn/gtqgmhkogk.html

================================================================================
来源：http://hz.aibaodan.cn/gtaarebfdx.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.yuanzhike.top/gtvmyuyevw.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtpmkvcdvl.html

[Q01] 创建表
来源：http://hz.fzhhl.top/gtrvpcdgon.html

CREATE TABLE users (
来源：http://hz.sysykeji.top/gttohjdafb.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.zhijiandao.cn/gtyfiwdgps.html

name VARCHAR(50) NOT NULL,
来源：http://hz.meibo888.top/gtixczwvap.html

email VARCHAR(100) UNIQUE,
来源：http://hz.zdqjudy.top/gtgvezgmps.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.shangyingyoupin.top/gtfbizrtub.html

);
来源：http://hz.shanyushiyangtech.top/gtngwzlwbf.html

[Q02] 创建带外键的表
来源：http://hz.tanke756.top/gtrichikyp.html

CREATE TABLE orders (
来源：http://hz.zhaomingkeji.xyz/gtjdkugycr.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yuxming.cn/gtjzgzzzew.html

user_id INT NOT NULL,
来源：http://hz.cashguo.top/gtfgmgvqhz.html

amount DECIMAL(10, 2),
来源：http://hz.ydjk.org.cn/gtybjdkujn.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.wangdashe.top/gtngyeoejv.html

);
来源：http://hz.xuanzx.com/gttubscutk.html

[Q03] 增加列
来源：http://hz.yj202588.top/gtoiniqjti.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.svipenyu.cn/gtjnibscfd.html

[Q04] 修改列类型
来源：http://hz.meibo888.top/gtrjulmqqd.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.mhx1999.top/gttvlkqtfa.html

[Q05] 重命名列
来源：http://hz.xuanzx.com/gtnqpmnpxt.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.fengsongda.top/gthgvlimxz.html

[Q06] 删除列
来源：http://hz.zycfv.cn/gtkmrbrvhp.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.tian-w.cn/gtzufnotdf.html

[Q07] 删除表
来源：http://hz.zdqjudy.top/gtglhrcqqm.html

DROP TABLE IF EXISTS orders;
来源：http://hz.pengpengdd.cyou/gtoebldxuc.html

[Q08] 创建普通索引
来源：http://hz.ydzc1.top/gtvbabtndr.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.ivvv.top/gtabbgdoiq.html

[Q09] 创建唯一索引
来源：http://hz.cashguo.top/gtydwjmdcl.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.xziqi.cn/gtinrhhlra.html

[Q10] 插入单行
来源：http://hz.yj20258.top/gtyryvyaqe.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.kuanghao11.cn/gtsmuyphfg.html

[Q11] 一次插入多行
来源：http://hz.daxiang520.top/gtvgwtaqcv.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.hnqzz.top/gtkhvnydtz.html

[Q12] 插入后取自增 ID
来源：http://hz.kuanghao11.cn/gtklvstpxc.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.chenlongwang.top/gtmelwfske.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.jianghu66.top/gtaoyroxtz.html

[Q13] 忽略重复插入
来源：http://hz.hnxiangtu.top/gtkpaowyra.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.birdmap.top/gtnxhbnpob.html

[Q14] 存在则更新（upsert）
来源：http://hz.hysaishi.cn/gtivjavday.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.xylfe.cn/gtkshepedb.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.jqgufenzy.top/gtcycuwlfw.html

[Q15] 查询全部
来源：http://hz.shangyingyoupin.top/gtnrqhwnqy.html

SELECT * FROM users;
来源：http://hz.zycfv.cn/gtggoagdfn.html

[Q16] 查询指定列
来源：http://hz.sysykeji.top/gtgqqajxub.html

SELECT id, name FROM users;
来源：http://hz.tian-w.cn/gtccyyrhrq.html

[Q17] 条件查询
来源：http://hz.chenjidiqi.icu/gtniajdoyu.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.meibo888.top/gtkpbpodmc.html

[Q18] 模糊匹配
来源：http://hz.zhoulong.xyz/gtfhcroota.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.pengpengdd.cyou/gtokckuvuq.html

[Q19] 范围查询
来源：http://hz.zycfv.cn/gtgmrbemrz.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.shanyushiyangtech.top/gtnbjbcjup.html

[Q20] IN 列表
来源：http://hz.yonumen.top/gtdrbnclbl.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.zhongyouzk.top/gtdgkpsguj.html

[Q21] 空值判断
来源：http://hz.aibaodan.cn/gtfhvlxzmn.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.shanyushiyangtech.top/gtjdizqjss.html

[Q22] 排序
来源：http://hz.feifeiyinyue.top/gtooxshufu.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.kuanghao11.cn/gtluiwvxvl.html

[Q23] 分页
来源：http://hz.redwolf501.top/gtuyqufpbi.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.aibaodan.cn/gtebzgchjd.html

[Q24] 去重
来源：http://hz.yuxming.cn/gtqbzaeluu.html

SELECT DISTINCT city FROM users;
来源：http://hz.hnxiangtu.top/gtapgifwgh.html

[Q25] 只取前 N 条
来源：http://hz.zhoulong.xyz/gtzerfsffh.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.nanxinkj.top/gtavurotas.html

[Q26] 计数
来源：http://hz.yj20258.top/gttoitaljz.html

SELECT COUNT(*) FROM users;
来源：http://hz.zdqjudy.top/gtzuoqsbov.html

[Q27] 条件计数
来源：http://hz.jiagoushi.top/gtfuonrhmi.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.dianchejie.cn/gtyascxfce.html

[Q28] 求和与平均
来源：http://hz.haohaochexian.top/gtzicgozie.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.ppjwa.cn/gtxlvvhwnp.html

[Q29] 最大最小值
来源：http://hz.ywan-chungtsiang.top/gtmvautoyl.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.zhongyouzk.top/gtcwctupwm.html

[Q30] 分组统计
来源：http://hz.9152youxi.cn/gtofaaqoae.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.fzhhl.top/gttqetcris.html

[Q31] 分组后过滤
来源：http://hz.mhx1999.top/gtqqwezyes.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.feifeiyinyue.top/gthpkjugdh.html

[Q32] 分组拼接字符串
来源：http://hz.zycfv.cn/gtqbcwghbn.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.52xcode.cn/gtwfptgvck.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.jinghuilouyu.cn/gtvyqgbcue.html

[Q33] 多列分组
来源：http://hz.snrcjt.cn/gthiqdfpjn.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.52xcode.cn/gtvuowqvhd.html

[Q34] 每组取第一条
来源：http://hz.feifeiyinyue.top/gtnmgzmguk.html

SELECT * FROM (
来源：http://hz.hnxiangtu.top/gterqamugo.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.quarkkingdee.top/gtlwuqhaau.html

) t WHERE rn = 1;
来源：http://hz.yueranfly.top/gtqlxuocgt.html

[Q35] 内连接
来源：http://hz.wangdashe.top/gtloxuutgt.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.yvedp.cn/gtydgtcvvx.html

[Q36] 左连接
来源：http://hz.zdqjudy.top/gtwmrtabpz.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.jinqigfzy.top/gtgjaysmjm.html

[Q37] 右连接
来源：http://hz.xuanzx.com/gtorwejbvw.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.xingfuxueyuan.xyz/gtqdlfweab.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.yj20258888.top/gtiyzbvxjz.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.fengsongda.top/gtazcjhhud.html

[Q39] 自连接（查上下级）
来源：http://hz.daxiang520.top/gtconojxzy.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.yongpay.top/gtxqvhcria.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.jinyuanbaomall.cn/gtgijalilo.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.gzhubu.top/gtiezxqred.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.yj20258888.top/gtqelhqvav.html

[Q41] 多表连接
来源：http://hz.ppjwa.cn/gtkgbfowkd.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.chenzaomai.com/gtoxjomkjk.html

JOIN users u ON u.id = o.user_id
来源：http://hz.aizwys.cn/gtjvztqtne.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.ydzc1.top/gthxknkbpr.html

[Q42] 连接条件附加过滤
来源：http://hz.redwolf501.top/gtmebsmloa.html

SELECT u.name, o.amount FROM users u
来源：http://hz.gzhubu.top/gtvfzgcwkw.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.ywan-chungtsiang.top/gtacnhnxmt.html

[Q43] 标量子查询
来源：http://hz.zhoulong.xyz/gtndxjlalm.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.dashuyun.cn/gtbwedvsiv.html

[Q44] IN 子查询
来源：http://hz.hfpthk.cn/gtnlohfduz.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.zhoulong.xyz/gtqenaqxoa.html

[Q45] EXISTS 判断存在
来源：http://hz.dashuyun.cn/gturharioy.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zhoulong.xyz/gtamndzkjh.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.ivvv.top/gtqmbmcxwo.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.cashguo.top/gtuphqjgin.html

[Q47] 与平均值比较
来源：http://hz.pycfn.com/gtjbvoasfv.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.yueranfly.top/gtaddgjiot.html

[Q48] CTE 公用表表达式
来源：http://hz.snrcjt.cn/gttpwnkxjk.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.cucudq.cn/gtfnqolooq.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.yuanzhike.top/gtmmzpxbwf.html

[Q49] 更新单行
来源：http://hz.nwbrower.top/gttadneayu.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.zhiwuduotai.top/gtooyekduc.html

[Q50] 批量更新
来源：http://hz.xuanzx.com/gtyleqxgkg.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.sufxvd.cn/gteqiqtxbn.html

[Q51] 用子查询更新
来源：http://hz.andypj.xyz/gtytfsmrji.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.yj202588.top/gtdvrxmxae.html

[Q52] 删除指定行
来源：http://hz.nanxinkj.top/gtdarvojmb.html

DELETE FROM users WHERE id = 10;
来源：http://hz.aibaodan.cn/gtpsgvdyar.html

[Q53] 按条件删除
来源：http://hz.zhiwuduotai.top/gtewyiodyb.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.yongpay.top/gtsrepljlf.html

[Q54] 清空表
来源：http://hz.shuidangran.top/gtcqndvvdj.html

TRUNCATE TABLE logs;
来源：http://hz.0kj1m.cn/gtcehzumuy.html

[Q55] 排名（并列占位）
来源：http://hz.yongpay.top/gtzywhvqtf.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.cdnleiting.top/gtumjoujeh.html

[Q56] 密集排名（并列不占位）
来源：http://hz.hnxiangtu.top/gtosezvuse.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.zhijiandao.cn/gtgtzhphjt.html

[Q57] 行号
来源：http://hz.xylfe.cn/gtjxtdovkk.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.yongpay.top/gtpjolcwdb.html

[Q58] 累计求和
来源：http://hz.cheryme.top/gtfwfngpbs.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.sysykeji.top/gtggaxshek.html

[Q59] 分组内累计
来源：http://hz.feifeiyinyue.top/gtbbpjvttw.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.shanyushiyangkeji.top/gtsjmaeupl.html

[Q60] 取上一行 / 下一行
来源：http://hz.52xcode.cn/gtyiaoekws.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.tanke756.top/gtmhnjhbrm.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.shzxlz.cn/gtehuymili.html

[Q61] 移动平均
来源：http://hz.jinqigufen.top/gtjcmlnvgd.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.yanxiufei.cn/gtffcevuvb.html

[Q62] 分组占比
来源：http://hz.fzhhl.top/gtcapyzmrx.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.chenlongwang.top/gtsfkxsvus.html

[Q63] 开启事务
来源：http://hz.sxryk.cn/gtgeohdece.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.shanyushiyangkeji.top/gtzemlrrjp.html

[Q64] 提交事务
来源：http://hz.pengpengdd.cyou/gtgcwtlkjx.html

COMMIT;
来源：http://hz.aibaodan.cn/gtzieafuql.html

[Q65] 回滚事务
来源：http://hz.ehwqpu.com/gtbhpyatfk.html

ROLLBACK;
来源：http://hz.zhaomingkeji.xyz/gtgqqpxbuc.html

[Q66] 行锁查询
来源：http://hz.0kj1m.cn/gtaocuhxil.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.chenzaomai.com/gtnwqyilep.html

[Q67] 设置隔离级别
来源：http://hz.svipenyu.cn/gtufmnxdwv.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.guowangkeji.top/gtllrnxadr.html

[Q68] 保存点
来源：http://hz.sufxvd.cn/gtxtmlcvwv.html

SAVEPOINT sp1;
来源：http://hz.chenjidiqi.icu/gtjlqmggyg.html

ROLLBACK TO sp1;
来源：http://hz.yuxming.cn/gtyggwpzmx.html

[Q69] 查看执行计划
来源：http://hz.zhiwuduotai.top/gtqfstkymi.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.feifeiyinyue.top/gtjalmypza.html

[Q70] 更新统计信息
来源：http://hz.chenlongwang.top/gtqnqfjoun.html

ANALYZE TABLE users;
来源：http://hz.bjfxy.top/gtnzflaxit.html

[Q71] 查看建表语句
来源：http://hz.jinqigfzy.top/gtexabecza.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.yj20258888.top/gteqnpbphm.html

[Q72] 查看索引
来源：http://hz.redwolf501.top/gtkurytwyj.html

SHOW INDEX FROM users;
来源：http://hz.nanxinkj.top/gtdhhegexx.html

[Q73] 查看表状态
来源：http://hz.pengpengdd.cyou/gtgxzpbcoq.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.zhijiandao.cn/gtonajbxjm.html

[Q74] 强制使用索引
来源：http://hz.c1oappe.top/gtlrrsmquo.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.tianlin.xyz/gtubuyxxsn.html

[Q75] 日期格式化
来源：http://hz.guowangkeji.top/gtstsvszsd.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.feifeiyinyue.top/gtumltfman.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.daxiang520.top/gtebjjvkvf.html

[Q76] 按天统计
来源：http://hz.yueranfly.top/gtfyuhkjev.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.yj20258888.top/gtcnllupyk.html

[Q77] 时间加减
来源：http://hz.mhx1999.top/gtrxfwqsbu.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.zhixingplan.top/gteyunmqwo.html

[Q78] 当前时间
来源：http://hz.jiagoushi.top/gtyphdyzwb.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.tianlin.xyz/gtscnqgrgd.html

[Q79] 字符串拼接
来源：http://hz.yangfankeji.com/gtumvacykm.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.0kj1m.cn/gtzkwlrpnv.html

[Q80] 字符串截取
来源：http://hz.sysykeji.top/gtrndtobwf.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.jianghu66.top/gteskpoiwo.html

[Q81] 字符串替换
来源：http://hz.pengpengdd.cyou/gtbskfobnj.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.aizwys.cn/gtfgklawst.html

[Q82] 字符长度与字节长度
来源：http://hz.chenjidiqi.icu/gtftzlryai.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.ehwqpu.com/gtsjgtrxkt.html

[Q83] 大小写转换
来源：http://hz.iojbl.cn/gtlyyfrfvb.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.zhoulong.xyz/gtpzihdsea.html

[Q84] 去除首尾空格
来源：http://hz.pengpengdd.cyou/gtzslxrgvp.html

SELECT TRIM(name) FROM users;
来源：http://hz.xinyue.icu/gtywsswwbc.html

[Q85] 数值取整
来源：http://hz.cqqwz.cn/gtvkgcqviz.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.yvedp.cn/gtfzzumyth.html

[Q86] 读取 JSON 字段
来源：http://hz.gogol.net.cn/gthvjzvzvs.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.guannengcc.top/gtjhwqhocc.html

[Q87] JSON 字段做条件
来源：http://hz.aizwys.cn/gtdahsaevp.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.xuetiantiany.cn/gtajggepth.html

[Q88] 行转列（条件聚合）
来源：http://hz.shangyingyoupin.top/gtrgglprzm.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.yueranfly.top/gttblkqsmc.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.chenzaomai.com/gtktmgqjwa.html

[Q89] 判断表是否存在
来源：http://hz.nanxinkj.top/gtgdefauxx.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.xinyue.icu/gtspvyhzan.html

[Q90] 生成序号列
来源：http://hz.yj20258.top/gttaeqsrqy.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.vqdsnc.cn/gttmyamiov.html

================================================================================
来源：http://hz.yanxiufei.cn/gtcjhaklls.html

R. Bash 专题
来源：http://hz.nwbrower.top/gtlyktvmfp.html

================================================================================
来源：http://hz.guowangkeji.top/gtcuzmimpk.html

[R01] shebang 与严格模式
来源：http://hz.yueranfly.top/gtbcmdgwlz.html

#!/usr/bin/env bash
来源：http://hz.pengpengdd.cyou/gtroymtipt.html

set -euo pipefail
来源：http://hz.chenlongwang.top/gtseglwaco.html

[R02] 变量赋值与使用
来源：http://hz.yanxiufei.cn/gtxqlccvao.html

name="Tom"; echo "$name"
来源：http://hz.meibo888.top/gtflcljjci.html

[R03] 只读变量
来源：http://hz.feifeiyinyue.top/gtopruydvf.html

readonly PI=3.14
来源：http://hz.jlsjyb.cn/gtzlmpnliv.html

[R04] 位置参数
来源：http://hz.sysykeji.top/gtarzldjla.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.zhongyouzk.top/gtwoljvoxi.html

[R05] 参数默认值
来源：http://hz.yongpay.top/gtwacjmomu.html

name="${1:-default}"
来源：http://hz.iojbl.cn/gtrdazlmrn.html

[R06] 判断命令是否存在
来源：http://hz.andypj.xyz/gtnfusrhqe.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.cqqwz.cn/gtlwpjxjpq.html

[R07] if 判断文件
来源：http://hz.gaohongyu789.top/gtysqxmnjt.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.sweek.top/gtqpiydecz.html

[R08] 数值比较
来源：http://hz.yj20258.top/gtebmqytji.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.tanke756.top/gtartredlc.html

[R09] 字符串比较
来源：http://hz.yj20258.top/gtcbbclovh.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.pengpengdd.cyou/gtmpcoayux.html

[R10] 正则匹配
来源：http://hz.yueranfly.top/gtlgsqkige.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.shangyingyoupin.top/gtbfzmbrqn.html

[R11] case 多分支
来源：http://hz.gzhubu.top/gtrfslwzbv.html


<!-- 参考信息 -->