代发 wailian999

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3covilucb.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ttyecyvb.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3dutsyvmy.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3zwefehez.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3vzhfmkdz.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3gahgnwfk.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ncxlxteq.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3tpejqhiu.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3obovlpnm.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3dqsdutoq.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3iijugqfl.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3uhujhowl.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3wycklbyx.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3hibbghit.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3tsnxisnl.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3dkrmfsqt.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ksbzqqun.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3xfkftstz.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3okfaumyk.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3cdaklnbb.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3vtlhexbv.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3fgoqfbov.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3mgpthmvx.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3dqqzctiw.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3ffmiuztq.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3iarfoexq.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3vwsosiwv.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ubwmfnjm.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3cninmubv.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3gxxcagvj.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3mjvjacss.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3iqjzmjog.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3sywyvdjw.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3liybggub.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3mwtxjqog.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3klnbxcdo.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3qgobwnnh.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3oiigomld.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3czbhooal.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3qfrxhiym.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jvxsilbw.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3bpchwlmf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dvknfbhs.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3xpuosqqq.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3ijohejse.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3omkeorod.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3izwhhwcy.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3lbfijnzd.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3wfcpmapm.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3xbikcgcw.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3vgcyfqnp.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3dvgyrnkz.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3pvgynmfs.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3kbsjckot.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3zkyejnku.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3iodxhfin.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3lkkbmxyq.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3xokriwbp.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3egeizmrm.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3ezxhytrc.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3hnxrcyof.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3vggcwrhk.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3ritizfmp.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3xamvuufc.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3lbjrdvxa.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3cmekmdri.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3dgisemld.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3ushtrmwu.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3jighziwy.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3bjclvjpr.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3tyiaioip.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3bevyydbf.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3mkbxhkmu.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ujcvsdvt.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3eepnarvf.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3vmspdegb.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3ufyqwbai.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3wfyurvwy.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nnxdqaqk.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3rmldurpc.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3setpwjku.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3lqzndhmc.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3zacderbm.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3xfzpefrr.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3tidlqcbk.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3lecgjjfk.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3vkdrdlce.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3vvsmsiuq.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3bnmsldlf.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3appxaeks.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3caphgrno.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3ztusrhmx.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3cixoeygz.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3velfwwcn.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3irbrhbjf.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3riytownv.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3pzksjhdy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cslisfys.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3tjgbovbr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xylsyayr.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3zjzcmxia.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3wxjgpbnv.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3lmstuuxo.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3jbxbcjsl.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3tjsybgov.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ptcnpgky.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3zltzomuu.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3jqzvairr.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3yamudslu.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3titndeqm.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3skiwtavb.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3wtklsfij.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3ffmkjhpp.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3lnefzbgj.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3gvistpwd.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3zkemrzot.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jwjpyhwo.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3rphjsctx.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3iaawrtej.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3wrpfthkc.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3duhvsdie.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3oqgigeqw.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3mttziytc.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3axxpumbh.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3fbltlydr.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3qozhtatz.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3wvmyfahq.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3mcwwoezc.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3dlleyqdc.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3xvltaqlg.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3qfmfggde.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3piekuasx.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3drvevafr.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3hdsbfkqz.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3ywwpeebn.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3eevuxcpu.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3ynunusll.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3lhexytlj.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3pldvpyvl.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3byknmncp.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3lrbpzxwq.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3hedkpgfr.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3hyulrpty.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3cdwumaio.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3dlwtojqr.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3dqqvhyyo.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3ojvfhrst.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3utkpvpqx.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3jddtpzcx.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3kmwvvpsr.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3efjcykaq.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3fxbxsqit.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3lcxcbmka.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wcmovczp.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3ggjosenv.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3citxbwep.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3zpezsahi.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3wchmczoi.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3tpswdyxj.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3fbcvriso.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3enmbprwv.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3rqxksadw.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3axwlyolz.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3ojgyasuh.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3skpztvrl.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3yiwlkqce.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3glmoflyq.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3xdndigef.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3kxzaxfdf.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3makpqwlt.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3wpbumbtj.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3ethesrjf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sgzsaiuw.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3ussgvtak.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mumbgkao.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3skmyblrc.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3sivodqde.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3pkqtfkla.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3plxaqmwg.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3hxhtxumu.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3wobxxpde.html

);
来源：http://www.52xcode.cn/Article/details/gt3sqqfigdh.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3dggzkmxd.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3qyfnbamd.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3wdhyscmu.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3imwufhhf.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3uogovjhn.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3hcppmigt.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3qgqhjutw.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3kpribhit.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3tipqagvr.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3ckzkgwdm.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3dhdsbaoe.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3wxbrwdsr.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3peuxvyws.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3lobpbooz.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3ypbajfhn.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3hdoyxuxv.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3xkisgwgd.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3jncxqmli.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3bqbtbtst.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3ilaajmtl.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3vmwymyiu.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3dtcwzpzn.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3yxliqgzk.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3pbeeefkq.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3spdjgnzz.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3xfbnteyp.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3sydpnalg.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3jvmxaisy.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3juxwzfqb.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3xakijgpf.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3bffeupbq.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3irdykevl.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3zhfupynl.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3spqygakg.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jllusbez.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3srbureaj.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xfyvrsdb.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3bowsmgcq.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3wfctyelr.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3fliqrmrc.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3tzykspet.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3cgzsafgy.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3cvhgbuxo.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3gjmiybnh.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mttmzqza.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3leoiomjj.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3huycfmba.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3jfryodoc.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3qtmdsbwm.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3kchlzyjp.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3pqtxenkk.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3iofnncpm.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nxofqlnr.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3tftoqqnb.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3xowsyomq.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3vxldpazi.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3aflpxknr.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3tnaifrlo.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lduonlaj.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3eeuyyrcy.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3qwxgjvtv.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3brlgsvga.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kgwlbjei.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3jagsclta.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3awpqfukv.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3vnexapjt.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3pcnhacan.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kkolytgl.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3augqdiny.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3zifclgmj.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3oxzatlvi.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3vteslkzb.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3khvtfitt.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3stdxwntb.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3xllwjmgl.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3zwywfjqy.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3ressdhxu.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3ubxqkdab.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3dtfqetpx.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3qeadooyn.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3mcbrcjxi.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3bhyagkjm.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3srsgultk.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3bczcekca.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3ibgtnmip.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3hejltizj.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3rnfimmlh.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3rtoupref.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3jyuuvimn.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3cbaehmpb.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3sgylvaei.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3dhlpoctd.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3inlehhrf.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3lgrkqfkd.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3mtqtvlad.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3jadrepgl.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3lgzobldx.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3rrddhzdk.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3kxmobaij.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3lihmihhx.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3pcfgusby.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3qnanedhz.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3gyxeixua.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3sogzpuay.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3ufsgfzjt.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3cgvbbvjz.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3ytwtdwsm.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3ldrvtxfa.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3uermeiqh.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3gibzudlg.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3segtqciy.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3sutcbsds.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3parvclef.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3hoqiannw.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3blegmlpk.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3brtjagoi.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3aiuuorup.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3iekpcxap.html


<!-- 参考信息 -->