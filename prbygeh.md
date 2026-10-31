代发 wailian999

Ruby: exit 1
来源：http://jo.huixinmuqiang.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://er.szxytkj.cn

[M06] 向标准错误输出
来源：http://hd.colortex.cn

Py:   print("err", file=sys.stderr)
来源：http://pu.nszjky.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://gj.newstarts.cn

JS:   console.error("err")
来源：http://zw.yuexingan06.cn

TS:   console.error("err")
来源：http://vg.jianghongdianzi.cn

Java: System.err.println("err")
来源：http://xg.bjjhwx.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ei.shxzukj.cn

Ruby: warn "err"
来源：http://gi.bookmarksfly.cn

C#:   Console.Error.WriteLine("err")
来源：http://vq.521024.cn

[M07] 判断是否为主入口
来源：http://ko.newstarts.cn

Py:   if __name__ == "__main__":
来源：http://re.shxzskj.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://nf.chemitech.net.cn

JS:   require.main === module
来源：http://qf.shxzukj.cn

TS:   require.main === module
来源：http://hm.haigaiapp.cn

Java: public static void main(String[] args)
来源：http://mt.hahajie.cn

Go:   func main()
来源：http://ql.lnxyls.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://we.asd995.cn

C#:   static void Main(string[] args)
来源：http://ry.bjjhwx.cn

[M08] 获取系统与运行时信息
来源：http://wo.asd995.cn

Py:   platform.system();  platform.python_version()
来源：http://pb.haigaiapp.cn

PHP:  PHP_OS;  phpversion();
来源：http://eu.panjiajie.cn

JS:   process.platform;  process.version
来源：http://ea.shtwfgs.cn

TS:   process.platform;  process.version
来源：http://sn.9csxet.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ie.nszjky.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://sa.lnxyls.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wh.newstarts.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://uk.yuntaijiaju.cn

================================================================================
来源：http://bq.shxzskj.cn

N. 数据结构与算法
来源：http://lh.shxzskj.cn

================================================================================
来源：http://fp.hahajie.cn

[N01] 二分查找（有序数组）
来源：http://ka.gzmigu.cn

Py:   bisect.bisect_left(arr, x)
来源：http://xk.huixinmuqiang.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://js.jctech888.com.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xi.szsharing.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ae.newstarts.cn

Java: Arrays.binarySearch(arr, x)
来源：http://jg.szsharing.cn

Go:   sort.SearchInts(arr, x)
来源：http://ts.huixinmuqiang.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://hu.nicolike.cn

C#:   Array.BinarySearch(arr, x)
来源：http://rb.colortex.cn

[N02] 排序（工程实践用内置实现）
来源：http://cn.chemitech.net.cn

Py:   sorted(arr);  arr.sort()
来源：http://sz.yuexingan06.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://yk.colortex.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://xb.9csxet.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://hf.szsharing.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ex.jianghongdianzi.cn

Go:   slices.Sort(arr)
来源：http://aw.bjjhwx.cn

Ruby: arr.sort
来源：http://lz.asd995.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://we.shxzukj.cn

[N03] 快速排序（分治示例）
来源：http://nx.521024.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://qm.colortex.cn

PHP:  // 递归实现，或用 usort
来源：http://oj.asd995.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://oh.newstarts.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ch.nszjky.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ql.nicolike.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://pi.haigaiapp.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://zs.huixinmuqiang.cn

C#:   // 手写递归，或 Array.Sort
来源：http://hq.bjjhwx.cn

[N04] 斐波那契数列
来源：http://xa.szsharing.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zt.jianghongdianzi.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://gs.nicolike.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fw.chemitech.net.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ba.haigaiapp.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://vg.521024.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://lg.wgjwhj.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://tg.colortex.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://vq.hahajie.cn

[N05] 最大公约数
来源：http://ik.wgjwhj.cn

Py:   math.gcd(a, b)
来源：http://ar.lnxyls.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://dd.521024.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ua.szxytkj.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tu.lnxyls.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://bb.nicolike.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://qq.gzmigu.cn

Ruby: a.gcd(b)
来源：http://un.muxihuayi.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://oh.bookmarksfly.cn

[N06] 判断回文字符串
来源：http://oq.9csxet.cn

Py:   s == s[::-1]
来源：http://dr.huixiangedu.cn

PHP:  $s === strrev($s);
来源：http://pb.9csxet.cn

JS:   s === [...s].reverse().join("")
来源：http://qn.bookmarksfly.cn

TS:   s === [...s].reverse().join("")
来源：http://fc.nicolike.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mh.bjjhwx.cn

Go:   // 双指针从两端比较
来源：http://ck.bookmarksfly.cn

Ruby: s == s.reverse
来源：http://mm.newstarts.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://uv.521024.cn

[N07] 两数之和（返回下标）
来源：http://xx.chemitech.net.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://lp.yuexingan06.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://sl.jianghongdianzi.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://uw.newstarts.cn

TS:   // 手写 Map<string, number>
来源：http://dq.9csxet.cn

Java: // 手写 HashMap
来源：http://ax.muxihuayi.cn

Go:   // 手写 map[int]int
来源：http://kx.521024.cn

Ruby: // 手写 Hash
来源：http://qm.nszjky.cn

C#:   // 手写 Dictionary<int, int>
来源：http://km.chemitech.net.cn

[N08] 生成全排列
来源：http://hq.nszjky.cn

Py:   itertools.permutations(arr)
来源：http://gs.huixinmuqiang.cn

PHP:  // 手写递归交换
来源：http://kn.nicolike.cn

JS:   // 手写回溯递归
来源：http://fb.szsharing.cn

TS:   // 手写回溯递归
来源：http://pw.shtwfgs.cn

Java: // 手写回溯递归
来源：http://qj.shxzukj.cn

Go:   // 手写回溯递归
来源：http://ag.wgjwhj.cn

Ruby: arr.permutation.to_a
来源：http://xp.asd995.cn

C#:   // 手写回溯递归
来源：http://ov.lnxyls.cn

[N09] 栈与队列
来源：http://gy.gzmigu.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://es.haigaiapp.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://gj.hnjuh.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://bt.szxytkj.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://qj.521024.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://et.szsharing.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://go.haigaiapp.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://xx.huixiangedu.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://zt.muxihuayi.cn

[N10] 链表节点定义
来源：http://be.jctech888.com.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://sh.shtwfgs.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ea.gzmigu.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://uk.muxihuayi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ob.colortex.cn

Java: class Node { int v; Node next; }
来源：http://ny.9csxet.cn

Go:   type Node struct { V int; Next *Node }
来源：http://no.huixinmuqiang.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://tt.muxihuayi.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://dv.shtwfgs.cn

[N11] 二叉树中序遍历
来源：http://sa.huanxung.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://he.jianghongdianzi.cn

PHP:  // 手写递归函数
来源：http://ir.jctech888.com.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dc.huixiangedu.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ce.yuexingan06.cn

Java: // 手写递归
来源：http://bl.szsharing.cn

Go:   // 手写递归
来源：http://rf.jctech888.com.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://aj.shxzukj.cn

C#:   // 手写递归
来源：http://qx.muxihuayi.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://id.panjiajie.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://da.haigaiapp.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://kx.bjjhwx.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ib.huixiangedu.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bv.bjjhwx.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wz.yuntaijiaju.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://yc.szsharing.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://lg.shxzukj.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ga.szsharing.cn

================================================================================
来源：http://gx.shxzskj.cn

O. 并发与异步
来源：http://ds.nicolike.cn

================================================================================
来源：http://tr.chemitech.net.cn

[O01] 启动一个线程
来源：http://ax.gzmigu.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://cd.lnxyls.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://eu.szxytkj.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://es.szsharing.cn

TS:   // 同 JS
来源：http://gu.muxihuayi.cn

Java: new Thread(() -> f()).start()
来源：http://uc.shtwfgs.cn

Go:   go f()
来源：http://ix.haigaiapp.cn

Ruby: Thread.new { f }
来源：http://pp.asd995.cn

C#:   Task.Run(() => F());
来源：http://gb.huixinmuqiang.cn

[O02] 使用线程池
来源：http://gv.wgjwhj.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://kf.shtwfgs.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://dh.nicolike.cn

JS:   // worker_threads 线程池
来源：http://ze.chemitech.net.cn

TS:   // worker_threads 线程池
来源：http://tq.gzmigu.cn

Java: Executors.newFixedThreadPool(4)
来源：http://tm.chemitech.net.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ch.shxzukj.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://iy.shtwfgs.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ox.hahajie.cn

[O03] 加锁保护共享数据
来源：http://er.shxzskj.cn

Py:   with lock: shared += 1
来源：http://rz.bjjhwx.cn

PHP:  // 用 flock() 做文件锁
来源：http://lt.nicolike.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://gu.bjjhwx.cn

TS:   // 同 JS
来源：http://hf.jianghongdianzi.cn

Java: synchronized (this) { shared++; }
来源：http://je.9csxet.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ih.nicolike.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://zy.panjiajie.cn

C#:   lock (gate) { shared++; }
来源：http://pv.shtwfgs.cn

[O04] 定义异步函数并等待
来源：http://hx.chemitech.net.cn

Py:   async def f():⏎    await g()
来源：http://ra.wgjwhj.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wg.bookmarksfly.cn

JS:   async function f() { await g(); }
来源：http://ts.szxytkj.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ks.bookmarksfly.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ye.jctech888.com.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://tr.yuntaijiaju.cn

Ruby: # 用 Fiber 或 async gem
来源：http://rh.nszjky.cn

C#:   async Task F() { await G(); }
来源：http://im.yuntaijiaju.cn

[O05] 并发执行并等待全部完成
来源：http://lw.szxytkj.cn

Py:   asyncio.gather(*tasks)
来源：http://kf.shtwfgs.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://uw.nicolike.cn

JS:   await Promise.all(tasks)
来源：http://ko.huanxung.cn

TS:   await Promise.all(tasks)
来源：http://wh.chemitech.net.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mx.bjjhwx.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://xe.shxzukj.cn

Ruby: threads.map(&:join)
来源：http://gn.jianghongdianzi.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://en.shtwfgs.cn

[O06] 使用进程池
来源：http://eu.szxytkj.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://li.jctech888.com.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ag.hahajie.cn

JS:   // child_process / cluster 模块
来源：http://xg.gzmigu.cn

TS:   // child_process / cluster 模块
来源：http://tx.lnxyls.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://df.panjiajie.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ov.colortex.cn

Ruby: // fork 块
来源：http://iv.huixiangedu.cn

C#:   Parallel.For
来源：http://yd.panjiajie.cn

================================================================================
来源：http://qy.shxzskj.cn

P. 常用工具函数
来源：http://lh.bjjhwx.cn

================================================================================
来源：http://sy.bookmarksfly.cn

[P01] 生成 UUID
来源：http://pu.nicolike.cn

Py:   str(uuid.uuid4())
来源：http://di.9csxet.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.nszjky.cn

JS:   crypto.randomUUID()
来源：http://qf.yuexingan06.cn

TS:   crypto.randomUUID()
来源：http://lr.shxzukj.cn

Java: UUID.randomUUID().toString()
来源：http://my.nszjky.cn

Go:   // 用 github.com/google/uuid
来源：http://dd.9csxet.cn

Ruby: SecureRandom.uuid
来源：http://xm.yuexingan06.cn

C#:   Guid.NewGuid().ToString()
来源：http://fi.nicolike.cn

[P02] MD5 / SHA256 摘要
来源：http://ms.gzmigu.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://aw.asd995.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://jd.colortex.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://xp.nicolike.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ti.wgjwhj.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://fm.newstarts.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://kx.nicolike.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://yu.newstarts.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://iw.hahajie.cn

[P03] 生成短随机字符串
来源：http://qb.shtwfgs.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://yj.yuntaijiaju.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://oe.newstarts.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vd.haigaiapp.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rq.huanxung.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://rz.szxytkj.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wb.521024.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://gf.szsharing.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://uh.muxihuayi.cn

[P04] 求长度
来源：http://ov.shxzukj.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://yy.panjiajie.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://oe.muxihuayi.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qh.nszjky.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xp.chemitech.net.cn

Java: list.size();  map.size();  s.length()
来源：http://kh.huixiangedu.cn

Go:   len(arr);  len(m)
来源：http://mh.jctech888.com.cn

Ruby: x.length;  x.size
来源：http://dd.huixiangedu.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://pn.nszjky.cn

[P05] 判断两个对象内容是否相等
来源：http://bl.huixiangedu.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://re.shtwfgs.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://pz.521024.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://zf.shxzukj.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://bw.panjiajie.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://oa.lnxyls.cn

Go:   reflect.DeepEqual(a, b)
来源：http://kl.jctech888.com.cn

Ruby: a == b
来源：http://ss.nszjky.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ih.hahajie.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://rx.asd995.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://nc.haigaiapp.cn

PHP:  if (empty($x)) {}
来源：http://xe.wgjwhj.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://rh.muxihuayi.cn

TS:   if (x == null) {}
来源：http://xh.huixiangedu.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://yl.szxytkj.cn

Go:   if x == nil {}
来源：http://kj.wgjwhj.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://eu.szxytkj.cn

C#:   if (x is null) {}
来源：http://tt.chemitech.net.cn

[P07] 防抖与节流
来源：http://bq.huixinmuqiang.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wz.bjjhwx.cn

PHP:  // 手写时间戳比较
来源：http://yk.chemitech.net.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rc.szsharing.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://oa.hnjuh.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://kt.panjiajie.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://xd.jctech888.com.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ek.hahajie.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://cq.jianghongdianzi.cn

[P08] 处理浮点精度问题
来源：http://ob.huanxung.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://xd.nicolike.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://uu.szsharing.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://nh.bjjhwx.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ud.panjiajie.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://uw.yuntaijiaju.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://pd.jctech888.com.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://sq.jctech888.com.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://sq.colortex.cn

================================================================================
来源：http://mv.nszjky.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ft.9csxet.cn

================================================================================
来源：http://lt.haigaiapp.cn

[Q01] 创建表
来源：http://mj.yuntaijiaju.cn

CREATE TABLE users (
来源：http://zk.jianghongdianzi.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://dp.hahajie.cn

name VARCHAR(50) NOT NULL,
来源：http://li.yuntaijiaju.cn

email VARCHAR(100) UNIQUE,
来源：http://ig.9csxet.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hm.jianghongdianzi.cn

);
来源：http://jp.jianghongdianzi.cn

[Q02] 创建带外键的表
来源：http://mh.hahajie.cn

CREATE TABLE orders (
来源：http://qh.huixinmuqiang.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://rk.asd995.cn

user_id INT NOT NULL,
来源：http://ot.yuexingan06.cn

amount DECIMAL(10, 2),
来源：http://pa.521024.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ds.lnxyls.cn

);
来源：http://ut.jianghongdianzi.cn

[Q03] 增加列
来源：http://ed.521024.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://qj.muxihuayi.cn

[Q04] 修改列类型
来源：http://op.huanxung.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://oq.jctech888.com.cn

[Q05] 重命名列
来源：http://mq.haigaiapp.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://bb.chemitech.net.cn

[Q06] 删除列
来源：http://mj.9csxet.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ji.nicolike.cn

[Q07] 删除表
来源：http://xf.nicolike.cn

DROP TABLE IF EXISTS orders;
来源：http://rv.nicolike.cn

[Q08] 创建普通索引
来源：http://dn.nszjky.cn


<!-- 参考信息 -->