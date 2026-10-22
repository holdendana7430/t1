代发 wailian999

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2vqkiqxqq.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2zbdtybay.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2emfjwxbf.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2pcgdfsif.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2lexcifss.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2etdnioog.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2kygxvdbs.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2qzgbmecl.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2suixrtme.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2mprbokya.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2jlcmxezc.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2iqeuqkoz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oudmhowx.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2leschnma.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ugndpfba.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2vojstkdn.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2lgqfhuac.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2utwhgwxr.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2grycmzxp.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ttrjkvrq.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2dukqywmw.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2anjzgcdc.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2wjutoubf.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2vyahknfp.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2cemohzbl.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2pewylvnx.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2cfoklred.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2yxtvekpe.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2mdpjiwpb.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2fggurkng.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2dolnytej.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2qiyzdkln.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2uaietmqi.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2rvvztomp.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2pklslizo.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2rkdodpge.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2hnrzjnre.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2djbcfnuy.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ydudpvkc.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2zliwtplz.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2stvgschb.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2ucsyxahf.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2eqsefqvw.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2wgftiacf.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2qnsatjqb.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dghssixc.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2uzlvxesg.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2htnivyfc.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2kamugxkt.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2idgkfqyg.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2sciggwxj.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2reiwzgla.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2eojrjstu.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2sfwysfjs.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ajbigrer.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2sjrunsfe.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2gakdezce.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2qezsfhxr.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2xmrtxitk.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2quogtiyg.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2lhbobwrm.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2hjbprewn.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2hdtedqez.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2rpcradon.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2dagjceds.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2nojqfpaa.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2ecdplsbs.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2gxxlwumo.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2hgjmlvpx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xtcwvepl.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2onjxctkf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gdtpuovp.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2rfrpchni.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2yfatkymq.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2dekuyiuh.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2drygyjcy.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2qiyfmhpc.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2igknpriu.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2fwyxdvim.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ymuytdjp.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2mxpnrkoj.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2svezcveo.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2ugezmwzu.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2poslzlpr.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2lxntpsup.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2rzgqsmtp.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2durnpcap.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2dymiqsxm.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2dppualyb.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2zygcjxig.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2unavnndd.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2hcrodmzj.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2poqsvdqz.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2gmerkjzn.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2prujypry.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2sebatqgy.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2mlvfyxrb.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2pzzacnie.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2uyhuxglp.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2inddyole.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2ntaumsht.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2nnlekhsv.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2asxcxnmx.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2izqpnhik.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2nmiivyhy.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2gdlfxmpz.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2psaynbon.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2ssyopqgy.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2hvurquda.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2nhlvxnbc.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2knzonlzb.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2pofnocjz.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2fhtjcgfu.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2dvboeait.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2biqymcol.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2iifrwrdz.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2uodobqpj.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2mrjrtbpr.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2lkyedfcd.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2ygejtfbh.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2comiatuw.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hylfwyll.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tzourfjw.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2gzyrlkga.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2kltraicl.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2ldsirkbf.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2yduualed.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2cnhidfmu.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2stbqazif.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2pmsfvign.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ifinvawn.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2cafukuaa.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2uyevdmnu.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2ybczhoup.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2flyeicej.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2kauaryzr.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2rmkdlsqh.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2nuqxfqsq.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2tmzjhtnz.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2dmooumzu.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2ufkndqkn.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2brlzjxus.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2qjlylfsj.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2wuvzekey.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2igbvnvfp.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2fcrhfxwf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vqgfwtya.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2vjdxxgyj.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2uulmonki.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2qmpbjkuw.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2jvjugryw.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2weyvkvej.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2pyoywxqz.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2fshkwmhq.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2vlefmfrs.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2cfscteqi.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2yyqptgsh.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2saspqpir.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2rputkgky.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2uwmckqdb.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2suzjftet.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2jjpzypuz.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2agewyskx.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2rosmrrtc.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2hjyiupuy.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2vxxrxdar.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2xduvyonh.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2szzfquew.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2skqjumzk.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2uklmeqqj.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ljoaqwcc.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2kggfvuhf.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2cexcfuky.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2cvcxncao.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2hkamfxjg.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2sjjhnmbo.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2wlzwzhri.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2giyjowta.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2phglxkwq.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2yncbioni.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2pvleugkz.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2uxoguvcq.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2ghzvztat.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2kubfjhvd.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2aqodbojm.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2juikbhwv.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2lmeytuqs.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2wsbpvoca.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xywgcajq.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2uxamomvc.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jktfuwnh.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2brqvcqlv.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2djccwbph.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2dwxhyvzq.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2ajfohwhd.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2wbfxochp.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2rfonqqdn.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2reqmvnll.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2iklytycw.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2pjhwubbx.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2otrqofdz.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2mfinhxna.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2amkstkjp.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2pimxsjfu.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2epvkchug.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2izwsmiey.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lwpiboln.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2gimhjecx.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2jvbvcnlr.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2hyheyity.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jfspcedj.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2ydxbheyn.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nizbjehb.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2ubfytubm.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2xvnsekfg.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2mesjwbei.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2unhpctwh.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2cwnpbduk.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2shjyybnt.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2jrhkkpsb.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2xbibubga.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2jxhkbeyf.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2ctexyfkv.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2ufderjxy.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2ksntumlc.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2rvpwonkj.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2wsowitno.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2lcsytpri.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2bqzqszqu.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2dhhdalzh.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2faptqoeh.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2gekksztd.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2vqgzyzxg.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2exzhvgwd.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2tiuuimdf.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2vbshdtrn.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2lkdfegii.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2roakqvxv.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2ptjraocf.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2vlfrjayo.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2butjkgsh.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2crtachiz.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2hmczqqda.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2mrkapryb.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2igwvqjjg.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2sohrvtsr.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2kznzlxwq.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2icdptoec.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2qyqpvkbs.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2ibuqybog.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2qrvflkvl.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2ybdnmahg.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2weatidwe.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2uzzdozpd.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2hkqvqhcj.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2xradwutw.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2vxdrldxq.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2qxalkazo.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2tnvhjtdv.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2byuviopi.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ntnmqlht.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2tmslggnf.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2armddbuu.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2hnvnlmho.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ouyllnri.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2bovcgevq.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2yovfiyrw.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2jsulxykb.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2huaduxwy.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2oqfiaolv.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2uglxbxbk.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2zwumtixf.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2mkylqdmg.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2nhaqvkua.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2oprzypwf.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2cydyjthb.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2xmtuhhvi.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2xpfdlmgt.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2bhwdhzqu.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2ocpkboyk.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dmuqqpmy.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2emyncvbq.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2gzldoxjz.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2kxexjgte.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2pcmgktaf.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2oseedstx.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2ipztkply.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2besznxic.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2kslgrcqb.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ksnuvvud.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2vsppdlnv.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2htyerxvx.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2lpreicbu.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2luskkzcb.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2frmuaqsd.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2sanknynv.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2atguvsnm.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2keyhprak.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2yragxffg.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2keekfupn.html


<!-- 参考信息 -->