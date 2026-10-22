代发 wailian999

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gsnejntb.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2puwqkggo.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2nsfnpoqa.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2dxyrltim.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2uibjsdfn.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2fljujpxw.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2zwbgbhhm.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2iexncwkl.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2jrsthxlf.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2qevqxwnu.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2mpjpbpez.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2danagdvc.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2oldqsmni.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2gwhnqbcf.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2jihnstiw.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ywcwygza.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2cqtkhpvn.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2qhjnvwvr.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2sdpnbdgo.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2gcyysjdf.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2vjcybgwi.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2tlphzoik.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2umwhjpwi.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2aweniptv.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2svdfahzh.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2ulyufkpl.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2tqghetsb.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2etxwdhlj.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2wnuefpeq.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2kfqrkugv.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2ubpeaqgc.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2xggnuhqf.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2dpbezpmx.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2lziuvoml.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2owbcicfk.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2khqrpuzs.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rdvjwuww.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2cafmawha.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2cmrbivcp.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2lmshelbm.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2rqzvtlog.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2hipwmdcz.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2iidwipij.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2aijfnjxj.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2nqeqppnb.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2vfwiqtfn.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ssrugtdj.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ntiarvvi.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2hqslvebk.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2agjodbqu.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2ptygivxi.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2vzqhemtp.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2lxbpfjfd.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2mbeeirfs.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2tnzwplia.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2tuwxblou.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2gqrkyxje.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2dnmmctsh.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2ewzlyiia.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2egvxjctk.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2sempwnhg.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2itgwvjer.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jbywulua.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2hqylfxzc.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2ncfvvqce.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2rkgyjemd.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2luzmdvxw.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2oqacxgja.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2bkeisluv.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2ctjjvhpg.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ptiqjdyn.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2uzvzyblr.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2bjkrgytd.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2uoysdqdd.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2ccikefos.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2vsvhbhto.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2rtsmrzxu.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2zunabnsy.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ajtrecww.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2bmxgmoxo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vwrysbuq.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2knhemszj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bvjjmabd.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2fchmhdtn.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2epmbeupe.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2ezqvrvpy.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2wepvosbq.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2puhvonrk.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2wsptpldn.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2suyxbvci.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2kcsbihiv.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2bnnomuug.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2cpqyjhoy.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2vpictalk.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2sfojyitz.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ohzylndq.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2cywdiadf.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2ympmmjnc.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2hkojekng.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2uiwvtncm.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2ieszzfbj.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2dqotlotz.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2rjmjicxm.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2xqgzrkaz.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2rbidlgew.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2nmdybheb.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2vfeqrozm.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2eydpkfjq.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2buvgeyfb.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2mcaudrmu.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2bebphstt.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2hpaqwrsw.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2sfboswfy.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ktxvpdzi.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ozhvnbdr.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2mknnvpti.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2ikuyapro.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2iyqmhmme.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2yaloaxwq.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2cfclapdd.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2rqkotqad.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2jehgnmgz.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ujpunkri.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2roeedthl.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2hqhevfgs.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2inlgfqew.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2byuudrfo.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2omqdsxiz.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2gfmhtrya.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2iuhrsnot.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2ilzysgod.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2eskgolcm.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2vqiunxpl.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2cvuanikd.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2csofklxl.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2pznrdibl.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2gsfumpwa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2llbidspc.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2iluwetyr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ddtyifhi.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2jyqoklwp.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2xuoqvleq.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2upivinqq.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2elmvdaqn.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2uvwdamlk.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2mnyrfsgx.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2lvvpmzmt.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2hhglvuwl.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2ooveprrm.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2eeppeati.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2qahfjdou.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2kfyqqtla.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2kbogybhs.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2zyxlcjsj.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2sxspmidf.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2yozaoryo.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gjixzryj.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2ppwqdbif.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cyujrikn.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2vwzkhchj.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2itocbuaj.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2onouuopp.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2pjeaypnt.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2dfwnvkqj.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2zqzowzuo.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2tgdqqmjl.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2fdndedax.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2rhvhdqns.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2mkyzztfd.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2gcqkirmb.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2cxekwjkr.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2mnlmqben.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2qyowgvfl.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2lltejpxb.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2cqfcydia.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2rkeefdxs.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2lbfnytmu.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2huxovlzj.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2eudlvezw.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2yflubqkd.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2nlwfdafb.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2uwthjozg.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2pwwufsee.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2pwhmhqdp.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2afkrflgx.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2wygezrcq.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2zkwubabm.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2tlbesgjf.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2vznysghm.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2cnzcxstl.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vabwlkwe.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2ncrwyfdc.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2omxxpnig.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ypixabup.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2fmwteqao.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2ythmaghi.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2vwnpbatc.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2hfewokrp.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2sygrqcpi.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2vqcovepo.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2snotrlik.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2gmlxtkgq.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2aajmuvbx.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2gzvwqxth.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2qamibpoa.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2fjyuqdgm.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2hrluchse.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2zagoqbyo.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2tscnyvhw.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2nnxzlfhz.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2dulgjygk.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2kfipwnsh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pneykvjx.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2hmyeglin.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2smyfhwfy.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2nqctndoz.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2wteffowm.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2dalexlei.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2tdnossll.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2lyqldfhs.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2rnlilyrg.html

);
来源：http://www.52xcode.cn/Article/details/gt2ppldiqde.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2ykafhlhv.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2pxjzytkt.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2agakcfit.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2ayymkshv.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2paqndgob.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2csqmibqx.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2snorbvlj.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2gphmazss.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2uhihhslb.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2jwtgwzxw.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2mmmpvtwn.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2fmnvizlh.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2amkpyvqf.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2upiuqkbj.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2panaudpi.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2lsyjwcmr.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2ugnyyipd.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2dpnqowdn.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2xucxxsen.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2bvovlkgf.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2phtvuivr.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2exiygffb.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2tndjvzpz.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2pirushmj.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2kcsoucke.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2sjldmyxr.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2iiwdqqke.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2obcpomvl.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2xppjoxmc.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2buglwyqd.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2nnkgacbx.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2efzavktp.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2dgzhorxi.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2vozvcrkn.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qhjzxdpi.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2vylefyvk.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xyigqynd.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2wghzuuum.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2cayjmupb.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2rdismfsk.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2agfyhkdu.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2rvjygjfe.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2tuftcrwr.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2ddifsnqy.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2ullfnwsp.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2pvqavbew.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2qhiucymu.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2lhixkgfb.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2bbdeifcn.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2gvdoyhee.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2bgplongx.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2eevtpsmc.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xmxnzlpq.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2nudblsaw.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2dnrhuqyn.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2eebajsdd.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2baxwzowi.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2nerqqvif.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2oiqobtzb.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2mrsyatvx.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2saaivjhv.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2mdvdbshz.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2quemikej.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2vbpaatoq.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2biuffkkd.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2fuwwdozv.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2kjzqjlmr.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qzldbrma.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2ygaybjqp.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2zimiejdc.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2lxaqwixw.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2mceflbri.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2lypqkilt.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2vwgbikdm.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2tvhhnjvj.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ltpfmwlt.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2kkmhorgd.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2bdrlruug.html


<!-- 参考信息 -->