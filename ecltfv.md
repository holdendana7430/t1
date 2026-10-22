代发 wailian999

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2fjplxmki.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2lqlupezm.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2riytpfsm.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rjmslvsy.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2modhcmzh.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2qsulrejy.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2ppmooplg.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ynxcpqyz.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2ucbdodxz.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2vozycfuj.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2fqmypfrj.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2rawhyaen.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2tkstfjox.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2ovblirvy.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2gxrdahky.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2rahespmg.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2acpcvfrb.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2zceyjoag.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2roqykezc.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2tkbkqbkk.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mbevknwb.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2rwsttcon.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2sowtxanm.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2uimwvyse.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2bsngytap.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2uzyyrxea.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2salbbtyq.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2sqtndtac.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2piyxpncf.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2dxzfqsfu.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2djbxcqwn.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2ixxnssho.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2wisevsgv.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2fvzzqqea.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2nyxxgqrz.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2jdgsqvqk.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2nxlknhco.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2bavxegts.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ycgkdonx.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2yxktptkg.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2lwzimvym.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2tafsasen.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2jbqejosc.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2imjmonfu.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2nwpuruzb.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2hlimqycr.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ygmcebeg.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2fbkvqhsf.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2uxwmfsjh.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2pnqvgoyg.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2fmlzhzqk.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2yxmjwooz.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2rnnhegdv.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2kqnrobcf.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2ihpogvtb.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2uicddbts.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2hijxdmks.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2cpbnjboi.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2qzhgptdv.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2ekkhjmvy.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2tnjkccoa.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2khkznfsw.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rsccbwjz.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2tofxnfnm.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2xtfofbwa.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2fpnhroyi.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2wduczpie.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2tmvwbnpv.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ohmrzntc.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2wmytptfl.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2arzdyvel.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2nhaewfbm.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2rmhwzazs.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2prlfxqec.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2ayyznwii.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2xzsifsdy.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2bbzalong.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2bzelgyvc.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2sronlsmv.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2ybzimocq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jkribtjl.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2icnmxqmb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fywdrjnk.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2xhprvggr.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2yjxbwkca.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2arkayrfn.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2relndfzt.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2kgkolivm.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2ssyvxfjo.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2xmuzwrzr.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2fbyyaoao.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2etklhdeu.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2mvcfxicr.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2gqajsmdf.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2mceqviis.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2utqljtnq.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2ydoflzlj.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2jryjrkcq.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2xbdhnxeo.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2jqeeyutb.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2vibverpk.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2oogrbfhy.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2oyuaxgwx.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2cdtxcyug.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2epqakfmd.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ivueqadp.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2zahsdfxl.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2rlcvvuut.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2hzkypbqk.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2xntadtpy.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2imqvapry.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2wrmrkspw.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2mnterlmg.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2bkkogzic.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2kctiqneu.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2oprbkakp.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2hfpsjvxr.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2amfomwnx.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2jbqvijhf.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2kgzxohwe.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2cgfyggwk.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2kjamgvhu.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2auvvktfv.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2fynualaq.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2pipfpzfi.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2hbtzlkif.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2tjtwiuoy.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2jrxjujel.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2hgrmrlbs.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2nraqiopf.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2mtvslpmb.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2hfkcajjj.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2cirtujjm.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2htpnygnm.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2ocmtygcd.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2ghsqauqb.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2zduiisdm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zowmfrsw.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2vnofctdv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fihnphyb.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2eywyunkb.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2zoztwael.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2xgqyycni.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2tgrgrvlg.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2tkhxnjeu.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2pqatahjq.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2tcuzvetl.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2rkrvhvio.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2htxknhrt.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2methpcah.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2ukfyyoyg.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2haloyivi.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2kgyguvcq.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2dsqwimwo.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2knafeihn.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2nhjjaktd.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2walwonpc.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2infwgjwv.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lylidybv.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2pkpoekag.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2abppsnpa.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2kmzwtfwf.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2tdqwycla.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2obrfpzdh.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2uycgmjqk.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2hcdissgr.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2xnpyktvc.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2ezrzcxeq.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2hvwqwctz.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2yarprhar.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2xqpduuoh.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2ppfebtwn.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2ubyqocgz.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2lyprfbbg.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2cdjjcjax.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2wwlbhewr.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2yhqqplpr.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2cnkrrsuc.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2qaasysdh.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2fvilmern.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2jiqzhrre.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2ejnfusto.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2uahnogeu.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2mnhjdkbq.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2xvsdwatf.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2bxnsiyqa.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2vzebhrtr.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2vgqfixhv.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2lulfzbbv.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2chijcmxh.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wlgzxjih.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2cuykqtqn.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2ziunkxio.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2teymmyse.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2fmugpryx.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2hxrslplx.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2przvoyjv.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2vbudwxhm.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2apzzrfiz.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2xmwvolqe.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2yhckycpq.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2vityqnwi.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2ztpvzujw.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2dceaxvpu.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2ojyxuncr.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2omjmfywy.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2jyvucmlh.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2yntakrdb.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2cztlzojm.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2ykxhznac.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2avcsuzuk.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2xiscfysv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2akbndwlv.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2fiussmnb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2khptrapu.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2jvovkfgd.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2avrhdmry.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2kerjjhcf.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2aqvdyjrn.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2gltxjeva.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2lsjsizxd.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2hpvewvvq.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2ixsboshe.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2kfzewdwe.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2mwdhowmp.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2ghhirupt.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2ozpslfga.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2xlyrijrm.html

);
来源：http://www.52xcode.cn/Article/details/gt2azklpyju.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2ymzanlun.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2wmvtjycu.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2wibgircb.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2lizrmdly.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2evexwguk.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2awyrbwiv.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2ickscdgs.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2zadpgadu.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2ucuqrwlv.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2jxcrcuai.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2mwwyelxa.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2ldatneqe.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2kkyggcpj.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2mcdqrign.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2xlyepvqi.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2yjtwjjsa.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2yehkwtbr.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2rswvtiyb.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2luuyehye.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2eulmpgle.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2mdsazaoh.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2nrmfeplk.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2wfxlaien.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2oeutzfzv.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2rzrijxsf.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2mdxvypav.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2rnhurrju.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ekivvdfk.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2xsejoqei.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jqhlyled.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2lxrtggdn.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2tqloesyx.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2tnhymsik.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2prugglim.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2hgecxfvy.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2iclkgoht.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2yimkljim.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2qjkyzvod.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2qvwqdqcp.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2nypvkvwj.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2yxirjozj.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2fgxlujuh.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2gehrdxro.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2rhujeweg.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2ewpstukf.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2iubvtxsf.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2uviuwkti.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2mtpoedvc.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2zvnaoxhn.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lfjafodc.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2riffotgz.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jnidwrgo.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2aewzoujq.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2scfmjxdv.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2femeypqn.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ibhbpdmu.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2bzroaswz.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2lbwepzft.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2gxsvsfmq.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2htekfbhp.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2tzneeeeh.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2agqkspxd.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2wraasoce.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2fnxvjnqf.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2dpievlax.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2evhkrtrv.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2erodeyzi.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2cpqovruj.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2zilqrzig.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2qprdoiuv.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2bwnwyfyl.html


<!-- 参考信息 -->