代发 wailian999

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3vivwzjph.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3jbqewksp.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3kzojnvoz.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3phbuofqy.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3zyqvghbw.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3hecmafrm.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3pehbrwfo.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3ckusinbl.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3yfejoblu.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3mzvnkypf.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3uyriharx.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3zmksyktk.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3xuhlnjrm.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3rvzhcgkz.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3smoybwpg.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3nobjosex.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3xgslktvx.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3keuctsnw.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3slnktcit.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3ybofbvto.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3ewnbnbsc.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3exmlgsgw.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ckdshivx.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3nbgzsygw.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3yedswemd.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3iajkvuqj.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3vdqtetzl.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3nbgdckbz.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3eqsrqwtu.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3rzuilqyd.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3irqupvgu.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3kxnjbmfq.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3tuajcpoc.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3bbkkqsku.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3xnbpumia.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3uubgunkj.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3jtswlnxj.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3cobrycsv.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3pntweqbe.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3ucebvxvt.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3eqeqngto.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3ceylwnvj.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3ppetjugv.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3ahbostyi.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3yjgprkwu.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3ljeizzez.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jzxpbnwa.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3omganfbk.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3qrwpxwfq.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3thpbwyjm.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3mznybgvz.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3idlvpwde.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3fnaeucza.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3wsyrsapv.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ycmavzwr.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3sqmoxrte.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3kjgkoknc.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3daigesjg.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3fyodumdt.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3revnbmfa.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3efrjzbfe.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3kbbtlalb.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3urxnfiye.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3hpovmhzl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ylnxpnsd.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3qzjznyxe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nwvmyzpb.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3hsypkbkk.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3hgoqurrz.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3orrbuipb.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3eqqyolfm.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3xhwxhnag.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3mhgcblui.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3vyeqjfrd.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3oezeimze.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3wplwjtvm.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3fehckwzq.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3hahmsssm.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3jiocfkvf.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3dhgpqdmm.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3bnwpkoie.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3qqyzdrkq.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3ihpksuqf.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3gkmsljty.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3bekudktw.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3keivxtmq.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3dbkausys.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3almhtemt.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3zupnbsdk.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3tlnpddij.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3jwnsrfvx.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3dyorrniv.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3abolwfid.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3iirmcetc.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3earpsnbr.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3lahutios.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3geiyoduh.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qmmabvvt.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zbkbjwxv.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3hwuepnjf.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3upjxxqvm.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3emarlzsq.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xewhafpb.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3anhdsocc.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3efomhlpr.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3mbmkpzrg.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3qmixapbe.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ztarnkrg.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3cwnsqcgv.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3byqhrnba.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3hxcuqfiq.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3ydewncpw.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3eypabage.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3iawfgozb.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3jbmrfijl.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3fftqaruu.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3ffzghlbx.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3cxndrkuw.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3camztdwt.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3vpncjroy.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3agksomae.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fauaeozf.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3yjjjvypl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lldpeprq.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3luoqtmph.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3kwjjeady.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ulujgpde.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3tnamjgwh.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3hgwrlfbm.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3lcjcvxra.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3etdxdwun.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3uldrcmlr.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3vskfsreg.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3bzigatnn.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3rmgrvirc.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3avngrgtj.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3olcoqcad.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3xebjvujf.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3jwqtorbo.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3wudmthoz.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3shlmheuv.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3sjgkhjje.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ykghsxaj.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3favacdgq.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3ixpldfyi.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3unmkalnq.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3dkmrxeaz.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3qilijhmk.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3avjmzaje.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3eyvlgpqm.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3zaqhwfoa.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3ldzxcymm.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3yddkdcbr.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3rronikic.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3ciqijixr.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3dkbhqgrz.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3vfmpviuy.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3qyqdmdce.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3ujxahbvq.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3qnwcibex.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3zceacpzg.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3igfepuya.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3alloeghh.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3bbknnkcx.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3yfjgowcx.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3vadcmryr.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3hiuveapg.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3ctyqlwtz.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3vaovpwmq.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3tiipnomj.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3azqqfgpf.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3jvaqnqki.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3oefwrdrw.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3zpujdvoo.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3frezeymm.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3gsvsdawt.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3ohqdmesp.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tmtravgh.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3weyriwuh.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3qjsuxcts.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3dtmvgeyv.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3uphfvuff.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ovywqhfw.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3ghpnoyxg.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3jbxtpitn.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3aezaroay.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3gzlojrzp.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3xpsfubfw.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3zdzpnvfk.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3cldniave.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3dymevuth.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ebyqynkz.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3fazdqpsq.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3mmgqbgoc.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3jihisdpr.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3cmkmvpvr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ocvbauxg.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3pxlabqga.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fltynwwe.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3ghjsgrce.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3gssibmmg.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3ertuhfpr.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3nwhzmlvt.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3zfzpzonp.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3rsmgbrnu.html

);
来源：http://www.52xcode.cn/Article/details/gt3rvnmwstb.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3aezragjt.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3uipwysne.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3zlyguoya.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3xnzdbcag.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3iqqomoeb.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3zxxauibr.html

);
来源：http://www.52xcode.cn/Article/details/gt3sqmrrkfg.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3vjogrpls.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3whrobbzs.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3mghxttgi.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3yndjxbna.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3qnyeqsvy.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3ugaxdkfy.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3kjhoiaee.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3uflzpugr.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3gfzwrrfk.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ftngqefp.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3jqnrxnui.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3cifxesft.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3npgmxqma.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3yijddmrm.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3voengife.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3wqxbbhbe.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3jcsxourf.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3mglaoggf.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3xbplhjya.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3nfjdzpbt.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3dvcsjncn.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3vlqrzggx.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3dztvjgvs.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3rwtolies.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3nuqcijql.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3adzbydjr.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3eedksgtc.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mctrepqu.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3xwbzwuwk.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3awtaeexb.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3bfhyshqh.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3djbnqqrz.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3iwndsjdp.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3xcefeyeg.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3dufdozrz.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3nmlrvqoa.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3crcrqzxs.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qhhjwoki.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3gcomivzb.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3hlurnfye.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3tgqwvltv.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3qvimjnnq.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3vgcjoxom.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3obqipkqq.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3jxgzlrcg.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vbaclyaj.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3lxpxjvti.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3ugwjnpvc.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3dbaimzlb.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3omgivylp.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3bnbeitgr.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3koelaers.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3qeekfgoo.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3cfhggjcr.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3kzvvyoaa.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xuqphrfm.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3mcswxtvp.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3vnnkychu.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3cqzhzafw.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3rykbkbbp.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mgyfnqru.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3kabfjhue.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3rsexayuk.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3ywyuikxj.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3hlyypvir.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3reyavrhh.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3rhgfaxsi.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3algtmtcw.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ycdfttns.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3camddtgw.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3pkixsgun.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3ujmwbsbr.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ngnzwelv.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3qevybtyi.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3yjhjtejp.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3vwkdznoz.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3fbwnkyjk.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3tvjodfmx.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3djtnqwbe.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3qzdnilsz.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3pmwnrlet.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3sirffski.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3ruddcwae.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3dbhzawnx.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3aoahqxnv.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3avngdpbp.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3grsssici.html


<!-- 参考信息 -->