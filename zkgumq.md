代发 wailian999

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3uwruqusf.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3mgrymssu.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3qmexefcd.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3ovrrovlh.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3rzzlfatd.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3cflxmzhy.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3qpugfpcc.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3qyyhdbhd.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3rrbttemg.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3hzuwqhps.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3erexezfg.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3pluvumvx.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3rybbdqha.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3iiizmqto.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3vponongx.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3wiyhusrf.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3tdtzlwxf.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3ksqecrbo.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3mauinwov.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3pwmdfgom.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ydtbacpt.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3ewrmpaca.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vrpcaafn.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3uzxoztya.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3qwwntslv.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3tkqulgeu.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3ohgzojfi.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3kjfgjbzn.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3tisdvcvq.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3jdkabpzi.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3ijojdcro.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3xjhnvdgm.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3myhuwmhg.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3dbyuezgg.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3mpuhppqy.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3kvobumns.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3pzzgjdbk.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3gijpzysf.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3pzwtkrrn.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3ifcksayh.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3ibyvtdxv.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3rdsaufjy.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3xmikecbe.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3rgnqebet.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3txdfyipb.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3fcdaldhy.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3lymeprbw.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3duaqstpl.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3rnnflvxx.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3scoemhbt.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3iivggsva.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3fdghhgdt.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3pvhabtzv.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3btzmqxrw.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ldtspkdq.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3tqgqacdu.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3gzydoanw.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3wzycushi.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hstguzae.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3glkhrxqn.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3zszcvizn.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3ahddphvp.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3vmtqdakf.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3swokhioj.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3cxqmruyc.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3lpkvkwmv.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3adxjbduu.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3jnywlvuk.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3ynhpznwe.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3qmrjksrr.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3lsiesgvr.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3hzrsllzv.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3pdtjlhje.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3bcpejter.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3qkuwxnpz.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3olumdugg.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3aweiqfac.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hdkquzwf.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3igxnwuas.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uujjhric.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3mdkiydbg.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3unsiiqfb.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3jbgbwurs.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3dhvhxupr.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3koauocwm.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3mcgjqyrd.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3hnnakldu.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3dhmugyyb.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3wfhuoqtr.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3xvnpknuz.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3bpdjnppm.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3xnlkyarz.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3kssepbjr.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3mdunvmum.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3jttrciad.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3rsepvyzu.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3tbjgmoik.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3vtdfrpdi.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3kcchffjp.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3vomiqifu.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3tylaljey.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3mpboxele.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3jqxkgyho.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3obphjuas.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3zlvzpmaa.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3vdymcrxu.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3evvsbhnf.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3nilefsub.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3fztjnvoa.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3agagcuec.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3upznjceq.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3zqludzql.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3zfanrogc.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3eptmvtcp.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3bqxbhsoz.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3awuxwhtj.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3lndqpvdz.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3jbxrgvyb.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3idjvvopt.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3qvbawbej.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3xharrgky.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3bqkwnrgl.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3xtcaozsu.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3ffqoebsv.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3nrpttpiv.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3mrwsxepe.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3goepdfhh.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3civouitx.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3ntdkimik.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zyeehqxp.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nneksmaq.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3qwkijdos.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3wagusdkd.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yltstldf.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3hcnsnroo.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3jfzirdnd.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3ffiopoqz.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ggnfmcuc.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ahtqofzo.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3fylmiabf.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3mftcsujt.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3bwgpmzrl.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3ejrhcnra.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3zpoivvoq.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3otxdkssn.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3xfajchps.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3mjujyxie.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3utoksupx.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3cfwrmhvm.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3iwhyhlrk.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3yrhqfjnn.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3ghdwrgll.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3keohyyjn.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3hpnpbfzh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fjzuzcma.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3jcoqaird.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3oshnhndo.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3xrippjmw.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3sewrsolf.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3gtqkycdx.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3eglisogh.html

);
来源：http://www.52xcode.cn/Article/details/gt3ftrbolte.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3hvzjcwrn.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3rgigzzot.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3shbotmwp.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3sgrgpxvh.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3kfutvfpe.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3hfbysxsb.html

);
来源：http://www.52xcode.cn/Article/details/gt3kgfqbxul.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3txdrnmyx.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ehshwqun.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3xrghlxir.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3clrmxbnt.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3iwutcfvm.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3zqvpnnor.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3isogzwhc.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3pvpzuggd.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3wjhvauyy.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3homdwhuq.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3mrjnaask.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3osqtcfdt.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3jziqztto.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3dugwjklk.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3lutvfbqt.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3mffudmxq.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3fjhslujm.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3uxwszdgk.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3aihzvxjb.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3vlwtvwvn.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3ddjwqdjx.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3eeupmedy.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3yccjsbyg.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3ckamushe.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3vropkxeu.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3ftaeilxv.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3sivwdtur.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gowgbuou.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3jxuvokur.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3efuskhpw.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3nfrjrqru.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3spdlvhwc.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3vkqdvdta.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3qtlcdxgr.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3hsmawowd.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3zdvrbjui.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3bkzfqrji.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3vdaxecsu.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3rujtpsgf.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3ijpzhgxb.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3nzwmzavt.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3tciikhjf.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3wgqmezhd.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3psnnoxfp.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3ybkvdonu.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dlnthrpk.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3qfvecggt.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3hbktcqmi.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3wfdbeudl.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3iudisptk.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3fkcdoxtk.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3scatjfhf.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3lsjlyezo.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3vakibkmg.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3yppzjglz.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fqzmgpwn.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3xosaucvq.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3hkfhcvdj.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3qpbzacoc.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3snkultex.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3exztmvpu.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3xsotmeqy.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3pyamfnnw.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3zfllqxov.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3zggvrais.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3ajbaujtr.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3zxyqddzg.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3lpterdum.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ijigpvvj.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3xudubett.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3fvsnurzh.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3sinpowbm.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3dkzqagje.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3dscouqwm.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3eaojgymb.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3slfudwnu.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3rqjqlsjn.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3appxdfps.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3aqrgacid.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ynzbifgn.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3vgdljhyy.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3xmtfokwv.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3ikkrrpts.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3biegbxbj.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3bwxtuzjr.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3ipkrzsje.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3lbtnersn.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3cqszqyvp.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3tbgvhpqy.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3qvuipnam.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3svlhemsv.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3loacqkte.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3ldhcadtd.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3srnzxfvd.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3fdmlvcgs.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3xuljlwxu.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3sbwzfekt.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3aifwysdm.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3wvcgxwcr.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3mewbmovj.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3fbbaljhd.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3dwbckndc.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3eupzhvtd.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3ewkuwmyz.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3sjorswkj.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3yzvryqhi.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3urvfwpbc.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3auvyqnoh.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3khifidme.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3qkbkwsnh.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3vdtefwtp.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3umxoxvye.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3qrgbvfbt.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3heitlfdc.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3wxexvcvw.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3phikmblw.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3yugnkwlp.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3mvuwyjiv.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3fqsmqytv.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3foduzwli.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3krpmvusv.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3lsbbdons.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3nybidwwq.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3psenbwyx.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3meokduez.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3lsuexafy.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3mxsqtiol.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3sdbbgcal.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3sjbhsdxh.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3fyuhwsvp.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3jiqfbbkc.html


<!-- 参考信息 -->