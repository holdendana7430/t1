代发 wailian999

C#:   Directory.GetCurrentDirectory()
来源：http://mx.newstarts.cn

[M05] 设置退出码
来源：http://ai.haigaiapp.cn

Py:   sys.exit(1)
来源：http://xq.huanxung.cn

PHP:  exit(1);
来源：http://wg.newstarts.cn

JS:   process.exit(1)
来源：http://ol.wgjwhj.cn

TS:   process.exit(1)
来源：http://be.asd995.cn

Java: System.exit(1)
来源：http://xu.bookmarksfly.cn

Go:   os.Exit(1)
来源：http://aa.szsharing.cn

Ruby: exit 1
来源：http://am.shxzukj.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ff.nszjky.cn

[M06] 向标准错误输出
来源：http://tr.chemitech.net.cn

Py:   print("err", file=sys.stderr)
来源：http://hz.bjjhwx.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://en.gzmigu.cn

JS:   console.error("err")
来源：http://iy.nicolike.cn

TS:   console.error("err")
来源：http://xu.asd995.cn

Java: System.err.println("err")
来源：http://bh.jctech888.com.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://lk.huanxung.cn

Ruby: warn "err"
来源：http://jx.gzmigu.cn

C#:   Console.Error.WriteLine("err")
来源：http://px.bookmarksfly.cn

[M07] 判断是否为主入口
来源：http://sx.jctech888.com.cn

Py:   if __name__ == "__main__":
来源：http://sh.lnxyls.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://at.gzmigu.cn

JS:   require.main === module
来源：http://du.shxzskj.cn

TS:   require.main === module
来源：http://pu.hnjuh.cn

Java: public static void main(String[] args)
来源：http://hj.shtwfgs.cn

Go:   func main()
来源：http://uo.nszjky.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hg.haigaiapp.cn

C#:   static void Main(string[] args)
来源：http://hy.shxzukj.cn

[M08] 获取系统与运行时信息
来源：http://ox.huixiangedu.cn

Py:   platform.system();  platform.python_version()
来源：http://th.jctech888.com.cn

PHP:  PHP_OS;  phpversion();
来源：http://rx.panjiajie.cn

JS:   process.platform;  process.version
来源：http://st.jctech888.com.cn

TS:   process.platform;  process.version
来源：http://bu.wgjwhj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://io.shxzukj.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ts.hnjuh.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://xd.jianghongdianzi.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ng.yuntaijiaju.cn

================================================================================
来源：http://om.lnxyls.cn

N. 数据结构与算法
来源：http://rz.jctech888.com.cn

================================================================================
来源：http://bh.shxzukj.cn

[N01] 二分查找（有序数组）
来源：http://lf.haigaiapp.cn

Py:   bisect.bisect_left(arr, x)
来源：http://hx.shtwfgs.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://rr.shtwfgs.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://px.panjiajie.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ct.szxytkj.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ce.yuntaijiaju.cn

Go:   sort.SearchInts(arr, x)
来源：http://pi.bookmarksfly.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://mj.panjiajie.cn

C#:   Array.BinarySearch(arr, x)
来源：http://rr.shtwfgs.cn

[N02] 排序（工程实践用内置实现）
来源：http://pw.bookmarksfly.cn

Py:   sorted(arr);  arr.sort()
来源：http://qd.jctech888.com.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://tf.yuexingan06.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://dw.panjiajie.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ua.gzmigu.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://yr.gzmigu.cn

Go:   slices.Sort(arr)
来源：http://mh.bjjhwx.cn

Ruby: arr.sort
来源：http://uj.haigaiapp.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://gf.szsharing.cn

[N03] 快速排序（分治示例）
来源：http://hs.bookmarksfly.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://tv.9csxet.cn

PHP:  // 递归实现，或用 usort
来源：http://wr.shxzukj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jx.newstarts.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ip.gzmigu.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://zc.szsharing.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://er.gzmigu.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://lg.szxytkj.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ee.lnxyls.cn

[N04] 斐波那契数列
来源：http://wl.hahajie.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://gr.shtwfgs.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hw.bookmarksfly.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://uf.gzmigu.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gm.haigaiapp.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://om.huixinmuqiang.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mv.haigaiapp.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://do.szxytkj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://qr.chemitech.net.cn

[N05] 最大公约数
来源：http://sl.hnjuh.cn

Py:   math.gcd(a, b)
来源：http://hm.haigaiapp.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://xg.gzmigu.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://uq.yuexingan06.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fp.panjiajie.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://nf.asd995.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ez.asd995.cn

Ruby: a.gcd(b)
来源：http://zm.shxzukj.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://rf.huanxung.cn

[N06] 判断回文字符串
来源：http://pf.lnxyls.cn

Py:   s == s[::-1]
来源：http://kt.521024.cn

PHP:  $s === strrev($s);
来源：http://yr.wgjwhj.cn

JS:   s === [...s].reverse().join("")
来源：http://ap.lnxyls.cn

TS:   s === [...s].reverse().join("")
来源：http://ko.huixinmuqiang.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://jb.szxytkj.cn

Go:   // 双指针从两端比较
来源：http://ro.panjiajie.cn

Ruby: s == s.reverse
来源：http://si.bjjhwx.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ym.szsharing.cn

[N07] 两数之和（返回下标）
来源：http://bw.wgjwhj.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ju.hnjuh.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://lk.gzmigu.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ap.huixinmuqiang.cn

TS:   // 手写 Map<string, number>
来源：http://kz.hnjuh.cn

Java: // 手写 HashMap
来源：http://fi.nicolike.cn

Go:   // 手写 map[int]int
来源：http://js.521024.cn

Ruby: // 手写 Hash
来源：http://qv.gzmigu.cn

C#:   // 手写 Dictionary<int, int>
来源：http://zm.521024.cn

[N08] 生成全排列
来源：http://ny.asd995.cn

Py:   itertools.permutations(arr)
来源：http://ol.huanxung.cn

PHP:  // 手写递归交换
来源：http://pj.muxihuayi.cn

JS:   // 手写回溯递归
来源：http://hu.hahajie.cn

TS:   // 手写回溯递归
来源：http://an.chemitech.net.cn

Java: // 手写回溯递归
来源：http://nf.hnjuh.cn

Go:   // 手写回溯递归
来源：http://ud.newstarts.cn

Ruby: arr.permutation.to_a
来源：http://pe.newstarts.cn

C#:   // 手写回溯递归
来源：http://lu.asd995.cn

[N09] 栈与队列
来源：http://zg.chemitech.net.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://me.asd995.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://pu.521024.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mj.colortex.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ri.szxytkj.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://xv.bookmarksfly.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://uk.yuexingan06.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://uf.nszjky.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://cy.hahajie.cn

[N10] 链表节点定义
来源：http://bp.szxytkj.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://il.bjjhwx.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ha.muxihuayi.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://fv.colortex.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://rs.wgjwhj.cn

Java: class Node { int v; Node next; }
来源：http://lt.szxytkj.cn

Go:   type Node struct { V int; Next *Node }
来源：http://or.bjjhwx.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://wz.shxzukj.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://xd.yuexingan06.cn

[N11] 二叉树中序遍历
来源：http://pr.haigaiapp.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://qa.colortex.cn

PHP:  // 手写递归函数
来源：http://te.9csxet.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bg.asd995.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dg.bookmarksfly.cn

Java: // 手写递归
来源：http://yg.bjjhwx.cn

Go:   // 手写递归
来源：http://xw.nicolike.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://jt.jianghongdianzi.cn

C#:   // 手写递归
来源：http://xd.hahajie.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hr.jctech888.com.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://dk.haigaiapp.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://fo.huixinmuqiang.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hy.chemitech.net.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wx.jctech888.com.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://qf.szsharing.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://rr.szxytkj.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://fs.hnjuh.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://zd.bjjhwx.cn

================================================================================
来源：http://kc.huixiangedu.cn

O. 并发与异步
来源：http://xl.newstarts.cn

================================================================================
来源：http://bj.lnxyls.cn

[O01] 启动一个线程
来源：http://mq.szxytkj.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://qm.colortex.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ya.nszjky.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ub.hahajie.cn

TS:   // 同 JS
来源：http://ty.szxytkj.cn

Java: new Thread(() -> f()).start()
来源：http://jo.shxzukj.cn

Go:   go f()
来源：http://yh.szxytkj.cn

Ruby: Thread.new { f }
来源：http://dk.shxzskj.cn

C#:   Task.Run(() => F());
来源：http://nk.haigaiapp.cn

[O02] 使用线程池
来源：http://us.shtwfgs.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://gu.asd995.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://fg.nicolike.cn

JS:   // worker_threads 线程池
来源：http://ls.gzmigu.cn

TS:   // worker_threads 线程池
来源：http://jx.szsharing.cn

Java: Executors.newFixedThreadPool(4)
来源：http://hp.hnjuh.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://fp.huanxung.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ic.nszjky.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://of.shxzskj.cn

[O03] 加锁保护共享数据
来源：http://dj.yuexingan06.cn

Py:   with lock: shared += 1
来源：http://hb.shtwfgs.cn

PHP:  // 用 flock() 做文件锁
来源：http://ue.gzmigu.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://pw.panjiajie.cn

TS:   // 同 JS
来源：http://fe.shxzskj.cn

Java: synchronized (this) { shared++; }
来源：http://of.gzmigu.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://le.asd995.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://zb.wgjwhj.cn

C#:   lock (gate) { shared++; }
来源：http://xb.chemitech.net.cn

[O04] 定义异步函数并等待
来源：http://yv.asd995.cn

Py:   async def f():⏎    await g()
来源：http://iy.hahajie.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://dm.521024.cn

JS:   async function f() { await g(); }
来源：http://eo.huanxung.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://tz.9csxet.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://qe.yuexingan06.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://cb.colortex.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ya.chemitech.net.cn

C#:   async Task F() { await G(); }
来源：http://bc.yuntaijiaju.cn

[O05] 并发执行并等待全部完成
来源：http://of.huixiangedu.cn

Py:   asyncio.gather(*tasks)
来源：http://ca.haigaiapp.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://pz.yuntaijiaju.cn

JS:   await Promise.all(tasks)
来源：http://od.haigaiapp.cn

TS:   await Promise.all(tasks)
来源：http://qu.newstarts.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hm.yuexingan06.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://yu.haigaiapp.cn

Ruby: threads.map(&:join)
来源：http://la.shtwfgs.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ra.newstarts.cn

[O06] 使用进程池
来源：http://uo.lnxyls.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://vj.hahajie.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://fa.hnjuh.cn

JS:   // child_process / cluster 模块
来源：http://xv.jianghongdianzi.cn

TS:   // child_process / cluster 模块
来源：http://nw.hahajie.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ec.asd995.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://bm.wgjwhj.cn

Ruby: // fork 块
来源：http://xh.nicolike.cn

C#:   Parallel.For
来源：http://my.haigaiapp.cn

================================================================================
来源：http://vo.jianghongdianzi.cn

P. 常用工具函数
来源：http://iw.szxytkj.cn

================================================================================
来源：http://cz.jctech888.com.cn

[P01] 生成 UUID
来源：http://cl.huixinmuqiang.cn

Py:   str(uuid.uuid4())
来源：http://ls.muxihuayi.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://uc.shtwfgs.cn

JS:   crypto.randomUUID()
来源：http://sa.wgjwhj.cn

TS:   crypto.randomUUID()
来源：http://iy.newstarts.cn

Java: UUID.randomUUID().toString()
来源：http://xh.muxihuayi.cn

Go:   // 用 github.com/google/uuid
来源：http://gl.hnjuh.cn

Ruby: SecureRandom.uuid
来源：http://he.gzmigu.cn

C#:   Guid.NewGuid().ToString()
来源：http://zc.shxzskj.cn

[P02] MD5 / SHA256 摘要
来源：http://eq.muxihuayi.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mh.nszjky.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://be.nicolike.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://pp.521024.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://dx.colortex.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ut.shxzukj.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://qd.shxzskj.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://bq.bookmarksfly.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://sx.yuntaijiaju.cn

[P03] 生成短随机字符串
来源：http://dy.huixinmuqiang.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://tz.shxzskj.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://qv.hnjuh.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ew.nicolike.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wd.shtwfgs.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://uu.chemitech.net.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://sr.yuexingan06.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://qt.newstarts.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://lb.yuexingan06.cn

[P04] 求长度
来源：http://it.panjiajie.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ye.asd995.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vj.yuntaijiaju.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mj.jianghongdianzi.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://px.shxzukj.cn

Java: list.size();  map.size();  s.length()
来源：http://dg.521024.cn

Go:   len(arr);  len(m)
来源：http://rq.hnjuh.cn

Ruby: x.length;  x.size
来源：http://zh.panjiajie.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://nc.yuexingan06.cn

[P05] 判断两个对象内容是否相等
来源：http://rr.jianghongdianzi.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://vx.9csxet.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://zs.9csxet.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://pu.szsharing.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ww.521024.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://zi.panjiajie.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ra.szxytkj.cn

Ruby: a == b
来源：http://cu.huixinmuqiang.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://kv.haigaiapp.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://bc.shxzukj.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://uo.jctech888.com.cn

PHP:  if (empty($x)) {}
来源：http://tu.hahajie.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://vi.hahajie.cn

TS:   if (x == null) {}
来源：http://vp.newstarts.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://da.521024.cn

Go:   if x == nil {}
来源：http://pi.shtwfgs.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ak.gzmigu.cn

C#:   if (x is null) {}
来源：http://ms.jianghongdianzi.cn

[P07] 防抖与节流
来源：http://kp.asd995.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ab.colortex.cn

PHP:  // 手写时间戳比较
来源：http://oo.szxytkj.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sk.panjiajie.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vv.bookmarksfly.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ae.huanxung.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://el.bjjhwx.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://uk.asd995.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://yl.panjiajie.cn

[P08] 处理浮点精度问题
来源：http://cc.huanxung.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://bt.yuexingan06.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ta.hnjuh.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ek.lnxyls.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://xt.bookmarksfly.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://pf.szsharing.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://yp.jianghongdianzi.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wz.bookmarksfly.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://zw.521024.cn

================================================================================
来源：http://vs.hnjuh.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://op.szxytkj.cn

================================================================================
来源：http://rr.nicolike.cn

[Q01] 创建表
来源：http://gs.asd995.cn

CREATE TABLE users (
来源：http://qy.bookmarksfly.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://bu.szsharing.cn

name VARCHAR(50) NOT NULL,
来源：http://wq.jianghongdianzi.cn

email VARCHAR(100) UNIQUE,
来源：http://of.gzmigu.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://jh.gzmigu.cn

);
来源：http://nd.jianghongdianzi.cn

[Q02] 创建带外键的表
来源：http://jk.huanxung.cn

CREATE TABLE orders (
来源：http://db.chemitech.net.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://kg.hnjuh.cn

user_id INT NOT NULL,
来源：http://hu.shtwfgs.cn

amount DECIMAL(10, 2),
来源：http://lq.jianghongdianzi.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ob.shtwfgs.cn

);
来源：http://rl.huixinmuqiang.cn

[Q03] 增加列
来源：http://cf.muxihuayi.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wr.huixiangedu.cn

[Q04] 修改列类型
来源：http://en.521024.cn


<!-- 参考信息 -->