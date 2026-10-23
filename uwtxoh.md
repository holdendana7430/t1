代发 wailian999

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3gnooquul.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3obrotoml.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3ibtsdsqw.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3qfvydpwk.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tnxwfenl.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3jecprndn.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3rdxapnrb.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3qpfjrchc.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3xrltvdbs.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3zpwqmrea.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3ikhrtesx.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3nfafnutr.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3fofsrokc.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3qayknsxh.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3krvherzg.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3syijaqst.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3urtufpvv.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3fwcsglsv.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3umhplbrx.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3dnwowzvx.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3kgnmqofm.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nffjmhem.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3uftkuyst.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3jfkrhjqv.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3pxnbiomm.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3nnqjdfrl.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3ustasqfu.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3woiubveo.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3zzungvxn.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3lqdwdign.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3lspqjgks.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3cinczoru.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3gqrkqdlj.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3lfacsolj.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3dtkvfrxg.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3iinamuvh.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3xxxlitim.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3umloybju.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3rhtczyqv.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3ynzqbwnt.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3ygpztkge.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3wrmjvcut.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3qdeynrec.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3cqoixxxa.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3wgwrucgk.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3qxcmqbub.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3cjnkxvyg.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3vakzpshw.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3yzrmruxz.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3moftlqqb.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3wqaaxuiu.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3nbstwkog.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3qkoopwsd.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3yfawqktl.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3qgmizwao.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3njcusqtx.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3mjzrklhn.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3csezccip.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3wbpmhyyj.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3kezoukjr.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3suhaaqwy.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3cumwdhbw.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3pdgynoyk.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3ktwdsevh.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3qsgltnoa.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3whxmxnju.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3accrrrbu.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3xwcrjgnb.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3fpxvabht.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3mydfjtky.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3jlbknbum.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3skoajlzv.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3cpgqcdfl.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3ndwotlul.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3gmpovowh.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3hlkdbwrl.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3jkdykhrm.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3qtocctcj.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3noqkrhsg.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3uokygcgu.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3figbzndl.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3kbuvibnf.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3hvuoasgo.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3rknwhylk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ivpivmbl.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3kkckpaov.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fvwvguda.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3bikyjfkn.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3dlbcjslf.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3nnzczkpw.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3xlqeizub.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3wgyipgpe.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3pbqlzmbq.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3axszksks.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3cwatylaz.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3qrirszht.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3oedsipzp.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3cbldahyp.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3ugvjeesh.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3fqhwbtil.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3xpixbvvc.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3ekyudhec.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3tapyqrft.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3vubuhuud.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3tgmgquct.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3grmvvkhc.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3lwvrjkxi.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3gzftztgz.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3ppnzvyuz.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3lrkpdgtn.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3vyuiwcyv.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3jovlvxwo.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3xlhpfckc.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jlizefuj.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3ejgvpsvr.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3vqxtckfq.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3svsnkkcm.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3xaklegcj.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3robyuaqj.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3atgahavd.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3uckrcizo.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3smmgmbtr.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lofpjmex.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3mfsjhpxm.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3ojstykhd.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3drcrankr.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3nfuwxxri.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3pskcmfxe.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3yniqdotu.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3nsywcdsz.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3shoytpqk.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3odulnpnn.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3gpmldtcs.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3usypdljs.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3xzmqybqg.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3zofoawmm.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3nnxiaykt.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3kzrezdvh.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3eyntnlmc.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3lvyndxav.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3zjihkhhy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zbdqzwjk.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3wflltfat.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3njaxxqel.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3rghcwubf.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3mrzwxrwy.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3dqdxbmvp.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ylifuxtd.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3nigqywrk.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3hipscpkl.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3vqullnuw.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3argjoomk.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3zmnjkguh.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3kogjrhea.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3iownxjdw.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3zgjlregc.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3lbjoultg.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3wcamfqpt.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3shnotquk.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3ladynrnt.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3vsllkjcg.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3idlyphxw.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qdctdbec.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3olnaehut.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3veebjkzd.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3swjsiblb.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3clpqwzke.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3gdcavxvr.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3nxxphmai.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3bwhmcuwq.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3ppppwxya.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3ydnaxtla.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3cowuzqii.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3bqrihkwe.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3kefgvlkx.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3pyjvhsuk.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3sbivzfoy.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3nupjlfyb.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3wbssimny.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3wxnkofii.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3axrmffka.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3nowbtfra.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3zzmflglo.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3jsyevwja.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3tgbavasa.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3snlikmed.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3sawxdtrj.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3rzqwmnsr.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3ybzaqvcf.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3bynalgnl.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3reuechqg.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qxuteehe.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3hdjitsuu.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3tpbejbep.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3onazwzaa.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3ifqdmybb.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3eprwzhvx.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mawodrng.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3sixsounp.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3qilaufuf.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3dcnnwqeg.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3xbnahmcy.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ktxsgcqt.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qvgpbcvj.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3wrivkvkn.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3ophksfnx.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3fhbkbfhe.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3tmmjgzcz.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3fkeiohma.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3aklmobiu.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3tspetnjp.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3utjhbwhc.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3khiwyexc.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3mwhrasgs.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3ypltveys.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3hukbcwwm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iwwaywig.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3tbgovxdv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pnahcbyu.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3scbbhxja.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3kymybfyq.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3ftpgvpze.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3xwgzfwqy.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3odbswrzu.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3ofsmrtxb.html

);
来源：http://www.52xcode.cn/Article/details/gt3durtnwwu.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3ynfqnkrr.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3jeodfxuo.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3rewjyfhb.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3fuijcsqk.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3tlcmhjta.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3yrovzdvh.html

);
来源：http://www.52xcode.cn/Article/details/gt3bxsxptdi.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3owrhicwc.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3jwehhkyv.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3cylkfvjl.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3emaghhml.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3xlmpnshg.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3nyuvapyk.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3aexukphm.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3gtxnrumn.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3mhocqaym.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3ztqmdcua.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3uguqzwtb.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3bflqhbiu.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3sovddnri.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3idgirdzg.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3qqqlmahu.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3vmoudsin.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3ublsjacl.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3mlpbegpk.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3bofsukyr.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3jilwyeaz.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3ymsldlbl.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3bujtleay.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ekqkxhde.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3jdsntoqp.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3nsnkfdxl.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3tfylkrrq.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3kwrslhjl.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3usxlwxji.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3mzbsqqca.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tbbjcnvh.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3csydelhl.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3lrpkpfor.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3sqjpsvki.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3uzbibgln.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3dhcntgdd.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3mzbzpqyq.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3bqwvqscs.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3kgpukvnj.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3jiasmlwu.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3qzdludrw.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3aebzzgwy.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3jdemzazx.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3ubjsiand.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3dpbknbdv.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3vzlkschv.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ekqokopl.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3pwikdcba.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3ywhaulvg.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3sjzxaskf.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qwnkrkrd.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3idjzblsq.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rmlvgjkj.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3hmqnzpab.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3wxtdarwa.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3larkkuke.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ndsdrgkp.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3nyjqjqby.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3utcpfqbo.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3flonbhdx.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3mmbleqge.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3acqwxpvn.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3xykusxvy.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3hdufcjvl.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3gmydkqjq.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3gpjcqtlb.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3rtqfqmga.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3vcnelcyk.html


<!-- 参考信息 -->