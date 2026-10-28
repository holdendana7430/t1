代发 wailian999

[O06] 使用进程池
来源：http://hz.zhijiandao.cn/gtokscttma.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.52xcode.cn/gtgkytnpfw.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.nanxinkj.top/gtrpsiprbc.html

JS:   // child_process / cluster 模块
来源：http://hz.andypj.xyz/gtmpouqbzx.html

TS:   // child_process / cluster 模块
来源：http://hz.guowangkeji.top/gtdatrsoqu.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.gotoacloud.top/gtmcdxrble.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.cdnleiting.top/gtczaadcqc.html

Ruby: // fork 块
来源：http://hz.cdnleiting.top/gtzzevzsvl.html

C#:   Parallel.For
来源：http://hz.pengpengdd.cyou/gtqxqqhrao.html

================================================================================
来源：http://hz.gzhubu.top/gtmyvmihtm.html

P. 常用工具函数
来源：http://hz.zhengqikj.top/gtzltwrnzu.html

================================================================================
来源：http://hz.yueranfly.top/gtynwdlfmp.html

[P01] 生成 UUID
来源：http://hz.ybcxt.top/gtilfrllql.html

Py:   str(uuid.uuid4())
来源：http://hz.jiagoushi.top/gtzyiaubbj.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.zhongyouzk.top/gtkruzgcnf.html

JS:   crypto.randomUUID()
来源：http://hz.xuetiantiany.cn/gtgqkfaqix.html

TS:   crypto.randomUUID()
来源：http://hz.aizwys.cn/gtcuvoatjz.html

Java: UUID.randomUUID().toString()
来源：http://hz.tianlin.xyz/gtlkdugnft.html

Go:   // 用 github.com/google/uuid
来源：http://hz.xinyue.icu/gtbrapsyqf.html

Ruby: SecureRandom.uuid
来源：http://hz.yj20258.top/gtpsbavdhz.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.birdmap.top/gtjqnnpmgt.html

[P02] MD5 / SHA256 摘要
来源：http://hz.guannengcc.top/gtxplknryb.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.gaohongyu789.top/gtnpynifso.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.jinqigufen.top/gtgcusbzcx.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.bjfxy.top/gthynlirpf.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.quarkkingdee.top/gtdgezyocb.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.kuanghao11.cn/gtteagwlun.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.jyoumei.cn/gtircxwyrs.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.xziqi.cn/gttwmbivlk.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.aizwys.cn/gtvupkrbnd.html

[P03] 生成短随机字符串
来源：http://hz.sxryk.cn/gtpsyamjqv.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.xziqi.cn/gtbevsqhec.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.yongpay.top/gtbeqcslol.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jiagoushi.top/gtorkaqlqp.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yangfankeji.com/gtoakurgzq.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.nanxinkj.top/gtotniwjxo.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.xinyue.icu/gtekwgzdtb.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.kuanghao11.cn/gtcfrvinzk.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.dianchejie.cn/gtbggosisb.html

[P04] 求长度
来源：http://hz.xuanzx.com/gtqpariuix.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.sxryk.cn/gtefnsvrvd.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zhoulong.xyz/gtxztwjoep.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.jiagoushi.top/gtaatxdsij.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.wangshuangyany.cn/gtbjziesvs.html

Java: list.size();  map.size();  s.length()
来源：http://hz.tianlin.xyz/gtgkcozkek.html

Go:   len(arr);  len(m)
来源：http://hz.jqgfzy.top/gtdtehudmp.html

Ruby: x.length;  x.size
来源：http://hz.hammf.cn/gtwimxnwnv.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.cucudq.cn/gtxlyswonm.html

[P05] 判断两个对象内容是否相等
来源：http://hz.shzxlz.cn/gtmukhprll.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.52xcode.cn/gtlxvbfwwe.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.0kj1m.cn/gtbsqguboc.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.shzxlz.cn/gtnlkqjpgy.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.aizwys.cn/gtehcznnku.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.c1oappe.top/gtafoomnhj.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.redwolf501.top/gtsqpkrbhy.html

Ruby: a == b
来源：http://hz.jlsjyb.cn/gtodmflvij.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.sweek.top/gthkhisqqw.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.zycfv.cn/gtebpimdpt.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.zhaomingkeji.xyz/gtlxsbmyll.html

PHP:  if (empty($x)) {}
来源：http://hz.feifeiyinyue.top/gtdwiobmyu.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.tanke756.top/gtnnhxecvt.html

TS:   if (x == null) {}
来源：http://hz.redwolf501.top/gtfkhtfnfe.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.redwolf501.top/gtcjboybzz.html

Go:   if x == nil {}
来源：http://hz.zhoulong.xyz/gthfbksdwy.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.feifeiyinyue.top/gtpljvfolj.html

C#:   if (x is null) {}
来源：http://hz.meibo888.top/gtcjuttoll.html

[P07] 防抖与节流
来源：http://hz.c1oappe.top/gtmqqfdlzp.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.wangdashe.top/gtwqbwigpr.html

PHP:  // 手写时间戳比较
来源：http://hz.aibaodan.cn/gtlqvampjc.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.9152youxi.cn/gtbgtpsfgw.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jyoumei.cn/gtnwmrscyt.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.yj20258.top/gthvzjaoqf.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.ydzc1.top/gtnpyaqdtm.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.vqdsnc.cn/gtywewrace.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.cdnleiting.top/gtbrpeepuh.html

[P08] 处理浮点精度问题
来源：http://hz.gogol.net.cn/gtsniqiyje.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.9152youxi.cn/gtwtbnruoc.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.snrcjt.cn/gtulqszfec.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.zhijiandao.cn/gtvsvseyyz.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.zdqjudy.top/gtbgpqjpvf.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.svipenyu.cn/gtdecjeqig.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.yj20258888.top/gtxjexomng.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.wangdashe.top/gtvmgmwkmf.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.kuanghao11.cn/gturwbaysn.html

================================================================================
来源：http://hz.xylfe.cn/gthkwhmsgb.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.chenzaomai.com/gtmumhuinr.html

================================================================================
来源：http://hz.shuidangran.top/gtfkhseepq.html

[Q01] 创建表
来源：http://hz.nwbrower.top/gtolbwikwk.html

CREATE TABLE users (
来源：http://hz.chenlongwang.top/gtdmekfmut.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.dianchejie.cn/gtuooeoviq.html

name VARCHAR(50) NOT NULL,
来源：http://hz.yanxiufei.cn/gtyckhantp.html

email VARCHAR(100) UNIQUE,
来源：http://hz.tianlin.xyz/gtnkxosehj.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.52xcode.cn/gtddvcuted.html

);
来源：http://hz.andypj.xyz/gtjqtztdmd.html

[Q02] 创建带外键的表
来源：http://hz.zdqjudy.top/gtdbjiuerd.html

CREATE TABLE orders (
来源：http://hz.gaohongyu789.top/gttzmxrefm.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.tianlin.xyz/gtnuxvflbl.html

user_id INT NOT NULL,
来源：http://hz.gzhubu.top/gtyabwibpk.html

amount DECIMAL(10, 2),
来源：http://hz.jinqigfzy.top/gtcirrwdtr.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.hongshengwenyu.top/gtjqbqexll.html

);
来源：http://hz.chenzaomai.com/gtkiaamira.html

[Q03] 增加列
来源：http://hz.zhaomingkeji.xyz/gtbtypruvn.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.dianchejie.cn/gtsrwzpbsp.html

[Q04] 修改列类型
来源：http://hz.zhongyouzk.top/gtlyutyons.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.ppjwa.cn/gtppmvppky.html

[Q05] 重命名列
来源：http://hz.yongpay.top/gtotsgwunj.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.chenlongwang.top/gtlxmcamot.html

[Q06] 删除列
来源：http://hz.yvedp.cn/gtxnyylrdb.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.gaohongyu789.top/gtgcokmngr.html

[Q07] 删除表
来源：http://hz.cucudq.cn/gtvditryws.html

DROP TABLE IF EXISTS orders;
来源：http://hz.jinghuilouyu.cn/gtlxzyybma.html

[Q08] 创建普通索引
来源：http://hz.ybcxt.top/gtzkjrptye.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.cdnleiting.top/gtuqawprqr.html

[Q09] 创建唯一索引
来源：http://hz.hywenlv.cn/gtykwanasb.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.mhx1999.top/gtkammyzke.html

[Q10] 插入单行
来源：http://hz.pengpengdd.cyou/gtkktglorp.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.nanxuanxn.top/gtizrzskjw.html

[Q11] 一次插入多行
来源：http://hz.ppjwa.cn/gtlhkljurd.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.aibaodan.cn/gtimhedhlx.html

[Q12] 插入后取自增 ID
来源：http://hz.hysaishi.cn/gtprbnbrbj.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.chenzaomai.com/gtgutzvfex.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.tian-w.cn/gtpineekwv.html

[Q13] 忽略重复插入
来源：http://hz.iojbl.cn/gtskvaqesa.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.hnxiangtu.top/gtucbubfwa.html

[Q14] 存在则更新（upsert）
来源：http://hz.hysaishi.cn/gtdnrgfhhq.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.ppjwa.cn/gtvhisiwnm.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.yuxming.cn/gtgnemzpbn.html

[Q15] 查询全部
来源：http://hz.zhongyouzk.top/gtojwvoojg.html

SELECT * FROM users;
来源：http://hz.wangshuangyany.cn/gttxztsxli.html

[Q16] 查询指定列
来源：http://hz.birdmap.top/gtajietaia.html

SELECT id, name FROM users;
来源：http://hz.andypj.xyz/gtlptcprkp.html

[Q17] 条件查询
来源：http://hz.snrcjt.cn/gtosfqfylq.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.feifeiyinyue.top/gtlewhiwca.html

[Q18] 模糊匹配
来源：http://hz.dianchejie.cn/gtnbqlbnks.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.yangfankeji.com/gttytfpxmb.html

[Q19] 范围查询
来源：http://hz.0kj1m.cn/gtxanxlkon.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.cdnleiting.top/gtbfgzgonn.html

[Q20] IN 列表
来源：http://hz.ehwqpu.com/gtjrishsvz.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.yuanzhike.top/gtitjrikym.html

[Q21] 空值判断
来源：http://hz.pengpengdd.cyou/gtzqpjeulv.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.xingfuxueyuan.xyz/gtqxhhpzni.html

[Q22] 排序
来源：http://hz.wangshuangyany.cn/gtajqueyrh.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.xziqi.cn/gtrqwbggdb.html

[Q23] 分页
来源：http://hz.jiagoushi.top/gtkviyknfc.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.jyoumei.cn/gtgaoazjbt.html

[Q24] 去重
来源：http://hz.yanxiufei.cn/gtcucelpxs.html

SELECT DISTINCT city FROM users;
来源：http://hz.zdqjudy.top/gtwbzbfclq.html

[Q25] 只取前 N 条
来源：http://hz.dashuyun.cn/gtvwpiidij.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.shangyingyoupin.top/gtkgsfmmpj.html

[Q26] 计数
来源：http://hz.fzhhl.top/gtdijkndmr.html

SELECT COUNT(*) FROM users;
来源：http://hz.zycfv.cn/gttzfokwpu.html

[Q27] 条件计数
来源：http://hz.jinqigfzy.top/gtxohuptxj.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.zycfv.cn/gtqevscllu.html

[Q28] 求和与平均
来源：http://hz.yongpay.top/gtrczdgcyj.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.hnqzz.top/gtmtytyykb.html

[Q29] 最大最小值
来源：http://hz.ydzc1.top/gtuoqixzzk.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.hammf.cn/gtytygcicv.html

[Q30] 分组统计
来源：http://hz.jinghuilouyu.cn/gtbplnnfnx.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.xuanzx.com/gtplwvtfmh.html

[Q31] 分组后过滤
来源：http://hz.svipenyu.cn/gtmuunjpsq.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.hfpthk.cn/gtiytxzwwm.html

[Q32] 分组拼接字符串
来源：http://hz.ydjk.org.cn/gtdcvcgbvb.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.guowangkeji.top/gtrdhcdhsm.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.cashguo.top/gtsslxhdqi.html

[Q33] 多列分组
来源：http://hz.cdnleiting.top/gthkfyltor.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.tian-w.cn/gtzffqgxtz.html

[Q34] 每组取第一条
来源：http://hz.jiagoushi.top/gtkwpxkjkq.html

SELECT * FROM (
来源：http://hz.chenzaomai.com/gtlyumklwx.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.aizwys.cn/gtnfpmkyyf.html

) t WHERE rn = 1;
来源：http://hz.quarkkingdee.top/gtobxpvmwx.html

[Q35] 内连接
来源：http://hz.aibaodan.cn/gtokvchreb.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.jinghuilouyu.cn/gtvsyglrmw.html

[Q36] 左连接
来源：http://hz.nwbrower.top/gtejbcoxrv.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.zhongyouzk.top/gtmcruenss.html

[Q37] 右连接
来源：http://hz.daxiang520.top/gtlmjbzsbw.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.xylfe.cn/gtnkvlhxmb.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.xinyue.icu/gtnxgicczu.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.shanyushiyangkeji.top/gtdpsgkeom.html

[Q39] 自连接（查上下级）
来源：http://hz.daria6918.cn/gtfheucuep.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.gaohongyu789.top/gtsuyiqcuw.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.hysaishi.cn/gtbrciocqn.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.xingfuxueyuan.xyz/gtznvlnafy.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.hywenlv.cn/gtrpubkmmn.html

[Q41] 多表连接
来源：http://hz.yj20258888.top/gtlkgkhpvc.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.cashguo.top/gtucsisjpr.html

JOIN users u ON u.id = o.user_id
来源：http://hz.feifeiyinyue.top/gtwkwjweun.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.yj202588.top/gtnauvfiow.html

[Q42] 连接条件附加过滤
来源：http://hz.shangyingyoupin.top/gtdvizotot.html

SELECT u.name, o.amount FROM users u
来源：http://hz.ppjwa.cn/gtmziyrdth.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.tian-w.cn/gtycaletee.html

[Q43] 标量子查询
来源：http://hz.wangdashe.top/gtnossaypy.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.cashguo.top/gtmubscbqf.html

[Q44] IN 子查询
来源：http://hz.cdnleiting.top/gtbjycnddj.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.nanxuanxn.top/gtyqsljohp.html

[Q45] EXISTS 判断存在
来源：http://hz.xinyue.icu/gtqariwptz.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.guowangkeji.top/gtufwhhiho.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.ydjk.org.cn/gtqmpxxqlu.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.fzhhl.top/gtmdttyylt.html

[Q47] 与平均值比较
来源：http://hz.sysykeji.top/gtsfkesqzu.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.zhoulong.xyz/gthmelamxd.html

[Q48] CTE 公用表表达式
来源：http://hz.hysaishi.cn/gtmverrfyj.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.yuanzhike.top/gtvfcnjywa.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.xuanzx.com/gtnxwbswiw.html

[Q49] 更新单行
来源：http://hz.hfpthk.cn/gtxwerkxfk.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.smart0.xyz/gtrlitxjao.html

[Q50] 批量更新
来源：http://hz.shanyushiyangtech.top/gtfvvpoyls.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.nwbrower.top/gtgnzyezup.html

[Q51] 用子查询更新
来源：http://hz.xingfuxueyuan.xyz/gtdeirirye.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.nanxuanxn.top/gtobtxhhlr.html

[Q52] 删除指定行
来源：http://hz.gotoacloud.top/gtrxpmiecr.html

DELETE FROM users WHERE id = 10;
来源：http://hz.zhixingplan.top/gtakzuewfb.html

[Q53] 按条件删除
来源：http://hz.9152youxi.cn/gtneixrklk.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.pycfn.com/gtkxsfroct.html

[Q54] 清空表
来源：http://hz.c1oappe.top/gttepysvkc.html

TRUNCATE TABLE logs;
来源：http://hz.chenzaomai.com/gtkxkrizlm.html

[Q55] 排名（并列占位）
来源：http://hz.jlsjyb.cn/gtlatcjwqb.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.shanyushiyangkeji.top/gtruvbprqw.html

[Q56] 密集排名（并列不占位）
来源：http://hz.zhoulong.xyz/gtgspuglot.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.yuxming.cn/gtjmqjrsgp.html

[Q57] 行号
来源：http://hz.hysaishi.cn/gtjzkcllil.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.meibo888.top/gtmdpznxpn.html

[Q58] 累计求和
来源：http://hz.zhengqikj.top/gtxyzbwtum.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.jinqigufen.top/gtuoeqzivb.html

[Q59] 分组内累计
来源：http://hz.snrcjt.cn/gtyszintii.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.haohaochexian.top/gtxelxjhdl.html

[Q60] 取上一行 / 下一行
来源：http://hz.wangdashe.top/gtqkodmkzf.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.jqgfzy.top/gtvdptoyqt.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.yangfankeji.com/gtmforadib.html

[Q61] 移动平均
来源：http://hz.dashuyun.cn/gtfukgclgi.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.snrcjt.cn/gthgdjdqrg.html

[Q62] 分组占比
来源：http://hz.haohaochexian.top/gtxkphvsnh.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.shangyingyoupin.top/gtwexylutk.html

[Q63] 开启事务
来源：http://hz.jqgfzy.top/gtxeyxwbmy.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.sufxvd.cn/gtkgdojfpx.html

[Q64] 提交事务
来源：http://hz.shzxlz.cn/gttkfygaaa.html

COMMIT;
来源：http://hz.andypj.xyz/gtmghdeawh.html

[Q65] 回滚事务
来源：http://hz.nwbrower.top/gtmmywzqzu.html

ROLLBACK;
来源：http://hz.ywan-chungtsiang.top/gtvtfwdtop.html

[Q66] 行锁查询
来源：http://hz.jlsjyb.cn/gtsegzicpz.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.ywan-chungtsiang.top/gtecrtocyh.html

[Q67] 设置隔离级别
来源：http://hz.yanxiufei.cn/gtequidwmi.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.c1oappe.top/gtnvpqfnty.html

[Q68] 保存点
来源：http://hz.dashuyun.cn/gtdfyxzifz.html

SAVEPOINT sp1;
来源：http://hz.jianghu66.top/gtyatxgxax.html

ROLLBACK TO sp1;
来源：http://hz.daria6918.cn/gtaaeorbzn.html

[Q69] 查看执行计划
来源：http://hz.jianghu66.top/gtlrvhzqie.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.shanyushiyangkeji.top/gtzfaamgni.html

[Q70] 更新统计信息
来源：http://hz.cdnleiting.top/gtcekhgngx.html

ANALYZE TABLE users;
来源：http://hz.zhaomingkeji.xyz/gtnxybquao.html

[Q71] 查看建表语句
来源：http://hz.snrcjt.cn/gtjqypavsj.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.chenjidiqi.icu/gtlrfykyfq.html

[Q72] 查看索引
来源：http://hz.jqgufenzy.top/gtqhctjswc.html

SHOW INDEX FROM users;
来源：http://hz.52xcode.cn/gtqpfpxszx.html

[Q73] 查看表状态
来源：http://hz.jianghu66.top/gtvdekxmbn.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.yanxiufei.cn/gtwwtlxsxi.html

[Q74] 强制使用索引
来源：http://hz.ivvv.top/gttuinzroz.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.svipenyu.cn/gtkcnzreet.html

[Q75] 日期格式化
来源：http://hz.birdmap.top/gtayuywxvg.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.tianlin.xyz/gtbyyqnube.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.sufxvd.cn/gtmufaytks.html

[Q76] 按天统计
来源：http://hz.hnqzz.top/gtkghzjgtq.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.ydjk.org.cn/gtvrjdlkpb.html

[Q77] 时间加减
来源：http://hz.shangyingyoupin.top/gtgxjzonle.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.hywenlv.cn/gtbpoddafw.html

[Q78] 当前时间
来源：http://hz.zycfv.cn/gtwgovhxej.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.wangshuangyany.cn/gtldrzpxxa.html

[Q79] 字符串拼接
来源：http://hz.nanxinkj.top/gtpicdqdar.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.kuanghao11.cn/gttbhjxfcr.html

[Q80] 字符串截取
来源：http://hz.shzxlz.cn/gtyfoawoxt.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.xingfuxueyuan.xyz/gtxdciglax.html

[Q81] 字符串替换
来源：http://hz.shzxlz.cn/gthofnlwla.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.yangfankeji.com/gtivjmiffy.html

[Q82] 字符长度与字节长度
来源：http://hz.zhixingplan.top/gtqpvzrsjp.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.mhx1999.top/gtfaybtbru.html

[Q83] 大小写转换
来源：http://hz.tianlin.xyz/gtpoyadpib.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.jinqigfzy.top/gtdtgkqzvn.html

[Q84] 去除首尾空格
来源：http://hz.zhixingplan.top/gtxvsdyqdw.html

SELECT TRIM(name) FROM users;
来源：http://hz.ivvv.top/gtmwvyofjj.html

[Q85] 数值取整
来源：http://hz.yongpay.top/gtmyfcywbt.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.svipenyu.cn/gtjerxfots.html

[Q86] 读取 JSON 字段
来源：http://hz.xylfe.cn/gtysqohasp.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.iojbl.cn/gtdxgofpaz.html

[Q87] JSON 字段做条件
来源：http://hz.jinqigufen.top/gtenikbudn.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.cheryme.top/gtswpssdov.html

[Q88] 行转列（条件聚合）
来源：http://hz.yj20258888.top/gthvmavmzl.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.aizwys.cn/gthcawyeym.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.gzhubu.top/gtnpmpakgz.html

[Q89] 判断表是否存在
来源：http://hz.yuanzhike.top/gtntmhebzp.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.smart0.xyz/gtogxuxmsh.html

[Q90] 生成序号列
来源：http://hz.zhiwuduotai.top/gtrvebqrei.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.sxryk.cn/gtxyizzpeq.html

================================================================================
来源：http://hz.yj202588.top/gtjiaqxhzw.html

R. Bash 专题
来源：http://hz.shanyushiyangkeji.top/gtmhorcyba.html

================================================================================
来源：http://hz.yj20258.top/gthcumdjmb.html

[R01] shebang 与严格模式
来源：http://hz.redwolf501.top/gtdojsrviq.html

#!/usr/bin/env bash
来源：http://hz.yj202588.top/gtuothdbey.html

set -euo pipefail
来源：http://hz.zhoulong.xyz/gtvzhypeog.html

[R02] 变量赋值与使用
来源：http://hz.snrcjt.cn/gtdavmqjid.html

name="Tom"; echo "$name"
来源：http://hz.aibaodan.cn/gtqxzmgopj.html

[R03] 只读变量
来源：http://hz.9152youxi.cn/gtjxrosors.html


<!-- 参考信息 -->