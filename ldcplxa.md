代发 wailian999

C#:   Directory.GetCurrentDirectory()
来源：http://dh.huanxung.cn

[M05] 设置退出码
来源：http://zc.szsharing.cn

Py:   sys.exit(1)
来源：http://gg.bookmarksfly.cn

PHP:  exit(1);
来源：http://ed.nszjky.cn

JS:   process.exit(1)
来源：http://rt.9csxet.cn

TS:   process.exit(1)
来源：http://jm.panjiajie.cn

Java: System.exit(1)
来源：http://ua.jianghongdianzi.cn

Go:   os.Exit(1)
来源：http://fy.szsharing.cn

Ruby: exit 1
来源：http://ns.jianghongdianzi.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://sr.asd995.cn

[M06] 向标准错误输出
来源：http://ij.wgjwhj.cn

Py:   print("err", file=sys.stderr)
来源：http://je.panjiajie.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://bo.521024.cn

JS:   console.error("err")
来源：http://we.shxzukj.cn

TS:   console.error("err")
来源：http://sv.huanxung.cn

Java: System.err.println("err")
来源：http://sq.bookmarksfly.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wa.chemitech.net.cn

Ruby: warn "err"
来源：http://vi.shxzukj.cn

C#:   Console.Error.WriteLine("err")
来源：http://yt.jctech888.com.cn

[M07] 判断是否为主入口
来源：http://rk.huanxung.cn

Py:   if __name__ == "__main__":
来源：http://br.yuexingan06.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://dk.jianghongdianzi.cn

JS:   require.main === module
来源：http://rx.szsharing.cn

TS:   require.main === module
来源：http://pq.9csxet.cn

Java: public static void main(String[] args)
来源：http://jf.9csxet.cn

Go:   func main()
来源：http://oq.asd995.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mh.nszjky.cn

C#:   static void Main(string[] args)
来源：http://zm.huixiangedu.cn

[M08] 获取系统与运行时信息
来源：http://jj.gzmigu.cn

Py:   platform.system();  platform.python_version()
来源：http://vu.panjiajie.cn

PHP:  PHP_OS;  phpversion();
来源：http://gr.yuexingan06.cn

JS:   process.platform;  process.version
来源：http://ia.huixinmuqiang.cn

TS:   process.platform;  process.version
来源：http://af.nszjky.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mg.hnjuh.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://uh.nicolike.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ww.gzmigu.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://lp.yuntaijiaju.cn

================================================================================
来源：http://rj.shtwfgs.cn

N. 数据结构与算法
来源：http://db.chemitech.net.cn

================================================================================
来源：http://am.jianghongdianzi.cn

[N01] 二分查找（有序数组）
来源：http://dy.huanxung.cn

Py:   bisect.bisect_left(arr, x)
来源：http://so.hnjuh.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://cq.asd995.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fx.hnjuh.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vp.shxzukj.cn

Java: Arrays.binarySearch(arr, x)
来源：http://he.jianghongdianzi.cn

Go:   sort.SearchInts(arr, x)
来源：http://ug.huixinmuqiang.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://wd.panjiajie.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ua.newstarts.cn

[N02] 排序（工程实践用内置实现）
来源：http://im.gzmigu.cn

Py:   sorted(arr);  arr.sort()
来源：http://uq.bjjhwx.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://pm.hnjuh.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://lq.bjjhwx.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://jk.9csxet.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mu.lnxyls.cn

Go:   slices.Sort(arr)
来源：http://eo.9csxet.cn

Ruby: arr.sort
来源：http://qg.asd995.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://os.nicolike.cn

[N03] 快速排序（分治示例）
来源：http://aq.jianghongdianzi.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hr.wgjwhj.cn

PHP:  // 递归实现，或用 usort
来源：http://al.szsharing.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ii.wgjwhj.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ql.bookmarksfly.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://vn.colortex.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hc.huixiangedu.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://vi.haigaiapp.cn

C#:   // 手写递归，或 Array.Sort
来源：http://il.9csxet.cn

[N04] 斐波那契数列
来源：http://ue.szsharing.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qn.szxytkj.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://sg.yuexingan06.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ul.nszjky.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yu.hahajie.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://xw.shxzskj.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://pt.bookmarksfly.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://pb.shtwfgs.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ip.panjiajie.cn

[N05] 最大公约数
来源：http://ze.wgjwhj.cn

Py:   math.gcd(a, b)
来源：http://pm.nszjky.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://uw.panjiajie.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tl.jianghongdianzi.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mg.yuntaijiaju.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://pf.9csxet.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://zg.jctech888.com.cn

Ruby: a.gcd(b)
来源：http://ho.huixinmuqiang.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ao.muxihuayi.cn

[N06] 判断回文字符串
来源：http://qg.9csxet.cn

Py:   s == s[::-1]
来源：http://wt.wgjwhj.cn

PHP:  $s === strrev($s);
来源：http://ur.jianghongdianzi.cn

JS:   s === [...s].reverse().join("")
来源：http://qc.huanxung.cn

TS:   s === [...s].reverse().join("")
来源：http://mr.shxzukj.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ue.asd995.cn

Go:   // 双指针从两端比较
来源：http://ez.nszjky.cn

Ruby: s == s.reverse
来源：http://tl.bjjhwx.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ye.muxihuayi.cn

[N07] 两数之和（返回下标）
来源：http://ut.huixiangedu.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://zf.yuexingan06.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://eh.lnxyls.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://gy.shxzskj.cn

TS:   // 手写 Map<string, number>
来源：http://dw.bjjhwx.cn

Java: // 手写 HashMap
来源：http://zx.shxzskj.cn

Go:   // 手写 map[int]int
来源：http://xp.9csxet.cn

Ruby: // 手写 Hash
来源：http://zh.colortex.cn

C#:   // 手写 Dictionary<int, int>
来源：http://jg.huixinmuqiang.cn

[N08] 生成全排列
来源：http://jr.yuexingan06.cn

Py:   itertools.permutations(arr)
来源：http://cv.chemitech.net.cn

PHP:  // 手写递归交换
来源：http://ze.nszjky.cn

JS:   // 手写回溯递归
来源：http://oq.szsharing.cn

TS:   // 手写回溯递归
来源：http://of.shtwfgs.cn

Java: // 手写回溯递归
来源：http://vj.asd995.cn

Go:   // 手写回溯递归
来源：http://rp.shxzskj.cn

Ruby: arr.permutation.to_a
来源：http://be.newstarts.cn

C#:   // 手写回溯递归
来源：http://hh.huanxung.cn

[N09] 栈与队列
来源：http://pq.bookmarksfly.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ne.wgjwhj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://vm.nicolike.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wk.yuexingan06.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://cs.asd995.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://iw.bookmarksfly.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://jk.chemitech.net.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://yv.shtwfgs.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://xr.nicolike.cn

[N10] 链表节点定义
来源：http://gg.wgjwhj.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wh.521024.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ll.hahajie.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://sw.haigaiapp.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://im.9csxet.cn

Java: class Node { int v; Node next; }
来源：http://uh.bjjhwx.cn

Go:   type Node struct { V int; Next *Node }
来源：http://qn.chemitech.net.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ut.hnjuh.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://py.gzmigu.cn

[N11] 二叉树中序遍历
来源：http://hr.huanxung.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ma.muxihuayi.cn

PHP:  // 手写递归函数
来源：http://hj.jctech888.com.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fd.nicolike.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ro.hahajie.cn

Java: // 手写递归
来源：http://aq.panjiajie.cn

Go:   // 手写递归
来源：http://ua.haigaiapp.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://rg.521024.cn

C#:   // 手写递归
来源：http://jh.haigaiapp.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ik.huixiangedu.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://zv.hahajie.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://cz.huixiangedu.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hp.bjjhwx.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rz.huixinmuqiang.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://lr.jianghongdianzi.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ui.huanxung.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://cc.gzmigu.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://xm.muxihuayi.cn

================================================================================
来源：http://gv.szsharing.cn

O. 并发与异步
来源：http://iw.haigaiapp.cn

================================================================================
来源：http://of.huixinmuqiang.cn

[O01] 启动一个线程
来源：http://sw.jianghongdianzi.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mz.gzmigu.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ik.newstarts.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://li.jianghongdianzi.cn

TS:   // 同 JS
来源：http://tz.shtwfgs.cn

Java: new Thread(() -> f()).start()
来源：http://mg.szsharing.cn

Go:   go f()
来源：http://qq.yuntaijiaju.cn

Ruby: Thread.new { f }
来源：http://go.newstarts.cn

C#:   Task.Run(() => F());
来源：http://vx.gzmigu.cn

[O02] 使用线程池
来源：http://qx.nszjky.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://vu.yuntaijiaju.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://qp.hnjuh.cn

JS:   // worker_threads 线程池
来源：http://pm.nicolike.cn

TS:   // worker_threads 线程池
来源：http://pm.bjjhwx.cn

Java: Executors.newFixedThreadPool(4)
来源：http://vs.colortex.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://qg.shtwfgs.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://fm.hnjuh.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hs.chemitech.net.cn

[O03] 加锁保护共享数据
来源：http://jn.newstarts.cn

Py:   with lock: shared += 1
来源：http://ix.bookmarksfly.cn

PHP:  // 用 flock() 做文件锁
来源：http://ji.jianghongdianzi.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://br.bjjhwx.cn

TS:   // 同 JS
来源：http://wj.nicolike.cn

Java: synchronized (this) { shared++; }
来源：http://ii.wgjwhj.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://fv.colortex.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://pg.hahajie.cn

C#:   lock (gate) { shared++; }
来源：http://mz.shxzukj.cn

[O04] 定义异步函数并等待
来源：http://za.colortex.cn

Py:   async def f():⏎    await g()
来源：http://co.jctech888.com.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://bf.jianghongdianzi.cn

JS:   async function f() { await g(); }
来源：http://kw.panjiajie.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ri.shxzukj.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://of.nicolike.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ed.colortex.cn

Ruby: # 用 Fiber 或 async gem
来源：http://tg.huixinmuqiang.cn

C#:   async Task F() { await G(); }
来源：http://sr.colortex.cn

[O05] 并发执行并等待全部完成
来源：http://qp.jianghongdianzi.cn

Py:   asyncio.gather(*tasks)
来源：http://bs.nszjky.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://gq.shxzukj.cn

JS:   await Promise.all(tasks)
来源：http://al.szxytkj.cn

TS:   await Promise.all(tasks)
来源：http://uz.yuexingan06.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ic.chemitech.net.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://rv.lnxyls.cn

Ruby: threads.map(&:join)
来源：http://ix.haigaiapp.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://iu.colortex.cn

[O06] 使用进程池
来源：http://tk.asd995.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://gp.9csxet.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://sy.jianghongdianzi.cn

JS:   // child_process / cluster 模块
来源：http://oz.shxzukj.cn

TS:   // child_process / cluster 模块
来源：http://rg.huanxung.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://fk.huixinmuqiang.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://if.lnxyls.cn

Ruby: // fork 块
来源：http://em.shtwfgs.cn

C#:   Parallel.For
来源：http://ik.lnxyls.cn

================================================================================
来源：http://iv.shxzskj.cn

P. 常用工具函数
来源：http://io.bjjhwx.cn

================================================================================
来源：http://cz.9csxet.cn

[P01] 生成 UUID
来源：http://th.haigaiapp.cn

Py:   str(uuid.uuid4())
来源：http://fu.bookmarksfly.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ak.gzmigu.cn

JS:   crypto.randomUUID()
来源：http://tq.nicolike.cn

TS:   crypto.randomUUID()
来源：http://pf.shxzukj.cn

Java: UUID.randomUUID().toString()
来源：http://vb.wgjwhj.cn

Go:   // 用 github.com/google/uuid
来源：http://pz.wgjwhj.cn

Ruby: SecureRandom.uuid
来源：http://qr.hahajie.cn

C#:   Guid.NewGuid().ToString()
来源：http://ag.panjiajie.cn

[P02] MD5 / SHA256 摘要
来源：http://mk.jctech888.com.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://te.hahajie.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ev.jianghongdianzi.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://db.colortex.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://tk.huanxung.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ni.bjjhwx.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://es.shtwfgs.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://cs.521024.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://jc.bjjhwx.cn

[P03] 生成短随机字符串
来源：http://nt.huixiangedu.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://gk.9csxet.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://js.nszjky.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gs.shxzukj.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ba.521024.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ou.chemitech.net.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://he.jianghongdianzi.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://lj.yuntaijiaju.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://do.bookmarksfly.cn

[P04] 求长度
来源：http://fl.yuntaijiaju.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://kb.nicolike.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zw.nicolike.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lm.szxytkj.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lb.huanxung.cn

Java: list.size();  map.size();  s.length()
来源：http://ue.haigaiapp.cn

Go:   len(arr);  len(m)
来源：http://hg.jianghongdianzi.cn

Ruby: x.length;  x.size
来源：http://bv.9csxet.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://cn.shxzskj.cn

[P05] 判断两个对象内容是否相等
来源：http://ks.newstarts.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://zb.jctech888.com.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://qr.9csxet.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://fg.hnjuh.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://jj.gzmigu.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ww.lnxyls.cn

Go:   reflect.DeepEqual(a, b)
来源：http://er.huixinmuqiang.cn

Ruby: a == b
来源：http://zc.hnjuh.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ro.hnjuh.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ho.jianghongdianzi.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://eo.szsharing.cn

PHP:  if (empty($x)) {}
来源：http://zy.nicolike.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://xg.haigaiapp.cn

TS:   if (x == null) {}
来源：http://bu.9csxet.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://jl.lnxyls.cn

Go:   if x == nil {}
来源：http://qc.hnjuh.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://pd.szsharing.cn

C#:   if (x is null) {}
来源：http://kv.gzmigu.cn

[P07] 防抖与节流
来源：http://sg.gzmigu.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://gr.colortex.cn

PHP:  // 手写时间戳比较
来源：http://vx.newstarts.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://oq.muxihuayi.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ax.huanxung.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://gz.asd995.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://nk.panjiajie.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://kt.gzmigu.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://vs.szsharing.cn

[P08] 处理浮点精度问题
来源：http://dq.panjiajie.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://iq.huixinmuqiang.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://sj.chemitech.net.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ir.szsharing.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://pr.gzmigu.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://rh.shxzskj.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://vk.nszjky.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://sn.shtwfgs.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://pd.nicolike.cn

================================================================================
来源：http://lb.huixinmuqiang.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://jo.jctech888.com.cn

================================================================================
来源：http://jk.jctech888.com.cn

[Q01] 创建表
来源：http://mh.huanxung.cn

CREATE TABLE users (
来源：http://lf.lnxyls.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://iw.haigaiapp.cn

name VARCHAR(50) NOT NULL,
来源：http://bc.panjiajie.cn

email VARCHAR(100) UNIQUE,
来源：http://rn.asd995.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hw.nicolike.cn

);
来源：http://sc.nszjky.cn

[Q02] 创建带外键的表
来源：http://dz.hahajie.cn

CREATE TABLE orders (
来源：http://iu.jctech888.com.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://zs.yuntaijiaju.cn

user_id INT NOT NULL,
来源：http://ld.wgjwhj.cn

amount DECIMAL(10, 2),
来源：http://tq.newstarts.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ab.bjjhwx.cn

);
来源：http://rx.chemitech.net.cn

[Q03] 增加列
来源：http://hb.9csxet.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://qi.wgjwhj.cn

[Q04] 修改列类型
来源：http://aw.newstarts.cn


<!-- 参考信息 -->