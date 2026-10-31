代发 wailian999

JS:   process.exit(1)
来源：http://vo.huixinmuqiang.cn

TS:   process.exit(1)
来源：http://ea.shxzskj.cn

Java: System.exit(1)
来源：http://pr.gzmigu.cn

Go:   os.Exit(1)
来源：http://oi.panjiajie.cn

Ruby: exit 1
来源：http://oi.asd995.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ia.nicolike.cn

[M06] 向标准错误输出
来源：http://su.yuexingan06.cn

Py:   print("err", file=sys.stderr)
来源：http://cm.521024.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://qw.hnjuh.cn

JS:   console.error("err")
来源：http://sv.nicolike.cn

TS:   console.error("err")
来源：http://za.9csxet.cn

Java: System.err.println("err")
来源：http://vo.nicolike.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://nh.gzmigu.cn

Ruby: warn "err"
来源：http://hc.jctech888.com.cn

C#:   Console.Error.WriteLine("err")
来源：http://ve.yuexingan06.cn

[M07] 判断是否为主入口
来源：http://ow.yuntaijiaju.cn

Py:   if __name__ == "__main__":
来源：http://qd.wgjwhj.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wb.yuexingan06.cn

JS:   require.main === module
来源：http://ge.asd995.cn

TS:   require.main === module
来源：http://op.chemitech.net.cn

Java: public static void main(String[] args)
来源：http://qr.521024.cn

Go:   func main()
来源：http://ii.huixinmuqiang.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://eo.muxihuayi.cn

C#:   static void Main(string[] args)
来源：http://uw.jianghongdianzi.cn

[M08] 获取系统与运行时信息
来源：http://ie.panjiajie.cn

Py:   platform.system();  platform.python_version()
来源：http://rn.nszjky.cn

PHP:  PHP_OS;  phpversion();
来源：http://hx.9csxet.cn

JS:   process.platform;  process.version
来源：http://gx.yuntaijiaju.cn

TS:   process.platform;  process.version
来源：http://jj.chemitech.net.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hn.bookmarksfly.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ac.muxihuayi.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://rb.lnxyls.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://nb.gzmigu.cn

================================================================================
来源：http://qx.szxytkj.cn

N. 数据结构与算法
来源：http://yw.521024.cn

================================================================================
来源：http://ve.wgjwhj.cn

[N01] 二分查找（有序数组）
来源：http://ak.nszjky.cn

Py:   bisect.bisect_left(arr, x)
来源：http://oj.shtwfgs.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://xw.shtwfgs.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ll.shtwfgs.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://se.wgjwhj.cn

Java: Arrays.binarySearch(arr, x)
来源：http://xi.bookmarksfly.cn

Go:   sort.SearchInts(arr, x)
来源：http://ui.yuntaijiaju.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://lt.chemitech.net.cn

C#:   Array.BinarySearch(arr, x)
来源：http://jn.nicolike.cn

[N02] 排序（工程实践用内置实现）
来源：http://jp.chemitech.net.cn

Py:   sorted(arr);  arr.sort()
来源：http://yd.9csxet.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://zg.jctech888.com.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://gn.shxzukj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://dh.nicolike.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://op.nicolike.cn

Go:   slices.Sort(arr)
来源：http://yu.shxzukj.cn

Ruby: arr.sort
来源：http://kr.shxzskj.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ew.yuexingan06.cn

[N03] 快速排序（分治示例）
来源：http://mq.shxzukj.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://to.jctech888.com.cn

PHP:  // 递归实现，或用 usort
来源：http://hn.hnjuh.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dz.yuexingan06.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zr.szxytkj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://cj.wgjwhj.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://kj.jctech888.com.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://lv.yuntaijiaju.cn

C#:   // 手写递归，或 Array.Sort
来源：http://fy.asd995.cn

[N04] 斐波那契数列
来源：http://hh.yuexingan06.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zi.haigaiapp.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://dq.jianghongdianzi.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tm.haigaiapp.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cz.lnxyls.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://xl.521024.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://qp.huixiangedu.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://yc.muxihuayi.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wd.panjiajie.cn

[N05] 最大公约数
来源：http://th.hahajie.cn

Py:   math.gcd(a, b)
来源：http://uw.521024.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://xt.lnxyls.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xs.nszjky.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bk.muxihuayi.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zr.muxihuayi.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://zc.gzmigu.cn

Ruby: a.gcd(b)
来源：http://on.colortex.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://yh.hnjuh.cn

[N06] 判断回文字符串
来源：http://hn.szsharing.cn

Py:   s == s[::-1]
来源：http://fc.huanxung.cn

PHP:  $s === strrev($s);
来源：http://ul.yuntaijiaju.cn

JS:   s === [...s].reverse().join("")
来源：http://np.bjjhwx.cn

TS:   s === [...s].reverse().join("")
来源：http://xn.muxihuayi.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mx.jianghongdianzi.cn

Go:   // 双指针从两端比较
来源：http://ii.huanxung.cn

Ruby: s == s.reverse
来源：http://ga.huixiangedu.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://iu.jctech888.com.cn

[N07] 两数之和（返回下标）
来源：http://tm.bjjhwx.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://tq.gzmigu.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ld.nicolike.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://qt.muxihuayi.cn

TS:   // 手写 Map<string, number>
来源：http://cy.asd995.cn

Java: // 手写 HashMap
来源：http://km.wgjwhj.cn

Go:   // 手写 map[int]int
来源：http://kw.bjjhwx.cn

Ruby: // 手写 Hash
来源：http://hk.bjjhwx.cn

C#:   // 手写 Dictionary<int, int>
来源：http://iw.muxihuayi.cn

[N08] 生成全排列
来源：http://gh.jctech888.com.cn

Py:   itertools.permutations(arr)
来源：http://yq.hnjuh.cn

PHP:  // 手写递归交换
来源：http://go.asd995.cn

JS:   // 手写回溯递归
来源：http://zc.huixinmuqiang.cn

TS:   // 手写回溯递归
来源：http://jc.huixinmuqiang.cn

Java: // 手写回溯递归
来源：http://on.newstarts.cn

Go:   // 手写回溯递归
来源：http://np.yuexingan06.cn

Ruby: arr.permutation.to_a
来源：http://fl.bookmarksfly.cn

C#:   // 手写回溯递归
来源：http://di.muxihuayi.cn

[N09] 栈与队列
来源：http://kq.shtwfgs.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://nf.szxytkj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://bw.hnjuh.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ba.muxihuayi.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://qu.szxytkj.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://vm.gzmigu.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ba.newstarts.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ss.jianghongdianzi.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hc.gzmigu.cn

[N10] 链表节点定义
来源：http://hk.nszjky.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://cn.gzmigu.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://yr.jctech888.com.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://rs.shxzukj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ro.jctech888.com.cn

Java: class Node { int v; Node next; }
来源：http://uq.yuexingan06.cn

Go:   type Node struct { V int; Next *Node }
来源：http://hx.gzmigu.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://nq.haigaiapp.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://li.shxzskj.cn

[N11] 二叉树中序遍历
来源：http://vu.newstarts.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://gn.wgjwhj.cn

PHP:  // 手写递归函数
来源：http://qm.9csxet.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hq.wgjwhj.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wg.shxzukj.cn

Java: // 手写递归
来源：http://ew.newstarts.cn

Go:   // 手写递归
来源：http://rn.shxzukj.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://aq.wgjwhj.cn

C#:   // 手写递归
来源：http://zc.asd995.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hj.jianghongdianzi.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://tr.jianghongdianzi.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://lt.bookmarksfly.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lb.szsharing.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hj.muxihuayi.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wo.newstarts.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ns.huixinmuqiang.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ta.colortex.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wf.huixinmuqiang.cn

================================================================================
来源：http://rt.chemitech.net.cn

O. 并发与异步
来源：http://gq.shtwfgs.cn

================================================================================
来源：http://wh.yuntaijiaju.cn

[O01] 启动一个线程
来源：http://ux.hahajie.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ot.nicolike.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ur.shtwfgs.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://iv.wgjwhj.cn

TS:   // 同 JS
来源：http://qu.muxihuayi.cn

Java: new Thread(() -> f()).start()
来源：http://jv.huixiangedu.cn

Go:   go f()
来源：http://de.szxytkj.cn

Ruby: Thread.new { f }
来源：http://gc.huixiangedu.cn

C#:   Task.Run(() => F());
来源：http://sp.9csxet.cn

[O02] 使用线程池
来源：http://yy.bjjhwx.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wi.newstarts.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://pw.huanxung.cn

JS:   // worker_threads 线程池
来源：http://pz.gzmigu.cn

TS:   // worker_threads 线程池
来源：http://qv.huixinmuqiang.cn

Java: Executors.newFixedThreadPool(4)
来源：http://qe.szxytkj.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://dd.shxzukj.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://co.yuntaijiaju.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://st.shxzskj.cn

[O03] 加锁保护共享数据
来源：http://iy.haigaiapp.cn

Py:   with lock: shared += 1
来源：http://sk.szxytkj.cn

PHP:  // 用 flock() 做文件锁
来源：http://dk.9csxet.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ec.bookmarksfly.cn

TS:   // 同 JS
来源：http://yh.jctech888.com.cn

Java: synchronized (this) { shared++; }
来源：http://dc.yuntaijiaju.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://xa.wgjwhj.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://xb.nicolike.cn

C#:   lock (gate) { shared++; }
来源：http://ox.yuexingan06.cn

[O04] 定义异步函数并等待
来源：http://en.szsharing.cn

Py:   async def f():⏎    await g()
来源：http://ye.huixinmuqiang.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ro.szsharing.cn

JS:   async function f() { await g(); }
来源：http://xy.newstarts.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ys.bookmarksfly.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://yr.bjjhwx.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://da.colortex.cn

Ruby: # 用 Fiber 或 async gem
来源：http://pi.muxihuayi.cn

C#:   async Task F() { await G(); }
来源：http://vb.haigaiapp.cn

[O05] 并发执行并等待全部完成
来源：http://wd.muxihuayi.cn

Py:   asyncio.gather(*tasks)
来源：http://al.huixinmuqiang.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wb.chemitech.net.cn

JS:   await Promise.all(tasks)
来源：http://mj.hahajie.cn

TS:   await Promise.all(tasks)
来源：http://if.szxytkj.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://tf.huixiangedu.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://bn.haigaiapp.cn

Ruby: threads.map(&:join)
来源：http://fs.521024.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://lj.huixinmuqiang.cn

[O06] 使用进程池
来源：http://kn.521024.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://xe.gzmigu.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://zc.hahajie.cn

JS:   // child_process / cluster 模块
来源：http://is.shxzukj.cn

TS:   // child_process / cluster 模块
来源：http://wy.nszjky.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ro.wgjwhj.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://um.nicolike.cn

Ruby: // fork 块
来源：http://bd.yuexingan06.cn

C#:   Parallel.For
来源：http://pt.yuexingan06.cn

================================================================================
来源：http://sn.hahajie.cn

P. 常用工具函数
来源：http://cn.bookmarksfly.cn

================================================================================
来源：http://kv.asd995.cn

[P01] 生成 UUID
来源：http://im.nicolike.cn

Py:   str(uuid.uuid4())
来源：http://uh.jctech888.com.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hi.jianghongdianzi.cn

JS:   crypto.randomUUID()
来源：http://qe.hnjuh.cn

TS:   crypto.randomUUID()
来源：http://cz.jianghongdianzi.cn

Java: UUID.randomUUID().toString()
来源：http://pg.lnxyls.cn

Go:   // 用 github.com/google/uuid
来源：http://hi.yuntaijiaju.cn

Ruby: SecureRandom.uuid
来源：http://bn.shtwfgs.cn

C#:   Guid.NewGuid().ToString()
来源：http://sq.yuntaijiaju.cn

[P02] MD5 / SHA256 摘要
来源：http://yk.muxihuayi.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://at.colortex.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ax.newstarts.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://oi.nicolike.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ob.chemitech.net.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wp.haigaiapp.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://qj.wgjwhj.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://tt.yuexingan06.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://rx.wgjwhj.cn

[P03] 生成短随机字符串
来源：http://ba.gzmigu.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://aj.panjiajie.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://th.newstarts.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://oj.huixinmuqiang.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rt.yuexingan06.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://eb.hnjuh.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ie.yuntaijiaju.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://pi.nicolike.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://jn.panjiajie.cn

[P04] 求长度
来源：http://ym.bookmarksfly.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://iq.wgjwhj.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gl.bookmarksfly.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fc.nszjky.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ph.haigaiapp.cn

Java: list.size();  map.size();  s.length()
来源：http://dw.hahajie.cn

Go:   len(arr);  len(m)
来源：http://hj.nicolike.cn

Ruby: x.length;  x.size
来源：http://yp.colortex.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://mc.gzmigu.cn

[P05] 判断两个对象内容是否相等
来源：http://fq.szxytkj.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://hs.shxzukj.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://yc.nicolike.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://pn.gzmigu.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mx.panjiajie.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://zn.shxzskj.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ro.lnxyls.cn

Ruby: a == b
来源：http://jy.chemitech.net.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://be.nszjky.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://zv.szsharing.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://tx.nszjky.cn

PHP:  if (empty($x)) {}
来源：http://dr.newstarts.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hl.gzmigu.cn

TS:   if (x == null) {}
来源：http://nx.newstarts.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://dz.huixiangedu.cn

Go:   if x == nil {}
来源：http://zo.bjjhwx.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wo.yuexingan06.cn

C#:   if (x is null) {}
来源：http://sm.nicolike.cn

[P07] 防抖与节流
来源：http://er.szsharing.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mr.shtwfgs.cn

PHP:  // 手写时间戳比较
来源：http://yu.shtwfgs.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ws.huanxung.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://an.yuntaijiaju.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://bi.wgjwhj.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://tr.panjiajie.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://hs.shtwfgs.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://do.521024.cn

[P08] 处理浮点精度问题
来源：http://ev.nicolike.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mb.nicolike.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://oi.lnxyls.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://zw.yuexingan06.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://rp.9csxet.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://zq.colortex.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ez.panjiajie.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://zf.muxihuayi.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://yc.hnjuh.cn

================================================================================
来源：http://vb.szsharing.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://dg.szxytkj.cn

================================================================================
来源：http://wf.yuntaijiaju.cn

[Q01] 创建表
来源：http://rx.panjiajie.cn

CREATE TABLE users (
来源：http://de.shxzukj.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mf.hahajie.cn

name VARCHAR(50) NOT NULL,
来源：http://ei.yuexingan06.cn

email VARCHAR(100) UNIQUE,
来源：http://tg.nszjky.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://de.lnxyls.cn

);
来源：http://xs.bjjhwx.cn

[Q02] 创建带外键的表
来源：http://rn.huixiangedu.cn

CREATE TABLE orders (
来源：http://ii.haigaiapp.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://sd.yuexingan06.cn

user_id INT NOT NULL,
来源：http://ys.shtwfgs.cn

amount DECIMAL(10, 2),
来源：http://sf.nszjky.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://gi.nszjky.cn

);
来源：http://ly.bjjhwx.cn

[Q03] 增加列
来源：http://yx.jctech888.com.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://uw.huanxung.cn

[Q04] 修改列类型
来源：http://ol.huanxung.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ar.bookmarksfly.cn

[Q05] 重命名列
来源：http://pt.jianghongdianzi.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://bv.panjiajie.cn

[Q06] 删除列
来源：http://kb.shtwfgs.cn


<!-- 参考信息 -->