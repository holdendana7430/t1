代发 wailian999

C#:   Parallel.For
来源：http://hz.havefunace.top/gtvwuyhebm.html

================================================================================
来源：http://hz.cucudq.cn/gtfahheuou.html

P. 常用工具函数
来源：http://hz.zhengqikj.top/gtxdabxycu.html

================================================================================
来源：http://hz.52xcode.cn/gtfziiydgy.html

[P01] 生成 UUID
来源：http://hz.ybcxt.top/gttgupndqs.html

Py:   str(uuid.uuid4())
来源：http://hz.yongpay.top/gtukkrcppy.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.cdnleiting.top/gtsptffmmm.html

JS:   crypto.randomUUID()
来源：http://hz.daxiang520.top/gtgoeenxgv.html

TS:   crypto.randomUUID()
来源：http://hz.ybcxt.top/gtqhufibnv.html

Java: UUID.randomUUID().toString()
来源：http://hz.jinyuanbaomall.cn/gtbooclyia.html

Go:   // 用 github.com/google/uuid
来源：http://hz.tanke756.top/gtnvzkkotg.html

Ruby: SecureRandom.uuid
来源：http://hz.mhx1999.top/gtqxcptzoi.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.kuanghao11.cn/gtacwvnnkb.html

[P02] MD5 / SHA256 摘要
来源：http://hz.ehwqpu.com/gtllxecxou.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.xinyue.icu/gtlnupemmy.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.shuidangran.top/gtvrpnymly.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.jqgufenzy.top/gthezfxfab.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.zdqjudy.top/gtiqepkvck.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.ydzc1.top/gtqbwyqrnz.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.jiagoushi.top/gtghjfiujg.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.meibo888.top/gtpaetphuz.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.zhongyouzk.top/gthzjgjnwh.html

[P03] 生成短随机字符串
来源：http://hz.daria6918.cn/gtlvhqgfcr.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.jiagoushi.top/gtbjkevzlw.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.yongpay.top/gtkcjxxzbu.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.nanxuanxn.top/gtqfoqsfyg.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.birdmap.top/gtluidgphz.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.wangdashe.top/gtzshnmlap.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.zhaomingkeji.xyz/gtpevrdqpx.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.chenjidiqi.icu/gtnyfdzklp.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.meibo888.top/gtdygryzme.html

[P04] 求长度
来源：http://hz.yongpay.top/gtmbvuzivm.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.guannengcc.top/gtwvjivxem.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.ydjk.org.cn/gtctbvabip.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.ydjk.org.cn/gtlmfnyiuc.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.xingfuxueyuan.xyz/gtewashzqw.html

Java: list.size();  map.size();  s.length()
来源：http://hz.cucudq.cn/gtyseqvxzj.html

Go:   len(arr);  len(m)
来源：http://hz.yvedp.cn/gtiiechoyz.html

Ruby: x.length;  x.size
来源：http://hz.guowangkeji.top/gtiqikkcxh.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.xuetiantiany.cn/gtvjxxbafo.html

[P05] 判断两个对象内容是否相等
来源：http://hz.ydzc1.top/gtbiptjrmc.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.wangdashe.top/gtobwravkc.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.sweek.top/gtfgkouecy.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.jlsjyb.cn/gtjvzymgtu.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.0kj1m.cn/gtaacqyser.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.yanxiufei.cn/gtxljnulxc.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.tian-w.cn/gtcncpmmxp.html

Ruby: a == b
来源：http://hz.yangfankeji.com/gteyuonriw.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.yangfankeji.com/gtxmymnono.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.sxryk.cn/gtykbrhhqt.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.ydjk.org.cn/gtctiomoce.html

PHP:  if (empty($x)) {}
来源：http://hz.cucudq.cn/gtrzpzisee.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.svipenyu.cn/gtzqnipjjb.html

TS:   if (x == null) {}
来源：http://hz.nanxuanxn.top/gthwbfhzbo.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.tanke756.top/gtbzafnpyn.html

Go:   if x == nil {}
来源：http://hz.jinqigufen.top/gtxldyysip.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.aizwys.cn/gtaaclbvdm.html

C#:   if (x is null) {}
来源：http://hz.gogol.net.cn/gtycefrsog.html

[P07] 防抖与节流
来源：http://hz.xingfuxueyuan.xyz/gtsruqfpcy.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.vqdsnc.cn/gtzhckqcqc.html

PHP:  // 手写时间戳比较
来源：http://hz.gzhubu.top/gtmwsbumef.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.shangyingyoupin.top/gtygmxxltz.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jinyuanbaomall.cn/gtxdartvji.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.pengpengdd.cyou/gtwaknsmel.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.cdnleiting.top/gtzjlogrqa.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.52xcode.cn/gtiyzspugv.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.tian-w.cn/gtnyyzvwhj.html

[P08] 处理浮点精度问题
来源：http://hz.yongpay.top/gtpvlundol.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.chenlongwang.top/gtlpuunkur.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.c1oappe.top/gtjomafheh.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.yuxming.cn/gtpbjlctle.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.nanxuanxn.top/gthxzcrqle.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.bjfxy.top/gtyjupsooy.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.shuidangran.top/gtobuytfnw.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.jiagoushi.top/gtlwxswdff.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.gzhubu.top/gtfptwvahu.html

================================================================================
来源：http://hz.zdqjudy.top/gttnzrabkf.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.vqdsnc.cn/gthhwjdbml.html

================================================================================
来源：http://hz.chenlongwang.top/gtsxpidzlu.html

[Q01] 创建表
来源：http://hz.yj202588.top/gtomzzmslj.html

CREATE TABLE users (
来源：http://hz.pengpengdd.cyou/gtnoythsfj.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.zhengqikj.top/gtxcumvpto.html

name VARCHAR(50) NOT NULL,
来源：http://hz.zycfv.cn/gtsmicytin.html

email VARCHAR(100) UNIQUE,
来源：http://hz.zdqjudy.top/gtehfemoqp.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.jqgfzy.top/gtketftdhj.html

);
来源：http://hz.shzxlz.cn/gtayupoyrk.html

[Q02] 创建带外键的表
来源：http://hz.jinqigfzy.top/gtuqzolkuu.html

CREATE TABLE orders (
来源：http://hz.dianchejie.cn/gtkkqeitbz.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.xylfe.cn/gtosgoixtu.html

user_id INT NOT NULL,
来源：http://hz.dashuyun.cn/gtvftgzdxk.html

amount DECIMAL(10, 2),
来源：http://hz.nwbrower.top/gtcxpvyzgv.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.kuanghao11.cn/gtjkmpyymq.html

);
来源：http://hz.meibo888.top/gtvrqnhqrl.html

[Q03] 增加列
来源：http://hz.ybcxt.top/gtcewmrikw.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.tanke756.top/gtutgplcff.html

[Q04] 修改列类型
来源：http://hz.chenjidiqi.icu/gtroxhepxu.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.shzxlz.cn/gtmlzkglrv.html

[Q05] 重命名列
来源：http://hz.bjfxy.top/gtbbzjiuuy.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.jqgufenzy.top/gtvooutxrb.html

[Q06] 删除列
来源：http://hz.gzhubu.top/gtnifgrncf.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.cqqwz.cn/gtevsqmgxv.html

[Q07] 删除表
来源：http://hz.ydjk.org.cn/gtvzmqwvkq.html

DROP TABLE IF EXISTS orders;
来源：http://hz.dianchejie.cn/gtctxkfxnq.html

[Q08] 创建普通索引
来源：http://hz.0kj1m.cn/gtrfzybsbc.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.daria6918.cn/gtomepakzx.html

[Q09] 创建唯一索引
来源：http://hz.nanxuanxn.top/gtsfvjtsuo.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.ydjk.org.cn/gtuydbwgro.html

[Q10] 插入单行
来源：http://hz.daria6918.cn/gtczzbfxib.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.tianlin.xyz/gtxjiibgic.html

[Q11] 一次插入多行
来源：http://hz.gaohongyu789.top/gtnlyjfbac.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.52xcode.cn/gtgxuctpgf.html

[Q12] 插入后取自增 ID
来源：http://hz.ybcxt.top/gtuxzbqdqq.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.xinyue.icu/gtuiyyorkd.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.meibo888.top/gtpvqgwuqv.html

[Q13] 忽略重复插入
来源：http://hz.quarkkingdee.top/gtlxdwwllg.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.zhengqikj.top/gtogxwiurq.html

[Q14] 存在则更新（upsert）
来源：http://hz.9152youxi.cn/gtsitndrqn.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.zdqjudy.top/gtzfqjehji.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.zhengqikj.top/gttbidppjf.html

[Q15] 查询全部
来源：http://hz.yonumen.top/gtgxwxzckf.html

SELECT * FROM users;
来源：http://hz.jinqigufen.top/gtpqxhoxbv.html

[Q16] 查询指定列
来源：http://hz.zhaomingkeji.xyz/gtougydabq.html

SELECT id, name FROM users;
来源：http://hz.gaohongyu789.top/gtxxfrvsbd.html

[Q17] 条件查询
来源：http://hz.jqgufenzy.top/gtptvrvbpn.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.yonumen.top/gtrqbhswwv.html

[Q18] 模糊匹配
来源：http://hz.jinyuanbaomall.cn/gtjkvmncjt.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.havefunace.top/gtdyvpvneg.html

[Q19] 范围查询
来源：http://hz.jinqigufen.top/gtevixlpeo.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.chenzaomai.com/gtngurltcw.html

[Q20] IN 列表
来源：http://hz.ywan-chungtsiang.top/gtzksqtwry.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.cashguo.top/gtcqooqtox.html

[Q21] 空值判断
来源：http://hz.9152youxi.cn/gtpxbcptzu.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.daria6918.cn/gtcxhjyjoe.html

[Q22] 排序
来源：http://hz.jyoumei.cn/gtoxbzrnjd.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.ivvv.top/gtptapxupg.html

[Q23] 分页
来源：http://hz.aibaodan.cn/gtdtbavasf.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.shuidangran.top/gtbteelkrj.html

[Q24] 去重
来源：http://hz.hnxiangtu.top/gtyjkjkomi.html

SELECT DISTINCT city FROM users;
来源：http://hz.316326.xyz/gtzeeqtybn.html

[Q25] 只取前 N 条
来源：http://hz.pycfn.com/gtpzqulpqn.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.ivvv.top/gtxokqqsha.html

[Q26] 计数
来源：http://hz.guannengcc.top/gtppqesomt.html

SELECT COUNT(*) FROM users;
来源：http://hz.zhixingplan.top/gtevvviymg.html

[Q27] 条件计数
来源：http://hz.yueranfly.top/gtcwfhpetf.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.shangyingyoupin.top/gtyoexnkdt.html

[Q28] 求和与平均
来源：http://hz.xuanzx.com/gtnvlatxne.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.mhx1999.top/gtcocasspb.html

[Q29] 最大最小值
来源：http://hz.dianchejie.cn/gtcvfswgvp.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.jianghu66.top/gtzzxpxcli.html

[Q30] 分组统计
来源：http://hz.hnqzz.top/gtvjnkgydg.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.mhx1999.top/gtrfqrcydc.html

[Q31] 分组后过滤
来源：http://hz.yj20258.top/gtxkvnuvul.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.zhengqikj.top/gtimbvphef.html

[Q32] 分组拼接字符串
来源：http://hz.nanxinkj.top/gtqgaaktnb.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.yj202588.top/gtuqxwsbvv.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.chenzaomai.com/gtwfkmikdp.html

[Q33] 多列分组
来源：http://hz.aizwys.cn/gtmmjrhiik.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.hnxiangtu.top/gtxblaohpw.html

[Q34] 每组取第一条
来源：http://hz.zhoulong.xyz/gtdjokgytp.html

SELECT * FROM (
来源：http://hz.yuxming.cn/gtvqoazqdm.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.sysykeji.top/gtcmjzqqsw.html

) t WHERE rn = 1;
来源：http://hz.zhijiandao.cn/gtuohotdni.html

[Q35] 内连接
来源：http://hz.nanxinkj.top/gttnnvdjmm.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.zdqjudy.top/gteaoilvxb.html

[Q36] 左连接
来源：http://hz.aibaodan.cn/gtixhrjmzg.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.tian-w.cn/gtdgrynnre.html

[Q37] 右连接
来源：http://hz.zhiwuduotai.top/gtwipphpyh.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.pycfn.com/gtgkyvifif.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.pengpengdd.cyou/gtuvqlznjq.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.svipenyu.cn/gtvnzuzozc.html

[Q39] 自连接（查上下级）
来源：http://hz.daria6918.cn/gtygjvfarm.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.hnqzz.top/gtgmwjmtip.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.wangdashe.top/gttdhqmrsa.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.cheryme.top/gtawbrmuul.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.zhoulong.xyz/gtugvovmyd.html

[Q41] 多表连接
来源：http://hz.ybcxt.top/gthnpecgts.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.jqgufenzy.top/gtzgxqofpt.html

JOIN users u ON u.id = o.user_id
来源：http://hz.pycfn.com/gtntumegmp.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.shzxlz.cn/gtolejlbof.html

[Q42] 连接条件附加过滤
来源：http://hz.xingfuxueyuan.xyz/gtjqkseugc.html

SELECT u.name, o.amount FROM users u
来源：http://hz.chenlongwang.top/gtngsexczg.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.ppjwa.cn/gtwnmhjmnf.html

[Q43] 标量子查询
来源：http://hz.redwolf501.top/gtzsvyzzzh.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.xingfuxueyuan.xyz/gtuocnnmdf.html

[Q44] IN 子查询
来源：http://hz.quarkkingdee.top/gtctydvlkb.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.sxryk.cn/gtjpclafvc.html

[Q45] EXISTS 判断存在
来源：http://hz.jyoumei.cn/gtndvyrxys.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.fzhhl.top/gtrduhvzkf.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.ydzc1.top/gtxigbzkni.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.vqdsnc.cn/gtycewdfkf.html

[Q47] 与平均值比较
来源：http://hz.xylfe.cn/gtnwxxlpct.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.zhiwuduotai.top/gtgdbnuqdc.html

[Q48] CTE 公用表表达式
来源：http://hz.daxiang520.top/gtwfsrqluf.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.316326.xyz/gtydfsrgcw.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.havefunace.top/gtasmveavi.html

[Q49] 更新单行
来源：http://hz.yj20258888.top/gtasepiykd.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.daxiang520.top/gtbppfgvse.html

[Q50] 批量更新
来源：http://hz.ydjk.org.cn/gtdzlbsnsg.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.tianlin.xyz/gtzlwltvyr.html

[Q51] 用子查询更新
来源：http://hz.ydjk.org.cn/gtbyziibij.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.c1oappe.top/gttlwknjqp.html

[Q52] 删除指定行
来源：http://hz.yueranfly.top/gtfpavoxkq.html

DELETE FROM users WHERE id = 10;
来源：http://hz.svipenyu.cn/gtepfecqri.html

[Q53] 按条件删除
来源：http://hz.yuxming.cn/gtbnxjocvz.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.52xcode.cn/gtkgmnjwgw.html

[Q54] 清空表
来源：http://hz.c1oappe.top/gtmqcbtxso.html

TRUNCATE TABLE logs;
来源：http://hz.feifeiyinyue.top/gtfcizuunx.html

[Q55] 排名（并列占位）
来源：http://hz.hnxiangtu.top/gtorprrlau.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.pycfn.com/gtrohrzbbt.html

[Q56] 密集排名（并列不占位）
来源：http://hz.svipenyu.cn/gtgdyztbzh.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.iojbl.cn/gtnbzwheyh.html

[Q57] 行号
来源：http://hz.jinqigufen.top/gtauxztuod.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.hammf.cn/gtoflihwfy.html

[Q58] 累计求和
来源：http://hz.ydjk.org.cn/gtddtwcifr.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.ydzc1.top/gtxiypjoky.html

[Q59] 分组内累计
来源：http://hz.vqdsnc.cn/gtigophbqn.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.pengpengdd.cyou/gtgjtewczn.html

[Q60] 取上一行 / 下一行
来源：http://hz.ywan-chungtsiang.top/gtjyyffmnm.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.cqqwz.cn/gtemfuuskj.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.pycfn.com/gteqoutpdk.html

[Q61] 移动平均
来源：http://hz.zhaomingkeji.xyz/gtnirtnjej.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.zhaomingkeji.xyz/gttivyjywy.html

[Q62] 分组占比
来源：http://hz.guannengcc.top/gtwohyajno.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.shanyushiyangkeji.top/gtuuuutacy.html

[Q63] 开启事务
来源：http://hz.hfpthk.cn/gthxcgyaaf.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.yuxming.cn/gthmosigqj.html

[Q64] 提交事务
来源：http://hz.ybcxt.top/gtmgybgdyc.html

COMMIT;
来源：http://hz.yanxiufei.cn/gthpttefnf.html

[Q65] 回滚事务
来源：http://hz.cucudq.cn/gtbrhqsiyp.html

ROLLBACK;
来源：http://hz.nwbrower.top/gtsgwphnbh.html

[Q66] 行锁查询
来源：http://hz.nanxuanxn.top/gtmrpoxufh.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.guowangkeji.top/gttxjrrxly.html

[Q67] 设置隔离级别
来源：http://hz.zhijiandao.cn/gtlckdyyts.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.shangyingyoupin.top/gtgzldcilq.html

[Q68] 保存点
来源：http://hz.cdnleiting.top/gtnxvcfgwj.html

SAVEPOINT sp1;
来源：http://hz.hywenlv.cn/gtbqcddtuu.html

ROLLBACK TO sp1;
来源：http://hz.aibaodan.cn/gtjynfiyna.html

[Q69] 查看执行计划
来源：http://hz.yangfankeji.com/gtjxpauxwa.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.52xcode.cn/gtiodcytrq.html

[Q70] 更新统计信息
来源：http://hz.mhx1999.top/gtxugmqtbg.html

ANALYZE TABLE users;
来源：http://hz.zhengqikj.top/gtslcylwxk.html

[Q71] 查看建表语句
来源：http://hz.pycfn.com/gtbmuzblmp.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.hammf.cn/gtvhizwpmh.html

[Q72] 查看索引
来源：http://hz.yonumen.top/gtvvsvwzrw.html

SHOW INDEX FROM users;
来源：http://hz.fzhhl.top/gtnynkfisu.html

[Q73] 查看表状态
来源：http://hz.cucudq.cn/gtptoubjeh.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.sysykeji.top/gtuefarhod.html

[Q74] 强制使用索引
来源：http://hz.meibo888.top/gtfgsnofee.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.jianghu66.top/gtvnrjezwi.html

[Q75] 日期格式化
来源：http://hz.chenlongwang.top/gtdeeumntv.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.aibaodan.cn/gtajgprqhr.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.hongshengwenyu.top/gtbtbmhwrb.html

[Q76] 按天统计
来源：http://hz.aizwys.cn/gtgutgcjom.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.dashuyun.cn/gtwzfwxxrf.html

[Q77] 时间加减
来源：http://hz.nanxuanxn.top/gtddzdamib.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.yangfankeji.com/gtutvsllto.html

[Q78] 当前时间
来源：http://hz.nanxuanxn.top/gtpzyrjyyt.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.svipenyu.cn/gtwknbjiru.html

[Q79] 字符串拼接
来源：http://hz.cqqwz.cn/gtswtxmvnt.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.jinghuilouyu.cn/gthyyhvzmd.html

[Q80] 字符串截取
来源：http://hz.zycfv.cn/gtfpbmxtbd.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.snrcjt.cn/gtuiuwgmft.html

[Q81] 字符串替换
来源：http://hz.gzhubu.top/gtuwodqdhr.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.haohaochexian.top/gtpluzccrd.html

[Q82] 字符长度与字节长度
来源：http://hz.dashuyun.cn/gtddcgnaid.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.ivvv.top/gtknkhbflr.html

[Q83] 大小写转换
来源：http://hz.ehwqpu.com/gtccuebark.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.andypj.xyz/gtzrekvxhn.html

[Q84] 去除首尾空格
来源：http://hz.chenzaomai.com/gtxvxjeoxl.html

SELECT TRIM(name) FROM users;
来源：http://hz.ywan-chungtsiang.top/gtgoollhgh.html

[Q85] 数值取整
来源：http://hz.guannengcc.top/gtmmzhyxpt.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.aibaodan.cn/gtzefjufde.html

[Q86] 读取 JSON 字段
来源：http://hz.guannengcc.top/gtusagpivp.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.daria6918.cn/gttjujloss.html

[Q87] JSON 字段做条件
来源：http://hz.hfpthk.cn/gtyaxamlhl.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.gogol.net.cn/gtcgxfgmtb.html

[Q88] 行转列（条件聚合）
来源：http://hz.ywan-chungtsiang.top/gtauiirwhz.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.meibo888.top/gtfpeeuojk.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.yj20258.top/gtnhpkweyu.html

[Q89] 判断表是否存在
来源：http://hz.shangyingyoupin.top/gttjaauoqf.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.ybcxt.top/gttzyakjyp.html

[Q90] 生成序号列
来源：http://hz.shzxlz.cn/gtgdgovfyg.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.zhijiandao.cn/gtjzrqcchm.html

================================================================================
来源：http://hz.chenlongwang.top/gttvamhnos.html

R. Bash 专题
来源：http://hz.jinyuanbaomall.cn/gtjjgfmmka.html

================================================================================
来源：http://hz.jlsjyb.cn/gtxzgduxwx.html

[R01] shebang 与严格模式
来源：http://hz.xylfe.cn/gtnindlbmr.html

#!/usr/bin/env bash
来源：http://hz.cdnleiting.top/gtdnwdxass.html

set -euo pipefail
来源：http://hz.andypj.xyz/gtlybgsrse.html

[R02] 变量赋值与使用
来源：http://hz.sweek.top/gtmuzpxbaa.html

name="Tom"; echo "$name"
来源：http://hz.kuanghao11.cn/gtzjslpjfi.html

[R03] 只读变量
来源：http://hz.yj20258888.top/gtiurxmxdt.html

readonly PI=3.14
来源：http://hz.yj20258.top/gtbmmkgemh.html

[R04] 位置参数
来源：http://hz.smart0.xyz/gtdbbpoixg.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.wangdashe.top/gtcrphoect.html

[R05] 参数默认值
来源：http://hz.yj202588.top/gtuqzbdkfo.html

name="${1:-default}"
来源：http://hz.tian-w.cn/gtnrvlddhk.html

[R06] 判断命令是否存在
来源：http://hz.ehwqpu.com/gtuywsnmmd.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.shangyingyoupin.top/gttdoxbbhj.html

[R07] if 判断文件
来源：http://hz.gogol.net.cn/gtrlbynygg.html


<!-- 参考信息 -->