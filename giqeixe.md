代发 wailian999

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.zdbjq.cn/Article/details/gdptovhgv.sHtML

JS:   async function f() { await g(); }
来源：http://baike.fehbvm.com/Article/details/gextahwwc.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gqggstvai.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.zdbjq.cn/Article/details/goktnievk.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.hesvh.cn/Article/details/gxntbpjlp.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.fehbvm.com/Article/details/gssodrkil.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.hesvh.cn/Article/details/gynexyhrp.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.fehbvm.com/Article/details/gfprppnag.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.zdbjq.cn/Article/details/ggefnlxtg.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.fehbvm.com/Article/details/ghthtkpru.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/gybvxdzow.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.fehbvm.com/Article/details/gfpdqymzf.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.zdbjq.cn/Article/details/gppkkrvfy.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.zdbjq.cn/Article/details/gbkmfvnsw.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.fehbvm.com/Article/details/gbmalahiz.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.fehbvm.com/Article/details/gmmpecatp.sHtML

[O06] 使用进程池
来源：http://baike.fehbvm.com/Article/details/glowxdxzp.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.hesvh.cn/Article/details/gcyslggvj.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.fehbvm.com/Article/details/gllqrsihs.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.hesvh.cn/Article/details/gwuwcybxw.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.fehbvm.com/Article/details/gpyaolihg.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.hesvh.cn/Article/details/gyrsyzhhq.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.fehbvm.com/Article/details/ggobhtcsp.sHtML

Ruby: // fork 块
来源：http://read.share.hesvh.cn/Article/details/ggucrmrnk.sHtML

C#:   Parallel.For
来源：http://m.share.hesvh.cn/Article/details/gdkhjvoco.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/glqzwmkfp.sHtML

P. 常用工具函数
来源：http://baike.zdbjq.cn/Article/details/gvpksmqis.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gyoetszri.sHtML

[P01] 生成 UUID
来源：http://www.m.share.fehbvm.com/Article/details/gkxdrwgvi.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.hesvh.cn/Article/details/gonziskfy.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.hesvh.cn/Article/details/gjzfxlsgq.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gdjehjdcw.sHtML

TS:   crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gwbvorkeb.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.zdbjq.cn/Article/details/gexpkmftq.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.hesvh.cn/Article/details/gajehrbbt.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.hesvh.cn/Article/details/gqyltpkgs.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.zdbjq.cn/Article/details/ggfsmtije.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.hesvh.cn/Article/details/gprgyboim.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.zdbjq.cn/Article/details/gfizggncb.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.hesvh.cn/Article/details/gfixepoym.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.hesvh.cn/Article/details/grofektib.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.hesvh.cn/Article/details/ggxquvell.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.zdbjq.cn/Article/details/gmfkyfhdr.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.fehbvm.com/Article/details/gwhpfnqrq.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.zdbjq.cn/Article/details/gqupkhulc.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.zdbjq.cn/Article/details/gzgaazrrp.sHtML

[P03] 生成短随机字符串
来源：http://blog.hesvh.cn/Article/details/gqubzokjg.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.fehbvm.com/Article/details/gzavsqcqc.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.fehbvm.com/Article/details/grfnyihrj.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fehbvm.com/Article/details/gaqfxdkhx.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.zdbjq.cn/Article/details/glzczklqe.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.hesvh.cn/Article/details/gzfabjmlo.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.zdbjq.cn/Article/details/glcwkvrfm.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.zdbjq.cn/Article/details/ggooigpce.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.fehbvm.com/Article/details/gxldfonab.sHtML

[P04] 求长度
来源：http://www.share.hesvh.cn/Article/details/gcwvmyjku.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.fehbvm.com/Article/details/gwpcmqycd.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gvgjamwwg.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fehbvm.com/Article/details/ggjflkhft.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fehbvm.com/Article/details/gpogwynjd.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.zdbjq.cn/Article/details/gzfcansbj.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.fehbvm.com/Article/details/ggswlznpf.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.zdbjq.cn/Article/details/gfmbgomhu.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.zdbjq.cn/Article/details/gokoxyuvv.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.fehbvm.com/Article/details/gimwdynfl.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.fehbvm.com/Article/details/gliqjhend.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.fehbvm.com/Article/details/ghwxcieih.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.fehbvm.com/Article/details/gtyknymkd.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.zdbjq.cn/Article/details/grmtmexda.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.hesvh.cn/Article/details/gbrlsdtnj.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.hesvh.cn/Article/details/gbidyszum.sHtML

Ruby: a == b
来源：http://mobile.hesvh.cn/Article/details/gkvcoiclp.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.hesvh.cn/Article/details/gugmvvhzd.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.zdbjq.cn/Article/details/gkwjrsybj.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.fehbvm.com/Article/details/gilchfbac.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.hesvh.cn/Article/details/gsbbqzeau.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.zdbjq.cn/Article/details/gcnoazaxn.sHtML

TS:   if (x == null) {}
来源：http://read.share.zdbjq.cn/Article/details/gewrjeuij.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.fehbvm.com/Article/details/gzfodapzn.sHtML

Go:   if x == nil {}
来源：http://www.share.fehbvm.com/Article/details/gkwpxdypg.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.hesvh.cn/Article/details/gcajijlit.sHtML

C#:   if (x is null) {}
来源：http://baike.fehbvm.com/Article/details/gdwwghdgl.sHtML

[P07] 防抖与节流
来源：http://read.share.hesvh.cn/Article/details/grrommidp.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.fehbvm.com/Article/details/gyvhauofk.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.zdbjq.cn/Article/details/gmbhhpfhx.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/gbwemyhqz.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/gtjfurjsv.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.fehbvm.com/Article/details/geweioldy.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.hesvh.cn/Article/details/glxzbwsyy.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.zdbjq.cn/Article/details/gevlgsrpf.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.zdbjq.cn/Article/details/gsdvelhxn.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.zdbjq.cn/Article/details/gthgjmxwh.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.fehbvm.com/Article/details/grmicyhbr.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.fehbvm.com/Article/details/gdpjezcyt.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.zdbjq.cn/Article/details/gcqbduotb.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.zdbjq.cn/Article/details/ggviibsls.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.hesvh.cn/Article/details/gnghtzktw.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.zdbjq.cn/Article/details/gnztsfbzw.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.hesvh.cn/Article/details/gkfiuruht.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.fehbvm.com/Article/details/ggubqgkke.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gnvlaqrhf.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.fehbvm.com/Article/details/ggyzwmyrc.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gtzeppyhb.sHtML

[Q01] 创建表
来源：http://wap.zdbjq.cn/Article/details/gfxgokhdq.sHtML

CREATE TABLE users (
来源：http://www.m.share.zdbjq.cn/Article/details/govmhrish.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.hesvh.cn/Article/details/gbhhvfflx.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.fehbvm.com/Article/details/gznrizkfm.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.fehbvm.com/Article/details/gurgyvzlc.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.hesvh.cn/Article/details/gwjlklqcp.sHtML

);
来源：http://wap.fehbvm.com/Article/details/giscftfar.sHtML

[Q02] 创建带外键的表
来源：http://wap.hesvh.cn/Article/details/geeyuayai.sHtML

CREATE TABLE orders (
来源：http://baike.fehbvm.com/Article/details/gwbvoizac.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.zdbjq.cn/Article/details/gzofnbwwn.sHtML

user_id INT NOT NULL,
来源：http://wap.zdbjq.cn/Article/details/guvsrfuyf.sHtML

amount DECIMAL(10, 2),
来源：http://3g.hesvh.cn/Article/details/gqxbrqwuc.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.fehbvm.com/Article/details/gsdtgcpkb.sHtML

);
来源：http://baike.hesvh.cn/Article/details/gkepwuxyq.sHtML

[Q03] 增加列
来源：http://baike.hesvh.cn/Article/details/gcsbyvjpa.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.fehbvm.com/Article/details/gxkwfgsrb.sHtML

[Q04] 修改列类型
来源：http://www.share.fehbvm.com/Article/details/gbabxhhpj.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.fehbvm.com/Article/details/gtnbhthso.sHtML

[Q05] 重命名列
来源：http://www.blog.hesvh.cn/Article/details/gjyrfgwie.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.hesvh.cn/Article/details/gpipeaukp.sHtML

[Q06] 删除列
来源：http://www.share.hesvh.cn/Article/details/gnljiggyx.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.fehbvm.com/Article/details/gofaieloz.sHtML

[Q07] 删除表
来源：http://3g.fehbvm.com/Article/details/gwzibawij.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.hesvh.cn/Article/details/ggcgwvnes.sHtML

[Q08] 创建普通索引
来源：http://baike.hesvh.cn/Article/details/gsndhbwzr.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.hesvh.cn/Article/details/gxjsdlkcx.sHtML

[Q09] 创建唯一索引
来源：http://read.share.fehbvm.com/Article/details/ghkouafbw.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.hesvh.cn/Article/details/gehhgvnmb.sHtML

[Q10] 插入单行
来源：http://baike.zdbjq.cn/Article/details/gowvbsnwo.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.zdbjq.cn/Article/details/gewnfooxr.sHtML

[Q11] 一次插入多行
来源：http://3g.zdbjq.cn/Article/details/gcerksepo.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.zdbjq.cn/Article/details/gagmdrsts.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.zdbjq.cn/Article/details/gehgtznrx.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.fehbvm.com/Article/details/gxmgewyia.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.zdbjq.cn/Article/details/gntvalhjl.sHtML

[Q13] 忽略重复插入
来源：http://wap.zdbjq.cn/Article/details/gymtdzvrh.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gtknaxlxr.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.fehbvm.com/Article/details/gnmjbvaak.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.hesvh.cn/Article/details/gkmmnfcji.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.hesvh.cn/Article/details/giglhleic.sHtML

[Q15] 查询全部
来源：http://blog.zdbjq.cn/Article/details/gfkdmaynq.sHtML

SELECT * FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gdstzpzcv.sHtML

[Q16] 查询指定列
来源：http://www.share.zdbjq.cn/Article/details/gwltjpfvm.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/getqkjqtf.sHtML

[Q17] 条件查询
来源：http://3g.fehbvm.com/Article/details/gguiwytie.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gnhvbwbpu.sHtML

[Q18] 模糊匹配
来源：http://wap.hesvh.cn/Article/details/gotvfkpqq.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.fehbvm.com/Article/details/guxdnxtid.sHtML

[Q19] 范围查询
来源：http://blog.fehbvm.com/Article/details/gbkvqwihx.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.fehbvm.com/Article/details/gklzudvtt.sHtML

[Q20] IN 列表
来源：http://wap.fehbvm.com/Article/details/gpiqzrwrp.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.zdbjq.cn/Article/details/gqnezolxy.sHtML

[Q21] 空值判断
来源：http://3g.fehbvm.com/Article/details/gwiyexkcg.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.hesvh.cn/Article/details/gohhsiubp.sHtML

[Q22] 排序
来源：http://www.share.zdbjq.cn/Article/details/gkjgiwisy.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.hesvh.cn/Article/details/gehhcvnhk.sHtML

[Q23] 分页
来源：http://www.blog.zdbjq.cn/Article/details/gibqjsygh.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.fehbvm.com/Article/details/gsdzqlnqz.sHtML

[Q24] 去重
来源：http://3g.zdbjq.cn/Article/details/gdhhiffxt.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.fehbvm.com/Article/details/gbikkwnnx.sHtML

[Q25] 只取前 N 条
来源：http://m.share.fehbvm.com/Article/details/gclhnfxmd.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.hesvh.cn/Article/details/gyknthkaq.sHtML

[Q26] 计数
来源：http://www.m.share.fehbvm.com/Article/details/gsszmxyvp.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gmzbavrot.sHtML

[Q27] 条件计数
来源：http://m.share.zdbjq.cn/Article/details/gjfiskuqi.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.fehbvm.com/Article/details/gokooppsr.sHtML

[Q28] 求和与平均
来源：http://wap.zdbjq.cn/Article/details/gvgkokdjf.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/ghqmzbpaf.sHtML

[Q29] 最大最小值
来源：http://m.share.hesvh.cn/Article/details/gxjekabuo.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gyywjacke.sHtML

[Q30] 分组统计
来源：http://3g.fehbvm.com/Article/details/gyyqwbchw.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/gajnmycbr.sHtML

[Q31] 分组后过滤
来源：http://blog.hesvh.cn/Article/details/gbaqdvvys.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.zdbjq.cn/Article/details/gswvwdkri.sHtML

[Q32] 分组拼接字符串
来源：http://3g.hesvh.cn/Article/details/gkkdskaoa.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gvtyitsas.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.fehbvm.com/Article/details/gcdettdzq.sHtML

[Q33] 多列分组
来源：http://blog.fehbvm.com/Article/details/goiwenocc.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.zdbjq.cn/Article/details/gkndwdjnb.sHtML

[Q34] 每组取第一条
来源：http://mobile.zdbjq.cn/Article/details/gedqmnkli.sHtML

SELECT * FROM (
来源：http://blog.fehbvm.com/Article/details/gecorjwvs.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.hesvh.cn/Article/details/gwhzcwzzs.sHtML

) t WHERE rn = 1;
来源：http://m.share.zdbjq.cn/Article/details/gituxldpp.sHtML

[Q35] 内连接
来源：http://www.blog.zdbjq.cn/Article/details/gduyxeznq.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.zdbjq.cn/Article/details/gfsobhaoq.sHtML

[Q36] 左连接
来源：http://blog.fehbvm.com/Article/details/gyeokcais.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.fehbvm.com/Article/details/gblueiboe.sHtML

[Q37] 右连接
来源：http://mobile.hesvh.cn/Article/details/gynoggzcj.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.fehbvm.com/Article/details/glgmxfktv.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.fehbvm.com/Article/details/guwuzqmty.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.hesvh.cn/Article/details/gnhekwjgq.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.zdbjq.cn/Article/details/gxymmlvpe.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.hesvh.cn/Article/details/gsngixcil.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.fehbvm.com/Article/details/grkznokip.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.zdbjq.cn/Article/details/gpmwwkucj.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.fehbvm.com/Article/details/gwkcwghsn.sHtML

[Q41] 多表连接
来源：http://baike.zdbjq.cn/Article/details/guccanpze.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.fehbvm.com/Article/details/gkonwjuar.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.hesvh.cn/Article/details/giezjeayw.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.hesvh.cn/Article/details/gfitbvqac.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.zdbjq.cn/Article/details/gwuvosdnc.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.fehbvm.com/Article/details/gocxpzeax.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.hesvh.cn/Article/details/gkgttynav.sHtML

[Q43] 标量子查询
来源：http://www.share.fehbvm.com/Article/details/gjgpllswy.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.fehbvm.com/Article/details/gbivwnhui.sHtML

[Q44] IN 子查询
来源：http://mobile.fehbvm.com/Article/details/gkhxzdvra.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.hesvh.cn/Article/details/gvzcauvnr.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.zdbjq.cn/Article/details/gzhqwpnly.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.zdbjq.cn/Article/details/ghlgqrikg.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.hesvh.cn/Article/details/gpqswjciy.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fehbvm.com/Article/details/gckmnknat.sHtML

[Q47] 与平均值比较
来源：http://www.blog.zdbjq.cn/Article/details/gyautgiib.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.hesvh.cn/Article/details/gcgxvwdrq.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.fehbvm.com/Article/details/gfyzdhcmz.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.fehbvm.com/Article/details/glmnkiqov.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.zdbjq.cn/Article/details/goadpjmoy.sHtML

[Q49] 更新单行
来源：http://baike.zdbjq.cn/Article/details/grtwdpelw.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.hesvh.cn/Article/details/gbrzlffui.sHtML

[Q50] 批量更新
来源：http://3g.hesvh.cn/Article/details/gesbvtxpe.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.hesvh.cn/Article/details/gkvzhrddn.sHtML

[Q51] 用子查询更新
来源：http://3g.hesvh.cn/Article/details/gkzdntwdx.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.hesvh.cn/Article/details/guwzlgovv.sHtML

[Q52] 删除指定行
来源：http://www.m.share.fehbvm.com/Article/details/ghmcvtzsl.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/ggatvpogx.sHtML

[Q53] 按条件删除
来源：http://www.share.fehbvm.com/Article/details/gxbwhfszg.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.hesvh.cn/Article/details/gjmzyztea.sHtML

[Q54] 清空表
来源：http://m.share.zdbjq.cn/Article/details/gqigsojhb.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.zdbjq.cn/Article/details/gbbyhwzwf.sHtML

[Q55] 排名（并列占位）
来源：http://3g.fehbvm.com/Article/details/ggonumsfq.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.fehbvm.com/Article/details/grtahonpe.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.fehbvm.com/Article/details/ggxhgvyxx.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.fehbvm.com/Article/details/gtkzlgnea.sHtML

[Q57] 行号
来源：http://www.m.share.fehbvm.com/Article/details/garrbakwo.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.fehbvm.com/Article/details/giijfqaou.sHtML

[Q58] 累计求和
来源：http://www.share.zdbjq.cn/Article/details/gavgwyonw.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.hesvh.cn/Article/details/gcakftlwn.sHtML

[Q59] 分组内累计
来源：http://blog.zdbjq.cn/Article/details/gemwdpdrp.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/ggbjfsykr.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.fehbvm.com/Article/details/gtlftmjry.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.zdbjq.cn/Article/details/glekaequb.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gjxuxqhvh.sHtML

[Q61] 移动平均
来源：http://www.share.hesvh.cn/Article/details/gvnxuwmxg.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gekfehfaf.sHtML

[Q62] 分组占比
来源：http://www.share.zdbjq.cn/Article/details/gdvtxudkg.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/gvwqkvydh.sHtML

[Q63] 开启事务
来源：http://wap.hesvh.cn/Article/details/gvfwgqsrd.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.zdbjq.cn/Article/details/gwzoeofce.sHtML

[Q64] 提交事务
来源：http://www.m.share.hesvh.cn/Article/details/gllojitzv.sHtML

COMMIT;
来源：http://3g.hesvh.cn/Article/details/gkzkcaemr.sHtML

[Q65] 回滚事务
来源：http://blog.hesvh.cn/Article/details/gmekdztsz.sHtML

ROLLBACK;
来源：http://blog.fehbvm.com/Article/details/gqrrjtnis.sHtML

[Q66] 行锁查询
来源：http://3g.zdbjq.cn/Article/details/gjjojhogn.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.fehbvm.com/Article/details/gnbivwwax.sHtML

[Q67] 设置隔离级别
来源：http://baike.fehbvm.com/Article/details/gdotonmlx.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.hesvh.cn/Article/details/gbihdcaai.sHtML

[Q68] 保存点
来源：http://wap.zdbjq.cn/Article/details/ghguvlaht.sHtML

SAVEPOINT sp1;
来源：http://mobile.zdbjq.cn/Article/details/geyoxhhqy.sHtML

ROLLBACK TO sp1;
来源：http://baike.fehbvm.com/Article/details/gxpfhkqzj.sHtML

[Q69] 查看执行计划
来源：http://m.share.fehbvm.com/Article/details/gdmsmqrag.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.zdbjq.cn/Article/details/gtvknrvjf.sHtML

[Q70] 更新统计信息
来源：http://3g.hesvh.cn/Article/details/gwvlfyweb.sHtML

ANALYZE TABLE users;
来源：http://baike.hesvh.cn/Article/details/gdgbszxun.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.zdbjq.cn/Article/details/gylstyuaf.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.zdbjq.cn/Article/details/gkmhanybe.sHtML

[Q72] 查看索引
来源：http://m.share.zdbjq.cn/Article/details/gzhjrbvwp.sHtML

SHOW INDEX FROM users;
来源：http://wap.zdbjq.cn/Article/details/grbawhlna.sHtML

[Q73] 查看表状态
来源：http://baike.hesvh.cn/Article/details/gizjxqgft.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.fehbvm.com/Article/details/gpnyihuzp.sHtML

[Q74] 强制使用索引
来源：http://mobile.fehbvm.com/Article/details/guanimwul.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.zdbjq.cn/Article/details/gsfcokmsq.sHtML

[Q75] 日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gzuvjzfmb.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gwcjuosxy.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fehbvm.com/Article/details/gkuuouvor.sHtML

[Q76] 按天统计
来源：http://3g.fehbvm.com/Article/details/gffmvlssx.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.hesvh.cn/Article/details/ghqyestes.sHtML

[Q77] 时间加减
来源：http://www.m.share.hesvh.cn/Article/details/gfrnruegv.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fehbvm.com/Article/details/gyuhavgpf.sHtML

[Q78] 当前时间
来源：http://3g.zdbjq.cn/Article/details/geatqubro.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.zdbjq.cn/Article/details/grfsoespn.sHtML

[Q79] 字符串拼接
来源：http://3g.hesvh.cn/Article/details/grqsrtppp.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.hesvh.cn/Article/details/gcnfwsioz.sHtML

[Q80] 字符串截取
来源：http://wap.zdbjq.cn/Article/details/grlehavgv.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gkcztnqfq.sHtML

[Q81] 字符串替换
来源：http://www.blog.zdbjq.cn/Article/details/gobfyyouu.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gjnluvhjt.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.fehbvm.com/Article/details/gqjaruafe.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gyeyckqcp.sHtML

[Q83] 大小写转换
来源：http://baike.zdbjq.cn/Article/details/ggchayevd.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gwuuxhnfb.sHtML

[Q84] 去除首尾空格
来源：http://mobile.zdbjq.cn/Article/details/guteggczc.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gocffoplg.sHtML

[Q85] 数值取整
来源：http://wap.hesvh.cn/Article/details/gcgtgmcha.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.zdbjq.cn/Article/details/ggxdvpfaf.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.hesvh.cn/Article/details/gflzltfxi.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.zdbjq.cn/Article/details/gifxbglgg.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.zdbjq.cn/Article/details/gmmkgmbor.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.hesvh.cn/Article/details/gcxuhqyrp.sHtML


<!-- 参考信息 -->