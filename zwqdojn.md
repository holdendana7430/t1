代发 wailian999

Ruby: exit 1
来源：http://dn.szsharing.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://pu.wgjwhj.cn

[M06] 向标准错误输出
来源：http://xf.chemitech.net.cn

Py:   print("err", file=sys.stderr)
来源：http://wq.bookmarksfly.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://jb.panjiajie.cn

JS:   console.error("err")
来源：http://tj.shxzskj.cn

TS:   console.error("err")
来源：http://kj.hnjuh.cn

Java: System.err.println("err")
来源：http://kj.huixinmuqiang.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ha.newstarts.cn

Ruby: warn "err"
来源：http://qy.huanxung.cn

C#:   Console.Error.WriteLine("err")
来源：http://bi.muxihuayi.cn

[M07] 判断是否为主入口
来源：http://ph.yuntaijiaju.cn

Py:   if __name__ == "__main__":
来源：http://gl.szsharing.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://vg.haigaiapp.cn

JS:   require.main === module
来源：http://vq.panjiajie.cn

TS:   require.main === module
来源：http://ec.bjjhwx.cn

Java: public static void main(String[] args)
来源：http://fu.shxzskj.cn

Go:   func main()
来源：http://rb.szsharing.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://kx.panjiajie.cn

C#:   static void Main(string[] args)
来源：http://lb.huixinmuqiang.cn

[M08] 获取系统与运行时信息
来源：http://sw.521024.cn

Py:   platform.system();  platform.python_version()
来源：http://gv.jianghongdianzi.cn

PHP:  PHP_OS;  phpversion();
来源：http://ja.newstarts.cn

JS:   process.platform;  process.version
来源：http://xw.nicolike.cn

TS:   process.platform;  process.version
来源：http://jn.hnjuh.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://cq.521024.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://sr.bookmarksfly.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ib.yuexingan06.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://yq.huanxung.cn

================================================================================
来源：http://ab.yuexingan06.cn

N. 数据结构与算法
来源：http://wt.haigaiapp.cn

================================================================================
来源：http://gk.panjiajie.cn

[N01] 二分查找（有序数组）
来源：http://yl.nszjky.cn

Py:   bisect.bisect_left(arr, x)
来源：http://rx.gzmigu.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://pc.wgjwhj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ym.shtwfgs.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ln.nszjky.cn

Java: Arrays.binarySearch(arr, x)
来源：http://xx.huixiangedu.cn

Go:   sort.SearchInts(arr, x)
来源：http://lr.shtwfgs.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://xg.lnxyls.cn

C#:   Array.BinarySearch(arr, x)
来源：http://pc.jctech888.com.cn

[N02] 排序（工程实践用内置实现）
来源：http://ji.huixinmuqiang.cn

Py:   sorted(arr);  arr.sort()
来源：http://vq.yuexingan06.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://br.9csxet.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://qd.huanxung.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://dy.shxzskj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ap.wgjwhj.cn

Go:   slices.Sort(arr)
来源：http://lz.gzmigu.cn

Ruby: arr.sort
来源：http://xh.shxzukj.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://un.yuexingan06.cn

[N03] 快速排序（分治示例）
来源：http://vm.huanxung.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ux.shxzukj.cn

PHP:  // 递归实现，或用 usort
来源：http://fu.yuntaijiaju.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uf.yuntaijiaju.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rk.shtwfgs.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://sl.9csxet.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://zb.muxihuayi.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ll.huixiangedu.cn

C#:   // 手写递归，或 Array.Sort
来源：http://dl.haigaiapp.cn

[N04] 斐波那契数列
来源：http://gi.bookmarksfly.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ty.szxytkj.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://gx.hahajie.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pg.colortex.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pi.lnxyls.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://db.huixiangedu.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://gb.haigaiapp.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ou.jianghongdianzi.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://jc.lnxyls.cn

[N05] 最大公约数
来源：http://jv.chemitech.net.cn

Py:   math.gcd(a, b)
来源：http://dy.yuntaijiaju.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://qo.nicolike.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jd.newstarts.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wz.newstarts.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mo.jctech888.com.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wt.jianghongdianzi.cn

Ruby: a.gcd(b)
来源：http://ss.shxzskj.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://eq.colortex.cn

[N06] 判断回文字符串
来源：http://sv.wgjwhj.cn

Py:   s == s[::-1]
来源：http://bs.hnjuh.cn

PHP:  $s === strrev($s);
来源：http://zj.huixinmuqiang.cn

JS:   s === [...s].reverse().join("")
来源：http://nt.lnxyls.cn

TS:   s === [...s].reverse().join("")
来源：http://nj.hnjuh.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://se.huixiangedu.cn

Go:   // 双指针从两端比较
来源：http://yt.asd995.cn

Ruby: s == s.reverse
来源：http://gf.haigaiapp.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://vn.yuntaijiaju.cn

[N07] 两数之和（返回下标）
来源：http://uq.hnjuh.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://sc.colortex.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://rb.yuexingan06.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://dm.gzmigu.cn

TS:   // 手写 Map<string, number>
来源：http://jc.wgjwhj.cn

Java: // 手写 HashMap
来源：http://jn.shxzukj.cn

Go:   // 手写 map[int]int
来源：http://wk.panjiajie.cn

Ruby: // 手写 Hash
来源：http://qe.hnjuh.cn

C#:   // 手写 Dictionary<int, int>
来源：http://tu.lnxyls.cn

[N08] 生成全排列
来源：http://tm.yuntaijiaju.cn

Py:   itertools.permutations(arr)
来源：http://in.lnxyls.cn

PHP:  // 手写递归交换
来源：http://uj.nszjky.cn

JS:   // 手写回溯递归
来源：http://ol.szsharing.cn

TS:   // 手写回溯递归
来源：http://wy.shxzskj.cn

Java: // 手写回溯递归
来源：http://zm.jianghongdianzi.cn

Go:   // 手写回溯递归
来源：http://re.huixinmuqiang.cn

Ruby: arr.permutation.to_a
来源：http://ep.wgjwhj.cn

C#:   // 手写回溯递归
来源：http://xb.bookmarksfly.cn

[N09] 栈与队列
来源：http://av.newstarts.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://om.chemitech.net.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hk.yuexingan06.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://am.nszjky.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://xq.newstarts.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ap.asd995.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://vn.huixiangedu.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://is.yuexingan06.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://dp.jianghongdianzi.cn

[N10] 链表节点定义
来源：http://qg.szsharing.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://xj.haigaiapp.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://mk.newstarts.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://jp.shxzukj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ek.newstarts.cn

Java: class Node { int v; Node next; }
来源：http://cn.huanxung.cn

Go:   type Node struct { V int; Next *Node }
来源：http://gg.521024.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://hd.hnjuh.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://zt.yuntaijiaju.cn

[N11] 二叉树中序遍历
来源：http://jx.bjjhwx.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://sy.bjjhwx.cn

PHP:  // 手写递归函数
来源：http://av.huanxung.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cf.shtwfgs.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vn.huixiangedu.cn

Java: // 手写递归
来源：http://ni.szsharing.cn

Go:   // 手写递归
来源：http://uy.yuexingan06.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ae.szxytkj.cn

C#:   // 手写递归
来源：http://tl.yuntaijiaju.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://yv.bookmarksfly.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://aw.yuexingan06.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ii.nicolike.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sd.szxytkj.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gy.9csxet.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://bg.hahajie.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://on.colortex.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://lw.asd995.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://eg.yuntaijiaju.cn

================================================================================
来源：http://ii.shxzukj.cn

O. 并发与异步
来源：http://in.9csxet.cn

================================================================================
来源：http://kp.9csxet.cn

[O01] 启动一个线程
来源：http://kc.521024.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://pd.jianghongdianzi.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://nj.szsharing.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://tr.nszjky.cn

TS:   // 同 JS
来源：http://hl.szxytkj.cn

Java: new Thread(() -> f()).start()
来源：http://us.shtwfgs.cn

Go:   go f()
来源：http://cg.nszjky.cn

Ruby: Thread.new { f }
来源：http://ys.szsharing.cn

C#:   Task.Run(() => F());
来源：http://gs.nszjky.cn

[O02] 使用线程池
来源：http://wz.bookmarksfly.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://di.521024.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ky.shtwfgs.cn

JS:   // worker_threads 线程池
来源：http://ew.shxzskj.cn

TS:   // worker_threads 线程池
来源：http://cc.hnjuh.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ei.bookmarksfly.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hx.gzmigu.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://gv.asd995.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://zg.bookmarksfly.cn

[O03] 加锁保护共享数据
来源：http://nv.haigaiapp.cn

Py:   with lock: shared += 1
来源：http://ds.jctech888.com.cn

PHP:  // 用 flock() 做文件锁
来源：http://nu.jctech888.com.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://po.yuexingan06.cn

TS:   // 同 JS
来源：http://qv.nicolike.cn

Java: synchronized (this) { shared++; }
来源：http://ku.shtwfgs.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://st.bookmarksfly.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://aw.nszjky.cn

C#:   lock (gate) { shared++; }
来源：http://nt.yuntaijiaju.cn

[O04] 定义异步函数并等待
来源：http://hy.huixinmuqiang.cn

Py:   async def f():⏎    await g()
来源：http://fy.9csxet.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://do.lnxyls.cn

JS:   async function f() { await g(); }
来源：http://bs.yuntaijiaju.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ss.colortex.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://bj.panjiajie.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://nx.nicolike.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ld.hahajie.cn

C#:   async Task F() { await G(); }
来源：http://lr.jctech888.com.cn

[O05] 并发执行并等待全部完成
来源：http://qy.9csxet.cn

Py:   asyncio.gather(*tasks)
来源：http://nt.szsharing.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://nw.hahajie.cn

JS:   await Promise.all(tasks)
来源：http://et.asd995.cn

TS:   await Promise.all(tasks)
来源：http://xk.nszjky.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://tj.muxihuayi.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://fz.jctech888.com.cn

Ruby: threads.map(&:join)
来源：http://jg.colortex.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://jl.jianghongdianzi.cn

[O06] 使用进程池
来源：http://bm.wgjwhj.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://vc.haigaiapp.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://cx.jctech888.com.cn

JS:   // child_process / cluster 模块
来源：http://hi.szxytkj.cn

TS:   // child_process / cluster 模块
来源：http://fx.huanxung.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://za.chemitech.net.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://js.szxytkj.cn

Ruby: // fork 块
来源：http://to.jianghongdianzi.cn

C#:   Parallel.For
来源：http://cs.haigaiapp.cn

================================================================================
来源：http://qp.muxihuayi.cn

P. 常用工具函数
来源：http://my.wgjwhj.cn

================================================================================
来源：http://mu.521024.cn

[P01] 生成 UUID
来源：http://sy.nszjky.cn

Py:   str(uuid.uuid4())
来源：http://aa.szxytkj.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://yh.jianghongdianzi.cn

JS:   crypto.randomUUID()
来源：http://zd.gzmigu.cn

TS:   crypto.randomUUID()
来源：http://yh.bookmarksfly.cn

Java: UUID.randomUUID().toString()
来源：http://pw.newstarts.cn

Go:   // 用 github.com/google/uuid
来源：http://bg.jianghongdianzi.cn

Ruby: SecureRandom.uuid
来源：http://xc.szsharing.cn

C#:   Guid.NewGuid().ToString()
来源：http://bq.muxihuayi.cn

[P02] MD5 / SHA256 摘要
来源：http://hr.shxzskj.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://dx.chemitech.net.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://gc.wgjwhj.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://dc.asd995.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://dk.jctech888.com.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://kf.panjiajie.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wz.gzmigu.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://cg.gzmigu.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://xo.9csxet.cn

[P03] 生成短随机字符串
来源：http://ek.szxytkj.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wd.hahajie.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://az.nszjky.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wj.yuntaijiaju.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bu.shxzukj.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://lo.nszjky.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://yl.muxihuayi.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://vu.yuntaijiaju.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ed.wgjwhj.cn

[P04] 求长度
来源：http://zo.newstarts.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://sb.shxzukj.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vo.lnxyls.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tn.521024.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rl.jianghongdianzi.cn

Java: list.size();  map.size();  s.length()
来源：http://wq.shxzukj.cn

Go:   len(arr);  len(m)
来源：http://tc.gzmigu.cn

Ruby: x.length;  x.size
来源：http://zt.colortex.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://yk.jianghongdianzi.cn

[P05] 判断两个对象内容是否相等
来源：http://nn.huanxung.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ni.shtwfgs.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://tq.chemitech.net.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://cz.gzmigu.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://xe.lnxyls.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mj.chemitech.net.cn

Go:   reflect.DeepEqual(a, b)
来源：http://su.jianghongdianzi.cn

Ruby: a == b
来源：http://ih.muxihuayi.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://zl.panjiajie.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ii.muxihuayi.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://tv.gzmigu.cn

PHP:  if (empty($x)) {}
来源：http://nh.lnxyls.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wf.yuntaijiaju.cn

TS:   if (x == null) {}
来源：http://me.jctech888.com.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://wu.hahajie.cn

Go:   if x == nil {}
来源：http://rg.nicolike.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://sa.panjiajie.cn

C#:   if (x is null) {}
来源：http://tc.panjiajie.cn

[P07] 防抖与节流
来源：http://oh.huanxung.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ag.yuntaijiaju.cn

PHP:  // 手写时间戳比较
来源：http://kw.asd995.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://my.gzmigu.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uz.lnxyls.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ye.yuntaijiaju.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://dg.wgjwhj.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ef.nicolike.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ra.haigaiapp.cn

[P08] 处理浮点精度问题
来源：http://ww.nicolike.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://vs.jianghongdianzi.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hb.chemitech.net.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://vq.shtwfgs.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ni.nszjky.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://yu.jctech888.com.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ro.nszjky.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://kp.muxihuayi.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ci.nicolike.cn

================================================================================
来源：http://ao.bookmarksfly.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://lf.huanxung.cn

================================================================================
来源：http://zf.nszjky.cn

[Q01] 创建表
来源：http://hj.huixiangedu.cn

CREATE TABLE users (
来源：http://bl.hahajie.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://av.yuexingan06.cn

name VARCHAR(50) NOT NULL,
来源：http://um.shtwfgs.cn

email VARCHAR(100) UNIQUE,
来源：http://ui.nszjky.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://xj.bookmarksfly.cn

);
来源：http://ze.wgjwhj.cn

[Q02] 创建带外键的表
来源：http://zm.panjiajie.cn

CREATE TABLE orders (
来源：http://qg.wgjwhj.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://he.muxihuayi.cn

user_id INT NOT NULL,
来源：http://ro.9csxet.cn

amount DECIMAL(10, 2),
来源：http://xm.szsharing.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://pa.jctech888.com.cn

);
来源：http://xy.shtwfgs.cn

[Q03] 增加列
来源：http://cv.szxytkj.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://xf.shxzukj.cn

[Q04] 修改列类型
来源：http://uc.wgjwhj.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://eu.yuexingan06.cn

[Q05] 重命名列
来源：http://wz.lnxyls.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://zs.hahajie.cn

[Q06] 删除列
来源：http://jm.newstarts.cn

ALTER TABLE users DROP COLUMN age;
来源：http://rb.newstarts.cn

[Q07] 删除表
来源：http://xg.shxzukj.cn

DROP TABLE IF EXISTS orders;
来源：http://bw.szxytkj.cn

[Q08] 创建普通索引
来源：http://rz.muxihuayi.cn


<!-- 参考信息 -->