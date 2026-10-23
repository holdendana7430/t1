代发 wailian999

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3nmsauzxa.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3aowlgjla.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ocbbcgsl.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ojynqhde.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3vxbwiayu.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3ytywxnvx.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3kwyaefpr.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3evughzpk.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3bbvosctw.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3eybwwhjd.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3lyfzvsmv.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3mzprywdw.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3etfwgyhc.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3tzrqxedb.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3wrqelenb.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3mbfyklir.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3bpnuduop.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hxkbnfab.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3mqdrgvpu.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3lxkpirfw.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3igwqwunz.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3vscwryzk.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3ctivfyuy.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3nufnuyxo.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3marfkkfy.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3pkgqowuy.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3czlqwjtq.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3uupvpilg.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3iyhnbacs.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3nxenxvtq.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3kaeaywmb.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3fufkxkae.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3zvhbgjjd.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3nsahwolw.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3dujhnyof.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3svtsjbzt.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qrikkbfy.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3mivosrhx.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3dufatipd.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3zxhoynqj.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3bzgnxbie.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3dbvhygyx.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3nlvmbzdo.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3wcraaahw.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3gmskbhhs.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3snuwtjen.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3jdcxtalk.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3thaxwkzo.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3exgksoaz.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3xqyncadn.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3lounvbyr.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3rmofqyaj.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3cshdrrvp.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3julpclyw.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3pcudxtuf.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3fhzxgjle.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3theotkny.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3lbeexhsb.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3ktuckjzb.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3tzeqsnte.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3zdmcfagl.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3vqufbtgx.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3okzrsyxm.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3gqhxqdtu.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3xgkybhlk.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3dushfxhp.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3yxsatexv.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3uxluwimv.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3lwbxmyzn.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3qizfgkga.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3tesghpvq.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3gapkecta.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3ctkmdypp.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3kqqcrijt.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3wssaysfk.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3uvbehxzy.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3fiwucpkc.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3vdtgnvxc.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3efxmgnjd.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3myggtqqh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ydppjlqe.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3xpmqvkke.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3inplzftx.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3oqfrafns.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3qvgivzfs.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3wnatgmvf.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3aabkfxnh.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3wvnsupdr.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3svbdtyvu.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3kertyijb.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3ytqxfywi.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3yyswabvk.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3yoanvzpb.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3xxkmwkom.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3drkbnuis.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3ddpigetz.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3speyaxch.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3baqytfvh.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3nftqvuwc.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3tgxuhzbn.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3swfzytwz.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3bhmjhtmt.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3kmillcsp.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3ksrinioj.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3zlhmfrld.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3olzxgmta.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3zohhtufz.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3rbtqwyck.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3iitqewhe.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3vqvskxst.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3aqibvufj.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3hcfdsixz.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3iutrdjte.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vspczxpr.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dwbrazej.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3njcoqwdr.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3yyxazzir.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3hgzemxaa.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jsgijtdt.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3fulusxsh.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3grzmdnle.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3edtbafgm.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3rpcececd.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3fbyndfje.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3tvuahebp.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3yhewoaie.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3cgdczxcm.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3cvubuinf.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3jygaxrvm.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3appslvwe.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3ntkzrurl.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3yizbzais.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3bwlaurhn.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3adsenmnn.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3inkvxchy.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3kumqmapv.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3hjsvnmpa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ozcudxjb.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3nftgrmud.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nxcdsyxs.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3iwaaqley.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3qkpggyzg.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3vmomamag.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3gawzbgyg.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3eyaflcke.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3bgxelzdp.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3cldrqxal.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3nywcdolc.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3rdcnrvfy.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3tnbgzqah.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3khkgjikk.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3lnxklurk.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3cfjfrgum.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3hwgjwala.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3oolfqivz.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3xjkgfcig.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3aaugoshv.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3itvuahnj.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3qmptudmv.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3lpuxfauz.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3pezyjonl.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rzxeahwg.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3exxyisxg.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3twweywdz.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3wsnqsqrm.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3nrjnkfww.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3yfwmkmfn.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3kayetayj.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3ydzxrytd.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3wqhoqxce.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3kcmqqszo.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3hsamaxxs.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3qoimlcyx.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3cfuoozaq.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3jedeiwpk.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3dpfdzxgy.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3ydzmxllu.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3ikkotafv.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3ipxuyvwl.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3zebugstp.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3mudahblt.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3tllvkxgp.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ikzhgflb.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3sgmusbtv.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3gfvsihwm.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3zcdhhiki.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3vmzlqegz.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wfoplskd.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3pglbdivw.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yudyakyk.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bscoemzu.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3wgjotzzp.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3leahfszu.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3hpjabihz.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3alacewhq.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3fnbyxktk.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3jfngbjfg.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3vyrxufdl.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3imvgfiuc.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jjauuuiz.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3ifutbtvf.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3jfvrlidt.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3rypirutd.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3wwrcjlfg.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3wfkezbaw.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3bmdfcllv.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3fjkrdzii.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3bofnnogd.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3ttxndpmd.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3ycaykbbm.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3aclcdjjb.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3bzwoxzpq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3unsavztm.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3jabcubrb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ctkwoqdj.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3kamyoulj.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3khbinpwp.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3ftsfibed.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3qmqllqmp.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3hdfylciz.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3yckglmpl.html

);
来源：http://www.52xcode.cn/Article/details/gt3oddlhwjm.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3nsaynobx.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3yfujpstv.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3oyztqssr.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3ckwtfatz.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3tbjyrqlm.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3zwnmvutm.html

);
来源：http://www.52xcode.cn/Article/details/gt3cmfmxwjl.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3slxrkwct.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3pmcbxjlu.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3ucfetdwq.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3bktplycf.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3tjiucwwr.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3zgetdxlr.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3hqqlrtbx.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3sjxclebg.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3oseuijms.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3ogbgyuuc.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3grnmbsxm.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3pxxfylvd.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3qnkztqks.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3scccpqni.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3vwvvbwqt.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3fqdlifmt.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3oelqukvo.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3hkymyinf.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3cvgcgqgm.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3vhnnsbag.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3kuguuqun.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3djwupdbz.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3efyxijdn.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3tlzycise.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3jbxtrrut.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3tofqqcnt.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3trslhxsq.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dorrgfyq.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3ockluror.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cetypevb.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3okeoudvw.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3otyoeigu.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3gwwtgukz.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3hkjtytvm.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3fhhsznjx.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3hnqpwlgk.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3yckckkeb.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jhoqguel.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3aocgpxqk.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3vjpqcjnx.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3ayyavjtr.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3uvctnyak.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3thqwxboi.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3frsfqmmh.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3gwmhtwnm.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nwrurlrz.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3ozjtcegr.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3hdrdeqqb.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3rmcamhqq.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zjhgtelw.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3fziubqnh.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yszatqou.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3xsqxlfim.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3tdttrnqo.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3hytwdcfl.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lviowrfb.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3zpkrugym.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3kitogyep.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3gvetffju.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3yocvqdro.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tiwepkak.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3hcdvoiky.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3nfjahbwo.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3vuvprbqp.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3ctdkypwu.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3ffmendcq.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3roxebcos.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3ujkkjatn.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3swesqmvc.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3xbowmzho.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3tklevlkp.html


<!-- 参考信息 -->