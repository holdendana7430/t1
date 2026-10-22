代发 wailian999

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2klewzwqw.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2bxcomlad.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2khvlborh.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2qeoyocag.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2lujlgpxm.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2gudbouqh.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2pzsoytap.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2xhtszlhh.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2jeafskgm.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2nvnieflp.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gkgignnm.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2havkukuk.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2hjhlabew.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2lniqdsfk.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ludngoqq.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2tmxjmsim.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2ryeewbur.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2qkleyifn.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ujbnojfw.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2qkfgmllq.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2djyqnsfe.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2bbvkarss.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2mtjojvri.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2yfruxdjq.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2pxwkbkps.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2krmjkvon.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2jrtdcftj.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2fovndymn.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2fmpmuqyw.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2jnphyibh.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2kblalsiq.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2nrnfdxtn.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2idzvysdj.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2ttlpthkd.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2qxshvhgs.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2rgodxqwc.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2xogzbute.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2xlvqshgp.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2ygmzzowf.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2opehuyfx.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2dxovrcgv.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2smwdrbmk.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2mxpivmqy.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2pntdbosn.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2vsgdxurj.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2kgwemvid.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2zasgoiko.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ffeoiday.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2thhxkyvb.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2eujmjmia.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2hfnmxjac.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2qjhfprea.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2gvfrwgjm.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2mzwvbkmo.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2azvcvzaa.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2syabjhos.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2jizxeino.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2gnyjeawf.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2acmigcxu.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2dpvhldji.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2tjvfjktg.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2yzadjkgo.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2hecxknup.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2eoeaaxzr.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2whzlaige.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2mvnmscbh.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2vcjedjny.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2kzjzicoi.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2edndzpti.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2dqwjbxxr.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2zerewjox.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2lpfkochk.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2awcagiju.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2mjwnftjz.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2cqjoucfu.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2xwyfzpyj.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2qvocszfo.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2mtoymrdb.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2ahglycmt.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2vfrefjus.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2xjppozth.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2hohizaxy.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2qpauqdgd.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2kyxdmwty.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2yinpfzty.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2wycboiyf.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2htecbpyj.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2cpczvuaq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kscqtxbb.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2xneghdgb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ccltspls.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2lamcbdth.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2mzwmuput.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2aowlktwq.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2ueotdveo.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2eetkagdq.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2gdmgltaf.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2qpzxzsvx.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2jsxvagvn.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2lophkhzz.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2tnhxpsut.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2bmdamayu.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2tqpziknz.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ynwizsln.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2hkfqwbem.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2bsubpcse.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2robxfrrh.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2xqjkdcdr.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2nwywqhio.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2oigcocwu.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2kbbydgpy.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2iempkmtu.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2tqnnadyt.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2hheyncaf.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2rrbqlwnu.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2yrttlwnm.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2gsgagveh.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2gvkensfy.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2lllorkdc.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2fsxphvne.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2ugtncnom.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2gxcqoaza.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2bnrihgke.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2rupxabrf.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2sxrkbhlq.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2ofbmifxx.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fmskfukz.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2dwpllwdz.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2cltshhlr.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2eligiywq.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2jdjrkauo.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2lhstqyxl.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2hmyopcow.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2vdxsdmss.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2ofcjiung.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2glwkftht.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2ocizklaq.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2tntivasa.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2lypfdxcq.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2tfjvatxk.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2wwotiktx.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2qbsjuwfp.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2jhoetjqn.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2wrntkdod.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2uhhsnvzv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2szlauhax.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2dwsprbpg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2frvaojze.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2qwbnnhhb.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2tkahobmn.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2eikxtogn.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2bhhltefd.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2qesvwamq.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2vqjcszne.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2exujidar.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2bpzrgdfb.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2vpboyyok.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2dwbbeupz.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2rqqavnuk.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2sdamsbyd.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2wkecuvwa.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2ouxnjvfz.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2mdnqclem.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2cojkgwmk.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2baecnqmq.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2lyxchked.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2rvwzxkvs.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2virevlre.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2xubcwlly.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ncmsynby.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2spgfwgog.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2xvozlyou.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2rmtcaibi.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2taxeyuba.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2qtyfzypi.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2cznhosxj.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2cskbktqt.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2fgiotwow.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2vuqstfse.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2ncrklius.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2lycurxma.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2lqthwmym.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2fyjiewfw.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2rbncdlgw.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2yxnxxcuz.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2yvkwdknz.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2ojchkmxm.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2qodkfclc.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2mybowagf.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2ibkseneb.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2smrinkca.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2nrtpxout.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2okmwporr.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2oolixcev.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2filmjjjf.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2exhcoihe.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2cweaspkj.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2rlgadkjh.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2qogiokhk.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2qseonpdo.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2dzipnccb.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2albboxpt.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2uxsrlqyn.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2havjqmux.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2xezrkwka.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2pxbfjojk.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2kjvvxqol.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nzxzmuwy.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2kpgciwkw.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2quprvxma.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2dbgaofwt.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2ctyxwusq.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2djigcboa.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2swgansst.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2aatcunon.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2jrgklwmq.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2lukqbvbu.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2sanbmyre.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2fqooison.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2ahujhvdh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dfrzyszs.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2nzoervkz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rdmcwttn.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2vzckgqfd.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2wnailhrs.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2srebijph.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2jgignnau.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2bsjkjbmp.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2avkmvfhw.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2suysxoge.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2onqpmaop.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2epnyetmx.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2wzuylgoe.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2vpsfgutp.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2lvtsrbfr.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2xjbqzzyy.html

);
来源：http://www.52xcode.cn/Article/details/gt2ldyknuza.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2nluszlpo.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2tupaduuz.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2tyquutha.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2usyqdgsk.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2bzfimbur.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2fyowwgeq.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2hhrskxrr.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2rjwuheav.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2jfiaasas.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2prtxezaj.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2boqrxwoa.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2pzipwybi.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2gznenqni.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2ojmzxhtk.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2dfaevuyr.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2ddvtejhj.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2yhwsnteh.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2ziazomsm.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2tzjopkqd.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2uxzvwtwp.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2uughcmok.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2mgdcahiy.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2elgchagj.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2svjthimb.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2fngfdnvy.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2aehbdbxa.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2jgwrzion.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qgrsdcfc.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2fyamlabt.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2skmzvvtw.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2shvguvif.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2mteblkzg.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2korxumfg.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2fdhpbccq.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2gdbezmoa.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2wdxkyawx.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2zkfiybfl.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2jmqhsfaq.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2yuaeiktl.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2omtqauaa.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2sohtwfyo.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2mlcdrfeo.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2ixuofzxv.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2opxvtbzj.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2yhehjafh.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2msdqnlrt.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2xlkaqwgb.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2innsncut.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2bzdsbgqe.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tjqveupy.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2epizepso.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ogzntuxo.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2yrocmxob.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2pliaqzly.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2gqgizlyk.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fsjndabf.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2gbypmuoq.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2arxyfboh.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2hjutpocw.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2wrqyqkvf.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2kcdeefqv.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2sqmpovzs.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2hjkmfpra.html


<!-- 参考信息 -->