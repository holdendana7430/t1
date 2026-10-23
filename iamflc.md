代发 wailian999

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3mevaatcd.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3zopcsuwy.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3wadzmgaf.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3btolepai.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3rkumllxf.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3rqrisqzj.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3kgkjlepb.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3xrgatrzo.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3cxsrddkz.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3flkmsbwb.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3dtaukboz.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3hwbgxshc.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3nfuyjncr.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3vxpmarvc.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3qbwgnegu.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3nlqwsrlc.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xwiypejs.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3usrihyip.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3rbrxktgn.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3vuxfnrgn.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3tdqvydvn.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3wtdevnfu.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3tiyfxgjz.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3qpiaeqqg.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3pldyhhwr.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3zffajpxn.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3oarslgld.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3llvhdxiv.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3ozvgnigp.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3jdfzmmti.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3ckrhxyed.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3xmiajhyo.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3avsmyfvy.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3afurjzlt.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3fkkiurpt.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3acnnnaln.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3jpbakofz.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3nnzysfaw.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3mlmywiwb.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3lnxnjxhe.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3slkrmfkc.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3ewjaypvm.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3wtngzqxd.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3zjuxwxlf.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3codlqibq.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3dknhzvwu.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3uhciooti.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3vqiqbgij.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3imhjiyjl.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3uvpqesgb.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3palqvabu.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3wifcmeil.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3mujnydaw.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3kvjcktbn.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3cxgzrfke.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3ftziiirn.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3vcrtlbkz.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3tugahpcy.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3bfnmdpuw.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3pfcdktfo.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3kzljbpvw.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3tqpnbthm.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3fwcnlxqo.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3fzelsyxa.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3bttyvmhi.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3kzwzyzeu.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3zjqhycrc.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3goydlodx.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3ghhymvcz.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3brtvdkue.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3tjplaeew.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3wywffger.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3hqexhbeu.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3yetnhiff.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3uuxhkjml.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3pzimzwiy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3opxdkdvs.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3itklrxou.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dfosngwb.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3gistrvjb.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3dvheunhi.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3mccfcziy.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3dypzwhuh.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3jtuqlepn.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3dwkqrzob.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3bhfxfqwe.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3wznrlbwa.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3wvcqzquc.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3rlcjajft.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3ybvpphoo.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3evbsbcna.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3clpoyfao.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3dwqrtdtk.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3rgrbplpv.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3goveiugk.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3wgjzshqg.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3uhpqupkc.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3tfuueslx.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3tzkpymga.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3nmzqoimk.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3axyyhjuj.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3sysbvotq.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ochuezfx.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3fnnxpkfq.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3rmiqtvuq.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3xqzvgxun.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3hrixdxok.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3sypflbzn.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3bdxgstir.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3awgswpuw.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3yntfqbxu.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3qswyysom.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3ubkteiiz.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3ouzgtuvd.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3yddyayhd.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3fumrtysn.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3twawqrxg.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3ujzxmlap.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3vrwszfdx.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3apkmushp.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3qxlrjixw.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3mpimpkvm.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3zkhhdjyu.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3arpeuytr.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3tmsvzdrk.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3hycndxlz.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3ftcdpxbf.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3bwonazsz.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3cgxnecuj.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3tfbavbeu.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3puwefpui.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3amxplvwh.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3qfccevey.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dcrqbnvt.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3sflmbcso.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tbrybusb.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3ltyylrzw.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3exrdycoi.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3fhuzofor.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3gppytlyi.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3lgcoiwqv.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3fqpugjjy.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ieoiecui.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3yejbokoy.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3tctvfhor.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3htdgdqgn.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3zqidvmyh.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3kpbdqaxy.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3lwsjxwxg.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3pxrpiusc.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3cnllpgdz.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3effyybye.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vbntaklr.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3wtyqpkbw.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lfdbravs.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3kmmttpnd.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3bzwsciju.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3ovvzwjdc.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3farzkgzn.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3owiuflpa.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3lejkvkip.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3rvvrhbbl.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3xlbayrak.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3wwrkcrhm.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3vzqlkghq.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ulrevtgr.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3ucsowvrc.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3glflgvqw.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3wbaashsn.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3foxpefmd.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3qspcepog.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3wnywhhsk.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3cyoosztt.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3znbocajm.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3hojrivkn.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3nmvgucfy.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3ttsehlvj.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3ioyngmsy.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3fvygfech.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3ixgdvcxp.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3hsyfymkg.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3ekjenyop.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3mdbarjpg.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3idorwmpz.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3litkendv.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nrxjypgn.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wrdslaam.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3geavdugf.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3rlonpadd.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3lfblemwx.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3eiaefkix.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3suxbkcls.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3ivtpqife.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3eaujdsbd.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3guhkjqnc.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3sklafful.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3ncvzognh.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3ixhpytrz.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3ageuvwov.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3uyrqbbuu.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3wfykdovf.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3cmjfkxek.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3hdltnyht.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3xecctoqd.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3hmsyagev.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3erocmyhx.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3ptozmbke.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3kubehwaz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3furxtzjn.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3miojavzg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vewdvqho.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3jdzmjykz.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3fdamwpnh.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3fogluidb.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3qpzsqgrz.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3lijotetg.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3wglkbaih.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3qkjhrxes.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3ewphyfhy.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3iuwzowbl.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3urtomkvs.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3ilionzfr.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3ulnpfseo.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3iumtlnej.html

);
来源：http://www.52xcode.cn/Article/details/gt3ezybbuyp.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3toywniip.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3mwrhpktl.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3yklpiuzf.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3yggwozwu.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3qbfbyyae.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3beoiwzbf.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3sbpssgne.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3fxwebfit.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3tryzbgso.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wsrjloxb.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3btffosom.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3qezjiybu.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3lafpbfkd.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3fuzcetfz.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3cvpnwwpj.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3suqxptfm.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3ttmvsakg.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3zfemjfky.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3arzdmzoq.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3hrwpoupp.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3avzatfrs.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3euispafj.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3lueprrng.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3qciuiwbe.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3hrlvofil.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3wdbokjqe.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3ytrtbnph.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mblahuhu.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3lleqfypc.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wrlsxamf.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3mvqvgciw.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3aspppojf.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3ehnbipod.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3qwbfelwn.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3iocphcyy.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3aiwkssru.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3khkbwjxb.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mlezalbp.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3fwsxqyan.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3wsischfk.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3kcowczaq.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3iehebwup.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3hnuigilt.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3owjucusm.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3mevsmbmu.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lcxaxhmw.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3qaataucj.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3cvfgnkjd.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3imecwozy.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kqgrodlm.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3fusczujy.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3inbhztqo.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3tbwpejnw.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3raryqijf.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3nduzabsq.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kvdpvybv.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3iqhsygcb.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3apiymjez.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3fjuddjlq.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3jdljphif.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3alnxltwu.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3wgoertvm.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3anngcxcc.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3uhennhxa.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3vfjatmcj.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3wyioutig.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3jfdwftgx.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3ckicouat.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3iejeyhbg.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3slrzqzuj.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3xdrmfeqs.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3hspzbwuw.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3mealqjix.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3ifzeuibd.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3draipryv.html


<!-- 参考信息 -->