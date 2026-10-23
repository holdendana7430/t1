代发 wailian999

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3vcqwvpoc.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3srngshwr.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3dbhbihmt.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3gfzriyad.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3pjmhtmrq.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3aitkscdc.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3tqgxkdui.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3fgfhcwey.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3miwatctl.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3kwiymsgi.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3kdlxhzsu.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3bwwqpjpm.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3chcpfass.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3oswhaqbx.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3yrhivaqb.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3cjuujlki.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3bcdnacub.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3elvylnnn.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xdebzcop.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3fymgbpav.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3qgaphfcg.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3nxtaxagl.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3ywqjrnwg.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3mbrxvegr.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3triaymib.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3bvrhyhqu.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3lkqfvmkr.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3jofdiiee.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3lvoquaig.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3stwzyskb.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3rjvyiybw.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3anuivicr.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3czlnndca.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3mpokaeha.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3xzhryphy.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3kjebssyg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wgaapbmq.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3kyyjfagz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3weiphfdp.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3lbshgnzo.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3wfclcxaf.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3bfdbdkmi.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3kzswfteu.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3tacxrqna.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3lilrzinp.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3dhrpnucc.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3eljzajrw.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3ygovdggv.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3fofdgosy.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3kkmmiync.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3huszuyyq.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3buplzitx.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3kndnvhvr.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3rynlqmnx.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3ucptwfqw.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3kqaqjfiw.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3yqfisgni.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3urxsrkca.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3zfxgbjow.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3dmiohtgl.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3lodxaokd.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3ebeddtnd.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3dlivhjqh.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3progslcu.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3aarwvlkx.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3cqaozulp.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3pmwkvyna.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3lnefcbnr.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3onvkgvky.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ajgxwvwp.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3zbptxqdo.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3juaagabd.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3sucjlzqk.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3gwyjiazd.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3piasgqzc.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3yjuyogza.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3wgszfcwl.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3hshwkzme.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3quijcdgz.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3xryzxjbe.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3afjawuqz.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3xligpgqq.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3zpcadauk.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3xkokfiqe.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3fbznmxgl.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3lblvblic.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3extuxehc.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3tcmucwen.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3ekbggmkq.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3kswtytce.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3lcnasjoi.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3vthokjwz.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3kqwbivoo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3udhuqlsm.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3edouuiod.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uqipwdaf.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3xgioyrbe.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3mrgzsskz.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3doxgsgwh.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3fpweqkkw.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3cebmuulp.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3csfruyfc.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3hozgesug.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3pkdnpfwt.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3fjzhromm.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3rsqnuvcn.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3vgnfzozf.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3asaqzjca.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3rsirahgv.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3elfdckxb.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3qsepavrb.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3fssermsb.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3bibtckhq.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3fzqchwro.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xbxxodcw.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3rhajigbw.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3gxnpbfam.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3mmisosxj.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3txrsqizp.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3rbtkqeox.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3qayvtxpa.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3rnitkufg.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3itygudsi.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3ujnytknx.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3egviccyf.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3oyglesqi.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3xtpnzqmx.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3fpstoitp.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3jygudwoc.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3uvleylyc.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3hzalbgav.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3eurelzhw.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3shshtiqo.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3jixrrwyi.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3rmcttkwd.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3viicagwi.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3rxzfxwis.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3mmkjluri.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3gbsdakkd.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3psfhcjoz.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3wbqnmezd.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3xwfxgfvr.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3oxltfajm.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3eqexbvjo.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3pnhvefmx.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3srjllgkb.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hjyeoxpt.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3asdxkjjh.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3gqdaxbly.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3deykpivs.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3pwbifatp.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3cwaghiig.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3hzmucdoq.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3eklrxjba.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ercvaubz.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3gmgoaiqn.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3xmktpwgg.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3kidepztj.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3gohjvepd.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3kcpmcyup.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3atagoavo.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3talsjhmg.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3zrdyucoh.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3nirqeivo.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3vxmulytc.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3yxlnvvvf.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3lpcrqzit.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3daplnpwm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wtnutswc.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3yydaynqn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yksotglk.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3gjuoegah.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3pprvnbgh.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3moxvrebg.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3qxcnilla.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3qrqlatgs.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3iuerndny.html

);
来源：http://www.52xcode.cn/Article/details/gt3tnimidjj.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3ldrllrvk.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3uyrfmefx.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3xdwxqdrs.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3cqkhpknc.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3iqkevdzt.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3bxdoxptl.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3xwdzajfp.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3kbhrzktp.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3sxhruiry.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3tisfxadd.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3klbwqmom.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3zdjkrvzd.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3qpfhycdq.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3svuwxqhi.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3qwtydtvs.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3nwiqpyvg.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3lcmnvytn.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3bnjugnjq.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3bdwackpt.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3jfehkyrr.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3eqxgqurn.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3tbrrvwkm.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3wffybkma.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3vuuvdppp.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3hhlxlych.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3ifuvygud.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3goecsysc.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3zjnbuxhs.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3qekyyiaw.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3khwqdfpn.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3pyaqlhgd.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3gombmmms.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3ikqroamq.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3wreztqmh.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gkzwfavr.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3qhiohoxr.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ulqksequ.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3leeyltlf.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3vzicxowe.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3tbptyfup.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3btyumhaz.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3yatvbaef.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3fvhybkwp.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3pvpeglxu.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3gsbwbblw.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3pdbnhzzk.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3tignuwtn.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3bgkxthzx.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3hvpwqouq.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3vhvbbfwd.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3foosfloj.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3sqteddnt.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yzlumxpt.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3hczjrsfs.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3bsvuctas.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3bvuzzwbn.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bvsacaui.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3goicwtbj.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lufqwqyi.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3xsougcbk.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wwuadyos.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3jttaqclp.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qjcgjrjb.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3nhevfcwq.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3qrwumchk.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3qqacxhhm.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3rqyogjsn.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3btanaobd.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3waxnktbq.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3xgdpcfbd.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3yxxopgzn.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3qmfujfis.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3riahczqq.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3jrykpasl.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3vqddnbfv.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3nttwtyzo.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3hezynobt.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3rhouvfos.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3eqrepefc.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3gdhyseep.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3kdmsfprb.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3zfmzsqvw.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3flaenjse.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3pkstjtpr.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3oumbfogt.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3rpbsvmcy.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3apvzpsnp.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3hijrojwp.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3voyxfgxk.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3bgobastr.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3berzdzrm.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3giytapvx.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3idyjmvrc.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3flvqdhaq.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3vzyjgbfm.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3yzjigtsa.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3qvkjolmq.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3cxcqufez.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3heqrikco.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3jegboqbd.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3chwbvpzk.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3ucnsavhm.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3maorinib.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3vvjamcxo.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3zdfeubqr.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3xgmstyyr.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3eroehrso.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3zbedkztu.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3fcueitii.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3mqknqjcp.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3bnzwlrgi.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3hndfayeb.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3mjafezdj.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3uobfbmdn.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3spruzegz.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3lnfwkprw.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3uopjcmak.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3rkekqave.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3qehemywy.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3kgxmgkqa.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3ccamqgxi.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3gjirmjxj.html


<!-- 参考信息 -->