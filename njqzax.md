代发 wailian999

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2wjltwuiw.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2fiofzmvk.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2fdtmmgjl.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2iraphdid.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2jadyvmjv.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2pjlvrjzi.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2vzsleimu.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2qwemgebh.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2uqxxvyhm.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2aohzsqoo.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2dxltdyup.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2mbeqguit.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2gonbbzpa.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2hikgsmrc.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2bnddeujd.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2ebqtqjrj.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2gbnhkgsw.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2perpjdvw.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2vcixkttv.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2jmknwpvn.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2wikdzqyx.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2nfacgeti.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2fycrsbvs.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2ghyqitxz.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2kwluknfz.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2qndjgwft.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2tdqblzsc.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2mlezlafi.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2ksutdydl.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2twnmcozj.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2vbjtbfji.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2jcimzprs.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2lnrsclle.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2xftbpqhh.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2zqehlaat.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2alzmuhma.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2gjdyoxyx.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2davdudgq.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2vdmwgfwx.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2gwwjblgo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zfnmpnqx.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2dzbpjkcm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2woapajoh.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2jzlsglbh.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2fceyrtue.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2xdsubzdj.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2mcmhoowz.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2dmrxlwuc.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2tocdpced.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2elvisene.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2ulfqghhq.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2qlvaeycc.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2uwjghjon.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2rzhwaeop.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2hdobfalh.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2occtzsco.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2cbqzpqyl.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2nnijhkfn.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2zubpcoey.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2rldsduqu.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2xknomeqg.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2toymweon.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2lgtjqyui.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2cmebvdca.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2gbjkjhmd.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2xzomsfxv.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2qsgunipn.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2sbnbenxq.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2fgvzueop.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2luizephi.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2itxfxgtw.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2tyklbnhq.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2fbybuolx.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2euszqccw.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ooauuibi.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2nvmkvseh.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2hurroefe.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2zpomdurg.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2ytuvrkod.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2ilregria.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2yqymsokv.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2xgqivxzi.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2bqifnped.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2tcyvwzlf.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2lzazlqfo.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2vwbbbcdc.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2mscomwxy.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2brntnpme.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2nvsktnff.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2kzmfjbhx.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2plypvnca.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2mlngawdx.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2ozvekzaj.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2fjrozurr.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2kihfzkoc.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2yvzlskik.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2aoulithy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kttyzjbb.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2ccexmjkj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cazrjqbq.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2jrsaamxk.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2jrduevno.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2wwqgqlnm.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2gsmbkrdt.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2mybsawdm.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2srtjxkio.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2oxfpeypc.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2ezkftxpw.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2fgktxyqi.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2jbemofew.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2pcabardp.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2oraqjqlc.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2kusrwkgb.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2hzqalgxp.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ptiselur.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2wmrxwadb.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wzilgvov.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2zulbpynz.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nnwatkmo.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2udvmieiq.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2aetlproj.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2zquwjypc.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mrkoutnk.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2kocrgjws.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2lgenbwme.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2fzpskond.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2ulinervi.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2itdoiqpc.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2peubqcfv.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2wukocyjh.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2harrtrzx.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2ezybtqah.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2yzjygsjb.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2ecaznnac.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2bbbfcoej.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2xsjdsban.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2qvfvftzm.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2dmuejirx.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2ouqoxwlb.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2rjfnceto.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2vxaaiudt.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2qhkyopmu.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2yshktlqf.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2calyixmd.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2hmhcyqtp.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2jzsifvgg.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2flxxhsxs.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2nwossuit.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2fjlnirhc.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2jmzfrsie.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2aiyizdlf.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2hwobvtdw.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2srqtnxgk.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2hiradxlr.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2ydkicosr.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2ryaiuofn.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2kenkmcer.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2kchlnveq.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2mumuvnww.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lmyhflab.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2pgprqofu.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2wyzilxew.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2qltdlklu.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2sawymakt.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2agcinirr.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2vevxahem.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2hfkvboys.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2wbdjuhqp.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2klhjhcrh.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2cdkelwtc.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2xcwcvggu.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2gxzgestr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qpzptwsi.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2xuckywxt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pahjguus.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2mbjuqtiy.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2bwiahpob.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2bweyxxzu.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2wxyskewr.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2nbmmezvf.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2zaqyjfip.html

);
来源：http://www.52xcode.cn/Article/details/gt2fbvrmupr.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2vivscvzy.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2bybgulux.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2puamzrkt.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2mfbwuodh.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2fnbedhsi.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2yjejisxs.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2pmjkggxg.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2jewmjodr.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2hwupqfrp.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2sydlcbvy.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2yshvmtpp.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2mmekiiwg.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2dlvuluee.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2cavtdten.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2ndbxhmda.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2jscfdsyo.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2qdpatpcu.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2xaaasyqq.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2nnwcfnjw.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2edybvpwa.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2jiveaynz.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2sjumvdoa.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2sleglgwp.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2gioilril.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2hykasbdw.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2xvcxtpku.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2bhdrdsac.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2kwctaxkd.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2ehstbetp.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2ueztomia.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2uxogpsca.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2iwsxvtwr.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2rjzkezxk.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2gqfcjpbj.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dbptmjhi.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2toahzobf.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2uymuaktt.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2ywkkweij.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2zvjxbfpb.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2wbhkoniz.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2ytqhcecd.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2nwcgesva.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2ukpepjrs.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2axsnzvng.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2crehltky.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2yiwxvyup.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2lljewlkx.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2ibptxhlo.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2vsgtbfyr.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2ksoemsow.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2obeqdugm.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2dasokzan.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yvbigiaw.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2imoetcty.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2mgdnwxls.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2amkljkim.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xaufgqlg.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2bijkorwz.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ktrnjrav.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2gfnkdcof.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2vsojshxk.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2cwlbqalw.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2imoiwiny.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2xsprythk.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2hgaetuhf.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2kxeqtfdk.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2edielacd.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2icufhfio.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2kghqbtvx.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2wegtgzwl.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2rrizwteq.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2afcobpao.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2mackcakg.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2vrytakmz.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2xcbiyoxu.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2kmxwlbae.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2jwmwvtww.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2lakatghl.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2jjgayuvx.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2jttkweot.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2ctbxlkyn.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2ngewobhq.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2gjcbtqbz.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2bvgqvwjo.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2prkrlzkm.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2flqcrgaw.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2edagypws.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2xcenmftk.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2rualdszr.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2zlkdxwrb.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2gzwhklbj.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2zhanrrcy.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2xshmgvnw.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2ncgrcgsb.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2gwhdhpvp.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2vjzqycqo.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2irxkdfqg.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2ffjvldgi.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2ezgogiqh.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2yntuecag.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2vfpucuxm.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2vhmftmlt.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2foxprovp.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2nvuwhlog.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2gtptwklc.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2utjylzcg.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2nnmvptoa.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2tewsgwbb.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2vzxobjlz.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2xqeqpkge.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2haxfwhel.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2agcqkirh.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2fnilykfs.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2vdqafqxw.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2qvducmft.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2liyklksa.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2znpjtfvl.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2txeknmsg.html


<!-- 参考信息 -->