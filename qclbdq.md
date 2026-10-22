代发 wailian999

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2jswuvvwq.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2wejrqmes.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2hysmyewz.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2rbqxupqe.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2qepgqegt.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2glvopqdk.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2yztotnek.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ebvdezmt.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2zqrqyrnt.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2rfxpanth.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2fjuuugjd.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2frdwjasz.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2bhvymsle.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2xxoytbqg.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2gecfanep.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2rtzywgar.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2gtinopfy.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2dhorkznv.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2filfiwgo.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2zgggqfet.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2gzvqzfph.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2cynprtzg.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2ppnwmkkr.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2kwecuwsi.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2bqgoxryf.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2jwrkghzr.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2ndududrb.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2tabmyhjc.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2ztogtfbk.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2eeoomzwl.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2tcuqsoux.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2spmjzfzc.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2kafzlsvd.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2ddkzunoo.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2tnonwfqp.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2gzthlhgh.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2dsqohgap.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2samubczh.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2pgzwembq.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2iapywgvo.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2vxzqsxye.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2mvwtvpfd.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2qmunooht.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2oyxybibf.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2pfceizim.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2jycnqnxu.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2dllpjtzg.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2zzcftphy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rsuddjky.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2kveqmuwf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2apkxstom.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2uewpywfk.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2mlnyjweq.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2jjbjrmxo.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2jtsjtlol.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2guumryrz.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2thcdctul.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2ztxmhjbf.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2opyooheh.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2jlhzaanl.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2prtauiiz.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2siqllyzw.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2rxingskh.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2mcluklqh.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2wjcxchfk.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2khxzhedc.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2bkyzzloo.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2zrcdhdsb.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2zolsigwe.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2apeisbjj.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2erdwviwy.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2brjblfib.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2mjdzeeya.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2ikervjcp.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2ialjdeee.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2xuskzpxn.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2ubbmfrcz.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2rqwlqfdz.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2kdohiifh.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2rnyqkqaf.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2muqakkfc.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2qbhtubox.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2fxmkizjr.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2rkcqcrkm.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2zajmffuz.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2ltgxkhdw.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ocbqahkp.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2afthwagy.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2jimchhhy.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2owxezied.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2zghucfwc.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2mrcprzcq.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2rjjfocpp.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2tngtfbci.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2kqkeiwnw.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2joxgfscj.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2odtelcnm.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2ewqusrsx.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2kleiqsww.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2iubbvqjr.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2czsdvjss.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2lieabxjv.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2yuayfnnn.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2ncsdbxsx.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2yzmtcctd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xpflwgot.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2vmscmasn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2expqyrnq.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2ztopcyda.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2yjtqrdrk.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2sduqalmr.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2zvyzfiqn.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2jmknhkfa.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2htmdebrf.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2gneqnftb.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2xtmugqgv.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2ubttjcib.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2phhqetmu.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2nzeretkm.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2abwvbnlm.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2uwohbgtp.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2rqtnltys.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2xocfskyt.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2kptmkodm.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2ijegvddz.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2qkyruygq.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nmzhgkrj.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2sdmdnhhz.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2trrhadfj.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jfdtpdrn.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2oceankuy.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2yyqzmsnx.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2inhsbkvl.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2zdkuupaf.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2fruwmeth.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2iwbinoea.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2fhipdxpy.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2urkcrvmq.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2rzhepkku.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2raifzvtq.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2qiwchaxc.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2fihvsutn.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2jppemega.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2vsxvusxj.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2twctjzpt.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2uviuigmy.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2qvsqxgeo.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2kdgrqqvd.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2zllinzdq.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2ikklzdyn.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2txeshoou.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2azjuoqxf.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2hxyqjulc.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2kppegxnr.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2exgqnfgh.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2enndckuq.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2azinajnf.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2hqmieoef.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2iinpmryl.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2otxnmztk.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2pufsqnpz.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wwfrhmfu.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2xtpgzjry.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2webyvmls.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2wlflmcxq.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2upvvuiff.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2wnpulsnp.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ukfzgqzs.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2illyjlfy.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2lepdreay.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2zqdlvprb.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2qoovhfbh.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2iewejghm.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2jepcfkdg.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2kuhqnufl.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2kqndtcbx.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2wmpgxstk.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2gogvfrjz.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2gzxpetmf.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2nbrilohr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gpbhixoi.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2kgqzlofu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eksklycj.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2hprjrlco.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2cxrzjtjb.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2fgjpakcn.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2oyshqzcc.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2zeruxxnp.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2jnxvyjkp.html

);
来源：http://www.52xcode.cn/Article/details/gt2tfqsntkv.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2nqowmfod.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2qdnqupdq.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2vgquvycz.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2obxbatdd.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2mnqjxuor.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2tdlflrin.html

);
来源：http://www.52xcode.cn/Article/details/gt2ekodxeqz.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2ustdbnow.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2neihotwx.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2mgpbqrel.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2idezjjze.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2bzqadhdq.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2fkvxrfkc.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2jqylbvdv.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2jzlamhdh.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2pdklgagi.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2haeplsgd.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2gpeccnop.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2zqpyxjup.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2fmemcwke.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2dovqijgh.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2fonzvmxt.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2xfssbbsa.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2wsfmchyv.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2setfwscc.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2govtdwrq.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2rozfdzeq.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2domlgufs.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2kugoaarg.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2efxqbngg.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2ackmwban.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2xdbearfd.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2thpijqon.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2zdgojvku.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ripvizeu.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2kyhvlncc.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vpxtakqo.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2tcdxihff.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2kyghymcf.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2pkbkfdmp.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2ipusmqyb.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2btugonev.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2zngpubjr.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2bdldzgbs.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2dnetltnf.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2ikfuhhrj.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2thiovcoj.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2fdgsjvbu.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2waqleetg.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2kyrozdwy.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2dhkrqwzx.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2jfctbopy.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gunmmxoh.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2bkqxwvpv.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2fqwcwrok.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2qtazfjch.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rimacjvf.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2thmmgzwc.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2elwghxjx.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2lekxchll.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2uiherxmh.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2eagbajsn.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lbyquvdp.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2dkpoynun.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2lhgrtpsk.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2objnkxpp.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2nugyelqh.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2oqznvkfq.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2jgwlrknu.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2rwwyzada.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2uvkozfxf.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2kbtmkwur.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2iwqddgji.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2gyjubrvi.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2ekudjhhc.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2xbtmqedp.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2uagkpzar.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2goglzuid.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2zssxfcrt.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2rkvzoxng.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2hnhbsbzo.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2ydxyiiko.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2vmqqapvm.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2ttfzaqqs.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2dzetwdsp.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2tjxvafjx.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2wsvetwkq.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2krhmncno.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2axqucvoa.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2lwzbdgdb.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2onwfiyyu.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2dhagfmcq.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2vtdlybfr.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2dumuwzwu.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2keufehep.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2qcoybbig.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2zpnoebkc.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2kluhgwpp.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2oloitaaz.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2xcybenhs.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2ayhblovq.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2mekmkdwj.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2agnoyfsq.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2abgtupvo.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2urhgijgm.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2japfaxaa.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2glegqaua.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2pqdudbka.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2lgsjjtqa.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2fpbhegex.html


<!-- 参考信息 -->