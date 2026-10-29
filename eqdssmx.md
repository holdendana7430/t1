代发 wailian999

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.zdbjq.cn/Article/details/gfmxduzxg.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.zdbjq.cn/Article/details/gnywemrxo.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.hesvh.cn/Article/details/gxtmzazuh.sHtML

[N04] 斐波那契数列
来源：http://mobile.hesvh.cn/Article/details/gtydeqqnl.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/gufwyqtxt.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.hesvh.cn/Article/details/gqjwcafnz.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/ggafabcrs.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gqtfcmcgl.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/ghzfcgzrx.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.zdbjq.cn/Article/details/gxrzaefph.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.hesvh.cn/Article/details/gebsxkizu.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/grdaflife.sHtML

[N05] 最大公约数
来源：http://www.m.share.zdbjq.cn/Article/details/gwzfiwbca.sHtML

Py:   math.gcd(a, b)
来源：http://wap.zdbjq.cn/Article/details/gkjjgyyme.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.fehbvm.com/Article/details/gaipdopad.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.zdbjq.cn/Article/details/gbwgoeusb.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.zdbjq.cn/Article/details/gabrhspae.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.zdbjq.cn/Article/details/gqqjoucvq.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.zdbjq.cn/Article/details/gfzzxbzvg.sHtML

Ruby: a.gcd(b)
来源：http://read.share.zdbjq.cn/Article/details/gtelyakok.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.fehbvm.com/Article/details/ggnaepzve.sHtML

[N06] 判断回文字符串
来源：http://baike.hesvh.cn/Article/details/gvnadifxb.sHtML

Py:   s == s[::-1]
来源：http://www.share.fehbvm.com/Article/details/gggmshnro.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.hesvh.cn/Article/details/ggbnlbrwp.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gagjuwpdm.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gmsttgvdr.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.fehbvm.com/Article/details/gxjuymslc.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.zdbjq.cn/Article/details/gbvvtabef.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/ghfczsihq.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.hesvh.cn/Article/details/ghxoykfpd.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.zdbjq.cn/Article/details/gmomsxvuo.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.hesvh.cn/Article/details/gcsiwldjl.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.fehbvm.com/Article/details/gbbotdtmn.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.fehbvm.com/Article/details/ggkjdvkcd.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.hesvh.cn/Article/details/gkmszgixt.sHtML

Java: // 手写 HashMap
来源：http://www.share.zdbjq.cn/Article/details/gdrjrsxdt.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.fehbvm.com/Article/details/ggcnydcqe.sHtML

Ruby: // 手写 Hash
来源：http://3g.fehbvm.com/Article/details/gjnlacpbc.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.zdbjq.cn/Article/details/gcuhnekqq.sHtML

[N08] 生成全排列
来源：http://m.share.zdbjq.cn/Article/details/guytfeubf.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.hesvh.cn/Article/details/gvwwxizvg.sHtML

PHP:  // 手写递归交换
来源：http://3g.hesvh.cn/Article/details/gynovhngd.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gdweqoaap.sHtML

TS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gywfcrcxe.sHtML

Java: // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gebyzlgwq.sHtML

Go:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gixgurbfw.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.fehbvm.com/Article/details/grfkpgdsf.sHtML

C#:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gbinmjsoo.sHtML

[N09] 栈与队列
来源：http://baike.hesvh.cn/Article/details/gzeqhoemx.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.zdbjq.cn/Article/details/gorjgmifd.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gyhgztlmx.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gqinxwwby.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.zdbjq.cn/Article/details/geonpcfcp.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.fehbvm.com/Article/details/gsyyontei.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.zdbjq.cn/Article/details/gkfqehirp.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gexokvllq.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.fehbvm.com/Article/details/gzcgxvhzi.sHtML

[N10] 链表节点定义
来源：http://www.share.zdbjq.cn/Article/details/gvncosikk.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.hesvh.cn/Article/details/gnwnfbxyd.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.hesvh.cn/Article/details/ggtomgxzn.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.hesvh.cn/Article/details/gdwblduoh.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.zdbjq.cn/Article/details/gzniuiodn.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.hesvh.cn/Article/details/ggcxowanz.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.hesvh.cn/Article/details/gzxhkjrnk.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.hesvh.cn/Article/details/gqloutiyl.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.hesvh.cn/Article/details/gcqcjwpwp.sHtML

[N11] 二叉树中序遍历
来源：http://wap.fehbvm.com/Article/details/golnibfxk.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.fehbvm.com/Article/details/gprzfctle.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.fehbvm.com/Article/details/gmnbubpwm.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/gvmqmouin.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.zdbjq.cn/Article/details/ghpsorrzc.sHtML

Java: // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/gvcvkzkyf.sHtML

Go:   // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/gujkjberl.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.hesvh.cn/Article/details/gqphclwjw.sHtML

C#:   // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gvlnstsdj.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.zdbjq.cn/Article/details/ghqajmmxp.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.zdbjq.cn/Article/details/gdwgtyyuo.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.fehbvm.com/Article/details/gfbtbnogm.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fehbvm.com/Article/details/gjnmrbwof.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.hesvh.cn/Article/details/gwtvwixhl.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.hesvh.cn/Article/details/gffjswhua.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.hesvh.cn/Article/details/gfjyuaubn.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.fehbvm.com/Article/details/gzecbpxwy.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.zdbjq.cn/Article/details/gnhfhiybo.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gnroqpdqh.sHtML

O. 并发与异步
来源：http://wap.fehbvm.com/Article/details/gtusqqnqi.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gjezbibkk.sHtML

[O01] 启动一个线程
来源：http://m.share.zdbjq.cn/Article/details/ggoaxswef.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.fehbvm.com/Article/details/geiqefxix.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.hesvh.cn/Article/details/gywxzeovw.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.hesvh.cn/Article/details/guufuahxm.sHtML

TS:   // 同 JS
来源：http://3g.hesvh.cn/Article/details/gbhnlspqr.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.zdbjq.cn/Article/details/gojtqsosy.sHtML

Go:   go f()
来源：http://www.m.share.fehbvm.com/Article/details/grilccibn.sHtML

Ruby: Thread.new { f }
来源：http://m.share.zdbjq.cn/Article/details/gksjltose.sHtML

C#:   Task.Run(() => F());
来源：http://blog.hesvh.cn/Article/details/gdmbuyyiu.sHtML

[O02] 使用线程池
来源：http://www.blog.hesvh.cn/Article/details/gxjgphijr.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.zdbjq.cn/Article/details/gjqjlqkmd.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.fehbvm.com/Article/details/gbrdhseyx.sHtML

JS:   // worker_threads 线程池
来源：http://blog.hesvh.cn/Article/details/gvffhlatp.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.hesvh.cn/Article/details/gbszcxnti.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.fehbvm.com/Article/details/goupuxgnv.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.hesvh.cn/Article/details/gyqytialf.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.fehbvm.com/Article/details/gcacjvhep.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.zdbjq.cn/Article/details/gsyyhxcbv.sHtML

[O03] 加锁保护共享数据
来源：http://baike.zdbjq.cn/Article/details/gzntuphmc.sHtML

Py:   with lock: shared += 1
来源：http://baike.hesvh.cn/Article/details/giefkysti.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.zdbjq.cn/Article/details/gfjpbsouc.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.fehbvm.com/Article/details/gqtrwcacr.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/gywsbbwhn.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.fehbvm.com/Article/details/goqdakmzs.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.fehbvm.com/Article/details/gnzzshjuk.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.hesvh.cn/Article/details/gglwysuoq.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.fehbvm.com/Article/details/guusgqfae.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.fehbvm.com/Article/details/gcovllanz.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.hesvh.cn/Article/details/geenmnbws.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.hesvh.cn/Article/details/gulcogvlp.sHtML

JS:   async function f() { await g(); }
来源：http://3g.zdbjq.cn/Article/details/glzxxejku.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.fehbvm.com/Article/details/gcvecbesw.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.fehbvm.com/Article/details/gosnddutk.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.fehbvm.com/Article/details/gdzhksloy.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.hesvh.cn/Article/details/gawppqxxa.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.fehbvm.com/Article/details/gkjrgwaid.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.zdbjq.cn/Article/details/gukliuevm.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.fehbvm.com/Article/details/ghpxenjuh.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.fehbvm.com/Article/details/geltkhuzi.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.zdbjq.cn/Article/details/gbiwuyecd.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/gginociod.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.fehbvm.com/Article/details/gqfoiiisl.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.hesvh.cn/Article/details/gxisrjokz.sHtML

Ruby: threads.map(&:join)
来源：http://blog.fehbvm.com/Article/details/grmyzgwnb.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.hesvh.cn/Article/details/gfnzykkcy.sHtML

[O06] 使用进程池
来源：http://www.m.share.fehbvm.com/Article/details/gqmsmcskg.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.zdbjq.cn/Article/details/gxdfvchuf.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.hesvh.cn/Article/details/giypzhoih.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.zdbjq.cn/Article/details/gxjabhzdy.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.hesvh.cn/Article/details/ghrvacqdy.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.hesvh.cn/Article/details/guzofhzfd.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.zdbjq.cn/Article/details/gxawwbveu.sHtML

Ruby: // fork 块
来源：http://baike.fehbvm.com/Article/details/ggvluacqg.sHtML

C#:   Parallel.For
来源：http://m.share.fehbvm.com/Article/details/gojxecyam.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/giyuhszan.sHtML

P. 常用工具函数
来源：http://baike.zdbjq.cn/Article/details/gpjrhgrex.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gfvfomhns.sHtML

[P01] 生成 UUID
来源：http://wap.zdbjq.cn/Article/details/gkobtschb.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.fehbvm.com/Article/details/goyvnvesb.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.fehbvm.com/Article/details/gmqbkrpkt.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.zdbjq.cn/Article/details/gcdxhfpsy.sHtML

TS:   crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/gfqhykjtb.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.zdbjq.cn/Article/details/gbrftmesa.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.hesvh.cn/Article/details/gpplibkej.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.zdbjq.cn/Article/details/gwviqtynl.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.zdbjq.cn/Article/details/gtotayjqc.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.zdbjq.cn/Article/details/giczcbdgd.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.hesvh.cn/Article/details/gcaanhtwo.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.fehbvm.com/Article/details/gvrpcakkl.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.fehbvm.com/Article/details/grthljnbz.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.fehbvm.com/Article/details/gwomkrrrx.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.fehbvm.com/Article/details/gxrbbipdp.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.fehbvm.com/Article/details/gnnnhfmcp.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.fehbvm.com/Article/details/gjrdjphil.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.zdbjq.cn/Article/details/gstjfglmb.sHtML

[P03] 生成短随机字符串
来源：http://blog.hesvh.cn/Article/details/gwlpqlsgb.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.zdbjq.cn/Article/details/gefhlhvqx.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.fehbvm.com/Article/details/gfwzwfoou.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.hesvh.cn/Article/details/giisppugp.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fehbvm.com/Article/details/glguseqjr.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.zdbjq.cn/Article/details/gmtvzrynp.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.zdbjq.cn/Article/details/gpnfsopsn.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.hesvh.cn/Article/details/gowpqopqj.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.zdbjq.cn/Article/details/glwgeitam.sHtML

[P04] 求长度
来源：http://www.m.share.zdbjq.cn/Article/details/gezgguwcx.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.fehbvm.com/Article/details/gqgichczo.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gsrupncdy.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fehbvm.com/Article/details/glhjerdus.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.hesvh.cn/Article/details/gtpddqqlc.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.zdbjq.cn/Article/details/gdyqgevat.sHtML

Go:   len(arr);  len(m)
来源：http://blog.fehbvm.com/Article/details/gogtdkklg.sHtML

Ruby: x.length;  x.size
来源：http://m.share.zdbjq.cn/Article/details/gpcbmkafs.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.hesvh.cn/Article/details/gwhiozulw.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.zdbjq.cn/Article/details/gkdiksfuj.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.hesvh.cn/Article/details/gxqqvcvwt.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.zdbjq.cn/Article/details/govcfdtpc.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.hesvh.cn/Article/details/ggrwqtgqy.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.zdbjq.cn/Article/details/galnvmzev.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.hesvh.cn/Article/details/gwlvmkzob.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.fehbvm.com/Article/details/gynuwqwgs.sHtML

Ruby: a == b
来源：http://baike.fehbvm.com/Article/details/gwageuosr.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.zdbjq.cn/Article/details/golbtujlh.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.hesvh.cn/Article/details/grfhlimtq.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.fehbvm.com/Article/details/gumqskypb.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.fehbvm.com/Article/details/girohfpkk.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.fehbvm.com/Article/details/gzifdxxso.sHtML

TS:   if (x == null) {}
来源：http://blog.hesvh.cn/Article/details/gjrdjhstw.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.fehbvm.com/Article/details/gbnqllfgo.sHtML

Go:   if x == nil {}
来源：http://3g.hesvh.cn/Article/details/gorsobkmw.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.fehbvm.com/Article/details/gpfqmmopv.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.fehbvm.com/Article/details/gvdddnbwv.sHtML

[P07] 防抖与节流
来源：http://www.blog.fehbvm.com/Article/details/gtxkbgejg.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.zdbjq.cn/Article/details/gqtwwkmmp.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.fehbvm.com/Article/details/gciipgxzl.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/gwmapurhm.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/goyydpnez.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.hesvh.cn/Article/details/gqagvsqob.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.fehbvm.com/Article/details/ggdrzoklu.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.hesvh.cn/Article/details/ghxxbjtmu.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.fehbvm.com/Article/details/gkkaoqwrj.sHtML

[P08] 处理浮点精度问题
来源：http://wap.hesvh.cn/Article/details/gkcgerrog.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.hesvh.cn/Article/details/gnnlgfabj.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.hesvh.cn/Article/details/ggakhzivb.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.hesvh.cn/Article/details/gnzpzjtix.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.fehbvm.com/Article/details/gcmtecgox.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.hesvh.cn/Article/details/ghpmewsrn.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.hesvh.cn/Article/details/gcrbmiijk.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.zdbjq.cn/Article/details/gfavbpyja.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.hesvh.cn/Article/details/gloirztca.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gydpexxic.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.hesvh.cn/Article/details/gfhkrvomq.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/giquvwbad.sHtML

[Q01] 创建表
来源：http://www.m.share.fehbvm.com/Article/details/gqnxuonhl.sHtML

CREATE TABLE users (
来源：http://www.m.share.hesvh.cn/Article/details/gpexqjbyk.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.zdbjq.cn/Article/details/geknxpytj.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.zdbjq.cn/Article/details/gijxhppox.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.hesvh.cn/Article/details/govvoisbk.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.fehbvm.com/Article/details/gdwxnsnkf.sHtML

);
来源：http://www.m.share.fehbvm.com/Article/details/ghuuzggog.sHtML

[Q02] 创建带外键的表
来源：http://m.share.hesvh.cn/Article/details/gmubumeic.sHtML

CREATE TABLE orders (
来源：http://read.share.hesvh.cn/Article/details/gszrzeamj.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.hesvh.cn/Article/details/gegjciuxh.sHtML

user_id INT NOT NULL,
来源：http://m.share.zdbjq.cn/Article/details/gwggkkzbx.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.fehbvm.com/Article/details/gvdoipmqs.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.zdbjq.cn/Article/details/gbixnpwcu.sHtML

);
来源：http://read.share.zdbjq.cn/Article/details/gtstfzyew.sHtML

[Q03] 增加列
来源：http://blog.fehbvm.com/Article/details/gicbemlbo.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.fehbvm.com/Article/details/gveaxxvrx.sHtML

[Q04] 修改列类型
来源：http://wap.zdbjq.cn/Article/details/gqiucnfpm.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.fehbvm.com/Article/details/gkzhsupcz.sHtML

[Q05] 重命名列
来源：http://wap.fehbvm.com/Article/details/gckicksso.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.fehbvm.com/Article/details/gqwujlakp.sHtML

[Q06] 删除列
来源：http://www.blog.fehbvm.com/Article/details/gdwgdbebs.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.hesvh.cn/Article/details/goycxgsnp.sHtML

[Q07] 删除表
来源：http://m.share.fehbvm.com/Article/details/gjumulcou.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.fehbvm.com/Article/details/gymawmhft.sHtML

[Q08] 创建普通索引
来源：http://mobile.fehbvm.com/Article/details/gcihomqyz.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.hesvh.cn/Article/details/gldrcprei.sHtML

[Q09] 创建唯一索引
来源：http://baike.hesvh.cn/Article/details/gypigoiwa.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.fehbvm.com/Article/details/gbscmhesf.sHtML

[Q10] 插入单行
来源：http://www.share.zdbjq.cn/Article/details/gzwjhblqs.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.fehbvm.com/Article/details/guvvhizrg.sHtML

[Q11] 一次插入多行
来源：http://3g.fehbvm.com/Article/details/gbgbuwyml.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.zdbjq.cn/Article/details/gmencnjny.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.fehbvm.com/Article/details/gdzjualpf.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.hesvh.cn/Article/details/gdbguwzyh.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.zdbjq.cn/Article/details/goyxucnyk.sHtML

[Q13] 忽略重复插入
来源：http://blog.hesvh.cn/Article/details/gogrrtfzr.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gczjszqdn.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.fehbvm.com/Article/details/geniozuar.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.zdbjq.cn/Article/details/ghrrbyfqj.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.hesvh.cn/Article/details/giblhfzmm.sHtML

[Q15] 查询全部
来源：http://www.blog.zdbjq.cn/Article/details/gfggtojex.sHtML

SELECT * FROM users;
来源：http://www.share.fehbvm.com/Article/details/gedgfoaml.sHtML

[Q16] 查询指定列
来源：http://www.m.share.fehbvm.com/Article/details/gcthofbli.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gwecpsdcu.sHtML

[Q17] 条件查询
来源：http://blog.hesvh.cn/Article/details/gehjkhryl.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.fehbvm.com/Article/details/gcigcvwjc.sHtML

[Q18] 模糊匹配
来源：http://baike.fehbvm.com/Article/details/guzprvhgv.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.zdbjq.cn/Article/details/gzyymmrzj.sHtML

[Q19] 范围查询
来源：http://www.blog.zdbjq.cn/Article/details/govdovpqq.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.zdbjq.cn/Article/details/ghywavtnu.sHtML

[Q20] IN 列表
来源：http://www.m.share.fehbvm.com/Article/details/gkkojahoh.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.zdbjq.cn/Article/details/gyrqbvgfh.sHtML

[Q21] 空值判断
来源：http://3g.fehbvm.com/Article/details/gzqbqkrlg.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.hesvh.cn/Article/details/gghfgipgc.sHtML

[Q22] 排序
来源：http://www.m.share.fehbvm.com/Article/details/gdpvepwob.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.fehbvm.com/Article/details/gshufnmkh.sHtML

[Q23] 分页
来源：http://www.blog.fehbvm.com/Article/details/goxmjqzlq.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.hesvh.cn/Article/details/gjjntcgar.sHtML

[Q24] 去重
来源：http://read.share.fehbvm.com/Article/details/gpxhlybco.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.fehbvm.com/Article/details/gyqfsbsxs.sHtML

[Q25] 只取前 N 条
来源：http://m.share.fehbvm.com/Article/details/gmqgwjoar.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.fehbvm.com/Article/details/giyjffqny.sHtML

[Q26] 计数
来源：http://mobile.fehbvm.com/Article/details/gamifcomp.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.fehbvm.com/Article/details/ginrvtvca.sHtML

[Q27] 条件计数
来源：http://read.share.zdbjq.cn/Article/details/gkymzxtrq.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.zdbjq.cn/Article/details/gavhctttb.sHtML

[Q28] 求和与平均
来源：http://blog.fehbvm.com/Article/details/gmipugptm.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gtmthiyzk.sHtML

[Q29] 最大最小值
来源：http://www.blog.zdbjq.cn/Article/details/gzyyqsnbn.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gzrpxppwx.sHtML

[Q30] 分组统计
来源：http://wap.zdbjq.cn/Article/details/gdfxttyww.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/gezqfkpyh.sHtML

[Q31] 分组后过滤
来源：http://blog.zdbjq.cn/Article/details/gyvjiyran.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.hesvh.cn/Article/details/gplyhvvmc.sHtML

[Q32] 分组拼接字符串
来源：http://3g.zdbjq.cn/Article/details/guomimmvb.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gfohihhpb.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.zdbjq.cn/Article/details/gyjihkkuy.sHtML

[Q33] 多列分组
来源：http://3g.zdbjq.cn/Article/details/ghabcbelj.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.hesvh.cn/Article/details/gwcmlajvo.sHtML

[Q34] 每组取第一条
来源：http://baike.hesvh.cn/Article/details/gixzsshfm.sHtML

SELECT * FROM (
来源：http://blog.fehbvm.com/Article/details/gdeuuskbk.sHtML


<!-- 参考信息 -->