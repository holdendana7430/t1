代发 wailian999

Py:   asyncio.gather(*tasks)
来源：http://hz.xinyue.icu/gtikxudvsw.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.ybcxt.top/gtwaphbfyd.html

JS:   await Promise.all(tasks)
来源：http://hz.ywan-chungtsiang.top/gtpvnlyrxw.html

TS:   await Promise.all(tasks)
来源：http://hz.shzxlz.cn/gtrzwbvayp.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.jlsjyb.cn/gtkqklcydz.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.yuxming.cn/gtyipyjlnu.html

Ruby: threads.map(&:join)
来源：http://hz.shanyushiyangtech.top/gtdloihqlz.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.guowangkeji.top/gtxvmqwscq.html

[O06] 使用进程池
来源：http://hz.shanyushiyangkeji.top/gtrzskplye.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.yanxiufei.cn/gtoirkzzkc.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.fzhhl.top/gtnlkcdnyk.html

JS:   // child_process / cluster 模块
来源：http://hz.ppjwa.cn/gtqtadoyoo.html

TS:   // child_process / cluster 模块
来源：http://hz.yanxiufei.cn/gtrvxhmest.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.gotoacloud.top/gtzflvjopx.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.zhixingplan.top/gtzptrknsy.html

Ruby: // fork 块
来源：http://hz.hywenlv.cn/gtvsirjjfh.html

C#:   Parallel.For
来源：http://hz.chenzaomai.com/gtpemtudal.html

================================================================================
来源：http://hz.guowangkeji.top/gtgodateqv.html

P. 常用工具函数
来源：http://hz.guannengcc.top/gtjcnypbyc.html

================================================================================
来源：http://hz.redwolf501.top/gtdgvmeyyl.html

[P01] 生成 UUID
来源：http://hz.wangdashe.top/gtiehatlcl.html

Py:   str(uuid.uuid4())
来源：http://hz.gaohongyu789.top/gtpqyvhvmt.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.chenlongwang.top/gtjognlojg.html

JS:   crypto.randomUUID()
来源：http://hz.tianlin.xyz/gtquwfltro.html

TS:   crypto.randomUUID()
来源：http://hz.quarkkingdee.top/gtsyobqvlr.html

Java: UUID.randomUUID().toString()
来源：http://hz.smart0.xyz/gtzmjtzoql.html

Go:   // 用 github.com/google/uuid
来源：http://hz.yanxiufei.cn/gtlsxaqfov.html

Ruby: SecureRandom.uuid
来源：http://hz.dashuyun.cn/gtoqbyhiql.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.havefunace.top/gtxxvzcbbm.html

[P02] MD5 / SHA256 摘要
来源：http://hz.aibaodan.cn/gttjvbsqzi.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.sysykeji.top/gtciphnihd.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.nanxinkj.top/gtiuydapoz.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.chenzaomai.com/gtjjurfabk.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.ivvv.top/gtkfgbkbis.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.xuanzx.com/gtfsdtdzyn.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.jqgfzy.top/gtlgejgdvj.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.pycfn.com/gtonsdvndo.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.yuxming.cn/gtuymztngh.html

[P03] 生成短随机字符串
来源：http://hz.yuanzhike.top/gtqrvpjfdg.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.yvedp.cn/gtkujmupzx.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.hongshengwenyu.top/gtiooigrmb.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.ydzc1.top/gtrmwpzfhi.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.andypj.xyz/gttpocjvkz.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.c1oappe.top/gtlkqjpymx.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.cdnleiting.top/gtzbbmsyxa.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.gaohongyu789.top/gtecbkyhfv.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.jinyuanbaomall.cn/gtykfyuxev.html

[P04] 求长度
来源：http://hz.mhx1999.top/gtfzfernsx.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.hnqzz.top/gtjtyochuw.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yj202588.top/gtpbfdmphe.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.nanxinkj.top/gtwghvgnxx.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.svipenyu.cn/gtwxauxgpr.html

Java: list.size();  map.size();  s.length()
来源：http://hz.ydzc1.top/gthozytbil.html

Go:   len(arr);  len(m)
来源：http://hz.quarkkingdee.top/gtccfekhqs.html

Ruby: x.length;  x.size
来源：http://hz.ivvv.top/gtgzttbipc.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.guannengcc.top/gtqzguffhg.html

[P05] 判断两个对象内容是否相等
来源：http://hz.tianlin.xyz/gtvkqszabx.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.shangyingyoupin.top/gtzneknngz.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.nanxuanxn.top/gtmbunuzxt.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.bjfxy.top/gtqbvnaczu.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.52xcode.cn/gtaufuqalr.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.xylfe.cn/gtfzctvxxq.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.hywenlv.cn/gtexsjcebx.html

Ruby: a == b
来源：http://hz.sxryk.cn/gtdkissvle.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.cdnleiting.top/gtookdxmll.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.dianchejie.cn/gtakvroixa.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.kuanghao11.cn/gtdtmqstks.html

PHP:  if (empty($x)) {}
来源：http://hz.zhongyouzk.top/gtlqdpmnmd.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.yj202588.top/gtqzirherk.html

TS:   if (x == null) {}
来源：http://hz.chenlongwang.top/gttheamrbm.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.yongpay.top/gtkljvmkoh.html

Go:   if x == nil {}
来源：http://hz.shanyushiyangkeji.top/gtkeolcrda.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.jyoumei.cn/gthgeygtft.html

C#:   if (x is null) {}
来源：http://hz.bjfxy.top/gtpevxsdyq.html

[P07] 防抖与节流
来源：http://hz.quarkkingdee.top/gtsuinhusm.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.gotoacloud.top/gtsudzaaca.html

PHP:  // 手写时间戳比较
来源：http://hz.haohaochexian.top/gteafkzevs.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.svipenyu.cn/gthikgakmb.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zycfv.cn/gtnrvtrhju.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.yj202588.top/gtnlfwvgro.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.cqqwz.cn/gtoabalpig.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.vqdsnc.cn/gtzwonljkq.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.52xcode.cn/gtdcufohwf.html

[P08] 处理浮点精度问题
来源：http://hz.tianlin.xyz/gtmzfrelbi.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.c1oappe.top/gtxrtscavp.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.shanyushiyangkeji.top/gttcgyaqnx.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.yj20258.top/gtwprxvyoi.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.hammf.cn/gtknyvatgl.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.ydzc1.top/gtzjsekafc.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.fengsongda.top/gtofsuaqbl.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.ehwqpu.com/gtqxacxtet.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.zhoulong.xyz/gteqclvetd.html

================================================================================
来源：http://hz.jqgufenzy.top/gtscnpbxdf.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.iojbl.cn/gtjynixfge.html

================================================================================
来源：http://hz.jqgufenzy.top/gtaqdubqjg.html

[Q01] 创建表
来源：http://hz.kuanghao11.cn/gtqkjisyzi.html

CREATE TABLE users (
来源：http://hz.zycfv.cn/gtvvekvhqd.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.nwbrower.top/gtkfpxamxe.html

name VARCHAR(50) NOT NULL,
来源：http://hz.jinyuanbaomall.cn/gtrvzddxyt.html

email VARCHAR(100) UNIQUE,
来源：http://hz.shanyushiyangkeji.top/gtxlwvqohr.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.aibaodan.cn/gtbmxhaqpo.html

);
来源：http://hz.ivvv.top/gtodnhjufk.html

[Q02] 创建带外键的表
来源：http://hz.jqgfzy.top/gtjzdieesq.html

CREATE TABLE orders (
来源：http://hz.ydjk.org.cn/gtwmelkzdt.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.shzxlz.cn/gtvmnmkwmf.html

user_id INT NOT NULL,
来源：http://hz.hongshengwenyu.top/gtkjgcngch.html

amount DECIMAL(10, 2),
来源：http://hz.jqgufenzy.top/gttomcmrlg.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.yanxiufei.cn/gtpqsdwmtb.html

);
来源：http://hz.cqqwz.cn/gtxuuptakj.html

[Q03] 增加列
来源：http://hz.ydjk.org.cn/gtcpgcfjmb.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.bjfxy.top/gtpzmeeknk.html

[Q04] 修改列类型
来源：http://hz.ivvv.top/gtegyauozs.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.316326.xyz/gtdsghqfgp.html

[Q05] 重命名列
来源：http://hz.gaohongyu789.top/gtrlqrqbok.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.birdmap.top/gtqfzjbkow.html

[Q06] 删除列
来源：http://hz.zhengqikj.top/gtzwormyyb.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.jinqigufen.top/gtkgaewjon.html

[Q07] 删除表
来源：http://hz.sweek.top/gtmddtepmf.html

DROP TABLE IF EXISTS orders;
来源：http://hz.dianchejie.cn/gtmyotocen.html

[Q08] 创建普通索引
来源：http://hz.ydzc1.top/gttokrxizh.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.shangyingyoupin.top/gtnuxvrgmq.html

[Q09] 创建唯一索引
来源：http://hz.jiagoushi.top/gtodifljac.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.aibaodan.cn/gthgxdjtyq.html

[Q10] 插入单行
来源：http://hz.ybcxt.top/gtkjgapjsr.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.zhoulong.xyz/gtrjevthcv.html

[Q11] 一次插入多行
来源：http://hz.ydjk.org.cn/gtyhjiipaw.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.zhijiandao.cn/gtufpnelup.html

[Q12] 插入后取自增 ID
来源：http://hz.feifeiyinyue.top/gtyieyueox.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.nanxinkj.top/gtqplkrgee.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.cashguo.top/gtphdnyifl.html

[Q13] 忽略重复插入
来源：http://hz.guannengcc.top/gtbmuizabb.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.nanxuanxn.top/gtivekmezy.html

[Q14] 存在则更新（upsert）
来源：http://hz.andypj.xyz/gtcljrlpyi.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.shangyingyoupin.top/gtnuppbfet.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.sxryk.cn/gtrhikvwlv.html

[Q15] 查询全部
来源：http://hz.cucudq.cn/gtpapvvvuu.html

SELECT * FROM users;
来源：http://hz.jyoumei.cn/gtrcliiriq.html

[Q16] 查询指定列
来源：http://hz.jinghuilouyu.cn/gtjpxujqjp.html

SELECT id, name FROM users;
来源：http://hz.0kj1m.cn/gtgxrtsbcx.html

[Q17] 条件查询
来源：http://hz.xuetiantiany.cn/gtbzkzvvds.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.shanyushiyangkeji.top/gtrawbnzeu.html

[Q18] 模糊匹配
来源：http://hz.cdnleiting.top/gtjjfzgalz.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.pycfn.com/gtoxgxbmhe.html

[Q19] 范围查询
来源：http://hz.smart0.xyz/gtfhlpmsrw.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.xylfe.cn/gtepfngeky.html

[Q20] IN 列表
来源：http://hz.cdnleiting.top/gtziujhrvv.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.guannengcc.top/gthgoiyktb.html

[Q21] 空值判断
来源：http://hz.yj20258.top/gtiehfnpiv.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.redwolf501.top/gtuofmtxrf.html

[Q22] 排序
来源：http://hz.havefunace.top/gtbjhvcfan.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.xuetiantiany.cn/gthfwdocxn.html

[Q23] 分页
来源：http://hz.hongshengwenyu.top/gtecrvwrux.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.yj202588.top/gteqlwivei.html

[Q24] 去重
来源：http://hz.feifeiyinyue.top/gtwxziprex.html

SELECT DISTINCT city FROM users;
来源：http://hz.wangshuangyany.cn/gtjjkeiotw.html

[Q25] 只取前 N 条
来源：http://hz.dianchejie.cn/gtotpmzvzs.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.zhoulong.xyz/gtlsrmbvma.html

[Q26] 计数
来源：http://hz.redwolf501.top/gtrrhimpvs.html

SELECT COUNT(*) FROM users;
来源：http://hz.0kj1m.cn/gtvcwrxjnx.html

[Q27] 条件计数
来源：http://hz.yanxiufei.cn/gtsdqwispx.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.wangdashe.top/gtbgsjcclg.html

[Q28] 求和与平均
来源：http://hz.yonumen.top/gtooevucqy.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.sweek.top/gtimomkaxy.html

[Q29] 最大最小值
来源：http://hz.9152youxi.cn/gtlrecypnh.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.aibaodan.cn/gtieudnhet.html

[Q30] 分组统计
来源：http://hz.redwolf501.top/gtfkxgelld.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.jlsjyb.cn/gthfptyzxr.html

[Q31] 分组后过滤
来源：http://hz.yvedp.cn/gtwddesqti.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.hnxiangtu.top/gthtwqtwqj.html

[Q32] 分组拼接字符串
来源：http://hz.wangdashe.top/gtzwooefzd.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.52xcode.cn/gtijbugekr.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.dianchejie.cn/gtkkjciqya.html

[Q33] 多列分组
来源：http://hz.cashguo.top/gtuijmttuh.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.shzxlz.cn/gtmlbwoafj.html

[Q34] 每组取第一条
来源：http://hz.nwbrower.top/gtaedyndpu.html

SELECT * FROM (
来源：http://hz.tianlin.xyz/gtnigxwidf.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.cqqwz.cn/gtfplbtyxb.html

) t WHERE rn = 1;
来源：http://hz.shzxlz.cn/gtpbdxmgbv.html

[Q35] 内连接
来源：http://hz.jlsjyb.cn/gtqqtvkovy.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.ivvv.top/gtyvstbskh.html

[Q36] 左连接
来源：http://hz.cashguo.top/gtoqfjmhcp.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.zycfv.cn/gtdiujlrwd.html

[Q37] 右连接
来源：http://hz.havefunace.top/gttcuyjkkx.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.jiagoushi.top/gtlorxtwzn.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.yj202588.top/gtzhcewvqv.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.ywan-chungtsiang.top/gtvjgbeepb.html

[Q39] 自连接（查上下级）
来源：http://hz.hnxiangtu.top/gtjeytpafg.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.0kj1m.cn/gtisjllrmk.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.zycfv.cn/gtwsrilxdt.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.cucudq.cn/gtqrwocjhs.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.cdnleiting.top/gtydcoqdlk.html

[Q41] 多表连接
来源：http://hz.snrcjt.cn/gtrjlcafkx.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.jianghu66.top/gtubfbgqzj.html

JOIN users u ON u.id = o.user_id
来源：http://hz.hywenlv.cn/gtoxjaiokt.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.jinqigfzy.top/gtgmyxfkty.html

[Q42] 连接条件附加过滤
来源：http://hz.shuidangran.top/gtldtgdpnk.html

SELECT u.name, o.amount FROM users u
来源：http://hz.jyoumei.cn/gtblhypbfm.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.svipenyu.cn/gtehptdprz.html

[Q43] 标量子查询
来源：http://hz.yuxming.cn/gtmxwcedte.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.yvedp.cn/gtbydkqltr.html

[Q44] IN 子查询
来源：http://hz.zhaomingkeji.xyz/gtmxeaexvn.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.cqqwz.cn/gtfbvxlajc.html

[Q45] EXISTS 判断存在
来源：http://hz.ydzc1.top/gtqpcusvxl.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jianghu66.top/gtduydybxc.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.316326.xyz/gtyclubdct.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.sweek.top/gtuerntvbs.html

[Q47] 与平均值比较
来源：http://hz.quarkkingdee.top/gtfqvjwjyj.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.jinghuilouyu.cn/gtfolijtjl.html

[Q48] CTE 公用表表达式
来源：http://hz.gzhubu.top/gtivivpbkq.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.yj20258.top/gtdaoxkdtz.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.svipenyu.cn/gtlfuwmjvd.html

[Q49] 更新单行
来源：http://hz.sufxvd.cn/gtfiimvakn.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.gotoacloud.top/gtxjgrjaqw.html

[Q50] 批量更新
来源：http://hz.quarkkingdee.top/gtjkaumtrr.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.chenzaomai.com/gtijbpcdck.html

[Q51] 用子查询更新
来源：http://hz.yj20258.top/gtbxrjbdyv.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.shuidangran.top/gttdfigqhq.html

[Q52] 删除指定行
来源：http://hz.sufxvd.cn/gtswinhini.html

DELETE FROM users WHERE id = 10;
来源：http://hz.zhixingplan.top/gtsngctnog.html

[Q53] 按条件删除
来源：http://hz.zhoulong.xyz/gtphdpzkvo.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.aibaodan.cn/gtjcvospot.html

[Q54] 清空表
来源：http://hz.zhixingplan.top/gtwmhwerdp.html

TRUNCATE TABLE logs;
来源：http://hz.sufxvd.cn/gtnwrxbypj.html

[Q55] 排名（并列占位）
来源：http://hz.iojbl.cn/gtwieyplwu.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.feifeiyinyue.top/gtovlteawq.html

[Q56] 密集排名（并列不占位）
来源：http://hz.hysaishi.cn/gtulavjkac.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.jqgufenzy.top/gtsiwusevd.html

[Q57] 行号
来源：http://hz.zhixingplan.top/gtzavheswh.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.zhiwuduotai.top/gtkghexqhy.html

[Q58] 累计求和
来源：http://hz.sxryk.cn/gtmsaklzhs.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.tianlin.xyz/gtgblcoogx.html

[Q59] 分组内累计
来源：http://hz.0kj1m.cn/gtmrgwrnam.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.redwolf501.top/gteafxsage.html

[Q60] 取上一行 / 下一行
来源：http://hz.ywan-chungtsiang.top/gtivdfsswk.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.meibo888.top/gtaxyoxaew.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.chenzaomai.com/gtkhrgnxiz.html

[Q61] 移动平均
来源：http://hz.shangyingyoupin.top/gtqrhgwlvc.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.kuanghao11.cn/gthyhxokbz.html

[Q62] 分组占比
来源：http://hz.xingfuxueyuan.xyz/gtdwiurklq.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.yj202588.top/gtnexslpss.html

[Q63] 开启事务
来源：http://hz.fengsongda.top/gtziilevjn.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.gaohongyu789.top/gtzspthhxf.html

[Q64] 提交事务
来源：http://hz.shanyushiyangkeji.top/gtiflplodi.html

COMMIT;
来源：http://hz.tianlin.xyz/gtveuhhbho.html

[Q65] 回滚事务
来源：http://hz.havefunace.top/gtlvbpwypz.html

ROLLBACK;
来源：http://hz.316326.xyz/gtjbqnzwgw.html

[Q66] 行锁查询
来源：http://hz.yuxming.cn/gtcsiurukp.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.nanxuanxn.top/gtmqqwfmcm.html

[Q67] 设置隔离级别
来源：http://hz.zycfv.cn/gtpqzvhorf.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.gaohongyu789.top/gtmgluhyoy.html

[Q68] 保存点
来源：http://hz.sweek.top/gtgketgvmt.html

SAVEPOINT sp1;
来源：http://hz.jinqigufen.top/gtgowfheou.html

ROLLBACK TO sp1;
来源：http://hz.sxryk.cn/gtuwphtzqh.html

[Q69] 查看执行计划
来源：http://hz.xingfuxueyuan.xyz/gtcphznowj.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.ywan-chungtsiang.top/gtmwelvrgt.html

[Q70] 更新统计信息
来源：http://hz.pycfn.com/gtxkongcvs.html

ANALYZE TABLE users;
来源：http://hz.havefunace.top/gtuwzueiex.html

[Q71] 查看建表语句
来源：http://hz.ydjk.org.cn/gtbfqhdfsb.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.jinyuanbaomall.cn/gtsbaqkjva.html

[Q72] 查看索引
来源：http://hz.ivvv.top/gtpvmjrpdb.html

SHOW INDEX FROM users;
来源：http://hz.jqgfzy.top/gthwgxworr.html

[Q73] 查看表状态
来源：http://hz.aizwys.cn/gtmtwvskrd.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.jqgufenzy.top/gtaywtunfi.html

[Q74] 强制使用索引
来源：http://hz.316326.xyz/gtifzqnhzd.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.sxryk.cn/gtotfpaayt.html

[Q75] 日期格式化
来源：http://hz.jqgfzy.top/gtaayuqcww.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.jqgfzy.top/gttjkhrngd.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.mhx1999.top/gtaiecileo.html

[Q76] 按天统计
来源：http://hz.316326.xyz/gtkflqxltf.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.quarkkingdee.top/gtdgwtxquu.html

[Q77] 时间加减
来源：http://hz.cqqwz.cn/gtxftmyfuf.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.xuetiantiany.cn/gtbsiekswv.html

[Q78] 当前时间
来源：http://hz.gotoacloud.top/gtmksnnsqi.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.chenzaomai.com/gttkwbosux.html

[Q79] 字符串拼接
来源：http://hz.jinyuanbaomall.cn/gtarphiqkm.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.shuidangran.top/gtbubvylcr.html

[Q80] 字符串截取
来源：http://hz.zhengqikj.top/gtkbmwmrsi.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.cqqwz.cn/gtsxrbfzmn.html

[Q81] 字符串替换
来源：http://hz.gogol.net.cn/gtbetmhrsm.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.daria6918.cn/gtdqjxvsen.html

[Q82] 字符长度与字节长度
来源：http://hz.yongpay.top/gtwykquuko.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.meibo888.top/gtnvkhmzsb.html

[Q83] 大小写转换
来源：http://hz.jinyuanbaomall.cn/gtriodubdi.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.gaohongyu789.top/gtvhifpact.html

[Q84] 去除首尾空格
来源：http://hz.xingfuxueyuan.xyz/gtxuihctid.html

SELECT TRIM(name) FROM users;
来源：http://hz.dashuyun.cn/gtleegqpgy.html

[Q85] 数值取整
来源：http://hz.chenzaomai.com/gtelrifagu.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.9152youxi.cn/gtuibkywuo.html

[Q86] 读取 JSON 字段
来源：http://hz.tianlin.xyz/gtmqqbipky.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.kuanghao11.cn/gtdodzpnkq.html

[Q87] JSON 字段做条件
来源：http://hz.ybcxt.top/gtjtjkplpw.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.pycfn.com/gtvnyntuxt.html

[Q88] 行转列（条件聚合）
来源：http://hz.yuxming.cn/gtlgnrchhh.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.xinyue.icu/gtamfneryp.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.quarkkingdee.top/gtjyecdbri.html

[Q89] 判断表是否存在
来源：http://hz.fengsongda.top/gtqfabcncf.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.andypj.xyz/gtlojdzliu.html

[Q90] 生成序号列
来源：http://hz.xuetiantiany.cn/gtmptvlucy.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.chenlongwang.top/gtapcckntc.html

================================================================================
来源：http://hz.kuanghao11.cn/gtxokobqzy.html


<!-- 参考信息 -->