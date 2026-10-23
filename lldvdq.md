代发 wailian999

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3epguhvko.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3xwcmwbas.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3scdsuzba.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3yhznwmvd.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3jcjdoasz.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3dktvitab.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3bksxhdlp.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3ptqymhuh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tniudppt.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3bfloowvk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ysumoghe.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3frintlhy.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3ihmntsub.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3fgtgmfjo.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3glxwoshy.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3objjtezf.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3rnsfmmqe.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3ffznjkix.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3npfdjiay.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3krrcaolr.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3bguleryb.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3hnmanikw.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3fczhrvwp.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3nbzllzyi.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3jvsucnyu.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3dqaofawp.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3gbobbpkh.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3rxchwqcu.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3zexowyip.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3hubhgdvl.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3ultsfqta.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3xubuzotl.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3eskbabcp.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3opeupfer.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3cbyjlgoy.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3nfwtuiin.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3buqmnfho.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3cgadfnla.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3gtghfqya.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3fpxexkdx.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3imjpuduz.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xvxycvln.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bvnykalf.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3gtpoeptp.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3nffqrkns.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3ezcxzcjs.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ryvoselc.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3qbhkzonf.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3rjzrvwic.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3cvwfklfa.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3zbcsqidr.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3pticqtjt.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3sijfyplt.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3mwcvbuyy.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3fyppjvml.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3uzvuofxy.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3ckrafjaq.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3zcynfpjv.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3cjxgornu.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3ymifvgmm.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3uwnrugul.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3qdonpxwz.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3lxctvfyg.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3ajhwqluf.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3ssepkcxk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rqilbfmz.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3bzggrnvu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hjvtouup.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3ozjsmhoz.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3yywxhzqi.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3xeznvylr.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3rjoihhna.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3vllxdvfk.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3ajrxurzm.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3jojmgkka.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3vggmabjs.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3zphjpmia.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3tszcdvny.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3ibrkulbb.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3fhsyljbq.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3wrqsocnh.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3rdwtqmuu.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3itzujwfq.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3vcelyycb.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3zuuzbpsr.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3nxjtwxxa.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3uvjjagdq.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3olmtfoqm.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3sxluoihq.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3pjztcqyo.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ufwpsnkq.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3yfmjqqxv.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3mxyooskj.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3cekhxnme.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3puciwlfo.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3jdfxkdpo.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3xjsmmpht.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ckjxiooi.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3jedghouf.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3kspjmbyt.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3ijbogbsh.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3kmwsqhck.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3yxfhnrnh.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3zyxjlkmv.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3jyodvszd.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3gnpcixla.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3vrscwkzl.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3bemaizig.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3ztcbcylo.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3ljrxqdme.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3xlfnoxpl.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3pejdmahy.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3rneyrxxh.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3mmmkshpg.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3yoaknasj.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3ppijfwbt.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3uluhqdfb.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3cykkidbb.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jnnevdru.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3dixuljmz.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3kmrlthnm.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gbhnifxd.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3nohtkarv.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3waqbcxlg.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3norhryui.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3hvncopoe.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3nnvjjros.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vuqckbwh.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3wtnjlnma.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3iztnbhug.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3nwuzrrlc.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3ehkakkfj.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3msmvtfqb.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3symtljbz.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3ouhslfgo.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3kobxmmsf.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3padueljx.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3efsgksga.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3nxvbhhea.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3hxfkoowo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dxntnfqd.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3fzfrywyd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nncdbdod.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3ryaccybr.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3qbwctlyg.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3seuctilx.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3nsnlcslg.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3cttptuhy.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3toupqjej.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3nhaygcrh.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3wcbexjzq.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3aimmiugo.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3sewmafbl.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3qgmsythm.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3jehnuzfh.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3znpshelg.html

);
来源：http://www.52xcode.cn/Article/details/gt3ebzswcxa.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3upccrlqp.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3lllkjosg.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3omfztgfx.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3ktymqgma.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3xcsckpog.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3nfxkjbsp.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3vhvbgcwc.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3dzvrkbah.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3hsffmdrt.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3gvmhmdwz.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3qbpywnzq.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3lenxdjtr.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3kaxvbqfd.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3niverekp.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3zkqxzguf.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3ckoxlwil.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3rfolsolk.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3atsqidfx.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3eusmhsjw.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3cqghftjz.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3tniztxbp.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3autcglud.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3llczkaph.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3gwhjtcrp.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3bbuztcpz.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3qjnlgbee.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3oekkypzj.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jexwmmru.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3scvcwpae.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tlagodjh.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3tkladtmm.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3yplrmhgk.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3vhwdihkb.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3kzodtfst.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3xdwhralp.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3kzdgsust.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3wmdnkyqj.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3polwnbmj.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3podyzgev.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3taedrjrp.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3mrvdyiks.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3savubtnd.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3sxorxtxo.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3vazmjmnf.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3jxfoocns.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3quvyypvy.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3ysibrork.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3acyufavr.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3ukkyqhej.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3eiofqzsa.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3ixhtmgtz.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vlshopcz.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3pskxvoub.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3vrlyycme.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3jcoishwg.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zyaajdzs.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3hcicsvjq.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3xknxfjsm.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3yjeexomr.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3dtiwiqlu.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3znmlfrkb.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3mrfeccgw.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3wlvmyaxu.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3rvrvdkwn.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3ikoqemxe.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3tviwcxme.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3mkxeuxat.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3dzsdbycv.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3eoomwdrw.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3vsvrmbry.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3eplaegjs.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3tqjroghm.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3zosmymrx.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3oufkteri.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3wpdqxurd.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3fngtbvpk.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3puoiaiao.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3bpsgtqqc.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3wuwfeslz.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3shtwhafm.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3zmzcwyfj.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3wjxgppja.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3ozgghvdu.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3xwwcvgkt.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3ngzobjua.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3hqjswmey.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ixtlvzal.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3tdbybipc.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3dqdyxtzw.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3wsqigsjp.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3djlcatal.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3oqbhutbn.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3ccwydqjn.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3tinaante.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3oeesmwtr.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3ukffofje.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3livfziez.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3lcvpbtte.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3uynknbje.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3vyjaigke.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3spnkweas.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3ejhepudt.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3lelvdmir.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3zbacjnty.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3mmzukovo.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3jqjikytg.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3fpqpoyjc.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3xrkgbsnj.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3esundqqc.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3fbabiqnn.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3vrnqbihw.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3cmmecnzd.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3huddnpsf.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3qpcmxhjr.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3xdoqfslr.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3rbyeguru.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3nsifesdn.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3dsxefsmq.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3zoamoaob.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jslsllne.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3fruciyfr.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3cvrzltzn.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3btyzsryd.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3rjhgaisx.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3kljtytkb.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3murwzuuq.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ybpcwunx.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3setoolrl.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3qzxsughq.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3gjstuwwb.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3qlxwrcyq.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3ialqmvej.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3tmfatyqd.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3pbjewaco.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3evkbvioc.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3ljtdrjdl.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3gymiimok.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3impuydsh.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3vtudxifj.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3zhvubfwz.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3grttcutv.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3kpqppfwy.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3xjspdcub.html


<!-- 参考信息 -->