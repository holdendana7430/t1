代发 wailian999

C#:   Directory.GetCurrentDirectory()
来源：http://vo.jctech888.com.cn

[M05] 设置退出码
来源：http://hn.muxihuayi.cn

Py:   sys.exit(1)
来源：http://eu.9csxet.cn

PHP:  exit(1);
来源：http://lt.shxzskj.cn

JS:   process.exit(1)
来源：http://cm.muxihuayi.cn

TS:   process.exit(1)
来源：http://ob.nszjky.cn

Java: System.exit(1)
来源：http://nh.szxytkj.cn

Go:   os.Exit(1)
来源：http://qf.bjjhwx.cn

Ruby: exit 1
来源：http://py.jianghongdianzi.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://es.9csxet.cn

[M06] 向标准错误输出
来源：http://yk.hahajie.cn

Py:   print("err", file=sys.stderr)
来源：http://rq.huanxung.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://hm.szxytkj.cn

JS:   console.error("err")
来源：http://tu.newstarts.cn

TS:   console.error("err")
来源：http://nn.huanxung.cn

Java: System.err.println("err")
来源：http://ud.jctech888.com.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ir.huanxung.cn

Ruby: warn "err"
来源：http://ps.newstarts.cn

C#:   Console.Error.WriteLine("err")
来源：http://ab.yuexingan06.cn

[M07] 判断是否为主入口
来源：http://lb.wgjwhj.cn

Py:   if __name__ == "__main__":
来源：http://yp.bjjhwx.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://tn.bookmarksfly.cn

JS:   require.main === module
来源：http://je.haigaiapp.cn

TS:   require.main === module
来源：http://we.huanxung.cn

Java: public static void main(String[] args)
来源：http://rg.asd995.cn

Go:   func main()
来源：http://ci.bookmarksfly.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://uq.lnxyls.cn

C#:   static void Main(string[] args)
来源：http://nb.bookmarksfly.cn

[M08] 获取系统与运行时信息
来源：http://om.wgjwhj.cn

Py:   platform.system();  platform.python_version()
来源：http://ik.gzmigu.cn

PHP:  PHP_OS;  phpversion();
来源：http://yf.asd995.cn

JS:   process.platform;  process.version
来源：http://yl.jianghongdianzi.cn

TS:   process.platform;  process.version
来源：http://km.huixiangedu.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://rv.bookmarksfly.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://bl.shxzukj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://to.huanxung.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://eo.newstarts.cn

================================================================================
来源：http://lm.yuexingan06.cn

N. 数据结构与算法
来源：http://zz.colortex.cn

================================================================================
来源：http://os.shtwfgs.cn

[N01] 二分查找（有序数组）
来源：http://mm.jctech888.com.cn

Py:   bisect.bisect_left(arr, x)
来源：http://mr.shxzskj.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://fa.yuntaijiaju.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lz.wgjwhj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cj.muxihuayi.cn

Java: Arrays.binarySearch(arr, x)
来源：http://uv.szxytkj.cn

Go:   sort.SearchInts(arr, x)
来源：http://bb.huanxung.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://oz.nicolike.cn

C#:   Array.BinarySearch(arr, x)
来源：http://fg.shxzukj.cn

[N02] 排序（工程实践用内置实现）
来源：http://sc.huixiangedu.cn

Py:   sorted(arr);  arr.sort()
来源：http://ao.shtwfgs.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ck.colortex.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://nj.colortex.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://hn.hahajie.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://oz.yuntaijiaju.cn

Go:   slices.Sort(arr)
来源：http://wv.haigaiapp.cn

Ruby: arr.sort
来源：http://dg.lnxyls.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://qk.bookmarksfly.cn

[N03] 快速排序（分治示例）
来源：http://af.bookmarksfly.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mv.newstarts.cn

PHP:  // 递归实现，或用 usort
来源：http://rl.bjjhwx.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://oo.521024.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nc.bjjhwx.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://og.chemitech.net.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ie.9csxet.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ad.asd995.cn

C#:   // 手写递归，或 Array.Sort
来源：http://lj.nszjky.cn

[N04] 斐波那契数列
来源：http://we.huanxung.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ev.shxzskj.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ks.nszjky.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ab.szsharing.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nx.huixiangedu.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://uy.yuexingan06.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ep.shxzskj.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://bt.hnjuh.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ri.shxzskj.cn

[N05] 最大公约数
来源：http://ph.szxytkj.cn

Py:   math.gcd(a, b)
来源：http://ax.521024.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://rx.huixiangedu.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lz.521024.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ek.szsharing.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://gp.shxzukj.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://co.9csxet.cn

Ruby: a.gcd(b)
来源：http://vc.huixinmuqiang.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://xz.szxytkj.cn

[N06] 判断回文字符串
来源：http://ej.shxzskj.cn

Py:   s == s[::-1]
来源：http://an.jctech888.com.cn

PHP:  $s === strrev($s);
来源：http://sx.yuexingan06.cn

JS:   s === [...s].reverse().join("")
来源：http://ad.jianghongdianzi.cn

TS:   s === [...s].reverse().join("")
来源：http://ok.wgjwhj.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://vd.asd995.cn

Go:   // 双指针从两端比较
来源：http://bs.yuntaijiaju.cn

Ruby: s == s.reverse
来源：http://tc.shtwfgs.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://dm.nszjky.cn

[N07] 两数之和（返回下标）
来源：http://jt.gzmigu.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://qy.jctech888.com.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://pu.huixinmuqiang.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://tn.szsharing.cn

TS:   // 手写 Map<string, number>
来源：http://vx.bookmarksfly.cn

Java: // 手写 HashMap
来源：http://fc.wgjwhj.cn

Go:   // 手写 map[int]int
来源：http://wz.hnjuh.cn

Ruby: // 手写 Hash
来源：http://vx.szsharing.cn

C#:   // 手写 Dictionary<int, int>
来源：http://kg.521024.cn

[N08] 生成全排列
来源：http://pb.lnxyls.cn

Py:   itertools.permutations(arr)
来源：http://zu.colortex.cn

PHP:  // 手写递归交换
来源：http://ja.panjiajie.cn

JS:   // 手写回溯递归
来源：http://vg.shxzskj.cn

TS:   // 手写回溯递归
来源：http://oi.hahajie.cn

Java: // 手写回溯递归
来源：http://oo.huanxung.cn

Go:   // 手写回溯递归
来源：http://vz.huanxung.cn

Ruby: arr.permutation.to_a
来源：http://qa.shxzskj.cn

C#:   // 手写回溯递归
来源：http://bc.huixinmuqiang.cn

[N09] 栈与队列
来源：http://hb.chemitech.net.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wg.nicolike.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://br.bookmarksfly.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://pg.wgjwhj.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://lt.nszjky.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://rk.chemitech.net.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://tw.asd995.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ho.jctech888.com.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ei.shtwfgs.cn

[N10] 链表节点定义
来源：http://bk.huixinmuqiang.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hn.shxzukj.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://iq.panjiajie.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://cj.nicolike.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ms.9csxet.cn

Java: class Node { int v; Node next; }
来源：http://re.nszjky.cn

Go:   type Node struct { V int; Next *Node }
来源：http://za.521024.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://fg.panjiajie.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://wa.colortex.cn

[N11] 二叉树中序遍历
来源：http://zn.shtwfgs.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://cw.szsharing.cn

PHP:  // 手写递归函数
来源：http://xr.muxihuayi.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wa.yuntaijiaju.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zn.yuntaijiaju.cn

Java: // 手写递归
来源：http://dt.lnxyls.cn

Go:   // 手写递归
来源：http://oe.shxzukj.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://jy.bookmarksfly.cn

C#:   // 手写递归
来源：http://ys.nicolike.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wl.shxzskj.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ie.9csxet.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://br.521024.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ae.bjjhwx.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fa.newstarts.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://yl.hahajie.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mh.huixinmuqiang.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://cr.9csxet.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://rl.nszjky.cn

================================================================================
来源：http://cn.hahajie.cn

O. 并发与异步
来源：http://tm.haigaiapp.cn

================================================================================
来源：http://me.chemitech.net.cn

[O01] 启动一个线程
来源：http://op.nicolike.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://cv.521024.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://yc.9csxet.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ez.haigaiapp.cn

TS:   // 同 JS
来源：http://vj.szxytkj.cn

Java: new Thread(() -> f()).start()
来源：http://uz.hahajie.cn

Go:   go f()
来源：http://gs.yuntaijiaju.cn

Ruby: Thread.new { f }
来源：http://de.hnjuh.cn

C#:   Task.Run(() => F());
来源：http://tb.hahajie.cn

[O02] 使用线程池
来源：http://ys.muxihuayi.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://sb.newstarts.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://cs.huixinmuqiang.cn

JS:   // worker_threads 线程池
来源：http://al.muxihuayi.cn

TS:   // worker_threads 线程池
来源：http://sh.szxytkj.cn

Java: Executors.newFixedThreadPool(4)
来源：http://gq.bjjhwx.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://bo.panjiajie.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://kp.huixiangedu.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://bj.shxzskj.cn

[O03] 加锁保护共享数据
来源：http://mw.szxytkj.cn

Py:   with lock: shared += 1
来源：http://en.panjiajie.cn

PHP:  // 用 flock() 做文件锁
来源：http://ns.huixinmuqiang.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ki.yuntaijiaju.cn

TS:   // 同 JS
来源：http://qs.nszjky.cn

Java: synchronized (this) { shared++; }
来源：http://tw.chemitech.net.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://vv.521024.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://kh.newstarts.cn

C#:   lock (gate) { shared++; }
来源：http://jm.bookmarksfly.cn

[O04] 定义异步函数并等待
来源：http://sw.panjiajie.cn

Py:   async def f():⏎    await g()
来源：http://vw.shtwfgs.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://vi.haigaiapp.cn

JS:   async function f() { await g(); }
来源：http://ll.bookmarksfly.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ap.hnjuh.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://oz.jianghongdianzi.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ol.newstarts.cn

Ruby: # 用 Fiber 或 async gem
来源：http://io.gzmigu.cn

C#:   async Task F() { await G(); }
来源：http://nt.nszjky.cn

[O05] 并发执行并等待全部完成
来源：http://po.wgjwhj.cn

Py:   asyncio.gather(*tasks)
来源：http://ya.lnxyls.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://rv.colortex.cn

JS:   await Promise.all(tasks)
来源：http://sm.gzmigu.cn

TS:   await Promise.all(tasks)
来源：http://tx.asd995.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hn.huixinmuqiang.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://jb.yuntaijiaju.cn

Ruby: threads.map(&:join)
来源：http://sy.colortex.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://kw.haigaiapp.cn

[O06] 使用进程池
来源：http://ta.hnjuh.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://gc.chemitech.net.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://fs.hahajie.cn

JS:   // child_process / cluster 模块
来源：http://lj.yuntaijiaju.cn

TS:   // child_process / cluster 模块
来源：http://xo.yuntaijiaju.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://dp.asd995.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ua.yuntaijiaju.cn

Ruby: // fork 块
来源：http://ot.bookmarksfly.cn

C#:   Parallel.For
来源：http://ra.szxytkj.cn

================================================================================
来源：http://ae.shtwfgs.cn

P. 常用工具函数
来源：http://qg.521024.cn

================================================================================
来源：http://cx.bookmarksfly.cn

[P01] 生成 UUID
来源：http://jd.hnjuh.cn

Py:   str(uuid.uuid4())
来源：http://rd.haigaiapp.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://bg.bookmarksfly.cn

JS:   crypto.randomUUID()
来源：http://lr.wgjwhj.cn

TS:   crypto.randomUUID()
来源：http://uj.asd995.cn

Java: UUID.randomUUID().toString()
来源：http://rp.huixiangedu.cn

Go:   // 用 github.com/google/uuid
来源：http://yo.haigaiapp.cn

Ruby: SecureRandom.uuid
来源：http://rw.wgjwhj.cn

C#:   Guid.NewGuid().ToString()
来源：http://zb.huixiangedu.cn

[P02] MD5 / SHA256 摘要
来源：http://mu.jctech888.com.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://dl.szxytkj.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://kq.newstarts.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://gt.lnxyls.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://lt.muxihuayi.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://dx.wgjwhj.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://fw.shxzukj.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://lt.szxytkj.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://te.colortex.cn

[P03] 生成短随机字符串
来源：http://sr.colortex.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://gt.nicolike.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://nn.jianghongdianzi.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zl.newstarts.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ks.jianghongdianzi.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://pf.szsharing.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ma.huanxung.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://el.newstarts.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://xc.9csxet.cn

[P04] 求长度
来源：http://ll.yuexingan06.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://gl.chemitech.net.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fl.asd995.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hg.newstarts.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rc.nszjky.cn

Java: list.size();  map.size();  s.length()
来源：http://uu.panjiajie.cn

Go:   len(arr);  len(m)
来源：http://zh.shtwfgs.cn

Ruby: x.length;  x.size
来源：http://yi.hahajie.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://sn.huanxung.cn

[P05] 判断两个对象内容是否相等
来源：http://kq.wgjwhj.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ad.panjiajie.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wn.szsharing.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ni.shtwfgs.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://um.asd995.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://rq.wgjwhj.cn

Go:   reflect.DeepEqual(a, b)
来源：http://br.szsharing.cn

Ruby: a == b
来源：http://go.wgjwhj.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://rb.muxihuayi.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wz.bookmarksfly.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://gc.huanxung.cn

PHP:  if (empty($x)) {}
来源：http://cm.asd995.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://qp.bjjhwx.cn

TS:   if (x == null) {}
来源：http://rr.szxytkj.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://bc.shxzskj.cn

Go:   if x == nil {}
来源：http://zu.panjiajie.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://lg.lnxyls.cn

C#:   if (x is null) {}
来源：http://ff.shxzskj.cn

[P07] 防抖与节流
来源：http://yx.asd995.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://oc.9csxet.cn

PHP:  // 手写时间戳比较
来源：http://dy.muxihuayi.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sq.muxihuayi.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ug.bookmarksfly.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://el.shxzskj.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://px.asd995.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://cf.huanxung.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://kc.muxihuayi.cn

[P08] 处理浮点精度问题
来源：http://zo.asd995.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://rg.haigaiapp.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hi.wgjwhj.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wx.newstarts.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://qw.newstarts.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ru.nicolike.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://dp.colortex.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ee.panjiajie.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wa.bjjhwx.cn

================================================================================
来源：http://it.jianghongdianzi.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hh.chemitech.net.cn

================================================================================
来源：http://nk.haigaiapp.cn

[Q01] 创建表
来源：http://wg.hnjuh.cn

CREATE TABLE users (
来源：http://ea.bjjhwx.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://zb.shxzukj.cn

name VARCHAR(50) NOT NULL,
来源：http://kj.shtwfgs.cn

email VARCHAR(100) UNIQUE,
来源：http://qh.colortex.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://me.huixinmuqiang.cn

);
来源：http://rf.chemitech.net.cn

[Q02] 创建带外键的表
来源：http://yr.bjjhwx.cn

CREATE TABLE orders (
来源：http://jg.shxzskj.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ul.bjjhwx.cn

user_id INT NOT NULL,
来源：http://kn.jctech888.com.cn

amount DECIMAL(10, 2),
来源：http://xi.asd995.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://nb.hnjuh.cn

);
来源：http://xw.muxihuayi.cn

[Q03] 增加列
来源：http://mc.muxihuayi.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://sb.muxihuayi.cn

[Q04] 修改列类型
来源：http://ey.huanxung.cn


<!-- 参考信息 -->