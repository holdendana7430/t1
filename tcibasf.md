代发 wailian999

JS:   process.exit(1)
来源：http://ct.panjiajie.cn

TS:   process.exit(1)
来源：http://qm.lnxyls.cn

Java: System.exit(1)
来源：http://qf.yuntaijiaju.cn

Go:   os.Exit(1)
来源：http://ss.bookmarksfly.cn

Ruby: exit 1
来源：http://up.gzmigu.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://fb.yuexingan06.cn

[M06] 向标准错误输出
来源：http://ny.shtwfgs.cn

Py:   print("err", file=sys.stderr)
来源：http://fy.hnjuh.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://mh.newstarts.cn

JS:   console.error("err")
来源：http://yj.szxytkj.cn

TS:   console.error("err")
来源：http://xy.nszjky.cn

Java: System.err.println("err")
来源：http://ct.nicolike.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://fw.shxzukj.cn

Ruby: warn "err"
来源：http://zk.shxzskj.cn

C#:   Console.Error.WriteLine("err")
来源：http://tz.huixiangedu.cn

[M07] 判断是否为主入口
来源：http://qu.colortex.cn

Py:   if __name__ == "__main__":
来源：http://uu.shxzukj.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wk.nszjky.cn

JS:   require.main === module
来源：http://xt.asd995.cn

TS:   require.main === module
来源：http://zk.jianghongdianzi.cn

Java: public static void main(String[] args)
来源：http://yk.wgjwhj.cn

Go:   func main()
来源：http://yp.yuexingan06.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://sw.huixiangedu.cn

C#:   static void Main(string[] args)
来源：http://rw.9csxet.cn

[M08] 获取系统与运行时信息
来源：http://cb.shxzskj.cn

Py:   platform.system();  platform.python_version()
来源：http://uj.huixiangedu.cn

PHP:  PHP_OS;  phpversion();
来源：http://yz.hahajie.cn

JS:   process.platform;  process.version
来源：http://lc.shtwfgs.cn

TS:   process.platform;  process.version
来源：http://rn.jctech888.com.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hu.bjjhwx.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://fk.gzmigu.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://jz.huixiangedu.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://cx.521024.cn

================================================================================
来源：http://kb.yuntaijiaju.cn

N. 数据结构与算法
来源：http://lj.bjjhwx.cn

================================================================================
来源：http://vx.lnxyls.cn

[N01] 二分查找（有序数组）
来源：http://bd.huixinmuqiang.cn

Py:   bisect.bisect_left(arr, x)
来源：http://zf.shxzukj.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://dc.521024.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fb.wgjwhj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qf.lnxyls.cn

Java: Arrays.binarySearch(arr, x)
来源：http://so.jctech888.com.cn

Go:   sort.SearchInts(arr, x)
来源：http://qs.newstarts.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://jl.jctech888.com.cn

C#:   Array.BinarySearch(arr, x)
来源：http://mp.bjjhwx.cn

[N02] 排序（工程实践用内置实现）
来源：http://dv.gzmigu.cn

Py:   sorted(arr);  arr.sort()
来源：http://bh.hnjuh.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ao.nszjky.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://bv.jctech888.com.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://fd.panjiajie.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://tl.chemitech.net.cn

Go:   slices.Sort(arr)
来源：http://rk.huanxung.cn

Ruby: arr.sort
来源：http://sa.521024.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://vw.jianghongdianzi.cn

[N03] 快速排序（分治示例）
来源：http://yu.yuntaijiaju.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ub.muxihuayi.cn

PHP:  // 递归实现，或用 usort
来源：http://fz.huanxung.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://my.szxytkj.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lq.newstarts.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mv.hahajie.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ck.nszjky.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://cl.shtwfgs.cn

C#:   // 手写递归，或 Array.Sort
来源：http://gd.gzmigu.cn

[N04] 斐波那契数列
来源：http://vh.newstarts.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://fk.huixinmuqiang.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://kr.bjjhwx.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zm.lnxyls.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fd.yuexingan06.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://gk.shxzukj.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://lj.wgjwhj.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://qt.gzmigu.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://oe.bookmarksfly.cn

[N05] 最大公约数
来源：http://ht.gzmigu.cn

Py:   math.gcd(a, b)
来源：http://nv.huixinmuqiang.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://kf.asd995.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vg.9csxet.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://im.gzmigu.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://dh.szsharing.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mh.nszjky.cn

Ruby: a.gcd(b)
来源：http://ha.shxzskj.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://vs.shtwfgs.cn

[N06] 判断回文字符串
来源：http://mj.szsharing.cn

Py:   s == s[::-1]
来源：http://vh.shxzukj.cn

PHP:  $s === strrev($s);
来源：http://ai.jianghongdianzi.cn

JS:   s === [...s].reverse().join("")
来源：http://mq.yuntaijiaju.cn

TS:   s === [...s].reverse().join("")
来源：http://jh.colortex.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://dw.szxytkj.cn

Go:   // 双指针从两端比较
来源：http://yu.jctech888.com.cn

Ruby: s == s.reverse
来源：http://mc.lnxyls.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://tl.9csxet.cn

[N07] 两数之和（返回下标）
来源：http://jl.szsharing.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mg.hnjuh.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ut.shxzukj.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://fe.gzmigu.cn

TS:   // 手写 Map<string, number>
来源：http://cr.colortex.cn

Java: // 手写 HashMap
来源：http://jg.shxzskj.cn

Go:   // 手写 map[int]int
来源：http://nw.colortex.cn

Ruby: // 手写 Hash
来源：http://sk.shxzukj.cn

C#:   // 手写 Dictionary<int, int>
来源：http://sv.colortex.cn

[N08] 生成全排列
来源：http://uc.asd995.cn

Py:   itertools.permutations(arr)
来源：http://kr.shtwfgs.cn

PHP:  // 手写递归交换
来源：http://ma.shtwfgs.cn

JS:   // 手写回溯递归
来源：http://uo.yuexingan06.cn

TS:   // 手写回溯递归
来源：http://jh.nicolike.cn

Java: // 手写回溯递归
来源：http://yf.jctech888.com.cn

Go:   // 手写回溯递归
来源：http://gf.hahajie.cn

Ruby: arr.permutation.to_a
来源：http://lt.shxzukj.cn

C#:   // 手写回溯递归
来源：http://yo.shxzskj.cn

[N09] 栈与队列
来源：http://kq.521024.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://xk.yuexingan06.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://cp.panjiajie.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://og.szsharing.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://sn.shxzukj.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mz.hahajie.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://gj.521024.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://kk.nicolike.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://su.huixiangedu.cn

[N10] 链表节点定义
来源：http://mz.nszjky.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qb.huanxung.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ub.muxihuayi.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ma.9csxet.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://zn.jianghongdianzi.cn

Java: class Node { int v; Node next; }
来源：http://ai.haigaiapp.cn

Go:   type Node struct { V int; Next *Node }
来源：http://yr.szxytkj.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://fo.muxihuayi.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://hp.huanxung.cn

[N11] 二叉树中序遍历
来源：http://gs.hnjuh.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://so.hahajie.cn

PHP:  // 手写递归函数
来源：http://eh.nicolike.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hd.huixiangedu.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qt.jctech888.com.cn

Java: // 手写递归
来源：http://oh.shxzskj.cn

Go:   // 手写递归
来源：http://kc.huixiangedu.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://bg.shxzukj.cn

C#:   // 手写递归
来源：http://ib.bookmarksfly.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://li.shtwfgs.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://fi.521024.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://uf.huixinmuqiang.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ae.jctech888.com.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ef.bookmarksfly.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ul.huixiangedu.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://kt.yuexingan06.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://sq.newstarts.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://th.colortex.cn

================================================================================
来源：http://jf.9csxet.cn

O. 并发与异步
来源：http://jc.hnjuh.cn

================================================================================
来源：http://jk.521024.cn

[O01] 启动一个线程
来源：http://rl.huanxung.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://qw.hahajie.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://jc.bjjhwx.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://eo.shxzskj.cn

TS:   // 同 JS
来源：http://rz.9csxet.cn

Java: new Thread(() -> f()).start()
来源：http://zr.szsharing.cn

Go:   go f()
来源：http://kw.newstarts.cn

Ruby: Thread.new { f }
来源：http://lr.haigaiapp.cn

C#:   Task.Run(() => F());
来源：http://yo.bookmarksfly.cn

[O02] 使用线程池
来源：http://lh.nicolike.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://tl.colortex.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mr.bjjhwx.cn

JS:   // worker_threads 线程池
来源：http://hy.bjjhwx.cn

TS:   // worker_threads 线程池
来源：http://cd.yuexingan06.cn

Java: Executors.newFixedThreadPool(4)
来源：http://av.szsharing.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://fs.huixiangedu.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://vh.yuntaijiaju.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://og.hahajie.cn

[O03] 加锁保护共享数据
来源：http://ru.haigaiapp.cn

Py:   with lock: shared += 1
来源：http://nt.panjiajie.cn

PHP:  // 用 flock() 做文件锁
来源：http://um.huixinmuqiang.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://xd.muxihuayi.cn

TS:   // 同 JS
来源：http://bc.szsharing.cn

Java: synchronized (this) { shared++; }
来源：http://cg.nicolike.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://nz.wgjwhj.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ys.huixinmuqiang.cn

C#:   lock (gate) { shared++; }
来源：http://ro.hnjuh.cn

[O04] 定义异步函数并等待
来源：http://ii.shxzskj.cn

Py:   async def f():⏎    await g()
来源：http://km.chemitech.net.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://nd.nszjky.cn

JS:   async function f() { await g(); }
来源：http://qq.panjiajie.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ci.hahajie.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://lp.panjiajie.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ce.chemitech.net.cn

Ruby: # 用 Fiber 或 async gem
来源：http://bf.panjiajie.cn

C#:   async Task F() { await G(); }
来源：http://dn.huixinmuqiang.cn

[O05] 并发执行并等待全部完成
来源：http://kr.huixiangedu.cn

Py:   asyncio.gather(*tasks)
来源：http://vo.newstarts.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://lx.yuexingan06.cn

JS:   await Promise.all(tasks)
来源：http://me.haigaiapp.cn

TS:   await Promise.all(tasks)
来源：http://jo.yuexingan06.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://bv.shxzukj.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://lf.521024.cn

Ruby: threads.map(&:join)
来源：http://nt.521024.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://tr.9csxet.cn

[O06] 使用进程池
来源：http://df.huanxung.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://tc.asd995.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://kz.hahajie.cn

JS:   // child_process / cluster 模块
来源：http://bo.shxzskj.cn

TS:   // child_process / cluster 模块
来源：http://io.colortex.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://rv.lnxyls.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://tb.szsharing.cn

Ruby: // fork 块
来源：http://fd.shxzukj.cn

C#:   Parallel.For
来源：http://ig.huixinmuqiang.cn

================================================================================
来源：http://ul.colortex.cn

P. 常用工具函数
来源：http://jo.521024.cn

================================================================================
来源：http://vi.panjiajie.cn

[P01] 生成 UUID
来源：http://wj.szsharing.cn

Py:   str(uuid.uuid4())
来源：http://tp.jianghongdianzi.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://tw.chemitech.net.cn

JS:   crypto.randomUUID()
来源：http://bi.hahajie.cn

TS:   crypto.randomUUID()
来源：http://rd.panjiajie.cn

Java: UUID.randomUUID().toString()
来源：http://wu.huanxung.cn

Go:   // 用 github.com/google/uuid
来源：http://dh.lnxyls.cn

Ruby: SecureRandom.uuid
来源：http://cu.szsharing.cn

C#:   Guid.NewGuid().ToString()
来源：http://wc.colortex.cn

[P02] MD5 / SHA256 摘要
来源：http://gh.panjiajie.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ui.huixinmuqiang.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://sy.wgjwhj.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://kc.shxzskj.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://fu.jctech888.com.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://na.huixiangedu.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wc.hnjuh.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://tb.shtwfgs.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://tx.newstarts.cn

[P03] 生成短随机字符串
来源：http://eu.jianghongdianzi.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://bk.9csxet.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://qr.chemitech.net.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hu.yuexingan06.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yt.shxzskj.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ri.huixinmuqiang.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://bk.9csxet.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://qs.szxytkj.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://qw.yuntaijiaju.cn

[P04] 求长度
来源：http://dz.shxzukj.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://an.asd995.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cr.bjjhwx.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fs.lnxyls.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://km.chemitech.net.cn

Java: list.size();  map.size();  s.length()
来源：http://hm.huixinmuqiang.cn

Go:   len(arr);  len(m)
来源：http://gv.newstarts.cn

Ruby: x.length;  x.size
来源：http://mt.haigaiapp.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://jd.yuexingan06.cn

[P05] 判断两个对象内容是否相等
来源：http://iu.szsharing.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://jh.colortex.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://dg.huixinmuqiang.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://fl.shxzskj.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://rm.asd995.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://lm.nszjky.cn

Go:   reflect.DeepEqual(a, b)
来源：http://uk.szsharing.cn

Ruby: a == b
来源：http://ki.jctech888.com.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://cw.521024.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hc.szsharing.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://lr.haigaiapp.cn

PHP:  if (empty($x)) {}
来源：http://cs.chemitech.net.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://cz.shtwfgs.cn

TS:   if (x == null) {}
来源：http://os.huixinmuqiang.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://gj.asd995.cn

Go:   if x == nil {}
来源：http://yv.521024.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://pq.bookmarksfly.cn

C#:   if (x is null) {}
来源：http://bz.szxytkj.cn

[P07] 防抖与节流
来源：http://zy.nicolike.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://yy.szxytkj.cn

PHP:  // 手写时间戳比较
来源：http://ho.huanxung.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ar.huixinmuqiang.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hy.szxytkj.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://pb.asd995.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://sy.asd995.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://zm.szsharing.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mz.asd995.cn

[P08] 处理浮点精度问题
来源：http://il.shxzskj.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hy.bookmarksfly.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://so.gzmigu.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://dy.gzmigu.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://xe.szsharing.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hu.yuexingan06.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://cq.asd995.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://yi.nszjky.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://sm.haigaiapp.cn

================================================================================
来源：http://gt.bookmarksfly.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ii.bjjhwx.cn

================================================================================
来源：http://aj.huixinmuqiang.cn

[Q01] 创建表
来源：http://zu.hahajie.cn

CREATE TABLE users (
来源：http://tp.nicolike.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://nj.9csxet.cn

name VARCHAR(50) NOT NULL,
来源：http://gj.muxihuayi.cn

email VARCHAR(100) UNIQUE,
来源：http://di.panjiajie.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ts.lnxyls.cn

);
来源：http://og.newstarts.cn

[Q02] 创建带外键的表
来源：http://by.9csxet.cn

CREATE TABLE orders (
来源：http://vp.nszjky.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://zq.hahajie.cn

user_id INT NOT NULL,
来源：http://ji.hnjuh.cn

amount DECIMAL(10, 2),
来源：http://yg.hahajie.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://xo.nszjky.cn

);
来源：http://qe.bjjhwx.cn

[Q03] 增加列
来源：http://nr.szsharing.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://yk.nszjky.cn

[Q04] 修改列类型
来源：http://up.newstarts.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://uh.gzmigu.cn

[Q05] 重命名列
来源：http://de.hahajie.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ji.bjjhwx.cn

[Q06] 删除列
来源：http://ph.9csxet.cn


<!-- 参考信息 -->