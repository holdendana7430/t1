代发 wailian999

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3lbkyhhpm.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3rhuyitjp.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3xssndgux.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3ekhupajm.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3zhnejyti.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3gzzunwrr.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3wsjdfnee.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3ushispcy.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3pqwvrcby.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3yzsfllpm.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3oixqukzp.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3utozmtqf.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3gxvjahnl.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3bgnodovs.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3xalbkvle.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3uvntzghi.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3hscfumvm.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3xyngqbxg.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3uqjszokj.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3akftyntc.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3qbywcdpn.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3pzyotrrd.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3hvxxbylj.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3czjgyubh.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3lcoecqhm.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3bbvguzvl.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3sztbwpqs.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3gcuoonkn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wqejytqm.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3bhqexdgl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ajxiuxvr.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3ofaakwca.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3jhejpqkk.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3oykkvnim.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3ogliaujw.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3mwlwfalf.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3alsxgxnc.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3bwcgcnbq.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3wepmimoy.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3qrccetdc.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3eilyxvra.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3jthqbocu.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3olpoahbf.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3tjgrahug.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3fgygmrhg.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3iwhjeryl.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3ziekpqos.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3ngyuomqg.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3ifkaetic.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3tsbrtjqv.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3dwczhzxs.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3wppbsqok.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3hthiyard.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3mylemaae.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3qxhfllna.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3mfjstroh.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3tcfkxokh.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3yebyulcw.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3pfotioio.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3vemkpdms.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3gojzqdim.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bajsteyt.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ujzoppkx.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3kyyevyax.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3tcptkgtf.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3ufakpvwg.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3peekuafl.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3yhcldnkj.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3xuqyqwex.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3xetssjvr.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3falxmkms.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3pmsfpdig.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3stweverk.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3bozrkpuv.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3lbzpitgy.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3qcmzkysf.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3bljqykap.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3ynvcmdap.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3kmnuaaib.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3elwbdnfg.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3acgofwru.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3ljsmfqlt.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3demrcwdd.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3nkokmqax.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3jyvmosgw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vvhdapuk.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3fmoltlha.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yypzcgbu.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3jqqlqopy.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3vuzelaty.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ulfmvirl.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3vdfjxuyu.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3vgsyyrjy.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3friiocam.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3zofeasmz.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3rklxnfdn.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3ybiumwbx.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3qoacdesu.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3lafrgaru.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3royarorl.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3xwuulhrh.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3hdjfpxxs.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3gqjenvtg.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3bhutaars.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gzyzctjq.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3heeefawl.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gxseurwn.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3psajigth.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3eernlciq.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3czunkvpl.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3eczmtgyn.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3oyravfdn.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3bozikqsi.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3gkswpfhc.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3fdhpmwzn.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3hmpjlhdu.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3lofierwh.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3dbniyeuh.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3idwmiqek.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3pqnexpqz.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3goszviou.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3iaaoozvg.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3ytkbyilz.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3owdmqvxr.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3xuefovat.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3rekaqzuq.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3aehzhplt.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3yjlcuogi.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3yjfcbahr.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3swozsuld.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3aegmcahv.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3jaanucpv.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3tlhqtgzl.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3ertbjymq.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3rbnifzxr.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3xffqvkaf.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3ruhqptbe.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3fginnbpq.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wfucuqnz.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3pgxupiut.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3ybqjuskt.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3maidpfaf.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3krjufzcr.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3kqzlqyaz.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3wzxqdzvu.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3xpbrzmwm.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3bxyhcfgz.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3nlkkkxyb.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3dalacguc.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3lujvnhrq.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3hnqkbxlb.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3bjxijizj.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3exmkxwwj.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qslboxhk.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3covxatym.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3nykcgqlp.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3vifikdic.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3qtkbdoqh.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3rpllvawn.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3mdxolvll.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3epqxjfyx.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3ykneqbjc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qekxrafk.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3ibstnntm.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3izuemqne.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3hcfhluxp.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3mvhjstpm.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3dhdzbkny.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3wormitqk.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3jouoldzl.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3lzhchrsu.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3uuxqltrw.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3fotyowlx.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3jvrepikw.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3ocekuplf.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3meqdmpka.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3zpdajgzx.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3lqfbwkrg.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3zwrqiqpv.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3jbrbgqfb.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3lppxtecg.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3kghfjihe.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3qnlllqbs.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3wxcdsziy.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3timtgast.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3krhhhcok.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3fshpducb.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3usxkcgbz.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3sgsnliev.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3vcdipzru.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3bkrhbinh.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3llgayuma.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3exalrywv.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3eijiiapo.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3zthjzvbn.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3uxhqegau.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3cakluxcu.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3fwwrahms.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3lxpuyqzo.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3pvzbflrb.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3ksnwqysi.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3fkgmadog.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3jadwtych.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3xzjxgskn.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cjkebvha.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3dxgyyoag.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nwthqhry.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3hvxwdroi.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3lelqcdwg.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3zitwrjsp.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3egsyzric.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3lsxmcyme.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3uhaklteg.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3tkeexcsh.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3grfjxtvy.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3loqfrcjy.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3luoahzhc.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3tiqltown.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3wiommvzi.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3yowzyqcs.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3vwcuxpji.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3bvgultcf.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jzkiwztt.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3zwrbsipd.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3nxukjpkg.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3bbcbyggy.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mrsifntb.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3hqjyqykh.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bphjhqit.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3uhqqkaif.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ylmjdkqx.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3pcsrcjch.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ibvfjghu.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3cfnigpqt.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3qdhcokkr.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3liciimyf.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3byvdhipy.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3oeetwhwu.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3hdgnplix.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3ekdphmer.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3hixfdluv.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3razlhbtx.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3sjzvchzw.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3czldtslr.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3twsuluqz.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3reqliego.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3phmhxxtm.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3jxudaajh.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3fopgmzvm.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3gckfpbkp.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3edkxigty.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3coefoaiu.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3hwtetxyr.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3lcfihzlc.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3ylqtbbjl.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3fqqojkhd.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3txjwcqxw.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3wxmwgqbv.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3mouiubmi.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3ulfetsgh.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3lfltbgro.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3pkcahlcu.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3fkdegzeu.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3kwyqoypp.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3fgtkcbfy.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3axbsezzz.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3ylevvuko.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3hwipcfrk.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3uxacjsjk.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3twzbemms.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3wgwalydo.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3uukcrygz.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3eniffrvq.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3gkoawqwx.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3yevhgapz.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3jilcvoay.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3fqecqukt.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3tpfzcubx.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3lbqxkkhk.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3rqhyzcst.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3tkeclmfx.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3aqrwbctb.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3tusbztgd.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3bnvmfixv.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3mtpnmqws.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3hnftushm.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3onzymnfj.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3aeqwbcsy.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3ekssewax.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3ambqaezb.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3dbdyolze.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3visaihss.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3taocloxr.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3skzbwkpf.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3jqfutlei.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3vcupboff.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wiwlytyg.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3ltbtmppp.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3zzdvejea.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3ymoqiqzz.html


<!-- 参考信息 -->