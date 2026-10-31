代发 wailian999

C#:   Directory.GetCurrentDirectory()
来源：http://tn.lnxyls.cn

[M05] 设置退出码
来源：http://og.bjjhwx.cn

Py:   sys.exit(1)
来源：http://ce.shxzskj.cn

PHP:  exit(1);
来源：http://rj.panjiajie.cn

JS:   process.exit(1)
来源：http://rq.panjiajie.cn

TS:   process.exit(1)
来源：http://em.shxzukj.cn

Java: System.exit(1)
来源：http://ri.yuntaijiaju.cn

Go:   os.Exit(1)
来源：http://ga.nszjky.cn

Ruby: exit 1
来源：http://ul.shxzukj.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://rn.lnxyls.cn

[M06] 向标准错误输出
来源：http://bj.szxytkj.cn

Py:   print("err", file=sys.stderr)
来源：http://jk.panjiajie.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://zq.lnxyls.cn

JS:   console.error("err")
来源：http://bu.chemitech.net.cn

TS:   console.error("err")
来源：http://ck.shtwfgs.cn

Java: System.err.println("err")
来源：http://bl.szxytkj.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ar.shxzukj.cn

Ruby: warn "err"
来源：http://bw.nszjky.cn

C#:   Console.Error.WriteLine("err")
来源：http://ie.gzmigu.cn

[M07] 判断是否为主入口
来源：http://co.521024.cn

Py:   if __name__ == "__main__":
来源：http://lf.newstarts.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://rc.haigaiapp.cn

JS:   require.main === module
来源：http://sr.9csxet.cn

TS:   require.main === module
来源：http://eo.shxzskj.cn

Java: public static void main(String[] args)
来源：http://ht.shxzskj.cn

Go:   func main()
来源：http://ap.lnxyls.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://cv.shxzukj.cn

C#:   static void Main(string[] args)
来源：http://zc.lnxyls.cn

[M08] 获取系统与运行时信息
来源：http://ds.nicolike.cn

Py:   platform.system();  platform.python_version()
来源：http://ww.szsharing.cn

PHP:  PHP_OS;  phpversion();
来源：http://fi.gzmigu.cn

JS:   process.platform;  process.version
来源：http://id.9csxet.cn

TS:   process.platform;  process.version
来源：http://yh.hnjuh.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://cn.huanxung.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ji.jianghongdianzi.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://fz.yuntaijiaju.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://cd.shxzukj.cn

================================================================================
来源：http://mr.wgjwhj.cn

N. 数据结构与算法
来源：http://xt.gzmigu.cn

================================================================================
来源：http://nu.jianghongdianzi.cn

[N01] 二分查找（有序数组）
来源：http://qt.chemitech.net.cn

Py:   bisect.bisect_left(arr, x)
来源：http://wp.muxihuayi.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://qe.asd995.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yp.szsharing.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ei.huixinmuqiang.cn

Java: Arrays.binarySearch(arr, x)
来源：http://mx.lnxyls.cn

Go:   sort.SearchInts(arr, x)
来源：http://ns.jianghongdianzi.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://kt.bookmarksfly.cn

C#:   Array.BinarySearch(arr, x)
来源：http://vi.panjiajie.cn

[N02] 排序（工程实践用内置实现）
来源：http://ht.colortex.cn

Py:   sorted(arr);  arr.sort()
来源：http://en.szsharing.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hk.yuexingan06.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ls.haigaiapp.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://dh.gzmigu.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://if.nicolike.cn

Go:   slices.Sort(arr)
来源：http://qm.hahajie.cn

Ruby: arr.sort
来源：http://qt.hahajie.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://jm.bookmarksfly.cn

[N03] 快速排序（分治示例）
来源：http://sb.chemitech.net.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ak.shtwfgs.cn

PHP:  // 递归实现，或用 usort
来源：http://zq.lnxyls.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ss.haigaiapp.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nk.shtwfgs.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://cq.newstarts.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://tz.lnxyls.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://iz.bjjhwx.cn

C#:   // 手写递归，或 Array.Sort
来源：http://pn.shxzukj.cn

[N04] 斐波那契数列
来源：http://ge.bjjhwx.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qo.shtwfgs.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://pl.szsharing.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rq.lnxyls.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://iy.hnjuh.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://be.hnjuh.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mx.huanxung.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ag.hahajie.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://tg.521024.cn

[N05] 最大公约数
来源：http://gh.huixinmuqiang.cn

Py:   math.gcd(a, b)
来源：http://fb.9csxet.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.gzmigu.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xj.hnjuh.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gq.yuntaijiaju.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ls.jctech888.com.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://us.yuexingan06.cn

Ruby: a.gcd(b)
来源：http://wi.wgjwhj.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://er.muxihuayi.cn

[N06] 判断回文字符串
来源：http://un.huixiangedu.cn

Py:   s == s[::-1]
来源：http://xl.szxytkj.cn

PHP:  $s === strrev($s);
来源：http://yz.hahajie.cn

JS:   s === [...s].reverse().join("")
来源：http://uy.yuexingan06.cn

TS:   s === [...s].reverse().join("")
来源：http://jy.shtwfgs.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://tx.9csxet.cn

Go:   // 双指针从两端比较
来源：http://rp.nszjky.cn

Ruby: s == s.reverse
来源：http://uc.bjjhwx.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ez.nicolike.cn

[N07] 两数之和（返回下标）
来源：http://ld.chemitech.net.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://tj.9csxet.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://os.9csxet.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ay.gzmigu.cn

TS:   // 手写 Map<string, number>
来源：http://th.shtwfgs.cn

Java: // 手写 HashMap
来源：http://fl.chemitech.net.cn

Go:   // 手写 map[int]int
来源：http://nx.nszjky.cn

Ruby: // 手写 Hash
来源：http://sf.newstarts.cn

C#:   // 手写 Dictionary<int, int>
来源：http://rn.nszjky.cn

[N08] 生成全排列
来源：http://ob.szxytkj.cn

Py:   itertools.permutations(arr)
来源：http://vt.colortex.cn

PHP:  // 手写递归交换
来源：http://km.yuntaijiaju.cn

JS:   // 手写回溯递归
来源：http://hv.bjjhwx.cn

TS:   // 手写回溯递归
来源：http://np.asd995.cn

Java: // 手写回溯递归
来源：http://be.huixiangedu.cn

Go:   // 手写回溯递归
来源：http://fw.panjiajie.cn

Ruby: arr.permutation.to_a
来源：http://lx.colortex.cn

C#:   // 手写回溯递归
来源：http://eb.hnjuh.cn

[N09] 栈与队列
来源：http://si.colortex.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://lh.szxytkj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ax.nszjky.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://lv.nicolike.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://rr.hnjuh.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://tv.huixiangedu.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ua.huixiangedu.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://oy.haigaiapp.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://dv.hnjuh.cn

[N10] 链表节点定义
来源：http://zz.huanxung.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://kw.szsharing.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://zc.hahajie.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qo.hnjuh.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://dp.asd995.cn

Java: class Node { int v; Node next; }
来源：http://so.9csxet.cn

Go:   type Node struct { V int; Next *Node }
来源：http://an.jctech888.com.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://yu.muxihuayi.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://zf.newstarts.cn

[N11] 二叉树中序遍历
来源：http://oi.jianghongdianzi.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://cn.huanxung.cn

PHP:  // 手写递归函数
来源：http://pc.yuntaijiaju.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zv.lnxyls.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rw.szxytkj.cn

Java: // 手写递归
来源：http://hb.szsharing.cn

Go:   // 手写递归
来源：http://yg.hahajie.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://uj.gzmigu.cn

C#:   // 手写递归
来源：http://sl.521024.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ku.szsharing.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://dj.shxzukj.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://du.shtwfgs.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jz.hnjuh.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://it.jianghongdianzi.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://gy.jctech888.com.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ij.bookmarksfly.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://sl.szxytkj.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ry.nszjky.cn

================================================================================
来源：http://fh.newstarts.cn

O. 并发与异步
来源：http://je.yuntaijiaju.cn

================================================================================
来源：http://uq.huixiangedu.cn

[O01] 启动一个线程
来源：http://nj.gzmigu.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ap.hnjuh.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://us.yuexingan06.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://fz.colortex.cn

TS:   // 同 JS
来源：http://tj.szsharing.cn

Java: new Thread(() -> f()).start()
来源：http://gn.wgjwhj.cn

Go:   go f()
来源：http://ox.shtwfgs.cn

Ruby: Thread.new { f }
来源：http://kl.hnjuh.cn

C#:   Task.Run(() => F());
来源：http://ey.9csxet.cn

[O02] 使用线程池
来源：http://vn.bjjhwx.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mg.nszjky.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://fi.hahajie.cn

JS:   // worker_threads 线程池
来源：http://uq.muxihuayi.cn

TS:   // worker_threads 线程池
来源：http://vd.jianghongdianzi.cn

Java: Executors.newFixedThreadPool(4)
来源：http://mr.shxzukj.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hc.newstarts.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wy.yuntaijiaju.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://dp.huixinmuqiang.cn

[O03] 加锁保护共享数据
来源：http://dq.szsharing.cn

Py:   with lock: shared += 1
来源：http://kr.wgjwhj.cn

PHP:  // 用 flock() 做文件锁
来源：http://nk.yuexingan06.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://km.bjjhwx.cn

TS:   // 同 JS
来源：http://gt.hahajie.cn

Java: synchronized (this) { shared++; }
来源：http://bw.jianghongdianzi.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://je.shxzukj.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://xz.huanxung.cn

C#:   lock (gate) { shared++; }
来源：http://dg.muxihuayi.cn

[O04] 定义异步函数并等待
来源：http://ro.szxytkj.cn

Py:   async def f():⏎    await g()
来源：http://lm.huixinmuqiang.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ce.jctech888.com.cn

JS:   async function f() { await g(); }
来源：http://cb.shxzukj.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://mv.panjiajie.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ox.wgjwhj.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://lt.wgjwhj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://tk.asd995.cn

C#:   async Task F() { await G(); }
来源：http://rr.shtwfgs.cn

[O05] 并发执行并等待全部完成
来源：http://ew.szxytkj.cn

Py:   asyncio.gather(*tasks)
来源：http://tk.shtwfgs.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://fa.jctech888.com.cn

JS:   await Promise.all(tasks)
来源：http://nn.shtwfgs.cn

TS:   await Promise.all(tasks)
来源：http://vo.haigaiapp.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://cq.hahajie.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://yp.huixiangedu.cn

Ruby: threads.map(&:join)
来源：http://yx.lnxyls.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://hm.521024.cn

[O06] 使用进程池
来源：http://be.jctech888.com.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://de.nicolike.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://sg.newstarts.cn

JS:   // child_process / cluster 模块
来源：http://tp.huanxung.cn

TS:   // child_process / cluster 模块
来源：http://zh.huixiangedu.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ko.9csxet.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wv.lnxyls.cn

Ruby: // fork 块
来源：http://py.lnxyls.cn

C#:   Parallel.For
来源：http://px.huixiangedu.cn

================================================================================
来源：http://hs.huixinmuqiang.cn

P. 常用工具函数
来源：http://xw.nicolike.cn

================================================================================
来源：http://mm.asd995.cn

[P01] 生成 UUID
来源：http://bn.wgjwhj.cn

Py:   str(uuid.uuid4())
来源：http://wx.gzmigu.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://re.huixiangedu.cn

JS:   crypto.randomUUID()
来源：http://kv.jianghongdianzi.cn

TS:   crypto.randomUUID()
来源：http://gv.szxytkj.cn

Java: UUID.randomUUID().toString()
来源：http://kw.huixinmuqiang.cn

Go:   // 用 github.com/google/uuid
来源：http://bd.haigaiapp.cn

Ruby: SecureRandom.uuid
来源：http://jy.gzmigu.cn

C#:   Guid.NewGuid().ToString()
来源：http://ps.shxzukj.cn

[P02] MD5 / SHA256 摘要
来源：http://kk.yuexingan06.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ww.szxytkj.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ii.panjiajie.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ze.panjiajie.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://uo.asd995.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://cl.yuexingan06.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://sv.jctech888.com.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://if.szxytkj.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ur.szxytkj.cn

[P03] 生成短随机字符串
来源：http://yp.jctech888.com.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://tg.wgjwhj.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://oi.hnjuh.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lz.asd995.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://oq.shtwfgs.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://kv.521024.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://xm.jctech888.com.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://bw.9csxet.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ux.newstarts.cn

[P04] 求长度
来源：http://gf.muxihuayi.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://pb.bjjhwx.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://oi.wgjwhj.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rx.haigaiapp.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qj.haigaiapp.cn

Java: list.size();  map.size();  s.length()
来源：http://tt.yuexingan06.cn

Go:   len(arr);  len(m)
来源：http://rd.huanxung.cn

Ruby: x.length;  x.size
来源：http://ec.shtwfgs.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://np.muxihuayi.cn

[P05] 判断两个对象内容是否相等
来源：http://xo.szxytkj.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://rv.521024.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://xd.newstarts.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://fr.bjjhwx.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ty.hnjuh.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mb.nszjky.cn

Go:   reflect.DeepEqual(a, b)
来源：http://gj.jctech888.com.cn

Ruby: a == b
来源：http://ib.colortex.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://gl.panjiajie.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://gd.newstarts.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ef.colortex.cn

PHP:  if (empty($x)) {}
来源：http://ab.bookmarksfly.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://id.nszjky.cn

TS:   if (x == null) {}
来源：http://ux.bookmarksfly.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://or.huixiangedu.cn

Go:   if x == nil {}
来源：http://ph.shxzskj.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://oy.nicolike.cn

C#:   if (x is null) {}
来源：http://jd.jianghongdianzi.cn

[P07] 防抖与节流
来源：http://fa.shxzskj.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://nb.huixiangedu.cn

PHP:  // 手写时间戳比较
来源：http://kp.nszjky.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uq.jianghongdianzi.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nj.shxzskj.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ec.shxzukj.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://dv.huixinmuqiang.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://sf.9csxet.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mf.szxytkj.cn

[P08] 处理浮点精度问题
来源：http://jo.huanxung.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://tu.muxihuayi.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://uq.bookmarksfly.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://gp.haigaiapp.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://zl.panjiajie.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://pr.haigaiapp.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://lj.colortex.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://qb.shxzskj.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ws.shxzskj.cn

================================================================================
来源：http://dw.colortex.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://kn.szxytkj.cn

================================================================================
来源：http://ci.newstarts.cn

[Q01] 创建表
来源：http://tv.colortex.cn

CREATE TABLE users (
来源：http://hp.yuntaijiaju.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://xb.colortex.cn

name VARCHAR(50) NOT NULL,
来源：http://hp.asd995.cn

email VARCHAR(100) UNIQUE,
来源：http://mw.jctech888.com.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://dd.hahajie.cn

);
来源：http://il.gzmigu.cn

[Q02] 创建带外键的表
来源：http://kp.shxzskj.cn

CREATE TABLE orders (
来源：http://ax.muxihuayi.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://og.shxzskj.cn

user_id INT NOT NULL,
来源：http://qj.lnxyls.cn

amount DECIMAL(10, 2),
来源：http://ot.shxzukj.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://cx.jianghongdianzi.cn

);
来源：http://wg.asd995.cn

[Q03] 增加列
来源：http://ag.szxytkj.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://of.521024.cn

[Q04] 修改列类型
来源：http://ez.yuntaijiaju.cn


<!-- 参考信息 -->