代发 wailian999

[P01] 生成 UUID
来源：http://hz.cdnleiting.top/gtvtwvpxrx.html

Py:   str(uuid.uuid4())
来源：http://hz.nwbrower.top/gtjfcznfbw.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.hongshengwenyu.top/gtaobcqosc.html

JS:   crypto.randomUUID()
来源：http://hz.52xcode.cn/gthlqrdhkq.html

TS:   crypto.randomUUID()
来源：http://hz.yj202588.top/gtbggkltdo.html

Java: UUID.randomUUID().toString()
来源：http://hz.cheryme.top/gtkswbzbtg.html

Go:   // 用 github.com/google/uuid
来源：http://hz.hnqzz.top/gtfqqxdwbj.html

Ruby: SecureRandom.uuid
来源：http://hz.quarkkingdee.top/gthuyjomym.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.ydjk.org.cn/gtruqlkyzy.html

[P02] MD5 / SHA256 摘要
来源：http://hz.shanyushiyangkeji.top/gtajqsfqeq.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.nanxuanxn.top/gtyicnzqqv.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.tanke756.top/gtusxzjpwv.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.ivvv.top/gtbunseigc.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.xuanzx.com/gtmdrjmzpz.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.tianlin.xyz/gtkklciguh.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.9152youxi.cn/gtvakkcjxy.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.jinyuanbaomall.cn/gtcgtghikp.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.hnxiangtu.top/gteodzorqj.html

[P03] 生成短随机字符串
来源：http://hz.sufxvd.cn/gtokqcoabz.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.xuanzx.com/gtkhhcmuep.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.ywan-chungtsiang.top/gtsiuacmoo.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yuanzhike.top/gttwooowii.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jiagoushi.top/gthsahfdmh.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.zhijiandao.cn/gtrqofdxmt.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.yj202588.top/gtjurbvmqb.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.cdnleiting.top/gtifqjkpga.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.jinyuanbaomall.cn/gttmlsgquy.html

[P04] 求长度
来源：http://hz.xuetiantiany.cn/gtbxlxwbjt.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.xylfe.cn/gtjnftadbh.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.gogol.net.cn/gtopwqcrjh.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.chenlongwang.top/gtojnrffld.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.hongshengwenyu.top/gtsncxbzge.html

Java: list.size();  map.size();  s.length()
来源：http://hz.xylfe.cn/gtenxnwvxm.html

Go:   len(arr);  len(m)
来源：http://hz.chenlongwang.top/gthimtrhqs.html

Ruby: x.length;  x.size
来源：http://hz.hnqzz.top/gtijtwhqrb.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.jinghuilouyu.cn/gtzsgffmvp.html

[P05] 判断两个对象内容是否相等
来源：http://hz.0kj1m.cn/gtjtvkvydm.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.iojbl.cn/gtdngqtjte.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.316326.xyz/gtdpcptfvh.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.haohaochexian.top/gtmjzmfrco.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.ehwqpu.com/gthvybuycs.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.jinyuanbaomall.cn/gtwdqwesyt.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.hysaishi.cn/gtfbivuwln.html

Ruby: a == b
来源：http://hz.xuanzx.com/gtvwzgavuv.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.jinghuilouyu.cn/gtietkvvoi.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.zdqjudy.top/gtcsrbjkub.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.meibo888.top/gtjxmacjfi.html

PHP:  if (empty($x)) {}
来源：http://hz.yongpay.top/gtdrbrxdpa.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.yuanzhike.top/gtiwmtvtvg.html

TS:   if (x == null) {}
来源：http://hz.fengsongda.top/gtxwjxzotq.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.xylfe.cn/gtbfwzsgvs.html

Go:   if x == nil {}
来源：http://hz.hammf.cn/gtrcwdtnex.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.gzhubu.top/gtavkxhgfw.html

C#:   if (x is null) {}
来源：http://hz.fengsongda.top/gtnebxnfmo.html

[P07] 防抖与节流
来源：http://hz.fzhhl.top/gtyjtnxkgk.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.dashuyun.cn/gtzwphxzjl.html

PHP:  // 手写时间戳比较
来源：http://hz.hywenlv.cn/gtuqztexar.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.guannengcc.top/gtmxmdmarx.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.shangyingyoupin.top/gtrnmnswxf.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.vqdsnc.cn/gtrrulcykf.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.cqqwz.cn/gtgljjcsvp.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.shanyushiyangtech.top/gtwawlskmx.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.tian-w.cn/gtxrpdjymr.html

[P08] 处理浮点精度问题
来源：http://hz.zhoulong.xyz/gttphuxhfb.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.svipenyu.cn/gtfjrlmpsf.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.jinyuanbaomall.cn/gttihvjgvy.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.hysaishi.cn/gtusrtmfuv.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.zycfv.cn/gtoybvaavo.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.jinqigufen.top/gtkhotytby.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.shanyushiyangtech.top/gtkmikzadl.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.sufxvd.cn/gthfhvjbax.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.hammf.cn/gtmoymimdb.html

================================================================================
来源：http://hz.wangdashe.top/gtowikrpbl.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.yj20258.top/gtnhvsxsjv.html

================================================================================
来源：http://hz.hnxiangtu.top/gtqcksrate.html

[Q01] 创建表
来源：http://hz.xingfuxueyuan.xyz/gtyfiejnrk.html

CREATE TABLE users (
来源：http://hz.hnqzz.top/gtxqmrdljx.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.nwbrower.top/gtwllexmmf.html

name VARCHAR(50) NOT NULL,
来源：http://hz.yj202588.top/gtjsasoank.html

email VARCHAR(100) UNIQUE,
来源：http://hz.52xcode.cn/gtkpipouvn.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.jinyuanbaomall.cn/gtiocjfhln.html

);
来源：http://hz.yanxiufei.cn/gtiosehqnr.html

[Q02] 创建带外键的表
来源：http://hz.daxiang520.top/gtbbfjclkv.html

CREATE TABLE orders (
来源：http://hz.jqgfzy.top/gtiquyetxo.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.hnqzz.top/gtnpatomho.html

user_id INT NOT NULL,
来源：http://hz.sweek.top/gtbnrpemyq.html

amount DECIMAL(10, 2),
来源：http://hz.cqqwz.cn/gtrkuiuahc.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.yueranfly.top/gtrkagzivg.html

);
来源：http://hz.9152youxi.cn/gtqcphaysl.html

[Q03] 增加列
来源：http://hz.meibo888.top/gtmzznlvcj.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.cheryme.top/gtrnvulldy.html

[Q04] 修改列类型
来源：http://hz.hfpthk.cn/gtkxzrdnsa.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.jqgufenzy.top/gtdjqmdzbz.html

[Q05] 重命名列
来源：http://hz.hnqzz.top/gtzgocohde.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.hysaishi.cn/gttujjgutb.html

[Q06] 删除列
来源：http://hz.xylfe.cn/gtcdtnygvg.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.yueranfly.top/gtmlxmvwhp.html

[Q07] 删除表
来源：http://hz.hywenlv.cn/gtdlfwnshw.html

DROP TABLE IF EXISTS orders;
来源：http://hz.xingfuxueyuan.xyz/gtwiiaekso.html

[Q08] 创建普通索引
来源：http://hz.hywenlv.cn/gtjxomqaoo.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.iojbl.cn/gtwoenpvqj.html

[Q09] 创建唯一索引
来源：http://hz.pengpengdd.cyou/gtgftknmfn.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.dianchejie.cn/gtfvorrxtu.html

[Q10] 插入单行
来源：http://hz.fzhhl.top/gtxnymqpof.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.shzxlz.cn/gtuglmiiya.html

[Q11] 一次插入多行
来源：http://hz.yuanzhike.top/gtyqyncoka.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.yonumen.top/gtbhvlbhfv.html

[Q12] 插入后取自增 ID
来源：http://hz.jqgfzy.top/gtoxmpbjvu.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.wangshuangyany.cn/gtixiqjugm.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.cdnleiting.top/gtttkfcjvb.html

[Q13] 忽略重复插入
来源：http://hz.52xcode.cn/gtewbatkcd.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.sufxvd.cn/gtlowmkqzp.html

[Q14] 存在则更新（upsert）
来源：http://hz.tanke756.top/gtbszjppdk.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.cashguo.top/gtywlujboa.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.hysaishi.cn/gttfoylqvc.html

[Q15] 查询全部
来源：http://hz.dianchejie.cn/gtgamzkmui.html

SELECT * FROM users;
来源：http://hz.havefunace.top/gtfzkkjvsz.html

[Q16] 查询指定列
来源：http://hz.gzhubu.top/gtxapbuake.html

SELECT id, name FROM users;
来源：http://hz.nanxinkj.top/gtcdurekpi.html

[Q17] 条件查询
来源：http://hz.zhiwuduotai.top/gtkbhmxbag.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.chenzaomai.com/gtpdjdbhzx.html

[Q18] 模糊匹配
来源：http://hz.yanxiufei.cn/gtjlaphgex.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.zhongyouzk.top/gtbftracsy.html

[Q19] 范围查询
来源：http://hz.zhijiandao.cn/gtdxgnmgry.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.shangyingyoupin.top/gtcreqeveo.html

[Q20] IN 列表
来源：http://hz.sufxvd.cn/gtavxzwyod.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.jlsjyb.cn/gtwftvphus.html

[Q21] 空值判断
来源：http://hz.cucudq.cn/gtagwtnkxs.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.zhijiandao.cn/gtcmgbjaad.html

[Q22] 排序
来源：http://hz.ehwqpu.com/gtxvehodmj.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.xylfe.cn/gtdxnlawwb.html

[Q23] 分页
来源：http://hz.cashguo.top/gtqwhzxgoy.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.fzhhl.top/gtpnpokkmg.html

[Q24] 去重
来源：http://hz.quarkkingdee.top/gtzlsifryn.html

SELECT DISTINCT city FROM users;
来源：http://hz.svipenyu.cn/gtbjgkwtal.html

[Q25] 只取前 N 条
来源：http://hz.fzhhl.top/gttehtdjkj.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.andypj.xyz/gtntjorpds.html

[Q26] 计数
来源：http://hz.jiagoushi.top/gtlvvkuvba.html

SELECT COUNT(*) FROM users;
来源：http://hz.aizwys.cn/gtkgqubrnz.html

[Q27] 条件计数
来源：http://hz.chenzaomai.com/gtvftrilao.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.feifeiyinyue.top/gthzqussya.html

[Q28] 求和与平均
来源：http://hz.jinghuilouyu.cn/gtwmepeqgc.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.ivvv.top/gtnrytyzhi.html

[Q29] 最大最小值
来源：http://hz.jyoumei.cn/gtmmsbuuor.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.chenjidiqi.icu/gtozbwbnof.html

[Q30] 分组统计
来源：http://hz.hfpthk.cn/gtuatswawf.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.chenzaomai.com/gtdawfbqfg.html

[Q31] 分组后过滤
来源：http://hz.wangdashe.top/gtiakwidmz.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.xziqi.cn/gtycutzshc.html

[Q32] 分组拼接字符串
来源：http://hz.xingfuxueyuan.xyz/gtoyimngnn.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.svipenyu.cn/gtlxozahvj.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.dashuyun.cn/gtyvxbdfrv.html

[Q33] 多列分组
来源：http://hz.hnqzz.top/gttmaimayr.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.tanke756.top/gtdlsibasv.html

[Q34] 每组取第一条
来源：http://hz.bjfxy.top/gtcuptbqpu.html

SELECT * FROM (
来源：http://hz.nanxuanxn.top/gtwybaczyu.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.bjfxy.top/gtvitxgfbi.html

) t WHERE rn = 1;
来源：http://hz.mhx1999.top/gtrqhavogk.html

[Q35] 内连接
来源：http://hz.cheryme.top/gthmhwdtpw.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.zdqjudy.top/gtimizbjyg.html

[Q36] 左连接
来源：http://hz.sufxvd.cn/gtcjqakuwc.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.xylfe.cn/gtzwqalmip.html

[Q37] 右连接
来源：http://hz.tianlin.xyz/gtymehkxbz.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.0kj1m.cn/gtzpbhimjh.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.wangdashe.top/gtrjdbvxkv.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.xylfe.cn/gtxmkcbbyc.html

[Q39] 自连接（查上下级）
来源：http://hz.yangfankeji.com/gtvrdkntlj.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.hammf.cn/gtobhqbzaf.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.feifeiyinyue.top/gtpduwszcx.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.jinqigufen.top/gtxflsjgpy.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.hongshengwenyu.top/gtbxxllsvk.html

[Q41] 多表连接
来源：http://hz.52xcode.cn/gtvqezarku.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.tanke756.top/gtnieirynx.html

JOIN users u ON u.id = o.user_id
来源：http://hz.zhixingplan.top/gtlhotvqof.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.zhongyouzk.top/gtzxcnfwky.html

[Q42] 连接条件附加过滤
来源：http://hz.gotoacloud.top/gtlfsjijlp.html

SELECT u.name, o.amount FROM users u
来源：http://hz.zhijiandao.cn/gtdjivgeak.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.xingfuxueyuan.xyz/gtogoidjxb.html

[Q43] 标量子查询
来源：http://hz.pycfn.com/gtyamocsuq.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.yongpay.top/gtmffimlhx.html

[Q44] IN 子查询
来源：http://hz.haohaochexian.top/gtwttzpkzk.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.smart0.xyz/gtvweftbuk.html

[Q45] EXISTS 判断存在
来源：http://hz.jiagoushi.top/gtuxegnyya.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.wangshuangyany.cn/gttzmsiplv.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.mhx1999.top/gtxdgxrfgb.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.ppjwa.cn/gtnnbubwtc.html

[Q47] 与平均值比较
来源：http://hz.zhiwuduotai.top/gtnrfuqnec.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.ppjwa.cn/gtjeothxnp.html

[Q48] CTE 公用表表达式
来源：http://hz.daria6918.cn/gtdlpqvpnq.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.wangshuangyany.cn/gtsijrfgdc.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.gzhubu.top/gtvfiaomlb.html

[Q49] 更新单行
来源：http://hz.yueranfly.top/gtsbxtdrlb.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.chenjidiqi.icu/gttuxsdodv.html

[Q50] 批量更新
来源：http://hz.zhixingplan.top/gtcatgpyyu.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.mhx1999.top/gtnblzxhmt.html

[Q51] 用子查询更新
来源：http://hz.kuanghao11.cn/gtitnlrtfo.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.fengsongda.top/gtbclezytd.html

[Q52] 删除指定行
来源：http://hz.zhengqikj.top/gtnunikyhc.html

DELETE FROM users WHERE id = 10;
来源：http://hz.cheryme.top/gtxuwyhljr.html

[Q53] 按条件删除
来源：http://hz.iojbl.cn/gtcxsthpot.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.ywan-chungtsiang.top/gteernkskf.html

[Q54] 清空表
来源：http://hz.hysaishi.cn/gtfsuqxusf.html

TRUNCATE TABLE logs;
来源：http://hz.hywenlv.cn/gtmhswmcge.html

[Q55] 排名（并列占位）
来源：http://hz.vqdsnc.cn/gtwkyvxvls.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.jinqigfzy.top/gtgniqluty.html

[Q56] 密集排名（并列不占位）
来源：http://hz.0kj1m.cn/gtcpnbenop.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.ehwqpu.com/gtoaydtjlg.html

[Q57] 行号
来源：http://hz.feifeiyinyue.top/gteuepsfbd.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.xingfuxueyuan.xyz/gtcuziyupn.html

[Q58] 累计求和
来源：http://hz.smart0.xyz/gtbrphyekd.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.zhaomingkeji.xyz/gtufzcvggn.html

[Q59] 分组内累计
来源：http://hz.zdqjudy.top/gtadgdgqyv.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.ybcxt.top/gtkkamjdqa.html

[Q60] 取上一行 / 下一行
来源：http://hz.316326.xyz/gtwfhhuslf.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.guannengcc.top/gtcsedifwm.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.hywenlv.cn/gtsdsdvaan.html

[Q61] 移动平均
来源：http://hz.daxiang520.top/gttkidyaao.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.ivvv.top/gtsnrkqjja.html

[Q62] 分组占比
来源：http://hz.wangdashe.top/gtddqahbra.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.tian-w.cn/gtjqtgqrsq.html

[Q63] 开启事务
来源：http://hz.xylfe.cn/gtwfxqguxw.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.yongpay.top/gtovwyxjhd.html

[Q64] 提交事务
来源：http://hz.fengsongda.top/gtezurihmr.html

COMMIT;
来源：http://hz.0kj1m.cn/gtxpygcyvw.html

[Q65] 回滚事务
来源：http://hz.tian-w.cn/gtyngahvmp.html

ROLLBACK;
来源：http://hz.yj20258888.top/gtphpiicjj.html

[Q66] 行锁查询
来源：http://hz.ppjwa.cn/gtadprtrik.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.hongshengwenyu.top/gtuntxzsgm.html

[Q67] 设置隔离级别
来源：http://hz.yangfankeji.com/gtcnwhioeb.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.ehwqpu.com/gtapedsdfc.html

[Q68] 保存点
来源：http://hz.ydzc1.top/gtqueyufrt.html

SAVEPOINT sp1;
来源：http://hz.yanxiufei.cn/gtftzhdeeh.html

ROLLBACK TO sp1;
来源：http://hz.cucudq.cn/gtbkdcpoei.html

[Q69] 查看执行计划
来源：http://hz.hnqzz.top/gtwobxtzjc.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.jyoumei.cn/gtoiqcbmsx.html

[Q70] 更新统计信息
来源：http://hz.wangshuangyany.cn/gtlruvxuwg.html

ANALYZE TABLE users;
来源：http://hz.nwbrower.top/gtyeohlypd.html

[Q71] 查看建表语句
来源：http://hz.sufxvd.cn/gtfafuyruk.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.havefunace.top/gtsxwyvamg.html

[Q72] 查看索引
来源：http://hz.jyoumei.cn/gtgkdxpqcz.html

SHOW INDEX FROM users;
来源：http://hz.mhx1999.top/gtbrgahmrm.html

[Q73] 查看表状态
来源：http://hz.daria6918.cn/gtijnrwkrz.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.yj20258.top/gtknrtqoiw.html

[Q74] 强制使用索引
来源：http://hz.feifeiyinyue.top/gticsmzmyv.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.hammf.cn/gtqxdapahh.html

[Q75] 日期格式化
来源：http://hz.shanyushiyangtech.top/gttmnzugwa.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.kuanghao11.cn/gtkemvmnof.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.zhaomingkeji.xyz/gtcmsjlqbl.html

[Q76] 按天统计
来源：http://hz.ywan-chungtsiang.top/gtmwqmzqcz.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.xuanzx.com/gtkgmbqhnd.html

[Q77] 时间加减
来源：http://hz.zdqjudy.top/gtwwzawfhk.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.xziqi.cn/gtwasvbysc.html

[Q78] 当前时间
来源：http://hz.yvedp.cn/gtrdxpjmgm.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.shzxlz.cn/gtokblrrqf.html

[Q79] 字符串拼接
来源：http://hz.mhx1999.top/gtewphbtbs.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.pycfn.com/gtibirxrcw.html

[Q80] 字符串截取
来源：http://hz.chenjidiqi.icu/gtoinviwdb.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.yongpay.top/gtzstsebmi.html

[Q81] 字符串替换
来源：http://hz.snrcjt.cn/gtqwcxmmxz.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.xziqi.cn/gtqnmebwqa.html

[Q82] 字符长度与字节长度
来源：http://hz.xingfuxueyuan.xyz/gtkxkagmvw.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.jinqigufen.top/gtlroqoyks.html

[Q83] 大小写转换
来源：http://hz.yuanzhike.top/gtgymatrrn.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.tian-w.cn/gtixakscbi.html

[Q84] 去除首尾空格
来源：http://hz.nanxinkj.top/gtegdyjwxj.html

SELECT TRIM(name) FROM users;
来源：http://hz.zhongyouzk.top/gtvcpcuoef.html

[Q85] 数值取整
来源：http://hz.xuanzx.com/gtyfiluseb.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.cdnleiting.top/gtlsorcmnp.html

[Q86] 读取 JSON 字段
来源：http://hz.jinqigfzy.top/gtjntfphem.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.shanyushiyangtech.top/gtifnnukhx.html

[Q87] JSON 字段做条件
来源：http://hz.kuanghao11.cn/gtfmeohfuf.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.yonumen.top/gtpgpalpzp.html

[Q88] 行转列（条件聚合）
来源：http://hz.yonumen.top/gtijscnucb.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.tian-w.cn/gtteisqhsk.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.jianghu66.top/gtxvjdarvk.html

[Q89] 判断表是否存在
来源：http://hz.jyoumei.cn/gtxyimzton.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.jyoumei.cn/gtapmpstgt.html

[Q90] 生成序号列
来源：http://hz.hfpthk.cn/gtdfenvxxq.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.xinyue.icu/gtfjqxmonm.html

================================================================================
来源：http://hz.guannengcc.top/gtjwvtvula.html

R. Bash 专题
来源：http://hz.xuanzx.com/gtanulmtst.html

================================================================================
来源：http://hz.jianghu66.top/gtkipqjfxi.html

[R01] shebang 与严格模式
来源：http://hz.tianlin.xyz/gtqbaugegs.html

#!/usr/bin/env bash
来源：http://hz.vqdsnc.cn/gtqwpxnayo.html

set -euo pipefail
来源：http://hz.hysaishi.cn/gtluurzjyk.html

[R02] 变量赋值与使用
来源：http://hz.shanyushiyangkeji.top/gtuwjlkuxz.html

name="Tom"; echo "$name"
来源：http://hz.feifeiyinyue.top/gtimmxkycn.html

[R03] 只读变量
来源：http://hz.ydzc1.top/gtrdrdjxmv.html

readonly PI=3.14
来源：http://hz.jqgfzy.top/gtjhttdfos.html

[R04] 位置参数
来源：http://hz.ydzc1.top/gteupfaiyg.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.ywan-chungtsiang.top/gtcqctqhbs.html

[R05] 参数默认值
来源：http://hz.jinyuanbaomall.cn/gtukuouteu.html

name="${1:-default}"
来源：http://hz.pycfn.com/gtrkkqxsxu.html

[R06] 判断命令是否存在
来源：http://hz.zhijiandao.cn/gtenprfnpt.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.pengpengdd.cyou/gtackeugla.html

[R07] if 判断文件
来源：http://hz.haohaochexian.top/gtpzsevrsh.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.haohaochexian.top/gtclsoswrs.html

[R08] 数值比较
来源：http://hz.jinqigfzy.top/gtbjpardcm.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.daria6918.cn/gtxlzdqlck.html

[R09] 字符串比较
来源：http://hz.chenzaomai.com/gtjjpquokk.html


<!-- 参考信息 -->