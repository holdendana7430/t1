代发 wailian999

TS:   // worker_threads 线程池
来源：http://www.blog.fehbvm.com/Article/details/gpevzgplc.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.fehbvm.com/Article/details/giqfroyqq.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.hesvh.cn/Article/details/gpogfrxwj.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.zdbjq.cn/Article/details/gnopjlcfl.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.fehbvm.com/Article/details/gjnvsguct.sHtML

[O03] 加锁保护共享数据
来源：http://blog.hesvh.cn/Article/details/gafugnhcw.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.zdbjq.cn/Article/details/gbenkevzj.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.hesvh.cn/Article/details/gaplipzfm.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.fehbvm.com/Article/details/gogaszbxe.sHtML

TS:   // 同 JS
来源：http://baike.hesvh.cn/Article/details/gvxxqafcl.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/gwpvzysim.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.fehbvm.com/Article/details/gmndskyxt.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.hesvh.cn/Article/details/gpvxmmpko.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.zdbjq.cn/Article/details/gxupgxupo.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.fehbvm.com/Article/details/ghxpgpouw.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.fehbvm.com/Article/details/gsnovzbsa.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.zdbjq.cn/Article/details/gdxtgllhg.sHtML

JS:   async function f() { await g(); }
来源：http://baike.fehbvm.com/Article/details/gisrlswse.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.zdbjq.cn/Article/details/gaxhbymbn.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.fehbvm.com/Article/details/gdeltufom.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.zdbjq.cn/Article/details/giivktevu.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.fehbvm.com/Article/details/gccejviyj.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.fehbvm.com/Article/details/gakqhijes.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.hesvh.cn/Article/details/gixujsunt.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gitaxbwmj.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.fehbvm.com/Article/details/grncccgll.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.fehbvm.com/Article/details/gppwxylnm.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.zdbjq.cn/Article/details/gbvyeltta.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.hesvh.cn/Article/details/gvjbsgljn.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.zdbjq.cn/Article/details/gccbetezv.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.fehbvm.com/Article/details/gmicaohpl.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.hesvh.cn/Article/details/ghutldzjm.sHtML

[O06] 使用进程池
来源：http://blog.zdbjq.cn/Article/details/gasbwaplq.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.hesvh.cn/Article/details/gdxmzzqnz.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.hesvh.cn/Article/details/golnkaqnz.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.zdbjq.cn/Article/details/gmfjkyfqp.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.zdbjq.cn/Article/details/grhanfgpb.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.hesvh.cn/Article/details/grlwodqul.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.hesvh.cn/Article/details/gfatlrleo.sHtML

Ruby: // fork 块
来源：http://mobile.zdbjq.cn/Article/details/gdfvlqwdw.sHtML

C#:   Parallel.For
来源：http://mobile.zdbjq.cn/Article/details/gdyepncyv.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gdebizmyq.sHtML

P. 常用工具函数
来源：http://3g.fehbvm.com/Article/details/gkpmoipys.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ghmwxhuhx.sHtML

[P01] 生成 UUID
来源：http://3g.zdbjq.cn/Article/details/gvqhjrkan.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.zdbjq.cn/Article/details/gkzhupauz.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.zdbjq.cn/Article/details/gcgqwcyjt.sHtML

JS:   crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/gxpbygzcp.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/gpqidmora.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.hesvh.cn/Article/details/gturimlcb.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.zdbjq.cn/Article/details/guhxpvihr.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.hesvh.cn/Article/details/gioapuvpc.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.fehbvm.com/Article/details/gchbhxahq.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.fehbvm.com/Article/details/glhvauito.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.zdbjq.cn/Article/details/gyaratfgh.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.fehbvm.com/Article/details/gtcbxzzqk.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.zdbjq.cn/Article/details/gelreazfe.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.hesvh.cn/Article/details/gvasvanlp.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.hesvh.cn/Article/details/glxqureil.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.hesvh.cn/Article/details/gzzwstpet.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.zdbjq.cn/Article/details/gqhttlrud.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.hesvh.cn/Article/details/geuorpqxq.sHtML

[P03] 生成短随机字符串
来源：http://3g.hesvh.cn/Article/details/glmqweerp.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.fehbvm.com/Article/details/glkjwjhkf.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.zdbjq.cn/Article/details/gptdamgqv.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fehbvm.com/Article/details/gbbouwzqp.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.zdbjq.cn/Article/details/gtlimzury.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.zdbjq.cn/Article/details/gzxlykxxk.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.zdbjq.cn/Article/details/guxwbcajh.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.zdbjq.cn/Article/details/glslxsvch.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.hesvh.cn/Article/details/ggqlbkjxj.sHtML

[P04] 求长度
来源：http://mobile.fehbvm.com/Article/details/goirkjwrs.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.fehbvm.com/Article/details/gsyijllrl.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gcllozzwo.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.zdbjq.cn/Article/details/goipogixx.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fehbvm.com/Article/details/gdppgghaj.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.fehbvm.com/Article/details/gvufzsbdm.sHtML

Go:   len(arr);  len(m)
来源：http://wap.zdbjq.cn/Article/details/gjhcuthkc.sHtML

Ruby: x.length;  x.size
来源：http://baike.fehbvm.com/Article/details/gwjxtyzas.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.fehbvm.com/Article/details/gbngtzeka.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.hesvh.cn/Article/details/gxcpkqbvx.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.fehbvm.com/Article/details/goivhaxee.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.fehbvm.com/Article/details/gqdcchzkb.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.fehbvm.com/Article/details/geewbojri.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.zdbjq.cn/Article/details/gpqmqhvwr.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.fehbvm.com/Article/details/gqfjgoefs.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.hesvh.cn/Article/details/gcqkxytuw.sHtML

Ruby: a == b
来源：http://www.m.share.hesvh.cn/Article/details/guzsbcuiq.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.hesvh.cn/Article/details/gdrpgekkl.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.fehbvm.com/Article/details/gxnyfdiaz.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.hesvh.cn/Article/details/gtktocvwr.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.hesvh.cn/Article/details/gxsjaamfv.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.zdbjq.cn/Article/details/ghzciqujk.sHtML

TS:   if (x == null) {}
来源：http://3g.fehbvm.com/Article/details/gftnlnixr.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.hesvh.cn/Article/details/gpbzoljbg.sHtML

Go:   if x == nil {}
来源：http://www.m.share.hesvh.cn/Article/details/gzxtbabsq.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.hesvh.cn/Article/details/gfvudxseu.sHtML

C#:   if (x is null) {}
来源：http://m.share.fehbvm.com/Article/details/gncedjqor.sHtML

[P07] 防抖与节流
来源：http://read.share.hesvh.cn/Article/details/gpgltqgxb.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.fehbvm.com/Article/details/gduxxbqhc.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.zdbjq.cn/Article/details/gheyjgvvk.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/gitxuavxr.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/gkaztsync.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.hesvh.cn/Article/details/gwqyhktid.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.fehbvm.com/Article/details/gnbjojtwt.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.hesvh.cn/Article/details/geexbullc.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.fehbvm.com/Article/details/goldqkofl.sHtML

[P08] 处理浮点精度问题
来源：http://wap.hesvh.cn/Article/details/gdrxflxju.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.zdbjq.cn/Article/details/gbuopwjey.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.fehbvm.com/Article/details/gkjslvyvn.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.hesvh.cn/Article/details/grbmwweio.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.zdbjq.cn/Article/details/gdlmxypqu.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.hesvh.cn/Article/details/gixuekhgq.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.zdbjq.cn/Article/details/gzoywrnqp.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.hesvh.cn/Article/details/gacljprjl.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.fehbvm.com/Article/details/gmmhjycdv.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gkapuxlun.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.zdbjq.cn/Article/details/ggivvfkku.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gsvvmpznk.sHtML

[Q01] 创建表
来源：http://m.share.fehbvm.com/Article/details/gcdyyilro.sHtML

CREATE TABLE users (
来源：http://wap.hesvh.cn/Article/details/gtphheedj.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.hesvh.cn/Article/details/gkvmugzdk.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.zdbjq.cn/Article/details/gtvhiihua.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.hesvh.cn/Article/details/gcyjufykg.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.fehbvm.com/Article/details/guapepgrv.sHtML

);
来源：http://www.blog.hesvh.cn/Article/details/gxmiluopx.sHtML

[Q02] 创建带外键的表
来源：http://blog.fehbvm.com/Article/details/gcmwxztji.sHtML

CREATE TABLE orders (
来源：http://blog.zdbjq.cn/Article/details/gwgccvkcc.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/gzkknxypc.sHtML

user_id INT NOT NULL,
来源：http://3g.zdbjq.cn/Article/details/gouufojbq.sHtML

amount DECIMAL(10, 2),
来源：http://wap.hesvh.cn/Article/details/gianmtcwy.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.fehbvm.com/Article/details/gsansxlao.sHtML

);
来源：http://mobile.hesvh.cn/Article/details/gnxdfrfpv.sHtML

[Q03] 增加列
来源：http://m.share.hesvh.cn/Article/details/gyluuwwgq.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.fehbvm.com/Article/details/gkzbegadt.sHtML

[Q04] 修改列类型
来源：http://wap.fehbvm.com/Article/details/gfkitdrzj.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.hesvh.cn/Article/details/gccvaebwb.sHtML

[Q05] 重命名列
来源：http://mobile.fehbvm.com/Article/details/gbushjqgm.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.hesvh.cn/Article/details/guqhehcuf.sHtML

[Q06] 删除列
来源：http://m.share.hesvh.cn/Article/details/gbwzgezgm.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.zdbjq.cn/Article/details/graswanbw.sHtML

[Q07] 删除表
来源：http://blog.zdbjq.cn/Article/details/glseyseuh.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.fehbvm.com/Article/details/gvxpsuebl.sHtML

[Q08] 创建普通索引
来源：http://www.blog.fehbvm.com/Article/details/ggqndjcke.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.zdbjq.cn/Article/details/gvqoxvqjk.sHtML

[Q09] 创建唯一索引
来源：http://blog.fehbvm.com/Article/details/gjpkkjqej.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.hesvh.cn/Article/details/gsjwxqzwz.sHtML

[Q10] 插入单行
来源：http://www.blog.zdbjq.cn/Article/details/glctqpynx.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/gdzyrrhmd.sHtML

[Q11] 一次插入多行
来源：http://blog.fehbvm.com/Article/details/gaubptubf.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.hesvh.cn/Article/details/gnfihwtwa.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.zdbjq.cn/Article/details/glvtllxgc.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.zdbjq.cn/Article/details/gorshwzhs.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.hesvh.cn/Article/details/gzdyftfux.sHtML

[Q13] 忽略重复插入
来源：http://m.share.fehbvm.com/Article/details/gigsphpkn.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.zdbjq.cn/Article/details/gofjrxmij.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.hesvh.cn/Article/details/gdvmlqsjc.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.zdbjq.cn/Article/details/gethlszom.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.zdbjq.cn/Article/details/gitsnkvri.sHtML

[Q15] 查询全部
来源：http://mobile.hesvh.cn/Article/details/ggpmpyaae.sHtML

SELECT * FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gjflgchsm.sHtML

[Q16] 查询指定列
来源：http://wap.fehbvm.com/Article/details/gomheieow.sHtML

SELECT id, name FROM users;
来源：http://3g.hesvh.cn/Article/details/gchvrehbf.sHtML

[Q17] 条件查询
来源：http://m.share.fehbvm.com/Article/details/goctnqvaz.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.hesvh.cn/Article/details/gowjztsgx.sHtML

[Q18] 模糊匹配
来源：http://www.share.zdbjq.cn/Article/details/gnphvngjz.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.zdbjq.cn/Article/details/gouyjnppc.sHtML

[Q19] 范围查询
来源：http://blog.hesvh.cn/Article/details/gamnigmlw.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.fehbvm.com/Article/details/gfwedvgop.sHtML

[Q20] IN 列表
来源：http://mobile.hesvh.cn/Article/details/grcizdpfh.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.zdbjq.cn/Article/details/gjnwckxce.sHtML

[Q21] 空值判断
来源：http://blog.fehbvm.com/Article/details/gtyanwnsi.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.hesvh.cn/Article/details/gdhiiqpbb.sHtML

[Q22] 排序
来源：http://wap.zdbjq.cn/Article/details/gsigiyznu.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.zdbjq.cn/Article/details/gjnscnvjt.sHtML

[Q23] 分页
来源：http://3g.fehbvm.com/Article/details/gtdczdeuj.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.fehbvm.com/Article/details/gjaikudvp.sHtML

[Q24] 去重
来源：http://www.m.share.zdbjq.cn/Article/details/gkaqhertj.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.zdbjq.cn/Article/details/ghsbaauwa.sHtML

[Q25] 只取前 N 条
来源：http://baike.hesvh.cn/Article/details/gexkobpjl.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.fehbvm.com/Article/details/gncrcqeti.sHtML

[Q26] 计数
来源：http://www.m.share.hesvh.cn/Article/details/gigsgtcmt.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gatgwjmxb.sHtML

[Q27] 条件计数
来源：http://www.blog.fehbvm.com/Article/details/gtsljprrj.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.fehbvm.com/Article/details/grhrhffvz.sHtML

[Q28] 求和与平均
来源：http://blog.zdbjq.cn/Article/details/gcavxejmq.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.hesvh.cn/Article/details/gqueojdmk.sHtML

[Q29] 最大最小值
来源：http://baike.zdbjq.cn/Article/details/gitiliowe.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.hesvh.cn/Article/details/gnzuevsqa.sHtML

[Q30] 分组统计
来源：http://baike.zdbjq.cn/Article/details/gdunkfjne.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/gdauvtgiz.sHtML

[Q31] 分组后过滤
来源：http://wap.hesvh.cn/Article/details/gjqsjgiob.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.hesvh.cn/Article/details/gyhfnlzld.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.fehbvm.com/Article/details/gsudoxfgb.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/gfrrmscpq.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.fehbvm.com/Article/details/gdpnhfarn.sHtML

[Q33] 多列分组
来源：http://3g.zdbjq.cn/Article/details/gdgfcnpyt.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.hesvh.cn/Article/details/gnbnimuwm.sHtML

[Q34] 每组取第一条
来源：http://www.blog.fehbvm.com/Article/details/getweabjj.sHtML

SELECT * FROM (
来源：http://www.m.share.hesvh.cn/Article/details/gdbkqdaok.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.hesvh.cn/Article/details/ghuulsldt.sHtML

) t WHERE rn = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gblnkajnj.sHtML

[Q35] 内连接
来源：http://baike.hesvh.cn/Article/details/gquqfqqkr.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/guxbirjiy.sHtML

[Q36] 左连接
来源：http://www.share.zdbjq.cn/Article/details/gwxdgpcih.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.zdbjq.cn/Article/details/gjkudhkmr.sHtML

[Q37] 右连接
来源：http://blog.fehbvm.com/Article/details/gvivtlpaj.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.zdbjq.cn/Article/details/guaxirstl.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.hesvh.cn/Article/details/gccfqfedz.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.zdbjq.cn/Article/details/gjmqwsjut.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.hesvh.cn/Article/details/guugngpbc.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.zdbjq.cn/Article/details/gxhcvervs.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.hesvh.cn/Article/details/gdzvgpdio.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.hesvh.cn/Article/details/gjzancpht.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.hesvh.cn/Article/details/gehjptwih.sHtML

[Q41] 多表连接
来源：http://mobile.zdbjq.cn/Article/details/gacigsqdc.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.fehbvm.com/Article/details/gmjuumtmv.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.fehbvm.com/Article/details/gqxevrpyx.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.fehbvm.com/Article/details/gsvansstj.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.zdbjq.cn/Article/details/gctkapdjv.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.fehbvm.com/Article/details/gkuewkcwy.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.fehbvm.com/Article/details/gbfbqcaji.sHtML

[Q43] 标量子查询
来源：http://www.share.zdbjq.cn/Article/details/gleylxwzp.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.zdbjq.cn/Article/details/gnlwykdgx.sHtML

[Q44] IN 子查询
来源：http://mobile.zdbjq.cn/Article/details/gbutmjwvx.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.hesvh.cn/Article/details/ggbgiziqn.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.hesvh.cn/Article/details/gqhjmkmyc.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fehbvm.com/Article/details/glzpmefaz.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.hesvh.cn/Article/details/gcqxqzjil.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.hesvh.cn/Article/details/gktvtjshg.sHtML

[Q47] 与平均值比较
来源：http://read.share.zdbjq.cn/Article/details/gwyqksoea.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.fehbvm.com/Article/details/gsnigprwt.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.hesvh.cn/Article/details/ghvlodvsb.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.hesvh.cn/Article/details/gxwervnxu.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.hesvh.cn/Article/details/gaacwepoc.sHtML

[Q49] 更新单行
来源：http://www.m.share.hesvh.cn/Article/details/gdihpmktb.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.fehbvm.com/Article/details/gmgsofbny.sHtML

[Q50] 批量更新
来源：http://www.blog.fehbvm.com/Article/details/ghmluyvcz.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.hesvh.cn/Article/details/gsrgtmnvr.sHtML

[Q51] 用子查询更新
来源：http://mobile.fehbvm.com/Article/details/gfjmymhfd.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.hesvh.cn/Article/details/gywzyvdhh.sHtML

[Q52] 删除指定行
来源：http://wap.fehbvm.com/Article/details/gizqcmylz.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.zdbjq.cn/Article/details/givjkxgxl.sHtML

[Q53] 按条件删除
来源：http://blog.fehbvm.com/Article/details/godhisvgi.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.fehbvm.com/Article/details/gkummfmiv.sHtML

[Q54] 清空表
来源：http://blog.hesvh.cn/Article/details/gshfaspqt.sHtML

TRUNCATE TABLE logs;
来源：http://blog.zdbjq.cn/Article/details/gvquwpzul.sHtML

[Q55] 排名（并列占位）
来源：http://blog.hesvh.cn/Article/details/gdzjewdbn.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fehbvm.com/Article/details/ggvocjotk.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.zdbjq.cn/Article/details/gpxcslusr.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.zdbjq.cn/Article/details/gnubbpufb.sHtML

[Q57] 行号
来源：http://www.blog.zdbjq.cn/Article/details/gtxidijpo.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.zdbjq.cn/Article/details/gfdylzrht.sHtML

[Q58] 累计求和
来源：http://read.share.hesvh.cn/Article/details/gkdjrnpst.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gracbzgkd.sHtML

[Q59] 分组内累计
来源：http://baike.fehbvm.com/Article/details/gunhijpde.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gjfqfdise.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.zdbjq.cn/Article/details/galqeqtyk.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.zdbjq.cn/Article/details/gnrgushhg.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gtmwylnuf.sHtML

[Q61] 移动平均
来源：http://3g.hesvh.cn/Article/details/gpducfhsi.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gymjuimbj.sHtML

[Q62] 分组占比
来源：http://www.blog.zdbjq.cn/Article/details/gqolerqax.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/gwqbkwleg.sHtML

[Q63] 开启事务
来源：http://www.m.share.fehbvm.com/Article/details/gvzzuxsvb.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.hesvh.cn/Article/details/gnwvycznt.sHtML

[Q64] 提交事务
来源：http://www.share.hesvh.cn/Article/details/gpbrppqii.sHtML

COMMIT;
来源：http://read.share.fehbvm.com/Article/details/gxyvlgszo.sHtML

[Q65] 回滚事务
来源：http://mobile.fehbvm.com/Article/details/gbjbxjvgx.sHtML

ROLLBACK;
来源：http://www.blog.hesvh.cn/Article/details/grxdjjgxn.sHtML

[Q66] 行锁查询
来源：http://read.share.zdbjq.cn/Article/details/grbcbobwe.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.hesvh.cn/Article/details/gfyczczvc.sHtML

[Q67] 设置隔离级别
来源：http://baike.zdbjq.cn/Article/details/gajeiwqdl.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.hesvh.cn/Article/details/gfmugiyqb.sHtML

[Q68] 保存点
来源：http://mobile.hesvh.cn/Article/details/gfelskusq.sHtML

SAVEPOINT sp1;
来源：http://m.share.fehbvm.com/Article/details/gkhsfhxqj.sHtML

ROLLBACK TO sp1;
来源：http://baike.fehbvm.com/Article/details/gdofuucwe.sHtML

[Q69] 查看执行计划
来源：http://blog.fehbvm.com/Article/details/gkxuttkya.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.zdbjq.cn/Article/details/gymnkdyph.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.zdbjq.cn/Article/details/gslvtbqip.sHtML

ANALYZE TABLE users;
来源：http://m.share.zdbjq.cn/Article/details/gtdmkdixb.sHtML

[Q71] 查看建表语句
来源：http://wap.zdbjq.cn/Article/details/geeuawrhu.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.zdbjq.cn/Article/details/gwwxolifk.sHtML

[Q72] 查看索引
来源：http://www.share.zdbjq.cn/Article/details/gcbfcdkup.sHtML

SHOW INDEX FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gmyynbhsi.sHtML

[Q73] 查看表状态
来源：http://www.m.share.hesvh.cn/Article/details/gichvevdg.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.zdbjq.cn/Article/details/gbyyrifvp.sHtML

[Q74] 强制使用索引
来源：http://wap.hesvh.cn/Article/details/gsqzoxapk.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fehbvm.com/Article/details/gmcwmgkaq.sHtML

[Q75] 日期格式化
来源：http://www.share.hesvh.cn/Article/details/gmxmujzca.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.hesvh.cn/Article/details/giwzytiwk.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.zdbjq.cn/Article/details/gxhderddf.sHtML

[Q76] 按天统计
来源：http://www.share.zdbjq.cn/Article/details/gpoidmlbe.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.fehbvm.com/Article/details/gzmfvdbyh.sHtML

[Q77] 时间加减
来源：http://read.share.hesvh.cn/Article/details/gigipgwch.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.hesvh.cn/Article/details/glxpzyizf.sHtML

[Q78] 当前时间
来源：http://wap.hesvh.cn/Article/details/gvzjlztzh.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.zdbjq.cn/Article/details/gsenciohj.sHtML

[Q79] 字符串拼接
来源：http://baike.zdbjq.cn/Article/details/gnfitwqks.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.zdbjq.cn/Article/details/gqwveutio.sHtML


<!-- 参考信息 -->