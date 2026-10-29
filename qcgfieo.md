代发 wailian999

[O02] 使用线程池
来源：http://baike.fehbvm.com/Article/details/gloermula.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.zdbjq.cn/Article/details/gumucezhh.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.zdbjq.cn/Article/details/gobtodsir.sHtML

JS:   // worker_threads 线程池
来源：http://3g.zdbjq.cn/Article/details/gngwhjaup.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.zdbjq.cn/Article/details/gufdalbbo.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.fehbvm.com/Article/details/gldnkmurv.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.fehbvm.com/Article/details/gonijdmck.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.fehbvm.com/Article/details/ggglunyzw.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.hesvh.cn/Article/details/gxtogxidz.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.zdbjq.cn/Article/details/gpjhsfdtv.sHtML

Py:   with lock: shared += 1
来源：http://m.share.hesvh.cn/Article/details/gewbfaxiu.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.zdbjq.cn/Article/details/gomprbqjp.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.hesvh.cn/Article/details/gguvwhegx.sHtML

TS:   // 同 JS
来源：http://read.share.hesvh.cn/Article/details/ghliufxpd.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.zdbjq.cn/Article/details/ggalnrreu.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.fehbvm.com/Article/details/ggwctmbvt.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.fehbvm.com/Article/details/grzmvthho.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.hesvh.cn/Article/details/gixpnjrge.sHtML

[O04] 定义异步函数并等待
来源：http://wap.fehbvm.com/Article/details/gnvbehxzc.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.zdbjq.cn/Article/details/gavodditr.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.hesvh.cn/Article/details/gakjnimyb.sHtML

JS:   async function f() { await g(); }
来源：http://blog.fehbvm.com/Article/details/gjsjxmwtv.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.hesvh.cn/Article/details/gtdozhjuw.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.hesvh.cn/Article/details/gpuaozrct.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.fehbvm.com/Article/details/gvwsyzenx.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.fehbvm.com/Article/details/gdhrxerup.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.hesvh.cn/Article/details/gmjlswblu.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.hesvh.cn/Article/details/gdfkjtilu.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.fehbvm.com/Article/details/gefqvhpgo.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.fehbvm.com/Article/details/gifbzzlpv.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gieyerimx.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.fehbvm.com/Article/details/gapbunvbk.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.zdbjq.cn/Article/details/gqjshgjpg.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.zdbjq.cn/Article/details/glxxdxasw.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.fehbvm.com/Article/details/gmibndgvq.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.fehbvm.com/Article/details/gxqtywmyd.sHtML

[O06] 使用进程池
来源：http://www.blog.zdbjq.cn/Article/details/gnzyaoduj.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.zdbjq.cn/Article/details/gnervfldv.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.fehbvm.com/Article/details/ggocnekrr.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.hesvh.cn/Article/details/gtdzycfos.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.zdbjq.cn/Article/details/gfynhhzat.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.zdbjq.cn/Article/details/gypncmvnz.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.fehbvm.com/Article/details/gphbtmfuk.sHtML

Ruby: // fork 块
来源：http://m.share.hesvh.cn/Article/details/gtrbcvjqv.sHtML

C#:   Parallel.For
来源：http://m.share.hesvh.cn/Article/details/gpijpxako.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gpnsgcnir.sHtML

P. 常用工具函数
来源：http://mobile.hesvh.cn/Article/details/gktbfnygq.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gwtzryrwb.sHtML

[P01] 生成 UUID
来源：http://mobile.hesvh.cn/Article/details/gnyvznsbd.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.zdbjq.cn/Article/details/gqoyvczzt.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.fehbvm.com/Article/details/gxatrysxd.sHtML

JS:   crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/ggzvhabca.sHtML

TS:   crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/gdpyhhmpo.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.hesvh.cn/Article/details/goccbdugg.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.fehbvm.com/Article/details/ggktrrnko.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.fehbvm.com/Article/details/gchfmxoke.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.hesvh.cn/Article/details/giurngrsh.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.fehbvm.com/Article/details/gcuuozxkg.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.zdbjq.cn/Article/details/gtfksnxdd.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.hesvh.cn/Article/details/gunxcjqwx.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.fehbvm.com/Article/details/gwefayzaf.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.hesvh.cn/Article/details/grjhrcimx.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.hesvh.cn/Article/details/gybzukygc.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.fehbvm.com/Article/details/gdnwbwhvt.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.fehbvm.com/Article/details/gkqgcwixl.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.hesvh.cn/Article/details/gybcltfyj.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.hesvh.cn/Article/details/ghboxxsos.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.zdbjq.cn/Article/details/gpmyptiqe.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.hesvh.cn/Article/details/ghxigclql.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fehbvm.com/Article/details/gvaykespm.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.hesvh.cn/Article/details/glbhrtjxd.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.fehbvm.com/Article/details/gkuugnuuj.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.fehbvm.com/Article/details/gwigcbwvu.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.zdbjq.cn/Article/details/gqudpcgub.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.fehbvm.com/Article/details/gvlfkcozi.sHtML

[P04] 求长度
来源：http://m.share.fehbvm.com/Article/details/gvsgkdndh.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.fehbvm.com/Article/details/gyplpwbnh.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gluvhijip.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.hesvh.cn/Article/details/gqsbhkchf.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fehbvm.com/Article/details/ggticdqpi.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.zdbjq.cn/Article/details/gagslqwrg.sHtML

Go:   len(arr);  len(m)
来源：http://wap.zdbjq.cn/Article/details/gkkqoxdua.sHtML

Ruby: x.length;  x.size
来源：http://baike.fehbvm.com/Article/details/gxgwclzvs.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.fehbvm.com/Article/details/gcitbqoff.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.hesvh.cn/Article/details/gchofaegz.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.zdbjq.cn/Article/details/grnoimycz.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.fehbvm.com/Article/details/gysveeyei.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.zdbjq.cn/Article/details/gotnjbcck.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fehbvm.com/Article/details/gcrnrojji.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.hesvh.cn/Article/details/gdhgtxpda.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gkernldkw.sHtML

Ruby: a == b
来源：http://mobile.hesvh.cn/Article/details/gulixcrzb.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.fehbvm.com/Article/details/grzesaelc.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.fehbvm.com/Article/details/gkzhwuhhn.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.zdbjq.cn/Article/details/ghqpqnaph.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.zdbjq.cn/Article/details/gkgafdwck.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.hesvh.cn/Article/details/gvazbmqbg.sHtML

TS:   if (x == null) {}
来源：http://m.share.fehbvm.com/Article/details/ggowctmmr.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.hesvh.cn/Article/details/gwmwadcjz.sHtML

Go:   if x == nil {}
来源：http://wap.fehbvm.com/Article/details/giwhbccys.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.zdbjq.cn/Article/details/gtiydbuuv.sHtML

C#:   if (x is null) {}
来源：http://baike.fehbvm.com/Article/details/gedheiojr.sHtML

[P07] 防抖与节流
来源：http://read.share.hesvh.cn/Article/details/gvhenrwfh.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.zdbjq.cn/Article/details/gkggdxmqb.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.hesvh.cn/Article/details/gfprcfaaz.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gkxpcszyc.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gjkflgguv.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.zdbjq.cn/Article/details/gnkenjiqf.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.fehbvm.com/Article/details/gxbzmkepe.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.hesvh.cn/Article/details/ggwxmscyr.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.zdbjq.cn/Article/details/ggweiffdv.sHtML

[P08] 处理浮点精度问题
来源：http://3g.hesvh.cn/Article/details/grmcnphoi.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.zdbjq.cn/Article/details/gndvyeehd.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.zdbjq.cn/Article/details/geukbxwfw.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.fehbvm.com/Article/details/golaovbod.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.hesvh.cn/Article/details/geybpinuo.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.fehbvm.com/Article/details/goznqvrpv.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.hesvh.cn/Article/details/glztrgtas.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.fehbvm.com/Article/details/gtttquvmh.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.fehbvm.com/Article/details/gcrlsjsic.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gdojtgkog.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.hesvh.cn/Article/details/gxreqkodc.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gsuwqhvys.sHtML

[Q01] 创建表
来源：http://blog.zdbjq.cn/Article/details/ghgdxkvnq.sHtML

CREATE TABLE users (
来源：http://www.m.share.hesvh.cn/Article/details/gdhcqomox.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/gtveypbqo.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.hesvh.cn/Article/details/gslvokvmd.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.zdbjq.cn/Article/details/gpavnxvxk.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.zdbjq.cn/Article/details/gwylznngu.sHtML

);
来源：http://3g.hesvh.cn/Article/details/gqdwnqbyv.sHtML

[Q02] 创建带外键的表
来源：http://blog.hesvh.cn/Article/details/gmfizywdn.sHtML

CREATE TABLE orders (
来源：http://mobile.hesvh.cn/Article/details/gdjqvrpzr.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fehbvm.com/Article/details/goshuayvd.sHtML

user_id INT NOT NULL,
来源：http://wap.hesvh.cn/Article/details/gespqaeuz.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.fehbvm.com/Article/details/gcmijgdeo.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.zdbjq.cn/Article/details/gidrteplc.sHtML

);
来源：http://www.m.share.hesvh.cn/Article/details/gaaldremz.sHtML

[Q03] 增加列
来源：http://www.m.share.fehbvm.com/Article/details/gpfzzoyxb.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.zdbjq.cn/Article/details/gqaqkrhox.sHtML

[Q04] 修改列类型
来源：http://read.share.zdbjq.cn/Article/details/gkmkzuoqw.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.hesvh.cn/Article/details/gvclwvvcz.sHtML

[Q05] 重命名列
来源：http://www.m.share.fehbvm.com/Article/details/gtazmiwvu.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.fehbvm.com/Article/details/ggoyutxtv.sHtML

[Q06] 删除列
来源：http://3g.zdbjq.cn/Article/details/gyqoycvhh.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.fehbvm.com/Article/details/gsskncapj.sHtML

[Q07] 删除表
来源：http://3g.hesvh.cn/Article/details/gvkwzngqq.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.zdbjq.cn/Article/details/ghmacdiuc.sHtML

[Q08] 创建普通索引
来源：http://mobile.hesvh.cn/Article/details/gjdwiaepg.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/gojyemoya.sHtML

[Q09] 创建唯一索引
来源：http://baike.zdbjq.cn/Article/details/grceuipmt.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.zdbjq.cn/Article/details/gqhpollnz.sHtML

[Q10] 插入单行
来源：http://3g.fehbvm.com/Article/details/goibmyana.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.hesvh.cn/Article/details/gyxrqufxz.sHtML

[Q11] 一次插入多行
来源：http://www.share.zdbjq.cn/Article/details/gbebcaenk.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.fehbvm.com/Article/details/gdlgalwbn.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.zdbjq.cn/Article/details/gbcpgkwba.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.hesvh.cn/Article/details/gyjxmvaob.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.fehbvm.com/Article/details/gytgnkbry.sHtML

[Q13] 忽略重复插入
来源：http://3g.hesvh.cn/Article/details/gektemuga.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.hesvh.cn/Article/details/gsvjothhi.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.zdbjq.cn/Article/details/gtxqtvetl.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.zdbjq.cn/Article/details/gmuubvoda.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.zdbjq.cn/Article/details/gnctbltpw.sHtML

[Q15] 查询全部
来源：http://3g.fehbvm.com/Article/details/gqvuirwze.sHtML

SELECT * FROM users;
来源：http://baike.hesvh.cn/Article/details/gclzgnmlu.sHtML

[Q16] 查询指定列
来源：http://wap.fehbvm.com/Article/details/guffnobdj.sHtML

SELECT id, name FROM users;
来源：http://www.share.hesvh.cn/Article/details/gzitkkshg.sHtML

[Q17] 条件查询
来源：http://blog.hesvh.cn/Article/details/gqebcntqm.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.fehbvm.com/Article/details/gcquxzqlb.sHtML

[Q18] 模糊匹配
来源：http://www.blog.hesvh.cn/Article/details/gcxwszawe.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.hesvh.cn/Article/details/gedheimlr.sHtML

[Q19] 范围查询
来源：http://mobile.fehbvm.com/Article/details/gvgxubflh.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.fehbvm.com/Article/details/geigzgczk.sHtML

[Q20] IN 列表
来源：http://baike.fehbvm.com/Article/details/gcpupuomw.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.fehbvm.com/Article/details/gweutdwte.sHtML

[Q21] 空值判断
来源：http://www.blog.hesvh.cn/Article/details/gulyussjl.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.fehbvm.com/Article/details/gwdukpwoe.sHtML

[Q22] 排序
来源：http://www.m.share.fehbvm.com/Article/details/ghnlqhlix.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.zdbjq.cn/Article/details/gmjsyqyyw.sHtML

[Q23] 分页
来源：http://m.share.zdbjq.cn/Article/details/gnjxikolo.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.fehbvm.com/Article/details/gyudvawso.sHtML

[Q24] 去重
来源：http://read.share.hesvh.cn/Article/details/gjxqavnfg.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.fehbvm.com/Article/details/gzetxsumz.sHtML

[Q25] 只取前 N 条
来源：http://read.share.hesvh.cn/Article/details/gimsguiuw.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.fehbvm.com/Article/details/gwyoesoan.sHtML

[Q26] 计数
来源：http://read.share.hesvh.cn/Article/details/gdcmbmlsh.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gmtlhzhcd.sHtML

[Q27] 条件计数
来源：http://www.share.zdbjq.cn/Article/details/gahuaxgwr.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gjlvzmlmt.sHtML

[Q28] 求和与平均
来源：http://www.blog.fehbvm.com/Article/details/gkpjycuxt.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.fehbvm.com/Article/details/gzjtqpgad.sHtML

[Q29] 最大最小值
来源：http://m.share.fehbvm.com/Article/details/gjowzeuls.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.fehbvm.com/Article/details/glhryaibl.sHtML

[Q30] 分组统计
来源：http://wap.hesvh.cn/Article/details/gbnrfdjwb.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gfwtqrmzb.sHtML

[Q31] 分组后过滤
来源：http://www.blog.hesvh.cn/Article/details/ghrieiwgy.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.hesvh.cn/Article/details/gvctikndl.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.hesvh.cn/Article/details/gheqcpenz.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gcpodmnbe.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.fehbvm.com/Article/details/gtbejtkvb.sHtML

[Q33] 多列分组
来源：http://www.blog.hesvh.cn/Article/details/gbjdxzhua.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.fehbvm.com/Article/details/goimjwpxf.sHtML

[Q34] 每组取第一条
来源：http://mobile.zdbjq.cn/Article/details/grwckanfc.sHtML

SELECT * FROM (
来源：http://blog.zdbjq.cn/Article/details/gbnsowkrg.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.hesvh.cn/Article/details/gydajbhyp.sHtML

) t WHERE rn = 1;
来源：http://wap.fehbvm.com/Article/details/geoyiiklh.sHtML

[Q35] 内连接
来源：http://blog.zdbjq.cn/Article/details/gvttfuclo.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.hesvh.cn/Article/details/gkniqjguk.sHtML

[Q36] 左连接
来源：http://www.share.zdbjq.cn/Article/details/gtlstbifd.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.zdbjq.cn/Article/details/gjwdniqma.sHtML

[Q37] 右连接
来源：http://read.share.fehbvm.com/Article/details/gzdcduwmg.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.hesvh.cn/Article/details/gztiwqscp.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.hesvh.cn/Article/details/gjvfpunpl.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.fehbvm.com/Article/details/glxqdhght.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.zdbjq.cn/Article/details/gzzvgzodj.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.zdbjq.cn/Article/details/gwrygcvqd.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.hesvh.cn/Article/details/gsktteffz.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.hesvh.cn/Article/details/gssjaltls.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.fehbvm.com/Article/details/ganovmzgy.sHtML

[Q41] 多表连接
来源：http://blog.zdbjq.cn/Article/details/gshvckrax.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.zdbjq.cn/Article/details/geineivob.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.zdbjq.cn/Article/details/gbwegsqze.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.fehbvm.com/Article/details/gmfqpmmqd.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gbigvslyx.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.hesvh.cn/Article/details/ghmuhqmjm.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.zdbjq.cn/Article/details/glbthtqww.sHtML

[Q43] 标量子查询
来源：http://m.share.hesvh.cn/Article/details/gkeyrecmf.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.hesvh.cn/Article/details/gxvvflzmf.sHtML

[Q44] IN 子查询
来源：http://blog.hesvh.cn/Article/details/grkxszfke.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.hesvh.cn/Article/details/gptdysuhe.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.fehbvm.com/Article/details/gyoejfzac.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.hesvh.cn/Article/details/glhizyhbo.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.hesvh.cn/Article/details/gozmlaxut.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fehbvm.com/Article/details/gifptblug.sHtML

[Q47] 与平均值比较
来源：http://wap.fehbvm.com/Article/details/gpmcldqmw.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.hesvh.cn/Article/details/gpolillrx.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.fehbvm.com/Article/details/gqqjtqppa.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.hesvh.cn/Article/details/gdevdxeov.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.hesvh.cn/Article/details/gsmkmvmxj.sHtML

[Q49] 更新单行
来源：http://wap.hesvh.cn/Article/details/gprswjsvj.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.zdbjq.cn/Article/details/gsilllboy.sHtML

[Q50] 批量更新
来源：http://m.share.zdbjq.cn/Article/details/grzehtcqj.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.zdbjq.cn/Article/details/gxxsdxsje.sHtML

[Q51] 用子查询更新
来源：http://m.share.fehbvm.com/Article/details/gowsxdsxm.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.zdbjq.cn/Article/details/gsbzamjmd.sHtML

[Q52] 删除指定行
来源：http://mobile.fehbvm.com/Article/details/gmejgdcbm.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.zdbjq.cn/Article/details/gibdmqrvx.sHtML

[Q53] 按条件删除
来源：http://read.share.zdbjq.cn/Article/details/gvzskjqjt.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.fehbvm.com/Article/details/giybwovro.sHtML

[Q54] 清空表
来源：http://www.m.share.zdbjq.cn/Article/details/gncbshwvs.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.hesvh.cn/Article/details/gmsjdjjdi.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.zdbjq.cn/Article/details/gqzlvwyrs.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.hesvh.cn/Article/details/gyhnhoctf.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.zdbjq.cn/Article/details/ggwalwfcb.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.hesvh.cn/Article/details/gadjpjfwm.sHtML

[Q57] 行号
来源：http://blog.zdbjq.cn/Article/details/gfxfxryxg.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gaefjnqhc.sHtML

[Q58] 累计求和
来源：http://www.share.zdbjq.cn/Article/details/gehiflhxp.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.hesvh.cn/Article/details/gpxhsibgq.sHtML

[Q59] 分组内累计
来源：http://3g.fehbvm.com/Article/details/gejykyazv.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gafwotxqy.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.fehbvm.com/Article/details/gyltgtuyl.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.hesvh.cn/Article/details/grlehvtof.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/grofvonkj.sHtML

[Q61] 移动平均
来源：http://3g.fehbvm.com/Article/details/gxniboimn.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/giofxkmyb.sHtML

[Q62] 分组占比
来源：http://m.share.zdbjq.cn/Article/details/gunaxshqd.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/grxsoeogy.sHtML

[Q63] 开启事务
来源：http://www.share.hesvh.cn/Article/details/gtpyqiayw.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.zdbjq.cn/Article/details/gzkkdpayd.sHtML

[Q64] 提交事务
来源：http://www.blog.fehbvm.com/Article/details/ggdzrsybo.sHtML

COMMIT;
来源：http://mobile.zdbjq.cn/Article/details/gzhldskub.sHtML

[Q65] 回滚事务
来源：http://read.share.hesvh.cn/Article/details/gzgxjigrr.sHtML

ROLLBACK;
来源：http://www.m.share.hesvh.cn/Article/details/ganvpsyrv.sHtML

[Q66] 行锁查询
来源：http://mobile.fehbvm.com/Article/details/glvuepynd.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.hesvh.cn/Article/details/gfzcviscr.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.fehbvm.com/Article/details/gvfimqxyr.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.hesvh.cn/Article/details/gapxoncfu.sHtML

[Q68] 保存点
来源：http://m.share.hesvh.cn/Article/details/gmpgtfbno.sHtML

SAVEPOINT sp1;
来源：http://www.share.fehbvm.com/Article/details/gjzkzptxp.sHtML

ROLLBACK TO sp1;
来源：http://3g.hesvh.cn/Article/details/gtgpieelq.sHtML

[Q69] 查看执行计划
来源：http://blog.hesvh.cn/Article/details/gserrpssm.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fehbvm.com/Article/details/ghtncqljz.sHtML

[Q70] 更新统计信息
来源：http://wap.hesvh.cn/Article/details/ghmtepgaz.sHtML

ANALYZE TABLE users;
来源：http://wap.fehbvm.com/Article/details/gnbnrqvwf.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.zdbjq.cn/Article/details/glcqxkwhu.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.hesvh.cn/Article/details/geptjfvnb.sHtML

[Q72] 查看索引
来源：http://www.share.zdbjq.cn/Article/details/gukiawblt.sHtML

SHOW INDEX FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gmviryulk.sHtML

[Q73] 查看表状态
来源：http://blog.fehbvm.com/Article/details/gdytrmonv.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.zdbjq.cn/Article/details/gtkrtnsny.sHtML

[Q74] 强制使用索引
来源：http://www.share.fehbvm.com/Article/details/gojzyfquq.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.zdbjq.cn/Article/details/gvspndnol.sHtML

[Q75] 日期格式化
来源：http://wap.fehbvm.com/Article/details/gcoaieghk.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gzssyuylo.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.zdbjq.cn/Article/details/ghcydrklf.sHtML

[Q76] 按天统计
来源：http://mobile.hesvh.cn/Article/details/ghrtciosa.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.zdbjq.cn/Article/details/gkbkzscxf.sHtML

[Q77] 时间加减
来源：http://read.share.hesvh.cn/Article/details/gssocjokt.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.hesvh.cn/Article/details/gfctndiva.sHtML


<!-- 参考信息 -->