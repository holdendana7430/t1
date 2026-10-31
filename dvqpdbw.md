代发 wailian999

C#:   Directory.GetCurrentDirectory()
来源：http://uj.bookmarksfly.cn

[M05] 设置退出码
来源：http://bo.521024.cn

Py:   sys.exit(1)
来源：http://jo.9csxet.cn

PHP:  exit(1);
来源：http://ps.muxihuayi.cn

JS:   process.exit(1)
来源：http://pl.lnxyls.cn

TS:   process.exit(1)
来源：http://vb.huixiangedu.cn

Java: System.exit(1)
来源：http://xg.szsharing.cn

Go:   os.Exit(1)
来源：http://ne.shxzukj.cn

Ruby: exit 1
来源：http://ce.yuntaijiaju.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://lh.yuexingan06.cn

[M06] 向标准错误输出
来源：http://wz.bjjhwx.cn

Py:   print("err", file=sys.stderr)
来源：http://fn.bookmarksfly.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ly.nszjky.cn

JS:   console.error("err")
来源：http://ft.shtwfgs.cn

TS:   console.error("err")
来源：http://av.gzmigu.cn

Java: System.err.println("err")
来源：http://zb.gzmigu.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://nl.lnxyls.cn

Ruby: warn "err"
来源：http://dr.muxihuayi.cn

C#:   Console.Error.WriteLine("err")
来源：http://yc.gzmigu.cn

[M07] 判断是否为主入口
来源：http://gr.wgjwhj.cn

Py:   if __name__ == "__main__":
来源：http://if.bookmarksfly.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ck.nszjky.cn

JS:   require.main === module
来源：http://oa.lnxyls.cn

TS:   require.main === module
来源：http://ic.huixinmuqiang.cn

Java: public static void main(String[] args)
来源：http://na.shxzskj.cn

Go:   func main()
来源：http://pa.nicolike.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://zw.bookmarksfly.cn

C#:   static void Main(string[] args)
来源：http://al.muxihuayi.cn

[M08] 获取系统与运行时信息
来源：http://gd.hahajie.cn

Py:   platform.system();  platform.python_version()
来源：http://fv.jctech888.com.cn

PHP:  PHP_OS;  phpversion();
来源：http://jy.gzmigu.cn

JS:   process.platform;  process.version
来源：http://cn.shxzukj.cn

TS:   process.platform;  process.version
来源：http://pe.gzmigu.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://gs.9csxet.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://gw.bjjhwx.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ic.9csxet.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://el.9csxet.cn

================================================================================
来源：http://cw.huixiangedu.cn

N. 数据结构与算法
来源：http://rs.panjiajie.cn

================================================================================
来源：http://au.jianghongdianzi.cn

[N01] 二分查找（有序数组）
来源：http://yx.shtwfgs.cn

Py:   bisect.bisect_left(arr, x)
来源：http://xc.huixiangedu.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://md.9csxet.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nh.bjjhwx.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jd.bjjhwx.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ju.jianghongdianzi.cn

Go:   sort.SearchInts(arr, x)
来源：http://kw.szxytkj.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://xz.521024.cn

C#:   Array.BinarySearch(arr, x)
来源：http://gz.szsharing.cn

[N02] 排序（工程实践用内置实现）
来源：http://aa.yuexingan06.cn

Py:   sorted(arr);  arr.sort()
来源：http://rx.colortex.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ff.asd995.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://mz.haigaiapp.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://mk.colortex.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://eo.wgjwhj.cn

Go:   slices.Sort(arr)
来源：http://sw.huixiangedu.cn

Ruby: arr.sort
来源：http://wb.chemitech.net.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://fe.asd995.cn

[N03] 快速排序（分治示例）
来源：http://rz.hahajie.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://cs.shxzukj.cn

PHP:  // 递归实现，或用 usort
来源：http://hf.jctech888.com.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zh.bookmarksfly.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qt.huixiangedu.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://lp.haigaiapp.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ev.szsharing.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://yp.shxzukj.cn

C#:   // 手写递归，或 Array.Sort
来源：http://vj.newstarts.cn

[N04] 斐波那契数列
来源：http://lb.panjiajie.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://yh.shxzukj.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wu.yuexingan06.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://uk.shtwfgs.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ba.521024.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://oh.asd995.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://gd.hnjuh.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ru.lnxyls.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mj.yuntaijiaju.cn

[N05] 最大公约数
来源：http://fz.nszjky.cn

Py:   math.gcd(a, b)
来源：http://mp.nicolike.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ah.521024.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zi.lnxyls.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sj.shxzskj.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://sy.wgjwhj.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hb.szxytkj.cn

Ruby: a.gcd(b)
来源：http://ay.haigaiapp.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://qh.colortex.cn

[N06] 判断回文字符串
来源：http://zr.huixinmuqiang.cn

Py:   s == s[::-1]
来源：http://wf.9csxet.cn

PHP:  $s === strrev($s);
来源：http://cg.colortex.cn

JS:   s === [...s].reverse().join("")
来源：http://uj.colortex.cn

TS:   s === [...s].reverse().join("")
来源：http://ly.shxzukj.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ac.panjiajie.cn

Go:   // 双指针从两端比较
来源：http://yw.521024.cn

Ruby: s == s.reverse
来源：http://yj.lnxyls.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://jr.shxzukj.cn

[N07] 两数之和（返回下标）
来源：http://yg.yuntaijiaju.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://cy.yuexingan06.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://gl.hahajie.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://vs.nszjky.cn

TS:   // 手写 Map<string, number>
来源：http://qs.nszjky.cn

Java: // 手写 HashMap
来源：http://ja.521024.cn

Go:   // 手写 map[int]int
来源：http://op.yuexingan06.cn

Ruby: // 手写 Hash
来源：http://dn.szsharing.cn

C#:   // 手写 Dictionary<int, int>
来源：http://hb.lnxyls.cn

[N08] 生成全排列
来源：http://yo.asd995.cn

Py:   itertools.permutations(arr)
来源：http://ry.bjjhwx.cn

PHP:  // 手写递归交换
来源：http://ou.shxzukj.cn

JS:   // 手写回溯递归
来源：http://ww.yuntaijiaju.cn

TS:   // 手写回溯递归
来源：http://co.521024.cn

Java: // 手写回溯递归
来源：http://yw.haigaiapp.cn

Go:   // 手写回溯递归
来源：http://jp.szxytkj.cn

Ruby: arr.permutation.to_a
来源：http://ag.panjiajie.cn

C#:   // 手写回溯递归
来源：http://mn.haigaiapp.cn

[N09] 栈与队列
来源：http://vn.szsharing.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://gv.521024.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://xt.bookmarksfly.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://pq.gzmigu.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://te.haigaiapp.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://br.yuexingan06.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://zj.yuexingan06.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ei.hnjuh.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://gh.lnxyls.cn

[N10] 链表节点定义
来源：http://ad.bookmarksfly.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qq.huixinmuqiang.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://hn.lnxyls.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://rg.jctech888.com.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://up.wgjwhj.cn

Java: class Node { int v; Node next; }
来源：http://hi.wgjwhj.cn

Go:   type Node struct { V int; Next *Node }
来源：http://as.yuexingan06.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://qk.lnxyls.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://lh.shtwfgs.cn

[N11] 二叉树中序遍历
来源：http://ns.shxzukj.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://gn.lnxyls.cn

PHP:  // 手写递归函数
来源：http://fw.asd995.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sy.huanxung.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pf.newstarts.cn

Java: // 手写递归
来源：http://ll.colortex.cn

Go:   // 手写递归
来源：http://em.bjjhwx.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://jb.shtwfgs.cn

C#:   // 手写递归
来源：http://hy.huixiangedu.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ua.shtwfgs.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ih.newstarts.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://kr.panjiajie.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://re.newstarts.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zf.muxihuayi.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://rr.colortex.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ow.jctech888.com.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://cu.haigaiapp.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://dg.hnjuh.cn

================================================================================
来源：http://bu.shxzskj.cn

O. 并发与异步
来源：http://vh.shxzukj.cn

================================================================================
来源：http://ho.521024.cn

[O01] 启动一个线程
来源：http://vs.9csxet.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://uf.shxzskj.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://er.yuexingan06.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://xh.yuexingan06.cn

TS:   // 同 JS
来源：http://tt.haigaiapp.cn

Java: new Thread(() -> f()).start()
来源：http://rd.huanxung.cn

Go:   go f()
来源：http://sz.chemitech.net.cn

Ruby: Thread.new { f }
来源：http://rf.lnxyls.cn

C#:   Task.Run(() => F());
来源：http://dj.shxzukj.cn

[O02] 使用线程池
来源：http://us.colortex.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://vh.shxzskj.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mg.9csxet.cn

JS:   // worker_threads 线程池
来源：http://hy.hnjuh.cn

TS:   // worker_threads 线程池
来源：http://yv.yuntaijiaju.cn

Java: Executors.newFixedThreadPool(4)
来源：http://pz.jianghongdianzi.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://pd.hnjuh.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ah.shxzskj.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hb.chemitech.net.cn

[O03] 加锁保护共享数据
来源：http://nq.huanxung.cn

Py:   with lock: shared += 1
来源：http://oy.jctech888.com.cn

PHP:  // 用 flock() 做文件锁
来源：http://ew.jianghongdianzi.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://zn.haigaiapp.cn

TS:   // 同 JS
来源：http://ol.colortex.cn

Java: synchronized (this) { shared++; }
来源：http://uq.yuntaijiaju.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hy.lnxyls.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://nu.wgjwhj.cn

C#:   lock (gate) { shared++; }
来源：http://my.nicolike.cn

[O04] 定义异步函数并等待
来源：http://gw.szxytkj.cn

Py:   async def f():⏎    await g()
来源：http://cr.szxytkj.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://fx.yuexingan06.cn

JS:   async function f() { await g(); }
来源：http://ar.hnjuh.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://zj.hahajie.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://tq.huixinmuqiang.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://tu.bookmarksfly.cn

Ruby: # 用 Fiber 或 async gem
来源：http://nv.yuexingan06.cn

C#:   async Task F() { await G(); }
来源：http://tg.nicolike.cn

[O05] 并发执行并等待全部完成
来源：http://ez.shxzukj.cn

Py:   asyncio.gather(*tasks)
来源：http://uf.521024.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://cx.colortex.cn

JS:   await Promise.all(tasks)
来源：http://kb.hahajie.cn

TS:   await Promise.all(tasks)
来源：http://az.shtwfgs.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://dg.nicolike.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://qw.asd995.cn

Ruby: threads.map(&:join)
来源：http://sh.newstarts.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://gn.gzmigu.cn

[O06] 使用进程池
来源：http://to.bookmarksfly.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://aw.yuntaijiaju.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://rw.szxytkj.cn

JS:   // child_process / cluster 模块
来源：http://oi.shxzukj.cn

TS:   // child_process / cluster 模块
来源：http://ll.shxzukj.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://vl.newstarts.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://uq.colortex.cn

Ruby: // fork 块
来源：http://fa.yuntaijiaju.cn

C#:   Parallel.For
来源：http://bu.huixiangedu.cn

================================================================================
来源：http://dg.yuntaijiaju.cn

P. 常用工具函数
来源：http://en.jctech888.com.cn

================================================================================
来源：http://pu.huixiangedu.cn

[P01] 生成 UUID
来源：http://di.yuntaijiaju.cn

Py:   str(uuid.uuid4())
来源：http://pi.yuexingan06.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://qm.shtwfgs.cn

JS:   crypto.randomUUID()
来源：http://zk.colortex.cn

TS:   crypto.randomUUID()
来源：http://yz.hnjuh.cn

Java: UUID.randomUUID().toString()
来源：http://vg.9csxet.cn

Go:   // 用 github.com/google/uuid
来源：http://ih.lnxyls.cn

Ruby: SecureRandom.uuid
来源：http://lc.shtwfgs.cn

C#:   Guid.NewGuid().ToString()
来源：http://bc.yuexingan06.cn

[P02] MD5 / SHA256 摘要
来源：http://ks.yuexingan06.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://np.wgjwhj.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://iw.shtwfgs.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://xr.yuntaijiaju.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://tm.gzmigu.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://cu.bookmarksfly.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ly.nicolike.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://qn.jianghongdianzi.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://un.jianghongdianzi.cn

[P03] 生成短随机字符串
来源：http://qi.yuntaijiaju.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://bl.haigaiapp.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ak.asd995.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pi.bjjhwx.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cu.yuntaijiaju.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wp.jianghongdianzi.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ma.haigaiapp.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://oa.yuntaijiaju.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ak.shxzukj.cn

[P04] 求长度
来源：http://sg.jctech888.com.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://uu.chemitech.net.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ya.huixiangedu.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nj.yuexingan06.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ud.yuntaijiaju.cn

Java: list.size();  map.size();  s.length()
来源：http://tt.9csxet.cn

Go:   len(arr);  len(m)
来源：http://hv.hahajie.cn

Ruby: x.length;  x.size
来源：http://zi.yuexingan06.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://lr.shxzukj.cn

[P05] 判断两个对象内容是否相等
来源：http://bp.newstarts.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://tc.shxzskj.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://pb.9csxet.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://sw.haigaiapp.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://fq.hnjuh.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://rs.haigaiapp.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ts.jctech888.com.cn

Ruby: a == b
来源：http://ng.jianghongdianzi.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://db.521024.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ae.nszjky.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://oi.asd995.cn

PHP:  if (empty($x)) {}
来源：http://zd.jctech888.com.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ne.jctech888.com.cn

TS:   if (x == null) {}
来源：http://cn.szsharing.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://uf.521024.cn

Go:   if x == nil {}
来源：http://pb.yuntaijiaju.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ud.yuntaijiaju.cn

C#:   if (x is null) {}
来源：http://un.shtwfgs.cn

[P07] 防抖与节流
来源：http://tl.newstarts.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://kc.szsharing.cn

PHP:  // 手写时间戳比较
来源：http://ko.shxzskj.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://di.bookmarksfly.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ve.jianghongdianzi.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://sf.jianghongdianzi.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://zn.yuntaijiaju.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://pj.chemitech.net.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ra.huixinmuqiang.cn

[P08] 处理浮点精度问题
来源：http://vm.asd995.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://za.chemitech.net.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://tg.9csxet.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://yu.hnjuh.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://dz.panjiajie.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wx.jctech888.com.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://tk.panjiajie.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mk.newstarts.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wc.shxzukj.cn

================================================================================
来源：http://bn.bookmarksfly.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://cx.hahajie.cn

================================================================================
来源：http://bu.lnxyls.cn

[Q01] 创建表
来源：http://bf.szsharing.cn

CREATE TABLE users (
来源：http://tb.yuntaijiaju.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://uf.521024.cn

name VARCHAR(50) NOT NULL,
来源：http://os.jianghongdianzi.cn

email VARCHAR(100) UNIQUE,
来源：http://zv.yuexingan06.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mj.szxytkj.cn

);
来源：http://ek.shtwfgs.cn

[Q02] 创建带外键的表
来源：http://ce.shtwfgs.cn

CREATE TABLE orders (
来源：http://ol.newstarts.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://vk.huixinmuqiang.cn

user_id INT NOT NULL,
来源：http://zh.panjiajie.cn

amount DECIMAL(10, 2),
来源：http://ui.newstarts.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hw.asd995.cn

);
来源：http://bs.hahajie.cn

[Q03] 增加列
来源：http://tq.szxytkj.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://qv.521024.cn

[Q04] 修改列类型
来源：http://mn.hnjuh.cn


<!-- 参考信息 -->