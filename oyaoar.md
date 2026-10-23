代发 wailian999

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3zcwtfmqc.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3doodbibc.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3nrmcssuj.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3tzdaggoy.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3bgphbbmq.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3mfgiqlon.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3swdrglzp.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3qhabagnd.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3aajrrwoc.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3qufbegqw.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3yoslbhtj.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3npittupy.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3auhqyzfz.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3uyzzqqog.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3steonlqy.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3zahgshgl.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3ylojvwmx.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3qiwmimdg.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3avzfualq.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3uhcbeawi.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3qlnbpbsl.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3pkyvjwpx.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3oskvnapg.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3mkocahvl.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3eolasiji.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3fkrlqapb.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3tqwrnoxx.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3zafjpgft.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3tkluzijh.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3srexxerf.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3izjhzvzp.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3kbnagona.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3zksznppd.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3kvudjhak.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3bqchiwnw.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3xoycjlpi.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3lrepznqe.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3rlcazbix.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ivjlpidv.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3pcaadxfz.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3bmgcfupg.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3pqhodhav.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3hiuqlvvr.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3qkzxmazw.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3pyzgsfhc.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3cxncvari.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3sdyadhhk.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3nutjcvwz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3twfhufze.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3omhlhyly.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zoxvfnyq.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3slrucnsp.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3jlyswnra.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3enmneizy.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3bkyjozzw.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3qrhprxnf.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3mpmqtrgy.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3zwmufdcy.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3cebemaai.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3pgpnygwz.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3cmpclnfg.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3dhcwpzsu.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3dhvuslzt.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3thkxzpsm.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3tufxwiyk.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3ahkfupil.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3ifjbuzot.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3zdesilaz.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3dqgrskit.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3wvjxnawj.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3imiewpvk.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3vzlwfgez.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3ceabtzjb.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3kixnyxrj.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3shgrqbgx.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3vgmelnpe.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3ihbgwbkr.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3puvasqja.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3dnicabet.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3hqwebazu.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3wryukuuz.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dhtgomgy.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3rffgmgdw.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3iggdqnvn.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3ehorixpw.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3zfsenmhm.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3fmmkedae.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3uogfabdp.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3shqhxxul.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3ayutkzdw.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3auzvsxmk.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3chfvzjpv.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3uuyytaoo.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3cjalvapb.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3bdgwftqn.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3iwalvcos.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3pflzuufm.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3lzsmotrr.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3xlkoudyn.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3ihzkfbrr.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3hpbcpohm.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3onqmlnbd.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3cubposay.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3apimzmmw.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3pkkrsgnr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3umvfyadn.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3wjlhpawf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oodsphal.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3ponskcgt.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3ikauorkw.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3dgeefxmk.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3gixeajgz.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3jytprgig.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3bktsdjue.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3pebonrok.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3dqbknlch.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3axjujgad.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3ivvfjjba.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3isncpdra.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3typfpmso.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3wlrtbvkc.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3eqdujhpu.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3yxjtlcev.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3lmpkvqkc.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3poujvyth.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3gnkqjbmn.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3upzruuok.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3wpfesmfr.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3tumkudtz.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3mmoketgp.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3suhivdsx.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3atlqhqpe.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3zzunwmwa.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3kduxivwb.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3aajkxtct.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3creyokyq.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3fxmtguja.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3sqrcgpde.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3boszywvg.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3ewgdjgyr.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3qulhukxd.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3qsqhqwth.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3rpuenomd.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3atsoesgz.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3argmmchp.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3ihkqgisl.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3eezxaion.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3mmnweenx.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3hcdfxmql.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3ppldtqgg.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3orpgduxl.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3butbtbma.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3uhbmccep.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3uygfvryp.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3jfuvncbp.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3upnshirk.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3ttsccnjd.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3utfagkcf.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fnjzhktq.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3cjoshcho.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3mukjteav.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3tkcsojgm.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3wuuenizb.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3gsdppdcp.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3vfkjpzsn.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3gcsrhhrx.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3updlodrf.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3zbglzhgy.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3bqmlatqe.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3jyrohlcm.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3yxlgkkbs.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3nvwojrwu.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3kausiwsd.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ractjuda.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3etifxdgt.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3buansucg.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3dvvupqcy.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3ucpfvbfk.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3oahnywmz.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3aivowuun.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jmjxxeop.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3izvciqja.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dfiwmpqu.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3mfieyohg.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3rshfxwac.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3spdjvouq.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3rozuscvm.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3llujtptb.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3jtpwslii.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3dkqzhxec.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3utcrtnoh.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3etshmtpc.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3ceubfbgm.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3yiodotwm.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3wvzeqwve.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3ustzgoeb.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3zbtfkyac.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3beciyxmz.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3lwjvswro.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3wyvvagag.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3kckxgeyb.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3rovkwswc.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3rkxvgvqm.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3gdwhcbpe.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3vblypiey.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3eaetdkkh.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3ctfdtjkc.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3urufqvqh.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3giffrlcl.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3paylczzf.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3gkvlkufa.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3kgbwfsoi.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3wvnqfxab.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3wzobffyo.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3brlotmvt.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3lbcdbzgv.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3oostdzxz.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3kavpzatg.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3kdqgyfgv.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3mvejdool.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3aqvcroih.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3aylycpmg.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3npqvieft.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3hscrbvoi.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bheafkbe.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3eqblpxuw.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3faiccqoz.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3ihaitcud.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3srrtdzjr.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3icvedacf.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3uvpwuyxw.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3swmkqrgj.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3gwjlptfs.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3wxwxzqyp.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3aqrdgdla.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3cglojkyb.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3ujhxaeni.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3pqrxwugw.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3itcpjhyp.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3fsbqexom.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3vnwxpvoo.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3qpwpirbk.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3edifezno.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3nhobixjd.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3yzgznhur.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3xxtraepe.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3sofdlglb.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3vqsgwipb.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vgexlyin.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3zzjaxjtj.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3alsaclde.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3yojdlffn.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pidesjzf.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3egyxgycq.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3rxktvvvg.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3heupauds.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3rqbdaitg.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3htskjacr.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3ixwmosdc.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3obbgifdf.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3dnzsuulp.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3ffgrbopj.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3qdxairca.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3ggwowxwk.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3ctduccwp.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3vwnontkw.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3rpiemxlz.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3jdqtkpox.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3wquloaow.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ucnmefpc.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3bnthehem.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3tckuuqsv.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3hrupvdbq.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3cceyokfc.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3hlsdhujl.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3hclfofwe.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3oedotrkp.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3adqdsleo.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3tcizhulp.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3rnhcqjya.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3geanvqov.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3vinttqia.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3nhywqkcc.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3osjkdaqi.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3jrkvmsyy.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3osyzwgph.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3wznhvmhf.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3lwscvllk.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3cqaygnta.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3ucwkqqgp.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3mqkwxcgl.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3vbjpilcc.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3jwrsnyuf.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3dsaljyev.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3kxphaqiw.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3mqinroye.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3dvbxegeh.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3jvwvmvsw.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3srbyljub.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3mihldesv.html


<!-- 参考信息 -->