代发 wailian999

C#:   Directory.GetCurrentDirectory()
来源：http://nh.huanxung.cn

[M05] 设置退出码
来源：http://lt.panjiajie.cn

Py:   sys.exit(1)
来源：http://cc.muxihuayi.cn

PHP:  exit(1);
来源：http://ct.521024.cn

JS:   process.exit(1)
来源：http://hr.nszjky.cn

TS:   process.exit(1)
来源：http://fq.yuexingan06.cn

Java: System.exit(1)
来源：http://tp.yuexingan06.cn

Go:   os.Exit(1)
来源：http://dg.hnjuh.cn

Ruby: exit 1
来源：http://xc.yuntaijiaju.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://te.wgjwhj.cn

[M06] 向标准错误输出
来源：http://my.nicolike.cn

Py:   print("err", file=sys.stderr)
来源：http://bj.521024.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://wl.jianghongdianzi.cn

JS:   console.error("err")
来源：http://vr.gzmigu.cn

TS:   console.error("err")
来源：http://uc.wgjwhj.cn

Java: System.err.println("err")
来源：http://uy.huixiangedu.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://as.yuntaijiaju.cn

Ruby: warn "err"
来源：http://qw.asd995.cn

C#:   Console.Error.WriteLine("err")
来源：http://jp.szxytkj.cn

[M07] 判断是否为主入口
来源：http://qq.szxytkj.cn

Py:   if __name__ == "__main__":
来源：http://lu.gzmigu.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://rh.hahajie.cn

JS:   require.main === module
来源：http://am.panjiajie.cn

TS:   require.main === module
来源：http://ja.shxzukj.cn

Java: public static void main(String[] args)
来源：http://fn.shxzskj.cn

Go:   func main()
来源：http://hw.bookmarksfly.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://zt.yuntaijiaju.cn

C#:   static void Main(string[] args)
来源：http://mn.bookmarksfly.cn

[M08] 获取系统与运行时信息
来源：http://na.yuexingan06.cn

Py:   platform.system();  platform.python_version()
来源：http://aw.gzmigu.cn

PHP:  PHP_OS;  phpversion();
来源：http://im.yuntaijiaju.cn

JS:   process.platform;  process.version
来源：http://nj.yuntaijiaju.cn

TS:   process.platform;  process.version
来源：http://ox.gzmigu.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ak.yuexingan06.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://qs.lnxyls.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ik.colortex.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://nm.gzmigu.cn

================================================================================
来源：http://xr.bookmarksfly.cn

N. 数据结构与算法
来源：http://ch.yuntaijiaju.cn

================================================================================
来源：http://vm.haigaiapp.cn

[N01] 二分查找（有序数组）
来源：http://ag.hnjuh.cn

Py:   bisect.bisect_left(arr, x)
来源：http://pz.yuexingan06.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://sl.nszjky.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ht.hnjuh.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fr.bookmarksfly.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ry.huixinmuqiang.cn

Go:   sort.SearchInts(arr, x)
来源：http://vw.colortex.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://df.9csxet.cn

C#:   Array.BinarySearch(arr, x)
来源：http://es.huixiangedu.cn

[N02] 排序（工程实践用内置实现）
来源：http://sh.521024.cn

Py:   sorted(arr);  arr.sort()
来源：http://cj.yuntaijiaju.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://gy.9csxet.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://qz.chemitech.net.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://yp.yuntaijiaju.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ya.bookmarksfly.cn

Go:   slices.Sort(arr)
来源：http://so.nszjky.cn

Ruby: arr.sort
来源：http://mh.yuexingan06.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://bs.jctech888.com.cn

[N03] 快速排序（分治示例）
来源：http://is.panjiajie.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://vm.chemitech.net.cn

PHP:  // 递归实现，或用 usort
来源：http://gh.521024.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fl.yuexingan06.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gv.shxzukj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://xy.muxihuayi.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ps.szxytkj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://rj.yuntaijiaju.cn

C#:   // 手写递归，或 Array.Sort
来源：http://rg.hnjuh.cn

[N04] 斐波那契数列
来源：http://mj.nicolike.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wh.wgjwhj.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ic.yuexingan06.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lo.colortex.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zg.gzmigu.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ew.colortex.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://jz.wgjwhj.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ay.shxzskj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://eu.newstarts.cn

[N05] 最大公约数
来源：http://sl.yuexingan06.cn

Py:   math.gcd(a, b)
来源：http://mf.yuexingan06.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hn.haigaiapp.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hn.colortex.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ic.szsharing.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://iq.jianghongdianzi.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ng.bjjhwx.cn

Ruby: a.gcd(b)
来源：http://qo.jianghongdianzi.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ki.szsharing.cn

[N06] 判断回文字符串
来源：http://ra.nszjky.cn

Py:   s == s[::-1]
来源：http://ds.huixinmuqiang.cn

PHP:  $s === strrev($s);
来源：http://dj.szsharing.cn

JS:   s === [...s].reverse().join("")
来源：http://ud.jianghongdianzi.cn

TS:   s === [...s].reverse().join("")
来源：http://oc.szxytkj.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://py.jianghongdianzi.cn

Go:   // 双指针从两端比较
来源：http://ga.chemitech.net.cn

Ruby: s == s.reverse
来源：http://ff.newstarts.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://mw.huixinmuqiang.cn

[N07] 两数之和（返回下标）
来源：http://ht.yuexingan06.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ah.colortex.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://rl.newstarts.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://sd.haigaiapp.cn

TS:   // 手写 Map<string, number>
来源：http://dc.shxzukj.cn

Java: // 手写 HashMap
来源：http://qk.chemitech.net.cn

Go:   // 手写 map[int]int
来源：http://jc.bjjhwx.cn

Ruby: // 手写 Hash
来源：http://qs.huixinmuqiang.cn

C#:   // 手写 Dictionary<int, int>
来源：http://vg.panjiajie.cn

[N08] 生成全排列
来源：http://hr.bookmarksfly.cn

Py:   itertools.permutations(arr)
来源：http://gr.shtwfgs.cn

PHP:  // 手写递归交换
来源：http://ge.gzmigu.cn

JS:   // 手写回溯递归
来源：http://ei.wgjwhj.cn

TS:   // 手写回溯递归
来源：http://om.yuexingan06.cn

Java: // 手写回溯递归
来源：http://ys.shtwfgs.cn

Go:   // 手写回溯递归
来源：http://tv.bjjhwx.cn

Ruby: arr.permutation.to_a
来源：http://oz.bookmarksfly.cn

C#:   // 手写回溯递归
来源：http://vv.newstarts.cn

[N09] 栈与队列
来源：http://kb.shxzskj.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://rm.shxzskj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://dn.yuexingan06.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hk.huanxung.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://is.chemitech.net.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://as.shxzukj.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://gp.asd995.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://no.gzmigu.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://rh.521024.cn

[N10] 链表节点定义
来源：http://mz.haigaiapp.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ua.muxihuayi.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://us.hnjuh.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://cx.jianghongdianzi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ov.szsharing.cn

Java: class Node { int v; Node next; }
来源：http://xr.haigaiapp.cn

Go:   type Node struct { V int; Next *Node }
来源：http://oc.asd995.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://pc.yuntaijiaju.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://qt.huixinmuqiang.cn

[N11] 二叉树中序遍历
来源：http://bs.asd995.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://lm.chemitech.net.cn

PHP:  // 手写递归函数
来源：http://ge.9csxet.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kx.muxihuayi.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fg.panjiajie.cn

Java: // 手写递归
来源：http://jx.yuexingan06.cn

Go:   // 手写递归
来源：http://vn.yuntaijiaju.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://gf.newstarts.cn

C#:   // 手写递归
来源：http://vu.yuntaijiaju.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://nm.bookmarksfly.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://up.huixiangedu.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://nh.chemitech.net.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://si.lnxyls.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ex.shxzukj.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://aq.panjiajie.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://il.huixiangedu.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://rb.asd995.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://os.huixinmuqiang.cn

================================================================================
来源：http://yx.gzmigu.cn

O. 并发与异步
来源：http://hu.nicolike.cn

================================================================================
来源：http://mq.9csxet.cn

[O01] 启动一个线程
来源：http://uf.huanxung.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://rf.colortex.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://vk.wgjwhj.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ag.gzmigu.cn

TS:   // 同 JS
来源：http://og.haigaiapp.cn

Java: new Thread(() -> f()).start()
来源：http://cx.gzmigu.cn

Go:   go f()
来源：http://vn.haigaiapp.cn

Ruby: Thread.new { f }
来源：http://te.yuexingan06.cn

C#:   Task.Run(() => F());
来源：http://cu.huanxung.cn

[O02] 使用线程池
来源：http://bv.muxihuayi.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://oq.newstarts.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://xa.nszjky.cn

JS:   // worker_threads 线程池
来源：http://vk.shxzukj.cn

TS:   // worker_threads 线程池
来源：http://gn.huixinmuqiang.cn

Java: Executors.newFixedThreadPool(4)
来源：http://pf.szsharing.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://nr.szsharing.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ov.nszjky.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://lk.huixiangedu.cn

[O03] 加锁保护共享数据
来源：http://hb.gzmigu.cn

Py:   with lock: shared += 1
来源：http://ez.szsharing.cn

PHP:  // 用 flock() 做文件锁
来源：http://rv.chemitech.net.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ju.shxzskj.cn

TS:   // 同 JS
来源：http://gd.bjjhwx.cn

Java: synchronized (this) { shared++; }
来源：http://tz.wgjwhj.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://sm.hnjuh.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://xk.colortex.cn

C#:   lock (gate) { shared++; }
来源：http://jt.jianghongdianzi.cn

[O04] 定义异步函数并等待
来源：http://lt.bookmarksfly.cn

Py:   async def f():⏎    await g()
来源：http://nx.chemitech.net.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://kr.muxihuayi.cn

JS:   async function f() { await g(); }
来源：http://pl.asd995.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://eh.521024.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://vl.shxzskj.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ek.jianghongdianzi.cn

Ruby: # 用 Fiber 或 async gem
来源：http://rg.huanxung.cn

C#:   async Task F() { await G(); }
来源：http://xk.nicolike.cn

[O05] 并发执行并等待全部完成
来源：http://bh.jctech888.com.cn

Py:   asyncio.gather(*tasks)
来源：http://uf.shxzukj.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://uy.nicolike.cn

JS:   await Promise.all(tasks)
来源：http://jg.chemitech.net.cn

TS:   await Promise.all(tasks)
来源：http://ob.huanxung.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://pw.szsharing.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://dy.nszjky.cn

Ruby: threads.map(&:join)
来源：http://yg.bjjhwx.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://fj.jianghongdianzi.cn

[O06] 使用进程池
来源：http://uc.huixinmuqiang.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://yp.lnxyls.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://pv.hahajie.cn

JS:   // child_process / cluster 模块
来源：http://ry.huanxung.cn

TS:   // child_process / cluster 模块
来源：http://bo.nszjky.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://oz.bjjhwx.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ck.muxihuayi.cn

Ruby: // fork 块
来源：http://fx.huixinmuqiang.cn

C#:   Parallel.For
来源：http://fm.yuntaijiaju.cn

================================================================================
来源：http://ye.colortex.cn

P. 常用工具函数
来源：http://op.nszjky.cn

================================================================================
来源：http://bo.nszjky.cn

[P01] 生成 UUID
来源：http://ir.muxihuayi.cn

Py:   str(uuid.uuid4())
来源：http://ky.hnjuh.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://nt.huixinmuqiang.cn

JS:   crypto.randomUUID()
来源：http://mb.shtwfgs.cn

TS:   crypto.randomUUID()
来源：http://me.chemitech.net.cn

Java: UUID.randomUUID().toString()
来源：http://bu.shtwfgs.cn

Go:   // 用 github.com/google/uuid
来源：http://tj.huanxung.cn

Ruby: SecureRandom.uuid
来源：http://zq.shxzukj.cn

C#:   Guid.NewGuid().ToString()
来源：http://xa.szsharing.cn

[P02] MD5 / SHA256 摘要
来源：http://lm.shxzukj.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://nt.yuntaijiaju.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://cf.9csxet.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://cd.9csxet.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mx.huixiangedu.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ko.huixiangedu.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://kr.521024.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://sz.shxzukj.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://zi.hahajie.cn

[P03] 生成短随机字符串
来源：http://kq.panjiajie.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://sq.shxzukj.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ew.haigaiapp.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fp.chemitech.net.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vr.haigaiapp.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://lk.szsharing.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ey.hnjuh.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ol.haigaiapp.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://zn.jctech888.com.cn

[P04] 求长度
来源：http://qh.szsharing.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://uy.shtwfgs.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kd.yuexingan06.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bn.huixinmuqiang.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xi.lnxyls.cn

Java: list.size();  map.size();  s.length()
来源：http://zj.asd995.cn

Go:   len(arr);  len(m)
来源：http://ha.yuexingan06.cn

Ruby: x.length;  x.size
来源：http://nv.jianghongdianzi.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ue.panjiajie.cn

[P05] 判断两个对象内容是否相等
来源：http://rg.asd995.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://is.jctech888.com.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://cf.jctech888.com.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://fk.panjiajie.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://dg.shxzukj.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://pe.muxihuayi.cn

Go:   reflect.DeepEqual(a, b)
来源：http://te.bookmarksfly.cn

Ruby: a == b
来源：http://zz.szsharing.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ks.jianghongdianzi.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://of.shxzskj.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://qk.szxytkj.cn

PHP:  if (empty($x)) {}
来源：http://nz.huanxung.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://pf.chemitech.net.cn

TS:   if (x == null) {}
来源：http://hm.gzmigu.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://tf.colortex.cn

Go:   if x == nil {}
来源：http://qw.521024.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://fh.newstarts.cn

C#:   if (x is null) {}
来源：http://fo.hnjuh.cn

[P07] 防抖与节流
来源：http://cu.jianghongdianzi.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://tu.jianghongdianzi.cn

PHP:  // 手写时间戳比较
来源：http://zz.shxzskj.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lt.newstarts.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pv.shtwfgs.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wc.szsharing.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://cf.huixiangedu.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://tu.colortex.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://oj.lnxyls.cn

[P08] 处理浮点精度问题
来源：http://kn.bookmarksfly.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://jr.chemitech.net.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mo.huixiangedu.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://gh.shxzukj.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://uu.hahajie.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://bl.haigaiapp.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://yv.huanxung.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://od.nszjky.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://kt.yuntaijiaju.cn

================================================================================
来源：http://ov.huixinmuqiang.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://dp.szsharing.cn

================================================================================
来源：http://bq.chemitech.net.cn

[Q01] 创建表
来源：http://rv.newstarts.cn

CREATE TABLE users (
来源：http://qk.huixinmuqiang.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://zx.huixinmuqiang.cn

name VARCHAR(50) NOT NULL,
来源：http://ly.yuexingan06.cn

email VARCHAR(100) UNIQUE,
来源：http://bx.colortex.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://xc.asd995.cn

);
来源：http://oz.yuntaijiaju.cn

[Q02] 创建带外键的表
来源：http://fr.hnjuh.cn

CREATE TABLE orders (
来源：http://ba.nicolike.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://qw.bjjhwx.cn

user_id INT NOT NULL,
来源：http://wi.jianghongdianzi.cn

amount DECIMAL(10, 2),
来源：http://fj.nszjky.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://zp.nszjky.cn

);
来源：http://qr.jctech888.com.cn

[Q03] 增加列
来源：http://bf.szxytkj.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://be.bjjhwx.cn

[Q04] 修改列类型
来源：http://tr.jianghongdianzi.cn


<!-- 参考信息 -->