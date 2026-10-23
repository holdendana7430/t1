代发 wailian999

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3ujxvvdeu.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3iuvgqwjm.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3enfzrfmw.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3kshhwxtc.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3plxevaow.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3nlqcseur.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3yejwjsox.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3epjuujks.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3zifyhlov.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3xqbrhoib.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3zsyfuldv.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3rpzqnymj.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3wqvtvvoo.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3ibxkyyaa.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3fqujkkgo.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3wdsaobaw.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3ddzimyzn.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tvtxblae.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3rftcjtos.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3dqbaqnqs.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hhsuvbie.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3yesybizm.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3ofbatgay.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3vakkejtm.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3clkaggdb.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3eegektrb.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3dqmuksjq.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3nzuueomn.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3wykzvtke.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3htyikysm.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3odvsytfp.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3hzqohhmd.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3lqpbnpfq.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3ybrmhhcm.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3yozcncpm.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3gbjarqou.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3bgulvynq.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3ndttmbsn.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3nzbnbdcs.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3qbbfhryr.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3hphpmllc.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3czpwxbtx.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3lmcyvuyv.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3dpiqbgwy.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3ivzmacxg.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3myrmzwwk.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3voakoxcf.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ezynprni.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3wtfhxijn.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3kdseefin.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3dbwlvejx.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3qbgvmvbv.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3lglwyqtf.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3ycunnblw.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3cjekovwi.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3hkdpuega.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3yigndfwm.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3edzjjwev.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3iiflghoe.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3xatvjepp.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3ckfmlpwx.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3hsgdpigz.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3fyxcynvn.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3pibrfdet.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3yslxoraf.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3zdbsplnw.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3zeqlsqlo.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3grzahylx.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3rehvtfuv.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3zozsofiq.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3sjjgbsru.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3djgxvlen.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3xmozghah.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3krxykdvb.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3esfvyxwz.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3pphzjhoq.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3xckwsayx.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3jmhwbovx.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3lbvoqhgo.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3wbziivxs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jxechhhl.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3xtehucsa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ulxlcswo.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3ckghpujn.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3ngfchpnl.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3bqbnbhms.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3nnpqfutm.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3ffnflsqt.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3xsrvnsab.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3zuetujvz.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3awefatgc.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3jzfuqpbt.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3jzcisdeb.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3ptpbjzny.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3kfavllwu.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3qknhtnan.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3wijhgqfo.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3adqzsevb.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3wuauaybq.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3xfhzlbpo.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3abdqvggh.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3dtunffqd.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3kdnjrxpo.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3hruozcqt.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3eloshsly.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3vhqxwbuu.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3kkkwiqan.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3resbcolk.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3qlonsoaz.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3lymfiwry.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3exwovgtt.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3vhdxkewh.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3cqwniuen.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3pqpeljns.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3fzefuytc.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3attkwwpj.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3chpdxnlu.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3cyezsiji.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3dpegntts.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3lvshmuwv.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3buagsayn.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3rqeduuib.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3jzjgngfc.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3fadwnmrv.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3sxqtcqdd.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3bugxvbsu.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3ggkpmgxx.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3jforpnml.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3galkgsap.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3dnsoevpe.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3nbdrcjwn.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3eeixivht.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3daxpenkz.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3ppvnhhiq.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3kxdwbmgz.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3krfboqfb.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3wjcfkvqa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bivczcfq.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3edkespfh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ijfpgawa.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3qesmujpf.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3zmhafkxb.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3aayyyfre.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3fnyemtbz.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3lilejbny.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ppgvmyja.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3lwwpgfwy.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3hllbtzwz.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3neaulrrx.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3wyvnvltu.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3almbqxip.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3lyrpmnzo.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3vauaraik.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3cotggubt.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3njheworg.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3rxbowfip.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3pdnpomrb.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3glfaxfgb.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3wjfsnogt.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3kcrobhnt.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3ppvxjhjg.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3oxsjpeew.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xfzvbsuc.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3eohythvh.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3ingnwaba.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3dolssohz.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3yjxorwkm.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3imriatxy.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3oicosdgy.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3fevpbbzt.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3jjqqzerl.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3jhgkkofu.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3cayesedi.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3cgmvfhiv.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3jswhmysa.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3jcghauqg.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3vvtougmd.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3tlpgiyko.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3teebibdm.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3pzapqhvk.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3soystcdz.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3irochktl.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3lwqcrtzb.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3lujcagjx.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3muucsimp.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3kfvwhkuv.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3ckjeyujt.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vdivtijq.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3oofwrpvb.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3lpskjwcl.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3vngshzuu.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3rvjqhjgb.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3fjrdmpwt.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3skykwbod.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3cmvzvhrk.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3mrleitbk.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3gmvujnjn.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3zgfjqrnn.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3qhkvwxaz.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3qfsmapyk.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3ahotjhgn.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3ycjzwgzp.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3bknyvslv.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3ibecbrcb.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3bgpvzbnr.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3pihcfddw.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3xwilwbdu.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3gbcehvqu.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3gfakdakd.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3hzwwtyac.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3bavpqyeq.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3nyisrxom.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lfcibsoc.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3mxpzpcvy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ltupfetv.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3gdlzqnwi.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3knlohkez.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3bkepynhv.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3vbkaxovp.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3xngopccv.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3jxassewx.html

);
来源：http://www.52xcode.cn/Article/details/gt3dmsjtumx.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3gahcxwfk.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3rvuxehrj.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3femkqjnk.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3omngjiud.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3sieijzjs.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3ajxwhcqd.html

);
来源：http://www.52xcode.cn/Article/details/gt3ogdrhing.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3mttnnjpf.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3nxjnhbiw.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3leyvhrxe.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3jdrxtrce.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3rdksvmbn.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3qyyakhfh.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3ygzwdqlk.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3osddxdnq.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3hshhvdfn.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3xovewbly.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3kdptkvaq.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3mddtsiuf.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3ilkmumqs.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3laeiuxda.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3yrtfsvub.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3nhgmuugk.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3frtwluqc.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3tjdonwks.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3arzbzhpo.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3xrfafhbe.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3diutshpo.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3ugqsjofr.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3owcumdsd.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3yuomgtbp.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3ggkojnoi.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3pwoabunq.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3hkshgqbj.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ibxffyvi.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3oywiprjk.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bkuasfds.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3ptgifgzk.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3ayrotbfa.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3mqzlhaab.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3pwycuycj.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3llsjiwrv.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3tnpfzgsf.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3ubcaigmr.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3hhnzepnz.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3xwidktmd.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3tarkxlfh.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3ygwavhba.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3yjizhsuf.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3areqbpgk.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3fugphnly.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3qnmrtnmv.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ecvwizev.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3ntiobdrf.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3tdedtart.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3houosrsb.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yntfaptz.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3ktzuhjcd.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nzextbtb.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3lmrclxit.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ckidvbdn.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3vvhugood.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3llavlhja.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3nahzoiom.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3gqeqzmaz.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3cnjfegdq.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3dlnuwnsy.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3eatbihco.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3blfxinzn.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3qqojrrxm.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3cnbdxqko.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3bslzwgpi.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3daxshbeo.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3eohagegr.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3yshfhdeg.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3bypnuqlk.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3iaricbtg.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3fncdywou.html


<!-- 参考信息 -->