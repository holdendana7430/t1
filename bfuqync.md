代发 wailian999

Ruby: exit 1
来源：http://mq.hahajie.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://sk.yuntaijiaju.cn

[M06] 向标准错误输出
来源：http://sf.shxzukj.cn

Py:   print("err", file=sys.stderr)
来源：http://ot.shtwfgs.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://rn.huixinmuqiang.cn

JS:   console.error("err")
来源：http://nh.huixiangedu.cn

TS:   console.error("err")
来源：http://vd.yuexingan06.cn

Java: System.err.println("err")
来源：http://di.chemitech.net.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://qc.bjjhwx.cn

Ruby: warn "err"
来源：http://xc.bookmarksfly.cn

C#:   Console.Error.WriteLine("err")
来源：http://ts.nszjky.cn

[M07] 判断是否为主入口
来源：http://zz.colortex.cn

Py:   if __name__ == "__main__":
来源：http://zc.shtwfgs.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://sa.yuexingan06.cn

JS:   require.main === module
来源：http://ob.wgjwhj.cn

TS:   require.main === module
来源：http://sj.521024.cn

Java: public static void main(String[] args)
来源：http://ff.huanxung.cn

Go:   func main()
来源：http://rd.521024.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://pm.hahajie.cn

C#:   static void Main(string[] args)
来源：http://wq.huixinmuqiang.cn

[M08] 获取系统与运行时信息
来源：http://dg.panjiajie.cn

Py:   platform.system();  platform.python_version()
来源：http://rx.bjjhwx.cn

PHP:  PHP_OS;  phpversion();
来源：http://xt.wgjwhj.cn

JS:   process.platform;  process.version
来源：http://al.gzmigu.cn

TS:   process.platform;  process.version
来源：http://uc.panjiajie.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://bs.wgjwhj.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://er.muxihuayi.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://vh.newstarts.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://th.colortex.cn

================================================================================
来源：http://xr.shxzskj.cn

N. 数据结构与算法
来源：http://by.bookmarksfly.cn

================================================================================
来源：http://nm.muxihuayi.cn

[N01] 二分查找（有序数组）
来源：http://aa.jianghongdianzi.cn

Py:   bisect.bisect_left(arr, x)
来源：http://na.huixinmuqiang.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ki.nicolike.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ij.panjiajie.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ui.muxihuayi.cn

Java: Arrays.binarySearch(arr, x)
来源：http://pm.colortex.cn

Go:   sort.SearchInts(arr, x)
来源：http://fi.wgjwhj.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://id.wgjwhj.cn

C#:   Array.BinarySearch(arr, x)
来源：http://zg.hahajie.cn

[N02] 排序（工程实践用内置实现）
来源：http://dz.nszjky.cn

Py:   sorted(arr);  arr.sort()
来源：http://ey.chemitech.net.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://kh.hahajie.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://mw.haigaiapp.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://mr.szxytkj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://sh.jctech888.com.cn

Go:   slices.Sort(arr)
来源：http://ch.nszjky.cn

Ruby: arr.sort
来源：http://xe.szsharing.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ak.jctech888.com.cn

[N03] 快速排序（分治示例）
来源：http://cx.bookmarksfly.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://nn.9csxet.cn

PHP:  // 递归实现，或用 usort
来源：http://jf.jianghongdianzi.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://or.shxzskj.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ut.szsharing.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wx.gzmigu.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://qk.panjiajie.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wv.chemitech.net.cn

C#:   // 手写递归，或 Array.Sort
来源：http://pl.asd995.cn

[N04] 斐波那契数列
来源：http://rk.huixiangedu.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ds.521024.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://xi.bjjhwx.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://co.shxzukj.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yl.panjiajie.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://th.haigaiapp.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://te.lnxyls.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://gm.huixiangedu.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://cd.huanxung.cn

[N05] 最大公约数
来源：http://oh.shxzskj.cn

Py:   math.gcd(a, b)
来源：http://it.szsharing.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ab.bjjhwx.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://du.szxytkj.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xx.shxzukj.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://cl.yuntaijiaju.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ax.hnjuh.cn

Ruby: a.gcd(b)
来源：http://jj.hahajie.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://nm.bjjhwx.cn

[N06] 判断回文字符串
来源：http://vn.521024.cn

Py:   s == s[::-1]
来源：http://dn.yuntaijiaju.cn

PHP:  $s === strrev($s);
来源：http://vh.asd995.cn

JS:   s === [...s].reverse().join("")
来源：http://kk.shxzukj.cn

TS:   s === [...s].reverse().join("")
来源：http://op.lnxyls.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://qg.lnxyls.cn

Go:   // 双指针从两端比较
来源：http://jb.asd995.cn

Ruby: s == s.reverse
来源：http://rj.bookmarksfly.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ik.bjjhwx.cn

[N07] 两数之和（返回下标）
来源：http://dv.wgjwhj.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ua.huixinmuqiang.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://tv.shtwfgs.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ul.shtwfgs.cn

TS:   // 手写 Map<string, number>
来源：http://hr.yuntaijiaju.cn

Java: // 手写 HashMap
来源：http://jm.hnjuh.cn

Go:   // 手写 map[int]int
来源：http://ok.bookmarksfly.cn

Ruby: // 手写 Hash
来源：http://fj.hahajie.cn

C#:   // 手写 Dictionary<int, int>
来源：http://gy.szxytkj.cn

[N08] 生成全排列
来源：http://fz.jianghongdianzi.cn

Py:   itertools.permutations(arr)
来源：http://yo.jianghongdianzi.cn

PHP:  // 手写递归交换
来源：http://db.gzmigu.cn

JS:   // 手写回溯递归
来源：http://mm.hahajie.cn

TS:   // 手写回溯递归
来源：http://rt.jianghongdianzi.cn

Java: // 手写回溯递归
来源：http://rc.huanxung.cn

Go:   // 手写回溯递归
来源：http://ej.huixinmuqiang.cn

Ruby: arr.permutation.to_a
来源：http://gk.shxzskj.cn

C#:   // 手写回溯递归
来源：http://qm.asd995.cn

[N09] 栈与队列
来源：http://ss.nszjky.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://vc.hnjuh.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://gb.bjjhwx.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://il.nszjky.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://nd.521024.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://nb.nicolike.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://dw.newstarts.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://la.szsharing.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://jl.yuexingan06.cn

[N10] 链表节点定义
来源：http://if.shtwfgs.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://da.huixinmuqiang.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://en.hnjuh.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://gn.hahajie.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://gl.hahajie.cn

Java: class Node { int v; Node next; }
来源：http://kq.szsharing.cn

Go:   type Node struct { V int; Next *Node }
来源：http://bl.yuexingan06.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://jl.jctech888.com.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://aw.bjjhwx.cn

[N11] 二叉树中序遍历
来源：http://bx.9csxet.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ge.szxytkj.cn

PHP:  // 手写递归函数
来源：http://et.bookmarksfly.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rq.gzmigu.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rt.nicolike.cn

Java: // 手写递归
来源：http://em.chemitech.net.cn

Go:   // 手写递归
来源：http://sx.szxytkj.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://cn.nszjky.cn

C#:   // 手写递归
来源：http://sm.szxytkj.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://nn.shxzukj.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://qa.chemitech.net.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://dy.9csxet.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sq.yuntaijiaju.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xm.huixinmuqiang.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ux.9csxet.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ul.shxzskj.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://qp.huixiangedu.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://bh.szsharing.cn

================================================================================
来源：http://gr.muxihuayi.cn

O. 并发与异步
来源：http://gj.shxzskj.cn

================================================================================
来源：http://ye.521024.cn

[O01] 启动一个线程
来源：http://jq.bookmarksfly.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://kd.521024.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ob.nszjky.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ht.asd995.cn

TS:   // 同 JS
来源：http://ti.shtwfgs.cn

Java: new Thread(() -> f()).start()
来源：http://ng.9csxet.cn

Go:   go f()
来源：http://jv.shxzskj.cn

Ruby: Thread.new { f }
来源：http://so.szsharing.cn

C#:   Task.Run(() => F());
来源：http://aq.lnxyls.cn

[O02] 使用线程池
来源：http://mj.huixiangedu.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://nf.jianghongdianzi.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://zj.nszjky.cn

JS:   // worker_threads 线程池
来源：http://pf.huixinmuqiang.cn

TS:   // worker_threads 线程池
来源：http://wz.jianghongdianzi.cn

Java: Executors.newFixedThreadPool(4)
来源：http://wd.haigaiapp.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wc.gzmigu.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://xj.muxihuayi.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ao.jianghongdianzi.cn

[O03] 加锁保护共享数据
来源：http://ho.wgjwhj.cn

Py:   with lock: shared += 1
来源：http://on.nicolike.cn

PHP:  // 用 flock() 做文件锁
来源：http://kr.shtwfgs.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ht.gzmigu.cn

TS:   // 同 JS
来源：http://zj.newstarts.cn

Java: synchronized (this) { shared++; }
来源：http://oo.nicolike.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://fw.shxzukj.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://tt.bjjhwx.cn

C#:   lock (gate) { shared++; }
来源：http://do.shxzukj.cn

[O04] 定义异步函数并等待
来源：http://wz.szxytkj.cn

Py:   async def f():⏎    await g()
来源：http://yf.chemitech.net.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://tw.huixinmuqiang.cn

JS:   async function f() { await g(); }
来源：http://sz.gzmigu.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://iy.hnjuh.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://xy.huanxung.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ud.521024.cn

Ruby: # 用 Fiber 或 async gem
来源：http://al.muxihuayi.cn

C#:   async Task F() { await G(); }
来源：http://cs.huixinmuqiang.cn

[O05] 并发执行并等待全部完成
来源：http://ma.9csxet.cn

Py:   asyncio.gather(*tasks)
来源：http://qn.nicolike.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://xm.yuexingan06.cn

JS:   await Promise.all(tasks)
来源：http://iy.szsharing.cn

TS:   await Promise.all(tasks)
来源：http://xq.bjjhwx.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://pp.muxihuayi.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://we.szsharing.cn

Ruby: threads.map(&:join)
来源：http://ld.hnjuh.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://st.bjjhwx.cn

[O06] 使用进程池
来源：http://kd.lnxyls.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://gu.yuexingan06.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://xh.gzmigu.cn

JS:   // child_process / cluster 模块
来源：http://up.shxzukj.cn

TS:   // child_process / cluster 模块
来源：http://yp.huanxung.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wy.jianghongdianzi.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://dp.shxzskj.cn

Ruby: // fork 块
来源：http://mv.wgjwhj.cn

C#:   Parallel.For
来源：http://lf.hahajie.cn

================================================================================
来源：http://la.521024.cn

P. 常用工具函数
来源：http://ok.521024.cn

================================================================================
来源：http://bz.hahajie.cn

[P01] 生成 UUID
来源：http://pm.nicolike.cn

Py:   str(uuid.uuid4())
来源：http://wd.chemitech.net.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://pp.yuexingan06.cn

JS:   crypto.randomUUID()
来源：http://ic.9csxet.cn

TS:   crypto.randomUUID()
来源：http://dz.gzmigu.cn

Java: UUID.randomUUID().toString()
来源：http://fk.521024.cn

Go:   // 用 github.com/google/uuid
来源：http://wc.colortex.cn

Ruby: SecureRandom.uuid
来源：http://au.szxytkj.cn

C#:   Guid.NewGuid().ToString()
来源：http://th.shxzukj.cn

[P02] MD5 / SHA256 摘要
来源：http://nk.9csxet.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://fk.yuntaijiaju.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://rw.chemitech.net.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://gs.shxzukj.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://xs.hnjuh.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://qt.gzmigu.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://us.gzmigu.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://fq.yuexingan06.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://uq.newstarts.cn

[P03] 生成短随机字符串
来源：http://wo.jctech888.com.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.gzmigu.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://tq.huanxung.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ve.shtwfgs.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wt.yuexingan06.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://yz.lnxyls.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ju.colortex.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://yj.9csxet.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ak.lnxyls.cn

[P04] 求长度
来源：http://qk.szsharing.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://uw.gzmigu.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bs.jctech888.com.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cz.haigaiapp.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nx.9csxet.cn

Java: list.size();  map.size();  s.length()
来源：http://mh.hnjuh.cn

Go:   len(arr);  len(m)
来源：http://kw.9csxet.cn

Ruby: x.length;  x.size
来源：http://uu.jctech888.com.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://xo.nicolike.cn

[P05] 判断两个对象内容是否相等
来源：http://wx.panjiajie.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://be.nicolike.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://yh.wgjwhj.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://la.panjiajie.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://fp.huixiangedu.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ec.shtwfgs.cn

Go:   reflect.DeepEqual(a, b)
来源：http://yu.bjjhwx.cn

Ruby: a == b
来源：http://ca.hnjuh.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://iq.hnjuh.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mc.9csxet.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://zc.lnxyls.cn

PHP:  if (empty($x)) {}
来源：http://rq.huanxung.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://nz.szxytkj.cn

TS:   if (x == null) {}
来源：http://ps.newstarts.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://hw.newstarts.cn

Go:   if x == nil {}
来源：http://kj.asd995.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://it.gzmigu.cn

C#:   if (x is null) {}
来源：http://cv.szxytkj.cn

[P07] 防抖与节流
来源：http://hf.nicolike.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://xq.haigaiapp.cn

PHP:  // 手写时间戳比较
来源：http://du.yuntaijiaju.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vd.shtwfgs.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jp.huixinmuqiang.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ny.huanxung.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ys.asd995.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://gr.shxzukj.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://pj.colortex.cn

[P08] 处理浮点精度问题
来源：http://nn.jianghongdianzi.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://zx.szxytkj.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ur.shtwfgs.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://kq.newstarts.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://op.521024.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://tq.colortex.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hr.521024.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ru.yuexingan06.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ta.haigaiapp.cn

================================================================================
来源：http://rv.huanxung.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ou.521024.cn

================================================================================
来源：http://rd.shxzskj.cn

[Q01] 创建表
来源：http://rg.newstarts.cn

CREATE TABLE users (
来源：http://fm.bookmarksfly.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://nv.colortex.cn

name VARCHAR(50) NOT NULL,
来源：http://wb.wgjwhj.cn

email VARCHAR(100) UNIQUE,
来源：http://bm.gzmigu.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://lx.asd995.cn

);
来源：http://ef.haigaiapp.cn

[Q02] 创建带外键的表
来源：http://tl.szxytkj.cn

CREATE TABLE orders (
来源：http://ii.shxzskj.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://gk.yuntaijiaju.cn

user_id INT NOT NULL,
来源：http://fs.shtwfgs.cn

amount DECIMAL(10, 2),
来源：http://hs.haigaiapp.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://dg.bookmarksfly.cn

);
来源：http://vq.shxzukj.cn

[Q03] 增加列
来源：http://kr.muxihuayi.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://sq.bjjhwx.cn

[Q04] 修改列类型
来源：http://uq.huixiangedu.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://fm.bjjhwx.cn

[Q05] 重命名列
来源：http://jf.chemitech.net.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://zn.huixiangedu.cn

[Q06] 删除列
来源：http://ku.jianghongdianzi.cn

ALTER TABLE users DROP COLUMN age;
来源：http://az.hnjuh.cn

[Q07] 删除表
来源：http://hy.szsharing.cn

DROP TABLE IF EXISTS orders;
来源：http://sq.haigaiapp.cn

[Q08] 创建普通索引
来源：http://zm.shxzukj.cn


<!-- 参考信息 -->