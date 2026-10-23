代发 wailian999

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3fzrxiryf.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3osithcty.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3zwgurnwt.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3xzuuzpru.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3ieglnvmt.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3xreggpov.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3fhsutdll.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3llcrcdgz.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3yyviuccj.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3crbylptd.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3ndvewmnz.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3lebbcokl.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mkzfbfcb.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3igfvgdco.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3pmhocbtp.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3zmqepsru.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3qtclrkcj.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3bezapaix.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3dlnzpety.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3refgiply.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3opbkwqcm.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3sccruxqc.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3gzdctbmt.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3czpeqjao.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ujqnyxpl.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3tsvawihx.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3hhrcdoxa.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3npkwvjke.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3ndinrvah.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rdkcuaqv.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3rfxjbrtm.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ipvhzhju.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rdbmtlsj.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3skgdphna.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3sxoximtn.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3wljoluaz.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3imbnzvvr.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3akbyozwg.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3wnkaddbn.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3lrqhbapm.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3hlkuqjss.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3snbxtvsj.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3lckxvhhf.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3hlvkohen.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3mkmraheh.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3ooqvpnos.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3ubbnkxpk.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3svxmtntt.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tfiafpre.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3jxylalkj.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3syoeivep.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3cuyajvnk.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3paflnfwv.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3qjrpxeko.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3ztttcobl.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3dwnmdniu.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3xjcznhuv.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3dihebqgg.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3wuubxrte.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ibuontyz.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3pgiejwkc.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3hfmmertn.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3zywaascz.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3vuesjnfk.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3jyftbtgp.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3dlkdffzw.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3dznlobnd.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3pvlyqofh.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3kcderepb.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3khibndgs.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3nwxyxqit.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3fzfrstzm.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3owniylvs.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3yzujdnir.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3bffgortz.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3unvqljxz.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3dcbbimnb.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3cyjlceml.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3bcaleqjl.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3cfffndpt.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ywgsarlc.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3bryuravt.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ladcmlfy.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3juaaektq.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3vugrbnse.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3hqtnfhgg.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3uwzsxclx.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3lwnnoirj.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3qsjcpfox.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3iidxsapc.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3amzsrwfr.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3kcctifhm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ijlqumfy.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3tcqftpco.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ecmnctlo.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3cmhwjgxm.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3pmihrzgv.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3xxivpxtc.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3tmjfwaye.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3hucixxth.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3ujnixwbn.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3brdgpnbz.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3dehghsfz.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3uxfjmmid.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3eqzjsczk.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3dgaadbrs.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3mzxmxmfa.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3tfmafsdj.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3ustcxgvq.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3afuzktql.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3mkfmnovq.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3hcmrhnyu.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3hwqqynxr.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3jchnkspf.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3pqxpdimo.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3qoidfhvn.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3bmkanbhx.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3exiyvvfo.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3msnrfgzy.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3wqhflwaz.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3llkmnyvd.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3rszdtkyb.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3rzkckeyr.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3bmicolnv.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3lpgyjfjz.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3xlgzostz.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3emeikmpb.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3xoovecrf.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3yllmimhp.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3tvnvgtwc.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cfepuwnu.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3axuxpmgq.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3zvxdgynj.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3ztfqzgqh.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3eirfeogk.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3cajbfqhg.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3zarhzlmm.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3ptmtfoif.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3fyfsiffb.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3iqccfbxi.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3wabuehsy.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3qrzrfxxl.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3dlynlcdl.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3xtqiahen.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3adbugruc.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3pqzsbgrh.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3dlrfnmmr.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3kjvlxruw.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3gtntnqey.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lfffjwlq.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3unmnjfro.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3afnohwng.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3wzvtzenu.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3hqrtphdd.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3afishkor.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3vvdbmbsr.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3hqcivufg.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3tdvjonqq.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3lehnkita.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3rfrjljus.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3mvdkizvm.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3eumencss.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3xhbeokqv.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3ykuociiu.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3mzvhhaot.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3igscgdsw.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3bwhwbklj.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3rntjbfpt.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fldnynsd.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3ohaujsoc.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3dunzsxro.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3hsitqymy.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3mobqemxo.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3wppxgdat.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3pyabhgxw.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3rmvpizwu.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3rfelsrgt.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3yffkxwrb.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3zmcwlyeb.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3rdtonukq.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3orrcewfa.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3blkyveje.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3wmlyfwsf.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3gxvfyfqk.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3nvwcculv.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3mckgmtol.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3rchbfjpc.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3bdwroenr.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3slvhgvfj.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3euaefotq.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3wctuvzaf.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3qdkviisl.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3jcrsawra.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3itxmwtlf.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ladtwutr.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3miifebpu.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3bqmmasen.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3igovqglv.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3dvbsuema.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3utacehaq.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3jonubeou.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xdgfvhew.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3qlmqumpo.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3wcfpnczk.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3tebnmznu.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yzpjzvbj.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3pgrqncna.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3cgntjsjb.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3jvitppuf.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3lihsuupd.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3xohhjlrg.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3qussbjlu.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3zcpakwdw.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3xizsoteb.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3lhorgfsi.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3kyuqwnmd.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3zpfnafdi.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3lajagywv.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3ztonrneq.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3snznlota.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3wjrpxnwj.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3tpnhifwr.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3krlzzizj.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3pqevgpxi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qipibvry.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3lephvkux.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3klcewvit.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3kbuafxnt.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3kjaxcnjr.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3hayvtehb.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3zefmcsjg.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3lqtxkgbk.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3rvydjjhh.html

);
来源：http://www.52xcode.cn/Article/details/gt3imzmffff.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3nlxwoszm.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3aatavztc.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3miwjpirp.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3itoecajn.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3snehvkfy.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3xtwmfdpa.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3rczwhxmi.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3zckoixkb.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3iyyaueuq.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3ixhpkylk.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3lssiairb.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3zfpimmtx.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3zzjtnhme.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3cpgggwbv.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3rjayvzka.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3uununlvg.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wzgxujfp.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3lhpzqbxf.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3lstgoriu.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3lpplaucw.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3kewxtsim.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3jncjoicg.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3rvqkiqmc.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3swjjnpuq.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3dckuhyef.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3ftryqnos.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3cvjuocsr.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3rqrnvcbr.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3mgkouown.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3dlzracwq.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3utibjyrr.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3gysjfhaa.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3gjogxvte.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3xdbynfxe.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ghzmgdjl.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3cjfoyeus.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kblvjcza.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3srtpxrng.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ivakktju.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3kqyhtjsj.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3maquxhrk.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3qfjmxhfe.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3jyevvvrr.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3fcimhqff.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ryrckmwe.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3ddgixoru.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3vekmerer.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3zmrkebve.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3lwqbxpiv.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3yaiqrols.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3doypnehs.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3avhbnimt.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vfjtddro.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3ctopmcju.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3mopxrjxo.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3owpncziw.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mnijmcqo.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3bwygbjkf.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3iuvfwuzn.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3bjvmgulz.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3dikirkrf.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3bzdyphdh.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tffrcwcq.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3ardzbccm.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3oenqrkmb.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3gtusmcbm.html


<!-- 参考信息 -->