代发 wailian999

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2imfoyebx.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2nhsuzmno.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2xqgsxxxx.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ewsoowyv.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2nfsemwxw.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2jxqdlmsp.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2ewfzkqoh.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2bjwjddia.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2vbhqbrau.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2tydigbvn.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2svmvbjak.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ladksveb.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2zastjftk.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2wqmcheto.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2aatairrl.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2jvmqhzpy.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2bcazqbxf.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2klpqeaji.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2wdcioyez.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2vdxpprhk.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2kurnnkiw.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2lzfzedbm.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2uhxlfjwe.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2uecijbxt.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2txzcbqal.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2ltrohrwo.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2aihdrunm.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2lckdzknb.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2tqbrvppo.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2uybabuua.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2pbqekpky.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2odfbraad.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2osfimpbg.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2sgegucxa.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2tmvieryz.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2qriexacb.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2vztmqvbo.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2uzmyobcc.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ngmjkzwz.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2edwkjovx.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2ccbkxidx.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2vqheweky.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2egplcujc.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2poqldszr.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2jmiaxwlf.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2llrwestg.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2kwqmynnh.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2sjzpaeaw.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2maquveno.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2idohbdcn.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2nbjjtzqd.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2eqtjtkxt.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2zgqnmoer.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wmimwhfn.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2ytmgkmmi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ysaxpbfo.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2tmtnirog.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2jfxzwhnn.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2mvogfnug.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2tmedpbaj.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2ejlrujes.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2lgxeaakl.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2aytkvgar.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2fezqdpuw.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2fsljxcjw.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2lupypncz.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2asffmlim.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2sdndhtan.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2chqdfpab.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2huzkbpek.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2jfoeuvcv.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2bxxsecgx.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jnkmotvh.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2zoeiafni.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tmfxdqfr.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2tbvhvgxv.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2dhgmlnex.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2kfydgckn.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jnnqcwhc.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2iggfhcno.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2gwoenxxv.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2tpakqtjk.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2zwhkkckg.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2eykmlbat.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2eftislev.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2hvvtagvi.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2fztimdmh.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2qadzilan.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2zltcbcrr.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2ibmjgotk.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2tpihbsqx.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2vifegxpr.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2wlbmuzrb.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2gvvjjjmu.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2pmsqwdtc.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2lehpnrpm.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2aylbnjiw.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2gfvzybur.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2vmruoyfl.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2fkvlepkd.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2ufysbixd.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2fjszpimq.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2mawneewx.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2eklizgwc.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2ytvpuduk.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2epmemhdq.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ymfeqpbx.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2ikjlrwlx.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2npjpfjwy.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xzucfvbu.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2ltcswnxl.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2bvypibuv.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2admckden.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2qcytzgxu.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2wtjjqehs.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dlstqwsx.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2qpugblqu.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2vksvhqra.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2liftfvbi.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2soyzyedi.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2bxswmcwb.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2fwvdvxge.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2cehmmuki.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2nurbdnjx.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2pvnzuxxn.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2kegyxlzm.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2ppeotjxb.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2cdimxqqo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ibjntrtx.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2tbmrqajn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ahclkmse.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2hamfmwbp.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2tjefzgdg.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2dpcirotn.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2dpqyudlo.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2ucmtydpl.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2hrdqjicm.html

);
来源：http://www.52xcode.cn/Article/details/gt2vymbnzez.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2fmnrmdsi.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2irnyazeh.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2tceuxspa.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2kupvdsnu.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2uquqabwm.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2sbhtvwxp.html

);
来源：http://www.52xcode.cn/Article/details/gt2xzwjpfki.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2swkuaklo.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2mgfalusl.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2drpmyuhq.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2bwppiuug.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2wsuseeox.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2peizddll.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2eldaxklf.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2jyotpbdh.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2ocrjclzh.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2vsjtswxx.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2qigqtfnf.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2zhrmxjoz.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2nbxkcpba.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2jmbpfazh.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2vjywakzw.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2lyfsyych.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2zbqnjdmh.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2shjqymvv.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2gexcrstc.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2hnmdapyl.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2txzsskzg.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2abvnnfbq.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2rxpheboe.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2vfkbrmxi.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2prdyztif.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2mwjrbupw.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2bpnuuyqv.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2aaadppni.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2jzcjvszf.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ouzuvnzs.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2wvqjoqup.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2wffecrkh.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2thjvrznb.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2htqspouv.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2ulgvojdd.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2afljqynu.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2xnedschq.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ggzkwfor.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2ydkyoski.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2pbozharj.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2awkvgwid.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2xdhkcbei.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2zlmvixkq.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2bqahaauh.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2prevezng.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jbfzqlqf.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2jvarjamm.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2flrievtr.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2vvoemfpe.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ridheymr.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2ifplyvql.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nvxpfmoz.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2aqukmqaf.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2oxljjbbe.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2dvgvqyfq.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cucbvrqz.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2cudsthtg.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2sptjhaot.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2lapahrxo.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2nmekuusf.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ttdzrlcg.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2ycqjuhbr.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2bqzpztun.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2rgfcvjti.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2cihgtyuw.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2xfynfleo.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2kkfnlbad.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2nasvbnec.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2vhdwggli.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2irdgoeuf.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2emrloiao.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2zbafsskx.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2osalaxqn.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2mvcyupka.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2uyhmfpjt.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2lhbxcoyl.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2mcabedex.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2slokwmxr.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2apoaibbv.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2uhqfzkqf.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2cufaifyl.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2twaiuyvs.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2cgridwtv.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2ugqphija.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2slvknczf.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2jgpdrjke.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2horymssk.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2rmbopgsj.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2bgxljzlp.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2cyozwqtf.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2afamjgfc.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2tfpomvzv.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2rwaawezl.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2kkertxgi.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2gudigxxb.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2cghodgwe.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2lqvjidht.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2kotxscbf.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2vntbbzxf.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2ehnculep.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2ikejcrlg.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2pbplkklu.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2uymdquop.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2ktrukqim.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2owqvindo.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2cjrilkjc.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2vierjmif.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2udylrioo.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2pgakbahv.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ktxhmukk.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2hiwnxhsb.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2wynyrzcp.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2jdaqtlcp.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2vkwcwanh.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2xedijshx.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2agwggwzy.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2evqjpjjm.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2gmhekict.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2ngigrkat.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kjgpkbkg.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2gyugeige.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2mttyveip.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2kavxhaoy.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2pnqocjbc.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2varhhvtz.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2dkjyrhet.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2rqxisysj.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2byflpbop.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zuipwozk.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2rxtwuhvq.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2urjfeevm.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2tutqgppk.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2einapvpj.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2pongpble.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2ehasumbp.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2zlrqalhr.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2sppvnkto.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2usbxrdoc.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2srqiacen.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2dilyminv.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2rxdsktsy.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2hivnzrws.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2zzeevrvh.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2pqpxsckc.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2txzdntnz.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2ixxgmsxy.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2jxoqudbq.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2mypchatm.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2fhimwvcy.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2ciaufseu.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2szaikkyr.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2sjsesknr.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2ybtzufxu.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2qvryidjg.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2rapstkoj.html


<!-- 参考信息 -->