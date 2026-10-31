代发 wailian999

JS:   process.exit(1)
来源：http://xf.hnjuh.cn

TS:   process.exit(1)
来源：http://em.jianghongdianzi.cn

Java: System.exit(1)
来源：http://ra.newstarts.cn

Go:   os.Exit(1)
来源：http://in.muxihuayi.cn

Ruby: exit 1
来源：http://sd.521024.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mw.newstarts.cn

[M06] 向标准错误输出
来源：http://qx.yuexingan06.cn

Py:   print("err", file=sys.stderr)
来源：http://oe.haigaiapp.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://yf.colortex.cn

JS:   console.error("err")
来源：http://wt.wgjwhj.cn

TS:   console.error("err")
来源：http://ko.huanxung.cn

Java: System.err.println("err")
来源：http://nj.shxzukj.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://pq.bookmarksfly.cn

Ruby: warn "err"
来源：http://xq.521024.cn

C#:   Console.Error.WriteLine("err")
来源：http://su.muxihuayi.cn

[M07] 判断是否为主入口
来源：http://aj.hnjuh.cn

Py:   if __name__ == "__main__":
来源：http://pt.521024.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://xw.szsharing.cn

JS:   require.main === module
来源：http://lc.yuexingan06.cn

TS:   require.main === module
来源：http://sr.jctech888.com.cn

Java: public static void main(String[] args)
来源：http://wa.asd995.cn

Go:   func main()
来源：http://xq.haigaiapp.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://oj.shxzskj.cn

C#:   static void Main(string[] args)
来源：http://oc.jianghongdianzi.cn

[M08] 获取系统与运行时信息
来源：http://ro.bjjhwx.cn

Py:   platform.system();  platform.python_version()
来源：http://es.newstarts.cn

PHP:  PHP_OS;  phpversion();
来源：http://ur.yuntaijiaju.cn

JS:   process.platform;  process.version
来源：http://bt.asd995.cn

TS:   process.platform;  process.version
来源：http://ic.shtwfgs.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://kd.shtwfgs.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://cf.gzmigu.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://sz.nicolike.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://si.9csxet.cn

================================================================================
来源：http://dl.521024.cn

N. 数据结构与算法
来源：http://jr.jianghongdianzi.cn

================================================================================
来源：http://js.gzmigu.cn

[N01] 二分查找（有序数组）
来源：http://fd.yuexingan06.cn

Py:   bisect.bisect_left(arr, x)
来源：http://et.panjiajie.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://nm.lnxyls.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ur.huixinmuqiang.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ky.colortex.cn

Java: Arrays.binarySearch(arr, x)
来源：http://nn.bjjhwx.cn

Go:   sort.SearchInts(arr, x)
来源：http://at.colortex.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://mq.9csxet.cn

C#:   Array.BinarySearch(arr, x)
来源：http://of.muxihuayi.cn

[N02] 排序（工程实践用内置实现）
来源：http://ji.yuntaijiaju.cn

Py:   sorted(arr);  arr.sort()
来源：http://qw.shxzukj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://zr.bjjhwx.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://rg.huixiangedu.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://dq.asd995.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://gd.huixinmuqiang.cn

Go:   slices.Sort(arr)
来源：http://oz.huixiangedu.cn

Ruby: arr.sort
来源：http://ph.bjjhwx.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://sy.shtwfgs.cn

[N03] 快速排序（分治示例）
来源：http://qa.huixiangedu.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://yd.jctech888.com.cn

PHP:  // 递归实现，或用 usort
来源：http://ig.nicolike.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qy.haigaiapp.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ku.jctech888.com.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://nh.panjiajie.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://sb.nszjky.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://rh.jctech888.com.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ij.lnxyls.cn

[N04] 斐波那契数列
来源：http://ve.newstarts.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://co.wgjwhj.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://sb.hnjuh.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hp.521024.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://va.szxytkj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://oo.szsharing.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wd.panjiajie.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ag.panjiajie.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ag.yuexingan06.cn

[N05] 最大公约数
来源：http://su.lnxyls.cn

Py:   math.gcd(a, b)
来源：http://cc.asd995.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://kb.panjiajie.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gv.szxytkj.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ze.huixinmuqiang.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ej.muxihuayi.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.bjjhwx.cn

Ruby: a.gcd(b)
来源：http://lt.nszjky.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://qc.szxytkj.cn

[N06] 判断回文字符串
来源：http://as.gzmigu.cn

Py:   s == s[::-1]
来源：http://ms.wgjwhj.cn

PHP:  $s === strrev($s);
来源：http://gd.huanxung.cn

JS:   s === [...s].reverse().join("")
来源：http://ag.huixiangedu.cn

TS:   s === [...s].reverse().join("")
来源：http://xy.chemitech.net.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://bf.shxzukj.cn

Go:   // 双指针从两端比较
来源：http://sr.newstarts.cn

Ruby: s == s.reverse
来源：http://qv.jctech888.com.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://wr.asd995.cn

[N07] 两数之和（返回下标）
来源：http://ua.9csxet.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://fc.hahajie.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://go.asd995.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://mg.521024.cn

TS:   // 手写 Map<string, number>
来源：http://mq.lnxyls.cn

Java: // 手写 HashMap
来源：http://dw.hnjuh.cn

Go:   // 手写 map[int]int
来源：http://os.hahajie.cn

Ruby: // 手写 Hash
来源：http://ym.shxzskj.cn

C#:   // 手写 Dictionary<int, int>
来源：http://he.9csxet.cn

[N08] 生成全排列
来源：http://pm.panjiajie.cn

Py:   itertools.permutations(arr)
来源：http://hv.nicolike.cn

PHP:  // 手写递归交换
来源：http://ga.9csxet.cn

JS:   // 手写回溯递归
来源：http://ih.huanxung.cn

TS:   // 手写回溯递归
来源：http://hs.yuexingan06.cn

Java: // 手写回溯递归
来源：http://sq.nszjky.cn

Go:   // 手写回溯递归
来源：http://yh.szxytkj.cn

Ruby: arr.permutation.to_a
来源：http://vf.huixinmuqiang.cn

C#:   // 手写回溯递归
来源：http://er.newstarts.cn

[N09] 栈与队列
来源：http://gk.yuexingan06.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://rm.jianghongdianzi.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://kn.huixiangedu.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ic.chemitech.net.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://gp.asd995.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://am.521024.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://cw.nicolike.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://gw.newstarts.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://cn.asd995.cn

[N10] 链表节点定义
来源：http://cv.chemitech.net.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://jk.newstarts.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://vo.wgjwhj.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wx.yuntaijiaju.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://nh.muxihuayi.cn

Java: class Node { int v; Node next; }
来源：http://qa.jianghongdianzi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://kv.nicolike.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://el.hahajie.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ed.szsharing.cn

[N11] 二叉树中序遍历
来源：http://ps.yuexingan06.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://av.szxytkj.cn

PHP:  // 手写递归函数
来源：http://rf.newstarts.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pl.chemitech.net.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fz.wgjwhj.cn

Java: // 手写递归
来源：http://ug.lnxyls.cn

Go:   // 手写递归
来源：http://wu.shtwfgs.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://xt.hnjuh.cn

C#:   // 手写递归
来源：http://wu.shtwfgs.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://db.jianghongdianzi.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ab.huanxung.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://lv.bookmarksfly.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dm.jctech888.com.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bk.hahajie.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://xo.chemitech.net.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://xk.wgjwhj.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://jz.asd995.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ab.gzmigu.cn

================================================================================
来源：http://zm.nicolike.cn

O. 并发与异步
来源：http://qb.nszjky.cn

================================================================================
来源：http://xa.colortex.cn

[O01] 启动一个线程
来源：http://bq.9csxet.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ep.chemitech.net.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ea.shxzskj.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://gq.szxytkj.cn

TS:   // 同 JS
来源：http://ps.gzmigu.cn

Java: new Thread(() -> f()).start()
来源：http://ko.huixiangedu.cn

Go:   go f()
来源：http://xj.chemitech.net.cn

Ruby: Thread.new { f }
来源：http://hk.chemitech.net.cn

C#:   Task.Run(() => F());
来源：http://fg.haigaiapp.cn

[O02] 使用线程池
来源：http://cy.hnjuh.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://xx.asd995.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ov.nszjky.cn

JS:   // worker_threads 线程池
来源：http://ul.colortex.cn

TS:   // worker_threads 线程池
来源：http://nd.gzmigu.cn

Java: Executors.newFixedThreadPool(4)
来源：http://nh.jctech888.com.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ss.hnjuh.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://av.jianghongdianzi.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://aj.lnxyls.cn

[O03] 加锁保护共享数据
来源：http://cm.521024.cn

Py:   with lock: shared += 1
来源：http://bu.szxytkj.cn

PHP:  // 用 flock() 做文件锁
来源：http://ez.yuntaijiaju.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://pp.jctech888.com.cn

TS:   // 同 JS
来源：http://sq.521024.cn

Java: synchronized (this) { shared++; }
来源：http://bv.521024.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://yr.chemitech.net.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://cj.huixiangedu.cn

C#:   lock (gate) { shared++; }
来源：http://md.lnxyls.cn

[O04] 定义异步函数并等待
来源：http://co.chemitech.net.cn

Py:   async def f():⏎    await g()
来源：http://bc.muxihuayi.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ek.newstarts.cn

JS:   async function f() { await g(); }
来源：http://lk.yuntaijiaju.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://wy.huixinmuqiang.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://as.szsharing.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://pz.muxihuayi.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ud.nicolike.cn

C#:   async Task F() { await G(); }
来源：http://ta.huixinmuqiang.cn

[O05] 并发执行并等待全部完成
来源：http://sn.wgjwhj.cn

Py:   asyncio.gather(*tasks)
来源：http://cp.huixiangedu.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mp.asd995.cn

JS:   await Promise.all(tasks)
来源：http://lo.hahajie.cn

TS:   await Promise.all(tasks)
来源：http://ns.panjiajie.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ft.wgjwhj.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://xd.huixiangedu.cn

Ruby: threads.map(&:join)
来源：http://zl.gzmigu.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ii.9csxet.cn

[O06] 使用进程池
来源：http://se.521024.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://cg.wgjwhj.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://dh.shtwfgs.cn

JS:   // child_process / cluster 模块
来源：http://bp.shxzskj.cn

TS:   // child_process / cluster 模块
来源：http://fc.jianghongdianzi.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://fj.wgjwhj.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://tr.colortex.cn

Ruby: // fork 块
来源：http://kg.gzmigu.cn

C#:   Parallel.For
来源：http://km.521024.cn

================================================================================
来源：http://mz.wgjwhj.cn

P. 常用工具函数
来源：http://mr.521024.cn

================================================================================
来源：http://ro.panjiajie.cn

[P01] 生成 UUID
来源：http://hx.asd995.cn

Py:   str(uuid.uuid4())
来源：http://cu.huixiangedu.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://gr.shtwfgs.cn

JS:   crypto.randomUUID()
来源：http://bv.bookmarksfly.cn

TS:   crypto.randomUUID()
来源：http://ur.panjiajie.cn

Java: UUID.randomUUID().toString()
来源：http://ef.panjiajie.cn

Go:   // 用 github.com/google/uuid
来源：http://aa.yuexingan06.cn

Ruby: SecureRandom.uuid
来源：http://xs.lnxyls.cn

C#:   Guid.NewGuid().ToString()
来源：http://xf.nicolike.cn

[P02] MD5 / SHA256 摘要
来源：http://cp.nszjky.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://bk.haigaiapp.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://yw.szsharing.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://kr.gzmigu.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://tc.huixinmuqiang.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://rv.szsharing.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://qz.bjjhwx.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mw.newstarts.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://or.shxzskj.cn

[P03] 生成短随机字符串
来源：http://ch.hnjuh.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ka.asd995.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://iy.szxytkj.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ta.szsharing.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wn.hnjuh.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://dv.yuexingan06.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://tj.yuexingan06.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ai.newstarts.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://jr.lnxyls.cn

[P04] 求长度
来源：http://ap.colortex.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ty.shtwfgs.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lc.9csxet.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://en.9csxet.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cw.yuntaijiaju.cn

Java: list.size();  map.size();  s.length()
来源：http://jq.asd995.cn

Go:   len(arr);  len(m)
来源：http://wp.panjiajie.cn

Ruby: x.length;  x.size
来源：http://ev.bookmarksfly.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://hv.newstarts.cn

[P05] 判断两个对象内容是否相等
来源：http://dg.panjiajie.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://uz.jianghongdianzi.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://md.haigaiapp.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://kv.huanxung.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://sz.hahajie.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://rt.colortex.cn

Go:   reflect.DeepEqual(a, b)
来源：http://hd.shtwfgs.cn

Ruby: a == b
来源：http://zj.szsharing.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://kl.asd995.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://yf.jctech888.com.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://le.gzmigu.cn

PHP:  if (empty($x)) {}
来源：http://tn.haigaiapp.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://oq.asd995.cn

TS:   if (x == null) {}
来源：http://mu.wgjwhj.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://px.yuntaijiaju.cn

Go:   if x == nil {}
来源：http://ax.shxzukj.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://da.521024.cn

C#:   if (x is null) {}
来源：http://bt.yuexingan06.cn

[P07] 防抖与节流
来源：http://as.szsharing.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://fk.hnjuh.cn

PHP:  // 手写时间戳比较
来源：http://vu.jctech888.com.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kz.szxytkj.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yl.gzmigu.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://sx.chemitech.net.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://am.shtwfgs.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://hf.shxzukj.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://dh.nszjky.cn

[P08] 处理浮点精度问题
来源：http://aw.hahajie.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://qh.muxihuayi.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://yr.yuntaijiaju.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ux.shxzukj.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ln.bookmarksfly.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ib.panjiajie.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://af.bjjhwx.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ru.jianghongdianzi.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ic.szxytkj.cn

================================================================================
来源：http://lt.colortex.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ez.shxzukj.cn

================================================================================
来源：http://zd.9csxet.cn

[Q01] 创建表
来源：http://uw.yuexingan06.cn

CREATE TABLE users (
来源：http://pp.szsharing.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://yv.szxytkj.cn

name VARCHAR(50) NOT NULL,
来源：http://iy.muxihuayi.cn

email VARCHAR(100) UNIQUE,
来源：http://rs.gzmigu.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://cb.newstarts.cn

);
来源：http://ie.shxzukj.cn

[Q02] 创建带外键的表
来源：http://pw.huixiangedu.cn

CREATE TABLE orders (
来源：http://lo.521024.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ew.shxzskj.cn

user_id INT NOT NULL,
来源：http://ny.haigaiapp.cn

amount DECIMAL(10, 2),
来源：http://sa.bookmarksfly.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ln.jianghongdianzi.cn

);
来源：http://jk.wgjwhj.cn

[Q03] 增加列
来源：http://gq.nszjky.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://lj.muxihuayi.cn

[Q04] 修改列类型
来源：http://rw.gzmigu.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ij.shxzskj.cn

[Q05] 重命名列
来源：http://ld.colortex.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ji.asd995.cn

[Q06] 删除列
来源：http://sg.hnjuh.cn


<!-- 参考信息 -->