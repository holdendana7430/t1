代发 wailian999

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2tuqpjjtv.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2fvepiyag.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2wnnaihmw.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2fgglahuq.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2uhwwoafb.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2iwqmbynz.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kfzewyho.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ewqapnuz.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2piztwwng.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2xidxcezq.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2tyyfdgza.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2olhfcyli.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2lwmyuzeo.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2ndkiyenz.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2tpvlxrvf.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2vzijowhw.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2vghmootn.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nqpdpbbq.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2djlewchi.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2aymwtoyu.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2nyulwejg.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2lulfdivg.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2okznrnlk.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2wqpveqqg.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2zgdemvcy.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2csucayxi.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2fajjqosb.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2fcocayau.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2yzsyqiwc.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2mjuwgmdh.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2mfekptpo.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2qiarffbj.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2spajcxkp.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2afduxmpa.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2oavwlvfc.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2kscyotwi.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2euejxlsa.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2bgwmpnno.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2wtjewxnx.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2zohtgtig.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2moqshhth.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2bdwnkzqq.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2buppzwez.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2bhrnfpfs.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2krtrvqmf.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2gmvohyqk.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2xgqgglkt.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2paiqplff.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2nicepckz.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2jfygoirx.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2jyfpwtfs.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2jnwnldez.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2dwopatzt.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2lqakacdv.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2arwptasy.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2oteltbgt.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2jxjgqhfc.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2rbyfaeab.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2gcbhvihd.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2ivcajgxh.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2msajezps.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2cbkwgyil.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2bkcugsly.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2hyzvfvvv.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2jdervjeh.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2gcjswlxe.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2kpreawuk.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2lqjmcxzc.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2aazvzvvs.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2kvotxzrg.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2fqklsopq.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2nwrkwbfa.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2mydlibgy.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2jhlwuanp.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2nkirkjqs.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2urmxofal.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2siuyolod.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2dqdzushw.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2zgbbqgek.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2rmmbdzbp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vjmujdov.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2xunwsqfg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eizgyhbr.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2uldmlqid.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2csnksrse.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2lrusoppu.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2wbtutjjk.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2wkgvlqia.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2jfedofvi.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2tsseusyf.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2ybfqlubi.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2vxdnkmwj.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2zoewieyd.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2mpfquxzh.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2zmfgbnjp.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2hjldcsgl.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ablxzgos.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2ijahiigm.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2blwlqezw.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2glxvtkis.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2zrraemlv.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2ukgooalr.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2wsxpcjfx.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2fuisykrx.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2znbwhmuz.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2kkxbwqjs.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2vkmkpgwi.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2nfdrdzcc.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2ucuqjfoj.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2zyvvfpry.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2abcelfbc.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2gnowdiwm.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2hyvehser.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2eyjvidaa.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2yborrfqi.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2rrecefur.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2fcozghrx.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2noumhkws.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hrxilzkc.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2kbuprfhx.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2zctcgbem.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2vaebzjmr.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2toabauhr.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2gpyifrrb.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2htossqiy.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2ltfgtady.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2mqvbqfkg.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2zgyroqbv.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2ykdpdkfj.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2cdolgmeq.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2oxjktmco.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2hibnjqxs.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2ewuyazeo.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2imxogjwh.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2pahyenvq.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2czpkizdx.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2rjrnasdj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2etadbokl.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2ezhqpqjn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2upsbkruj.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2hyxfdbtv.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2lsgvjslu.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2bqclxdae.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2uqcgrncy.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2plhtycmj.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2qxsqjjgd.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ipoysotn.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2vpcwzcih.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2covuksuc.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2skvykvrw.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2lpimwlbv.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2yuciwgya.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2wnfmrqdj.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2ltgrdbkx.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2bemuctqb.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2hgioqfvm.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2akdaxosa.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2huabbvch.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2zowkotjy.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2qxggqoyz.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2fqebsmrm.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2dlhrwskd.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2afwfepbd.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2ezzbdbfx.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2moenepyt.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2bmtwmyqj.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2iflvgzow.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2eafjowyf.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2rddyghrx.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2rwajuout.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2qiboblic.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2jxkylyiw.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2pdbpkydh.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2drqpnwmn.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2qlxvaiva.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2bfswczin.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2yjariobw.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2fdlznoym.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2yqovjcag.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2rwgpmuhj.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2czelvzzh.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2flpwiisf.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2dxaoxiwo.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2mecoxygb.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2jlxzcovq.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2mhqdjoff.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2lfxrooos.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2mmkwikda.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2xcbckeny.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cfrauabt.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2liftqham.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2frunrlqp.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2pjakvtzx.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2dseoygyh.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2pbxghgzu.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2fonkraih.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2etgqzasy.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2fdrnlopg.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2wilfttxo.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2klghqxan.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2lsekhhdb.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2ekhwvaov.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2gfxuxnem.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2xpnqrwhe.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2mjjidmmw.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2csmeeeeq.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2nytdfbov.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2nrvoyjmg.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2hizitifo.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2aqdjmpoq.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2dolhihuh.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2edfubgpe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oavbsqka.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2aefetjcr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2emrmfhqy.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2tpusbfkv.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2okkkbanj.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2kilzfzzy.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2nssvdnle.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2qzcumvyj.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2kwsbzfbm.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2dpomigey.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2fwgrdcae.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2lmdvvaqm.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2hjtaigqs.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2dkgtrrbr.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2yrtmrghc.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2bmustsun.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2xzydkwmq.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2bjmzilsz.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2ewvwizfz.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2jhcvxiis.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2takasods.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2uwxjpxjd.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2smfztroc.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2smspnuhi.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2mcnpbjvo.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2yjdrvuzn.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2catdxaxw.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2zgnmegkz.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2dppgvsyj.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2cevgycpz.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2ksmvkjln.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2zsanseyr.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2wneqfdhk.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2iwkjvhde.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2wxnstvre.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2aknxytkz.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2mbhdsass.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2mtkbxtih.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2pmqbicgd.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2omzkuxdq.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2ilnksvuo.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2szftpxxg.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2bgnzqidm.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2esvhdavk.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rqkuetqk.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2nmyzfxwu.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kcxtqcqn.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2ntnrtuiw.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ykazmrvt.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2drctggxz.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2osfjenpm.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2pfflctii.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2ugeoyexx.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2auebudik.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2odyohlyu.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2jmlmznyy.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2tqjugvrb.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2voejcrxf.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2taozyojf.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2nbohgxrp.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2qxvofhph.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2ssafgaju.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2sljsjfdu.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2fgwkbryx.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2dtoszmqw.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2ulnsdtau.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zrdhkszo.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2ggowhezq.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tdyxgshv.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2xiigndbg.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2obgofgwl.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2nycmasfi.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vbnqnvrv.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2ohvrclri.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2vijghdwg.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2pbwqjodd.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2wsdyybec.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2twtpbyzs.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2zwdoseaj.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2dlicxexy.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2kktxjqio.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2mpyyckgw.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2lqmxhqrm.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2krncavbb.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2nrdovltt.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2vuietamg.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2rsiozblc.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2imvyzuje.html


<!-- 参考信息 -->