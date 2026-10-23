代发 wailian999

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qkobtizw.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3pwiwezju.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qhakcimz.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3dcucxdpo.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3xoqloaip.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3hivefxlh.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3spnzrrso.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3euxnenae.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3rsunejqp.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3nwsxjfdp.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3lcwhdfrs.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3blmpnjoa.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3xlkyafyy.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3lgcpazis.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3rjyrycka.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3ievimfcl.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3sfcegtvg.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qnwrodre.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3ybvxcnqr.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3ahirycfb.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3nbhwiqnx.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3isijypfv.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3nfqoiztt.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3kcfmtyzt.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ofkfyots.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3launboll.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3qedoajlf.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3gifrqoro.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3govdkpvq.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3fqnadsiw.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3qvcowmhm.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3lpkisyhp.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3tycwhyzx.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3rkrkoauo.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3mjpnexql.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3zyoqhqvz.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kjnhjpfl.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3pafagdfz.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3dgseujei.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3wlnhilaq.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3dwtkxznz.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3mtdvordb.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3sifrlack.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3qpyabzru.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3ljjknolr.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3iqazdexn.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3fmuevaxl.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3nyehrwvn.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3abwbssbo.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3ludkhzoe.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3camkbssl.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3vpjvkvzj.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3gxlttewo.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3jzoqpuif.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3mdbuteoe.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3vjwobmze.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3rcpwzmah.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3vwbkeuio.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3pqbgyces.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3xlczmuuc.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3iyazufau.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3znqazeze.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3rggaqbly.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3uonrrpee.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3kvaybuxb.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3bslpddtc.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3fplcywob.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3aaiqzuus.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3tctrrdzu.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3etsihwpe.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3rfzybdno.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3lkiexgap.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3ybuenmef.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3jdhmtcal.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3kzziqmcf.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3ouexofpk.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3uyclzbhw.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3pxopqzsa.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3mkqeoqam.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3pobjkzvn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jidwmlgh.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3crkrvopb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ipbrmbgt.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3ykthdoye.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3egxdtwgo.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3uctckdsc.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3soiwdrkt.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3rxcybhzr.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3jckykrkl.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3vuirdqrg.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3hwyxddgg.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3ggdolzhv.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3xtrbvcnk.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3wjxwqptx.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3nzrfolkk.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3mejkrxci.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3ekkllhwm.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3beofpsqi.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3smdygswz.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3kgltduix.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3ujgrxdyu.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3tospfbry.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3vceoayju.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3zxotyegz.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3nibxuojs.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3hiloikka.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3wfrojqpu.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3ftzsspco.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3upjqporb.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3fmxxrnuy.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3vfbyabpn.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3waqjdztj.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3ltdjclfk.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cnolpvrt.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3wuwqymqe.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3eqcuyxos.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3vgoptzuw.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3xajecikm.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xvohfcos.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3tnotfstp.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3pjhruakc.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3qluiaekm.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3tjvkyuvu.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3tcczosag.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3iulahmhj.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3avhlndni.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3ppustzmc.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3ufekmotj.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3tloamekx.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3eljwknrj.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3hpcwxklu.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3kfobfnzn.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3berlntbl.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3rupiifet.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3iitjzpzg.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3ysmatbqs.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3qpqchbgj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kagfjnir.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3aocmxciy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qpyctluy.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3tixahymu.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3bwznwvwi.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3dfdbvvwx.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3xtgbgifg.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3nnxjbdyb.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3ypijnhpd.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3rnrihlrs.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3kdrcjhlf.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3corrymtc.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3yjmhrmbg.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3thxhffve.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3dvlncrnb.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3xkckcbni.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3zxnfvrak.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3mlhzytwg.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3thsvqfvg.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vewvvyke.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3rzyasloa.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cttpuzql.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3yhotpidj.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3pewgrjee.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3pbaonpod.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hbyiyfwt.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3tjdmglhc.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3monbxukv.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3bwipdzkq.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3uctcruss.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3hqybetxb.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3bpqaoqmg.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3hdbcbvqm.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3ogoszwzn.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3nndffaiw.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3cnywykfq.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3omsfrgmi.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3majnmasu.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3zajnbmdl.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3oqmtocyi.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3rhonzbpb.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3rtigrcod.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3syoftdlj.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3bdqlislu.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3fqxkoxef.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3lchaummv.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3qsnexnpy.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3xinujdhy.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3cgvokqns.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3nrxafqft.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3ydmkudjh.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3pkgevapa.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3aaxwfmqa.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iswbjxai.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3arkpauew.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3ratydqzn.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yxkfmniu.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3bdfemtdh.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3fggasadc.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3itbvpayd.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3buhtsxpy.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3wvhuoraq.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3vjfwbgbx.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3mbvhtpwy.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3xbxugnut.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3fqrcfzmh.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3xuuyhdtw.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3qjftzmhk.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ksjatkgm.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3oxmvnjcy.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3bpbhhckm.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3dnliybah.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3wbnlqszs.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3najubbzc.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3qlvbbmah.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cwnqutat.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3dagyhjzn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ibocmndb.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3yslngzbe.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3dewmxynf.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3utikqeys.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3evqrbwaw.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3jpglkrkl.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3hxytleds.html

);
来源：http://www.52xcode.cn/Article/details/gt3refzmuwa.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3jbjcyvxv.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3elfcgbdh.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3iqdgqgti.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3xuaocqqr.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3axpzjfas.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3dqybsbbt.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3gewicvaa.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3nzvhnneq.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3rofyvmpf.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3ohsbecza.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3tolgpsim.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3rjcuhkjm.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3ekxrllsi.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3ybrvgepz.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3oaasiadi.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3fjxaugyj.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3xzupqdlr.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3xfvzryub.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3sjqbdvfc.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3tztodtkm.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3ihsznxdi.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3xienajbj.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3lrilfdsb.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3ljalpwkd.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3gwggyjre.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3ublctmkx.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3uqtsbrwx.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3qiymhriu.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3muablujg.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3quxerius.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3xrpfuicc.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3lwifujgd.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3fsobbvqk.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3bllsbend.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rodctveu.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3xtpzhuaw.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jtvvmaio.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3uybgxxvc.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3xpjgtoee.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3viajbrli.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3xbqnvdob.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3lahoqmus.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3fziinyhv.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3mndxqipi.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3akibcpuv.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3qtykqknp.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3hzbkhuvs.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3wgbhamps.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3ubzxsbhm.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3hxntdxjz.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3yowkevfn.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3bihfepaf.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ohxvkfqv.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3rjpdmtda.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3rrkuacbo.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3xvffmesb.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pxxuxhvd.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3uxhqscdf.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bnnedfak.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3ncgmeozq.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wiymjuhv.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3tbkcmcst.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nhytasou.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3umzjckpi.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3wznrgasu.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3zkcorssa.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3jmbfitpb.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3wfvtmter.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3tclhyxss.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3tjmjwera.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3dubgouxr.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3iwmcniar.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3pmykpyue.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3efltojeb.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3esfpitsl.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ggckquqw.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3kwovngie.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3ulemocge.html


<!-- 参考信息 -->