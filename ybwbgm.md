代发 wailian999

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3nctudsqd.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3xvydjkty.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3kwerzbqs.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3gmvwphvg.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xjfzotgb.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3xqvdcbgx.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3oaxvrdnl.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3smqkeeyu.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3wgqpwjnq.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ygcvbfgt.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3abykvgyv.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3aqrezpwb.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3mfasoygg.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3fdtrdolg.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3jblhahma.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3guelcfgu.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3koeqexsv.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3aachwsxg.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3vgiajwgr.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3idqrcumh.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3eqqkilkz.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3lipewnoi.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3mtdrasep.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3wbxhnoqk.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3nctfkasu.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3ittaxucv.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3evwiwhpp.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3tcpsppwe.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3swkabhso.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3yzhqkhok.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3lmaonxop.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3yprbyhba.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3nxzdxsoh.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3xfdkhqyl.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3urbqxakg.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3drphiyrm.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3niepltyg.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3ezsndtbv.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ywnixfwc.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3zlauvtql.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3inyufupu.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3ywwpjtov.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3psdpibgo.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3jbdjeyfn.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3qlytzyhg.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3iffsanam.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3jbxgtqav.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3dpqxfmzo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3enogjgcg.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3ztnjthpm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ugaxzzsz.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3hxqkslxj.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3xvloxrky.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3abigjscw.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3gxjcpetf.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3illquvpk.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3cenbnnbx.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3shpsipfz.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3affkeggc.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3oviijinm.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3zceddnop.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3bppgegop.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3aiedhtdj.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3mhmwzhms.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3puntbkld.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3iojveofo.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3xnvooyjv.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3yhsddint.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3ttljqylv.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3teawqrjm.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3mluziurc.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3xdxetffm.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3fbrkiqlh.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3jwwvqbtf.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3tgcipiyv.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3fyejxjdj.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3vvdhxcjv.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3gapnrrad.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3cypiqbon.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3fmvtnczp.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3bdfctzul.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3coiwuhol.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jkraxpej.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3frfhdtrb.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3hsgazojc.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3amwyxoxz.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3gteaajrz.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3wjjzrkpb.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3ewsszyzx.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3lpykcxyw.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3vcekkpro.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3yotyjzin.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3rujogkmi.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3qijfgkyu.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3wwjvdoon.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3rbqpkiby.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3siyjzdjs.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3xscxjgqz.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3jeaimxcy.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3roqghejz.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3aewgvdog.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3rwopwckm.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3vrksyeez.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3ypscjepb.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3wkotbqqf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xnbbuvji.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3iisrapti.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yhdlirpu.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3heefpotg.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3lttdyztu.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3zcsgsjso.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3prdpsqbi.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3eminrwzq.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3etnbczfi.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3dcsfhhdt.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3lutvgcoz.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3gthuvrux.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3yzifxidj.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3crytoyuh.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3hbyzevxg.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3tlsnmcza.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3vvxtgdgz.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3pxywdudd.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3zqrrbffn.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3ptlfteuj.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3yvkxmlhl.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3eyfmgehi.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3juzvayiq.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3jhxhhavw.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3peinqtun.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3twvfmvtu.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3zcdbuvga.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3vyeaodnv.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3mtujxljc.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3omqipxyj.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3cvnxlfwc.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3fdsphybe.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ybwrqook.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3aqmjdklf.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3zpsvyien.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3mokcaimv.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3mleikbsj.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3mranarhe.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3wdwltqrr.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3hbfuydag.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3bwocuwst.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3kutqclkx.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3wdxgbpxq.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ttuoaeuk.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3ttvuwwzs.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3zxkppnrz.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3pceedarh.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3qcgbqqgu.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3eertzdxc.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3jdeyfkfi.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hcatomzp.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3kcqsjiin.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xsardupd.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bbkbvbyw.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3cohmhgxc.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3pljcnoui.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tmdnvvpp.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3uxzncnkg.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3lxedlmqt.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3nltqoprf.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3pljbwfzs.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3jerijkgd.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3bwejhgom.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3jamsvujr.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3kwuheibs.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3zptqipvl.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3ekohvgkx.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3bqputtdr.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3bguftjii.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3eesspuzi.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3kexiaxgo.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3jgcofryx.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3vzrkvpws.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3ktusswee.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3wvykqvhb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pwqxmgaw.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3olilvcfo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jxitjucy.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3mhqxwohf.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3hvbyizxp.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3outaenic.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3lgkpcxoq.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3gwrnhmsd.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3nsapsjbj.html

);
来源：http://www.52xcode.cn/Article/details/gt3nskkbpux.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3nibexrsv.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3cuoksssk.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3cjiegxww.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3uqwnagkv.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3arnzfynd.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3mfjsajik.html

);
来源：http://www.52xcode.cn/Article/details/gt3oqzxxlav.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3tqesbmyw.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3salcbvtx.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3ssdjhwkt.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3ekkslfaz.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3hupdnhlg.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3hseywgth.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3wwvlrxmm.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3fmpadzbs.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3kmndbjdq.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3rvwlxunx.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3tjbmqwyz.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3umcgtuyo.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3otrghlct.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3pzcegrkz.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3shsoxwrm.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3kkqhdwtl.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3btodansy.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3oqshduax.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3zfueyahj.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3mwoagqxe.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3iapapvng.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3dudhvrlo.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3yvhiuahw.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3eynssnsf.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3euxujkqj.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3pbepbalt.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3ogvamhev.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cocozhss.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3pggnclmy.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jmsunsri.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3yznramdu.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3xnynmsuo.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3mnqgfnsy.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3qmixmsjc.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3sdvdjabm.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3cfsejvia.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3bgjgdjjq.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3odfxavnt.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3bxtzohph.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3llltzdtu.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3plnzptsl.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3igtfevzk.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3ltadkhca.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3quqdfgiw.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3biwfbcsk.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zlvhcvju.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3qcmbryle.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3rgldblhi.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3hzvaeeng.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gnijxvhp.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3nvcqrlrr.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3itzkmkkh.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3pfmjarhc.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3zkbwcprq.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3xtzsiekq.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yehfjmat.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3dorrodsa.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3qpjjjgqg.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3yvcdnrmo.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3drtxnnnb.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3byqbccus.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3uuydwbjy.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3odyxwhlw.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3cqfczmxn.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3mhmedrxc.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3vffxxovk.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3owerlmdi.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3fhuwrpmu.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3cwzhdpxx.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3pvrrtvay.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3hrmdygoa.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3xqijkukj.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3tsbixdqy.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3tnbrkcnd.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3lazjvwrl.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3cpjcbkco.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3txuzbzyh.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3qglsysam.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3jfrldmti.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3bhgonwdj.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3pdbyuawz.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3mtxagrlf.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3xxrxkunt.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3gsrthtzr.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3dvubtuke.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3czcutyql.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3xjubnrei.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3sxrtlsay.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3yfobtznl.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3epejumci.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3pewzsadl.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3tbvifbjj.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3zwfmbyxt.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3mdfgktxk.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3shzulwmd.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3spcwucdl.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3bygqjwnu.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3zwinolui.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3vzscvoig.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3mtqzpsnh.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3pfhdmjht.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3cwwfkzet.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3fatjndcp.html


<!-- 参考信息 -->