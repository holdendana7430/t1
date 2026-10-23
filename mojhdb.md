代发 wailian999

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3pqxlpnbz.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3aulcguwm.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3gfysgxze.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3hbvagros.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3ljfzhtja.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3cbspbcls.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3ypnlgglf.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3megqiqru.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3tnarwydu.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3thwrhhjt.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3ocojfxjd.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3ktsguyry.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3omturkph.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3ndphxqlq.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3xfkmptdg.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3hnkchnlx.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3ysqylxyh.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3mssgwwtl.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3bbusnmsr.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3mmtmuetk.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3omwlkqfu.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3jyghqnzd.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3dvwbrgtc.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3lxuenkrq.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3fsolozyr.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3pccknooy.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3gmtfgbrc.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3gvqouxhl.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3dhvbwrqn.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3xpilefov.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3ckgcjsmk.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3wfyauzkp.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3eholyroq.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ldwbywkv.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3qodwwsop.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3ncrnpzmn.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3viidactz.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3ctlzrhty.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3foqguirt.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3ouiohmwj.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3gdaezgbt.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3tvbvemda.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3qtvbatuz.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3xirrggms.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3cxhcqzsy.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3bcfwmcxn.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3irasxcqt.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3lptbaxds.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vnlotfpr.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3fqfamdxh.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ynrznhuu.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3kpsaoqjs.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3dccqmwww.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3olcgnkab.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3kamtsbcn.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3vyxuapzb.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3uvcnzsvj.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3fwmymysu.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ccnkchyn.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3eeoqdsju.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3foagbfhz.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3tukyzhld.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3xumxnfak.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3htkdpdkw.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3vdnxhplc.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3tgaffyzc.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3wzzbifcd.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3vqozafem.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3kjaxpzas.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3mqhwsbne.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3vqhqwjpt.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3knaeevju.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3fgiifxdh.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3jpevcqbw.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3etuohpvo.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3qjyzvwmr.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3xuoptwre.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3aournvzs.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3hbwxoqtz.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ezlodyfu.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3oyydhjza.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3atgqiwdj.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3cdnmqkpo.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3vsemquge.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3ezwwzmmg.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3saszlnmz.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3iwoomxcq.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3xffwgdzf.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3fnntjovu.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3rqcvcgpd.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3cbfwlwqz.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3yvdcrcli.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3djugsdwf.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3mrdgysmi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yshxwieo.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3tvelgbhg.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3wcowtpaa.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3unykaihs.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3azkztiya.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3zrwjmktd.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3bszonhks.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3bobscvmt.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3xwmlompp.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3jnucloyq.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3qthbkxrx.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3rbrpdtyj.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3sqztvqmf.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3hvnsfyxa.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3cxuonjgj.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3uiwcjcjw.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3mxvwdvjb.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3mnmsvcto.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3jaslwefn.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3prvgrtjv.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3ojyljpmd.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3vbrsqegd.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3padbgxvs.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3iwmggkms.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3dowmvzam.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3xiroanff.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3niihiixh.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3lffkubqb.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3cjvyduqp.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3uqqdoazi.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3dpgbgugh.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3zttonhle.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cnglgdyh.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3nxkwkbhx.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3ckzhcoal.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3wositsil.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3wdzlpshd.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3hyqumdzc.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3yibcrknj.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3kxlfdpys.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3behijyge.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3ruuonouj.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3npmuhzuv.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3rmugylvq.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3qrjgbjny.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3aiwaivvm.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3onjddgfi.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3ccxdmgyw.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3fktcjyfu.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3asgefghw.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3neogfzqq.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3ifrruviu.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3zjutvrwj.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3wfiihuit.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3crgsnebb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gbqvdozs.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3dajmvard.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eeypxvjm.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3warxvygm.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3ayyqzirn.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3uihpxkrd.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3xrpnjqvn.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3myshzmrk.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3zubmgpnr.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3rjxuykid.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3saqsqhov.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3uzbepcyc.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3uggjkhfn.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3rfzzreck.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3yywtoiqw.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3kjrvfywd.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3tcncobwb.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ypgwspbp.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3fayqyuad.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3pcsyqahn.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3anctqhnq.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rqdrvhsy.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3dxidopat.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3whsmkrxa.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3eabutkxx.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3etqvipri.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3qgxubblt.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3psidlmjj.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3ttfjdnsz.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3jilahozk.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3mklbpypn.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3rqbzbred.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3iejwwsbq.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3hacjufut.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3vnnuvagz.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3kzdtxmbq.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3tqscrzmq.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3kglvhosq.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3skizveln.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3psmmodxc.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3lgnctphp.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3zxpwtuxu.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3xrbennue.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3tmsunvmb.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3bwcnuboy.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3vtfpeivt.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3kjobjwat.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3rfycnldi.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3nxqrfndm.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3kkyvnhxs.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3nwvlgssh.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3mszafraz.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uqayfamb.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3cskawaqb.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3jvfrugcx.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3znqqxgdo.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3dwvxdljq.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3gevjvpdd.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3wwtmyafd.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3qbelthvy.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3kikmohij.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3kfmgzngz.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kdaviqpx.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3daooawxi.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3tckmhbmy.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3qoxloija.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3ucwxutsk.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3zkpxbzyq.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3ivfstybh.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3captqvkj.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3zpsoecsg.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3augncypa.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3tuitfbrs.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3hfpddddc.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3gzjywgdp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rnphhhnv.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3lpjvrndx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wfstnzpn.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3mbcxrzax.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3oemyhasm.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3jnfwgozv.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3pkluiyfg.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3krwadvbs.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3lhppzwyf.html

);
来源：http://www.52xcode.cn/Article/details/gt3ijeggjpt.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3epzgrnbx.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3xvmmmmcs.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3cjowlhgp.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3zlcsowpg.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3jraipnqq.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3gknvhcwm.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3ylajugrm.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3qsmvvfnf.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3znqwnjhm.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3hgagnkfh.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3aowngkhl.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3odycdyiw.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3vhnopfhr.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3bfjbqkuj.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3nrbsuuze.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3rwogfaaz.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3zicybvqm.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3rivjmozc.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3taeygrea.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3ztzlgalb.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3ldfeljpz.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3hjxbefzo.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3rtwtmuww.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3ejxlgtnz.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3tuydcapd.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3bufhvkzz.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3hodjclrz.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3ngttminy.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3jlmlfqqe.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3dxcorxjo.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3boqtdoei.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3qqtefkgo.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3fjgbtscv.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3vptqlofb.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ugxjocal.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3cpdoeamb.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3awxxdgix.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3cwuhagpr.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3edglsjtl.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3oathxowj.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3nmyfjlld.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3awyfzfms.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3sgomvcjs.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3ucbrhfsr.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3vluismre.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3cmxfgzkr.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3yykyypoc.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3rsyitjji.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3aeeiioyh.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3lgrtjdzw.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3mqynqnrv.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3uunueqli.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qdgolhox.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3ujndusrc.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3ofjdxlwx.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3ymkckboz.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kbayixuo.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3bziziomk.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3sjomicaj.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3benufdul.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3gwctbqhn.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3wjsngrqi.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3daknvhpp.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3raqmtmjc.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3csikcgqh.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3lrzzxbuo.html


<!-- 参考信息 -->