代发 wailian999

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3oijpouhm.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3cwdfdkhg.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3yotyqovp.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3tkmsrkhz.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3mjctotnc.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3phoikfzx.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3ylmvfsdd.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3whkdjqzs.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3ttgnnusj.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3wxinezot.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3kdijxkur.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3ufaukggi.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hsughmva.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3liulmuzj.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3vyavgdhl.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3gdruoyst.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3upeqtnlz.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3xrgaepfe.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3vweafvdf.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ndtjpoun.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3zmtuebut.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3xhznlvaq.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3gwufnctk.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3jymnqhsp.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3hhoelaav.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3cjqlubsi.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3bwxtqqdm.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3wwigtrbe.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3zedqxulu.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3cgwhlafq.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3zshejeyx.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3qeiouemu.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3iaunvfko.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3ltgluaxg.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3rxhuppkm.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3skvxymti.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3ioigzmme.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3gtsmkeqw.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3azujfipy.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3uivvcxoc.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3onfzkkgu.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3kqokhiva.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3zpuggqmj.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3etptspgw.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3riciytzq.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3tttmloar.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3mcsunmve.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3upbxtdow.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3qdxstbye.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3fdjrgdgk.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3dqzbmfjn.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3znkbeiev.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3muebsxfr.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3lpxtnqng.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3llsszdaq.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3olaxzieq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pqvfvagx.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3hvkrincm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qpalfnyw.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3wwrllhto.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3bamnzsex.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3dvtyjpkf.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3zkdsnetf.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3cnndkvqf.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3icshqhsd.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3xduferhw.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3edhsffvr.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3nbfafsus.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3cndlcyme.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3yodinopr.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3rxygnkum.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3jfffzosy.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3sqbppnuj.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3kmtypand.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3pwmgrzhx.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3hraprvdx.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3aiyfkzeb.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3djkbsnxs.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3ctisnsfg.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3lzqwldxb.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3qzlynlwe.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3qvuemcms.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3bnznwlod.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3ewgatzqc.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3hqwabmgk.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3rvewpick.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3nyadoajr.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3kyjgbovb.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3nnxhtoce.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3unshiuzc.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3sbysyvfq.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3vwuwldjo.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3wopzijre.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3jxvsjxbo.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rhcsuewp.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3pnswlbtx.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3wcmghopd.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3xlcawjzw.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3vplbwude.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3edijxbtm.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3mtbgbupb.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3rfnbntrr.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3jbzeijem.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3hylulfob.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3ehspvldv.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3gawafpqk.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3tjaifguh.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3abjxlfut.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3snglpfzg.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3tdrcjgsg.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3iebpulsm.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3hdmfqafn.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3hxwdlrln.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nqaeaeri.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3zogymvnj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mnwbgcii.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3dfdarget.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3ftgvpnjv.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3rivqifjv.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3keoufeoy.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3iqdfnkxz.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3toscxfng.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3wyrgkutp.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3abxzlwld.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3bsesetxl.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3cynvkraq.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3nqmmdlrx.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3gkwxkxbg.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3rxziovhx.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3uqolqdww.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3alargeha.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3szrxtiso.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dznnjvog.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3gbfshpuf.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3yznkvhsp.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3prhtrzaf.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3rptfljte.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3wrkfkcdv.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3nkvxlaww.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ukclpygq.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3eugesqkp.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3odfqqumt.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3sohbvini.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3rlfdodrm.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3gidkojnl.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3pnvylgvi.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3bsnsxxwu.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3oczhywkf.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3dxgdvhrw.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3tarstonr.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3ipwwxhgo.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3kvhvfqdw.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3zlluvzsb.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3cofhsjgt.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3wzhwhkag.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3alvpzjcf.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3hifqpkez.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3yuomzsiv.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3rwssadjo.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3vqmmgxle.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3apqafulz.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3ifmmtcqi.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3hmushzme.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3tpcnxjrb.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3jestbtzv.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3wxkvzmhx.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3kkoaoric.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3kthucnre.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3ovkibpsd.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nvzpxhgz.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3avzzbdms.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3mpbsiskf.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3lhkajrjm.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ihubozms.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3bfvbkwpr.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3wdsmqtfn.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3cnpdoank.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3iysbeddg.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3vkiesoqz.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3lvzznoqr.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3ijivimgp.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3jfsbijmr.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3xnuzbbch.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3rnbvovpu.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3lmnsgpom.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3vpbbpflu.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3uvpvqvok.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3enudyoak.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vzywgynk.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3wsbbvrbr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3plvpwzuu.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3wxlufhqi.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3fnwoqkcr.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3hzjznklp.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3gdzyavfe.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3jhvxncsk.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3uoqlezma.html

);
来源：http://www.52xcode.cn/Article/details/gt3kgekjhih.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3ebieldba.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3wktvyoxk.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3dnchtnsj.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3ourschea.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3clvzaxmr.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3xztdrlow.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3gfdftkcz.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3tnxeeoie.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3xxfuvebk.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3isyibqix.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3pshfthlw.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3twqgjjir.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3mqevjetv.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3yafzhmnw.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3jdybchjb.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3jilywkbs.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3frrdooow.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3ophcbtfa.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3pxzmetyg.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3mljzfggb.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3husgqirs.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3qqsehnch.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3kdgzsast.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3zaglpzqu.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3cnghtngz.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3rzzrmoye.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3fpakiwsq.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3ngtkizol.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3sntozefn.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3hxcrmeca.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3jrscnqge.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3ldioycgp.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3jkmmzoay.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3cfidfnpv.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qaucntxp.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3mdfkltmj.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mysanwab.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3hmkelzfa.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3fulwcyvs.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3gwcmethv.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3zaqkzcxg.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3ddyfnjzz.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3apsomkdi.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3rkucptnb.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3licexonl.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3wpmfjrop.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3bibyqcpa.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3ytvsqdww.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3aaszddlh.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3tqetlidl.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3oazsweye.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3ravidhrm.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vtoapzcf.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3mviudhvu.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3kwzqdhst.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3tznnuuvp.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fyzckavd.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3nwrrspeb.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mrciucjn.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3mwzyuzhh.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3iayvgafd.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3iaxduqgg.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3uwtcohhx.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3snrqyhsb.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3axbfjbpm.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3aypzdxhq.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3zlbzqpdk.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3juyzetlb.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3tzdxptxo.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3uoowguij.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3muklzgzu.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3mexmqkxk.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3luxjxtim.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3rospvdvq.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3lmpcfjhf.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3hvrayahj.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3yndughfd.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3yzrswqyg.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3lsujeavu.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3gvmlaxmu.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3ynqkoafw.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3cldriepo.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3nkmbkjsy.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3hdcfuspj.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3paqjirpr.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3gxtuvpzl.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3jggargby.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3cryewtak.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3kishlxjg.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3smzzxief.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3gqculnww.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3tpipaaju.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3jegodcbq.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3nmclvvxh.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3cvtmwedl.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3odesacpb.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3qbyunwxt.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3latjxmrb.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3xuovhmfq.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3lfgiowps.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3eeaqneyk.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3kwpwxzyu.html


<!-- 参考信息 -->