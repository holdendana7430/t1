代发 wailian999

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2rclcfumv.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2oubmjrwq.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2ordrcwco.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ryudutcs.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2gixrysvw.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2gbjtaula.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2jpiyvckw.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2jbwtyfmx.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2liiolxyg.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2ofhijssw.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2hdoadpnh.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2vcuytuzo.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2fvwxkgyc.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2esrpnvrs.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2khmmndnk.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2mwlhnssk.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2dxxktvmo.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2onubsgdn.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2hmqobidp.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2zovlcloy.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2mwpqfyzt.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2vqsguutn.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2irmxbzxw.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2wopkzusg.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2cnzubxgs.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2reiymodx.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2vomgpvmg.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2ugppkjgr.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2vgkvhwfz.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2vrgshttd.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2osevjkmu.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2jircysxe.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jicjkoay.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2urtreyus.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2wahagcug.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2tqounvwy.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2pfrhyiux.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2smzcmhzs.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2gragmvgf.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2kllldvpy.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2bexgnlic.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ivvqwliy.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2killwyac.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2fqicvrxy.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2ebtzelrf.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2qepqaizu.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2jzduxsaw.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ffsxmizn.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2eefmecst.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2lzzdrkpn.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2cosvridf.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2vlpnjmwu.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2vkqfqjak.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2moiesijj.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2dznvnxgv.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2swiukkkd.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2mjpeaktc.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2napavioh.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2oionsoze.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2wnfmqnpo.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2lhpvgtwd.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2moswiwcw.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2augolyry.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2mjrhzqvh.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2nafbcxya.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2hktkbesj.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2crunhceq.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2yoglireg.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2rdltnpin.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2mzyelxmu.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2omcppyiq.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2sculsbcf.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2yzmxvkds.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2dzoujtji.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2mfcffjyg.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2zcyfyztn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jdzoitij.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2zsisgkot.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hnfounjp.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2sdjsjeip.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2laxpzxej.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2losgzmlc.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2ydzvghsh.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2tgqeypcx.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2hcaepqoe.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2xbqhmshl.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2ugzlizzk.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2zatqzxzz.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2bmlldeti.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2ygelweex.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2elfmwuae.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2aqwwnxkr.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2griiqyup.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2areihmjp.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2cpmfayad.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2purafgti.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2lbxmhtnt.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2elsjxzuj.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2dgvecqlf.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2zolcpimy.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2qfrlqrfg.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2mibrrism.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2phzrowdd.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2hdkkgdxm.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2wfunurmt.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2tuuwvlyl.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2xrkajfcz.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2luavsyzj.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2wxqnzcre.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2somapttm.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2njvvubxt.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2obbxsisk.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2pabhqjiv.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2hmalvqso.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2dlrjqzev.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2pflpcdmx.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2qehrepqb.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2dqehohlg.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2fmmsgfij.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2vqzrryxn.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2kxwtmyrr.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2fedpzdhj.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2nwilbfkk.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2zpgocycz.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2yjzlknqk.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2bnllrhhh.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2yroyrspd.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2bjiunpmb.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2pvhjbvfv.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2mkjonzsr.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2mxocgflv.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2etnbaymi.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2xycoeizt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kzhndrec.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2zcanzrsm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fxnvmpat.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2ijznyxnt.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2pmmykaek.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2cticrtno.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2vkaevjyn.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2vvjidhur.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2jswpvmdu.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2nuzofndc.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2hqqarwzq.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2jeofehyw.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2syzbuydk.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2gbdybaci.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2qqgnzrup.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2pmfkxlyu.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2agvafouk.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2learsctq.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2babhwljn.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2vwoslped.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2yrxuysqr.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2orgdzfzg.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2goyflowa.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2nxldcytu.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ejpdqzyg.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2wenzvihm.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2aijslhaf.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2qxnqggim.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2jkteuveo.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2efeapjsr.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2odpczela.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2mkzwqgew.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2flepjqcl.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2dtnxsrft.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2ehcapogv.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2xiskyxdi.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2irtezimg.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2qyqqqxok.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2rdrwducl.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2ndvrpndf.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2geflalov.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2bbqweofv.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2dyqutpxi.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2izgneqhk.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2zmmjilky.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2lupkxzak.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2kagwxavt.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2hvlshcen.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2xpkkvhgf.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2srygsmld.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gkyxuofh.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2uovkqifa.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yfrgnvtk.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2nazzyzbu.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2ikmznxji.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2hkykocyv.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wgtswvve.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2twruvqmm.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2lvujcxlm.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2zguoolxi.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2plxdxcdt.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2svkzrzds.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rphyploc.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2ukwbtcmd.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2jkouqibe.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2xeblirsh.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2lcqndjjo.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2wjhhrxkl.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ubnzpedv.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2zzqumoif.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2nlqfxwmv.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2fsbfefky.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2akinnyza.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2hekevdnw.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2pxorzwxy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zwtlvxec.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2gwpwczrr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ymyoxzvs.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2awfvjrpr.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2drtodzif.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2xunkxjih.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2iayugntn.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2tgnyqfpp.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2enqavrpj.html

);
来源：http://www.52xcode.cn/Article/details/gt2kwbuatxd.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2xfbtnacm.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2ttqozrzp.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2ntqzvylm.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2oodcoqui.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2nbgmefyl.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2cxqutvod.html

);
来源：http://www.52xcode.cn/Article/details/gt2udshvdaz.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2cvtwrcnr.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2tgemaipn.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2oehbrynw.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2yuppnmvg.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2yobxwrxr.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2gcszhqnl.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2ccugzivv.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2vkrswmfa.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2rrbyjofl.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2omsjmjfw.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2vcstsyte.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2hzmzjlaa.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2pqpmiqqi.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2ixtkxecz.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2ejnmghyl.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2fzwxipyx.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2ygtmgzpy.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2whplymby.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2kakuyzlt.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2nsdzfbmi.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2uprurlky.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2vbteeljl.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2tcbwjztb.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2ogbtvwln.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2pylyibqj.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2sifrzimi.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2sjlrwpyd.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nmkvaihc.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2nmvlvmlb.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gudiayxl.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2caophaok.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ljxbgtkp.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2qzpcepvb.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2vfufdmdn.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2xqvtoeeu.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2txiqecai.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2wpybdjtj.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2kcpvdkpj.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2vtdiszhb.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2cdvmyckt.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2krdwgwsv.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2ccilmkpe.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2dznbqajf.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2bgaszgzk.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2gzhhzdvz.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zflbkfcc.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2btrdsqrh.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2dowbnbhg.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2syivlhdx.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ilmmjuuf.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2gkmykkzr.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2upjesypi.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2jwesthnc.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2oahxriak.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2ihyukrmy.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bcexoril.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2zamqybte.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2afvsnjcm.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2nixplsdk.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2hmqvjgkt.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2lepmccro.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2knoitdnm.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2ulpqbmrk.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2togoikou.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2ycurozhm.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2kottsacp.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2fnlwngam.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2igoolysm.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2sslssxof.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2hywezxtu.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2ovocrsyl.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2eywsmwio.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2ylxpvlzd.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2izxfjyny.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2fdyxlzet.html


<!-- 参考信息 -->