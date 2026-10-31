代发 wailian999

TS:   process.cwd()
来源：http://rz.chemitech.net.cn

Java: Path.of("").toAbsolutePath()
来源：http://sk.bookmarksfly.cn

Go:   os.Getwd()
来源：http://ux.szxytkj.cn

Ruby: Dir.pwd
来源：http://yy.jctech888.com.cn

C#:   Directory.GetCurrentDirectory()
来源：http://px.wgjwhj.cn

[M05] 设置退出码
来源：http://qx.asd995.cn

Py:   sys.exit(1)
来源：http://az.jianghongdianzi.cn

PHP:  exit(1);
来源：http://eb.yuntaijiaju.cn

JS:   process.exit(1)
来源：http://tj.shxzukj.cn

TS:   process.exit(1)
来源：http://vi.nszjky.cn

Java: System.exit(1)
来源：http://ra.asd995.cn

Go:   os.Exit(1)
来源：http://zt.jianghongdianzi.cn

Ruby: exit 1
来源：http://qs.9csxet.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://oo.panjiajie.cn

[M06] 向标准错误输出
来源：http://do.9csxet.cn

Py:   print("err", file=sys.stderr)
来源：http://mk.yuexingan06.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://co.huixiangedu.cn

JS:   console.error("err")
来源：http://lv.lnxyls.cn

TS:   console.error("err")
来源：http://ko.9csxet.cn

Java: System.err.println("err")
来源：http://rh.521024.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://to.wgjwhj.cn

Ruby: warn "err"
来源：http://rx.colortex.cn

C#:   Console.Error.WriteLine("err")
来源：http://do.bookmarksfly.cn

[M07] 判断是否为主入口
来源：http://vi.huanxung.cn

Py:   if __name__ == "__main__":
来源：http://yn.gzmigu.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://zg.szsharing.cn

JS:   require.main === module
来源：http://gd.yuexingan06.cn

TS:   require.main === module
来源：http://jz.bjjhwx.cn

Java: public static void main(String[] args)
来源：http://vz.yuexingan06.cn

Go:   func main()
来源：http://en.nszjky.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://kv.bookmarksfly.cn

C#:   static void Main(string[] args)
来源：http://fi.jctech888.com.cn

[M08] 获取系统与运行时信息
来源：http://uq.hnjuh.cn

Py:   platform.system();  platform.python_version()
来源：http://cz.huanxung.cn

PHP:  PHP_OS;  phpversion();
来源：http://tf.nicolike.cn

JS:   process.platform;  process.version
来源：http://od.shtwfgs.cn

TS:   process.platform;  process.version
来源：http://tm.haigaiapp.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://th.haigaiapp.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://xq.521024.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://si.shtwfgs.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://xt.bjjhwx.cn

================================================================================
来源：http://zv.wgjwhj.cn

N. 数据结构与算法
来源：http://rz.szsharing.cn

================================================================================
来源：http://bm.hnjuh.cn

[N01] 二分查找（有序数组）
来源：http://ox.yuntaijiaju.cn

Py:   bisect.bisect_left(arr, x)
来源：http://th.chemitech.net.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://eb.panjiajie.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fo.shxzukj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ov.chemitech.net.cn

Java: Arrays.binarySearch(arr, x)
来源：http://aj.huixinmuqiang.cn

Go:   sort.SearchInts(arr, x)
来源：http://bq.nicolike.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://xs.jctech888.com.cn

C#:   Array.BinarySearch(arr, x)
来源：http://wt.jctech888.com.cn

[N02] 排序（工程实践用内置实现）
来源：http://vj.hahajie.cn

Py:   sorted(arr);  arr.sort()
来源：http://qh.shxzskj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://xo.hnjuh.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://co.bjjhwx.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://vh.wgjwhj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://fe.szsharing.cn

Go:   slices.Sort(arr)
来源：http://gz.yuexingan06.cn

Ruby: arr.sort
来源：http://xd.szxytkj.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ip.huixiangedu.cn

[N03] 快速排序（分治示例）
来源：http://xp.shtwfgs.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://uw.asd995.cn

PHP:  // 递归实现，或用 usort
来源：http://ju.szxytkj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ta.muxihuayi.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xk.lnxyls.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://po.lnxyls.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://db.haigaiapp.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://gj.521024.cn

C#:   // 手写递归，或 Array.Sort
来源：http://hm.hnjuh.cn

[N04] 斐波那契数列
来源：http://td.huixiangedu.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ug.gzmigu.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://kg.huanxung.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cg.shtwfgs.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://km.shxzskj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://zq.muxihuayi.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://bm.asd995.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://nk.szxytkj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://rm.haigaiapp.cn

[N05] 最大公约数
来源：http://yr.hnjuh.cn

Py:   math.gcd(a, b)
来源：http://nv.szxytkj.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mn.nicolike.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yi.wgjwhj.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bq.colortex.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://fj.shxzukj.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wt.jianghongdianzi.cn

Ruby: a.gcd(b)
来源：http://la.haigaiapp.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://vp.muxihuayi.cn

[N06] 判断回文字符串
来源：http://di.newstarts.cn

Py:   s == s[::-1]
来源：http://zo.huixinmuqiang.cn

PHP:  $s === strrev($s);
来源：http://qo.nicolike.cn

JS:   s === [...s].reverse().join("")
来源：http://ee.chemitech.net.cn

TS:   s === [...s].reverse().join("")
来源：http://md.chemitech.net.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mf.yuntaijiaju.cn

Go:   // 双指针从两端比较
来源：http://hn.gzmigu.cn

Ruby: s == s.reverse
来源：http://lr.jctech888.com.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ni.huanxung.cn

[N07] 两数之和（返回下标）
来源：http://yt.bookmarksfly.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wh.nszjky.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://lt.huixinmuqiang.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://pp.chemitech.net.cn

TS:   // 手写 Map<string, number>
来源：http://lm.panjiajie.cn

Java: // 手写 HashMap
来源：http://gc.colortex.cn

Go:   // 手写 map[int]int
来源：http://cn.panjiajie.cn

Ruby: // 手写 Hash
来源：http://yb.gzmigu.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ov.shtwfgs.cn

[N08] 生成全排列
来源：http://nm.jctech888.com.cn

Py:   itertools.permutations(arr)
来源：http://pt.huixinmuqiang.cn

PHP:  // 手写递归交换
来源：http://dn.chemitech.net.cn

JS:   // 手写回溯递归
来源：http://rm.shxzukj.cn

TS:   // 手写回溯递归
来源：http://og.521024.cn

Java: // 手写回溯递归
来源：http://iy.nicolike.cn

Go:   // 手写回溯递归
来源：http://tx.panjiajie.cn

Ruby: arr.permutation.to_a
来源：http://sv.chemitech.net.cn

C#:   // 手写回溯递归
来源：http://ad.lnxyls.cn

[N09] 栈与队列
来源：http://xs.huixiangedu.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ly.shxzukj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://sm.hahajie.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ty.shtwfgs.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://nl.chemitech.net.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://xx.wgjwhj.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://og.huixinmuqiang.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mt.bjjhwx.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ye.huixinmuqiang.cn

[N10] 链表节点定义
来源：http://jw.521024.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://gq.bjjhwx.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://rk.521024.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ue.shtwfgs.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ab.bookmarksfly.cn

Java: class Node { int v; Node next; }
来源：http://zm.panjiajie.cn

Go:   type Node struct { V int; Next *Node }
来源：http://hd.jctech888.com.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://fr.asd995.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://tw.lnxyls.cn

[N11] 二叉树中序遍历
来源：http://rd.jianghongdianzi.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://gu.newstarts.cn

PHP:  // 手写递归函数
来源：http://yb.huanxung.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ty.yuntaijiaju.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kz.yuntaijiaju.cn

Java: // 手写递归
来源：http://ko.wgjwhj.cn

Go:   // 手写递归
来源：http://ca.chemitech.net.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://yo.yuexingan06.cn

C#:   // 手写递归
来源：http://oy.huixiangedu.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://bn.yuntaijiaju.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ao.newstarts.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://sn.jianghongdianzi.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bz.521024.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://aq.panjiajie.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ke.huixinmuqiang.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://iy.shtwfgs.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://gr.asd995.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://lz.jianghongdianzi.cn

================================================================================
来源：http://uc.szsharing.cn

O. 并发与异步
来源：http://wo.9csxet.cn

================================================================================
来源：http://co.hahajie.cn

[O01] 启动一个线程
来源：http://sr.nicolike.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://fn.newstarts.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://uz.lnxyls.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://lp.bookmarksfly.cn

TS:   // 同 JS
来源：http://sl.shxzskj.cn

Java: new Thread(() -> f()).start()
来源：http://nq.haigaiapp.cn

Go:   go f()
来源：http://xa.bookmarksfly.cn

Ruby: Thread.new { f }
来源：http://lk.nszjky.cn

C#:   Task.Run(() => F());
来源：http://ou.huixiangedu.cn

[O02] 使用线程池
来源：http://tj.lnxyls.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://op.szxytkj.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://xb.jianghongdianzi.cn

JS:   // worker_threads 线程池
来源：http://wg.bookmarksfly.cn

TS:   // worker_threads 线程池
来源：http://qn.szsharing.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ki.yuexingan06.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://fx.nicolike.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ct.shxzskj.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ae.bjjhwx.cn

[O03] 加锁保护共享数据
来源：http://oe.panjiajie.cn

Py:   with lock: shared += 1
来源：http://zg.hnjuh.cn

PHP:  // 用 flock() 做文件锁
来源：http://ly.asd995.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://rr.newstarts.cn

TS:   // 同 JS
来源：http://xf.lnxyls.cn

Java: synchronized (this) { shared++; }
来源：http://ji.newstarts.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://gd.jctech888.com.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ba.chemitech.net.cn

C#:   lock (gate) { shared++; }
来源：http://gq.gzmigu.cn

[O04] 定义异步函数并等待
来源：http://lo.shxzukj.cn

Py:   async def f():⏎    await g()
来源：http://lx.hnjuh.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://am.haigaiapp.cn

JS:   async function f() { await g(); }
来源：http://kp.wgjwhj.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://xs.shxzskj.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://nx.chemitech.net.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://bd.shxzukj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://lx.wgjwhj.cn

C#:   async Task F() { await G(); }
来源：http://ed.bookmarksfly.cn

[O05] 并发执行并等待全部完成
来源：http://ac.shxzskj.cn

Py:   asyncio.gather(*tasks)
来源：http://de.szsharing.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://yj.chemitech.net.cn

JS:   await Promise.all(tasks)
来源：http://ya.szxytkj.cn

TS:   await Promise.all(tasks)
来源：http://zh.szsharing.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ec.bjjhwx.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://fr.asd995.cn

Ruby: threads.map(&:join)
来源：http://ln.yuexingan06.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://pq.yuntaijiaju.cn

[O06] 使用进程池
来源：http://as.panjiajie.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://pk.nicolike.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ui.colortex.cn

JS:   // child_process / cluster 模块
来源：http://wq.muxihuayi.cn

TS:   // child_process / cluster 模块
来源：http://sn.szxytkj.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://au.bjjhwx.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://cm.jctech888.com.cn

Ruby: // fork 块
来源：http://vi.chemitech.net.cn

C#:   Parallel.For
来源：http://uu.yuexingan06.cn

================================================================================
来源：http://aq.huixiangedu.cn

P. 常用工具函数
来源：http://qg.gzmigu.cn

================================================================================
来源：http://fe.shxzskj.cn

[P01] 生成 UUID
来源：http://tn.nicolike.cn

Py:   str(uuid.uuid4())
来源：http://dd.wgjwhj.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://oi.colortex.cn

JS:   crypto.randomUUID()
来源：http://qf.panjiajie.cn

TS:   crypto.randomUUID()
来源：http://mb.szsharing.cn

Java: UUID.randomUUID().toString()
来源：http://bq.bookmarksfly.cn

Go:   // 用 github.com/google/uuid
来源：http://ss.huixiangedu.cn

Ruby: SecureRandom.uuid
来源：http://vr.wgjwhj.cn

C#:   Guid.NewGuid().ToString()
来源：http://ki.colortex.cn

[P02] MD5 / SHA256 摘要
来源：http://zi.haigaiapp.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://cc.shxzskj.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://sn.lnxyls.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://pl.hahajie.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://bg.wgjwhj.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://gw.chemitech.net.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://vv.panjiajie.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://cg.nicolike.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://uz.jianghongdianzi.cn

[P03] 生成短随机字符串
来源：http://au.bjjhwx.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://rw.nszjky.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hx.gzmigu.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cr.9csxet.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mg.hnjuh.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ne.newstarts.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://cw.521024.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ss.szxytkj.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://et.muxihuayi.cn

[P04] 求长度
来源：http://lc.muxihuayi.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ok.shtwfgs.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rb.szsharing.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cy.newstarts.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ue.shxzskj.cn

Java: list.size();  map.size();  s.length()
来源：http://id.yuntaijiaju.cn

Go:   len(arr);  len(m)
来源：http://tv.yuntaijiaju.cn

Ruby: x.length;  x.size
来源：http://xf.521024.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://zp.shxzukj.cn

[P05] 判断两个对象内容是否相等
来源：http://qe.newstarts.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://wd.shxzukj.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://uh.bookmarksfly.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://pm.shtwfgs.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://xt.szsharing.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://qy.521024.cn

Go:   reflect.DeepEqual(a, b)
来源：http://wc.jctech888.com.cn

Ruby: a == b
来源：http://mv.huanxung.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://pl.szxytkj.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://zg.lnxyls.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://jc.huanxung.cn

PHP:  if (empty($x)) {}
来源：http://em.bjjhwx.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://gx.9csxet.cn

TS:   if (x == null) {}
来源：http://zc.hahajie.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://me.yuntaijiaju.cn

Go:   if x == nil {}
来源：http://td.hahajie.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://kv.bookmarksfly.cn

C#:   if (x is null) {}
来源：http://uo.haigaiapp.cn

[P07] 防抖与节流
来源：http://cy.nicolike.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://iw.shtwfgs.cn

PHP:  // 手写时间戳比较
来源：http://bw.nicolike.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ys.nszjky.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://be.colortex.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://gy.bjjhwx.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://om.szxytkj.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://jj.yuexingan06.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ls.shxzskj.cn

[P08] 处理浮点精度问题
来源：http://ew.huixiangedu.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://dx.wgjwhj.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://vx.shxzukj.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://li.wgjwhj.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ur.haigaiapp.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://yu.hnjuh.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://yc.colortex.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://su.yuexingan06.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://gm.szxytkj.cn

================================================================================
来源：http://hp.shtwfgs.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://el.jianghongdianzi.cn

================================================================================
来源：http://lw.nszjky.cn

[Q01] 创建表
来源：http://bx.chemitech.net.cn

CREATE TABLE users (
来源：http://ko.yuntaijiaju.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://kb.jctech888.com.cn

name VARCHAR(50) NOT NULL,
来源：http://wl.hnjuh.cn

email VARCHAR(100) UNIQUE,
来源：http://ef.szsharing.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://rc.nicolike.cn

);
来源：http://nu.newstarts.cn

[Q02] 创建带外键的表
来源：http://ie.shtwfgs.cn

CREATE TABLE orders (
来源：http://hm.shtwfgs.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ze.chemitech.net.cn

user_id INT NOT NULL,
来源：http://fd.newstarts.cn

amount DECIMAL(10, 2),
来源：http://ek.haigaiapp.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://fl.muxihuayi.cn


<!-- 参考信息 -->