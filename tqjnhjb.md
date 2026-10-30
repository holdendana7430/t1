代发 wailian999

[O06] 使用进程池
来源：http://baike.fanxiaobao.xyz/Article/details/gzcsioqce.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.fanxiaobao.xyz/Article/details/gkqcxfjzy.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.fanxiaobao.xyz/Article/details/gxrqvfnib.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.fanxiaobao.xyz/Article/details/gwtrrnulj.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.fanxiaobao.xyz/Article/details/gthethdcp.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.fanxiaobao.xyz/Article/details/gtbpmdcfn.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.fanxiaobao.xyz/Article/details/ganwnyrzs.sHtML

Ruby: // fork 块
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfvoaewzb.sHtML

C#:   Parallel.For
来源：http://www.share.fanxiaobao.xyz/Article/details/gdmvnevhp.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gplugnapz.sHtML

P. 常用工具函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gqfdclvhd.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/ggvbeypif.sHtML

[P01] 生成 UUID
来源：http://baike.fanxiaobao.xyz/Article/details/gdijblhso.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.fanxiaobao.xyz/Article/details/gaptzqxyi.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.fanxiaobao.xyz/Article/details/grdqtkiva.sHtML

JS:   crypto.randomUUID()
来源：http://wap.fanxiaobao.xyz/Article/details/gtohujboz.sHtML

TS:   crypto.randomUUID()
来源：http://baike.fanxiaobao.xyz/Article/details/gqjgaqajh.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.fanxiaobao.xyz/Article/details/gvdfyytbz.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.fanxiaobao.xyz/Article/details/gkwmynldv.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grlmmnekw.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.fanxiaobao.xyz/Article/details/gvndatirw.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.fanxiaobao.xyz/Article/details/gazwnrrqe.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.fanxiaobao.xyz/Article/details/gkiofwwib.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.fanxiaobao.xyz/Article/details/goeweaijc.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.fanxiaobao.xyz/Article/details/gvwnkbgal.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.fanxiaobao.xyz/Article/details/gvrtrvufq.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.fanxiaobao.xyz/Article/details/glgpdxlnc.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.fanxiaobao.xyz/Article/details/gtubkpdon.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gkuvtiorq.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.fanxiaobao.xyz/Article/details/gafqqlmpf.sHtML

[P03] 生成短随机字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gcrpyqjej.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.fanxiaobao.xyz/Article/details/gztlowois.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.fanxiaobao.xyz/Article/details/gbpzyyzlh.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fanxiaobao.xyz/Article/details/grbhzjeis.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fanxiaobao.xyz/Article/details/ghcdwghqx.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaojlfxjn.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.fanxiaobao.xyz/Article/details/gvvoexczi.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.fanxiaobao.xyz/Article/details/gnaruojcg.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.fanxiaobao.xyz/Article/details/gqfwdsfbq.sHtML

[P04] 求长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gwsgbkbma.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.fanxiaobao.xyz/Article/details/grhrcinuz.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fanxiaobao.xyz/Article/details/gexhlyqal.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gryoziymn.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fanxiaobao.xyz/Article/details/glhfnivlk.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.fanxiaobao.xyz/Article/details/gzdjzqltp.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvohblcri.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.fanxiaobao.xyz/Article/details/gojzdhjgh.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.fanxiaobao.xyz/Article/details/gjytqjwtp.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.fanxiaobao.xyz/Article/details/gqjoxpzae.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggpywfdoh.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.fanxiaobao.xyz/Article/details/gaumzxcel.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyvbhsvbu.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkssuhpft.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.fanxiaobao.xyz/Article/details/geaniwfmd.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.fanxiaobao.xyz/Article/details/grtqoojmt.sHtML

Ruby: a == b
来源：http://baike.fanxiaobao.xyz/Article/details/gapmrohmd.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geksztfeh.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyeviihls.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpfhfaxkl.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggmekfjkg.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.fanxiaobao.xyz/Article/details/gaytmaide.sHtML

TS:   if (x == null) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gekpetpxm.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gqmikaitx.sHtML

Go:   if x == nil {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvtiwydhg.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqdvixuoi.sHtML

C#:   if (x is null) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gbgenydqa.sHtML

[P07] 防抖与节流
来源：http://wap.fanxiaobao.xyz/Article/details/gmszlbrsm.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxscmpdup.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/glkkkhbkf.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fanxiaobao.xyz/Article/details/gnqkzxzls.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gmmmhwdqe.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdalfcfci.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.fanxiaobao.xyz/Article/details/garjzrwla.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.fanxiaobao.xyz/Article/details/gguupyxov.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.fanxiaobao.xyz/Article/details/giejlolie.sHtML

[P08] 处理浮点精度问题
来源：http://3g.fanxiaobao.xyz/Article/details/gricapukv.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdhksfzhn.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gypagodxj.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.fanxiaobao.xyz/Article/details/glkvcetsk.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtgkledcf.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.fanxiaobao.xyz/Article/details/gvybtxwvp.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.fanxiaobao.xyz/Article/details/ggodjdwvf.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.fanxiaobao.xyz/Article/details/gbvfavook.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.fanxiaobao.xyz/Article/details/gptknukub.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/golsagfwj.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.fanxiaobao.xyz/Article/details/gqwkvivml.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gaajpiznf.sHtML

[Q01] 创建表
来源：http://blog.fanxiaobao.xyz/Article/details/gktqhnnqo.sHtML

CREATE TABLE users (
来源：http://read.share.fanxiaobao.xyz/Article/details/gyvqqftru.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fanxiaobao.xyz/Article/details/gswkguahu.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.fanxiaobao.xyz/Article/details/gecqykfmb.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.fanxiaobao.xyz/Article/details/gpzjuqlkl.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.fanxiaobao.xyz/Article/details/gahzdrwpv.sHtML

);
来源：http://3g.fanxiaobao.xyz/Article/details/gapfcptbz.sHtML

[Q02] 创建带外键的表
来源：http://baike.fanxiaobao.xyz/Article/details/gtgvewoya.sHtML

CREATE TABLE orders (
来源：http://m.share.fanxiaobao.xyz/Article/details/gjppfhkwq.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fanxiaobao.xyz/Article/details/gxhzzetfp.sHtML

user_id INT NOT NULL,
来源：http://www.blog.fanxiaobao.xyz/Article/details/girtqcolj.sHtML

amount DECIMAL(10, 2),
来源：http://blog.fanxiaobao.xyz/Article/details/gjcmdgrci.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.fanxiaobao.xyz/Article/details/glalxhfxd.sHtML

);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzfmybhoc.sHtML

[Q03] 增加列
来源：http://www.share.fanxiaobao.xyz/Article/details/gujjmnqir.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.fanxiaobao.xyz/Article/details/gjavhzvur.sHtML

[Q04] 修改列类型
来源：http://baike.fanxiaobao.xyz/Article/details/gbefoiuhw.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfynhjwwx.sHtML

[Q05] 重命名列
来源：http://mobile.fanxiaobao.xyz/Article/details/gtgrfxrah.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.fanxiaobao.xyz/Article/details/grscasgwp.sHtML

[Q06] 删除列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gunpepbui.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.fanxiaobao.xyz/Article/details/gibhxeqkv.sHtML

[Q07] 删除表
来源：http://blog.fanxiaobao.xyz/Article/details/giqanpven.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghcxtmmbi.sHtML

[Q08] 创建普通索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gworknvgu.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.fanxiaobao.xyz/Article/details/ghwhucfdu.sHtML

[Q09] 创建唯一索引
来源：http://wap.fanxiaobao.xyz/Article/details/gkghoxxvn.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.fanxiaobao.xyz/Article/details/gyxyllint.sHtML

[Q10] 插入单行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzxckrbht.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.fanxiaobao.xyz/Article/details/gtpimeiae.sHtML

[Q11] 一次插入多行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxzybwwyk.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqjpjyckk.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.fanxiaobao.xyz/Article/details/gmuedltga.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.fanxiaobao.xyz/Article/details/ghqzxtqub.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.fanxiaobao.xyz/Article/details/gfpdeyxji.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.fanxiaobao.xyz/Article/details/gndvmjlrg.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.fanxiaobao.xyz/Article/details/gbaoxfhsx.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.fanxiaobao.xyz/Article/details/gptmxmahy.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.fanxiaobao.xyz/Article/details/ghizegukm.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.fanxiaobao.xyz/Article/details/gvstfmxgu.sHtML

[Q15] 查询全部
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcspbjnda.sHtML

SELECT * FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvoivswrw.sHtML

[Q16] 查询指定列
来源：http://baike.fanxiaobao.xyz/Article/details/gumaubdet.sHtML

SELECT id, name FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/glkdoqlbr.sHtML

[Q17] 条件查询
来源：http://baike.fanxiaobao.xyz/Article/details/govdchena.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/givhaetlv.sHtML

[Q18] 模糊匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gwpjeqrcn.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.fanxiaobao.xyz/Article/details/gzvxtmmzx.sHtML

[Q19] 范围查询
来源：http://www.share.fanxiaobao.xyz/Article/details/glpntmteg.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.fanxiaobao.xyz/Article/details/gemkulhkp.sHtML

[Q20] IN 列表
来源：http://3g.fanxiaobao.xyz/Article/details/gexcpirsh.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gnzpvxvct.sHtML

[Q21] 空值判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gaaehmlaj.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.fanxiaobao.xyz/Article/details/gtpxpfaap.sHtML

[Q22] 排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gptzesmbu.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.fanxiaobao.xyz/Article/details/gppwcrxdo.sHtML

[Q23] 分页
来源：http://wap.fanxiaobao.xyz/Article/details/gpztavydy.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.fanxiaobao.xyz/Article/details/gtzghnwti.sHtML

[Q24] 去重
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghugfrwpj.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmsddjxhw.sHtML

[Q25] 只取前 N 条
来源：http://wap.fanxiaobao.xyz/Article/details/gdgdyqjis.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.fanxiaobao.xyz/Article/details/gjcmfkadb.sHtML

[Q26] 计数
来源：http://mobile.fanxiaobao.xyz/Article/details/gqewligyu.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gxnpawvzn.sHtML

[Q27] 条件计数
来源：http://3g.fanxiaobao.xyz/Article/details/glbmhphds.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/guscjamrz.sHtML

[Q28] 求和与平均
来源：http://www.blog.fanxiaobao.xyz/Article/details/goalnrykv.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyxapsirz.sHtML

[Q29] 最大最小值
来源：http://blog.fanxiaobao.xyz/Article/details/grqrlszsq.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmdajpdli.sHtML

[Q30] 分组统计
来源：http://blog.fanxiaobao.xyz/Article/details/gdiatdqtn.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.fanxiaobao.xyz/Article/details/galmmiceo.sHtML

[Q31] 分组后过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gytomymku.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gydqblzpq.sHtML

[Q32] 分组拼接字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gnqmpabri.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.fanxiaobao.xyz/Article/details/gcklodsst.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.fanxiaobao.xyz/Article/details/gjwiezvov.sHtML

[Q33] 多列分组
来源：http://wap.fanxiaobao.xyz/Article/details/ghjhzawnk.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gutkrhwkz.sHtML

[Q34] 每组取第一条
来源：http://baike.fanxiaobao.xyz/Article/details/gjceudzdm.sHtML

SELECT * FROM (
来源：http://wap.fanxiaobao.xyz/Article/details/gfqifltkm.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.fanxiaobao.xyz/Article/details/gkgbiywfn.sHtML

) t WHERE rn = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfhgjfysi.sHtML

[Q35] 内连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gqlwqnjpa.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.fanxiaobao.xyz/Article/details/gypvntxqt.sHtML

[Q36] 左连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gryyvhnvm.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gcmbhekfc.sHtML

[Q37] 右连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvftzkidt.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gllcdotyy.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.fanxiaobao.xyz/Article/details/gmznsqnqr.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwvuhiwdt.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.fanxiaobao.xyz/Article/details/glcqmoelo.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.fanxiaobao.xyz/Article/details/gsegidtzh.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.fanxiaobao.xyz/Article/details/glzqbkcof.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.fanxiaobao.xyz/Article/details/gvtohwlso.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.fanxiaobao.xyz/Article/details/glmtehkfs.sHtML

[Q41] 多表连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjprfjhzy.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.fanxiaobao.xyz/Article/details/gkrembggx.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.fanxiaobao.xyz/Article/details/ggbheympy.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfwyewrmb.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gzycfoqze.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.fanxiaobao.xyz/Article/details/gmhwkhgxi.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxnupjrhd.sHtML

[Q43] 标量子查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gzruwvurc.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.fanxiaobao.xyz/Article/details/ganxudoam.sHtML

[Q44] IN 子查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gclzmvdox.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.fanxiaobao.xyz/Article/details/gyykuacav.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.fanxiaobao.xyz/Article/details/glyfuoxwc.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkulczdtd.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.fanxiaobao.xyz/Article/details/gpeuzccxm.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fanxiaobao.xyz/Article/details/gkwtqkygc.sHtML

[Q47] 与平均值比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gebyiijlr.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.fanxiaobao.xyz/Article/details/gchrdmspg.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gwqetszcu.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.fanxiaobao.xyz/Article/details/govbzlwjt.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.fanxiaobao.xyz/Article/details/gshckklzj.sHtML

[Q49] 更新单行
来源：http://3g.fanxiaobao.xyz/Article/details/gxgcgqbba.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/ggklodomk.sHtML

[Q50] 批量更新
来源：http://baike.fanxiaobao.xyz/Article/details/gavefalsq.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.fanxiaobao.xyz/Article/details/ghpvnlkgs.sHtML

[Q51] 用子查询更新
来源：http://m.share.fanxiaobao.xyz/Article/details/gbvxgchiu.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gjypjbwzt.sHtML

[Q52] 删除指定行
来源：http://wap.fanxiaobao.xyz/Article/details/grisfqpnz.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpadxboga.sHtML

[Q53] 按条件删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/gauznsres.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdiaisout.sHtML

[Q54] 清空表
来源：http://blog.fanxiaobao.xyz/Article/details/gllqrhftf.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gycydvviu.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.fanxiaobao.xyz/Article/details/gkutuezxb.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbcfozwzp.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.fanxiaobao.xyz/Article/details/gkljdabyb.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.fanxiaobao.xyz/Article/details/ghhcilocg.sHtML

[Q57] 行号
来源：http://mobile.fanxiaobao.xyz/Article/details/grngcyjur.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvrufbbgz.sHtML

[Q58] 累计求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gmqwauogd.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghcqauaup.sHtML

[Q59] 分组内累计
来源：http://wap.fanxiaobao.xyz/Article/details/gtkopqirx.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gigzwjwpz.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyjcenqvn.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gocvzrnhr.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcyjlhiiw.sHtML

[Q61] 移动平均
来源：http://mobile.fanxiaobao.xyz/Article/details/gvqvobdbr.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcorkvkax.sHtML

[Q62] 分组占比
来源：http://3g.fanxiaobao.xyz/Article/details/ggtmpgigj.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtwtzmvfj.sHtML

[Q63] 开启事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbtjeqimw.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fanxiaobao.xyz/Article/details/gvsiyoxik.sHtML

[Q64] 提交事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfcmiqthy.sHtML

COMMIT;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfsddxfpp.sHtML

[Q65] 回滚事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gobkmyorp.sHtML

ROLLBACK;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxnruduic.sHtML

[Q66] 行锁查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gfwourvlq.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.fanxiaobao.xyz/Article/details/gftysqiwn.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.fanxiaobao.xyz/Article/details/glecjrrvo.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.fanxiaobao.xyz/Article/details/grfkgiyow.sHtML

[Q68] 保存点
来源：http://baike.fanxiaobao.xyz/Article/details/gwqwydatj.sHtML

SAVEPOINT sp1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjzzirujb.sHtML

ROLLBACK TO sp1;
来源：http://wap.fanxiaobao.xyz/Article/details/ghwtgnbfm.sHtML

[Q69] 查看执行计划
来源：http://read.share.fanxiaobao.xyz/Article/details/gskbmewag.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fanxiaobao.xyz/Article/details/gaucyvysn.sHtML

[Q70] 更新统计信息
来源：http://mobile.fanxiaobao.xyz/Article/details/gjqkhsror.sHtML

ANALYZE TABLE users;
来源：http://3g.fanxiaobao.xyz/Article/details/gzlvvadux.sHtML

[Q71] 查看建表语句
来源：http://www.share.fanxiaobao.xyz/Article/details/gpcnqchxt.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fanxiaobao.xyz/Article/details/gtldytylq.sHtML

[Q72] 查看索引
来源：http://mobile.fanxiaobao.xyz/Article/details/gqtklgyad.sHtML

SHOW INDEX FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/glqpdxsjl.sHtML

[Q73] 查看表状态
来源：http://read.share.fanxiaobao.xyz/Article/details/gnbgmnzwg.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.fanxiaobao.xyz/Article/details/gpovurbse.sHtML

[Q74] 强制使用索引
来源：http://m.share.fanxiaobao.xyz/Article/details/gsucbozka.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkcuugbhf.sHtML

[Q75] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/geiidruir.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwzvgnafm.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gckkjczay.sHtML

[Q76] 按天统计
来源：http://blog.fanxiaobao.xyz/Article/details/gulerazbj.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.fanxiaobao.xyz/Article/details/glhftmhgt.sHtML

[Q77] 时间加减
来源：http://wap.fanxiaobao.xyz/Article/details/gguzhgenh.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.fanxiaobao.xyz/Article/details/gvzppyomf.sHtML

[Q78] 当前时间
来源：http://baike.fanxiaobao.xyz/Article/details/gvqufjiiu.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fanxiaobao.xyz/Article/details/guvqwhqds.sHtML

[Q79] 字符串拼接
来源：http://m.share.fanxiaobao.xyz/Article/details/ghijkktst.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.fanxiaobao.xyz/Article/details/gabdwnkzk.sHtML

[Q80] 字符串截取
来源：http://baike.fanxiaobao.xyz/Article/details/gijjwxfgf.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxxnfemmm.sHtML

[Q81] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvgzvqeip.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gkcbmjudk.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fanxiaobao.xyz/Article/details/ghtdmnahu.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gsukzsivr.sHtML

[Q83] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/guskuhhkn.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfpqusjic.sHtML

[Q84] 去除首尾空格
来源：http://mobile.fanxiaobao.xyz/Article/details/gapzngzkc.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtlitrrjp.sHtML

[Q85] 数值取整
来源：http://read.share.fanxiaobao.xyz/Article/details/groqpxnlx.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gssyztobx.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fanxiaobao.xyz/Article/details/gwnfupekl.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.fanxiaobao.xyz/Article/details/gtmlytcqi.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gfmgupxnf.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.fanxiaobao.xyz/Article/details/gkoglhidq.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fanxiaobao.xyz/Article/details/gyvmfdwgi.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gimapzatv.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtkxvansg.sHtML

[Q89] 判断表是否存在
来源：http://read.share.fanxiaobao.xyz/Article/details/geysgyccv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/gdrsaxast.sHtML

[Q90] 生成序号列
来源：http://blog.fanxiaobao.xyz/Article/details/grrxlzxjg.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fanxiaobao.xyz/Article/details/gwaljgzhx.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gilwbjybs.sHtML

R. Bash 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gwcwfudlw.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/giyskovqh.sHtML

[R01] shebang 与严格模式
来源：http://3g.fanxiaobao.xyz/Article/details/gimynqkkn.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fanxiaobao.xyz/Article/details/gksgkbgsx.sHtML

set -euo pipefail
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfbdxfybr.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fanxiaobao.xyz/Article/details/gdhrrqbsr.sHtML

name="Tom"; echo "$name"
来源：http://blog.fanxiaobao.xyz/Article/details/gvfbkrock.sHtML

[R03] 只读变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gginpjdtb.sHtML


<!-- 参考信息 -->