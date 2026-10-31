代发 wailian999

C#:   Directory.GetCurrentDirectory()
来源：http://xi.bjjhwx.cn

[M05] 设置退出码
来源：http://us.bookmarksfly.cn

Py:   sys.exit(1)
来源：http://ha.hahajie.cn

PHP:  exit(1);
来源：http://ub.bjjhwx.cn

JS:   process.exit(1)
来源：http://gr.bjjhwx.cn

TS:   process.exit(1)
来源：http://mf.newstarts.cn

Java: System.exit(1)
来源：http://ll.yuexingan06.cn

Go:   os.Exit(1)
来源：http://jt.9csxet.cn

Ruby: exit 1
来源：http://gs.newstarts.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://uv.szxytkj.cn

[M06] 向标准错误输出
来源：http://ah.panjiajie.cn

Py:   print("err", file=sys.stderr)
来源：http://yx.bookmarksfly.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://nd.huixinmuqiang.cn

JS:   console.error("err")
来源：http://gd.haigaiapp.cn

TS:   console.error("err")
来源：http://tf.jianghongdianzi.cn

Java: System.err.println("err")
来源：http://oj.haigaiapp.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://zz.haigaiapp.cn

Ruby: warn "err"
来源：http://sc.newstarts.cn

C#:   Console.Error.WriteLine("err")
来源：http://ht.nszjky.cn

[M07] 判断是否为主入口
来源：http://sl.newstarts.cn

Py:   if __name__ == "__main__":
来源：http://du.muxihuayi.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://qi.panjiajie.cn

JS:   require.main === module
来源：http://lg.gzmigu.cn

TS:   require.main === module
来源：http://tj.haigaiapp.cn

Java: public static void main(String[] args)
来源：http://mt.lnxyls.cn

Go:   func main()
来源：http://ea.jianghongdianzi.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://jz.yuexingan06.cn

C#:   static void Main(string[] args)
来源：http://qn.jctech888.com.cn

[M08] 获取系统与运行时信息
来源：http://zb.szsharing.cn

Py:   platform.system();  platform.python_version()
来源：http://tk.huixiangedu.cn

PHP:  PHP_OS;  phpversion();
来源：http://dk.shtwfgs.cn

JS:   process.platform;  process.version
来源：http://sx.bookmarksfly.cn

TS:   process.platform;  process.version
来源：http://kn.bookmarksfly.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://kl.wgjwhj.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://oj.jianghongdianzi.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://np.wgjwhj.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://jh.9csxet.cn

================================================================================
来源：http://jh.jianghongdianzi.cn

N. 数据结构与算法
来源：http://xt.bjjhwx.cn

================================================================================
来源：http://wv.muxihuayi.cn

[N01] 二分查找（有序数组）
来源：http://fi.9csxet.cn

Py:   bisect.bisect_left(arr, x)
来源：http://sb.chemitech.net.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://cp.jianghongdianzi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fz.shtwfgs.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kp.bjjhwx.cn

Java: Arrays.binarySearch(arr, x)
来源：http://nu.huanxung.cn

Go:   sort.SearchInts(arr, x)
来源：http://nn.haigaiapp.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://jf.yuexingan06.cn

C#:   Array.BinarySearch(arr, x)
来源：http://xb.gzmigu.cn

[N02] 排序（工程实践用内置实现）
来源：http://wu.gzmigu.cn

Py:   sorted(arr);  arr.sort()
来源：http://ps.9csxet.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hr.nszjky.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://uj.shtwfgs.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://hi.yuntaijiaju.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://vm.nszjky.cn

Go:   slices.Sort(arr)
来源：http://nv.colortex.cn

Ruby: arr.sort
来源：http://qz.colortex.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://hc.szsharing.cn

[N03] 快速排序（分治示例）
来源：http://my.wgjwhj.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://zz.yuexingan06.cn

PHP:  // 递归实现，或用 usort
来源：http://yl.colortex.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ad.chemitech.net.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qf.huixiangedu.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hh.shxzskj.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ht.jctech888.com.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xp.szxytkj.cn

C#:   // 手写递归，或 Array.Sort
来源：http://hq.jianghongdianzi.cn

[N04] 斐波那契数列
来源：http://cw.szxytkj.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://it.chemitech.net.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://uh.nicolike.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pm.shxzskj.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lo.szxytkj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hh.9csxet.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://zy.yuexingan06.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://vo.yuexingan06.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://it.shtwfgs.cn

[N05] 最大公约数
来源：http://gm.lnxyls.cn

Py:   math.gcd(a, b)
来源：http://si.szsharing.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ad.nszjky.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://of.lnxyls.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ba.szsharing.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://vy.hahajie.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://qf.colortex.cn

Ruby: a.gcd(b)
来源：http://wv.yuntaijiaju.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://md.yuntaijiaju.cn

[N06] 判断回文字符串
来源：http://gq.nicolike.cn

Py:   s == s[::-1]
来源：http://ut.huixinmuqiang.cn

PHP:  $s === strrev($s);
来源：http://fp.szxytkj.cn

JS:   s === [...s].reverse().join("")
来源：http://ih.shxzukj.cn

TS:   s === [...s].reverse().join("")
来源：http://pa.shxzukj.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://jx.colortex.cn

Go:   // 双指针从两端比较
来源：http://ox.hahajie.cn

Ruby: s == s.reverse
来源：http://et.asd995.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://do.hnjuh.cn

[N07] 两数之和（返回下标）
来源：http://by.nicolike.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ih.newstarts.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ac.muxihuayi.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://mi.521024.cn

TS:   // 手写 Map<string, number>
来源：http://yr.shxzskj.cn

Java: // 手写 HashMap
来源：http://bn.lnxyls.cn

Go:   // 手写 map[int]int
来源：http://zq.huixinmuqiang.cn

Ruby: // 手写 Hash
来源：http://ld.jianghongdianzi.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ws.huanxung.cn

[N08] 生成全排列
来源：http://ho.shtwfgs.cn

Py:   itertools.permutations(arr)
来源：http://oa.muxihuayi.cn

PHP:  // 手写递归交换
来源：http://mc.jianghongdianzi.cn

JS:   // 手写回溯递归
来源：http://go.jctech888.com.cn

TS:   // 手写回溯递归
来源：http://lb.yuntaijiaju.cn

Java: // 手写回溯递归
来源：http://qz.9csxet.cn

Go:   // 手写回溯递归
来源：http://gc.chemitech.net.cn

Ruby: arr.permutation.to_a
来源：http://fc.9csxet.cn

C#:   // 手写回溯递归
来源：http://fk.521024.cn

[N09] 栈与队列
来源：http://ag.shtwfgs.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://kh.haigaiapp.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ms.jctech888.com.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ea.9csxet.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://gi.chemitech.net.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://zy.hahajie.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://je.gzmigu.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://oy.colortex.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://py.shtwfgs.cn

[N10] 链表节点定义
来源：http://je.shxzskj.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://go.shxzukj.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://go.yuntaijiaju.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://zh.huanxung.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ro.shtwfgs.cn

Java: class Node { int v; Node next; }
来源：http://di.shtwfgs.cn

Go:   type Node struct { V int; Next *Node }
来源：http://up.521024.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://hw.newstarts.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://zh.shxzskj.cn

[N11] 二叉树中序遍历
来源：http://xt.hahajie.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://dl.huixinmuqiang.cn

PHP:  // 手写递归函数
来源：http://zp.asd995.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cf.huanxung.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qe.hahajie.cn

Java: // 手写递归
来源：http://wf.lnxyls.cn

Go:   // 手写递归
来源：http://rr.szxytkj.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://em.asd995.cn

C#:   // 手写递归
来源：http://pq.huixinmuqiang.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://sw.haigaiapp.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hh.nszjky.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://de.9csxet.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ri.chemitech.net.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mc.nicolike.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ah.shtwfgs.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://jb.chemitech.net.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://jf.szsharing.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://gr.yuntaijiaju.cn

================================================================================
来源：http://ek.panjiajie.cn

O. 并发与异步
来源：http://dw.asd995.cn

================================================================================
来源：http://gx.asd995.cn

[O01] 启动一个线程
来源：http://bi.shxzskj.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://sh.bookmarksfly.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://of.gzmigu.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://cd.haigaiapp.cn

TS:   // 同 JS
来源：http://dy.jianghongdianzi.cn

Java: new Thread(() -> f()).start()
来源：http://hy.gzmigu.cn

Go:   go f()
来源：http://gz.9csxet.cn

Ruby: Thread.new { f }
来源：http://jg.huixiangedu.cn

C#:   Task.Run(() => F());
来源：http://du.huixinmuqiang.cn

[O02] 使用线程池
来源：http://xr.huixiangedu.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://vk.haigaiapp.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ce.szxytkj.cn

JS:   // worker_threads 线程池
来源：http://ke.szsharing.cn

TS:   // worker_threads 线程池
来源：http://cn.yuntaijiaju.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ac.haigaiapp.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://kl.newstarts.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://lm.shxzukj.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://km.szsharing.cn

[O03] 加锁保护共享数据
来源：http://rc.hahajie.cn

Py:   with lock: shared += 1
来源：http://mp.bjjhwx.cn

PHP:  // 用 flock() 做文件锁
来源：http://lp.asd995.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://je.hahajie.cn

TS:   // 同 JS
来源：http://uw.jianghongdianzi.cn

Java: synchronized (this) { shared++; }
来源：http://wi.huixiangedu.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://pj.yuntaijiaju.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ur.yuntaijiaju.cn

C#:   lock (gate) { shared++; }
来源：http://bw.hnjuh.cn

[O04] 定义异步函数并等待
来源：http://fk.yuexingan06.cn

Py:   async def f():⏎    await g()
来源：http://eo.nicolike.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mw.521024.cn

JS:   async function f() { await g(); }
来源：http://ek.521024.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://vu.nszjky.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ep.shtwfgs.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://qt.szsharing.cn

Ruby: # 用 Fiber 或 async gem
来源：http://oy.colortex.cn

C#:   async Task F() { await G(); }
来源：http://bz.gzmigu.cn

[O05] 并发执行并等待全部完成
来源：http://zt.huixinmuqiang.cn

Py:   asyncio.gather(*tasks)
来源：http://cr.szxytkj.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://od.shtwfgs.cn

JS:   await Promise.all(tasks)
来源：http://hj.jctech888.com.cn

TS:   await Promise.all(tasks)
来源：http://dh.yuntaijiaju.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://qj.huixiangedu.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://zx.yuexingan06.cn

Ruby: threads.map(&:join)
来源：http://qw.shtwfgs.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://yz.szsharing.cn

[O06] 使用进程池
来源：http://su.wgjwhj.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://yz.huixiangedu.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://vh.chemitech.net.cn

JS:   // child_process / cluster 模块
来源：http://hd.yuntaijiaju.cn

TS:   // child_process / cluster 模块
来源：http://ux.huixinmuqiang.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://gs.asd995.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://do.wgjwhj.cn

Ruby: // fork 块
来源：http://sc.hnjuh.cn

C#:   Parallel.For
来源：http://ck.huixinmuqiang.cn

================================================================================
来源：http://me.colortex.cn

P. 常用工具函数
来源：http://qq.hahajie.cn

================================================================================
来源：http://tx.chemitech.net.cn

[P01] 生成 UUID
来源：http://gv.bjjhwx.cn

Py:   str(uuid.uuid4())
来源：http://bb.9csxet.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://fd.huanxung.cn

JS:   crypto.randomUUID()
来源：http://kw.huanxung.cn

TS:   crypto.randomUUID()
来源：http://oa.szxytkj.cn

Java: UUID.randomUUID().toString()
来源：http://ld.haigaiapp.cn

Go:   // 用 github.com/google/uuid
来源：http://ql.huixinmuqiang.cn

Ruby: SecureRandom.uuid
来源：http://ll.asd995.cn

C#:   Guid.NewGuid().ToString()
来源：http://vl.colortex.cn

[P02] MD5 / SHA256 摘要
来源：http://rr.asd995.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://gn.szsharing.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://yi.shtwfgs.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ti.huanxung.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ia.chemitech.net.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://xy.huixinmuqiang.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ci.shtwfgs.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://in.panjiajie.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://kv.bjjhwx.cn

[P03] 生成短随机字符串
来源：http://xc.gzmigu.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://rx.wgjwhj.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://fl.haigaiapp.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://au.asd995.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gw.wgjwhj.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ti.lnxyls.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ci.asd995.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://gz.9csxet.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://aj.521024.cn

[P04] 求长度
来源：http://do.shxzskj.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wx.bjjhwx.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cf.haigaiapp.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gg.shxzukj.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tn.nicolike.cn

Java: list.size();  map.size();  s.length()
来源：http://kz.panjiajie.cn

Go:   len(arr);  len(m)
来源：http://sk.jianghongdianzi.cn

Ruby: x.length;  x.size
来源：http://ds.asd995.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://va.hahajie.cn

[P05] 判断两个对象内容是否相等
来源：http://md.chemitech.net.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://pn.shxzskj.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ul.colortex.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://qa.huixinmuqiang.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://pt.shxzukj.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ut.bookmarksfly.cn

Go:   reflect.DeepEqual(a, b)
来源：http://py.shxzukj.cn

Ruby: a == b
来源：http://ho.colortex.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://yc.haigaiapp.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://qw.huixinmuqiang.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://as.haigaiapp.cn

PHP:  if (empty($x)) {}
来源：http://yj.gzmigu.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ww.bjjhwx.cn

TS:   if (x == null) {}
来源：http://ln.nicolike.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://zt.jctech888.com.cn

Go:   if x == nil {}
来源：http://cy.muxihuayi.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://cu.szsharing.cn

C#:   if (x is null) {}
来源：http://to.bjjhwx.cn

[P07] 防抖与节流
来源：http://sy.haigaiapp.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ep.jianghongdianzi.cn

PHP:  // 手写时间戳比较
来源：http://gc.shtwfgs.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kk.shxzskj.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pk.hahajie.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hg.hnjuh.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://dr.wgjwhj.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://xr.wgjwhj.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://jm.yuntaijiaju.cn

[P08] 处理浮点精度问题
来源：http://ta.nszjky.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://yk.shtwfgs.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://tj.bjjhwx.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ua.yuntaijiaju.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://qc.panjiajie.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hn.huanxung.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://af.colortex.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ku.lnxyls.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://it.shxzskj.cn

================================================================================
来源：http://xd.nszjky.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://nd.szxytkj.cn

================================================================================
来源：http://tz.shxzukj.cn

[Q01] 创建表
来源：http://yz.shtwfgs.cn

CREATE TABLE users (
来源：http://ch.hahajie.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://fh.asd995.cn

name VARCHAR(50) NOT NULL,
来源：http://kf.newstarts.cn

email VARCHAR(100) UNIQUE,
来源：http://jj.chemitech.net.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://uc.haigaiapp.cn

);
来源：http://lo.colortex.cn

[Q02] 创建带外键的表
来源：http://ws.nicolike.cn

CREATE TABLE orders (
来源：http://qr.huixinmuqiang.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://la.shxzskj.cn

user_id INT NOT NULL,
来源：http://by.jctech888.com.cn

amount DECIMAL(10, 2),
来源：http://mt.huanxung.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://iu.bjjhwx.cn

);
来源：http://tv.shtwfgs.cn

[Q03] 增加列
来源：http://bm.huixiangedu.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://zh.nszjky.cn

[Q04] 修改列类型
来源：http://qg.shtwfgs.cn


<!-- 参考信息 -->