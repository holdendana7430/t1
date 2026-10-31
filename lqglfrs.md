代发 wailian999

[M04] 获取当前工作目录
来源：http://uz.bjjhwx.cn

Py:   os.getcwd()
来源：http://vj.jianghongdianzi.cn

PHP:  getcwd();
来源：http://xe.nszjky.cn

JS:   process.cwd()
来源：http://cz.szsharing.cn

TS:   process.cwd()
来源：http://mp.newstarts.cn

Java: Path.of("").toAbsolutePath()
来源：http://vx.shxzukj.cn

Go:   os.Getwd()
来源：http://oz.bjjhwx.cn

Ruby: Dir.pwd
来源：http://wd.huixiangedu.cn

C#:   Directory.GetCurrentDirectory()
来源：http://jo.nicolike.cn

[M05] 设置退出码
来源：http://yc.yuexingan06.cn

Py:   sys.exit(1)
来源：http://ej.huixiangedu.cn

PHP:  exit(1);
来源：http://jm.shxzukj.cn

JS:   process.exit(1)
来源：http://rz.huixinmuqiang.cn

TS:   process.exit(1)
来源：http://ex.jctech888.com.cn

Java: System.exit(1)
来源：http://bw.yuexingan06.cn

Go:   os.Exit(1)
来源：http://aw.huanxung.cn

Ruby: exit 1
来源：http://wi.gzmigu.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://vx.lnxyls.cn

[M06] 向标准错误输出
来源：http://kc.huixiangedu.cn

Py:   print("err", file=sys.stderr)
来源：http://ez.chemitech.net.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://so.nszjky.cn

JS:   console.error("err")
来源：http://nq.panjiajie.cn

TS:   console.error("err")
来源：http://ry.bookmarksfly.cn

Java: System.err.println("err")
来源：http://ry.shtwfgs.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://vn.huanxung.cn

Ruby: warn "err"
来源：http://tb.yuntaijiaju.cn

C#:   Console.Error.WriteLine("err")
来源：http://ks.huixinmuqiang.cn

[M07] 判断是否为主入口
来源：http://eh.chemitech.net.cn

Py:   if __name__ == "__main__":
来源：http://de.newstarts.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://jy.asd995.cn

JS:   require.main === module
来源：http://rn.haigaiapp.cn

TS:   require.main === module
来源：http://fe.chemitech.net.cn

Java: public static void main(String[] args)
来源：http://eg.shxzukj.cn

Go:   func main()
来源：http://qn.huixinmuqiang.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://vg.wgjwhj.cn

C#:   static void Main(string[] args)
来源：http://bl.nicolike.cn

[M08] 获取系统与运行时信息
来源：http://cu.9csxet.cn

Py:   platform.system();  platform.python_version()
来源：http://qx.shxzskj.cn

PHP:  PHP_OS;  phpversion();
来源：http://xo.jianghongdianzi.cn

JS:   process.platform;  process.version
来源：http://ls.nicolike.cn

TS:   process.platform;  process.version
来源：http://dr.szxytkj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://dc.muxihuayi.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://lk.shxzukj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ne.huanxung.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://lk.shxzukj.cn

================================================================================
来源：http://zz.newstarts.cn

N. 数据结构与算法
来源：http://le.yuexingan06.cn

================================================================================
来源：http://kp.panjiajie.cn

[N01] 二分查找（有序数组）
来源：http://eu.wgjwhj.cn

Py:   bisect.bisect_left(arr, x)
来源：http://cz.jianghongdianzi.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://bz.newstarts.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pj.huixiangedu.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lo.nszjky.cn

Java: Arrays.binarySearch(arr, x)
来源：http://fv.huixinmuqiang.cn

Go:   sort.SearchInts(arr, x)
来源：http://hp.gzmigu.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://dg.newstarts.cn

C#:   Array.BinarySearch(arr, x)
来源：http://xo.asd995.cn

[N02] 排序（工程实践用内置实现）
来源：http://os.wgjwhj.cn

Py:   sorted(arr);  arr.sort()
来源：http://me.nszjky.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://np.jianghongdianzi.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://vs.521024.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://vf.lnxyls.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://vj.shxzskj.cn

Go:   slices.Sort(arr)
来源：http://fd.muxihuayi.cn

Ruby: arr.sort
来源：http://jt.hahajie.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://lt.szxytkj.cn

[N03] 快速排序（分治示例）
来源：http://jg.nicolike.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://uf.colortex.cn

PHP:  // 递归实现，或用 usort
来源：http://rz.colortex.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dk.hnjuh.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://eg.huanxung.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mx.521024.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://lw.shtwfgs.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://dv.asd995.cn

C#:   // 手写递归，或 Array.Sort
来源：http://le.colortex.cn

[N04] 斐波那契数列
来源：http://fx.521024.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://dc.yuntaijiaju.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://pz.shxzukj.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sm.lnxyls.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tj.521024.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://gm.521024.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://eq.newstarts.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ld.szxytkj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ko.huixiangedu.cn

[N05] 最大公约数
来源：http://jx.wgjwhj.cn

Py:   math.gcd(a, b)
来源：http://hn.lnxyls.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://nw.9csxet.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gp.szsharing.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ty.asd995.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://vg.shtwfgs.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://bp.hnjuh.cn

Ruby: a.gcd(b)
来源：http://yg.asd995.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ef.yuexingan06.cn

[N06] 判断回文字符串
来源：http://hl.hnjuh.cn

Py:   s == s[::-1]
来源：http://lr.521024.cn

PHP:  $s === strrev($s);
来源：http://fd.9csxet.cn

JS:   s === [...s].reverse().join("")
来源：http://kx.muxihuayi.cn

TS:   s === [...s].reverse().join("")
来源：http://yt.shtwfgs.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://zx.jctech888.com.cn

Go:   // 双指针从两端比较
来源：http://yr.hahajie.cn

Ruby: s == s.reverse
来源：http://to.szxytkj.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://xw.chemitech.net.cn

[N07] 两数之和（返回下标）
来源：http://hp.shtwfgs.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://de.bjjhwx.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://lw.panjiajie.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ag.bookmarksfly.cn

TS:   // 手写 Map<string, number>
来源：http://ao.lnxyls.cn

Java: // 手写 HashMap
来源：http://js.jctech888.com.cn

Go:   // 手写 map[int]int
来源：http://de.bjjhwx.cn

Ruby: // 手写 Hash
来源：http://ou.bookmarksfly.cn

C#:   // 手写 Dictionary<int, int>
来源：http://er.colortex.cn

[N08] 生成全排列
来源：http://ez.panjiajie.cn

Py:   itertools.permutations(arr)
来源：http://zg.muxihuayi.cn

PHP:  // 手写递归交换
来源：http://ng.9csxet.cn

JS:   // 手写回溯递归
来源：http://br.nicolike.cn

TS:   // 手写回溯递归
来源：http://fl.lnxyls.cn

Java: // 手写回溯递归
来源：http://xm.chemitech.net.cn

Go:   // 手写回溯递归
来源：http://qq.huanxung.cn

Ruby: arr.permutation.to_a
来源：http://ca.lnxyls.cn

C#:   // 手写回溯递归
来源：http://tg.shxzukj.cn

[N09] 栈与队列
来源：http://cm.lnxyls.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://qp.huixinmuqiang.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://sm.jianghongdianzi.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://pw.yuexingan06.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://gl.9csxet.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://uh.shxzskj.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://kd.huixinmuqiang.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://gd.colortex.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://sn.shxzukj.cn

[N10] 链表节点定义
来源：http://vf.muxihuayi.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ha.panjiajie.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://lt.huanxung.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://te.nicolike.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://iq.asd995.cn

Java: class Node { int v; Node next; }
来源：http://fm.panjiajie.cn

Go:   type Node struct { V int; Next *Node }
来源：http://rx.shxzskj.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://we.huixinmuqiang.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ym.muxihuayi.cn

[N11] 二叉树中序遍历
来源：http://ei.hahajie.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://zv.nszjky.cn

PHP:  // 手写递归函数
来源：http://dw.yuexingan06.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nt.huixinmuqiang.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zh.huixiangedu.cn

Java: // 手写递归
来源：http://je.wgjwhj.cn

Go:   // 手写递归
来源：http://cl.szsharing.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://rr.yuntaijiaju.cn

C#:   // 手写递归
来源：http://bl.panjiajie.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://zw.lnxyls.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://sb.szxytkj.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://zf.newstarts.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xz.bookmarksfly.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://le.9csxet.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://vw.asd995.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://vj.bjjhwx.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://zq.asd995.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ea.shtwfgs.cn

================================================================================
来源：http://oy.shxzukj.cn

O. 并发与异步
来源：http://lo.panjiajie.cn

================================================================================
来源：http://vf.chemitech.net.cn

[O01] 启动一个线程
来源：http://kk.bookmarksfly.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://qe.9csxet.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://cg.chemitech.net.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ji.yuntaijiaju.cn

TS:   // 同 JS
来源：http://ex.muxihuayi.cn

Java: new Thread(() -> f()).start()
来源：http://al.nicolike.cn

Go:   go f()
来源：http://nk.9csxet.cn

Ruby: Thread.new { f }
来源：http://jd.shxzukj.cn

C#:   Task.Run(() => F());
来源：http://rw.szsharing.cn

[O02] 使用线程池
来源：http://zu.jianghongdianzi.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://gp.jianghongdianzi.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ba.shxzskj.cn

JS:   // worker_threads 线程池
来源：http://dl.shxzukj.cn

TS:   // worker_threads 线程池
来源：http://oi.bjjhwx.cn

Java: Executors.newFixedThreadPool(4)
来源：http://zy.jctech888.com.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://bc.shxzukj.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://kg.panjiajie.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://jq.haigaiapp.cn

[O03] 加锁保护共享数据
来源：http://xm.gzmigu.cn

Py:   with lock: shared += 1
来源：http://ne.newstarts.cn

PHP:  // 用 flock() 做文件锁
来源：http://pt.9csxet.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://pr.panjiajie.cn

TS:   // 同 JS
来源：http://bj.521024.cn

Java: synchronized (this) { shared++; }
来源：http://hk.yuntaijiaju.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://jp.shtwfgs.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://xg.muxihuayi.cn

C#:   lock (gate) { shared++; }
来源：http://nn.yuexingan06.cn

[O04] 定义异步函数并等待
来源：http://va.chemitech.net.cn

Py:   async def f():⏎    await g()
来源：http://de.shtwfgs.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://jo.jctech888.com.cn

JS:   async function f() { await g(); }
来源：http://ry.521024.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ut.wgjwhj.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ho.hahajie.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://pp.bjjhwx.cn

Ruby: # 用 Fiber 或 async gem
来源：http://kw.jianghongdianzi.cn

C#:   async Task F() { await G(); }
来源：http://rf.9csxet.cn

[O05] 并发执行并等待全部完成
来源：http://oj.hahajie.cn

Py:   asyncio.gather(*tasks)
来源：http://aj.panjiajie.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ln.bookmarksfly.cn

JS:   await Promise.all(tasks)
来源：http://uw.9csxet.cn

TS:   await Promise.all(tasks)
来源：http://lj.521024.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://lg.hnjuh.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wg.nszjky.cn

Ruby: threads.map(&:join)
来源：http://je.newstarts.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://sq.shtwfgs.cn

[O06] 使用进程池
来源：http://zz.newstarts.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://db.yuexingan06.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://qg.gzmigu.cn

JS:   // child_process / cluster 模块
来源：http://dq.bookmarksfly.cn

TS:   // child_process / cluster 模块
来源：http://bl.shxzukj.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ac.bookmarksfly.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://dt.shxzukj.cn

Ruby: // fork 块
来源：http://ij.wgjwhj.cn

C#:   Parallel.For
来源：http://dh.yuexingan06.cn

================================================================================
来源：http://tb.szxytkj.cn

P. 常用工具函数
来源：http://gc.wgjwhj.cn

================================================================================
来源：http://xz.wgjwhj.cn

[P01] 生成 UUID
来源：http://dl.muxihuayi.cn

Py:   str(uuid.uuid4())
来源：http://tu.yuntaijiaju.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://qb.huixiangedu.cn

JS:   crypto.randomUUID()
来源：http://jo.haigaiapp.cn

TS:   crypto.randomUUID()
来源：http://yf.yuexingan06.cn

Java: UUID.randomUUID().toString()
来源：http://yx.wgjwhj.cn

Go:   // 用 github.com/google/uuid
来源：http://tc.gzmigu.cn

Ruby: SecureRandom.uuid
来源：http://fv.bookmarksfly.cn

C#:   Guid.NewGuid().ToString()
来源：http://yd.521024.cn

[P02] MD5 / SHA256 摘要
来源：http://yl.huixiangedu.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hi.hahajie.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ci.shxzskj.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ln.jctech888.com.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://an.yuntaijiaju.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://xs.shxzskj.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://kc.9csxet.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hp.panjiajie.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://pa.hnjuh.cn

[P03] 生成短随机字符串
来源：http://xr.nicolike.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://zi.asd995.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://cc.huanxung.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cc.huanxung.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://df.jianghongdianzi.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://de.nicolike.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://fo.newstarts.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://zt.huanxung.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://vr.shtwfgs.cn

[P04] 求长度
来源：http://se.newstarts.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://lw.wgjwhj.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dc.colortex.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fa.shxzukj.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kg.asd995.cn

Java: list.size();  map.size();  s.length()
来源：http://ld.bjjhwx.cn

Go:   len(arr);  len(m)
来源：http://ys.nicolike.cn

Ruby: x.length;  x.size
来源：http://qn.yuexingan06.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://he.muxihuayi.cn

[P05] 判断两个对象内容是否相等
来源：http://bp.colortex.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ir.colortex.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://aw.asd995.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://lz.shxzukj.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://as.colortex.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ar.yuexingan06.cn

Go:   reflect.DeepEqual(a, b)
来源：http://gs.hahajie.cn

Ruby: a == b
来源：http://ox.haigaiapp.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://pc.shxzskj.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://cj.yuexingan06.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://em.muxihuayi.cn

PHP:  if (empty($x)) {}
来源：http://ns.shxzskj.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://bl.bookmarksfly.cn

TS:   if (x == null) {}
来源：http://bc.bookmarksfly.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://rz.colortex.cn

Go:   if x == nil {}
来源：http://ts.wgjwhj.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://vu.panjiajie.cn

C#:   if (x is null) {}
来源：http://ev.jianghongdianzi.cn

[P07] 防抖与节流
来源：http://tg.szsharing.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://xu.colortex.cn

PHP:  // 手写时间戳比较
来源：http://fz.haigaiapp.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ue.yuntaijiaju.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yn.wgjwhj.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wj.yuexingan06.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://qc.bookmarksfly.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ki.huixinmuqiang.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://yw.huanxung.cn

[P08] 处理浮点精度问题
来源：http://qh.huixiangedu.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://cn.szsharing.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ec.szxytkj.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://vy.521024.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://oa.chemitech.net.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://vh.colortex.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://eb.huixiangedu.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ec.haigaiapp.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://vx.bookmarksfly.cn

================================================================================
来源：http://pv.yuntaijiaju.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wn.newstarts.cn

================================================================================
来源：http://xs.521024.cn

[Q01] 创建表
来源：http://lp.lnxyls.cn

CREATE TABLE users (
来源：http://qp.gzmigu.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://px.lnxyls.cn

name VARCHAR(50) NOT NULL,
来源：http://lu.huixiangedu.cn

email VARCHAR(100) UNIQUE,
来源：http://bi.shxzskj.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://at.nicolike.cn

);
来源：http://mu.wgjwhj.cn

[Q02] 创建带外键的表
来源：http://na.bjjhwx.cn

CREATE TABLE orders (
来源：http://ti.asd995.cn


<!-- 参考信息 -->