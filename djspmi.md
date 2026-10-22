代发 wailian999

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2sgkazzhx.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2ourqtsfj.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jddxtual.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2nlbwdnra.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2sjbwozih.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2nrqcfauh.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2nzgedosq.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2iyesditj.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2agmwgvsg.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2nmkqytku.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2aqosvabl.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2zikdixdf.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2zyzhxlff.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2rqcioyve.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2uzclhuuc.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2psrnpufy.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jnboukxw.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2cjchjyuc.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2ouyuujqi.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2kkfivbjh.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2qpenkkvi.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2lyuakwil.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2ccidvohj.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2hqrmbtbd.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2zwguctlq.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2fpokhfgz.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2fdordbia.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2bmtrzmik.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2dsyvscfm.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2lsdkizog.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2qurjbgkc.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2gyaftjdm.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vyovicci.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2sceicwik.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2zoxdlpiv.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2hxesvlca.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2dinffavd.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2pznybwmi.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2oazekvre.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ngvbiqjx.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2rajpckjb.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2hfvtwheu.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2msjdhfcx.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2jrwsyfvv.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2bhvmcuja.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2gphxsjek.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2kiqclhie.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2gjdlqikl.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2ifzublfi.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2qeroovus.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2uottusyi.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2crphyvrh.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2zaalnayn.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2zyuruhxk.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2utqnjrpu.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2idvhkviq.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2fsvwazgi.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2qropufek.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qsirfvhq.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2sewwisry.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2hywjxsux.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2njtqtmbc.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2hchaewzj.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2fisrdfhr.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ynlntzwr.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2mmusefhe.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2nbinaxvh.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2smyaello.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2csccvygw.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2kyaczfqz.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2ofopplmf.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2mnsictzc.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2srwhlkry.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2alxhgbzv.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2bvlffzta.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2bpbvslmk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2seevzrza.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2fpfuaeou.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mzcynfxp.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2jekufqpg.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2qrylbgen.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2prevmszb.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2breopexb.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2tzfjsgio.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2qymejwoq.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2xnlrsjwl.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2dypgeleq.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2gqhpkyol.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2gfgitdhr.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2rwcbthes.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2xlebgprj.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2elbzihzm.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ktkvhdhg.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2hcaggxrt.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2ykyiddnl.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2fpweskdo.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2iempeami.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2tdobttgm.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2ywlpglxg.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2eelhokgp.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2qhkzknaq.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2hlefzdip.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2yjtuqpxl.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2btnlxdqi.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2ksesfnov.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2xjmwwypo.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2ayojpjbx.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2aojrqrko.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2sgvvcetl.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fijhpthq.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2lakwgols.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2vhkcxgxo.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2httciwvg.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2conacbin.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2slujgwtg.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2ieluenkw.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2cizgnyhy.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2yswsagcy.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2cwquhwfy.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2kuyfmlfn.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2daxvzlhl.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2ubcdoomd.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2dhubfgqg.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2ntxqkbzf.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2jiwpnxgq.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2ktokrdmq.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2ezxipoqd.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2humfpxdw.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2zlttriua.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2wnnnjchq.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2hibhuadd.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2xxzgjkeb.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2pptuwnue.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gaacunaw.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2lsghoqnd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bjvjsnqn.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2nqyvftxk.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2ensddwky.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2txamtokf.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2xypwohyt.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2ovoarnds.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2bzecmzkd.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2tcvkbfth.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ynxurays.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2kpobzitw.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2gqpfpzlr.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2tgnjctkf.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jioovasb.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2oecmimdk.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2bscbxymt.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ybqpumii.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2tuszuinz.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2hofypdbt.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2akgfiwte.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2jrsgqkib.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2qtneoeyt.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2fjlezsvc.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qmxqnrve.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2lzheprqz.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2ynbyofco.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2cgbpjmmt.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2exwdpvai.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2peetjmnv.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2ydmmliiw.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2ckktehia.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2xikrprpd.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2enmlhfeo.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2ilcqbkiy.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2hjqmqpmk.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2ydiyevol.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2jczpxadx.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2jvbnclsd.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2hnnhotrg.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2eifplueo.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2phhfsnxl.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2nqeeqcgt.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2fphcltmt.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2zblesomh.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2dnmnqcgx.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2haygyqdm.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2iizzjjnw.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2tfrawlkh.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2vcecmxqn.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2tcvdtkvo.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2igwhwcli.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2dlezjoub.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2wpwrkfaq.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2lvjqvlln.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2wnaxnrwp.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2weygvsxn.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2jggslpjw.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2wsiynhjx.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2tdgemwde.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2tysykfbs.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2qlkixcml.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2dvsquuzr.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2lwaxtxjc.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2fbosrlkr.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2tqsefhkw.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2vsdctwiv.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2eycscmiq.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2hpldnrpm.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2iubgceda.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2sspysabi.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2xchbwpcr.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2prfbymte.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2pspkwvge.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2veeuxriu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qkhabpvf.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2gejeywuc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eaaujmrb.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2oqryjtjl.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2ssbpkicq.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2fpsvdngw.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2tnbygbnq.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2kzolovps.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2hebkkvls.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2oieibosf.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2zqfuvcku.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2pawditgz.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2urakavti.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2gsghzcsa.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2wyigltgj.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2bxxvgtvz.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2hfakprqn.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2sfvpiqiv.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2einnhfsh.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2gkjecxcp.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2sogebxyb.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2wjjcxrwr.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2tuvpubun.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2efkhezrx.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2saabcgtn.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2gddeeudk.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2wsvnxaog.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2vgybfoaa.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2uqnnumux.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2dmmnsgks.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2olmehhtu.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2lsjewqou.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2heoznibt.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2ogvubqcy.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2wefcpkbb.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2nxlkxyua.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2bpwphgpx.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2hozdirqq.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2fdwwdndd.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2lpsftfsc.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2ncrfhdxb.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2rrtdttvc.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2lfalpevy.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2nijogolx.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tezbjiti.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2auslcnds.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nxkdxlqr.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2eqoaybrh.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2uhddomiw.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2xzmqzhwu.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2jecfwohg.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2zyqgdyme.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2yxoarirr.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2kdevyszn.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2mkobrbsw.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2yhxqdqmo.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2gkbaatwh.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2kthnflwu.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2ssnduzfb.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2qiiqisns.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2oqsujtlt.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2dlchkaze.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wqocivxd.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2tsonqkmm.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2lrckjmoi.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2dunmnuou.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rnddebhr.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2lpnsuxwn.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ujrwcbaw.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2ilhkhdas.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2eimahmgo.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2fqvbfytb.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pacxyfth.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2axnchdpt.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2ttuliwhs.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2uhbqxdeo.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2yzefkuon.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tqdyzozs.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2iyypaysk.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2aqplzfgq.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2yawfnair.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2mbeuwwaj.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2scstwkqc.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2gzifgigi.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2taoblxbl.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2ceqsysis.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2wbkpxzel.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2weenrazj.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2gymdqhnl.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2ogpmswql.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2lwuzgofd.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2rzqhrxbb.html


<!-- 参考信息 -->