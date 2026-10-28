代发 wailian999

C#:   Parallel.For
来源：http://hz.ydjk.org.cn/gtgzvgywip.html

================================================================================
来源：http://hz.chenzaomai.com/gtoyaygbrw.html

P. 常用工具函数
来源：http://hz.yuxming.cn/gtqdlogrfp.html

================================================================================
来源：http://hz.ppjwa.cn/gtvpsqhdkd.html

[P01] 生成 UUID
来源：http://hz.yangfankeji.com/gtstlfuvgi.html

Py:   str(uuid.uuid4())
来源：http://hz.jqgufenzy.top/gtedlpbvep.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.0kj1m.cn/gtzrsehsei.html

JS:   crypto.randomUUID()
来源：http://hz.cqqwz.cn/gtgwhqikmc.html

TS:   crypto.randomUUID()
来源：http://hz.xingfuxueyuan.xyz/gttnnyiyjo.html

Java: UUID.randomUUID().toString()
来源：http://hz.zhongyouzk.top/gtjyaupowc.html

Go:   // 用 github.com/google/uuid
来源：http://hz.hysaishi.cn/gtyjnaiigj.html

Ruby: SecureRandom.uuid
来源：http://hz.jinqigufen.top/gttjeaywgh.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.hnqzz.top/gtnelnvltk.html

[P02] MD5 / SHA256 摘要
来源：http://hz.tianlin.xyz/gthgwyqsnt.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.zhijiandao.cn/gtvythwaad.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.shzxlz.cn/gtzhmdoxck.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.smart0.xyz/gtdxctsmzm.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.hywenlv.cn/gtnieiirei.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.sysykeji.top/gtsambgvxc.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.zhijiandao.cn/gtbezgevdw.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.jianghu66.top/gtnnspewee.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.hysaishi.cn/gttihbcvcy.html

[P03] 生成短随机字符串
来源：http://hz.sweek.top/gtezgdzgrv.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.jinghuilouyu.cn/gtqkcopqaa.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.pycfn.com/gtzjryrxrj.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.wangdashe.top/gtuifwahdc.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.aizwys.cn/gtahfiyhjo.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.hammf.cn/gtqskdjbkz.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.nanxuanxn.top/gtcdgzagnn.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.gotoacloud.top/gtvjxpyszk.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.jinghuilouyu.cn/gtaykzzqqw.html

[P04] 求长度
来源：http://hz.tianlin.xyz/gtfpdsettu.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.andypj.xyz/gtiozcmxvb.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yangfankeji.com/gtsreaioig.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.shzxlz.cn/gtoqjwtmwg.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.daria6918.cn/gtswmdhsng.html

Java: list.size();  map.size();  s.length()
来源：http://hz.pengpengdd.cyou/gtbxjbyucj.html

Go:   len(arr);  len(m)
来源：http://hz.jinyuanbaomall.cn/gtyvactekr.html

Ruby: x.length;  x.size
来源：http://hz.mhx1999.top/gtnsbkgiay.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.zhoulong.xyz/gtxfbzskdv.html

[P05] 判断两个对象内容是否相等
来源：http://hz.guannengcc.top/gtjqcgmaio.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.xingfuxueyuan.xyz/gtfhxokkst.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.sufxvd.cn/gtomkjiqzt.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.tanke756.top/gtwtbtpyoa.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.jqgufenzy.top/gthxhstzhm.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.jinyuanbaomall.cn/gtglqjfxnr.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.c1oappe.top/gtwgnsmmrj.html

Ruby: a == b
来源：http://hz.hywenlv.cn/gtnrgrkfuz.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.bjfxy.top/gtivlmpnge.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.gzhubu.top/gtjvrzzkvq.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.svipenyu.cn/gtlovzqsug.html

PHP:  if (empty($x)) {}
来源：http://hz.ydjk.org.cn/gtdgdslnbq.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.52xcode.cn/gtdtjerqxm.html

TS:   if (x == null) {}
来源：http://hz.hongshengwenyu.top/gthiagzcff.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.wangdashe.top/gtdxjqwjzg.html

Go:   if x == nil {}
来源：http://hz.dianchejie.cn/gtewssmhog.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.ybcxt.top/gtqcmkmfso.html

C#:   if (x is null) {}
来源：http://hz.iojbl.cn/gtenbwskgl.html

[P07] 防抖与节流
来源：http://hz.316326.xyz/gtgzhbostr.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.shzxlz.cn/gtjbctjhxf.html

PHP:  // 手写时间戳比较
来源：http://hz.cucudq.cn/gtmietcdls.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.dashuyun.cn/gtgwlbnhlv.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.kuanghao11.cn/gtijxhgoob.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.zhiwuduotai.top/gtljgwvrlu.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.xinyue.icu/gtrasocizl.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.dashuyun.cn/gtssthgrbk.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.redwolf501.top/gttfpkwolm.html

[P08] 处理浮点精度问题
来源：http://hz.fzhhl.top/gtnfnykpae.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.yj20258.top/gthuyksuqn.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.smart0.xyz/gtmwrpbovw.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.gaohongyu789.top/gtknnijbhj.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.hysaishi.cn/gtaznxrswn.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.fzhhl.top/gtzpnmeiqf.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.cdnleiting.top/gtymykcmmg.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.yuanzhike.top/gtnicbwojd.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.yj202588.top/gtbpbhravk.html

================================================================================
来源：http://hz.tianlin.xyz/gtscthzytm.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.sweek.top/gtljchyjxu.html

================================================================================
来源：http://hz.gotoacloud.top/gtcmpdvtpa.html

[Q01] 创建表
来源：http://hz.hnxiangtu.top/gtemukvxfc.html

CREATE TABLE users (
来源：http://hz.yuxming.cn/gtjzeofzpa.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.hnqzz.top/gtjtxazemi.html

name VARCHAR(50) NOT NULL,
来源：http://hz.ehwqpu.com/gtbzlqcsub.html

email VARCHAR(100) UNIQUE,
来源：http://hz.haohaochexian.top/gtvodtryzf.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.shanyushiyangkeji.top/gtzgjaxbot.html

);
来源：http://hz.dashuyun.cn/gtfchmkxiq.html

[Q02] 创建带外键的表
来源：http://hz.ybcxt.top/gtspnnvkfb.html

CREATE TABLE orders (
来源：http://hz.gzhubu.top/gtfseuljvi.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yuanzhike.top/gtppvhxzud.html

user_id INT NOT NULL,
来源：http://hz.snrcjt.cn/gtukqgcsmm.html

amount DECIMAL(10, 2),
来源：http://hz.ywan-chungtsiang.top/gtjfcjozch.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.chenlongwang.top/gtwldohpwp.html

);
来源：http://hz.chenlongwang.top/gtpjobelge.html

[Q03] 增加列
来源：http://hz.nanxinkj.top/gtpnwgthlt.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.hywenlv.cn/gtxfgrazmq.html

[Q04] 修改列类型
来源：http://hz.zhijiandao.cn/gthwvgsvvz.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.redwolf501.top/gtfsskvxak.html

[Q05] 重命名列
来源：http://hz.chenjidiqi.icu/gtmjcfyzoe.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.chenjidiqi.icu/gtpzprvhxt.html

[Q06] 删除列
来源：http://hz.jqgufenzy.top/gtsnakumjt.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.dianchejie.cn/gtbpiytobs.html

[Q07] 删除表
来源：http://hz.cdnleiting.top/gtsnsresvc.html

DROP TABLE IF EXISTS orders;
来源：http://hz.xingfuxueyuan.xyz/gtjfqpsdlr.html

[Q08] 创建普通索引
来源：http://hz.nanxuanxn.top/gtsbiahevz.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.hammf.cn/gtpxmogder.html

[Q09] 创建唯一索引
来源：http://hz.cashguo.top/gtvxpgdboq.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.shangyingyoupin.top/gtawnvwwwe.html

[Q10] 插入单行
来源：http://hz.fzhhl.top/gtxflyiusl.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.ybcxt.top/gtuctokqvg.html

[Q11] 一次插入多行
来源：http://hz.meibo888.top/gtbgacpztn.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.jianghu66.top/gtvmzaoykv.html

[Q12] 插入后取自增 ID
来源：http://hz.haohaochexian.top/gtycqrglkd.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.chenzaomai.com/gtokpkampv.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.c1oappe.top/gtyfdgokor.html

[Q13] 忽略重复插入
来源：http://hz.hywenlv.cn/gtjjxjkrvl.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.dashuyun.cn/gtibiythye.html

[Q14] 存在则更新（upsert）
来源：http://hz.cucudq.cn/gtdpmhxthz.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.jinghuilouyu.cn/gtxzicgtgm.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.jinghuilouyu.cn/gtjuljgfzo.html

[Q15] 查询全部
来源：http://hz.ydjk.org.cn/gtxpbjzzvi.html

SELECT * FROM users;
来源：http://hz.hnxiangtu.top/gtaiifynxk.html

[Q16] 查询指定列
来源：http://hz.jiagoushi.top/gtmgoqjlyi.html

SELECT id, name FROM users;
来源：http://hz.guowangkeji.top/gtuxmtqind.html

[Q17] 条件查询
来源：http://hz.zhengqikj.top/gtpxyfiywl.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.sufxvd.cn/gtvtadsqji.html

[Q18] 模糊匹配
来源：http://hz.nanxuanxn.top/gtfxdktnsr.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.nanxuanxn.top/gttlfcjdoc.html

[Q19] 范围查询
来源：http://hz.yonumen.top/gtgeobigpf.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.tanke756.top/gtxfnlqvsi.html

[Q20] IN 列表
来源：http://hz.52xcode.cn/gtpehcobej.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.andypj.xyz/gtcxiurpnx.html

[Q21] 空值判断
来源：http://hz.dianchejie.cn/gtpvxjszoo.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.sweek.top/gtvmtlupwc.html

[Q22] 排序
来源：http://hz.xingfuxueyuan.xyz/gtkybysbmb.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.yueranfly.top/gtidmfqeln.html

[Q23] 分页
来源：http://hz.cashguo.top/gtzoqjwnme.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.hysaishi.cn/gtviahmdkw.html

[Q24] 去重
来源：http://hz.jqgfzy.top/gtcgkfcasz.html

SELECT DISTINCT city FROM users;
来源：http://hz.tianlin.xyz/gtnffnxrzo.html

[Q25] 只取前 N 条
来源：http://hz.iojbl.cn/gtjudiqxax.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.cashguo.top/gtxsaqcpwm.html

[Q26] 计数
来源：http://hz.cqqwz.cn/gtinisefzv.html

SELECT COUNT(*) FROM users;
来源：http://hz.zhijiandao.cn/gtfgcmyfhv.html

[Q27] 条件计数
来源：http://hz.birdmap.top/gtbphnsnav.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.dianchejie.cn/gtpebysqgi.html

[Q28] 求和与平均
来源：http://hz.ivvv.top/gtcsujmjwl.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.cdnleiting.top/gtpkczqzxs.html

[Q29] 最大最小值
来源：http://hz.yueranfly.top/gttmbtapvw.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.zdqjudy.top/gtgbkgiham.html

[Q30] 分组统计
来源：http://hz.jqgfzy.top/gtnjzydwjc.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.jyoumei.cn/gtqbvvevqf.html

[Q31] 分组后过滤
来源：http://hz.yongpay.top/gtfypkmeme.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.cdnleiting.top/gtlguhjjwy.html

[Q32] 分组拼接字符串
来源：http://hz.xingfuxueyuan.xyz/gtemytfhar.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.jianghu66.top/gtffzrpjho.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.jyoumei.cn/gthzylxtfz.html

[Q33] 多列分组
来源：http://hz.aibaodan.cn/gtfpftxgrl.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.shanyushiyangkeji.top/gttvhpnoxf.html

[Q34] 每组取第一条
来源：http://hz.smart0.xyz/gtskrjvwsr.html

SELECT * FROM (
来源：http://hz.chenlongwang.top/gttsrjzmls.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.ybcxt.top/gttxhjnmvs.html

) t WHERE rn = 1;
来源：http://hz.nanxuanxn.top/gtbjxlbbiq.html

[Q35] 内连接
来源：http://hz.dashuyun.cn/gtxmcuwzdj.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.9152youxi.cn/gtyvwgvzap.html

[Q36] 左连接
来源：http://hz.andypj.xyz/gtgfuvczcn.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.yj20258888.top/gteqehdkle.html

[Q37] 右连接
来源：http://hz.guannengcc.top/gtechmprpr.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.sweek.top/gtaqgnypxr.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.kuanghao11.cn/gtkzapwbsn.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.gogol.net.cn/gtvsqvtjhd.html

[Q39] 自连接（查上下级）
来源：http://hz.chenjidiqi.icu/gtecgbfnam.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.iojbl.cn/gtfivghldy.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.hnqzz.top/gtciidhpuo.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.ydzc1.top/gtikijdadj.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.hfpthk.cn/gtkrrrxnae.html

[Q41] 多表连接
来源：http://hz.hnqzz.top/gtdgkybqxk.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.yangfankeji.com/gtlqgvepcs.html

JOIN users u ON u.id = o.user_id
来源：http://hz.sufxvd.cn/gtmfqpmjyk.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.hysaishi.cn/gtewbdcnva.html

[Q42] 连接条件附加过滤
来源：http://hz.shangyingyoupin.top/gtgaatxnnj.html

SELECT u.name, o.amount FROM users u
来源：http://hz.hywenlv.cn/gtejjhuqao.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.hnxiangtu.top/gtmtydigta.html

[Q43] 标量子查询
来源：http://hz.nanxinkj.top/gtdelugrva.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.fengsongda.top/gtkrbsrsdu.html

[Q44] IN 子查询
来源：http://hz.sxryk.cn/gtspqyxcwv.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.daxiang520.top/gthbbvpbou.html

[Q45] EXISTS 判断存在
来源：http://hz.jianghu66.top/gtgcjjgsgf.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.nanxuanxn.top/gttzexfxnp.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.shanyushiyangkeji.top/gtwmwgahmj.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.cashguo.top/gtrbkctqoq.html

[Q47] 与平均值比较
来源：http://hz.zdqjudy.top/gtbuvqrlwq.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.bjfxy.top/gtzqnwyclq.html

[Q48] CTE 公用表表达式
来源：http://hz.shanyushiyangtech.top/gtsajksout.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.yueranfly.top/gtaieoccxh.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.gogol.net.cn/gtlxqtffko.html

[Q49] 更新单行
来源：http://hz.fengsongda.top/gtmfzybzre.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.chenjidiqi.icu/gtggbajity.html

[Q50] 批量更新
来源：http://hz.gogol.net.cn/gtmqakpnmp.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.dashuyun.cn/gtnnwmwlea.html

[Q51] 用子查询更新
来源：http://hz.chenzaomai.com/gtgvvdurgi.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.sysykeji.top/gtroqzvdsf.html

[Q52] 删除指定行
来源：http://hz.zdqjudy.top/gtlcfjqxtx.html

DELETE FROM users WHERE id = 10;
来源：http://hz.xziqi.cn/gtndfjuqul.html

[Q53] 按条件删除
来源：http://hz.ivvv.top/gtetugnbdb.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.yongpay.top/gtyxqllyrb.html

[Q54] 清空表
来源：http://hz.yj20258888.top/gtwoxoivzm.html

TRUNCATE TABLE logs;
来源：http://hz.chenjidiqi.icu/gtpstygwdn.html

[Q55] 排名（并列占位）
来源：http://hz.pengpengdd.cyou/gtrtzcyfrp.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.gzhubu.top/gtdctmghge.html

[Q56] 密集排名（并列不占位）
来源：http://hz.ydjk.org.cn/gtoxsminkz.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.cheryme.top/gtbenrgjno.html

[Q57] 行号
来源：http://hz.jinqigufen.top/gtkbznrtsc.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.yj202588.top/gtgzjdkmqk.html

[Q58] 累计求和
来源：http://hz.sufxvd.cn/gtjluiufac.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.0kj1m.cn/gtvpjpbcca.html

[Q59] 分组内累计
来源：http://hz.hnxiangtu.top/gtgijidtgb.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.316326.xyz/gtumtcfbwz.html

[Q60] 取上一行 / 下一行
来源：http://hz.xuetiantiany.cn/gtbmuqqfhw.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.yj20258888.top/gtomofvepn.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.c1oappe.top/gtjsagfprb.html

[Q61] 移动平均
来源：http://hz.redwolf501.top/gtbfwmyfsx.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.zhiwuduotai.top/gtaigbxvwn.html

[Q62] 分组占比
来源：http://hz.sxryk.cn/gttnjwjzul.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.chenzaomai.com/gtwbnhztaa.html

[Q63] 开启事务
来源：http://hz.wangshuangyany.cn/gtkkhiidvw.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.shzxlz.cn/gtrhlvcgqb.html

[Q64] 提交事务
来源：http://hz.gaohongyu789.top/gtekagrxjq.html

COMMIT;
来源：http://hz.quarkkingdee.top/gtzatqvaid.html

[Q65] 回滚事务
来源：http://hz.zdqjudy.top/gtnqeiirna.html

ROLLBACK;
来源：http://hz.shuidangran.top/gtolnnyykl.html

[Q66] 行锁查询
来源：http://hz.yanxiufei.cn/gtbqnddchx.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.cheryme.top/gtgzapqdkk.html

[Q67] 设置隔离级别
来源：http://hz.pycfn.com/gtwcvjvxxx.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.jqgfzy.top/gtfizoblht.html

[Q68] 保存点
来源：http://hz.nanxinkj.top/gtsphctcdv.html

SAVEPOINT sp1;
来源：http://hz.zhengqikj.top/gtxraudsoc.html

ROLLBACK TO sp1;
来源：http://hz.sufxvd.cn/gtfzibugvj.html

[Q69] 查看执行计划
来源：http://hz.cashguo.top/gtjhlmmlic.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.smart0.xyz/gtfxzvxjaj.html

[Q70] 更新统计信息
来源：http://hz.andypj.xyz/gtemfojobq.html

ANALYZE TABLE users;
来源：http://hz.vqdsnc.cn/gtswbzecod.html

[Q71] 查看建表语句
来源：http://hz.snrcjt.cn/gtfbkrgunz.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.andypj.xyz/gtrcmbypxv.html

[Q72] 查看索引
来源：http://hz.hysaishi.cn/gtqjdsxcto.html

SHOW INDEX FROM users;
来源：http://hz.gaohongyu789.top/gtjunbwrhb.html

[Q73] 查看表状态
来源：http://hz.yonumen.top/gthycflayd.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.bjfxy.top/gtnyhweffm.html

[Q74] 强制使用索引
来源：http://hz.yangfankeji.com/gtixpigzco.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.yuxming.cn/gthfwtohic.html

[Q75] 日期格式化
来源：http://hz.kuanghao11.cn/gtlwfzmchs.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.cqqwz.cn/gtxjizwyfn.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.sysykeji.top/gtoolfyjwq.html

[Q76] 按天统计
来源：http://hz.jinyuanbaomall.cn/gthyidaamd.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.ydjk.org.cn/gtbrbsnrwm.html

[Q77] 时间加减
来源：http://hz.yj202588.top/gtekpmsiew.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.sysykeji.top/gtcqdkqacs.html

[Q78] 当前时间
来源：http://hz.yj20258888.top/gtlzfnxizb.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.zhaomingkeji.xyz/gtcoafczdl.html

[Q79] 字符串拼接
来源：http://hz.cqqwz.cn/gtaoiyvdzt.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.hnxiangtu.top/gtstcxeobr.html

[Q80] 字符串截取
来源：http://hz.yuanzhike.top/gtqgoctplm.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.zhiwuduotai.top/gtijtqnzxf.html

[Q81] 字符串替换
来源：http://hz.zhixingplan.top/gtbzjbddah.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.hammf.cn/gtpztsltvz.html

[Q82] 字符长度与字节长度
来源：http://hz.gaohongyu789.top/gtcaaitepp.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.quarkkingdee.top/gtdqyqnyor.html

[Q83] 大小写转换
来源：http://hz.snrcjt.cn/gthfccnkbh.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.fengsongda.top/gtymdbfrdz.html

[Q84] 去除首尾空格
来源：http://hz.shanyushiyangkeji.top/gtvmwldhbo.html

SELECT TRIM(name) FROM users;
来源：http://hz.pycfn.com/gtbetwmzbw.html

[Q85] 数值取整
来源：http://hz.cqqwz.cn/gtetfnugra.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.ybcxt.top/gtcxdityrn.html

[Q86] 读取 JSON 字段
来源：http://hz.cheryme.top/gthwrytfhm.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.aibaodan.cn/gtlgznuolv.html

[Q87] JSON 字段做条件
来源：http://hz.jinqigufen.top/gtgqkciqik.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.hywenlv.cn/gtbepgxlaw.html

[Q88] 行转列（条件聚合）
来源：http://hz.feifeiyinyue.top/gtnidileaf.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.chenjidiqi.icu/gtqhotcmqi.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.meibo888.top/gtcwhqfjzo.html

[Q89] 判断表是否存在
来源：http://hz.52xcode.cn/gthgygqrxd.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.zhixingplan.top/gtyubpdeyo.html

[Q90] 生成序号列
来源：http://hz.aizwys.cn/gtmzlczdwi.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.vqdsnc.cn/gtsadywnit.html

================================================================================
来源：http://hz.jqgufenzy.top/gtpecslucd.html

R. Bash 专题
来源：http://hz.xylfe.cn/gtnftuwser.html

================================================================================
来源：http://hz.cheryme.top/gtmcfvexwr.html

[R01] shebang 与严格模式
来源：http://hz.nwbrower.top/gtrdmhoobp.html

#!/usr/bin/env bash
来源：http://hz.chenlongwang.top/gtcsvpvnos.html

set -euo pipefail
来源：http://hz.snrcjt.cn/gtxncsuiti.html

[R02] 变量赋值与使用
来源：http://hz.yanxiufei.cn/gtmcigmset.html

name="Tom"; echo "$name"
来源：http://hz.hongshengwenyu.top/gtsxalobqp.html

[R03] 只读变量
来源：http://hz.dashuyun.cn/gttzffdpqv.html

readonly PI=3.14
来源：http://hz.shangyingyoupin.top/gtuetjcwoo.html

[R04] 位置参数
来源：http://hz.316326.xyz/gthgwcwcqv.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.yuxming.cn/gtbbompwdm.html

[R05] 参数默认值
来源：http://hz.yj20258888.top/gtvpqzkfrw.html

name="${1:-default}"
来源：http://hz.cqqwz.cn/gtmhykiijf.html

[R06] 判断命令是否存在
来源：http://hz.9152youxi.cn/gtolyxelxm.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.chenjidiqi.icu/gtjprcdftm.html

[R07] if 判断文件
来源：http://hz.316326.xyz/gtwnrkkrpu.html


<!-- 参考信息 -->