代发 wailian999

TS:   // child_process / cluster 模块
来源：http://hz.jinqigfzy.top/gtplibkzxh.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.ivvv.top/gtkczbfojb.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.hywenlv.cn/gtykkbxvcc.html

Ruby: // fork 块
来源：http://hz.sxryk.cn/gtknjikiny.html

C#:   Parallel.For
来源：http://hz.cheryme.top/gtxpnmzygx.html

================================================================================
来源：http://hz.svipenyu.cn/gtdvlfflnf.html

P. 常用工具函数
来源：http://hz.yanxiufei.cn/gtqtinhxee.html

================================================================================
来源：http://hz.dianchejie.cn/gtbfbkwsfa.html

[P01] 生成 UUID
来源：http://hz.xuetiantiany.cn/gtdmpvnvjm.html

Py:   str(uuid.uuid4())
来源：http://hz.0kj1m.cn/gtpvarwitk.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.nanxinkj.top/gtmefivsin.html

JS:   crypto.randomUUID()
来源：http://hz.sufxvd.cn/gtfxguskfm.html

TS:   crypto.randomUUID()
来源：http://hz.vqdsnc.cn/gtjitgpqsx.html

Java: UUID.randomUUID().toString()
来源：http://hz.tianlin.xyz/gtyclvnrts.html

Go:   // 用 github.com/google/uuid
来源：http://hz.sufxvd.cn/gtwroumibl.html

Ruby: SecureRandom.uuid
来源：http://hz.yvedp.cn/gtclsixoik.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.xylfe.cn/gthjqhpjrw.html

[P02] MD5 / SHA256 摘要
来源：http://hz.haohaochexian.top/gtqphbdhkv.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.andypj.xyz/gtamtugjup.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.wangdashe.top/gtivjyegqg.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.chenjidiqi.icu/gtrdnxzojn.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.ehwqpu.com/gtebttjezt.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.guowangkeji.top/gtabmtzfzo.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.tanke756.top/gtodmhusnc.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.hfpthk.cn/gtsujdotfy.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.feifeiyinyue.top/gtzbcuibha.html

[P03] 生成短随机字符串
来源：http://hz.tian-w.cn/gtibmfsbrs.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.hfpthk.cn/gtdaoichtf.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.tian-w.cn/gtjqhvjntz.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.zhoulong.xyz/gtihmsctjn.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.quarkkingdee.top/gtyatgebpb.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.tanke756.top/gtldqbgaqa.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.yongpay.top/gtkdghklfe.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.zhiwuduotai.top/gtakzjkvnj.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.zhiwuduotai.top/gtzgfxqlim.html

[P04] 求长度
来源：http://hz.pengpengdd.cyou/gthohwejxc.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.ybcxt.top/gtiqzwqque.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.havefunace.top/gtunnboirv.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.gzhubu.top/gtjzrymfqr.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.9152youxi.cn/gtqfbyafxq.html

Java: list.size();  map.size();  s.length()
来源：http://hz.guannengcc.top/gtwmdmdosa.html

Go:   len(arr);  len(m)
来源：http://hz.wangdashe.top/gtsuuqqjma.html

Ruby: x.length;  x.size
来源：http://hz.yj20258.top/gtfssuemtz.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.zhiwuduotai.top/gtznduyujy.html

[P05] 判断两个对象内容是否相等
来源：http://hz.jyoumei.cn/gtbxzyplxf.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.hysaishi.cn/gtduitukcf.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.chenlongwang.top/gtesdzswtn.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.pycfn.com/gtnzzwatun.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.zdqjudy.top/gtnguvpoud.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.yonumen.top/gttopcioxh.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.zhijiandao.cn/gtvjcafixu.html

Ruby: a == b
来源：http://hz.jiagoushi.top/gtsjlbnfzr.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.jqgfzy.top/gtevvdugxu.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.jiagoushi.top/gtuiosgjfr.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.guannengcc.top/gtxdvpagfs.html

PHP:  if (empty($x)) {}
来源：http://hz.yj20258.top/gtuhdgeoqr.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.bjfxy.top/gtllnepgih.html

TS:   if (x == null) {}
来源：http://hz.jinghuilouyu.cn/gthzdubtwr.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.shangyingyoupin.top/gtakyvyrxo.html

Go:   if x == nil {}
来源：http://hz.guowangkeji.top/gtxypqwfxd.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.fzhhl.top/gtaiyjktpg.html

C#:   if (x is null) {}
来源：http://hz.ppjwa.cn/gtyefyrcuw.html

[P07] 防抖与节流
来源：http://hz.gotoacloud.top/gtzphnhhmc.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.sysykeji.top/gtxxcnemur.html

PHP:  // 手写时间戳比较
来源：http://hz.yongpay.top/gtyjdsbaof.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.redwolf501.top/gtmxgxwbje.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yonumen.top/gtzzsxpfsq.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.sxryk.cn/gtmwpvewle.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.nwbrower.top/gtsxncrjtb.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.zhiwuduotai.top/gtrpyllaap.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.ivvv.top/gttdxsyhdb.html

[P08] 处理浮点精度问题
来源：http://hz.daxiang520.top/gtnwdsyylo.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.yanxiufei.cn/gthwhyqwjt.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.chenzaomai.com/gthxbdfaen.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.pengpengdd.cyou/gtyftqgjqz.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.shuidangran.top/gtsxzjscss.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.zhijiandao.cn/gtkeeebepg.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.sufxvd.cn/gtlckhonrx.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.chenzaomai.com/gtlstewawd.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.andypj.xyz/gtxlnbjzwi.html

================================================================================
来源：http://hz.smart0.xyz/gtcvsltiiy.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.zhaomingkeji.xyz/gteazbmkxs.html

================================================================================
来源：http://hz.52xcode.cn/gtxebrduts.html

[Q01] 创建表
来源：http://hz.zhaomingkeji.xyz/gthjthvncv.html

CREATE TABLE users (
来源：http://hz.zhongyouzk.top/gtdyvfttpn.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.cqqwz.cn/gtypuaymuu.html

name VARCHAR(50) NOT NULL,
来源：http://hz.jinqigufen.top/gtuyizoksk.html

email VARCHAR(100) UNIQUE,
来源：http://hz.ehwqpu.com/gtraetuftf.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.xinyue.icu/gthrespupa.html

);
来源：http://hz.zhengqikj.top/gtnasivego.html

[Q02] 创建带外键的表
来源：http://hz.cashguo.top/gtuuupofqt.html

CREATE TABLE orders (
来源：http://hz.tianlin.xyz/gtprzakanx.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.daxiang520.top/gtlrwtjirx.html

user_id INT NOT NULL,
来源：http://hz.havefunace.top/gtfgsbownn.html

amount DECIMAL(10, 2),
来源：http://hz.ywan-chungtsiang.top/gtnxwvkbtu.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.hongshengwenyu.top/gtfbajaono.html

);
来源：http://hz.cashguo.top/gtobnotfcp.html

[Q03] 增加列
来源：http://hz.shangyingyoupin.top/gtmclngmzy.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.yvedp.cn/gtoainmsjg.html

[Q04] 修改列类型
来源：http://hz.daria6918.cn/gtvtvpirno.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.zhongyouzk.top/gtlkozjgwm.html

[Q05] 重命名列
来源：http://hz.zhengqikj.top/gtpssnhgrx.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.smart0.xyz/gtwhvnnxgt.html

[Q06] 删除列
来源：http://hz.dianchejie.cn/gttjdwuydb.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.yvedp.cn/gtvklhcwhz.html

[Q07] 删除表
来源：http://hz.haohaochexian.top/gtjwkgwlgn.html

DROP TABLE IF EXISTS orders;
来源：http://hz.birdmap.top/gtfnturrqk.html

[Q08] 创建普通索引
来源：http://hz.yuxming.cn/gtvvzyvuye.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.fengsongda.top/gtipzmkkso.html

[Q09] 创建唯一索引
来源：http://hz.52xcode.cn/gthwrzeehx.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.yj20258.top/gtrrcjgxsf.html

[Q10] 插入单行
来源：http://hz.zdqjudy.top/gtlvymemaw.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.shanyushiyangtech.top/gtwomietgr.html

[Q11] 一次插入多行
来源：http://hz.yangfankeji.com/gthzgonwtx.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.iojbl.cn/gtueckoocj.html

[Q12] 插入后取自增 ID
来源：http://hz.ybcxt.top/gtqgtviltz.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.zdqjudy.top/gteyzwrxyg.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.gaohongyu789.top/gthfbpfqyj.html

[Q13] 忽略重复插入
来源：http://hz.daria6918.cn/gtjxnpowes.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.meibo888.top/gtrlijjcpf.html

[Q14] 存在则更新（upsert）
来源：http://hz.quarkkingdee.top/gtgcdekify.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.316326.xyz/gtdxjqyrve.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.gotoacloud.top/gtatdrfrhx.html

[Q15] 查询全部
来源：http://hz.yvedp.cn/gtdswtwpqg.html

SELECT * FROM users;
来源：http://hz.xylfe.cn/gtqcibxvxm.html

[Q16] 查询指定列
来源：http://hz.meibo888.top/gtpezogcdg.html

SELECT id, name FROM users;
来源：http://hz.meibo888.top/gtvvkhdezs.html

[Q17] 条件查询
来源：http://hz.jqgfzy.top/gtxzdvilth.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.jinqigufen.top/gtqpislrrf.html

[Q18] 模糊匹配
来源：http://hz.aibaodan.cn/gtjfbsajyl.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.zhongyouzk.top/gthxzhmycy.html

[Q19] 范围查询
来源：http://hz.hongshengwenyu.top/gtklwkkzcp.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.guannengcc.top/gtxwpgbzgc.html

[Q20] IN 列表
来源：http://hz.xuanzx.com/gtvqxnqdgh.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.gaohongyu789.top/gtihwoacej.html

[Q21] 空值判断
来源：http://hz.zycfv.cn/gtcdqwcirn.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.snrcjt.cn/gtobnlgmei.html

[Q22] 排序
来源：http://hz.yvedp.cn/gtxstzfchw.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.ivvv.top/gtwibknfdw.html

[Q23] 分页
来源：http://hz.snrcjt.cn/gtwfwiybgh.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.xuetiantiany.cn/gtacwdcicb.html

[Q24] 去重
来源：http://hz.52xcode.cn/gtubwxglxs.html

SELECT DISTINCT city FROM users;
来源：http://hz.zdqjudy.top/gtqcxgvwyd.html

[Q25] 只取前 N 条
来源：http://hz.kuanghao11.cn/gtehmngixt.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.ywan-chungtsiang.top/gtoisecvib.html

[Q26] 计数
来源：http://hz.cdnleiting.top/gtfkrfauzi.html

SELECT COUNT(*) FROM users;
来源：http://hz.yueranfly.top/gtkwsvuruq.html

[Q27] 条件计数
来源：http://hz.andypj.xyz/gtjuykbcbb.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.svipenyu.cn/gttwbkkzgj.html

[Q28] 求和与平均
来源：http://hz.tanke756.top/gtseqaeqxj.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.dianchejie.cn/gtauminsct.html

[Q29] 最大最小值
来源：http://hz.havefunace.top/gtchtvrhzb.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.meibo888.top/gthsxngrzj.html

[Q30] 分组统计
来源：http://hz.sxryk.cn/gthuvsueuo.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.svipenyu.cn/gthjsotxhd.html

[Q31] 分组后过滤
来源：http://hz.zhoulong.xyz/gttoolaucc.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.jlsjyb.cn/gtwjqgdkdg.html

[Q32] 分组拼接字符串
来源：http://hz.kuanghao11.cn/gtenwwhrvv.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.shzxlz.cn/gtfdoeeaxv.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.dianchejie.cn/gtefwbjosr.html

[Q33] 多列分组
来源：http://hz.smart0.xyz/gtgysltusy.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.sufxvd.cn/gtjntoaozm.html

[Q34] 每组取第一条
来源：http://hz.sysykeji.top/gtqhttvyhb.html

SELECT * FROM (
来源：http://hz.gzhubu.top/gtkcddqnvq.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.quarkkingdee.top/gttpkfrrel.html

) t WHERE rn = 1;
来源：http://hz.zhiwuduotai.top/gtlvjvfpcr.html

[Q35] 内连接
来源：http://hz.chenzaomai.com/gtglykvsbs.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.yj202588.top/gtkfzcuenz.html

[Q36] 左连接
来源：http://hz.shzxlz.cn/gtehiesprc.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.redwolf501.top/gtbukubjaq.html

[Q37] 右连接
来源：http://hz.haohaochexian.top/gtirlmwsfz.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.yueranfly.top/gtnyfrbasd.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.cheryme.top/gtodhechxm.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.shanyushiyangtech.top/gtrzidepsn.html

[Q39] 自连接（查上下级）
来源：http://hz.yj202588.top/gtebcqmhis.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.shuidangran.top/gthszxulin.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.sxryk.cn/gtclticheh.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.ybcxt.top/gtxngtdoih.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.yueranfly.top/gtnrwiqczm.html

[Q41] 多表连接
来源：http://hz.chenzaomai.com/gtvtadjsmu.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.fengsongda.top/gtmglqmwut.html

JOIN users u ON u.id = o.user_id
来源：http://hz.ivvv.top/gtoiyiijdt.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.hysaishi.cn/gtkketfmqs.html

[Q42] 连接条件附加过滤
来源：http://hz.hongshengwenyu.top/gtjfeiemsv.html

SELECT u.name, o.amount FROM users u
来源：http://hz.fengsongda.top/gtsgomklog.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.yj20258.top/gtezmbhygk.html

[Q43] 标量子查询
来源：http://hz.zhixingplan.top/gtsyokalwf.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.zdqjudy.top/gthycrvady.html

[Q44] IN 子查询
来源：http://hz.jqgufenzy.top/gtulcgzjxv.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.hywenlv.cn/gtogcgmiww.html

[Q45] EXISTS 判断存在
来源：http://hz.sxryk.cn/gtckqfxjvm.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.kuanghao11.cn/gtzzdqreic.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.cashguo.top/gtzfsfmule.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yueranfly.top/gtjuaudsye.html

[Q47] 与平均值比较
来源：http://hz.xingfuxueyuan.xyz/gtzxaindck.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.cqqwz.cn/gtijswtuip.html

[Q48] CTE 公用表表达式
来源：http://hz.chenlongwang.top/gtbmydckxq.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.snrcjt.cn/gtweqftzpg.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.jinqigufen.top/gtpkxdijyk.html

[Q49] 更新单行
来源：http://hz.fzhhl.top/gtqviilemi.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.yonumen.top/gttdmtzbfz.html

[Q50] 批量更新
来源：http://hz.yj20258888.top/gttezzabmu.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.guannengcc.top/gtploulfys.html

[Q51] 用子查询更新
来源：http://hz.hfpthk.cn/gtidgekrpg.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.yangfankeji.com/gtcpcmhkad.html

[Q52] 删除指定行
来源：http://hz.hywenlv.cn/gtwosilfkf.html

DELETE FROM users WHERE id = 10;
来源：http://hz.tian-w.cn/gtlnzgegdh.html

[Q53] 按条件删除
来源：http://hz.jinyuanbaomall.cn/gtcznaxwjp.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.gaohongyu789.top/gthflllrqa.html

[Q54] 清空表
来源：http://hz.tian-w.cn/gtkolszkjy.html

TRUNCATE TABLE logs;
来源：http://hz.316326.xyz/gtothkbgpp.html

[Q55] 排名（并列占位）
来源：http://hz.hfpthk.cn/gtiampzbvz.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.ivvv.top/gtofrbatvi.html

[Q56] 密集排名（并列不占位）
来源：http://hz.jqgufenzy.top/gtfnvjtvos.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.ybcxt.top/gtjnryukup.html

[Q57] 行号
来源：http://hz.daria6918.cn/gtqyanooti.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.zycfv.cn/gtvadhbtqc.html

[Q58] 累计求和
来源：http://hz.fengsongda.top/gtrafkkggn.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.nwbrower.top/gtjwnuqufz.html

[Q59] 分组内累计
来源：http://hz.guowangkeji.top/gtizxsdhrf.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.xuanzx.com/gtxtndznii.html

[Q60] 取上一行 / 下一行
来源：http://hz.pycfn.com/gtbwgllnjm.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.zhaomingkeji.xyz/gtwdhvovqv.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.xuanzx.com/gtpyxlvvsq.html

[Q61] 移动平均
来源：http://hz.sysykeji.top/gtkrrhnskw.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.guannengcc.top/gtzdittfac.html

[Q62] 分组占比
来源：http://hz.wangshuangyany.cn/gtyztfdgvz.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.havefunace.top/gtfjqfeviq.html

[Q63] 开启事务
来源：http://hz.hywenlv.cn/gtmifyetbj.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.wangshuangyany.cn/gtixqxmitn.html

[Q64] 提交事务
来源：http://hz.xuanzx.com/gtphdlpiwq.html

COMMIT;
来源：http://hz.ywan-chungtsiang.top/gtopczvfcp.html

[Q65] 回滚事务
来源：http://hz.xinyue.icu/gtcwbjtrqj.html

ROLLBACK;
来源：http://hz.yj202588.top/gtwptjxsev.html

[Q66] 行锁查询
来源：http://hz.yuxming.cn/gtcwejmhxc.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.jinghuilouyu.cn/gtmiahzsir.html

[Q67] 设置隔离级别
来源：http://hz.jinghuilouyu.cn/gtvybnvlrx.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.smart0.xyz/gtcselxhev.html

[Q68] 保存点
来源：http://hz.yongpay.top/gtgkmtmxaf.html

SAVEPOINT sp1;
来源：http://hz.c1oappe.top/gtblikwqzi.html

ROLLBACK TO sp1;
来源：http://hz.zycfv.cn/gtcjjzmgdo.html

[Q69] 查看执行计划
来源：http://hz.hnqzz.top/gtnsdgolrc.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.zhongyouzk.top/gtmkoljzdg.html

[Q70] 更新统计信息
来源：http://hz.ehwqpu.com/gtqjtyltqy.html

ANALYZE TABLE users;
来源：http://hz.sufxvd.cn/gtkezxgjwz.html

[Q71] 查看建表语句
来源：http://hz.shzxlz.cn/gtdhmsohlz.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.hammf.cn/gteunrqsox.html

[Q72] 查看索引
来源：http://hz.nanxinkj.top/gtzdsglqmt.html

SHOW INDEX FROM users;
来源：http://hz.vqdsnc.cn/gtvffedttx.html

[Q73] 查看表状态
来源：http://hz.zhijiandao.cn/gtxpgvrpdi.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.zhaomingkeji.xyz/gtzcgekrln.html

[Q74] 强制使用索引
来源：http://hz.wangdashe.top/gtjbgeutgn.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.jqgfzy.top/gtktspqdie.html

[Q75] 日期格式化
来源：http://hz.ywan-chungtsiang.top/gtakiyntse.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.hnqzz.top/gtsocgjwmk.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.jqgfzy.top/gtueccgyqe.html

[Q76] 按天统计
来源：http://hz.havefunace.top/gtyneowbzu.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.ywan-chungtsiang.top/gtgfjuqser.html

[Q77] 时间加减
来源：http://hz.shangyingyoupin.top/gtmeltwgnr.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.zhengqikj.top/gtecaaxuxh.html

[Q78] 当前时间
来源：http://hz.gotoacloud.top/gtbdygnemp.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.yonumen.top/gtxocvcsdk.html

[Q79] 字符串拼接
来源：http://hz.nanxinkj.top/gtfhjjqwkx.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.ydjk.org.cn/gtvnrpbbmo.html

[Q80] 字符串截取
来源：http://hz.fzhhl.top/gteuhvlehv.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.shangyingyoupin.top/gtqdzbrsfz.html

[Q81] 字符串替换
来源：http://hz.fengsongda.top/gtaigvkzyj.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.svipenyu.cn/gtsvanprcz.html

[Q82] 字符长度与字节长度
来源：http://hz.vqdsnc.cn/gtrvdjzaja.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.sweek.top/gtvjdtojps.html

[Q83] 大小写转换
来源：http://hz.ydzc1.top/gtwzsbqmbh.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.ehwqpu.com/gtyrkaiyio.html

[Q84] 去除首尾空格
来源：http://hz.svipenyu.cn/gtbzdrudal.html

SELECT TRIM(name) FROM users;
来源：http://hz.yanxiufei.cn/gtnitkrhzg.html

[Q85] 数值取整
来源：http://hz.dashuyun.cn/gtoqgnksth.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.fengsongda.top/gtfoapznos.html

[Q86] 读取 JSON 字段
来源：http://hz.zhiwuduotai.top/gticqbjkzf.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.0kj1m.cn/gtbxpezqlx.html

[Q87] JSON 字段做条件
来源：http://hz.daria6918.cn/gtgjjstxtg.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.wangshuangyany.cn/gtwrvnxffb.html

[Q88] 行转列（条件聚合）
来源：http://hz.meibo888.top/gtvzzcaaqc.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.nanxinkj.top/gttsxfiswk.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.gzhubu.top/gtrqevalqx.html

[Q89] 判断表是否存在
来源：http://hz.havefunace.top/gtjiinuorq.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.chenzaomai.com/gtplsmbicn.html

[Q90] 生成序号列
来源：http://hz.cashguo.top/gtkmbaigkt.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.shuidangran.top/gtzottyopv.html

================================================================================
来源：http://hz.sxryk.cn/gttfhkevhk.html

R. Bash 专题
来源：http://hz.smart0.xyz/gtdrzqfxxd.html

================================================================================
来源：http://hz.fengsongda.top/gtfelirysu.html

[R01] shebang 与严格模式
来源：http://hz.zhijiandao.cn/gtndumeejh.html

#!/usr/bin/env bash
来源：http://hz.cheryme.top/gtztvepcbq.html

set -euo pipefail
来源：http://hz.gotoacloud.top/gtyyudrzpo.html

[R02] 变量赋值与使用
来源：http://hz.gogol.net.cn/gtsyfgsyzb.html

name="Tom"; echo "$name"
来源：http://hz.9152youxi.cn/gtekhsapss.html

[R03] 只读变量
来源：http://hz.dianchejie.cn/gtdqglzhxf.html

readonly PI=3.14
来源：http://hz.meibo888.top/gtroyqsqlj.html

[R04] 位置参数
来源：http://hz.vqdsnc.cn/gtmkgxwebr.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.0kj1m.cn/gtynijmsot.html

[R05] 参数默认值
来源：http://hz.zdqjudy.top/gtmpsbjqlt.html


<!-- 参考信息 -->