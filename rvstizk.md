代发 wailian999

[M04] 获取当前工作目录
来源：http://uc.colortex.cn

Py:   os.getcwd()
来源：http://sv.asd995.cn

PHP:  getcwd();
来源：http://kv.szxytkj.cn

JS:   process.cwd()
来源：http://ya.muxihuayi.cn

TS:   process.cwd()
来源：http://jf.nszjky.cn

Java: Path.of("").toAbsolutePath()
来源：http://ff.szsharing.cn

Go:   os.Getwd()
来源：http://er.jctech888.com.cn

Ruby: Dir.pwd
来源：http://fg.nszjky.cn

C#:   Directory.GetCurrentDirectory()
来源：http://zg.panjiajie.cn

[M05] 设置退出码
来源：http://se.muxihuayi.cn

Py:   sys.exit(1)
来源：http://qn.haigaiapp.cn

PHP:  exit(1);
来源：http://if.colortex.cn

JS:   process.exit(1)
来源：http://rn.shxzskj.cn

TS:   process.exit(1)
来源：http://ke.shxzukj.cn

Java: System.exit(1)
来源：http://vq.hnjuh.cn

Go:   os.Exit(1)
来源：http://aq.huixinmuqiang.cn

Ruby: exit 1
来源：http://fh.szxytkj.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://am.bjjhwx.cn

[M06] 向标准错误输出
来源：http://ce.bookmarksfly.cn

Py:   print("err", file=sys.stderr)
来源：http://ob.9csxet.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://pj.haigaiapp.cn

JS:   console.error("err")
来源：http://kf.yuexingan06.cn

TS:   console.error("err")
来源：http://px.szxytkj.cn

Java: System.err.println("err")
来源：http://sj.521024.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://so.chemitech.net.cn

Ruby: warn "err"
来源：http://uq.yuexingan06.cn

C#:   Console.Error.WriteLine("err")
来源：http://tb.shxzukj.cn

[M07] 判断是否为主入口
来源：http://bm.chemitech.net.cn

Py:   if __name__ == "__main__":
来源：http://ze.szxytkj.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://qv.wgjwhj.cn

JS:   require.main === module
来源：http://ay.colortex.cn

TS:   require.main === module
来源：http://sa.wgjwhj.cn

Java: public static void main(String[] args)
来源：http://lo.shxzskj.cn

Go:   func main()
来源：http://re.nszjky.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://pz.newstarts.cn

C#:   static void Main(string[] args)
来源：http://cf.lnxyls.cn

[M08] 获取系统与运行时信息
来源：http://vn.lnxyls.cn

Py:   platform.system();  platform.python_version()
来源：http://ff.szxytkj.cn

PHP:  PHP_OS;  phpversion();
来源：http://nz.muxihuayi.cn

JS:   process.platform;  process.version
来源：http://xd.yuexingan06.cn

TS:   process.platform;  process.version
来源：http://so.szxytkj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://us.nicolike.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://kl.nicolike.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://kn.gzmigu.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://nf.hahajie.cn

================================================================================
来源：http://of.hnjuh.cn

N. 数据结构与算法
来源：http://fy.gzmigu.cn

================================================================================
来源：http://ni.asd995.cn

[N01] 二分查找（有序数组）
来源：http://ig.huanxung.cn

Py:   bisect.bisect_left(arr, x)
来源：http://rv.colortex.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hd.yuexingan06.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dv.shxzskj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ct.szsharing.cn

Java: Arrays.binarySearch(arr, x)
来源：http://wd.muxihuayi.cn

Go:   sort.SearchInts(arr, x)
来源：http://iq.wgjwhj.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://as.newstarts.cn

C#:   Array.BinarySearch(arr, x)
来源：http://di.haigaiapp.cn

[N02] 排序（工程实践用内置实现）
来源：http://ok.muxihuayi.cn

Py:   sorted(arr);  arr.sort()
来源：http://fs.wgjwhj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://sx.nicolike.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://mm.bookmarksfly.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://xw.huixiangedu.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wl.szxytkj.cn

Go:   slices.Sort(arr)
来源：http://wa.muxihuayi.cn

Ruby: arr.sort
来源：http://yb.bjjhwx.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://am.shtwfgs.cn

[N03] 快速排序（分治示例）
来源：http://uh.bookmarksfly.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://qe.9csxet.cn

PHP:  // 递归实现，或用 usort
来源：http://bb.nszjky.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fg.yuntaijiaju.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zr.shxzukj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hw.yuexingan06.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://jm.521024.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://rp.shxzskj.cn

C#:   // 手写递归，或 Array.Sort
来源：http://mv.colortex.cn

[N04] 斐波那契数列
来源：http://gf.szxytkj.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zn.colortex.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ac.9csxet.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pn.chemitech.net.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kv.nicolike.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://aa.chemitech.net.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://pp.asd995.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hg.hnjuh.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://eo.panjiajie.cn

[N05] 最大公约数
来源：http://ex.haigaiapp.cn

Py:   math.gcd(a, b)
来源：http://go.jctech888.com.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://pc.521024.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yy.shxzukj.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ri.chemitech.net.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://cp.shxzskj.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://rv.yuntaijiaju.cn

Ruby: a.gcd(b)
来源：http://bf.szsharing.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hn.shxzukj.cn

[N06] 判断回文字符串
来源：http://ie.jctech888.com.cn

Py:   s == s[::-1]
来源：http://hw.shxzskj.cn

PHP:  $s === strrev($s);
来源：http://wt.huixinmuqiang.cn

JS:   s === [...s].reverse().join("")
来源：http://ws.gzmigu.cn

TS:   s === [...s].reverse().join("")
来源：http://ke.yuntaijiaju.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://fo.521024.cn

Go:   // 双指针从两端比较
来源：http://fa.shtwfgs.cn

Ruby: s == s.reverse
来源：http://cq.chemitech.net.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://gy.jianghongdianzi.cn

[N07] 两数之和（返回下标）
来源：http://lm.wgjwhj.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://vr.panjiajie.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mb.jctech888.com.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://pu.nszjky.cn

TS:   // 手写 Map<string, number>
来源：http://jd.haigaiapp.cn

Java: // 手写 HashMap
来源：http://uw.huixinmuqiang.cn

Go:   // 手写 map[int]int
来源：http://qf.lnxyls.cn

Ruby: // 手写 Hash
来源：http://qv.hnjuh.cn

C#:   // 手写 Dictionary<int, int>
来源：http://oz.yuntaijiaju.cn

[N08] 生成全排列
来源：http://rp.gzmigu.cn

Py:   itertools.permutations(arr)
来源：http://yo.lnxyls.cn

PHP:  // 手写递归交换
来源：http://yh.shxzskj.cn

JS:   // 手写回溯递归
来源：http://wl.newstarts.cn

TS:   // 手写回溯递归
来源：http://he.yuexingan06.cn

Java: // 手写回溯递归
来源：http://ir.lnxyls.cn

Go:   // 手写回溯递归
来源：http://im.jianghongdianzi.cn

Ruby: arr.permutation.to_a
来源：http://zz.521024.cn

C#:   // 手写回溯递归
来源：http://bd.shxzskj.cn

[N09] 栈与队列
来源：http://yw.521024.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://jg.wgjwhj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://xk.huixinmuqiang.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://se.521024.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mc.huixiangedu.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://gl.gzmigu.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://cy.bookmarksfly.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wn.huixiangedu.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://bi.huixinmuqiang.cn

[N10] 链表节点定义
来源：http://ph.9csxet.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wp.panjiajie.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://il.asd995.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://lg.chemitech.net.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://eg.shxzukj.cn

Java: class Node { int v; Node next; }
来源：http://px.hnjuh.cn

Go:   type Node struct { V int; Next *Node }
来源：http://xf.yuexingan06.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://gs.lnxyls.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://zz.jianghongdianzi.cn

[N11] 二叉树中序遍历
来源：http://bc.jctech888.com.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://sg.haigaiapp.cn

PHP:  // 手写递归函数
来源：http://ib.szxytkj.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tb.huixiangedu.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dl.newstarts.cn

Java: // 手写递归
来源：http://px.colortex.cn

Go:   // 手写递归
来源：http://at.newstarts.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://pe.hnjuh.cn

C#:   // 手写递归
来源：http://st.521024.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ab.bjjhwx.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://xt.bookmarksfly.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://md.asd995.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lt.lnxyls.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://iw.szsharing.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://di.muxihuayi.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://cv.wgjwhj.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://gl.panjiajie.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://oy.bookmarksfly.cn

================================================================================
来源：http://hl.newstarts.cn

O. 并发与异步
来源：http://mf.panjiajie.cn

================================================================================
来源：http://ma.jctech888.com.cn

[O01] 启动一个线程
来源：http://vn.521024.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://tu.yuexingan06.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://te.haigaiapp.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://qr.yuntaijiaju.cn

TS:   // 同 JS
来源：http://xv.szxytkj.cn

Java: new Thread(() -> f()).start()
来源：http://ry.bookmarksfly.cn

Go:   go f()
来源：http://uq.wgjwhj.cn

Ruby: Thread.new { f }
来源：http://ev.bjjhwx.cn

C#:   Task.Run(() => F());
来源：http://ul.szsharing.cn

[O02] 使用线程池
来源：http://ih.haigaiapp.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://nq.lnxyls.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ve.bookmarksfly.cn

JS:   // worker_threads 线程池
来源：http://jz.yuexingan06.cn

TS:   // worker_threads 线程池
来源：http://il.gzmigu.cn

Java: Executors.newFixedThreadPool(4)
来源：http://eo.bjjhwx.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://zv.muxihuayi.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hs.9csxet.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mj.szxytkj.cn

[O03] 加锁保护共享数据
来源：http://jt.gzmigu.cn

Py:   with lock: shared += 1
来源：http://fk.asd995.cn

PHP:  // 用 flock() 做文件锁
来源：http://fc.colortex.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://xc.wgjwhj.cn

TS:   // 同 JS
来源：http://zt.chemitech.net.cn

Java: synchronized (this) { shared++; }
来源：http://yq.huixiangedu.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://jc.szsharing.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://aw.szsharing.cn

C#:   lock (gate) { shared++; }
来源：http://lb.521024.cn

[O04] 定义异步函数并等待
来源：http://do.haigaiapp.cn

Py:   async def f():⏎    await g()
来源：http://bj.jianghongdianzi.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://jb.newstarts.cn

JS:   async function f() { await g(); }
来源：http://rm.colortex.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://wn.asd995.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wt.shtwfgs.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://dp.nszjky.cn

Ruby: # 用 Fiber 或 async gem
来源：http://iz.521024.cn

C#:   async Task F() { await G(); }
来源：http://yr.shxzskj.cn

[O05] 并发执行并等待全部完成
来源：http://yj.huanxung.cn

Py:   asyncio.gather(*tasks)
来源：http://wy.shxzukj.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://zg.chemitech.net.cn

JS:   await Promise.all(tasks)
来源：http://co.haigaiapp.cn

TS:   await Promise.all(tasks)
来源：http://xz.9csxet.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://uf.hahajie.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wi.chemitech.net.cn

Ruby: threads.map(&:join)
来源：http://vn.huixiangedu.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://vz.muxihuayi.cn

[O06] 使用进程池
来源：http://jc.panjiajie.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://lw.bookmarksfly.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://li.shtwfgs.cn

JS:   // child_process / cluster 模块
来源：http://bc.jianghongdianzi.cn

TS:   // child_process / cluster 模块
来源：http://ye.shxzukj.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ua.nszjky.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://xj.jianghongdianzi.cn

Ruby: // fork 块
来源：http://zz.haigaiapp.cn

C#:   Parallel.For
来源：http://rp.yuexingan06.cn

================================================================================
来源：http://vy.hnjuh.cn

P. 常用工具函数
来源：http://tz.hnjuh.cn

================================================================================
来源：http://lz.yuexingan06.cn

[P01] 生成 UUID
来源：http://ib.yuexingan06.cn

Py:   str(uuid.uuid4())
来源：http://mk.nicolike.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ur.asd995.cn

JS:   crypto.randomUUID()
来源：http://le.panjiajie.cn

TS:   crypto.randomUUID()
来源：http://qj.haigaiapp.cn

Java: UUID.randomUUID().toString()
来源：http://ab.szsharing.cn

Go:   // 用 github.com/google/uuid
来源：http://sb.shtwfgs.cn

Ruby: SecureRandom.uuid
来源：http://wb.panjiajie.cn

C#:   Guid.NewGuid().ToString()
来源：http://vs.shxzukj.cn

[P02] MD5 / SHA256 摘要
来源：http://vj.szxytkj.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://nw.shxzukj.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://gs.nszjky.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://su.9csxet.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wm.521024.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://om.asd995.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://op.nszjky.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://yu.chemitech.net.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://jy.521024.cn

[P03] 生成短随机字符串
来源：http://uu.yuexingan06.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://vk.huixinmuqiang.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wy.hnjuh.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ri.jctech888.com.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mk.yuntaijiaju.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://xc.colortex.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://pm.9csxet.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://yz.wgjwhj.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://gb.hnjuh.cn

[P04] 求长度
来源：http://lh.huanxung.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://tp.yuntaijiaju.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ei.szxytkj.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ut.hnjuh.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://na.jctech888.com.cn

Java: list.size();  map.size();  s.length()
来源：http://zs.yuntaijiaju.cn

Go:   len(arr);  len(m)
来源：http://rn.jianghongdianzi.cn

Ruby: x.length;  x.size
来源：http://wk.hnjuh.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ci.huixinmuqiang.cn

[P05] 判断两个对象内容是否相等
来源：http://tc.gzmigu.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://qg.huixinmuqiang.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://gb.nicolike.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://jd.shtwfgs.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://di.szxytkj.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://uv.colortex.cn

Go:   reflect.DeepEqual(a, b)
来源：http://du.szxytkj.cn

Ruby: a == b
来源：http://px.bjjhwx.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://je.huixiangedu.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mt.asd995.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ff.haigaiapp.cn

PHP:  if (empty($x)) {}
来源：http://qj.szxytkj.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://gy.asd995.cn

TS:   if (x == null) {}
来源：http://th.nicolike.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://tn.huixiangedu.cn

Go:   if x == nil {}
来源：http://jv.shtwfgs.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://cz.nszjky.cn

C#:   if (x is null) {}
来源：http://nf.wgjwhj.cn

[P07] 防抖与节流
来源：http://yp.asd995.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://jj.shtwfgs.cn

PHP:  // 手写时间戳比较
来源：http://kj.shxzukj.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nh.shxzukj.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fe.shxzskj.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ii.yuntaijiaju.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://fy.yuntaijiaju.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://xp.yuntaijiaju.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://df.9csxet.cn

[P08] 处理浮点精度问题
来源：http://pf.bookmarksfly.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://op.shxzskj.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ml.huixiangedu.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://vx.9csxet.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://kv.asd995.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://du.muxihuayi.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://dn.huixinmuqiang.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ld.wgjwhj.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ao.9csxet.cn

================================================================================
来源：http://wb.huixiangedu.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://rn.yuntaijiaju.cn

================================================================================
来源：http://ia.yuntaijiaju.cn

[Q01] 创建表
来源：http://qw.shxzskj.cn

CREATE TABLE users (
来源：http://wz.bjjhwx.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://jn.colortex.cn

name VARCHAR(50) NOT NULL,
来源：http://ix.nszjky.cn

email VARCHAR(100) UNIQUE,
来源：http://cl.lnxyls.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://rf.hnjuh.cn

);
来源：http://fj.wgjwhj.cn

[Q02] 创建带外键的表
来源：http://bh.hnjuh.cn

CREATE TABLE orders (
来源：http://ud.yuntaijiaju.cn


<!-- 参考信息 -->