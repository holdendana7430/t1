代发 wailian999

TS:   process.cwd()
来源：http://zl.nszjky.cn

Java: Path.of("").toAbsolutePath()
来源：http://xf.jianghongdianzi.cn

Go:   os.Getwd()
来源：http://fc.huixinmuqiang.cn

Ruby: Dir.pwd
来源：http://zy.shxzukj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ni.jctech888.com.cn

[M05] 设置退出码
来源：http://cb.wgjwhj.cn

Py:   sys.exit(1)
来源：http://pm.colortex.cn

PHP:  exit(1);
来源：http://ni.huixiangedu.cn

JS:   process.exit(1)
来源：http://hb.newstarts.cn

TS:   process.exit(1)
来源：http://gs.jianghongdianzi.cn

Java: System.exit(1)
来源：http://zv.lnxyls.cn

Go:   os.Exit(1)
来源：http://ay.huanxung.cn

Ruby: exit 1
来源：http://bc.chemitech.net.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://xg.colortex.cn

[M06] 向标准错误输出
来源：http://kv.nszjky.cn

Py:   print("err", file=sys.stderr)
来源：http://hi.nszjky.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://wn.panjiajie.cn

JS:   console.error("err")
来源：http://mr.nszjky.cn

TS:   console.error("err")
来源：http://yt.lnxyls.cn

Java: System.err.println("err")
来源：http://bj.szxytkj.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://bk.shxzskj.cn

Ruby: warn "err"
来源：http://xk.colortex.cn

C#:   Console.Error.WriteLine("err")
来源：http://cu.shtwfgs.cn

[M07] 判断是否为主入口
来源：http://at.nszjky.cn

Py:   if __name__ == "__main__":
来源：http://eo.wgjwhj.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ap.yuntaijiaju.cn

JS:   require.main === module
来源：http://gj.shxzukj.cn

TS:   require.main === module
来源：http://qm.jianghongdianzi.cn

Java: public static void main(String[] args)
来源：http://bx.521024.cn

Go:   func main()
来源：http://nm.nicolike.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ry.shtwfgs.cn

C#:   static void Main(string[] args)
来源：http://cy.yuntaijiaju.cn

[M08] 获取系统与运行时信息
来源：http://fa.newstarts.cn

Py:   platform.system();  platform.python_version()
来源：http://qi.hnjuh.cn

PHP:  PHP_OS;  phpversion();
来源：http://ot.szsharing.cn

JS:   process.platform;  process.version
来源：http://fo.szsharing.cn

TS:   process.platform;  process.version
来源：http://vh.9csxet.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://tw.9csxet.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://mi.jianghongdianzi.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://oa.newstarts.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://xo.yuexingan06.cn

================================================================================
来源：http://ot.haigaiapp.cn

N. 数据结构与算法
来源：http://lz.panjiajie.cn

================================================================================
来源：http://ra.huixinmuqiang.cn

[N01] 二分查找（有序数组）
来源：http://il.bjjhwx.cn

Py:   bisect.bisect_left(arr, x)
来源：http://bj.hnjuh.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://sm.lnxyls.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://oz.szsharing.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hl.lnxyls.cn

Java: Arrays.binarySearch(arr, x)
来源：http://uu.yuntaijiaju.cn

Go:   sort.SearchInts(arr, x)
来源：http://al.shtwfgs.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://te.hnjuh.cn

C#:   Array.BinarySearch(arr, x)
来源：http://co.nszjky.cn

[N02] 排序（工程实践用内置实现）
来源：http://wn.huixinmuqiang.cn

Py:   sorted(arr);  arr.sort()
来源：http://sh.yuntaijiaju.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://st.chemitech.net.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://fg.szsharing.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ax.chemitech.net.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://jc.muxihuayi.cn

Go:   slices.Sort(arr)
来源：http://eq.asd995.cn

Ruby: arr.sort
来源：http://zi.shxzskj.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://jn.shtwfgs.cn

[N03] 快速排序（分治示例）
来源：http://yd.yuexingan06.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://tk.hnjuh.cn

PHP:  // 递归实现，或用 usort
来源：http://hq.yuexingan06.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zl.yuexingan06.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cw.chemitech.net.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://yu.haigaiapp.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://gu.panjiajie.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://fr.panjiajie.cn

C#:   // 手写递归，或 Array.Sort
来源：http://cu.panjiajie.cn

[N04] 斐波那契数列
来源：http://fl.szxytkj.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://lw.hnjuh.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://am.bjjhwx.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ei.bookmarksfly.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ck.nicolike.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ap.wgjwhj.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ir.nicolike.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://rk.hahajie.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://qd.colortex.cn

[N05] 最大公约数
来源：http://xb.lnxyls.cn

Py:   math.gcd(a, b)
来源：http://zj.jianghongdianzi.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://lk.huixinmuqiang.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://os.wgjwhj.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vp.chemitech.net.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://lm.huixiangedu.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://gj.hahajie.cn

Ruby: a.gcd(b)
来源：http://wa.huanxung.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://zm.lnxyls.cn

[N06] 判断回文字符串
来源：http://fy.panjiajie.cn

Py:   s == s[::-1]
来源：http://bm.lnxyls.cn

PHP:  $s === strrev($s);
来源：http://mh.yuexingan06.cn

JS:   s === [...s].reverse().join("")
来源：http://bt.hnjuh.cn

TS:   s === [...s].reverse().join("")
来源：http://wr.shxzukj.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ym.521024.cn

Go:   // 双指针从两端比较
来源：http://vo.wgjwhj.cn

Ruby: s == s.reverse
来源：http://sd.9csxet.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://tb.shtwfgs.cn

[N07] 两数之和（返回下标）
来源：http://lo.shxzskj.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://tz.yuexingan06.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://bw.nicolike.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://vq.nszjky.cn

TS:   // 手写 Map<string, number>
来源：http://ma.szxytkj.cn

Java: // 手写 HashMap
来源：http://dw.bookmarksfly.cn

Go:   // 手写 map[int]int
来源：http://ih.chemitech.net.cn

Ruby: // 手写 Hash
来源：http://qp.gzmigu.cn

C#:   // 手写 Dictionary<int, int>
来源：http://bl.panjiajie.cn

[N08] 生成全排列
来源：http://sx.yuexingan06.cn

Py:   itertools.permutations(arr)
来源：http://uc.yuntaijiaju.cn

PHP:  // 手写递归交换
来源：http://lq.gzmigu.cn

JS:   // 手写回溯递归
来源：http://mz.muxihuayi.cn

TS:   // 手写回溯递归
来源：http://zd.jctech888.com.cn

Java: // 手写回溯递归
来源：http://ht.yuntaijiaju.cn

Go:   // 手写回溯递归
来源：http://sf.huixinmuqiang.cn

Ruby: arr.permutation.to_a
来源：http://ff.shxzukj.cn

C#:   // 手写回溯递归
来源：http://ug.jctech888.com.cn

[N09] 栈与队列
来源：http://oj.szsharing.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ed.shxzskj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ir.9csxet.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://kg.hahajie.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://tt.colortex.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://rh.muxihuayi.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://yh.bjjhwx.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://gm.hahajie.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wd.colortex.cn

[N10] 链表节点定义
来源：http://dd.wgjwhj.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://tx.bjjhwx.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://qw.shxzukj.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://vc.shxzskj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://za.shxzskj.cn

Java: class Node { int v; Node next; }
来源：http://zv.yuntaijiaju.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ja.chemitech.net.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://jv.muxihuayi.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://mt.shxzukj.cn

[N11] 二叉树中序遍历
来源：http://sb.colortex.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://rs.bjjhwx.cn

PHP:  // 手写递归函数
来源：http://xp.haigaiapp.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://in.yuntaijiaju.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dv.asd995.cn

Java: // 手写递归
来源：http://us.hnjuh.cn

Go:   // 手写递归
来源：http://mc.shxzukj.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://nr.521024.cn

C#:   // 手写递归
来源：http://kw.haigaiapp.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://tb.shxzskj.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hw.9csxet.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://pd.asd995.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://it.bjjhwx.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://da.chemitech.net.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ev.shxzukj.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://id.huanxung.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://nn.shxzukj.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://bt.asd995.cn

================================================================================
来源：http://zn.newstarts.cn

O. 并发与异步
来源：http://td.huanxung.cn

================================================================================
来源：http://vi.shtwfgs.cn

[O01] 启动一个线程
来源：http://xu.szsharing.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ng.huixiangedu.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://vi.hahajie.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://dk.yuntaijiaju.cn

TS:   // 同 JS
来源：http://ym.asd995.cn

Java: new Thread(() -> f()).start()
来源：http://su.szxytkj.cn

Go:   go f()
来源：http://vb.huanxung.cn

Ruby: Thread.new { f }
来源：http://sg.bookmarksfly.cn

C#:   Task.Run(() => F());
来源：http://uj.jctech888.com.cn

[O02] 使用线程池
来源：http://cr.hahajie.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://rz.jctech888.com.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ov.yuexingan06.cn

JS:   // worker_threads 线程池
来源：http://pk.huixinmuqiang.cn

TS:   // worker_threads 线程池
来源：http://wg.colortex.cn

Java: Executors.newFixedThreadPool(4)
来源：http://dw.chemitech.net.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wk.huixiangedu.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://oa.wgjwhj.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ln.wgjwhj.cn

[O03] 加锁保护共享数据
来源：http://wx.chemitech.net.cn

Py:   with lock: shared += 1
来源：http://iw.muxihuayi.cn

PHP:  // 用 flock() 做文件锁
来源：http://me.shtwfgs.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ij.9csxet.cn

TS:   // 同 JS
来源：http://pb.newstarts.cn

Java: synchronized (this) { shared++; }
来源：http://rt.huixinmuqiang.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ne.wgjwhj.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://en.shxzskj.cn

C#:   lock (gate) { shared++; }
来源：http://pv.huixinmuqiang.cn

[O04] 定义异步函数并等待
来源：http://kd.gzmigu.cn

Py:   async def f():⏎    await g()
来源：http://ib.haigaiapp.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://tf.521024.cn

JS:   async function f() { await g(); }
来源：http://aq.yuntaijiaju.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ci.shxzskj.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ew.hnjuh.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://lz.lnxyls.cn

Ruby: # 用 Fiber 或 async gem
来源：http://fj.yuntaijiaju.cn

C#:   async Task F() { await G(); }
来源：http://ng.muxihuayi.cn

[O05] 并发执行并等待全部完成
来源：http://ef.jianghongdianzi.cn

Py:   asyncio.gather(*tasks)
来源：http://gy.szsharing.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://nt.shxzukj.cn

JS:   await Promise.all(tasks)
来源：http://yy.chemitech.net.cn

TS:   await Promise.all(tasks)
来源：http://ws.chemitech.net.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ha.szxytkj.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://pv.szsharing.cn

Ruby: threads.map(&:join)
来源：http://lc.colortex.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ps.bookmarksfly.cn

[O06] 使用进程池
来源：http://kc.yuexingan06.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://pj.bjjhwx.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://tw.newstarts.cn

JS:   // child_process / cluster 模块
来源：http://px.colortex.cn

TS:   // child_process / cluster 模块
来源：http://wo.nszjky.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://yh.hnjuh.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://by.nszjky.cn

Ruby: // fork 块
来源：http://ac.wgjwhj.cn

C#:   Parallel.For
来源：http://ne.yuexingan06.cn

================================================================================
来源：http://ll.muxihuayi.cn

P. 常用工具函数
来源：http://ej.huanxung.cn

================================================================================
来源：http://yq.yuexingan06.cn

[P01] 生成 UUID
来源：http://pg.yuntaijiaju.cn

Py:   str(uuid.uuid4())
来源：http://he.bjjhwx.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://tl.jctech888.com.cn

JS:   crypto.randomUUID()
来源：http://sc.huixinmuqiang.cn

TS:   crypto.randomUUID()
来源：http://ez.szxytkj.cn

Java: UUID.randomUUID().toString()
来源：http://wq.9csxet.cn

Go:   // 用 github.com/google/uuid
来源：http://wi.shxzukj.cn

Ruby: SecureRandom.uuid
来源：http://ff.muxihuayi.cn

C#:   Guid.NewGuid().ToString()
来源：http://sb.hahajie.cn

[P02] MD5 / SHA256 摘要
来源：http://cr.muxihuayi.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://rt.huixiangedu.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://bo.hahajie.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ay.jctech888.com.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://pk.huixinmuqiang.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://aj.shxzukj.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://es.colortex.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ml.szxytkj.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://dy.bjjhwx.cn

[P03] 生成短随机字符串
来源：http://ui.muxihuayi.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ao.huixinmuqiang.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://pk.bookmarksfly.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hs.huanxung.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dp.gzmigu.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ul.panjiajie.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://rr.yuexingan06.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://iv.bookmarksfly.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://rr.jctech888.com.cn

[P04] 求长度
来源：http://pb.yuexingan06.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hw.gzmigu.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sh.colortex.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pu.colortex.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://po.huixinmuqiang.cn

Java: list.size();  map.size();  s.length()
来源：http://ck.asd995.cn

Go:   len(arr);  len(m)
来源：http://zn.lnxyls.cn

Ruby: x.length;  x.size
来源：http://kc.chemitech.net.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://dn.bookmarksfly.cn

[P05] 判断两个对象内容是否相等
来源：http://ri.chemitech.net.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://vg.huixiangedu.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://yc.muxihuayi.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ji.colortex.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://qw.huixiangedu.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://zm.jianghongdianzi.cn

Go:   reflect.DeepEqual(a, b)
来源：http://gc.szsharing.cn

Ruby: a == b
来源：http://vz.jianghongdianzi.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://qm.521024.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://lg.newstarts.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://bx.huixinmuqiang.cn

PHP:  if (empty($x)) {}
来源：http://al.newstarts.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://rs.bookmarksfly.cn

TS:   if (x == null) {}
来源：http://ib.szxytkj.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://zx.szxytkj.cn

Go:   if x == nil {}
来源：http://ik.szxytkj.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://qd.huixiangedu.cn

C#:   if (x is null) {}
来源：http://zz.bjjhwx.cn

[P07] 防抖与节流
来源：http://xl.muxihuayi.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://gx.jianghongdianzi.cn

PHP:  // 手写时间戳比较
来源：http://lr.szxytkj.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qv.bjjhwx.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wf.gzmigu.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://vg.521024.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://rj.szxytkj.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://qe.jianghongdianzi.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://kc.huixiangedu.cn

[P08] 处理浮点精度问题
来源：http://hm.9csxet.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hq.shxzskj.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://es.asd995.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://in.hahajie.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ip.panjiajie.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://bo.szsharing.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://gv.nicolike.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://no.jctech888.com.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mc.gzmigu.cn

================================================================================
来源：http://ie.yuexingan06.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://zt.haigaiapp.cn

================================================================================
来源：http://wa.nszjky.cn

[Q01] 创建表
来源：http://aa.shxzskj.cn

CREATE TABLE users (
来源：http://nw.bookmarksfly.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://xo.asd995.cn

name VARCHAR(50) NOT NULL,
来源：http://wa.huixinmuqiang.cn

email VARCHAR(100) UNIQUE,
来源：http://nn.wgjwhj.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://er.jianghongdianzi.cn

);
来源：http://pl.jctech888.com.cn

[Q02] 创建带外键的表
来源：http://cs.jianghongdianzi.cn

CREATE TABLE orders (
来源：http://ly.newstarts.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://uh.asd995.cn

user_id INT NOT NULL,
来源：http://ud.yuntaijiaju.cn

amount DECIMAL(10, 2),
来源：http://rs.jctech888.com.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://tk.muxihuayi.cn


<!-- 参考信息 -->