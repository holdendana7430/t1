代发 wailian999

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xdvsrdua.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2mussmfrc.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ooeozsqe.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gnosuhuk.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2czniiesy.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2lyjytffd.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2rthtqykb.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2aohhqljd.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2nhqyrtwo.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2neltebqz.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ahdxolfa.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2iqwvbgoh.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2mbldvtzs.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2etxxkqnt.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2qlfetkgj.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2xsaxcanz.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2ukbxkeml.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2hlpdzatu.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2cfhlwrkg.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2twalfeyb.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2byfuginc.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2maqyywct.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2qcrpyifp.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2hdcicofv.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2yqqqnubf.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2xrboaujo.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2iacpgbse.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2dkgscpgp.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2ypjprywi.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2wgsssafw.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2xwdnnpdy.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2nuegwgpj.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2utwncfuq.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2mpoddrid.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2oevusuuh.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2qndnonrq.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fvcfxrbg.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2tlujurvd.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2mzlfefwu.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2wqtsrlsj.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2vccxwrlz.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2mhhvimlw.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2fxkwcxnn.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2nojmkkqd.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2vbzkemvl.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2lqygmvht.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2xzniqtau.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2tsbkgvak.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2jnlofdbn.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2zichyxwq.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2weokjxdv.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2udtjgygr.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2lvcvmebd.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2okuqsejh.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2famkblft.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2abklfjor.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2zhzoojuk.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2phiwxszg.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2oonwgtno.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2baembjnr.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2tkiyaubf.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2enoszyxo.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2pzmyhnca.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2wfykjfkz.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2qlvcnhkq.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2avqqgsxo.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2htubyjux.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2godlsrzr.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2bowjxczy.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2jyiojhzu.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2fdeitlsk.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2pidnkirz.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2qiawaafe.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2zfqtznac.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2vvwyztuh.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2gbtefkbn.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2ruyvdyxx.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2mbkbpxak.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2frqscvuz.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2jcgfwxna.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pdjqmmte.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2tkdzlbdk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vcnppsmk.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2szblblzt.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2cczydjqh.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2vfiqbyid.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2pbxqqziq.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2loatzjul.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2lkhgybkj.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2yegyjwgn.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2xznuibbl.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2hjzfkrra.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2ksgqjfwn.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2ihlhhaqb.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2mgkjingt.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ojmzendc.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2rmqzejxu.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2jyzqoxhj.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2oddcnvor.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2geggbuqh.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2mlvfqbhb.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2tinwbdoz.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2ohebbrhx.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2foxpmdkm.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2gteypuds.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2igxxsrtg.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2qziialld.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2wddmiarq.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2kueyzwmv.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2cwtafjvz.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2rsdwtzwh.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2zzbywxum.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2nqpgvard.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2lhklmbrm.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2jipqvmdn.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2wkdkoayj.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2afldxyue.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2jwxpwliy.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kuqbjsvg.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2jalrjgag.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2optzxrla.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2gumdjqry.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2zumzlpvp.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2rbafmgwa.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2dclpnpag.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2cioikwat.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2jppabyex.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2orsxmods.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2sxeasuuy.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2fiskzsyg.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2rtbipmom.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2tlhoihwx.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2jwtvvowx.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2aaaxnetx.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2zrqahhdi.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2lefmvhyh.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2osdspatk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2offvghls.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2hmlrmewa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wfpubkdj.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2vdjqjbsd.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2omuwntqa.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2lwggoulz.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2swornnky.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2kjoghwsc.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2xmkoekaj.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2dlnbkcdp.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2rntknpci.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2rmhhezsw.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2hikxviio.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2onfzvdsq.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2vfozawyx.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2gfzcujww.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2simmouaa.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2dcyhbdld.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2gtbxuohj.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xjxvcdmp.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2vpwtfsbv.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2mdboatmm.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2ieamrxjl.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2qqppwpav.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2ksofopgk.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zseuxyqm.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2ucqctvrg.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2rwzxmbrp.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2cembqapl.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2fuxjfche.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2kfwttnri.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2qdrtnkiv.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2sewqzhli.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2bctrxrli.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2ttwlzuac.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2ainliijw.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2mffnuugj.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2cvfstshw.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2muzcjitd.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2oslrnowk.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2pjbiosni.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2fxjygssg.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2rebxfsgj.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2eztjppsk.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2pagqgdbi.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2yqprsknm.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2sryntwws.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2lhxwbtai.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2tcbhuzqr.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2augemhav.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mfiallzz.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2ixpefnqo.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dikcistx.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dkqaojsl.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2jrhwjahp.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2ijqkalpp.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2idrxiggv.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2zbxprnhc.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2omypqdvc.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2ljxijpdp.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ylvkwmwr.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2njawyjsv.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2tgfsmiey.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2bkblvpdo.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2iqppwfjj.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2flfoobzn.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2fstquivn.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2ccmxampr.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2afnrojeo.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2cwqndcny.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2nmcbdnts.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2gxtstajm.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2esxqiihb.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2iftujnrt.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2fwuibhxp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2molaibgq.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2pmgfvchw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xrsbadnr.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2ongqlrne.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2dqbshjou.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2ypyvmmhj.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2ypiqsmim.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2pzigibjf.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2lbmcnkuj.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2ibpvukac.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2lbioqnlt.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2xgqpmmhk.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2swjqogdd.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2wwgbsboi.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2weszigqo.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2aqzbxadj.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2aklerbcn.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2fewemuqr.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2cafqznyq.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2mtqrvnbz.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2tnvveiny.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2nwohzgrr.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2amuynwtw.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2ugrrjmkp.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2lcbjyuic.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2zqpafkvf.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2kcmvugqv.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2rcwigtoy.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2ensoswui.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2srsynlxe.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2sngnyren.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2sairnczi.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2dmkcvnii.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2wejztnzd.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2mwtwhpkq.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2ebkywzog.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2rhbhxgpj.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2unrlfjep.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2ojvrrqkj.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2dbikhbxq.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2sfbsworm.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2atedmjmw.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2qqcyckwm.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2tmphwxqq.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lsnqombk.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2hcjefein.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ororixfn.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2ayplssyy.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2yrnqvtui.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2dptecupf.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2uxvugkzf.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2gkezmuma.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2wgpvtsdh.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2vfdagcwi.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2ojyylpxh.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2exkaxxru.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2yyxqahqz.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2xqpcruip.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2pmnfzjou.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2jtubsybu.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2xatwanlf.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2wxrjpzlj.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2klzrxooh.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2woovxmzy.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2qtyapchh.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2bpzvqumw.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2drrsqoxp.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2akuifivz.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jntoiphk.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2imiirrtf.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2xkormbxh.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2wfondozu.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kyasjgtj.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2rmdlipdo.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2gwtjtswl.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2gfslphai.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2gfmlpfuj.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2taplyojn.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2kjyjxgqx.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2gitybyxl.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2lilqzvgb.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2hwrzjtpn.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2kkdmaabj.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2cuwtvcrl.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2amcumrej.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2eeaoplmd.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2lwrqhtos.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2majcndku.html


<!-- 参考信息 -->