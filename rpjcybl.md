代发 wailian999

Py:   asyncio.gather(*tasks)
来源：http://3g.fehbvm.com/Article/details/gjtrhhxqm.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.zdbjq.cn/Article/details/gzotresvi.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.hesvh.cn/Article/details/gdwlvxocu.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.zdbjq.cn/Article/details/gtouqpapb.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.zdbjq.cn/Article/details/grkdtrptq.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.zdbjq.cn/Article/details/gbbeaadis.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.zdbjq.cn/Article/details/gxefcldmf.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.fehbvm.com/Article/details/gjrxjqyqb.sHtML

[O06] 使用进程池
来源：http://mobile.hesvh.cn/Article/details/gfuhnqvqk.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.fehbvm.com/Article/details/gjkmzwdqn.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.zdbjq.cn/Article/details/gbwntierq.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.zdbjq.cn/Article/details/gjviskwxo.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.zdbjq.cn/Article/details/gtrghdvnh.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.fehbvm.com/Article/details/gcmcsbrig.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.zdbjq.cn/Article/details/gxujnylsl.sHtML

Ruby: // fork 块
来源：http://www.blog.zdbjq.cn/Article/details/garqrjmyj.sHtML

C#:   Parallel.For
来源：http://read.share.zdbjq.cn/Article/details/gipujctqv.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gvwbcnpmq.sHtML

P. 常用工具函数
来源：http://read.share.hesvh.cn/Article/details/gqpqdngpt.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gmvugnunc.sHtML

[P01] 生成 UUID
来源：http://baike.hesvh.cn/Article/details/gmhucmlyw.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.hesvh.cn/Article/details/gqcujuzvx.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.hesvh.cn/Article/details/guhgbmyne.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gusdzvwbd.sHtML

TS:   crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/ggkwlswde.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.hesvh.cn/Article/details/gvvqxhmny.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.fehbvm.com/Article/details/gebiaadzc.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.fehbvm.com/Article/details/gfqrunwel.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.hesvh.cn/Article/details/gebqqmats.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.zdbjq.cn/Article/details/grntbrwci.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.hesvh.cn/Article/details/gfdmkgsub.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.zdbjq.cn/Article/details/gfwuxtsoo.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.fehbvm.com/Article/details/gylltbqfb.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.fehbvm.com/Article/details/gjxbkhxis.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.zdbjq.cn/Article/details/gksmpsijd.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.hesvh.cn/Article/details/gvyghowed.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.fehbvm.com/Article/details/gniterhbj.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.hesvh.cn/Article/details/gcztsxfhk.sHtML

[P03] 生成短随机字符串
来源：http://wap.fehbvm.com/Article/details/gtjxeapmv.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.zdbjq.cn/Article/details/glsulxcng.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.hesvh.cn/Article/details/gdcwhzkmr.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.hesvh.cn/Article/details/gfrrokbsc.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.zdbjq.cn/Article/details/gtkpkehxq.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.zdbjq.cn/Article/details/gruridtbj.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.zdbjq.cn/Article/details/gdjpcujoa.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.zdbjq.cn/Article/details/gfpnkbtaw.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.fehbvm.com/Article/details/gfyabcmmt.sHtML

[P04] 求长度
来源：http://m.share.hesvh.cn/Article/details/gbhvwpmvf.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.hesvh.cn/Article/details/glnidfsrp.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/ghbcpzfig.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.zdbjq.cn/Article/details/gcjuhzgkr.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.zdbjq.cn/Article/details/gvlxxneus.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.zdbjq.cn/Article/details/guumknnqr.sHtML

Go:   len(arr);  len(m)
来源：http://3g.fehbvm.com/Article/details/grxkwmwtw.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.fehbvm.com/Article/details/gnwwfsziv.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.zdbjq.cn/Article/details/glwofkvzi.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.hesvh.cn/Article/details/gfslgopke.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.fehbvm.com/Article/details/gefarodve.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.fehbvm.com/Article/details/goyffoksh.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.hesvh.cn/Article/details/gziamdiou.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.zdbjq.cn/Article/details/ghhdjqdcv.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.zdbjq.cn/Article/details/ghelswvez.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.fehbvm.com/Article/details/gyhcbumfv.sHtML

Ruby: a == b
来源：http://m.share.zdbjq.cn/Article/details/gayylezxi.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.hesvh.cn/Article/details/geqwlfyxm.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.zdbjq.cn/Article/details/gtqxavbkk.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.fehbvm.com/Article/details/gqdtsghoh.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.hesvh.cn/Article/details/gzxeubrea.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.zdbjq.cn/Article/details/gujevraha.sHtML

TS:   if (x == null) {}
来源：http://blog.zdbjq.cn/Article/details/gaujreert.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.hesvh.cn/Article/details/gbpgszzid.sHtML

Go:   if x == nil {}
来源：http://3g.zdbjq.cn/Article/details/glidpnbpc.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.hesvh.cn/Article/details/gsxtvyxqr.sHtML

C#:   if (x is null) {}
来源：http://wap.hesvh.cn/Article/details/gdomtdlxd.sHtML

[P07] 防抖与节流
来源：http://baike.zdbjq.cn/Article/details/gjcsuozgb.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.fehbvm.com/Article/details/gbsrdfokd.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.fehbvm.com/Article/details/gksecahca.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/gnojtodpd.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/gszyxgjty.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.fehbvm.com/Article/details/gpalkbmky.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.fehbvm.com/Article/details/gfynnlrhp.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.fehbvm.com/Article/details/gctktxyfo.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.fehbvm.com/Article/details/gffczvixq.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.fehbvm.com/Article/details/gmogexuvw.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.hesvh.cn/Article/details/gckhuwsvk.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.fehbvm.com/Article/details/gefzyldcn.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.fehbvm.com/Article/details/gdbhhflvu.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.hesvh.cn/Article/details/gbqbildxi.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.zdbjq.cn/Article/details/gaecowojb.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.fehbvm.com/Article/details/gmnhdufeu.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.fehbvm.com/Article/details/gydplbccu.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.hesvh.cn/Article/details/gwxmkclkp.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gsunzaopf.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.fehbvm.com/Article/details/gnnaihuij.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gtslogehh.sHtML

[Q01] 创建表
来源：http://wap.hesvh.cn/Article/details/gmolpbnyi.sHtML

CREATE TABLE users (
来源：http://m.share.hesvh.cn/Article/details/ggofvxkdv.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.hesvh.cn/Article/details/gwkfumjuv.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.fehbvm.com/Article/details/gzkpanolr.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.zdbjq.cn/Article/details/gsgqrefpm.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.hesvh.cn/Article/details/gqhgmyghv.sHtML

);
来源：http://www.m.share.zdbjq.cn/Article/details/gorqoafxk.sHtML

[Q02] 创建带外键的表
来源：http://read.share.hesvh.cn/Article/details/gbeghhozt.sHtML

CREATE TABLE orders (
来源：http://baike.fehbvm.com/Article/details/gxcbbwxbj.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fehbvm.com/Article/details/ghpvasjvx.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.zdbjq.cn/Article/details/ghncqhjlr.sHtML

amount DECIMAL(10, 2),
来源：http://wap.fehbvm.com/Article/details/gcsunicnh.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.zdbjq.cn/Article/details/gqogrgvob.sHtML

);
来源：http://read.share.hesvh.cn/Article/details/gvdqyjgwy.sHtML

[Q03] 增加列
来源：http://read.share.hesvh.cn/Article/details/gfihtczfs.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.hesvh.cn/Article/details/gmmzjhzbg.sHtML

[Q04] 修改列类型
来源：http://blog.hesvh.cn/Article/details/gexzgdxux.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.fehbvm.com/Article/details/gzmikiqgk.sHtML

[Q05] 重命名列
来源：http://blog.fehbvm.com/Article/details/gdpdduyek.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.fehbvm.com/Article/details/gowadshms.sHtML

[Q06] 删除列
来源：http://3g.fehbvm.com/Article/details/gopesknof.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.zdbjq.cn/Article/details/gytlvjukr.sHtML

[Q07] 删除表
来源：http://www.m.share.zdbjq.cn/Article/details/gepvksbaz.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.zdbjq.cn/Article/details/gcandtmvi.sHtML

[Q08] 创建普通索引
来源：http://baike.fehbvm.com/Article/details/gcylcypsa.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.hesvh.cn/Article/details/glvfqxren.sHtML

[Q09] 创建唯一索引
来源：http://read.share.fehbvm.com/Article/details/gmncsotxf.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.hesvh.cn/Article/details/gzidwjlax.sHtML

[Q10] 插入单行
来源：http://read.share.zdbjq.cn/Article/details/gxxcgbajj.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.zdbjq.cn/Article/details/glgceovsa.sHtML

[Q11] 一次插入多行
来源：http://www.blog.zdbjq.cn/Article/details/gtuzykxqv.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.fehbvm.com/Article/details/ggwnucndb.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.hesvh.cn/Article/details/grzcrkgwf.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.zdbjq.cn/Article/details/grmuvbjmi.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.fehbvm.com/Article/details/ghhiksjto.sHtML

[Q13] 忽略重复插入
来源：http://www.share.hesvh.cn/Article/details/gyhqwywpc.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.zdbjq.cn/Article/details/gtoygidxt.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.fehbvm.com/Article/details/gqjcyixyl.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.fehbvm.com/Article/details/glfkfqpzh.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.hesvh.cn/Article/details/gmufvmkrk.sHtML

[Q15] 查询全部
来源：http://baike.fehbvm.com/Article/details/gcobpkfxl.sHtML

SELECT * FROM users;
来源：http://read.share.hesvh.cn/Article/details/guaqfpobi.sHtML

[Q16] 查询指定列
来源：http://wap.fehbvm.com/Article/details/gexiapbpb.sHtML

SELECT id, name FROM users;
来源：http://blog.zdbjq.cn/Article/details/gchtofadd.sHtML

[Q17] 条件查询
来源：http://blog.zdbjq.cn/Article/details/gftnisnxk.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.zdbjq.cn/Article/details/ghkwxrvog.sHtML

[Q18] 模糊匹配
来源：http://read.share.fehbvm.com/Article/details/gsjfexzdk.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.zdbjq.cn/Article/details/gyplywlib.sHtML

[Q19] 范围查询
来源：http://wap.zdbjq.cn/Article/details/grfptoanr.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.fehbvm.com/Article/details/ggzjiello.sHtML

[Q20] IN 列表
来源：http://blog.zdbjq.cn/Article/details/gitcwnqix.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.hesvh.cn/Article/details/gonnvkcri.sHtML

[Q21] 空值判断
来源：http://baike.zdbjq.cn/Article/details/glmnyyant.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.fehbvm.com/Article/details/gsgmnsdbl.sHtML

[Q22] 排序
来源：http://www.share.fehbvm.com/Article/details/gwqpvitme.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.hesvh.cn/Article/details/grmtgvzrh.sHtML

[Q23] 分页
来源：http://www.m.share.fehbvm.com/Article/details/gopzrymsw.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.hesvh.cn/Article/details/gkgshlbmt.sHtML

[Q24] 去重
来源：http://www.share.fehbvm.com/Article/details/ghykzdjvh.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.hesvh.cn/Article/details/gbbjhisgf.sHtML

[Q25] 只取前 N 条
来源：http://blog.fehbvm.com/Article/details/gitivxjad.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.fehbvm.com/Article/details/gibsnobcz.sHtML

[Q26] 计数
来源：http://www.share.hesvh.cn/Article/details/gawyrgioc.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.fehbvm.com/Article/details/ggekzqpvk.sHtML

[Q27] 条件计数
来源：http://wap.fehbvm.com/Article/details/gmwwdccjy.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gwjjjahtg.sHtML

[Q28] 求和与平均
来源：http://mobile.hesvh.cn/Article/details/gcxejavcv.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/ghjqddvex.sHtML

[Q29] 最大最小值
来源：http://blog.zdbjq.cn/Article/details/gxvvbjynh.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gkryxogzp.sHtML

[Q30] 分组统计
来源：http://mobile.zdbjq.cn/Article/details/gckckjwdb.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/gdvbqidna.sHtML

[Q31] 分组后过滤
来源：http://read.share.zdbjq.cn/Article/details/govrglalr.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.fehbvm.com/Article/details/gztfgyrqz.sHtML

[Q32] 分组拼接字符串
来源：http://3g.zdbjq.cn/Article/details/ghkmyprds.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/gvbkfuwwc.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.hesvh.cn/Article/details/gdvloizqm.sHtML

[Q33] 多列分组
来源：http://www.blog.fehbvm.com/Article/details/gaondeayq.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.zdbjq.cn/Article/details/gzxkbgdat.sHtML

[Q34] 每组取第一条
来源：http://www.blog.zdbjq.cn/Article/details/gkjddlkmy.sHtML

SELECT * FROM (
来源：http://3g.fehbvm.com/Article/details/gnvpbwcrn.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.hesvh.cn/Article/details/gyiytasxb.sHtML

) t WHERE rn = 1;
来源：http://wap.fehbvm.com/Article/details/gqlbwaqwp.sHtML

[Q35] 内连接
来源：http://read.share.fehbvm.com/Article/details/gphzbtlzb.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.zdbjq.cn/Article/details/gbatmqaew.sHtML

[Q36] 左连接
来源：http://mobile.fehbvm.com/Article/details/gpjqswgvg.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.zdbjq.cn/Article/details/gumtmipxk.sHtML

[Q37] 右连接
来源：http://wap.hesvh.cn/Article/details/ggbqefxrx.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.hesvh.cn/Article/details/gmovgjpee.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.fehbvm.com/Article/details/gakondque.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.fehbvm.com/Article/details/gfkyuwqbo.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.zdbjq.cn/Article/details/gywyfpiel.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.hesvh.cn/Article/details/gwuuwqeca.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.zdbjq.cn/Article/details/ghilfsrhj.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.fehbvm.com/Article/details/ggxiidsdd.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.fehbvm.com/Article/details/gluowxshk.sHtML

[Q41] 多表连接
来源：http://www.blog.zdbjq.cn/Article/details/gfihnheyv.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.fehbvm.com/Article/details/gqhhpbuxf.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.hesvh.cn/Article/details/gxxejcdny.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.fehbvm.com/Article/details/gxkgkeipu.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.hesvh.cn/Article/details/gxozfgugm.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.fehbvm.com/Article/details/gvqnjwrel.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.fehbvm.com/Article/details/gwytfdqxk.sHtML

[Q43] 标量子查询
来源：http://www.blog.fehbvm.com/Article/details/gcfnnuuba.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.hesvh.cn/Article/details/gxiclagnw.sHtML

[Q44] IN 子查询
来源：http://read.share.hesvh.cn/Article/details/gjaticimc.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.zdbjq.cn/Article/details/gdkaohspl.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.zdbjq.cn/Article/details/grjmmhukl.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.hesvh.cn/Article/details/gstdvwvlx.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.hesvh.cn/Article/details/gxtoknocf.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.zdbjq.cn/Article/details/goybapnwr.sHtML

[Q47] 与平均值比较
来源：http://mobile.zdbjq.cn/Article/details/glnflfhlh.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.hesvh.cn/Article/details/gyzcbcqll.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gqnrukgry.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.zdbjq.cn/Article/details/glbfdauok.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.fehbvm.com/Article/details/gpcprwpti.sHtML

[Q49] 更新单行
来源：http://baike.fehbvm.com/Article/details/gpsetoyqa.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.hesvh.cn/Article/details/glntedsms.sHtML

[Q50] 批量更新
来源：http://www.m.share.hesvh.cn/Article/details/gfzufustn.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.fehbvm.com/Article/details/ghqwzymcy.sHtML

[Q51] 用子查询更新
来源：http://baike.hesvh.cn/Article/details/gzddiwcay.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.zdbjq.cn/Article/details/gvksweyfk.sHtML

[Q52] 删除指定行
来源：http://blog.zdbjq.cn/Article/details/gozeqdwgr.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.zdbjq.cn/Article/details/gxvggijoe.sHtML

[Q53] 按条件删除
来源：http://wap.hesvh.cn/Article/details/gglugevjy.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fehbvm.com/Article/details/gzuarpmuu.sHtML

[Q54] 清空表
来源：http://wap.zdbjq.cn/Article/details/gfdvwxpcb.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fehbvm.com/Article/details/gcmeednui.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.zdbjq.cn/Article/details/gejeswipw.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.hesvh.cn/Article/details/gpzkghbbu.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.hesvh.cn/Article/details/gzhibygsq.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.fehbvm.com/Article/details/gbyrybwbw.sHtML

[Q57] 行号
来源：http://m.share.fehbvm.com/Article/details/guqpheixk.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.zdbjq.cn/Article/details/gdguhyzne.sHtML

[Q58] 累计求和
来源：http://www.share.fehbvm.com/Article/details/gzvzjfumx.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gouwseqro.sHtML

[Q59] 分组内累计
来源：http://read.share.hesvh.cn/Article/details/gbkqihazs.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gpfrtceto.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.zdbjq.cn/Article/details/ghhsxvpkr.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.zdbjq.cn/Article/details/gqljbidct.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gsogtyaey.sHtML

[Q61] 移动平均
来源：http://baike.hesvh.cn/Article/details/gpxyopzct.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gmghfmdyg.sHtML

[Q62] 分组占比
来源：http://www.m.share.zdbjq.cn/Article/details/ggoeqlcts.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/gneppwhay.sHtML

[Q63] 开启事务
来源：http://m.share.zdbjq.cn/Article/details/gcnhuwcjy.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.hesvh.cn/Article/details/gkbauuokh.sHtML

[Q64] 提交事务
来源：http://www.share.fehbvm.com/Article/details/glsyqiksk.sHtML

COMMIT;
来源：http://www.blog.hesvh.cn/Article/details/gzjuajpmq.sHtML

[Q65] 回滚事务
来源：http://mobile.hesvh.cn/Article/details/gwpxigmji.sHtML

ROLLBACK;
来源：http://baike.fehbvm.com/Article/details/gpvjcmmyq.sHtML

[Q66] 行锁查询
来源：http://www.share.fehbvm.com/Article/details/gpsulrvtz.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.zdbjq.cn/Article/details/gepjvtbld.sHtML

[Q67] 设置隔离级别
来源：http://www.share.zdbjq.cn/Article/details/gkhmktaba.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.zdbjq.cn/Article/details/gmqmjyjdz.sHtML

[Q68] 保存点
来源：http://3g.fehbvm.com/Article/details/goiavqljq.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.hesvh.cn/Article/details/gdxybjxxx.sHtML

ROLLBACK TO sp1;
来源：http://baike.fehbvm.com/Article/details/gfntsqxqt.sHtML

[Q69] 查看执行计划
来源：http://read.share.zdbjq.cn/Article/details/gsskanjib.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.hesvh.cn/Article/details/gzhjjxdcl.sHtML

[Q70] 更新统计信息
来源：http://baike.zdbjq.cn/Article/details/gnvmkhedw.sHtML

ANALYZE TABLE users;
来源：http://3g.fehbvm.com/Article/details/gjskcomkn.sHtML

[Q71] 查看建表语句
来源：http://m.share.zdbjq.cn/Article/details/ggpbyspuj.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.fehbvm.com/Article/details/gnwsrdovk.sHtML

[Q72] 查看索引
来源：http://3g.hesvh.cn/Article/details/ghvptjbio.sHtML

SHOW INDEX FROM users;
来源：http://m.share.hesvh.cn/Article/details/gxtxtildi.sHtML

[Q73] 查看表状态
来源：http://mobile.zdbjq.cn/Article/details/gjifmfqoc.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.hesvh.cn/Article/details/gsdqdpwsu.sHtML

[Q74] 强制使用索引
来源：http://wap.zdbjq.cn/Article/details/gstfxbnab.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fehbvm.com/Article/details/gdxnrnbby.sHtML

[Q75] 日期格式化
来源：http://www.share.hesvh.cn/Article/details/gbqpgbfhu.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gkmntqfwf.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fehbvm.com/Article/details/gpxznhqxu.sHtML

[Q76] 按天统计
来源：http://www.m.share.hesvh.cn/Article/details/ggzpdiwxo.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.fehbvm.com/Article/details/grljyvdpg.sHtML

[Q77] 时间加减
来源：http://blog.fehbvm.com/Article/details/gfmtgsnvz.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fehbvm.com/Article/details/gnikhgujf.sHtML

[Q78] 当前时间
来源：http://3g.fehbvm.com/Article/details/gerpqodce.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.hesvh.cn/Article/details/gkcjwixot.sHtML

[Q79] 字符串拼接
来源：http://www.share.zdbjq.cn/Article/details/gngggfgwb.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.fehbvm.com/Article/details/givejuucb.sHtML

[Q80] 字符串截取
来源：http://blog.fehbvm.com/Article/details/gshzsctca.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gitrsbelq.sHtML

[Q81] 字符串替换
来源：http://m.share.hesvh.cn/Article/details/gsvfsxdfy.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fehbvm.com/Article/details/grwkoafap.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fehbvm.com/Article/details/ghzibarry.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/goixohbii.sHtML

[Q83] 大小写转换
来源：http://m.share.zdbjq.cn/Article/details/gltcjljli.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gggaqozax.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fehbvm.com/Article/details/gfxsqdraq.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gfccdunsf.sHtML

[Q85] 数值取整
来源：http://baike.fehbvm.com/Article/details/gjsjbgfeq.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.hesvh.cn/Article/details/gpvwrpkro.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fehbvm.com/Article/details/gtdykjrsc.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.hesvh.cn/Article/details/gxfzmgqcf.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.hesvh.cn/Article/details/gvjsnxhcz.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.zdbjq.cn/Article/details/gnvlnlbcy.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.hesvh.cn/Article/details/gdosctsat.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fehbvm.com/Article/details/guuohxcsi.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gkcyxswjq.sHtML

[Q89] 判断表是否存在
来源：http://mobile.fehbvm.com/Article/details/gkkvrfjvo.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.hesvh.cn/Article/details/gsmxwhzsj.sHtML

[Q90] 生成序号列
来源：http://3g.fehbvm.com/Article/details/gyurjtusx.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.hesvh.cn/Article/details/gaduisqom.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gsayxseuh.sHtML


<!-- 参考信息 -->