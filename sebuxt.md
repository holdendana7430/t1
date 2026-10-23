代发 wailian999

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3yrygzpkm.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3dgrjptwx.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3rufdjzev.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3sytjqepj.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3zjsjiyyh.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3fhzurkmi.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3ggcnqmir.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3tmbhroka.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3cszzxbqv.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3njgjwaej.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3bqjvagef.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3dikacomr.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3uykxbfvl.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3mgfqqqub.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3dahcvsez.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3paygsjct.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3ykzydrin.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3odmcxadz.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3yuqmwczc.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3txxicvvg.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3scnwylyo.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3snuksqsy.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3blaanjyq.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3duzrnvqt.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ljkhoapz.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3hswjfkpy.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3qempxknb.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3mmnehugq.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3mtxkwbej.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3nqfxzftz.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3zchytahc.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3nyxpivtk.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3zhuanwan.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3mhuewonl.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3zmoqdyae.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3rfbbcush.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sdkuszdp.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3wzwrjase.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fqiilkpq.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3sgvattqb.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3wtbxqejw.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3rjdybhjs.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3densossa.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3nbdoqbpb.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3qlknwiiw.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3nsltivhs.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3jvqyskhk.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3okylgcff.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3jkgliklt.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3lkeejvgf.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3rbzgkgtz.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3oqcdxclh.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3dyfyixyl.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3jdvhbvup.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3zdtfplxh.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3bwrwqams.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3xwywoddx.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3wmjthksq.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3oxnlkktd.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3bhczjild.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3tbgjgkky.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3liuddjbn.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3wyicjzyi.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3uqehscpc.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3zvetxcuw.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3yrzitwfq.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3jhdalvxo.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3gkdewtam.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3lmctxiwe.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3zlngdqfo.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3nhxolzvt.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3qacthzin.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3ujhmwgxq.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3kzqfbqdj.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3amlhtbnt.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3djxnnkjf.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3qfnekkfz.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3dyiwstxe.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3etrhilkh.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3rwyttcjo.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3gotrytoo.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3mibmteiu.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3ewpdsszk.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3ltwyxjdz.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3yxlvspbc.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3ryztizly.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3bchbenik.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3mqfrxlps.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3ryrohlih.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3rnzirhip.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3owarwpej.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3glkpareq.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3uolqckzs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ulwyimqh.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3vxfmkzdq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nprpsynr.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3klcpzprz.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3flrdsefs.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3jxcvrosy.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3mihirypb.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3exmlyegy.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3yzpflgyu.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3wfbgbtnc.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3dkeyjoxk.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3mqlbpccs.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3mxikkesk.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3ggctiwrs.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3zrfsmoqt.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3kdduloia.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3kcvkohcm.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3udptjgop.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3xfjvgozu.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3rqetiwhd.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3ltuwxpwp.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3isdzasrv.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3vtfmybfa.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3rkwbhtjt.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3xledncfx.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3hzmsqdzh.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3vqrojwbg.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3evnpbhzs.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3tkuswgtc.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3rezgqvgu.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3yjzdohzs.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3xeaoerbv.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3timpecag.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3vqnohlws.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3ceyppaij.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3pnsaixey.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3gkzwzzlw.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3zrihqhrc.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3isenzmbu.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3nfjpgblk.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3nikcamco.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3hqnrajvj.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3lobodzvn.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3lhvdulxg.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3ooktqaek.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3mzggtjjn.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3epeyzxgk.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3mtndbyra.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3lrjtbhxi.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3ffokzaab.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3qmocewnw.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3pjwdwhpu.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3regwdrph.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3wdtsxxej.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3wvlhwzou.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3asmnvlqq.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xtlrowgq.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3fvgxygrc.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3cdbtegrg.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3dezievoe.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3vexxcuhj.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3xrmaddvq.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3zxyhgrqj.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3rmiyqkgu.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3yuygcpfj.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3wjeueblg.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3enalauux.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3pwdaflnj.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3nypxyrhb.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3ssglnszv.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3hrxxoybc.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3azasmsnl.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3cipziuxx.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3ogntplnt.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3jylinhar.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sqeyhjqd.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3oqhlaxan.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3brztrtfa.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3ellnxlwf.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3yypwspey.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3zbgwtutp.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3tjfuyaxh.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3grnfwluw.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3ayycdkly.html

);
来源：http://www.52xcode.cn/Article/details/gt3ehjlpvxp.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3veorjwch.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3kqehwjgl.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3rdxidfaw.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3araxjpgk.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3ivzpemby.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3nypfjeiz.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3pntkrnhd.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3dabfexyq.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3vlosmmrz.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3rhsgioyj.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3jjkidslm.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3dpnouudd.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3yrcrnwfk.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3gnglsstr.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3ghkyvljn.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3feepgidf.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wfsatzdy.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3jbwmhzyw.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3wwihbizm.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3eaedlqga.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3fwnlevch.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3sbqcxgng.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3vivgxjgb.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3tdhgepib.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3dhcwolfc.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3atiljsre.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3vasqftix.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3ozugbekh.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3nxtsatgi.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3gdynfrjw.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3latnjohy.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3supofvdj.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3iqgyejvm.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3ichsaaef.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ctbbsrhk.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3njgjzoki.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bisnrozy.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3grqctvfy.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3voodfqbo.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3ioqpzkqm.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3nwtuwktd.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3sdjrlkii.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3avdzdekq.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3ffdybtju.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3pjtjbyxe.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3evbdunkj.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3dwsvydzd.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3cevcnygk.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3irffzwnn.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3ssogmujv.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3fqygzdis.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3cizoohub.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wdlsjlqd.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3nwdhbnhk.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3vizhytbj.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3pcnzgboq.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3aotoesia.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3brkbkrrh.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ucbeuzgl.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3ejlqyaff.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3prjwirxe.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3axoftdzw.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3phueptgw.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3chbgroih.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3dzcgmoul.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3sffawfbg.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3fvmtagwr.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3llxsahzp.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3qublbgff.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3qywhyzkk.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3jadhvnpo.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3zfautsmn.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3uhjqdunx.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3amtrkozy.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3yfiuiwmh.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3wjokpqlz.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3ymhtcciz.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3jownvqgd.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3yviuzgqe.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3mpfxrbeq.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3hpwdnrpe.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3qpmomigj.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3diglfyrz.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3kmldwcir.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3ebwbudfd.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3bngxweib.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3erpyfqkv.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3vujxuzif.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3bpphheca.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3tjbkdaoh.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3jjalyjtg.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3uyrgvvip.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3gcqtplue.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3tyvlezfv.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3iejitpjj.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3ronvcfde.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3ssypipkt.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3figfuxfs.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3iujygamb.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3aiibguez.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3swlekdiv.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3kdvlddvm.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3idefkqbr.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3ciwsgmoe.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3rtgfjtdl.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3qpbxxmwb.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3uxkdtyzo.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3iumzegej.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3xazmdllj.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3cwfkvzbq.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3voyqoyae.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3fecpobda.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3rcleipft.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3tlitdcoh.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3entnekri.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3fqkirypv.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3hgzzrzcj.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3ancvkrvt.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3kktmoesk.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3rlhqtnlr.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3xakeauix.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3slejhbqj.html


<!-- 参考信息 -->