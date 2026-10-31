代发 wailian999

[M04] 获取当前工作目录
来源：http://rx.shxzukj.cn

Py:   os.getcwd()
来源：http://ia.hnjuh.cn

PHP:  getcwd();
来源：http://bh.muxihuayi.cn

JS:   process.cwd()
来源：http://cd.nicolike.cn

TS:   process.cwd()
来源：http://me.nicolike.cn

Java: Path.of("").toAbsolutePath()
来源：http://ng.nszjky.cn

Go:   os.Getwd()
来源：http://vc.huixinmuqiang.cn

Ruby: Dir.pwd
来源：http://jf.shxzskj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://mj.newstarts.cn

[M05] 设置退出码
来源：http://et.huixinmuqiang.cn

Py:   sys.exit(1)
来源：http://un.chemitech.net.cn

PHP:  exit(1);
来源：http://qx.yuntaijiaju.cn

JS:   process.exit(1)
来源：http://gp.bjjhwx.cn

TS:   process.exit(1)
来源：http://al.hahajie.cn

Java: System.exit(1)
来源：http://ll.panjiajie.cn

Go:   os.Exit(1)
来源：http://rl.hnjuh.cn

Ruby: exit 1
来源：http://qp.hahajie.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://bz.haigaiapp.cn

[M06] 向标准错误输出
来源：http://qm.hahajie.cn

Py:   print("err", file=sys.stderr)
来源：http://zv.521024.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://xc.bookmarksfly.cn

JS:   console.error("err")
来源：http://og.chemitech.net.cn

TS:   console.error("err")
来源：http://si.panjiajie.cn

Java: System.err.println("err")
来源：http://ua.shtwfgs.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://lk.hahajie.cn

Ruby: warn "err"
来源：http://ql.lnxyls.cn

C#:   Console.Error.WriteLine("err")
来源：http://cf.yuntaijiaju.cn

[M07] 判断是否为主入口
来源：http://xo.shxzskj.cn

Py:   if __name__ == "__main__":
来源：http://yp.szsharing.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://lj.shtwfgs.cn

JS:   require.main === module
来源：http://km.lnxyls.cn

TS:   require.main === module
来源：http://oo.nicolike.cn

Java: public static void main(String[] args)
来源：http://dy.bjjhwx.cn

Go:   func main()
来源：http://dc.9csxet.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://vq.shtwfgs.cn

C#:   static void Main(string[] args)
来源：http://ty.chemitech.net.cn

[M08] 获取系统与运行时信息
来源：http://la.jctech888.com.cn

Py:   platform.system();  platform.python_version()
来源：http://lc.szxytkj.cn

PHP:  PHP_OS;  phpversion();
来源：http://gv.huixiangedu.cn

JS:   process.platform;  process.version
来源：http://tk.nszjky.cn

TS:   process.platform;  process.version
来源：http://tf.szsharing.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://eg.nszjky.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ai.bjjhwx.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ii.wgjwhj.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ff.521024.cn

================================================================================
来源：http://pd.bookmarksfly.cn

N. 数据结构与算法
来源：http://fq.shxzskj.cn

================================================================================
来源：http://ud.bjjhwx.cn

[N01] 二分查找（有序数组）
来源：http://na.nicolike.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ox.bookmarksfly.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://sy.chemitech.net.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gw.shtwfgs.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sb.nszjky.cn

Java: Arrays.binarySearch(arr, x)
来源：http://bt.szsharing.cn

Go:   sort.SearchInts(arr, x)
来源：http://ag.huixinmuqiang.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ob.wgjwhj.cn

C#:   Array.BinarySearch(arr, x)
来源：http://gv.lnxyls.cn

[N02] 排序（工程实践用内置实现）
来源：http://zu.yuntaijiaju.cn

Py:   sorted(arr);  arr.sort()
来源：http://el.muxihuayi.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://oi.huixinmuqiang.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://dx.huixiangedu.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://gc.9csxet.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ui.panjiajie.cn

Go:   slices.Sort(arr)
来源：http://ut.hnjuh.cn

Ruby: arr.sort
来源：http://ot.hnjuh.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://wv.hnjuh.cn

[N03] 快速排序（分治示例）
来源：http://im.bjjhwx.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://dv.asd995.cn

PHP:  // 递归实现，或用 usort
来源：http://pr.haigaiapp.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zx.521024.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tw.hahajie.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.hahajie.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ky.jianghongdianzi.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://lx.521024.cn

C#:   // 手写递归，或 Array.Sort
来源：http://zf.colortex.cn

[N04] 斐波那契数列
来源：http://ly.shxzukj.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ga.9csxet.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://pd.newstarts.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gj.jianghongdianzi.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gp.szxytkj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://zq.nicolike.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ez.gzmigu.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://gh.szxytkj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://qw.huixinmuqiang.cn

[N05] 最大公约数
来源：http://um.yuexingan06.cn

Py:   math.gcd(a, b)
来源：http://vd.szxytkj.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://je.nszjky.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xo.521024.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vo.jctech888.com.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://lf.shtwfgs.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://dd.jctech888.com.cn

Ruby: a.gcd(b)
来源：http://hh.szxytkj.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://nh.gzmigu.cn

[N06] 判断回文字符串
来源：http://bx.colortex.cn

Py:   s == s[::-1]
来源：http://sv.chemitech.net.cn

PHP:  $s === strrev($s);
来源：http://bh.nicolike.cn

JS:   s === [...s].reverse().join("")
来源：http://ua.yuntaijiaju.cn

TS:   s === [...s].reverse().join("")
来源：http://de.shtwfgs.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://sv.panjiajie.cn

Go:   // 双指针从两端比较
来源：http://sj.hahajie.cn

Ruby: s == s.reverse
来源：http://cy.jctech888.com.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://jx.huanxung.cn

[N07] 两数之和（返回下标）
来源：http://cz.jctech888.com.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://oq.521024.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://xb.yuntaijiaju.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://mk.muxihuayi.cn

TS:   // 手写 Map<string, number>
来源：http://ix.hahajie.cn

Java: // 手写 HashMap
来源：http://yo.bjjhwx.cn

Go:   // 手写 map[int]int
来源：http://gj.hnjuh.cn

Ruby: // 手写 Hash
来源：http://qk.colortex.cn

C#:   // 手写 Dictionary<int, int>
来源：http://fn.9csxet.cn

[N08] 生成全排列
来源：http://ok.nicolike.cn

Py:   itertools.permutations(arr)
来源：http://ch.newstarts.cn

PHP:  // 手写递归交换
来源：http://xh.panjiajie.cn

JS:   // 手写回溯递归
来源：http://cz.bjjhwx.cn

TS:   // 手写回溯递归
来源：http://ny.shxzskj.cn

Java: // 手写回溯递归
来源：http://mc.huanxung.cn

Go:   // 手写回溯递归
来源：http://sr.nszjky.cn

Ruby: arr.permutation.to_a
来源：http://rw.lnxyls.cn

C#:   // 手写回溯递归
来源：http://eo.yuntaijiaju.cn

[N09] 栈与队列
来源：http://oh.shxzukj.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ty.jianghongdianzi.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://qi.lnxyls.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://vf.wgjwhj.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://md.jctech888.com.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://rh.yuexingan06.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://fa.muxihuayi.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://xs.hnjuh.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ay.yuexingan06.cn

[N10] 链表节点定义
来源：http://xw.shtwfgs.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ar.jctech888.com.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://xk.panjiajie.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://fv.shtwfgs.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://qz.hahajie.cn

Java: class Node { int v; Node next; }
来源：http://kz.shtwfgs.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ul.chemitech.net.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ky.hahajie.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ak.wgjwhj.cn

[N11] 二叉树中序遍历
来源：http://ey.shtwfgs.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wr.shtwfgs.cn

PHP:  // 手写递归函数
来源：http://kw.shxzukj.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ks.bjjhwx.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wi.yuntaijiaju.cn

Java: // 手写递归
来源：http://qd.shxzukj.cn

Go:   // 手写递归
来源：http://mz.shxzskj.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://or.szsharing.cn

C#:   // 手写递归
来源：http://lc.szxytkj.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ug.9csxet.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://kv.muxihuayi.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://le.yuexingan06.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mo.asd995.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wr.huixiangedu.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ob.gzmigu.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hx.chemitech.net.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://bs.jianghongdianzi.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://xl.shtwfgs.cn

================================================================================
来源：http://hx.lnxyls.cn

O. 并发与异步
来源：http://hn.chemitech.net.cn

================================================================================
来源：http://hy.shxzskj.cn

[O01] 启动一个线程
来源：http://bh.asd995.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://jy.jianghongdianzi.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://rj.chemitech.net.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mj.bjjhwx.cn

TS:   // 同 JS
来源：http://qv.chemitech.net.cn

Java: new Thread(() -> f()).start()
来源：http://qm.521024.cn

Go:   go f()
来源：http://cu.haigaiapp.cn

Ruby: Thread.new { f }
来源：http://aw.gzmigu.cn

C#:   Task.Run(() => F());
来源：http://wu.shtwfgs.cn

[O02] 使用线程池
来源：http://jn.hahajie.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ca.panjiajie.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://nk.szsharing.cn

JS:   // worker_threads 线程池
来源：http://sz.yuntaijiaju.cn

TS:   // worker_threads 线程池
来源：http://iw.wgjwhj.cn

Java: Executors.newFixedThreadPool(4)
来源：http://lp.shtwfgs.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://es.wgjwhj.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ku.huixinmuqiang.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ri.jctech888.com.cn

[O03] 加锁保护共享数据
来源：http://re.huanxung.cn

Py:   with lock: shared += 1
来源：http://aq.shxzukj.cn

PHP:  // 用 flock() 做文件锁
来源：http://eq.bjjhwx.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://lr.bookmarksfly.cn

TS:   // 同 JS
来源：http://rq.521024.cn

Java: synchronized (this) { shared++; }
来源：http://yj.nszjky.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://cd.newstarts.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://pn.szsharing.cn

C#:   lock (gate) { shared++; }
来源：http://la.jianghongdianzi.cn

[O04] 定义异步函数并等待
来源：http://zz.panjiajie.cn

Py:   async def f():⏎    await g()
来源：http://bx.jianghongdianzi.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ob.jctech888.com.cn

JS:   async function f() { await g(); }
来源：http://bp.hahajie.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://qk.yuntaijiaju.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ta.newstarts.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://js.huixiangedu.cn

Ruby: # 用 Fiber 或 async gem
来源：http://sg.jianghongdianzi.cn

C#:   async Task F() { await G(); }
来源：http://gg.szxytkj.cn

[O05] 并发执行并等待全部完成
来源：http://tc.521024.cn

Py:   asyncio.gather(*tasks)
来源：http://ak.szsharing.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://jk.szsharing.cn

JS:   await Promise.all(tasks)
来源：http://la.yuexingan06.cn

TS:   await Promise.all(tasks)
来源：http://qw.huixinmuqiang.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://kd.shtwfgs.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://do.chemitech.net.cn

Ruby: threads.map(&:join)
来源：http://eb.bjjhwx.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://we.9csxet.cn

[O06] 使用进程池
来源：http://db.9csxet.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://kt.9csxet.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://hm.wgjwhj.cn

JS:   // child_process / cluster 模块
来源：http://tx.hnjuh.cn

TS:   // child_process / cluster 模块
来源：http://ma.gzmigu.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://gp.newstarts.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://sg.shtwfgs.cn

Ruby: // fork 块
来源：http://ra.shxzukj.cn

C#:   Parallel.For
来源：http://wj.huixiangedu.cn

================================================================================
来源：http://ez.bjjhwx.cn

P. 常用工具函数
来源：http://jz.bookmarksfly.cn

================================================================================
来源：http://lr.huanxung.cn

[P01] 生成 UUID
来源：http://yt.szsharing.cn

Py:   str(uuid.uuid4())
来源：http://um.9csxet.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://sv.521024.cn

JS:   crypto.randomUUID()
来源：http://if.szxytkj.cn

TS:   crypto.randomUUID()
来源：http://bq.hahajie.cn

Java: UUID.randomUUID().toString()
来源：http://jy.hnjuh.cn

Go:   // 用 github.com/google/uuid
来源：http://js.yuexingan06.cn

Ruby: SecureRandom.uuid
来源：http://xq.huixiangedu.cn

C#:   Guid.NewGuid().ToString()
来源：http://yk.huanxung.cn

[P02] MD5 / SHA256 摘要
来源：http://il.shxzukj.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://gh.huixiangedu.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://vr.wgjwhj.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://yp.yuexingan06.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mx.hahajie.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mx.gzmigu.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://oh.nicolike.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://oj.huixiangedu.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://xk.jctech888.com.cn

[P03] 生成短随机字符串
来源：http://jn.newstarts.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://fj.jianghongdianzi.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://at.szsharing.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rn.hahajie.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fd.shtwfgs.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ko.shxzukj.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://qi.asd995.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://rr.jctech888.com.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ks.haigaiapp.cn

[P04] 求长度
来源：http://ia.muxihuayi.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ey.shtwfgs.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ox.9csxet.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://oy.jianghongdianzi.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jv.panjiajie.cn

Java: list.size();  map.size();  s.length()
来源：http://pd.chemitech.net.cn

Go:   len(arr);  len(m)
来源：http://ek.chemitech.net.cn

Ruby: x.length;  x.size
来源：http://mt.huixiangedu.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://mu.szsharing.cn

[P05] 判断两个对象内容是否相等
来源：http://ov.huanxung.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://fu.nszjky.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ga.szxytkj.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://gt.colortex.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://iw.szxytkj.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ez.muxihuayi.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ld.shxzskj.cn

Ruby: a == b
来源：http://xk.shxzskj.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ps.bjjhwx.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ch.szxytkj.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://qb.szxytkj.cn

PHP:  if (empty($x)) {}
来源：http://ph.yuntaijiaju.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://qu.huanxung.cn

TS:   if (x == null) {}
来源：http://jt.yuntaijiaju.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://nz.shxzukj.cn

Go:   if x == nil {}
来源：http://cw.szsharing.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ej.jctech888.com.cn

C#:   if (x is null) {}
来源：http://vl.bjjhwx.cn

[P07] 防抖与节流
来源：http://bs.nszjky.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://li.huanxung.cn

PHP:  // 手写时间戳比较
来源：http://aq.haigaiapp.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hd.yuntaijiaju.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sd.colortex.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://tw.jianghongdianzi.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://uo.yuntaijiaju.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://re.newstarts.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hk.gzmigu.cn

[P08] 处理浮点精度问题
来源：http://br.chemitech.net.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://bs.bjjhwx.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ot.yuntaijiaju.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://md.newstarts.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ey.panjiajie.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://uf.szsharing.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://rk.haigaiapp.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://xs.shxzskj.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://nt.panjiajie.cn

================================================================================
来源：http://cy.shxzskj.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://nj.hahajie.cn

================================================================================
来源：http://iu.gzmigu.cn

[Q01] 创建表
来源：http://ze.chemitech.net.cn

CREATE TABLE users (
来源：http://la.huixiangedu.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://et.asd995.cn

name VARCHAR(50) NOT NULL,
来源：http://zt.hahajie.cn

email VARCHAR(100) UNIQUE,
来源：http://rk.hnjuh.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ok.szxytkj.cn

);
来源：http://yh.huanxung.cn

[Q02] 创建带外键的表
来源：http://an.yuntaijiaju.cn

CREATE TABLE orders (
来源：http://em.jctech888.com.cn


<!-- 参考信息 -->