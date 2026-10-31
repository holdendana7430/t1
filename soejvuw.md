代发 wailian999

C#:   Directory.GetCurrentDirectory()
来源：http://cs.wgjwhj.cn

[M05] 设置退出码
来源：http://pk.huixiangedu.cn

Py:   sys.exit(1)
来源：http://sz.bjjhwx.cn

PHP:  exit(1);
来源：http://sc.szsharing.cn

JS:   process.exit(1)
来源：http://rd.yuntaijiaju.cn

TS:   process.exit(1)
来源：http://xt.nszjky.cn

Java: System.exit(1)
来源：http://ly.bookmarksfly.cn

Go:   os.Exit(1)
来源：http://rw.newstarts.cn

Ruby: exit 1
来源：http://ku.chemitech.net.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://pq.yuntaijiaju.cn

[M06] 向标准错误输出
来源：http://iy.chemitech.net.cn

Py:   print("err", file=sys.stderr)
来源：http://by.521024.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://eb.bookmarksfly.cn

JS:   console.error("err")
来源：http://cx.huixiangedu.cn

TS:   console.error("err")
来源：http://fb.szxytkj.cn

Java: System.err.println("err")
来源：http://hb.hahajie.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://vk.asd995.cn

Ruby: warn "err"
来源：http://we.huixiangedu.cn

C#:   Console.Error.WriteLine("err")
来源：http://hm.wgjwhj.cn

[M07] 判断是否为主入口
来源：http://gp.shtwfgs.cn

Py:   if __name__ == "__main__":
来源：http://qm.hahajie.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://xr.szsharing.cn

JS:   require.main === module
来源：http://ld.9csxet.cn

TS:   require.main === module
来源：http://rc.yuntaijiaju.cn

Java: public static void main(String[] args)
来源：http://ky.gzmigu.cn

Go:   func main()
来源：http://wt.nicolike.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://xr.colortex.cn

C#:   static void Main(string[] args)
来源：http://rr.panjiajie.cn

[M08] 获取系统与运行时信息
来源：http://xs.wgjwhj.cn

Py:   platform.system();  platform.python_version()
来源：http://ac.jctech888.com.cn

PHP:  PHP_OS;  phpversion();
来源：http://gc.szxytkj.cn

JS:   process.platform;  process.version
来源：http://uc.jctech888.com.cn

TS:   process.platform;  process.version
来源：http://sq.hnjuh.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://rq.asd995.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://sg.newstarts.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://kl.szsharing.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://gm.shtwfgs.cn

================================================================================
来源：http://gp.wgjwhj.cn

N. 数据结构与算法
来源：http://wy.hahajie.cn

================================================================================
来源：http://oe.yuexingan06.cn

[N01] 二分查找（有序数组）
来源：http://df.chemitech.net.cn

Py:   bisect.bisect_left(arr, x)
来源：http://mn.panjiajie.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://xf.yuntaijiaju.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xq.bjjhwx.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qu.jctech888.com.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ca.nszjky.cn

Go:   sort.SearchInts(arr, x)
来源：http://rq.shtwfgs.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://qt.jianghongdianzi.cn

C#:   Array.BinarySearch(arr, x)
来源：http://rx.haigaiapp.cn

[N02] 排序（工程实践用内置实现）
来源：http://yo.huanxung.cn

Py:   sorted(arr);  arr.sort()
来源：http://sh.gzmigu.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://an.shtwfgs.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://nq.panjiajie.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://xk.chemitech.net.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://nl.yuntaijiaju.cn

Go:   slices.Sort(arr)
来源：http://oh.panjiajie.cn

Ruby: arr.sort
来源：http://qa.nszjky.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://zh.muxihuayi.cn

[N03] 快速排序（分治示例）
来源：http://nh.jianghongdianzi.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://gi.gzmigu.cn

PHP:  // 递归实现，或用 usort
来源：http://fy.huixiangedu.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bb.jctech888.com.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://in.hnjuh.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://oe.9csxet.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://bv.gzmigu.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://eh.hnjuh.cn

C#:   // 手写递归，或 Array.Sort
来源：http://jp.haigaiapp.cn

[N04] 斐波那契数列
来源：http://jb.yuexingan06.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://cq.szsharing.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://zg.bookmarksfly.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ib.panjiajie.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ji.shxzukj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://qv.jianghongdianzi.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ze.nicolike.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://rn.wgjwhj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://yu.wgjwhj.cn

[N05] 最大公约数
来源：http://go.chemitech.net.cn

Py:   math.gcd(a, b)
来源：http://cl.shxzukj.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ey.asd995.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qc.shxzukj.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ty.newstarts.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ey.yuexingan06.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://jo.chemitech.net.cn

Ruby: a.gcd(b)
来源：http://eu.bjjhwx.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mn.colortex.cn

[N06] 判断回文字符串
来源：http://ze.asd995.cn

Py:   s == s[::-1]
来源：http://ed.jctech888.com.cn

PHP:  $s === strrev($s);
来源：http://qm.yuexingan06.cn

JS:   s === [...s].reverse().join("")
来源：http://dy.gzmigu.cn

TS:   s === [...s].reverse().join("")
来源：http://iu.wgjwhj.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://sy.gzmigu.cn

Go:   // 双指针从两端比较
来源：http://pm.nicolike.cn

Ruby: s == s.reverse
来源：http://wk.bjjhwx.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://jx.colortex.cn

[N07] 两数之和（返回下标）
来源：http://ls.jianghongdianzi.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://tr.colortex.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mh.shxzskj.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://eu.huixiangedu.cn

TS:   // 手写 Map<string, number>
来源：http://uc.shtwfgs.cn

Java: // 手写 HashMap
来源：http://un.bjjhwx.cn

Go:   // 手写 map[int]int
来源：http://xt.nszjky.cn

Ruby: // 手写 Hash
来源：http://vi.jianghongdianzi.cn

C#:   // 手写 Dictionary<int, int>
来源：http://hw.nicolike.cn

[N08] 生成全排列
来源：http://gf.bookmarksfly.cn

Py:   itertools.permutations(arr)
来源：http://mm.huixiangedu.cn

PHP:  // 手写递归交换
来源：http://lt.panjiajie.cn

JS:   // 手写回溯递归
来源：http://vh.haigaiapp.cn

TS:   // 手写回溯递归
来源：http://ts.hnjuh.cn

Java: // 手写回溯递归
来源：http://xn.huanxung.cn

Go:   // 手写回溯递归
来源：http://fo.huixiangedu.cn

Ruby: arr.permutation.to_a
来源：http://dq.szxytkj.cn

C#:   // 手写回溯递归
来源：http://ye.9csxet.cn

[N09] 栈与队列
来源：http://tt.hnjuh.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://of.muxihuayi.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hg.shtwfgs.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://df.szsharing.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ix.bjjhwx.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://qw.bjjhwx.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ji.gzmigu.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://bf.chemitech.net.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ef.muxihuayi.cn

[N10] 链表节点定义
来源：http://uf.bookmarksfly.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://bm.asd995.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://kb.lnxyls.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://to.bjjhwx.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://sl.bookmarksfly.cn

Java: class Node { int v; Node next; }
来源：http://hu.panjiajie.cn

Go:   type Node struct { V int; Next *Node }
来源：http://oo.asd995.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://zs.chemitech.net.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://je.gzmigu.cn

[N11] 二叉树中序遍历
来源：http://ae.chemitech.net.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://lv.yuntaijiaju.cn

PHP:  // 手写递归函数
来源：http://tk.lnxyls.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yi.yuexingan06.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wp.asd995.cn

Java: // 手写递归
来源：http://ut.jianghongdianzi.cn

Go:   // 手写递归
来源：http://ft.colortex.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://xy.jctech888.com.cn

C#:   // 手写递归
来源：http://ip.shxzskj.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://co.shxzukj.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ev.jianghongdianzi.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ci.hahajie.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ha.huanxung.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wq.jianghongdianzi.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://gf.huixiangedu.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://th.asd995.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://zp.panjiajie.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://iq.521024.cn

================================================================================
来源：http://ic.yuntaijiaju.cn

O. 并发与异步
来源：http://sm.9csxet.cn

================================================================================
来源：http://fd.huanxung.cn

[O01] 启动一个线程
来源：http://yq.shxzukj.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://gp.jctech888.com.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hs.yuexingan06.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://iw.yuexingan06.cn

TS:   // 同 JS
来源：http://id.shtwfgs.cn

Java: new Thread(() -> f()).start()
来源：http://ki.colortex.cn

Go:   go f()
来源：http://vs.bookmarksfly.cn

Ruby: Thread.new { f }
来源：http://wv.yuntaijiaju.cn

C#:   Task.Run(() => F());
来源：http://ip.wgjwhj.cn

[O02] 使用线程池
来源：http://rt.asd995.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://pl.asd995.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hu.huanxung.cn

JS:   // worker_threads 线程池
来源：http://hs.bookmarksfly.cn

TS:   // worker_threads 线程池
来源：http://ej.shxzskj.cn

Java: Executors.newFixedThreadPool(4)
来源：http://qk.yuexingan06.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ah.szxytkj.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://gp.hnjuh.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://xm.9csxet.cn

[O03] 加锁保护共享数据
来源：http://qi.nszjky.cn

Py:   with lock: shared += 1
来源：http://xu.colortex.cn

PHP:  // 用 flock() 做文件锁
来源：http://kv.shtwfgs.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://pt.bjjhwx.cn

TS:   // 同 JS
来源：http://dq.colortex.cn

Java: synchronized (this) { shared++; }
来源：http://pp.shxzskj.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://vi.asd995.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://vf.9csxet.cn

C#:   lock (gate) { shared++; }
来源：http://tg.asd995.cn

[O04] 定义异步函数并等待
来源：http://kc.jctech888.com.cn

Py:   async def f():⏎    await g()
来源：http://ny.bjjhwx.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://pb.yuntaijiaju.cn

JS:   async function f() { await g(); }
来源：http://mf.huanxung.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://gi.asd995.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://dp.gzmigu.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://vq.521024.cn

Ruby: # 用 Fiber 或 async gem
来源：http://jl.9csxet.cn

C#:   async Task F() { await G(); }
来源：http://dm.jianghongdianzi.cn

[O05] 并发执行并等待全部完成
来源：http://jk.asd995.cn

Py:   asyncio.gather(*tasks)
来源：http://we.hahajie.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://av.yuntaijiaju.cn

JS:   await Promise.all(tasks)
来源：http://ik.huixiangedu.cn

TS:   await Promise.all(tasks)
来源：http://pv.asd995.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://sb.hahajie.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://or.haigaiapp.cn

Ruby: threads.map(&:join)
来源：http://sb.shxzskj.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://dm.panjiajie.cn

[O06] 使用进程池
来源：http://mm.9csxet.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://nb.haigaiapp.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://qb.huixinmuqiang.cn

JS:   // child_process / cluster 模块
来源：http://rh.newstarts.cn

TS:   // child_process / cluster 模块
来源：http://jz.haigaiapp.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://cy.hnjuh.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://qj.nicolike.cn

Ruby: // fork 块
来源：http://kv.haigaiapp.cn

C#:   Parallel.For
来源：http://zu.nszjky.cn

================================================================================
来源：http://ru.colortex.cn

P. 常用工具函数
来源：http://vj.jctech888.com.cn

================================================================================
来源：http://az.gzmigu.cn

[P01] 生成 UUID
来源：http://qe.jianghongdianzi.cn

Py:   str(uuid.uuid4())
来源：http://cw.gzmigu.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ys.nicolike.cn

JS:   crypto.randomUUID()
来源：http://gr.haigaiapp.cn

TS:   crypto.randomUUID()
来源：http://sh.szsharing.cn

Java: UUID.randomUUID().toString()
来源：http://ap.bjjhwx.cn

Go:   // 用 github.com/google/uuid
来源：http://qv.bjjhwx.cn

Ruby: SecureRandom.uuid
来源：http://bn.colortex.cn

C#:   Guid.NewGuid().ToString()
来源：http://qg.bjjhwx.cn

[P02] MD5 / SHA256 摘要
来源：http://pc.panjiajie.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://kp.bjjhwx.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://yk.muxihuayi.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ri.muxihuayi.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://yr.chemitech.net.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://tc.9csxet.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://kt.panjiajie.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ee.huixinmuqiang.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://qv.hahajie.cn

[P03] 生成短随机字符串
来源：http://xp.wgjwhj.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wx.bookmarksfly.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://dn.wgjwhj.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kn.nszjky.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gz.shxzskj.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://cm.bjjhwx.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://vf.asd995.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ha.521024.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://dz.gzmigu.cn

[P04] 求长度
来源：http://la.wgjwhj.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://jh.wgjwhj.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rf.colortex.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://et.521024.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qu.muxihuayi.cn

Java: list.size();  map.size();  s.length()
来源：http://lc.yuexingan06.cn

Go:   len(arr);  len(m)
来源：http://jv.9csxet.cn

Ruby: x.length;  x.size
来源：http://fd.szsharing.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://dn.szxytkj.cn

[P05] 判断两个对象内容是否相等
来源：http://dz.hnjuh.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://vs.hnjuh.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ev.shxzukj.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://bf.newstarts.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://lo.nicolike.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://gm.chemitech.net.cn

Go:   reflect.DeepEqual(a, b)
来源：http://yo.huixinmuqiang.cn

Ruby: a == b
来源：http://oi.yuexingan06.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ve.panjiajie.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ny.shtwfgs.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://sy.asd995.cn

PHP:  if (empty($x)) {}
来源：http://pp.huanxung.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ii.newstarts.cn

TS:   if (x == null) {}
来源：http://fh.bjjhwx.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://jb.521024.cn

Go:   if x == nil {}
来源：http://ia.9csxet.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://vr.shxzskj.cn

C#:   if (x is null) {}
来源：http://xg.shtwfgs.cn

[P07] 防抖与节流
来源：http://bo.shxzukj.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://md.yuntaijiaju.cn

PHP:  // 手写时间戳比较
来源：http://sc.wgjwhj.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dg.nicolike.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://au.szxytkj.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://br.newstarts.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ki.yuntaijiaju.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://th.nicolike.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ng.9csxet.cn

[P08] 处理浮点精度问题
来源：http://ey.gzmigu.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://pq.521024.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://em.shtwfgs.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://rt.colortex.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://jb.nicolike.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ot.gzmigu.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://cq.shxzskj.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://vm.9csxet.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://gi.szxytkj.cn

================================================================================
来源：http://ls.chemitech.net.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://oj.jianghongdianzi.cn

================================================================================
来源：http://wf.muxihuayi.cn

[Q01] 创建表
来源：http://gd.yuntaijiaju.cn

CREATE TABLE users (
来源：http://rb.newstarts.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://jj.colortex.cn

name VARCHAR(50) NOT NULL,
来源：http://ed.hahajie.cn

email VARCHAR(100) UNIQUE,
来源：http://zd.szsharing.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://kl.panjiajie.cn

);
来源：http://ia.jianghongdianzi.cn

[Q02] 创建带外键的表
来源：http://kz.huixinmuqiang.cn

CREATE TABLE orders (
来源：http://gh.nicolike.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ro.nicolike.cn

user_id INT NOT NULL,
来源：http://jj.newstarts.cn

amount DECIMAL(10, 2),
来源：http://cg.jctech888.com.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hh.huixinmuqiang.cn

);
来源：http://sl.chemitech.net.cn

[Q03] 增加列
来源：http://io.haigaiapp.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ru.colortex.cn

[Q04] 修改列类型
来源：http://ou.shxzskj.cn


<!-- 参考信息 -->