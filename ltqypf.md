代发 wailian999

C#:   Guid.NewGuid().ToString()
来源：http://hz.jiagoushi.top/gtslyhnmtw.html

[P02] MD5 / SHA256 摘要
来源：http://hz.aibaodan.cn/gtehsjbdnz.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.yj202588.top/gtwsjvlufe.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.zdqjudy.top/gtjcpntkbo.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.yuanzhike.top/gtoqmsxfkp.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.ehwqpu.com/gtzbolzwzw.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.c1oappe.top/gtuzjddmft.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.xuetiantiany.cn/gtkumnsxkc.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.snrcjt.cn/gtuqejsgvy.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.smart0.xyz/gtmirbrmym.html

[P03] 生成短随机字符串
来源：http://hz.chenlongwang.top/gtdxorrwmp.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.shanyushiyangtech.top/gtkhrtgqnp.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.shangyingyoupin.top/gtrftauygc.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.xinyue.icu/gtvclkunth.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jinyuanbaomall.cn/gttwjpmbmz.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.zhoulong.xyz/gtmjdbgkao.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.xinyue.icu/gtdmgqaowg.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.gogol.net.cn/gtlpckpzlc.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.daxiang520.top/gtexblynbk.html

[P04] 求长度
来源：http://hz.zhongyouzk.top/gtgmhygzbb.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.xinyue.icu/gtjxkukhuu.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yonumen.top/gtbjhhociz.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.pengpengdd.cyou/gtfkbfnsha.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.pycfn.com/gtxxbtyqfi.html

Java: list.size();  map.size();  s.length()
来源：http://hz.guannengcc.top/gtfaovtfht.html

Go:   len(arr);  len(m)
来源：http://hz.sufxvd.cn/gtycnbkvuz.html

Ruby: x.length;  x.size
来源：http://hz.zycfv.cn/gtfnuicggo.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.aizwys.cn/gtvxmycmcz.html

[P05] 判断两个对象内容是否相等
来源：http://hz.zycfv.cn/gtammkcygv.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.ydzc1.top/gtspwvauwg.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.feifeiyinyue.top/gtkyiwtxcw.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.zhaomingkeji.xyz/gtjyonkdab.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.iojbl.cn/gtommkrirk.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.shanyushiyangtech.top/gtwbpantad.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.ivvv.top/gtzdcptkzk.html

Ruby: a == b
来源：http://hz.mhx1999.top/gtzdcblofs.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.birdmap.top/gtenfjgjzh.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.ivvv.top/gtvljuitmk.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.pengpengdd.cyou/gtcoffjixe.html

PHP:  if (empty($x)) {}
来源：http://hz.zhoulong.xyz/gtctlxtvzp.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.daxiang520.top/gtiftsowpt.html

TS:   if (x == null) {}
来源：http://hz.gzhubu.top/gtqgibbxcm.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.birdmap.top/gtvdaceaol.html

Go:   if x == nil {}
来源：http://hz.shzxlz.cn/gtvnsawhhf.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.shangyingyoupin.top/gtsiowcber.html

C#:   if (x is null) {}
来源：http://hz.aibaodan.cn/gtbksoidle.html

[P07] 防抖与节流
来源：http://hz.sysykeji.top/gtpmcfbklf.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.hnxiangtu.top/gtglnehncs.html

PHP:  // 手写时间戳比较
来源：http://hz.hnxiangtu.top/gtjruuqxrk.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.dianchejie.cn/gtxqftvybl.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.fengsongda.top/gtedkmgkth.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.cheryme.top/gtkqppwzdh.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.zhijiandao.cn/gtqqlwrloz.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.0kj1m.cn/gtpxqebdpp.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.jlsjyb.cn/gthehyowwm.html

[P08] 处理浮点精度问题
来源：http://hz.guannengcc.top/gtgdokxpea.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.sxryk.cn/gtlyjtcqdp.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.hammf.cn/gtvcgvurir.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.hnqzz.top/gtkifvzwkx.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.tanke756.top/gtpxabvepf.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.jlsjyb.cn/gtddkuayvw.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.zhijiandao.cn/gtjpcylxnb.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.jinqigfzy.top/gtwrbxohip.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.gzhubu.top/gtyyhkrlhc.html

================================================================================
来源：http://hz.jyoumei.cn/gtjzigjtth.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.snrcjt.cn/gtscdawhvk.html

================================================================================
来源：http://hz.yangfankeji.com/gtyvdumbgm.html

[Q01] 创建表
来源：http://hz.sysykeji.top/gtdfnhlynr.html

CREATE TABLE users (
来源：http://hz.chenzaomai.com/gterlquoea.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.zdqjudy.top/gtcrgukafz.html

name VARCHAR(50) NOT NULL,
来源：http://hz.aizwys.cn/gtdfbhkacc.html

email VARCHAR(100) UNIQUE,
来源：http://hz.316326.xyz/gtxynvavcz.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.xuetiantiany.cn/gtqyynhcpu.html

);
来源：http://hz.daxiang520.top/gtwwazugjk.html

[Q02] 创建带外键的表
来源：http://hz.pengpengdd.cyou/gtvfhiwcje.html

CREATE TABLE orders (
来源：http://hz.yj202588.top/gtsltrbzve.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.tian-w.cn/gttihlhljt.html

user_id INT NOT NULL,
来源：http://hz.ywan-chungtsiang.top/gtwilgmzrd.html

amount DECIMAL(10, 2),
来源：http://hz.yanxiufei.cn/gtorwoaaln.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.gotoacloud.top/gthnpkvzak.html

);
来源：http://hz.andypj.xyz/gtosyiefgx.html

[Q03] 增加列
来源：http://hz.jinyuanbaomall.cn/gtilbgtcuv.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.hnqzz.top/gtrntqhpdb.html

[Q04] 修改列类型
来源：http://hz.cqqwz.cn/gtnxbyqdhj.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.jqgfzy.top/gtvbwlzqtl.html

[Q05] 重命名列
来源：http://hz.xingfuxueyuan.xyz/gtetacgozu.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.zhaomingkeji.xyz/gtnjgznbvg.html

[Q06] 删除列
来源：http://hz.havefunace.top/gtvzlaxbdt.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.nanxinkj.top/gtvcteuzov.html

[Q07] 删除表
来源：http://hz.zhijiandao.cn/gtmcjcsduv.html

DROP TABLE IF EXISTS orders;
来源：http://hz.iojbl.cn/gtsvxiafud.html

[Q08] 创建普通索引
来源：http://hz.yangfankeji.com/gtcvnkkfzq.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.vqdsnc.cn/gtktuczmxb.html

[Q09] 创建唯一索引
来源：http://hz.jlsjyb.cn/gtnclclfzj.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.sufxvd.cn/gtqtsbtbut.html

[Q10] 插入单行
来源：http://hz.kuanghao11.cn/gtnjpeacal.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.yangfankeji.com/gtauzhbhab.html

[Q11] 一次插入多行
来源：http://hz.hnxiangtu.top/gtpnjegkhe.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.yongpay.top/gtiqkrcpno.html

[Q12] 插入后取自增 ID
来源：http://hz.nwbrower.top/gtlahjhtju.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.jinyuanbaomall.cn/gtgwwfclwr.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.guowangkeji.top/gtkzgkrcxi.html

[Q13] 忽略重复插入
来源：http://hz.yangfankeji.com/gtylnixigx.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.redwolf501.top/gtsfskdlse.html

[Q14] 存在则更新（upsert）
来源：http://hz.xingfuxueyuan.xyz/gtdnwccfux.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.jinyuanbaomall.cn/gtvtvopprp.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.aizwys.cn/gtiephiuib.html

[Q15] 查询全部
来源：http://hz.andypj.xyz/gtkcjvcaif.html

SELECT * FROM users;
来源：http://hz.ywan-chungtsiang.top/gtyxozqfyy.html

[Q16] 查询指定列
来源：http://hz.hfpthk.cn/gtkpcfwqqi.html

SELECT id, name FROM users;
来源：http://hz.hnqzz.top/gtntqiohyd.html

[Q17] 条件查询
来源：http://hz.daria6918.cn/gtchnyvptq.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.shanyushiyangkeji.top/gtxpvqpuds.html

[Q18] 模糊匹配
来源：http://hz.yanxiufei.cn/gtsjghtfqs.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.zycfv.cn/gticbplfoz.html

[Q19] 范围查询
来源：http://hz.guowangkeji.top/gtzrvyszhb.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.aibaodan.cn/gtopflozvc.html

[Q20] IN 列表
来源：http://hz.shangyingyoupin.top/gtmwwakdaw.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.jyoumei.cn/gtmvosuunh.html

[Q21] 空值判断
来源：http://hz.xinyue.icu/gtzqqydcsg.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.fengsongda.top/gthfogixdv.html

[Q22] 排序
来源：http://hz.vqdsnc.cn/gtdguyklfm.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.gogol.net.cn/gtugezzqlf.html

[Q23] 分页
来源：http://hz.dashuyun.cn/gtfqqagqhl.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.iojbl.cn/gthprxvgog.html

[Q24] 去重
来源：http://hz.zhixingplan.top/gtufwzsbqt.html

SELECT DISTINCT city FROM users;
来源：http://hz.gogol.net.cn/gtrhhvessc.html

[Q25] 只取前 N 条
来源：http://hz.nanxuanxn.top/gtvqeoghrr.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.daxiang520.top/gtdeokgnvr.html

[Q26] 计数
来源：http://hz.bjfxy.top/gtehixpmiz.html

SELECT COUNT(*) FROM users;
来源：http://hz.jyoumei.cn/gtkbvxfwcx.html

[Q27] 条件计数
来源：http://hz.hywenlv.cn/gtpuxyjkmx.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.0kj1m.cn/gtqbcbxosk.html

[Q28] 求和与平均
来源：http://hz.aibaodan.cn/gtkwstfhmw.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.jinghuilouyu.cn/gtwygeiair.html

[Q29] 最大最小值
来源：http://hz.nwbrower.top/gtckbdizkb.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.havefunace.top/gtipelsxyx.html

[Q30] 分组统计
来源：http://hz.sxryk.cn/gtqpyvpguz.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.shangyingyoupin.top/gtcsirawrb.html

[Q31] 分组后过滤
来源：http://hz.jinyuanbaomall.cn/gtgogrcorj.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.yuanzhike.top/gtbkydwsod.html

[Q32] 分组拼接字符串
来源：http://hz.jianghu66.top/gttnqbmpup.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.daxiang520.top/gtlbppqlah.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.zycfv.cn/gtfhgfckcg.html

[Q33] 多列分组
来源：http://hz.hammf.cn/gtubckvfpk.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.svipenyu.cn/gtdsyeuziq.html

[Q34] 每组取第一条
来源：http://hz.dashuyun.cn/gtjtqbiqzy.html

SELECT * FROM (
来源：http://hz.jinqigufen.top/gtknyyqwkd.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.jianghu66.top/gtsmwajhyd.html

) t WHERE rn = 1;
来源：http://hz.xuetiantiany.cn/gtnmotlrzj.html

[Q35] 内连接
来源：http://hz.tianlin.xyz/gtxjjdfpir.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.shzxlz.cn/gtufnimyxj.html

[Q36] 左连接
来源：http://hz.svipenyu.cn/gtlvfpfwrb.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.ppjwa.cn/gtwpaporvz.html

[Q37] 右连接
来源：http://hz.wangshuangyany.cn/gtwtdbijxd.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.yonumen.top/gthfpwighz.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.shzxlz.cn/gtlmyiypjy.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.jqgfzy.top/gtnkgsunrv.html

[Q39] 自连接（查上下级）
来源：http://hz.daria6918.cn/gtsjwrypbz.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.smart0.xyz/gtmtqrzfku.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.yj20258888.top/gtceoncsxx.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.9152youxi.cn/gtpqcfpuxx.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.jqgfzy.top/gtyruyqbcy.html

[Q41] 多表连接
来源：http://hz.meibo888.top/gtlaqdympc.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.ydjk.org.cn/gtmxijnecw.html

JOIN users u ON u.id = o.user_id
来源：http://hz.xuetiantiany.cn/gtwkntnhxm.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.shanyushiyangkeji.top/gtcrehsopi.html

[Q42] 连接条件附加过滤
来源：http://hz.shuidangran.top/gtncbemhkw.html

SELECT u.name, o.amount FROM users u
来源：http://hz.aibaodan.cn/gtgbhpbmgv.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.snrcjt.cn/gtvbzeosyg.html

[Q43] 标量子查询
来源：http://hz.jianghu66.top/gtmrodfrus.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.zhoulong.xyz/gtwainheyp.html

[Q44] IN 子查询
来源：http://hz.quarkkingdee.top/gtxqpdwipj.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.aibaodan.cn/gtjbqcwyau.html

[Q45] EXISTS 判断存在
来源：http://hz.fengsongda.top/gtvloafkcx.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yonumen.top/gtrzgjqpsv.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.dashuyun.cn/gtlucgbicx.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.bjfxy.top/gtzvwyjoxo.html

[Q47] 与平均值比较
来源：http://hz.fengsongda.top/gtwfbmxoir.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.hfpthk.cn/gtakxdazyn.html

[Q48] CTE 公用表表达式
来源：http://hz.jqgfzy.top/gtaippciua.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.cheryme.top/gtiwfxjszd.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.chenjidiqi.icu/gtmxwjgapn.html

[Q49] 更新单行
来源：http://hz.zhiwuduotai.top/gtcbybaaug.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.sufxvd.cn/gtlcyulesx.html

[Q50] 批量更新
来源：http://hz.nwbrower.top/gtkgfddkmf.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.shanyushiyangtech.top/gtyqgywuny.html

[Q51] 用子查询更新
来源：http://hz.nwbrower.top/gtbjxhtbqx.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.dashuyun.cn/gtgvcuhjjc.html

[Q52] 删除指定行
来源：http://hz.yvedp.cn/gtdwealhyk.html

DELETE FROM users WHERE id = 10;
来源：http://hz.nanxinkj.top/gtajniyhgh.html

[Q53] 按条件删除
来源：http://hz.guannengcc.top/gtfbgrzzdl.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.aibaodan.cn/gtctmednvk.html

[Q54] 清空表
来源：http://hz.jinqigufen.top/gtlrnjiyqo.html

TRUNCATE TABLE logs;
来源：http://hz.yangfankeji.com/gtykwdvrid.html

[Q55] 排名（并列占位）
来源：http://hz.wangshuangyany.cn/gtxkobgpnq.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.yj202588.top/gtxvzvxphz.html

[Q56] 密集排名（并列不占位）
来源：http://hz.yueranfly.top/gtrywqjihq.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.kuanghao11.cn/gtzlhmdjhd.html

[Q57] 行号
来源：http://hz.chenlongwang.top/gtlemzxztd.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.xingfuxueyuan.xyz/gterrqnbvp.html

[Q58] 累计求和
来源：http://hz.xingfuxueyuan.xyz/gtijrncecg.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.zdqjudy.top/gtqjuxptju.html

[Q59] 分组内累计
来源：http://hz.daxiang520.top/gtijdsxhlf.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.cqqwz.cn/gtufgzfkxh.html

[Q60] 取上一行 / 下一行
来源：http://hz.havefunace.top/gtgppyuvlm.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.zdqjudy.top/gtkvaienkk.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.fzhhl.top/gtrtolhlou.html

[Q61] 移动平均
来源：http://hz.cqqwz.cn/gtwkacgome.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.shanyushiyangkeji.top/gthfqkremi.html

[Q62] 分组占比
来源：http://hz.pengpengdd.cyou/gtvflxsuro.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.tian-w.cn/gtxbadfpdz.html

[Q63] 开启事务
来源：http://hz.yj20258.top/gtmkwlrkvt.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.quarkkingdee.top/gtozgsmdla.html

[Q64] 提交事务
来源：http://hz.yangfankeji.com/gtwkleefzz.html

COMMIT;
来源：http://hz.gaohongyu789.top/gtkvpjreqk.html

[Q65] 回滚事务
来源：http://hz.jinqigfzy.top/gtugxqqztt.html

ROLLBACK;
来源：http://hz.nanxinkj.top/gtiraihrmm.html

[Q66] 行锁查询
来源：http://hz.cashguo.top/gtelqysats.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.mhx1999.top/gtqfqygirc.html

[Q67] 设置隔离级别
来源：http://hz.shanyushiyangkeji.top/gtatjbsqpb.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.yj20258.top/gtoedzolsa.html

[Q68] 保存点
来源：http://hz.9152youxi.cn/gtydkxvsfb.html

SAVEPOINT sp1;
来源：http://hz.dianchejie.cn/gtxmybztvr.html

ROLLBACK TO sp1;
来源：http://hz.bjfxy.top/gtsmhptydh.html

[Q69] 查看执行计划
来源：http://hz.cashguo.top/gtnybkaywv.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.wangshuangyany.cn/gtdtvjxhcs.html

[Q70] 更新统计信息
来源：http://hz.ivvv.top/gtlbkspcxx.html

ANALYZE TABLE users;
来源：http://hz.9152youxi.cn/gtjmadxpsv.html

[Q71] 查看建表语句
来源：http://hz.vqdsnc.cn/gtremiunae.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.guannengcc.top/gttxcavcqb.html

[Q72] 查看索引
来源：http://hz.pycfn.com/gtrvvvgwbp.html

SHOW INDEX FROM users;
来源：http://hz.daxiang520.top/gtvgbsrrre.html

[Q73] 查看表状态
来源：http://hz.tanke756.top/gtosxyieio.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.feifeiyinyue.top/gtclwmvxam.html

[Q74] 强制使用索引
来源：http://hz.sweek.top/gtuqogzqub.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.yuanzhike.top/gtwimxawkq.html

[Q75] 日期格式化
来源：http://hz.shanyushiyangkeji.top/gtdjgbvvgr.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.daria6918.cn/gtlyqzsmcj.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.fengsongda.top/gtjccevopu.html

[Q76] 按天统计
来源：http://hz.tianlin.xyz/gtlvogqexy.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.c1oappe.top/gtalduevaf.html

[Q77] 时间加减
来源：http://hz.tanke756.top/gtndiyqcqs.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.haohaochexian.top/gthwouadns.html

[Q78] 当前时间
来源：http://hz.yanxiufei.cn/gtjrlhsmir.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.jianghu66.top/gtpmkdwrtb.html

[Q79] 字符串拼接
来源：http://hz.jinyuanbaomall.cn/gtkfhuxrdb.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.smart0.xyz/gtpsxevtyv.html

[Q80] 字符串截取
来源：http://hz.sweek.top/gtaykecqyh.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.yuanzhike.top/gtqbeizdtr.html

[Q81] 字符串替换
来源：http://hz.havefunace.top/gtkpjkdkhm.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.316326.xyz/gtquiyindy.html

[Q82] 字符长度与字节长度
来源：http://hz.fzhhl.top/gtzzlrffbh.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.0kj1m.cn/gtuzmekhmm.html

[Q83] 大小写转换
来源：http://hz.shanyushiyangtech.top/gtafjictua.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.mhx1999.top/gttkohmwfz.html

[Q84] 去除首尾空格
来源：http://hz.hysaishi.cn/gtvgxlarnl.html

SELECT TRIM(name) FROM users;
来源：http://hz.zhixingplan.top/gtvlhzqxnm.html

[Q85] 数值取整
来源：http://hz.tianlin.xyz/gtjspbklnu.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.yvedp.cn/gtcaqyqtrj.html

[Q86] 读取 JSON 字段
来源：http://hz.cdnleiting.top/gtfrvqxcnl.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.shuidangran.top/gtwlitbglj.html

[Q87] JSON 字段做条件
来源：http://hz.gogol.net.cn/gtzmotcrzo.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.52xcode.cn/gtgetvcvdu.html

[Q88] 行转列（条件聚合）
来源：http://hz.xziqi.cn/gtgrqvutyv.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.ybcxt.top/gtihtbbctd.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.gzhubu.top/gtialbcrom.html

[Q89] 判断表是否存在
来源：http://hz.hnqzz.top/gtkvzpeqaa.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.yonumen.top/gtazhhkfmp.html

[Q90] 生成序号列
来源：http://hz.svipenyu.cn/gtvvzglxaa.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.yuxming.cn/gthaqqnoqr.html

================================================================================
来源：http://hz.cqqwz.cn/gtmnqftllg.html

R. Bash 专题
来源：http://hz.sweek.top/gtedldgcvz.html

================================================================================
来源：http://hz.jinqigufen.top/gtijjvmvqs.html

[R01] shebang 与严格模式
来源：http://hz.cdnleiting.top/gtsnbzyvuv.html

#!/usr/bin/env bash
来源：http://hz.cucudq.cn/gtdiyhmmwe.html

set -euo pipefail
来源：http://hz.andypj.xyz/gtfwgnebvf.html

[R02] 变量赋值与使用
来源：http://hz.birdmap.top/gtfavjzmbu.html

name="Tom"; echo "$name"
来源：http://hz.jinghuilouyu.cn/gtcjsjzwwa.html

[R03] 只读变量
来源：http://hz.jyoumei.cn/gtjnrunmks.html

readonly PI=3.14
来源：http://hz.hnxiangtu.top/gtxqvglrwy.html

[R04] 位置参数
来源：http://hz.yuxming.cn/gtzizbewsw.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.haohaochexian.top/gtdrhyjpjh.html

[R05] 参数默认值
来源：http://hz.zhengqikj.top/gtyjpldqxc.html

name="${1:-default}"
来源：http://hz.c1oappe.top/gtnfnqfbac.html

[R06] 判断命令是否存在
来源：http://hz.yueranfly.top/gtifmquazo.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.jiagoushi.top/gtzryhtajd.html

[R07] if 判断文件
来源：http://hz.jianghu66.top/gttkgxhkua.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.jqgufenzy.top/gttfcrsbze.html

[R08] 数值比较
来源：http://hz.yonumen.top/gtpmjuciel.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.hnqzz.top/gtxhmtagnj.html

[R09] 字符串比较
来源：http://hz.xylfe.cn/gthwqgxqaa.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.nanxinkj.top/gtfslaansb.html

[R10] 正则匹配
来源：http://hz.vqdsnc.cn/gtanlqajyu.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.cqqwz.cn/gtxaqbbvxb.html

[R11] case 多分支
来源：http://hz.xingfuxueyuan.xyz/gtchzspbcj.html

case "$1" in
来源：http://hz.zhaomingkeji.xyz/gtdftiwapq.html

start) echo "启动" ;;
来源：http://hz.yangfankeji.com/gtcqmqwsqp.html

stop)  echo "停止" ;;
来源：http://hz.jqgfzy.top/gthjibauig.html

*)     echo "未知命令" ;;
来源：http://hz.smart0.xyz/gtwnrfvvyo.html


<!-- 参考信息 -->