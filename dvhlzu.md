代发 wailian999

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fofvrkqq.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2mephkhbo.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2bwhwluot.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2eciaeatw.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ixuhtjty.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2bkzwkbjq.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2uuqltuei.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2egyzqoly.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2ibcrhoyu.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2guyjyqqv.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2hcpaufyi.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2hrgrqwcf.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2uvvboxxn.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2xltncwhk.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2tqkartzb.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2jprjnuro.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2fvnmcdau.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2apiehtmb.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2zrmkqlbk.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2hryqihsh.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2kverchiq.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2wkbfcbno.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2antixpln.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2qhmatzia.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2agsedhja.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2fgcksjcd.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vrlxgtmi.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2jwnchluw.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2ynxuhcnf.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2ywoeolmm.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2bbfgcjqz.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2gevjglkx.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2altzicev.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2hpjigqxi.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2zaeangna.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2iqcvmein.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2fxxfjcba.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2tujzjwbc.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2sbcezght.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2nbnnqtqp.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2jmftouls.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2xbnamzze.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2vozjfbkf.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2xzfbkqlo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ukivjnoc.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2jwcmnhrt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dzwebmfj.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2yakegmfw.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2jdxeqjgo.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2jggywedc.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2kyjtyzpt.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2xsabofse.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2booxizzk.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2grhacndd.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2zyhnjqym.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2jeyuvwhb.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2fngzncxs.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2cphphpuu.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2cvfhgppc.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2zxpwjcrr.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2cpnevsfd.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2yrnjijkt.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2mnakbada.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2pwdyjhol.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2csxwgpce.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2thgvevak.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2jxhyqsaa.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2gotbluev.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2vwyvdpob.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2ekvchwaz.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2pvkrsnes.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2nqqrmnyp.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2jzjkcghu.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ggqtprtg.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2dnxdgcdu.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2bijswhgn.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2dzqijvfw.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2akuoxmvt.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bdlmfnkj.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2qsktzwqd.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2ljzchisd.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2cczmcohz.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2otaoorok.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2zehlllzh.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2yqgnkjpi.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2pdjpktcv.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2efaekwxq.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2iapzgkzw.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2ybvujfke.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2lvjevnun.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2lgbvcvpz.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2bpcjjgji.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2etuqpowv.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2noiffbyy.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2viaqbhao.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2nognnism.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2ytjdnmin.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2qhkvbtsp.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2kdqeleig.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2zlrbzovx.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2nsvetwou.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bubzgjtm.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2opfkwtyz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yhjxkzft.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2rqsdvwwu.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2ehhuvslb.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ynpzdrzl.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2wlwjubex.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2iszrbwtm.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2kxlwxtlq.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2lkbmtfxc.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2pkqgfdty.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2ynkvvmal.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2ddxizefb.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2wstuqkvy.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2dofqqmhm.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2hlajfdjh.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2opuljueb.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ebieyzel.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2abohlljm.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2arfclfhu.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2cmpjzwtf.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gesqbrmf.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2ijofkmng.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2dzmwnhwg.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2afrncwql.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2vgncnaay.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2etbzkxbf.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2nmdbblkk.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2kgnwvfef.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2tqssodkj.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2xzzkkugm.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2apuepisp.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2eejiqyqb.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2oqqxuvkd.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2gnnwtaym.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2hkulwkop.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2ozmiltaa.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2yelseqxj.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2pfxemprk.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2ipzgvhpl.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2picowqwn.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2bxmpqafj.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2ttusnfyw.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ifcjtkix.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2bdlduumt.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2jkbimwzp.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2ufsqizvt.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2rentkxoc.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2mxoqmikc.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2puywxppm.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2cdjvzdlu.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2tkeczfhq.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2evgrugjk.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2phiyaypz.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2vsiatfcf.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2kohtlgsr.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2rbinuctq.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2pxxvqhiv.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2bmnmetyw.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2zcshtqhc.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2lerkceiq.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2cfwmaqud.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2oyaxokgh.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2zqyvhzgc.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2wvuftxtx.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2ackkqltd.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2fckfhkxf.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2hiolqjat.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2ehrzfnks.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2zyobfpsa.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2ojkzdivq.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2yczotihs.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2tidwrgmw.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2tdbadijk.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2qbsbeyue.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bvfvwetp.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2kuufmyrc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mvzjccgk.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2afzycxea.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2xofflrhh.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2crbcwqbn.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2egftuirk.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2jrbtvjpx.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2alrbrwmp.html

);
来源：http://www.52xcode.cn/Article/details/gt2zpnmhsve.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2rrmpdsfv.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2zxalljsm.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2mfrmlhtj.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2fwstjaoz.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2nqnsmsfc.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2xqpouwlc.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2fuwfadfj.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2kukpmpxu.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2iedskyct.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2ubdsuose.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2hjllzyuh.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2npwwkmlr.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2lisjoczi.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2jovwpxyw.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2qcdpwgfq.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2glgbgxjz.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zvfrcgzw.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2acyijvtp.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2xrajrkhu.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2vlbfahds.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2jokpcwdp.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2djcpvxkt.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2slsfkrnz.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2jfvcmtns.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2cthkvlax.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2hmxhftsv.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2vqrbaawq.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2pxatuzba.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2ecuxrksi.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2oqcyoipy.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2npwbourk.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2cepizjyb.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2odwyekqp.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2pthtjgys.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kcmovphd.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2stixdvhb.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pteayyxt.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2eyeaaclm.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2srugtcsv.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2lpdqglie.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2xvvuiows.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2bpehymkc.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2yinggsfs.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2kdjqfsee.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2kuxbwquf.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2dzopflpk.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2anpbopwc.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2ewkavwzf.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2mbkjlojp.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2uppmfutu.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2tlkzkweg.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2vkzpwvee.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gsksduaj.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2wauehaux.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2hsouenzm.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2rxoiedko.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cntnrpmj.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2rgogyvon.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jvtxwuzt.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2caskjrde.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2meoldpxy.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2nmvibzwo.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2oywrlbos.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2gptpzdvr.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2lnvxnxpo.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2tnhyeocc.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2fkscrsai.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2mhkcjqhe.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2ujytzqzh.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2dkkrejkf.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2jxwgeivv.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2klgwvhby.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2jyfadrpl.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2vigwlxdl.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2lwfaakph.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2mbtxzarm.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2zybgfbxy.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2tqdtdald.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2gwbkfjir.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2kmerthjv.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2qgcbvsim.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2biqrrwbv.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2drsauyil.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2ldvhpxtz.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2mxbhztjv.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2knszvdlp.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2oynhdxjq.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2uzmyyijh.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2fbgsklbo.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2gnzrzvth.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2jtiacpcb.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2rkeqbrmw.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2bdxagoxe.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2ztvfqhtu.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2onkyblqf.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2tpohkuot.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2dsdsogty.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2hemxzgwh.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2ynhtaytm.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2lodvplqx.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2husnazge.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2uiwhosne.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2gfmhwkeg.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2twodnpar.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2zicqfbvo.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2umzcpgjq.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2irgdorex.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2cobmwovt.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2safbiokz.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2dlnpeqoe.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2vljjkfip.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2xgptenuy.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2fsrylqhd.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2elwcyzmv.html


<!-- 参考信息 -->