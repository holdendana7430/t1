代发 wailian999

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3tyezblic.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3bhusdumh.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3gccqkgls.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3sfxusmmk.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3zuaaoncg.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3tuhdgbeo.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3sawfldnf.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3sxfrjpfb.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3pgqojhct.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3ihgmjcsm.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3bvfgwgrh.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3alypfjxx.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3yzqcjzml.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3xwxxsnmy.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3pvneyscy.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3dzzrfszb.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3tlgwdjkf.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3alncwseg.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3agspuanx.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3rnowirvl.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3ycudearv.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3alitfplg.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3ouoctpee.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3fsnbhgrf.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3gdbwpxzp.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3tpccffkv.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3gemlwmpm.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3oovqdgji.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3zgobnjhi.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3sboecqeu.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3aeioczvd.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3nimqevpr.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3uikmymdy.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3sypnomjn.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3oknqkgnh.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3btbfksvs.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3midtbspg.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3aidstuah.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3tpyxlmok.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3tbzypzcc.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bwfginjt.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3sfyhvrmn.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3dmxhfpcg.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3exzwpunx.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3tceriwuc.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3fkedryle.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3rnrxlkzp.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3kgtlhoau.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3mvvqofph.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3yvnsqlrv.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3vusxvbtw.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3exzbxdjb.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3gsyhnpnt.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3spsusxbr.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3cnijeosk.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3uzgejmtm.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3mwfsdjlx.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3cksadyte.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3gjyeadur.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3xqsrsjqk.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3smvjbrye.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3pkvbanfn.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3jpwrcziu.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3dtjofwpu.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3uloecgep.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3kixjdnrx.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hggqoxrd.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3xakopcla.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3hzgbzldl.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3prjidhwy.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3qjywzbky.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3hhxmszcy.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3epmxjloa.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3aspmtpcy.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3mowwnzkp.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3njdlfryq.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3tludsong.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3rrmbrjaw.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3qzomnyfz.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3hryvdwmb.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3jtxvojve.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3rwrfqowp.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3yfcfjwzy.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3ujevftje.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gemtzagw.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3fhjglens.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lnvkptwq.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3xgewgibi.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3dmieisfn.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3uhuvdrpx.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3aioyznnn.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3kphxrune.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3igtqdkey.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3dhwdndet.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3brwdxpgk.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3mbjgtrob.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3ufzcpsda.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3xjfkqyas.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3cmxffpft.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3cpquxgrn.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3fzrdafvf.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3tlmfacxv.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3lxdrumgg.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3mrmxqvhe.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3tbfmjzun.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3ecnmqmpb.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3gkosrwwp.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3ucanitei.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3jzcgpuxj.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3vwchokfp.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ymjjxshi.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3mnkxcqcg.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3xhzcpvnp.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3tkuvzgrd.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3kmujnjlv.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3sodryyiw.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3yogeitfv.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vkrwyfis.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3cxzevbgj.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3cfukzler.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3mbpfjwmp.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3ohbzxfso.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3lokbnqtw.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3gvptbkvc.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3asvzsqmb.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3tppmmovr.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3mitswjxn.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3eibjvcdt.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3thrzxdof.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3ryydibih.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3zuvaulhz.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3dawqoaam.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3wlhuimal.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3bwokzwga.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3hyngoupx.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3gaxvjmuj.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3pywmkqbi.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3wuhukwhv.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3rcqlrgbj.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3xfwytwlc.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3pcukelqr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3siqypmjp.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3swhsnpuv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hjnukvug.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3bipkplfu.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3yvkhhsry.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3errnuedi.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3nuspmzbv.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3njxqjauz.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3rxeimhwj.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3fojclcuj.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3jgandezb.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3grxbgnfg.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3ttpemexq.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3szwnpfim.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3joufijrk.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3ebaprgdo.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3ximpyefw.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3zybyvwuv.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3wcgzohun.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hephpcpu.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3yxgtcnma.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mrgpilcs.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3tnwvmlsj.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3cvafgqnh.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jmnomzwz.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3jrdnwswd.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ynarjetw.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3zcsgdoxq.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3ymliuedq.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3ayjkqoha.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3emfexyhr.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3jvnmjler.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3hruiqzvk.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3xtavymgs.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3kzitgotv.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3tgpwnovo.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3dxwaswlo.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3pfqkwcwe.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3mgvzdqzc.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3gdffkscd.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3mpffcjqr.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3haiftdur.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3uyqqsunn.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3csqvacza.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3fcymvhqj.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3wqcdcszf.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3lhxdysbf.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3ujozdbhn.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3lktpgohv.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3leetuwwg.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xfmkglcm.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3kcpixazb.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3zjydcyqh.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vindsjub.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3vuyixjxs.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3fsgblrbx.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3ndrpqzmd.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3czkphgea.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3swbvljge.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3qizqufei.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3dvdblebv.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3yzssruka.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xxyqknou.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3dzniyjsq.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3sqqychqs.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3oyoelndh.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3ucsdpebg.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3aplhwrxk.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3onlkbmpb.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3jnzpbakr.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3lztdgxuq.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3jbsdeyeo.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3mxajhyah.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3ydisthle.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3zfqjjazm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dgdfbluc.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3dtdrerox.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3flqjiqln.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3uhsjwgtr.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3mktehhqz.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3ftstrhom.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3qgpepxzz.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3vnaleisc.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3ybtydivf.html

);
来源：http://www.52xcode.cn/Article/details/gt3vayhavpo.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3hupeugcq.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3ytumfcsa.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3nibzlxux.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3hquwbnap.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3nxihutiz.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3mdiecumh.html

);
来源：http://www.52xcode.cn/Article/details/gt3civcymqz.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3vwcgensp.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ztipukah.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3kyrqtnvg.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3dtpbarqz.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3hfkysjbz.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3ptsfueuv.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3ikolbdhu.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3uyoiuobz.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3qxpwxnmp.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3cejnvnkh.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3aytysxab.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3iqkbtobi.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3iimedlrv.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3ggduwvtj.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3lfprztva.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ytavoilx.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3dfdwchiy.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3xcgmaeyb.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3vbalqeip.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3aqtrttei.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3ztqyejgb.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3whtbsywd.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3dnphhfds.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3ynygqzob.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3rnicaqqo.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3suukptfr.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3omdhxkdw.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3njmnanhk.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3yovfmpqs.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3iqexjpdg.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3gvjarsld.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3uqeucxkc.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ousfbafp.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3rdkmblre.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3xazbgesr.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3xnyfhzwh.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3nsikfzvx.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3rpzizncj.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3dmaiwceu.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3lpymosdr.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3ywpsuitz.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3ibmheulz.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3lsbzkoii.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3opakyyld.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3zznmfjul.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dgngirsz.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3vbtdcsbm.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3xfibjxfl.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3klfxrlui.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bydgclry.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3csposdph.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wthhovzs.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3djcgcsjq.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ckymzqst.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3wigmbmrv.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3chhgclxv.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3utbjqysd.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3hlbfehqe.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3gpeyviry.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3urpccfsv.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3mrtqofvk.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3dnwqgktu.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3syhfmkkm.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3qiwldnyi.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3lmukxqny.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3naoddnbg.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3fkwjoobq.html


<!-- 参考信息 -->