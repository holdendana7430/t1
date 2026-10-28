代发 wailian999

TS:   crypto.randomUUID()
来源：http://hz.yj202588.top/gthafzhqna.html

Java: UUID.randomUUID().toString()
来源：http://hz.jyoumei.cn/gtyadjebsm.html

Go:   // 用 github.com/google/uuid
来源：http://hz.ywan-chungtsiang.top/gtjpkcmqei.html

Ruby: SecureRandom.uuid
来源：http://hz.chenzaomai.com/gtuemmgqks.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.ehwqpu.com/gtjdegfotj.html

[P02] MD5 / SHA256 摘要
来源：http://hz.jinqigufen.top/gtelpancvn.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.52xcode.cn/gtjsyfpgjm.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.ehwqpu.com/gtiknkdikm.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.hnqzz.top/gtxejkcjhy.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.daxiang520.top/gtsqbagmzk.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.yj20258.top/gtoudpsymp.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.pycfn.com/gtkluwaysk.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.gaohongyu789.top/gtbgobtdht.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.quarkkingdee.top/gtaoactkua.html

[P03] 生成短随机字符串
来源：http://hz.yangfankeji.com/gtspruodaf.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.fzhhl.top/gtyrqkdbvn.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.pengpengdd.cyou/gtvijpwtmk.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.gaohongyu789.top/gtxwhysazx.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yonumen.top/gtglirbefn.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.jinqigfzy.top/gtptihoeyd.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.havefunace.top/gtsevzccxu.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.nwbrower.top/gtzebqsjjw.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.shzxlz.cn/gtfitvnhqr.html

[P04] 求长度
来源：http://hz.yangfankeji.com/gtqbwpygva.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.jyoumei.cn/gtzdqqdfdp.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.hfpthk.cn/gttmwizzht.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.hywenlv.cn/gtsrspnyht.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.gogol.net.cn/gtdzakgrvt.html

Java: list.size();  map.size();  s.length()
来源：http://hz.gotoacloud.top/gtluyltqht.html

Go:   len(arr);  len(m)
来源：http://hz.jyoumei.cn/gtoilqrmsl.html

Ruby: x.length;  x.size
来源：http://hz.aizwys.cn/gtqqebncrb.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.birdmap.top/gtqgauqrlg.html

[P05] 判断两个对象内容是否相等
来源：http://hz.jqgfzy.top/gtgptanxue.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.gogol.net.cn/gtxdkxoiev.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.aibaodan.cn/gtabsdeuad.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.guowangkeji.top/gtprsgkkei.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.xuanzx.com/gthppostyv.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.snrcjt.cn/gtkulbzjum.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.jinqigfzy.top/gtuxzmbsqt.html

Ruby: a == b
来源：http://hz.meibo888.top/gtckovjipx.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.mhx1999.top/gtgwutylrj.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.jqgfzy.top/gtshoackyg.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.kuanghao11.cn/gtudblrpir.html

PHP:  if (empty($x)) {}
来源：http://hz.daxiang520.top/gtcwstepzl.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.gzhubu.top/gtbimqnahh.html

TS:   if (x == null) {}
来源：http://hz.hywenlv.cn/gtkfbjmbwa.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.pengpengdd.cyou/gtwqchnhpk.html

Go:   if x == nil {}
来源：http://hz.gzhubu.top/gtrhokspsn.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.cucudq.cn/gtkoquxrko.html

C#:   if (x is null) {}
来源：http://hz.mhx1999.top/gtylfdrlur.html

[P07] 防抖与节流
来源：http://hz.vqdsnc.cn/gteqycrrdt.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.aizwys.cn/gttedavcjn.html

PHP:  // 手写时间戳比较
来源：http://hz.dashuyun.cn/gtrpqkerms.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zhoulong.xyz/gthjtqqoff.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.gotoacloud.top/gtenepamyh.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.pengpengdd.cyou/gtnkvpmubg.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.xingfuxueyuan.xyz/gtfrgbmomx.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.pengpengdd.cyou/gtomshnakv.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.snrcjt.cn/gtomngrnmt.html

[P08] 处理浮点精度问题
来源：http://hz.guowangkeji.top/gtpirnzaxv.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.cqqwz.cn/gtypqplcjr.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.zycfv.cn/gtvgcziqfh.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.yonumen.top/gtmflkgbkr.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.gaohongyu789.top/gtuileqdpc.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.daxiang520.top/gtgmsduqip.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.gogol.net.cn/gtdeqviatv.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.gaohongyu789.top/gtdmatqndo.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.jinqigufen.top/gtvtfgvhuj.html

================================================================================
来源：http://hz.havefunace.top/gtmuzookrv.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.zhengqikj.top/gtxfgkrxmh.html

================================================================================
来源：http://hz.cheryme.top/gtgdqwthtq.html

[Q01] 创建表
来源：http://hz.0kj1m.cn/gtarqqovsh.html

CREATE TABLE users (
来源：http://hz.zdqjudy.top/gtbxlnwsqc.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.ydzc1.top/gtjumbpeox.html

name VARCHAR(50) NOT NULL,
来源：http://hz.svipenyu.cn/gttpctjwxw.html

email VARCHAR(100) UNIQUE,
来源：http://hz.aibaodan.cn/gtfksjvshi.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.vqdsnc.cn/gtvimooyou.html

);
来源：http://hz.hnxiangtu.top/gtiplbytsf.html

[Q02] 创建带外键的表
来源：http://hz.feifeiyinyue.top/gthepkbcyr.html

CREATE TABLE orders (
来源：http://hz.xuanzx.com/gtkowgnbti.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.9152youxi.cn/gtcyqcrgml.html

user_id INT NOT NULL,
来源：http://hz.jyoumei.cn/gthuhjxlgo.html

amount DECIMAL(10, 2),
来源：http://hz.kuanghao11.cn/gtifffbsvt.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.meibo888.top/gtrllsdixr.html

);
来源：http://hz.bjfxy.top/gtsdytdgfc.html

[Q03] 增加列
来源：http://hz.yj20258888.top/gtyocdiqti.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.ivvv.top/gtepnfifpa.html

[Q04] 修改列类型
来源：http://hz.aibaodan.cn/gtexjflujy.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.gogol.net.cn/gtqiixixjr.html

[Q05] 重命名列
来源：http://hz.zycfv.cn/gtjdzdhtea.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.zhoulong.xyz/gtbacjcwcw.html

[Q06] 删除列
来源：http://hz.ehwqpu.com/gtaieyomka.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.xuetiantiany.cn/gtbwpszulp.html

[Q07] 删除表
来源：http://hz.nanxinkj.top/gtpkuxqnlw.html

DROP TABLE IF EXISTS orders;
来源：http://hz.ppjwa.cn/gtzzwjyzdb.html

[Q08] 创建普通索引
来源：http://hz.ehwqpu.com/gtgjrnmahi.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.daria6918.cn/gttkkqlcfa.html

[Q09] 创建唯一索引
来源：http://hz.hammf.cn/gtvhyrttgs.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.jyoumei.cn/gtilcewfsa.html

[Q10] 插入单行
来源：http://hz.0kj1m.cn/gtuigysjtu.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.jianghu66.top/gtegjupwhe.html

[Q11] 一次插入多行
来源：http://hz.jinyuanbaomall.cn/gtrwzuovbp.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.316326.xyz/gtdyjzurwq.html

[Q12] 插入后取自增 ID
来源：http://hz.cheryme.top/gtjcyeemwn.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.shuidangran.top/gtmaihewvf.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.yanxiufei.cn/gtddkheqio.html

[Q13] 忽略重复插入
来源：http://hz.jianghu66.top/gtnrkoysig.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.nanxinkj.top/gtznpeccot.html

[Q14] 存在则更新（upsert）
来源：http://hz.yj20258888.top/gtbimdyryh.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.xylfe.cn/gtwobfqdjc.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.zhongyouzk.top/gtnikpclhe.html

[Q15] 查询全部
来源：http://hz.redwolf501.top/gtjfqgtwep.html

SELECT * FROM users;
来源：http://hz.tian-w.cn/gtzaqskgmk.html

[Q16] 查询指定列
来源：http://hz.quarkkingdee.top/gtnyhsxxdi.html

SELECT id, name FROM users;
来源：http://hz.sufxvd.cn/gtdrlxneiw.html

[Q17] 条件查询
来源：http://hz.fzhhl.top/gtumjwgovy.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.svipenyu.cn/gtinyvimww.html

[Q18] 模糊匹配
来源：http://hz.pycfn.com/gtzobtimve.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.yangfankeji.com/gtbwmhkznq.html

[Q19] 范围查询
来源：http://hz.guowangkeji.top/gtynawkhbk.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.aibaodan.cn/gtzzplmqmo.html

[Q20] IN 列表
来源：http://hz.jyoumei.cn/gtciotajhb.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.jqgfzy.top/gtzyvqgncc.html

[Q21] 空值判断
来源：http://hz.zhoulong.xyz/gtqdmpjqpw.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.cdnleiting.top/gtftdwfcye.html

[Q22] 排序
来源：http://hz.haohaochexian.top/gtildsmcyv.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.zhongyouzk.top/gtwcggsswz.html

[Q23] 分页
来源：http://hz.zhiwuduotai.top/gtwdxarpya.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.chenjidiqi.icu/gttyaiisms.html

[Q24] 去重
来源：http://hz.iojbl.cn/gtniicqsoo.html

SELECT DISTINCT city FROM users;
来源：http://hz.sxryk.cn/gtvcutyhot.html

[Q25] 只取前 N 条
来源：http://hz.hywenlv.cn/gtvnswkwbj.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.gaohongyu789.top/gtiqfzxlri.html

[Q26] 计数
来源：http://hz.yuxming.cn/gtaoahlcrc.html

SELECT COUNT(*) FROM users;
来源：http://hz.yuanzhike.top/gtxszbdnjz.html

[Q27] 条件计数
来源：http://hz.xuanzx.com/gthgpmafat.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.xingfuxueyuan.xyz/gtxrvliuqk.html

[Q28] 求和与平均
来源：http://hz.jianghu66.top/gtmnkrnhcu.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.bjfxy.top/gthilelbhz.html

[Q29] 最大最小值
来源：http://hz.yj20258888.top/gtzxoftmze.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.havefunace.top/gtbmehtpwr.html

[Q30] 分组统计
来源：http://hz.quarkkingdee.top/gtbjtbuetn.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.ivvv.top/gtjawbpala.html

[Q31] 分组后过滤
来源：http://hz.nanxinkj.top/gttcoghdfa.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.wangshuangyany.cn/gttxcoaqrh.html

[Q32] 分组拼接字符串
来源：http://hz.zhongyouzk.top/gtiukeubqt.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.cucudq.cn/gtshmstxqm.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.iojbl.cn/gtjbtxtmgp.html

[Q33] 多列分组
来源：http://hz.zhoulong.xyz/gtdhaalulv.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.jinqigfzy.top/gtqdtynpis.html

[Q34] 每组取第一条
来源：http://hz.ybcxt.top/gtwotlfrbp.html

SELECT * FROM (
来源：http://hz.havefunace.top/gtwojozxgi.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.zhiwuduotai.top/gtzwqrlegm.html

) t WHERE rn = 1;
来源：http://hz.yuxming.cn/gtxrdnmqls.html

[Q35] 内连接
来源：http://hz.gogol.net.cn/gtfnubzlfz.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.guowangkeji.top/gtpujoktmd.html

[Q36] 左连接
来源：http://hz.ydjk.org.cn/gtlsfbsufq.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.shanyushiyangtech.top/gttztkudcf.html

[Q37] 右连接
来源：http://hz.cqqwz.cn/gtdyrehisw.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.zhiwuduotai.top/gtrlaelxdg.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.snrcjt.cn/gtitlzrogr.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.jinghuilouyu.cn/gtrkckfksk.html

[Q39] 自连接（查上下级）
来源：http://hz.chenjidiqi.icu/gtkdwfhkaq.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.tanke756.top/gtbnutfhak.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.xuanzx.com/gtjqnntpzu.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.316326.xyz/gtfqdhnnat.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.bjfxy.top/gtdwqdrzyk.html

[Q41] 多表连接
来源：http://hz.guannengcc.top/gtludcyrch.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.jinyuanbaomall.cn/gtswzmreeu.html

JOIN users u ON u.id = o.user_id
来源：http://hz.wangshuangyany.cn/gtnofbofzi.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.nanxinkj.top/gtgyhijcfy.html

[Q42] 连接条件附加过滤
来源：http://hz.quarkkingdee.top/gtkprxdjqe.html

SELECT u.name, o.amount FROM users u
来源：http://hz.yvedp.cn/gtzwnhljbk.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.xziqi.cn/gtwwuedaxj.html

[Q43] 标量子查询
来源：http://hz.ivvv.top/gtniyenihf.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.yuanzhike.top/gtlguzwwea.html

[Q44] IN 子查询
来源：http://hz.nanxinkj.top/gtgimajrgz.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.zdqjudy.top/gtnymghpfw.html

[Q45] EXISTS 判断存在
来源：http://hz.kuanghao11.cn/gteqobuept.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.snrcjt.cn/gtcjtzsymc.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.yj20258.top/gtkogzvawt.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.daria6918.cn/gtcukbuajl.html

[Q47] 与平均值比较
来源：http://hz.jqgfzy.top/gttomlsreb.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.hnxiangtu.top/gtzicejgyp.html

[Q48] CTE 公用表表达式
来源：http://hz.yonumen.top/gtbmkisnhf.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.cqqwz.cn/gtnfnrtile.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.zycfv.cn/gtrphikgbd.html

[Q49] 更新单行
来源：http://hz.zhiwuduotai.top/gtnqeuvbzx.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.cqqwz.cn/gtcrcmonuc.html

[Q50] 批量更新
来源：http://hz.hfpthk.cn/gtsduoikrx.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.gaohongyu789.top/gtkvuafwbs.html

[Q51] 用子查询更新
来源：http://hz.chenjidiqi.icu/gtlbsyvolv.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.tian-w.cn/gtvjmgjuxc.html

[Q52] 删除指定行
来源：http://hz.xinyue.icu/gtqelgtvit.html

DELETE FROM users WHERE id = 10;
来源：http://hz.pengpengdd.cyou/gtblliqsrk.html

[Q53] 按条件删除
来源：http://hz.jyoumei.cn/gtfzrpkvfo.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.hnxiangtu.top/gtmsgbiexg.html

[Q54] 清空表
来源：http://hz.chenlongwang.top/gtwdlxdvhg.html

TRUNCATE TABLE logs;
来源：http://hz.quarkkingdee.top/gtptuwooay.html

[Q55] 排名（并列占位）
来源：http://hz.jianghu66.top/gtcdcmyhnt.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.ybcxt.top/gtwfdymmvy.html

[Q56] 密集排名（并列不占位）
来源：http://hz.cucudq.cn/gttudwnavq.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.ivvv.top/gtqaduwfrz.html

[Q57] 行号
来源：http://hz.shanyushiyangkeji.top/gtnozqbhyz.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.haohaochexian.top/gttrqgirxo.html

[Q58] 累计求和
来源：http://hz.snrcjt.cn/gtoewteubg.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.havefunace.top/gtucnwnjxo.html

[Q59] 分组内累计
来源：http://hz.dashuyun.cn/gtnninrtax.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.jianghu66.top/gtnpxddgfx.html

[Q60] 取上一行 / 下一行
来源：http://hz.yongpay.top/gtdrksogsu.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.shanyushiyangkeji.top/gtsezcoqma.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.daria6918.cn/gtndhffeer.html

[Q61] 移动平均
来源：http://hz.vqdsnc.cn/gtwxxdyhrq.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.yonumen.top/gtpinzvjoj.html

[Q62] 分组占比
来源：http://hz.tianlin.xyz/gtcbxprjnd.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.ybcxt.top/gtagjhwdxy.html

[Q63] 开启事务
来源：http://hz.guannengcc.top/gtmgjwznpl.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.gogol.net.cn/gtxleoncfu.html

[Q64] 提交事务
来源：http://hz.gzhubu.top/gthwxoqeav.html

COMMIT;
来源：http://hz.zhijiandao.cn/gtzxnwztam.html

[Q65] 回滚事务
来源：http://hz.tian-w.cn/gtcjcsnnkk.html

ROLLBACK;
来源：http://hz.ehwqpu.com/gtauoctnsd.html

[Q66] 行锁查询
来源：http://hz.zhijiandao.cn/gtxnwlzbht.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.jiagoushi.top/gteqcigzik.html

[Q67] 设置隔离级别
来源：http://hz.chenzaomai.com/gtvwqlcatu.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.nwbrower.top/gteygzdioe.html

[Q68] 保存点
来源：http://hz.jinqigfzy.top/gtltdrjspa.html

SAVEPOINT sp1;
来源：http://hz.birdmap.top/gtztwudahz.html

ROLLBACK TO sp1;
来源：http://hz.kuanghao11.cn/gtwxqefsmg.html

[Q69] 查看执行计划
来源：http://hz.chenzaomai.com/gtyikenzof.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.zycfv.cn/gtilmrbeuc.html

[Q70] 更新统计信息
来源：http://hz.bjfxy.top/gtuwnodfgf.html

ANALYZE TABLE users;
来源：http://hz.yongpay.top/gtummiuyhu.html

[Q71] 查看建表语句
来源：http://hz.andypj.xyz/gtrprwfpeq.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.sxryk.cn/gtesbqzktc.html

[Q72] 查看索引
来源：http://hz.yanxiufei.cn/gtliorxkit.html

SHOW INDEX FROM users;
来源：http://hz.yangfankeji.com/gtnqzzcjzy.html

[Q73] 查看表状态
来源：http://hz.ywan-chungtsiang.top/gtcalmhtfx.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.haohaochexian.top/gtrbiefniz.html

[Q74] 强制使用索引
来源：http://hz.shzxlz.cn/gtidgupmbt.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.hongshengwenyu.top/gtuanklrna.html

[Q75] 日期格式化
来源：http://hz.bjfxy.top/gtfeaaufpt.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.jyoumei.cn/gtdzxkofhr.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.meibo888.top/gtslqpwyvx.html

[Q76] 按天统计
来源：http://hz.ydjk.org.cn/gtmrrxixdc.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.shangyingyoupin.top/gtgyefagak.html

[Q77] 时间加减
来源：http://hz.daria6918.cn/gtpzlljpxm.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.zhixingplan.top/gtpourxrya.html

[Q78] 当前时间
来源：http://hz.vqdsnc.cn/gtzibbrnzo.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.zhoulong.xyz/gtkxkaczxc.html

[Q79] 字符串拼接
来源：http://hz.hnxiangtu.top/gtrpgwnwxd.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.jlsjyb.cn/gttihiyrnu.html

[Q80] 字符串截取
来源：http://hz.pycfn.com/gtwbmpvwmp.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.hysaishi.cn/gtgpiamjpu.html

[Q81] 字符串替换
来源：http://hz.xziqi.cn/gtzsyymxam.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.xuetiantiany.cn/gtpelnkwlk.html

[Q82] 字符长度与字节长度
来源：http://hz.zhoulong.xyz/gtryanuegu.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.chenzaomai.com/gtdudnfuvv.html

[Q83] 大小写转换
来源：http://hz.bjfxy.top/gtkqpyeqaq.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.guowangkeji.top/gtpanmjyxf.html

[Q84] 去除首尾空格
来源：http://hz.zhoulong.xyz/gtjpxmyfwx.html

SELECT TRIM(name) FROM users;
来源：http://hz.mhx1999.top/gtuwsdsiec.html

[Q85] 数值取整
来源：http://hz.aibaodan.cn/gtkfgunuse.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.hammf.cn/gtofeusyuk.html

[Q86] 读取 JSON 字段
来源：http://hz.cheryme.top/gtghatyqlu.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.shanyushiyangtech.top/gtzckbknsf.html

[Q87] JSON 字段做条件
来源：http://hz.guowangkeji.top/gtputcjyri.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.feifeiyinyue.top/gtfruidywd.html

[Q88] 行转列（条件聚合）
来源：http://hz.gogol.net.cn/gtwzromacr.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.gotoacloud.top/gtbzuarhga.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.ivvv.top/gtdhukvjdn.html

[Q89] 判断表是否存在
来源：http://hz.andypj.xyz/gtuihbgtya.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.zhoulong.xyz/gtwzknbesk.html

[Q90] 生成序号列
来源：http://hz.c1oappe.top/gtkxqeogfv.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.nwbrower.top/gtrelhzytz.html

================================================================================
来源：http://hz.guowangkeji.top/gtdonxagcz.html

R. Bash 专题
来源：http://hz.shuidangran.top/gtokvwivuw.html

================================================================================
来源：http://hz.tianlin.xyz/gtexpcfnuo.html

[R01] shebang 与严格模式
来源：http://hz.yj20258888.top/gtniacxxjn.html

#!/usr/bin/env bash
来源：http://hz.dashuyun.cn/gtwtmfojtw.html

set -euo pipefail
来源：http://hz.jinyuanbaomall.cn/gtqgbtikqe.html

[R02] 变量赋值与使用
来源：http://hz.hfpthk.cn/gtuwetfati.html

name="Tom"; echo "$name"
来源：http://hz.hammf.cn/gtakdrmfuy.html

[R03] 只读变量
来源：http://hz.zycfv.cn/gtzxfrwlyf.html

readonly PI=3.14
来源：http://hz.hysaishi.cn/gtyczlzmai.html

[R04] 位置参数
来源：http://hz.jyoumei.cn/gtmfxhmtqq.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.ivvv.top/gtgaimgzrn.html

[R05] 参数默认值
来源：http://hz.daria6918.cn/gtilbjrswn.html

name="${1:-default}"
来源：http://hz.zhijiandao.cn/gtnoictouz.html

[R06] 判断命令是否存在
来源：http://hz.0kj1m.cn/gtyfrixlrk.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.yvedp.cn/gtnbyojxbf.html

[R07] if 判断文件
来源：http://hz.mhx1999.top/gtuodhlmvz.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.hysaishi.cn/gtfwlynguv.html

[R08] 数值比较
来源：http://hz.jinyuanbaomall.cn/gtkunflmlw.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.kuanghao11.cn/gtcdtgamgl.html

[R09] 字符串比较
来源：http://hz.meibo888.top/gtxziobbfn.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.xinyue.icu/gtjtagqurp.html

[R10] 正则匹配
来源：http://hz.0kj1m.cn/gtsdmxertk.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.haohaochexian.top/gtubthlzrc.html

[R11] case 多分支
来源：http://hz.hnxiangtu.top/gtocwocbdb.html


<!-- 参考信息 -->