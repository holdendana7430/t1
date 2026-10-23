代发 wailian999

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3pdphgqmr.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3zsusedoj.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3lybcxeck.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3iuoanekm.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3axzweihm.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3swyaozsb.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3fxzgtwog.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3epbipyvp.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3jjyruypw.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3pvugimyb.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ikkdurxs.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ktiwlruh.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3zgypmidk.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3wwxicgon.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3jfobjzob.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3qbdjecax.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3eejmtxix.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3evuzcawb.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3laqdsuxy.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3kdbanjkn.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3nghbwsfl.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3znhqagvz.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3pnhycwam.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3swwdonon.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3mynvpcse.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3fiavoimf.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3vtfbeubl.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3jufrwxfd.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3joaodpka.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3rqimutcq.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3axknvnah.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3xpcslfhf.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3qwfzzeeh.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3rtrzipqn.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3anwfrplj.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3itnyhppc.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3zmvdqisw.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3tpiwisom.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3cyvjsnjb.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3iwmtmpke.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3bmkrijso.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3aqoaywxz.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3dwaqjqll.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3vbbfxlzs.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3swpwpmka.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3hpdnqgud.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3tztwyofo.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3pnhpvojc.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3eymexmyv.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3gkfdigbw.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3alhbtklq.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3xzxkrmsx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eslramkh.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3pcticnsx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jdoglchr.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3idxqzuth.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3anvjymbr.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3lvmvmbck.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3boququll.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3lazysfmv.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3smdobzpj.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3ddrzmzvr.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3lrddwjxl.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3ekzavjlz.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3lcujewqo.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3qvtcsphn.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3rpkxekhd.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3ymrmzqmo.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3qtdwnsmr.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3whnimqog.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3rbrxnlao.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3jnvsjuer.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3xrludjtd.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3azgqmlgg.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3bxpohvph.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3bknarlfe.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3cboudqxj.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3juzyndnm.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ufzbkfyi.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3idjzoenm.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3byspwpeq.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3hprzbdth.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3vrbjtxrv.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3amzqocim.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3obrxymts.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3yiacqcza.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3aghutiop.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3erbpghvg.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3noyxhnlm.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3ibwxcadt.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ssitblsn.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3szwszzko.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ypujiwme.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3ofscxken.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3mwoajlwc.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3kbhmveah.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3mobecdhs.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3xmjnxbfz.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3izexdbqw.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3eiklhziv.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3mwfgvelk.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3acpmexgx.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3kwtwqnnt.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3tppamcui.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3kzklbjvu.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3xsafxaas.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3ttruqcde.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3ekwludam.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3nkfumjav.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3topkfnbh.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3kvaclzgb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gssqgbim.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3pyffmjsr.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3tuulpubo.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3foxxfbnc.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3kqlsdong.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3ueeuqajv.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3fzrqsixu.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3liqpiifu.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3wrjkqhhm.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3avftyoyy.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3hbjjojbf.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3omudqgzi.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3kxdjeshj.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3symogpwb.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3kbxvwgim.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3xzstrcng.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3zrtpxphe.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3xwsjwinn.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3drbnqyfo.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dzqaebza.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3arokgzti.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3xzkbjvtg.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hznzxxup.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3kfxfldxh.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3jirmxivq.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3oowglqud.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3wnasqoya.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3eeyibhxf.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3hsqshdju.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3njglzvav.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3gevjfzmk.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3jlrjakfb.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3nubexupc.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3xviebakm.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3uekuwzge.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3wtxeogex.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3zyjppbec.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3bjpjvpmj.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3bgckvqol.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3kojxgwif.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3kwwagofv.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3wgfkhcpg.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3hpftcsae.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3vdnusnlx.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3pnghcafj.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3voljsylh.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3dhdikpxf.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3kuzneqks.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nsflostw.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3gujziojp.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3rtzpecyu.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zyhtnjrd.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3gkvmarrr.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3mdjmkscd.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lphqntmb.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3zqktztnh.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3stwydiio.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3evohqzuw.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3eqckkmrx.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ajxudgmt.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3oafafezy.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3jqlkgtvr.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3tbkgibor.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3ukuvorxr.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3ptcwibxl.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3wswifncp.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3syjuatxq.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3itsumtsz.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3wbuahrse.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3jysiqeuq.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3bjsqqwdr.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3ocqoolvv.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3nambvzbh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3conzajtz.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3viqukotu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zbilufbr.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3pqvgsher.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3wycktgux.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3irnpdlop.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3ushpqugm.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3nbyvxyle.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3ivwgubuk.html

);
来源：http://www.52xcode.cn/Article/details/gt3badqeiyc.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3lvvvgqxv.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3kzkkdyie.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3ligtpjfd.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3vltscsiv.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3rrjokdlz.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3cisgghus.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3hnsnczgk.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3pcgyepkc.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3anioqepm.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3updyzzqh.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3qqtzdvxb.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3vhfdobsa.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3soidixka.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3vwuyxwyo.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3rvtqegdw.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3hydlxpbg.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jahjgamg.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3nrhssqry.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3brgogusw.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3fyjtgnbc.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3bwugwybh.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3ezmdcpzt.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3nmixiwsn.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3feveigpm.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3xyjwnppx.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3xsiaigfb.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3hdnegons.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3rfmiyrbp.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3glcrucrq.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3otlmrldx.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3erlqpaps.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3rvklfwdb.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3ksjxccne.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3atprdvyp.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xttpwyze.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3xskqgzwd.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jrbwqxud.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3slzcdjlf.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3ncapvxtp.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3gvpttjea.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3lejmwvlz.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3xpvuppcf.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3ofywmzen.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3hhqmjpgf.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3euecqkvc.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3pdfiosjc.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3oausnchm.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3gtcoqifw.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3huhendiy.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3wlflodru.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3urnvlxdp.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3nzvxzpto.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rlvmktoa.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3nuclnesz.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3jcfyhbnc.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3raibhbtx.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rtqgdkmu.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3cqtrdffk.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3djgbdyam.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3wwubcrda.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3vhehleou.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3psqwoaes.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qrjworvv.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3oujfjwlg.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3hixxbyve.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3djbvhzhr.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3svwdzifr.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3borsaeph.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3hioqxgrf.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3avjirsxl.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3atltutla.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3akerkrpz.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3ardrqrly.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3emizcyha.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3tosifopx.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3actbmlxt.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3ojcdmqap.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3hmaxvfnu.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3ytjqfywk.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3qhzgehye.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3hafqrzrl.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3kgknhyty.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3wzxjntje.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3zxncuqve.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3azcgmbhb.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3afoktezr.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3pzdcmdni.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3zcmftmao.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3pomqwkij.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3sspxhtvd.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3ogriljwf.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3dgzolhdn.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3ikxlyrwj.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3xiuqjoso.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3mvnwvsvm.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3sgkyaphr.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3iqauqstw.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3nxtmjbth.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3zeqtfisi.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3jyxvvvhp.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3miyzcgbh.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3votvxkwp.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3nvqjkqam.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3pwgjrmav.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3inozjsjb.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3yhrumrcq.html


<!-- 参考信息 -->