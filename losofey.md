代发 wailian999

[M04] 获取当前工作目录
来源：http://jo.jctech888.com.cn

Py:   os.getcwd()
来源：http://fu.szxytkj.cn

PHP:  getcwd();
来源：http://pa.bjjhwx.cn

JS:   process.cwd()
来源：http://cq.huixinmuqiang.cn

TS:   process.cwd()
来源：http://mx.shxzukj.cn

Java: Path.of("").toAbsolutePath()
来源：http://jw.szxytkj.cn

Go:   os.Getwd()
来源：http://ws.hahajie.cn

Ruby: Dir.pwd
来源：http://yp.jctech888.com.cn

C#:   Directory.GetCurrentDirectory()
来源：http://tt.shxzukj.cn

[M05] 设置退出码
来源：http://zl.shtwfgs.cn

Py:   sys.exit(1)
来源：http://mx.szsharing.cn

PHP:  exit(1);
来源：http://om.huixiangedu.cn

JS:   process.exit(1)
来源：http://vr.jctech888.com.cn

TS:   process.exit(1)
来源：http://un.yuntaijiaju.cn

Java: System.exit(1)
来源：http://rd.shtwfgs.cn

Go:   os.Exit(1)
来源：http://vy.jianghongdianzi.cn

Ruby: exit 1
来源：http://pn.9csxet.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://li.shtwfgs.cn

[M06] 向标准错误输出
来源：http://lb.szsharing.cn

Py:   print("err", file=sys.stderr)
来源：http://ys.haigaiapp.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ke.yuexingan06.cn

JS:   console.error("err")
来源：http://uy.hahajie.cn

TS:   console.error("err")
来源：http://ti.jianghongdianzi.cn

Java: System.err.println("err")
来源：http://fa.jianghongdianzi.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://aw.yuexingan06.cn

Ruby: warn "err"
来源：http://gy.muxihuayi.cn

C#:   Console.Error.WriteLine("err")
来源：http://re.huixinmuqiang.cn

[M07] 判断是否为主入口
来源：http://pf.wgjwhj.cn

Py:   if __name__ == "__main__":
来源：http://eg.newstarts.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://tx.shxzskj.cn

JS:   require.main === module
来源：http://co.newstarts.cn

TS:   require.main === module
来源：http://sj.newstarts.cn

Java: public static void main(String[] args)
来源：http://qe.jianghongdianzi.cn

Go:   func main()
来源：http://lv.chemitech.net.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mq.huanxung.cn

C#:   static void Main(string[] args)
来源：http://fm.yuexingan06.cn

[M08] 获取系统与运行时信息
来源：http://na.huixiangedu.cn

Py:   platform.system();  platform.python_version()
来源：http://bw.wgjwhj.cn

PHP:  PHP_OS;  phpversion();
来源：http://ik.asd995.cn

JS:   process.platform;  process.version
来源：http://bh.huixinmuqiang.cn

TS:   process.platform;  process.version
来源：http://sk.haigaiapp.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://by.asd995.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://cw.nszjky.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://vj.shtwfgs.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://qx.hnjuh.cn

================================================================================
来源：http://az.521024.cn

N. 数据结构与算法
来源：http://na.bjjhwx.cn

================================================================================
来源：http://xj.nicolike.cn

[N01] 二分查找（有序数组）
来源：http://nx.asd995.cn

Py:   bisect.bisect_left(arr, x)
来源：http://rg.bookmarksfly.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://oj.jianghongdianzi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lu.nicolike.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://em.bjjhwx.cn

Java: Arrays.binarySearch(arr, x)
来源：http://yy.huixiangedu.cn

Go:   sort.SearchInts(arr, x)
来源：http://hr.nszjky.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://wm.huanxung.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ng.jianghongdianzi.cn

[N02] 排序（工程实践用内置实现）
来源：http://uz.nicolike.cn

Py:   sorted(arr);  arr.sort()
来源：http://gq.chemitech.net.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://sr.521024.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://sb.panjiajie.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://rm.huixiangedu.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://sz.szsharing.cn

Go:   slices.Sort(arr)
来源：http://xx.yuexingan06.cn

Ruby: arr.sort
来源：http://cs.chemitech.net.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://rt.huixinmuqiang.cn

[N03] 快速排序（分治示例）
来源：http://nc.gzmigu.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ja.huixinmuqiang.cn

PHP:  // 递归实现，或用 usort
来源：http://jk.asd995.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bi.asd995.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sv.huixinmuqiang.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://xi.nszjky.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://eg.wgjwhj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hq.muxihuayi.cn

C#:   // 手写递归，或 Array.Sort
来源：http://sr.nszjky.cn

[N04] 斐波那契数列
来源：http://nf.szsharing.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wg.bjjhwx.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mx.9csxet.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sl.bjjhwx.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vw.yuexingan06.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://rs.hnjuh.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://js.bjjhwx.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://qf.asd995.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://be.huixinmuqiang.cn

[N05] 最大公约数
来源：http://st.asd995.cn

Py:   math.gcd(a, b)
来源：http://xs.gzmigu.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://vt.chemitech.net.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dd.nszjky.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jt.chemitech.net.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://kp.huixinmuqiang.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ez.newstarts.cn

Ruby: a.gcd(b)
来源：http://cj.hahajie.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://qy.shtwfgs.cn

[N06] 判断回文字符串
来源：http://hw.jctech888.com.cn

Py:   s == s[::-1]
来源：http://fh.newstarts.cn

PHP:  $s === strrev($s);
来源：http://cy.9csxet.cn

JS:   s === [...s].reverse().join("")
来源：http://oq.szsharing.cn

TS:   s === [...s].reverse().join("")
来源：http://yl.lnxyls.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://fv.haigaiapp.cn

Go:   // 双指针从两端比较
来源：http://od.hnjuh.cn

Ruby: s == s.reverse
来源：http://jb.yuexingan06.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://xt.jianghongdianzi.cn

[N07] 两数之和（返回下标）
来源：http://ea.jctech888.com.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://az.521024.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://lv.haigaiapp.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://oo.nszjky.cn

TS:   // 手写 Map<string, number>
来源：http://ft.haigaiapp.cn

Java: // 手写 HashMap
来源：http://qv.shxzukj.cn

Go:   // 手写 map[int]int
来源：http://zy.lnxyls.cn

Ruby: // 手写 Hash
来源：http://dn.hahajie.cn

C#:   // 手写 Dictionary<int, int>
来源：http://zu.yuexingan06.cn

[N08] 生成全排列
来源：http://fc.asd995.cn

Py:   itertools.permutations(arr)
来源：http://cz.yuexingan06.cn

PHP:  // 手写递归交换
来源：http://tc.wgjwhj.cn

JS:   // 手写回溯递归
来源：http://tj.yuexingan06.cn

TS:   // 手写回溯递归
来源：http://ld.jianghongdianzi.cn

Java: // 手写回溯递归
来源：http://pd.shtwfgs.cn

Go:   // 手写回溯递归
来源：http://eq.colortex.cn

Ruby: arr.permutation.to_a
来源：http://ac.shtwfgs.cn

C#:   // 手写回溯递归
来源：http://sr.huixiangedu.cn

[N09] 栈与队列
来源：http://we.shxzskj.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://sf.huanxung.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wo.chemitech.net.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://il.panjiajie.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ni.shxzskj.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://us.panjiajie.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://qv.newstarts.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://fh.chemitech.net.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://tt.shxzskj.cn

[N10] 链表节点定义
来源：http://kh.521024.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ow.chemitech.net.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://eb.wgjwhj.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://me.newstarts.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ym.521024.cn

Java: class Node { int v; Node next; }
来源：http://np.lnxyls.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ra.huanxung.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://qg.jctech888.com.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://nz.shxzukj.cn

[N11] 二叉树中序遍历
来源：http://yz.shxzskj.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://xu.newstarts.cn

PHP:  // 手写递归函数
来源：http://ey.jctech888.com.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jy.shxzukj.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ws.shtwfgs.cn

Java: // 手写递归
来源：http://dj.szsharing.cn

Go:   // 手写递归
来源：http://kb.jctech888.com.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wb.szsharing.cn

C#:   // 手写递归
来源：http://lk.shxzskj.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://cp.jctech888.com.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://dp.nicolike.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ow.gzmigu.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ev.muxihuayi.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qp.hnjuh.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ub.chemitech.net.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://yy.wgjwhj.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ck.gzmigu.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://fj.bookmarksfly.cn

================================================================================
来源：http://wk.huanxung.cn

O. 并发与异步
来源：http://hx.huanxung.cn

================================================================================
来源：http://tz.shxzukj.cn

[O01] 启动一个线程
来源：http://az.wgjwhj.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ht.yuntaijiaju.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://as.colortex.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://sd.jctech888.com.cn

TS:   // 同 JS
来源：http://sw.9csxet.cn

Java: new Thread(() -> f()).start()
来源：http://gj.521024.cn

Go:   go f()
来源：http://ot.asd995.cn

Ruby: Thread.new { f }
来源：http://gu.muxihuayi.cn

C#:   Task.Run(() => F());
来源：http://tb.hahajie.cn

[O02] 使用线程池
来源：http://ce.jianghongdianzi.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://an.panjiajie.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://vf.colortex.cn

JS:   // worker_threads 线程池
来源：http://ve.huixinmuqiang.cn

TS:   // worker_threads 线程池
来源：http://vt.colortex.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ka.asd995.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://go.gzmigu.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://gu.521024.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://lg.bjjhwx.cn

[O03] 加锁保护共享数据
来源：http://jv.jctech888.com.cn

Py:   with lock: shared += 1
来源：http://ix.szsharing.cn

PHP:  // 用 flock() 做文件锁
来源：http://ps.nicolike.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hn.chemitech.net.cn

TS:   // 同 JS
来源：http://gv.asd995.cn

Java: synchronized (this) { shared++; }
来源：http://dc.gzmigu.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://zp.hahajie.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://br.chemitech.net.cn

C#:   lock (gate) { shared++; }
来源：http://qt.shtwfgs.cn

[O04] 定义异步函数并等待
来源：http://dz.huixinmuqiang.cn

Py:   async def f():⏎    await g()
来源：http://kx.colortex.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://dk.asd995.cn

JS:   async function f() { await g(); }
来源：http://eb.521024.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://jp.asd995.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://jt.nszjky.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://cg.hahajie.cn

Ruby: # 用 Fiber 或 async gem
来源：http://gs.shtwfgs.cn

C#:   async Task F() { await G(); }
来源：http://gn.newstarts.cn

[O05] 并发执行并等待全部完成
来源：http://in.muxihuayi.cn

Py:   asyncio.gather(*tasks)
来源：http://ny.huanxung.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ft.muxihuayi.cn

JS:   await Promise.all(tasks)
来源：http://ym.jctech888.com.cn

TS:   await Promise.all(tasks)
来源：http://ce.bjjhwx.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://at.colortex.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://fn.yuntaijiaju.cn

Ruby: threads.map(&:join)
来源：http://ip.bjjhwx.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://iu.muxihuayi.cn

[O06] 使用进程池
来源：http://to.gzmigu.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://jl.asd995.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://au.bjjhwx.cn

JS:   // child_process / cluster 模块
来源：http://hp.lnxyls.cn

TS:   // child_process / cluster 模块
来源：http://bs.huixinmuqiang.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://xo.muxihuayi.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://gw.bookmarksfly.cn

Ruby: // fork 块
来源：http://td.nszjky.cn

C#:   Parallel.For
来源：http://ur.huixiangedu.cn

================================================================================
来源：http://hr.haigaiapp.cn

P. 常用工具函数
来源：http://ue.shtwfgs.cn

================================================================================
来源：http://jm.huanxung.cn

[P01] 生成 UUID
来源：http://po.lnxyls.cn

Py:   str(uuid.uuid4())
来源：http://bt.newstarts.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://an.hahajie.cn

JS:   crypto.randomUUID()
来源：http://jt.yuntaijiaju.cn

TS:   crypto.randomUUID()
来源：http://mv.yuntaijiaju.cn

Java: UUID.randomUUID().toString()
来源：http://sp.shxzskj.cn

Go:   // 用 github.com/google/uuid
来源：http://ln.yuntaijiaju.cn

Ruby: SecureRandom.uuid
来源：http://zu.shxzskj.cn

C#:   Guid.NewGuid().ToString()
来源：http://dl.hnjuh.cn

[P02] MD5 / SHA256 摘要
来源：http://zk.jianghongdianzi.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ra.wgjwhj.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://gw.szxytkj.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://no.chemitech.net.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://cj.jctech888.com.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://zo.gzmigu.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ja.jianghongdianzi.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ag.nszjky.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://jm.shxzukj.cn

[P03] 生成短随机字符串
来源：http://ka.huanxung.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://qi.colortex.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mw.lnxyls.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rr.shtwfgs.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jc.521024.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://vh.jctech888.com.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://tl.jianghongdianzi.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://qj.huixinmuqiang.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wu.colortex.cn

[P04] 求长度
来源：http://gn.chemitech.net.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ob.shtwfgs.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yq.panjiajie.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nc.nszjky.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vs.hnjuh.cn

Java: list.size();  map.size();  s.length()
来源：http://qm.asd995.cn

Go:   len(arr);  len(m)
来源：http://da.chemitech.net.cn

Ruby: x.length;  x.size
来源：http://qa.szxytkj.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://sk.wgjwhj.cn

[P05] 判断两个对象内容是否相等
来源：http://tu.huixiangedu.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://iu.panjiajie.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://tw.chemitech.net.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://xg.shtwfgs.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://qi.asd995.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ke.muxihuayi.cn

Go:   reflect.DeepEqual(a, b)
来源：http://wy.shtwfgs.cn

Ruby: a == b
来源：http://zy.jianghongdianzi.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hq.gzmigu.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://dy.nicolike.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://lz.yuntaijiaju.cn

PHP:  if (empty($x)) {}
来源：http://dy.jianghongdianzi.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://yq.asd995.cn

TS:   if (x == null) {}
来源：http://gd.huixinmuqiang.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://xl.jianghongdianzi.cn

Go:   if x == nil {}
来源：http://ml.shtwfgs.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://tm.colortex.cn

C#:   if (x is null) {}
来源：http://hb.muxihuayi.cn

[P07] 防抖与节流
来源：http://df.521024.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://xw.panjiajie.cn

PHP:  // 手写时间戳比较
来源：http://kv.haigaiapp.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fg.panjiajie.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kv.shtwfgs.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://vc.gzmigu.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://bw.yuntaijiaju.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://sm.yuexingan06.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://pb.9csxet.cn

[P08] 处理浮点精度问题
来源：http://zd.colortex.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hs.bookmarksfly.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://zg.colortex.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://om.chemitech.net.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://do.nszjky.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mc.szxytkj.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://oo.yuexingan06.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://rc.asd995.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://qu.bjjhwx.cn

================================================================================
来源：http://do.colortex.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hf.nicolike.cn

================================================================================
来源：http://hf.yuexingan06.cn

[Q01] 创建表
来源：http://be.bookmarksfly.cn

CREATE TABLE users (
来源：http://qz.521024.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://st.yuntaijiaju.cn

name VARCHAR(50) NOT NULL,
来源：http://wv.gzmigu.cn

email VARCHAR(100) UNIQUE,
来源：http://ct.panjiajie.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ky.asd995.cn

);
来源：http://fk.hnjuh.cn

[Q02] 创建带外键的表
来源：http://ev.muxihuayi.cn

CREATE TABLE orders (
来源：http://om.bookmarksfly.cn


<!-- 参考信息 -->