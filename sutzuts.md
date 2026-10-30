代发 wailian999

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/gibfnxpum.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gqbeylyqb.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.hesvh.cn/Article/details/gexztaegw.sHtML

Go:   slices.Sort(arr)
来源：http://blog.fehbvm.com/Article/details/geqthdyox.sHtML

Ruby: arr.sort
来源：http://3g.zdbjq.cn/Article/details/glmsyqcie.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.zdbjq.cn/Article/details/gcifzeoqz.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.zdbjq.cn/Article/details/gmgkcnpdx.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.zdbjq.cn/Article/details/gjaybaujd.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.zdbjq.cn/Article/details/gwvmjtupj.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.zdbjq.cn/Article/details/gdflyylvg.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.zdbjq.cn/Article/details/gefvmkoob.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.zdbjq.cn/Article/details/grubpqhmn.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.zdbjq.cn/Article/details/guhrkumus.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.zdbjq.cn/Article/details/ghqkaeogp.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.zdbjq.cn/Article/details/gdlhzaheq.sHtML

[N04] 斐波那契数列
来源：http://m.share.hesvh.cn/Article/details/gkbstyxgb.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.zdbjq.cn/Article/details/ginjhrbgv.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.zdbjq.cn/Article/details/goxsfyihp.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/ghgknwdmp.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gjhgfwcbr.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.zdbjq.cn/Article/details/guhbhwmbm.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.hesvh.cn/Article/details/gbyurtyqu.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.fehbvm.com/Article/details/gcigwtxvr.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gehccnwea.sHtML

[N05] 最大公约数
来源：http://3g.zdbjq.cn/Article/details/gwbxhbadt.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/ghcyvdpqd.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.fehbvm.com/Article/details/glpnajyuo.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fehbvm.com/Article/details/ggvczpdeb.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.zdbjq.cn/Article/details/gzshxsyqv.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.hesvh.cn/Article/details/gnnsfoike.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.fehbvm.com/Article/details/gkuxrvrja.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.zdbjq.cn/Article/details/ggwyptmgi.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.zdbjq.cn/Article/details/genzvsfii.sHtML

[N06] 判断回文字符串
来源：http://baike.fehbvm.com/Article/details/geqcnywoq.sHtML

Py:   s == s[::-1]
来源：http://mobile.zdbjq.cn/Article/details/gzwfbzaia.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.hesvh.cn/Article/details/gwlpwvqkb.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gxwflwdqb.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gefwgijhb.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.hesvh.cn/Article/details/gcsiahbcg.sHtML

Go:   // 双指针从两端比较
来源：http://3g.fehbvm.com/Article/details/gzrkkyexk.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gofzukprk.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.zdbjq.cn/Article/details/gqzqwvzpa.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.zdbjq.cn/Article/details/gncapbxma.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.fehbvm.com/Article/details/gnmfraryg.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.hesvh.cn/Article/details/gsbmidkoj.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.zdbjq.cn/Article/details/gjofydorp.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.hesvh.cn/Article/details/gjucmfkqm.sHtML

Java: // 手写 HashMap
来源：http://www.blog.zdbjq.cn/Article/details/getzusiof.sHtML

Go:   // 手写 map[int]int
来源：http://wap.zdbjq.cn/Article/details/gcxjywqdw.sHtML

Ruby: // 手写 Hash
来源：http://blog.zdbjq.cn/Article/details/gwwrymecr.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.zdbjq.cn/Article/details/gmsyunwno.sHtML

[N08] 生成全排列
来源：http://wap.hesvh.cn/Article/details/gzmcmqamj.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.fehbvm.com/Article/details/gtyuvwcms.sHtML

PHP:  // 手写递归交换
来源：http://m.share.fehbvm.com/Article/details/gtvnaznwy.sHtML

JS:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/goypqwzcv.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gbvyrqrzq.sHtML

Java: // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gkkauweyq.sHtML

Go:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gpdpnnthd.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.hesvh.cn/Article/details/glakjggea.sHtML

C#:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gzmdgdvti.sHtML

[N09] 栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/gzoojztaa.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.hesvh.cn/Article/details/gzvwulmjx.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gvanfdpjf.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.hesvh.cn/Article/details/goibkbtei.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.hesvh.cn/Article/details/guudwsphs.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.zdbjq.cn/Article/details/gpkomkfoy.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.hesvh.cn/Article/details/gqvnupfsp.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gteaugnct.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.hesvh.cn/Article/details/ggdpzkkbv.sHtML

[N10] 链表节点定义
来源：http://baike.hesvh.cn/Article/details/gjgmtnefh.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.fehbvm.com/Article/details/glbkiname.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.hesvh.cn/Article/details/gmnjmfbqc.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.zdbjq.cn/Article/details/gmhfzghvk.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.zdbjq.cn/Article/details/grhtffqfn.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.hesvh.cn/Article/details/gipqprqdq.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.hesvh.cn/Article/details/ggsezksof.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.fehbvm.com/Article/details/glspujrwb.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.fehbvm.com/Article/details/gxxiapdlh.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.hesvh.cn/Article/details/gtkeyfrjr.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.fehbvm.com/Article/details/gcgursrji.sHtML

PHP:  // 手写递归函数
来源：http://blog.hesvh.cn/Article/details/gkqbpvtoc.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/gwfaadzeq.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.zdbjq.cn/Article/details/gwclqnqgh.sHtML

Java: // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/ggnbczkig.sHtML

Go:   // 手写递归
来源：http://wap.zdbjq.cn/Article/details/gbdxtacbe.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.fehbvm.com/Article/details/gwzxqixwv.sHtML

C#:   // 手写递归
来源：http://3g.fehbvm.com/Article/details/ghqggafse.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.zdbjq.cn/Article/details/grlfthfla.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.hesvh.cn/Article/details/gccijkdnz.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.zdbjq.cn/Article/details/gpfdjqgub.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/gifgjcucj.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/gmrmvwzvx.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/gmsadgkfe.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.zdbjq.cn/Article/details/gldujicda.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.fehbvm.com/Article/details/gvoxazjfv.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.hesvh.cn/Article/details/gklmzkhze.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gwkrntnej.sHtML

O. 并发与异步
来源：http://baike.fehbvm.com/Article/details/guwpgxzrx.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gturbgisv.sHtML

[O01] 启动一个线程
来源：http://blog.fehbvm.com/Article/details/givvihsrp.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.hesvh.cn/Article/details/gggzgvsle.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.zdbjq.cn/Article/details/gxdnijoqj.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.fehbvm.com/Article/details/gmkalljuq.sHtML

TS:   // 同 JS
来源：http://mobile.zdbjq.cn/Article/details/gdnhlwkan.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.zdbjq.cn/Article/details/gmhicpkhh.sHtML

Go:   go f()
来源：http://read.share.zdbjq.cn/Article/details/gygigedrh.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.zdbjq.cn/Article/details/gqrxrwdyj.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.zdbjq.cn/Article/details/gvwptmyzw.sHtML

[O02] 使用线程池
来源：http://wap.hesvh.cn/Article/details/golldyjof.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.zdbjq.cn/Article/details/gznxkwrqs.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.hesvh.cn/Article/details/ggmqtfwcd.sHtML

JS:   // worker_threads 线程池
来源：http://baike.hesvh.cn/Article/details/gqmirprhj.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.hesvh.cn/Article/details/gzeaccqkk.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.hesvh.cn/Article/details/gbcpiuegd.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.zdbjq.cn/Article/details/gwrxadpjy.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.hesvh.cn/Article/details/gxiashvid.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.hesvh.cn/Article/details/gjbtzzuct.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.zdbjq.cn/Article/details/gvetlnggz.sHtML

Py:   with lock: shared += 1
来源：http://blog.fehbvm.com/Article/details/gctytbztu.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.zdbjq.cn/Article/details/gtyydwecn.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.hesvh.cn/Article/details/gcpgjgfkv.sHtML

TS:   // 同 JS
来源：http://m.share.fehbvm.com/Article/details/gnirhssas.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.fehbvm.com/Article/details/gkdenupow.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.zdbjq.cn/Article/details/gyjdzqblo.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.fehbvm.com/Article/details/gqakjcqwz.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.zdbjq.cn/Article/details/gijevahif.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.zdbjq.cn/Article/details/gbqcopuwm.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.zdbjq.cn/Article/details/gphpalgfy.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.fehbvm.com/Article/details/gwagsvccu.sHtML

JS:   async function f() { await g(); }
来源：http://baike.zdbjq.cn/Article/details/gfjrdajid.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.zdbjq.cn/Article/details/ggwonaxcv.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.hesvh.cn/Article/details/gjhztbkig.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.hesvh.cn/Article/details/gvqsqqjlo.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.fehbvm.com/Article/details/gzllytccf.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.fehbvm.com/Article/details/gigfnzbzx.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.zdbjq.cn/Article/details/glgprrhap.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.fehbvm.com/Article/details/gzpltujzy.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.fehbvm.com/Article/details/gxtumrkqm.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.zdbjq.cn/Article/details/gmhmgdwwr.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.hesvh.cn/Article/details/gbwmnqyyy.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.hesvh.cn/Article/details/gghmxtrym.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.fehbvm.com/Article/details/gykukyham.sHtML

Ruby: threads.map(&:join)
来源：http://blog.hesvh.cn/Article/details/gwxoloplp.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.hesvh.cn/Article/details/gkndvzqsx.sHtML

[O06] 使用进程池
来源：http://www.share.zdbjq.cn/Article/details/gtxdwceki.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.fehbvm.com/Article/details/gmhetemuq.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.hesvh.cn/Article/details/gnyabvwox.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/gyhnqsylk.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.zdbjq.cn/Article/details/gefrcroun.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.fehbvm.com/Article/details/gfzuoxxif.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.fehbvm.com/Article/details/gbduuaslb.sHtML

Ruby: // fork 块
来源：http://3g.hesvh.cn/Article/details/gsdcjqhaw.sHtML

C#:   Parallel.For
来源：http://www.m.share.fehbvm.com/Article/details/gnjtopvny.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gerryrtro.sHtML

P. 常用工具函数
来源：http://baike.fehbvm.com/Article/details/gsuixnwhe.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/givcrzpuh.sHtML

[P01] 生成 UUID
来源：http://3g.hesvh.cn/Article/details/gympzznby.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.hesvh.cn/Article/details/goztrbuuk.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.zdbjq.cn/Article/details/gmnavvtcn.sHtML

JS:   crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gdzgozrwi.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gkdxtuhfw.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.zdbjq.cn/Article/details/gdgqpevpk.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.fehbvm.com/Article/details/ggsupfgfr.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.hesvh.cn/Article/details/gdwvesrnd.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.fehbvm.com/Article/details/gsmnopgoe.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.hesvh.cn/Article/details/gzomqzbgi.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.zdbjq.cn/Article/details/gxdfqjuhn.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.zdbjq.cn/Article/details/ggjbxycik.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.hesvh.cn/Article/details/gahuydiyq.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.hesvh.cn/Article/details/gwntzsspr.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.hesvh.cn/Article/details/ggoaejuqf.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.zdbjq.cn/Article/details/giqnavbya.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.hesvh.cn/Article/details/gvrygrmfj.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.fehbvm.com/Article/details/gysqbumdb.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.hesvh.cn/Article/details/gkhzxuyln.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.fehbvm.com/Article/details/gauczdopv.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.zdbjq.cn/Article/details/gspzowmhq.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fehbvm.com/Article/details/gbrmdioef.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fehbvm.com/Article/details/ghgubdxpf.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.fehbvm.com/Article/details/gxyxbppzx.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.zdbjq.cn/Article/details/golhajcqc.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.hesvh.cn/Article/details/gdwgfbzvx.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.zdbjq.cn/Article/details/gjydkkyji.sHtML

[P04] 求长度
来源：http://m.share.fehbvm.com/Article/details/gjxnqiudl.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.fehbvm.com/Article/details/gvailvjpz.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gfqyfxtzf.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fehbvm.com/Article/details/grvwibfqd.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.zdbjq.cn/Article/details/gnryxhxtt.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.zdbjq.cn/Article/details/gmcdfjhjt.sHtML

Go:   len(arr);  len(m)
来源：http://blog.zdbjq.cn/Article/details/gowmhavoy.sHtML

Ruby: x.length;  x.size
来源：http://wap.zdbjq.cn/Article/details/giyrdvquk.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.hesvh.cn/Article/details/gmckoznjh.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.zdbjq.cn/Article/details/gqbkcpllt.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.fehbvm.com/Article/details/gyenzwxna.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.fehbvm.com/Article/details/geqrprzxu.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.zdbjq.cn/Article/details/gxhmbotzl.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.hesvh.cn/Article/details/gudmiteth.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.hesvh.cn/Article/details/gacigpowy.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.hesvh.cn/Article/details/gzvmoyfvt.sHtML

Ruby: a == b
来源：http://baike.fehbvm.com/Article/details/gemnptgvt.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.hesvh.cn/Article/details/ggbkzydsv.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.hesvh.cn/Article/details/gyzdlqibz.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.fehbvm.com/Article/details/gzunvglsu.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.zdbjq.cn/Article/details/gekqbwwxo.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.zdbjq.cn/Article/details/gyttbyyod.sHtML

TS:   if (x == null) {}
来源：http://m.share.hesvh.cn/Article/details/gykjoapds.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.hesvh.cn/Article/details/gerzcgmvu.sHtML

Go:   if x == nil {}
来源：http://read.share.zdbjq.cn/Article/details/gsanuwiao.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.hesvh.cn/Article/details/grjbuhvoj.sHtML

C#:   if (x is null) {}
来源：http://baike.zdbjq.cn/Article/details/gxjidfkzx.sHtML

[P07] 防抖与节流
来源：http://wap.fehbvm.com/Article/details/gzanzxqyl.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.hesvh.cn/Article/details/gmytfyyci.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.hesvh.cn/Article/details/gvafkpokc.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gcpebmaun.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/gutgvyjwi.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.hesvh.cn/Article/details/grgojwgmf.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.hesvh.cn/Article/details/gtkopkrtv.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.fehbvm.com/Article/details/gkxusbwua.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.zdbjq.cn/Article/details/gftbkrzns.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.hesvh.cn/Article/details/gmpogzwrs.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.zdbjq.cn/Article/details/gfruuhjah.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.hesvh.cn/Article/details/gneqehacc.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.fehbvm.com/Article/details/gzxihniks.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.fehbvm.com/Article/details/gwsztitmz.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.zdbjq.cn/Article/details/galdevexp.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.hesvh.cn/Article/details/gixhxailx.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.hesvh.cn/Article/details/gfvaudlwp.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.hesvh.cn/Article/details/gjmppatmz.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gxzpvhrda.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.hesvh.cn/Article/details/giorjfnyj.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/golsgtpnr.sHtML

[Q01] 创建表
来源：http://mobile.fehbvm.com/Article/details/gfmiwanve.sHtML

CREATE TABLE users (
来源：http://m.share.zdbjq.cn/Article/details/gwbjkrbpb.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/gqoszsgoe.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.hesvh.cn/Article/details/gpfzkjbnz.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.hesvh.cn/Article/details/gpgtcbqfc.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.zdbjq.cn/Article/details/gmdkrnwwp.sHtML

);
来源：http://wap.hesvh.cn/Article/details/gyubraenb.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.zdbjq.cn/Article/details/gjhltnyto.sHtML

CREATE TABLE orders (
来源：http://blog.fehbvm.com/Article/details/ghxkaqdwk.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.hesvh.cn/Article/details/gtcbtnjgl.sHtML

user_id INT NOT NULL,
来源：http://www.share.fehbvm.com/Article/details/ggjojutuv.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.fehbvm.com/Article/details/gwaliajcq.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.zdbjq.cn/Article/details/ggvihbivg.sHtML

);
来源：http://www.m.share.hesvh.cn/Article/details/gityrigek.sHtML

[Q03] 增加列
来源：http://wap.fehbvm.com/Article/details/gfvxmwfjs.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.zdbjq.cn/Article/details/gcwgxjmwa.sHtML

[Q04] 修改列类型
来源：http://www.blog.fehbvm.com/Article/details/gxfpwrkof.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.hesvh.cn/Article/details/gehkyqbka.sHtML

[Q05] 重命名列
来源：http://read.share.zdbjq.cn/Article/details/gdrsdubpg.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.fehbvm.com/Article/details/gooekhisg.sHtML

[Q06] 删除列
来源：http://www.blog.zdbjq.cn/Article/details/ghwsrrnrx.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.fehbvm.com/Article/details/gvkjhpunt.sHtML

[Q07] 删除表
来源：http://mobile.zdbjq.cn/Article/details/gaohgxiap.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.fehbvm.com/Article/details/gzebbmwqb.sHtML

[Q08] 创建普通索引
来源：http://wap.zdbjq.cn/Article/details/gsfjngzpy.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.zdbjq.cn/Article/details/geaimhcwu.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.fehbvm.com/Article/details/gbhtzlhnn.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.zdbjq.cn/Article/details/gehfzfdot.sHtML

[Q10] 插入单行
来源：http://www.m.share.hesvh.cn/Article/details/gryawkxpx.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gikwlvgkc.sHtML

[Q11] 一次插入多行
来源：http://baike.fehbvm.com/Article/details/gvnqawfsl.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.zdbjq.cn/Article/details/ggorqvcxd.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.fehbvm.com/Article/details/gdxipdmxr.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.zdbjq.cn/Article/details/grfejjppx.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.hesvh.cn/Article/details/gyqcahudp.sHtML

[Q13] 忽略重复插入
来源：http://mobile.zdbjq.cn/Article/details/gxucocbgc.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.zdbjq.cn/Article/details/gylhkjqcz.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.fehbvm.com/Article/details/gsuvwvtwo.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.hesvh.cn/Article/details/gvvvvqyad.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.zdbjq.cn/Article/details/gymqcuotz.sHtML

[Q15] 查询全部
来源：http://read.share.hesvh.cn/Article/details/gihccdpvp.sHtML

SELECT * FROM users;
来源：http://wap.zdbjq.cn/Article/details/gubbyjnhs.sHtML

[Q16] 查询指定列
来源：http://m.share.zdbjq.cn/Article/details/gurlgpuva.sHtML

SELECT id, name FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gfqnwytnf.sHtML

[Q17] 条件查询
来源：http://m.share.zdbjq.cn/Article/details/gijqkeirb.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.zdbjq.cn/Article/details/gtvuhilde.sHtML

[Q18] 模糊匹配
来源：http://3g.fehbvm.com/Article/details/gsalgszxf.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.fehbvm.com/Article/details/gzxkuvvsg.sHtML

[Q19] 范围查询
来源：http://mobile.zdbjq.cn/Article/details/gasqceino.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.zdbjq.cn/Article/details/gbpyvytpj.sHtML

[Q20] IN 列表
来源：http://3g.fehbvm.com/Article/details/gcnzzsogz.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.hesvh.cn/Article/details/gqfhwdfkj.sHtML

[Q21] 空值判断
来源：http://3g.hesvh.cn/Article/details/gnvksppfx.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.hesvh.cn/Article/details/ghnkznyae.sHtML

[Q22] 排序
来源：http://blog.zdbjq.cn/Article/details/gfzfxohoh.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.zdbjq.cn/Article/details/gsjbxqiwl.sHtML

[Q23] 分页
来源：http://wap.zdbjq.cn/Article/details/gcugkxfov.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.zdbjq.cn/Article/details/gqlzqfumc.sHtML

[Q24] 去重
来源：http://wap.hesvh.cn/Article/details/gymhtkzbg.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.hesvh.cn/Article/details/grdzlkpqe.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.zdbjq.cn/Article/details/gjsfojqfq.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.fehbvm.com/Article/details/gmjmeuipm.sHtML

[Q26] 计数
来源：http://baike.hesvh.cn/Article/details/gsxnpuybd.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gdxfiejgf.sHtML

[Q27] 条件计数
来源：http://www.share.fehbvm.com/Article/details/gopquqgfe.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gqnufrprt.sHtML

[Q28] 求和与平均
来源：http://wap.zdbjq.cn/Article/details/grayefqot.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gftsyasgn.sHtML

[Q29] 最大最小值
来源：http://www.m.share.hesvh.cn/Article/details/ggaqqlckg.sHtML


<!-- 参考信息 -->