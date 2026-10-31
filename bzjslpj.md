代发 wailian999

C#:   Directory.GetCurrentDirectory()
来源：http://os.bookmarksfly.cn

[M05] 设置退出码
来源：http://do.nszjky.cn

Py:   sys.exit(1)
来源：http://ts.huanxung.cn

PHP:  exit(1);
来源：http://xy.yuntaijiaju.cn

JS:   process.exit(1)
来源：http://fd.9csxet.cn

TS:   process.exit(1)
来源：http://wq.bjjhwx.cn

Java: System.exit(1)
来源：http://ki.colortex.cn

Go:   os.Exit(1)
来源：http://ij.bookmarksfly.cn

Ruby: exit 1
来源：http://vo.hahajie.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ce.huixinmuqiang.cn

[M06] 向标准错误输出
来源：http://ql.shxzskj.cn

Py:   print("err", file=sys.stderr)
来源：http://dl.colortex.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://fq.9csxet.cn

JS:   console.error("err")
来源：http://ze.hahajie.cn

TS:   console.error("err")
来源：http://gi.9csxet.cn

Java: System.err.println("err")
来源：http://jp.yuexingan06.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://oq.newstarts.cn

Ruby: warn "err"
来源：http://vf.wgjwhj.cn

C#:   Console.Error.WriteLine("err")
来源：http://ii.gzmigu.cn

[M07] 判断是否为主入口
来源：http://mt.yuexingan06.cn

Py:   if __name__ == "__main__":
来源：http://qu.asd995.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://pk.newstarts.cn

JS:   require.main === module
来源：http://dv.huanxung.cn

TS:   require.main === module
来源：http://mz.bjjhwx.cn

Java: public static void main(String[] args)
来源：http://mr.lnxyls.cn

Go:   func main()
来源：http://hr.panjiajie.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://yx.jctech888.com.cn

C#:   static void Main(string[] args)
来源：http://dk.szxytkj.cn

[M08] 获取系统与运行时信息
来源：http://nw.szxytkj.cn

Py:   platform.system();  platform.python_version()
来源：http://nu.lnxyls.cn

PHP:  PHP_OS;  phpversion();
来源：http://uf.muxihuayi.cn

JS:   process.platform;  process.version
来源：http://jh.shxzskj.cn

TS:   process.platform;  process.version
来源：http://jc.lnxyls.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://lq.nszjky.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://eg.panjiajie.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://rv.shxzukj.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://gn.szsharing.cn

================================================================================
来源：http://xu.nicolike.cn

N. 数据结构与算法
来源：http://hy.chemitech.net.cn

================================================================================
来源：http://yg.chemitech.net.cn

[N01] 二分查找（有序数组）
来源：http://dz.chemitech.net.cn

Py:   bisect.bisect_left(arr, x)
来源：http://mn.szsharing.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ig.muxihuayi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mc.shxzukj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://md.hnjuh.cn

Java: Arrays.binarySearch(arr, x)
来源：http://yr.wgjwhj.cn

Go:   sort.SearchInts(arr, x)
来源：http://hx.hahajie.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://pj.nszjky.cn

C#:   Array.BinarySearch(arr, x)
来源：http://fz.huixiangedu.cn

[N02] 排序（工程实践用内置实现）
来源：http://aw.gzmigu.cn

Py:   sorted(arr);  arr.sort()
来源：http://ru.hahajie.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://jn.colortex.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://az.9csxet.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://za.bjjhwx.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ko.wgjwhj.cn

Go:   slices.Sort(arr)
来源：http://el.huixinmuqiang.cn

Ruby: arr.sort
来源：http://mf.huanxung.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://dn.hnjuh.cn

[N03] 快速排序（分治示例）
来源：http://tl.9csxet.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://vx.haigaiapp.cn

PHP:  // 递归实现，或用 usort
来源：http://bz.yuntaijiaju.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vm.szsharing.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tn.muxihuayi.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://td.newstarts.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://vy.newstarts.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://un.szsharing.cn

C#:   // 手写递归，或 Array.Sort
来源：http://js.jctech888.com.cn

[N04] 斐波那契数列
来源：http://nm.lnxyls.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wq.shxzukj.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://fm.haigaiapp.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sm.colortex.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kh.shtwfgs.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://fy.lnxyls.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://vd.nszjky.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://tp.haigaiapp.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://rk.bjjhwx.cn

[N05] 最大公约数
来源：http://eb.panjiajie.cn

Py:   math.gcd(a, b)
来源：http://zf.szxytkj.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://og.lnxyls.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ug.jianghongdianzi.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://af.jianghongdianzi.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://uw.asd995.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://bi.nszjky.cn

Ruby: a.gcd(b)
来源：http://fn.panjiajie.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ap.shxzukj.cn

[N06] 判断回文字符串
来源：http://oq.hahajie.cn

Py:   s == s[::-1]
来源：http://ze.haigaiapp.cn

PHP:  $s === strrev($s);
来源：http://jn.wgjwhj.cn

JS:   s === [...s].reverse().join("")
来源：http://ts.huanxung.cn

TS:   s === [...s].reverse().join("")
来源：http://cw.9csxet.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://vf.asd995.cn

Go:   // 双指针从两端比较
来源：http://iz.hahajie.cn

Ruby: s == s.reverse
来源：http://jk.huixinmuqiang.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://mx.lnxyls.cn

[N07] 两数之和（返回下标）
来源：http://av.wgjwhj.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ka.lnxyls.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://rd.szxytkj.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://dv.lnxyls.cn

TS:   // 手写 Map<string, number>
来源：http://wo.chemitech.net.cn

Java: // 手写 HashMap
来源：http://do.nicolike.cn

Go:   // 手写 map[int]int
来源：http://es.szxytkj.cn

Ruby: // 手写 Hash
来源：http://fl.szxytkj.cn

C#:   // 手写 Dictionary<int, int>
来源：http://yk.gzmigu.cn

[N08] 生成全排列
来源：http://ax.asd995.cn

Py:   itertools.permutations(arr)
来源：http://mo.huanxung.cn

PHP:  // 手写递归交换
来源：http://wk.9csxet.cn

JS:   // 手写回溯递归
来源：http://bc.muxihuayi.cn

TS:   // 手写回溯递归
来源：http://hb.shxzskj.cn

Java: // 手写回溯递归
来源：http://af.asd995.cn

Go:   // 手写回溯递归
来源：http://hq.hnjuh.cn

Ruby: arr.permutation.to_a
来源：http://gp.lnxyls.cn

C#:   // 手写回溯递归
来源：http://za.asd995.cn

[N09] 栈与队列
来源：http://co.lnxyls.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://pi.9csxet.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://vq.haigaiapp.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wj.colortex.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://cv.nszjky.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ql.shxzskj.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://js.huixiangedu.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://vg.521024.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://pm.shxzukj.cn

[N10] 链表节点定义
来源：http://ro.lnxyls.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://eo.huixiangedu.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://nh.jianghongdianzi.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://bv.szsharing.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://yw.gzmigu.cn

Java: class Node { int v; Node next; }
来源：http://cc.shxzskj.cn

Go:   type Node struct { V int; Next *Node }
来源：http://bv.newstarts.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://cv.bjjhwx.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://hm.szxytkj.cn

[N11] 二叉树中序遍历
来源：http://em.yuntaijiaju.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ac.panjiajie.cn

PHP:  // 手写递归函数
来源：http://pl.lnxyls.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nx.yuexingan06.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://io.huanxung.cn

Java: // 手写递归
来源：http://bs.nszjky.cn

Go:   // 手写递归
来源：http://ij.huixiangedu.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ok.jctech888.com.cn

C#:   // 手写递归
来源：http://lf.bookmarksfly.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://lz.chemitech.net.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hv.yuntaijiaju.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://et.huixinmuqiang.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mb.yuexingan06.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ix.jctech888.com.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://sq.hnjuh.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hr.yuexingan06.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://nl.nicolike.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://yt.colortex.cn

================================================================================
来源：http://pm.colortex.cn

O. 并发与异步
来源：http://rf.nszjky.cn

================================================================================
来源：http://bs.huixinmuqiang.cn

[O01] 启动一个线程
来源：http://dc.521024.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://tw.nszjky.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://be.wgjwhj.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://tk.gzmigu.cn

TS:   // 同 JS
来源：http://yt.yuexingan06.cn

Java: new Thread(() -> f()).start()
来源：http://lr.szsharing.cn

Go:   go f()
来源：http://co.haigaiapp.cn

Ruby: Thread.new { f }
来源：http://qb.bookmarksfly.cn

C#:   Task.Run(() => F());
来源：http://io.hnjuh.cn

[O02] 使用线程池
来源：http://hh.nicolike.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://rw.jianghongdianzi.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hx.lnxyls.cn

JS:   // worker_threads 线程池
来源：http://ki.huixinmuqiang.cn

TS:   // worker_threads 线程池
来源：http://ms.hnjuh.cn

Java: Executors.newFixedThreadPool(4)
来源：http://eo.haigaiapp.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://fd.lnxyls.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://sp.shxzukj.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wt.shxzukj.cn

[O03] 加锁保护共享数据
来源：http://sf.haigaiapp.cn

Py:   with lock: shared += 1
来源：http://bp.jctech888.com.cn

PHP:  // 用 flock() 做文件锁
来源：http://bh.shxzskj.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://fi.shxzukj.cn

TS:   // 同 JS
来源：http://xc.wgjwhj.cn

Java: synchronized (this) { shared++; }
来源：http://dt.jianghongdianzi.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://dk.bjjhwx.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://qy.yuexingan06.cn

C#:   lock (gate) { shared++; }
来源：http://ft.nicolike.cn

[O04] 定义异步函数并等待
来源：http://ke.newstarts.cn

Py:   async def f():⏎    await g()
来源：http://pg.nszjky.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://jy.szsharing.cn

JS:   async function f() { await g(); }
来源：http://fk.chemitech.net.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://tf.yuexingan06.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://tw.huanxung.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ik.bookmarksfly.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ua.yuntaijiaju.cn

C#:   async Task F() { await G(); }
来源：http://us.huixinmuqiang.cn

[O05] 并发执行并等待全部完成
来源：http://ut.huanxung.cn

Py:   asyncio.gather(*tasks)
来源：http://ha.nszjky.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mb.huanxung.cn

JS:   await Promise.all(tasks)
来源：http://ls.hnjuh.cn

TS:   await Promise.all(tasks)
来源：http://ai.colortex.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://pv.hahajie.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ke.hahajie.cn

Ruby: threads.map(&:join)
来源：http://oe.huanxung.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://xc.muxihuayi.cn

[O06] 使用进程池
来源：http://or.chemitech.net.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://fd.panjiajie.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://gc.szxytkj.cn

JS:   // child_process / cluster 模块
来源：http://oa.haigaiapp.cn

TS:   // child_process / cluster 模块
来源：http://kb.newstarts.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://fy.asd995.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ov.yuexingan06.cn

Ruby: // fork 块
来源：http://jd.bjjhwx.cn

C#:   Parallel.For
来源：http://gm.wgjwhj.cn

================================================================================
来源：http://ar.bjjhwx.cn

P. 常用工具函数
来源：http://ow.bjjhwx.cn

================================================================================
来源：http://vr.9csxet.cn

[P01] 生成 UUID
来源：http://lc.shxzukj.cn

Py:   str(uuid.uuid4())
来源：http://gy.huixinmuqiang.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://sw.hahajie.cn

JS:   crypto.randomUUID()
来源：http://yn.muxihuayi.cn

TS:   crypto.randomUUID()
来源：http://wq.muxihuayi.cn

Java: UUID.randomUUID().toString()
来源：http://dj.huixiangedu.cn

Go:   // 用 github.com/google/uuid
来源：http://oh.wgjwhj.cn

Ruby: SecureRandom.uuid
来源：http://oj.huixiangedu.cn

C#:   Guid.NewGuid().ToString()
来源：http://iw.huixiangedu.cn

[P02] MD5 / SHA256 摘要
来源：http://rv.wgjwhj.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://te.nicolike.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://kd.muxihuayi.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://bs.shxzskj.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ls.chemitech.net.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://eo.yuexingan06.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wa.huixiangedu.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://gf.huixinmuqiang.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://pk.hahajie.cn

[P03] 生成短随机字符串
来源：http://wp.shxzskj.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://di.hahajie.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ci.lnxyls.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ad.hahajie.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kt.asd995.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ww.bjjhwx.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://qf.panjiajie.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://oh.yuexingan06.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://op.haigaiapp.cn

[P04] 求长度
来源：http://rr.jctech888.com.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ap.szxytkj.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://os.wgjwhj.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dm.newstarts.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yy.bookmarksfly.cn

Java: list.size();  map.size();  s.length()
来源：http://fz.bookmarksfly.cn

Go:   len(arr);  len(m)
来源：http://xk.shxzskj.cn

Ruby: x.length;  x.size
来源：http://yq.huanxung.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://lc.521024.cn

[P05] 判断两个对象内容是否相等
来源：http://ec.shxzukj.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://eg.jctech888.com.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://um.huixiangedu.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://la.szxytkj.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://xt.shtwfgs.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://rl.9csxet.cn

Go:   reflect.DeepEqual(a, b)
来源：http://un.chemitech.net.cn

Ruby: a == b
来源：http://ty.bookmarksfly.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://il.nszjky.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://sn.panjiajie.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://td.yuexingan06.cn

PHP:  if (empty($x)) {}
来源：http://mr.nszjky.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wm.colortex.cn

TS:   if (x == null) {}
来源：http://do.wgjwhj.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://vp.shxzukj.cn

Go:   if x == nil {}
来源：http://ow.huixinmuqiang.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wo.huanxung.cn

C#:   if (x is null) {}
来源：http://fk.huixinmuqiang.cn

[P07] 防抖与节流
来源：http://qf.szxytkj.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ms.yuntaijiaju.cn

PHP:  // 手写时间戳比较
来源：http://uv.szxytkj.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jz.jianghongdianzi.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xz.muxihuayi.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://au.huixiangedu.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wv.shxzskj.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://nm.haigaiapp.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ud.shxzskj.cn

[P08] 处理浮点精度问题
来源：http://er.bjjhwx.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://qk.hahajie.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://pu.newstarts.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://at.bjjhwx.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://kv.shxzukj.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://on.szsharing.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://vt.521024.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://vs.bookmarksfly.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://st.shtwfgs.cn

================================================================================
来源：http://qm.jctech888.com.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hq.bookmarksfly.cn

================================================================================
来源：http://un.newstarts.cn

[Q01] 创建表
来源：http://cy.nicolike.cn

CREATE TABLE users (
来源：http://sq.newstarts.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://xz.wgjwhj.cn

name VARCHAR(50) NOT NULL,
来源：http://bd.muxihuayi.cn

email VARCHAR(100) UNIQUE,
来源：http://rt.nszjky.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://xd.shxzukj.cn

);
来源：http://ay.chemitech.net.cn

[Q02] 创建带外键的表
来源：http://jq.521024.cn

CREATE TABLE orders (
来源：http://fh.jctech888.com.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mv.huixiangedu.cn

user_id INT NOT NULL,
来源：http://zg.yuntaijiaju.cn

amount DECIMAL(10, 2),
来源：http://xi.hnjuh.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://uv.szxytkj.cn

);
来源：http://uu.chemitech.net.cn

[Q03] 增加列
来源：http://ha.gzmigu.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ie.jianghongdianzi.cn

[Q04] 修改列类型
来源：http://as.nszjky.cn


<!-- 参考信息 -->