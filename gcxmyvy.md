代发 wailian999

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://fk.panjiajie.cn

Ruby: warn "err"
来源：http://da.muxihuayi.cn

C#:   Console.Error.WriteLine("err")
来源：http://jx.9csxet.cn

[M07] 判断是否为主入口
来源：http://gv.shtwfgs.cn

Py:   if __name__ == "__main__":
来源：http://kb.521024.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wa.9csxet.cn

JS:   require.main === module
来源：http://dl.newstarts.cn

TS:   require.main === module
来源：http://xt.newstarts.cn

Java: public static void main(String[] args)
来源：http://zc.yuexingan06.cn

Go:   func main()
来源：http://ge.hnjuh.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hx.nszjky.cn

C#:   static void Main(string[] args)
来源：http://qd.huixiangedu.cn

[M08] 获取系统与运行时信息
来源：http://ah.muxihuayi.cn

Py:   platform.system();  platform.python_version()
来源：http://pn.haigaiapp.cn

PHP:  PHP_OS;  phpversion();
来源：http://ya.huanxung.cn

JS:   process.platform;  process.version
来源：http://sp.521024.cn

TS:   process.platform;  process.version
来源：http://xc.muxihuayi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wu.szxytkj.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://se.muxihuayi.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://el.nszjky.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ey.9csxet.cn

================================================================================
来源：http://mu.panjiajie.cn

N. 数据结构与算法
来源：http://mj.wgjwhj.cn

================================================================================
来源：http://fi.shtwfgs.cn

[N01] 二分查找（有序数组）
来源：http://jj.bjjhwx.cn

Py:   bisect.bisect_left(arr, x)
来源：http://gc.shxzukj.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://fv.yuntaijiaju.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fv.jctech888.com.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ys.muxihuayi.cn

Java: Arrays.binarySearch(arr, x)
来源：http://rw.yuntaijiaju.cn

Go:   sort.SearchInts(arr, x)
来源：http://wq.asd995.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://yd.yuexingan06.cn

C#:   Array.BinarySearch(arr, x)
来源：http://sd.chemitech.net.cn

[N02] 排序（工程实践用内置实现）
来源：http://ik.szxytkj.cn

Py:   sorted(arr);  arr.sort()
来源：http://mm.shxzskj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://pi.panjiajie.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://wi.lnxyls.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://zy.hahajie.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://qr.bjjhwx.cn

Go:   slices.Sort(arr)
来源：http://rc.shxzukj.cn

Ruby: arr.sort
来源：http://dh.bjjhwx.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://fe.wgjwhj.cn

[N03] 快速排序（分治示例）
来源：http://pi.bookmarksfly.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://nw.muxihuayi.cn

PHP:  // 递归实现，或用 usort
来源：http://wz.szxytkj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mv.521024.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.huanxung.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ew.wgjwhj.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://vp.hnjuh.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ob.muxihuayi.cn

C#:   // 手写递归，或 Array.Sort
来源：http://yd.lnxyls.cn

[N04] 斐波那契数列
来源：http://ee.jianghongdianzi.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://kc.hahajie.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://nl.jianghongdianzi.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rg.wgjwhj.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fn.chemitech.net.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ro.chemitech.net.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://si.yuexingan06.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ye.huixiangedu.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mf.bookmarksfly.cn

[N05] 最大公约数
来源：http://fd.521024.cn

Py:   math.gcd(a, b)
来源：http://mx.yuntaijiaju.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://dr.shtwfgs.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qb.bjjhwx.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gk.hahajie.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://nl.521024.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ub.nicolike.cn

Ruby: a.gcd(b)
来源：http://bj.bjjhwx.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://xm.shxzukj.cn

[N06] 判断回文字符串
来源：http://tf.hahajie.cn

Py:   s == s[::-1]
来源：http://sq.hahajie.cn

PHP:  $s === strrev($s);
来源：http://ri.nszjky.cn

JS:   s === [...s].reverse().join("")
来源：http://dc.gzmigu.cn

TS:   s === [...s].reverse().join("")
来源：http://ez.hahajie.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ye.szxytkj.cn

Go:   // 双指针从两端比较
来源：http://ka.haigaiapp.cn

Ruby: s == s.reverse
来源：http://kx.jianghongdianzi.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://kj.huixinmuqiang.cn

[N07] 两数之和（返回下标）
来源：http://qs.colortex.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://pk.panjiajie.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://yr.9csxet.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://iw.huanxung.cn

TS:   // 手写 Map<string, number>
来源：http://fc.szsharing.cn

Java: // 手写 HashMap
来源：http://ly.bookmarksfly.cn

Go:   // 手写 map[int]int
来源：http://qk.lnxyls.cn

Ruby: // 手写 Hash
来源：http://rj.newstarts.cn

C#:   // 手写 Dictionary<int, int>
来源：http://cm.wgjwhj.cn

[N08] 生成全排列
来源：http://pg.gzmigu.cn

Py:   itertools.permutations(arr)
来源：http://lx.haigaiapp.cn

PHP:  // 手写递归交换
来源：http://pn.asd995.cn

JS:   // 手写回溯递归
来源：http://kw.gzmigu.cn

TS:   // 手写回溯递归
来源：http://mg.hnjuh.cn

Java: // 手写回溯递归
来源：http://os.nicolike.cn

Go:   // 手写回溯递归
来源：http://nq.shtwfgs.cn

Ruby: arr.permutation.to_a
来源：http://tr.jianghongdianzi.cn

C#:   // 手写回溯递归
来源：http://yu.colortex.cn

[N09] 栈与队列
来源：http://jm.huanxung.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://tu.hnjuh.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://xy.newstarts.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mx.muxihuayi.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ic.chemitech.net.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://vh.chemitech.net.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://jb.jctech888.com.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ds.lnxyls.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://cb.bjjhwx.cn

[N10] 链表节点定义
来源：http://uv.jctech888.com.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://lb.haigaiapp.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://to.jianghongdianzi.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ca.shxzukj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://lq.nicolike.cn

Java: class Node { int v; Node next; }
来源：http://cn.shxzskj.cn

Go:   type Node struct { V int; Next *Node }
来源：http://jn.muxihuayi.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://fq.yuexingan06.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://sb.asd995.cn

[N11] 二叉树中序遍历
来源：http://ji.hahajie.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hy.jianghongdianzi.cn

PHP:  // 手写递归函数
来源：http://uk.panjiajie.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fw.9csxet.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jg.huixinmuqiang.cn

Java: // 手写递归
来源：http://gr.panjiajie.cn

Go:   // 手写递归
来源：http://ot.chemitech.net.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://xx.gzmigu.cn

C#:   // 手写递归
来源：http://tu.521024.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://lg.szxytkj.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ic.huanxung.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://cf.haigaiapp.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xj.9csxet.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ii.jctech888.com.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://by.jianghongdianzi.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://aj.nszjky.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://lr.panjiajie.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mm.shxzukj.cn

================================================================================
来源：http://sy.szsharing.cn

O. 并发与异步
来源：http://aj.hahajie.cn

================================================================================
来源：http://wb.bookmarksfly.cn

[O01] 启动一个线程
来源：http://nw.hnjuh.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ix.9csxet.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hs.jianghongdianzi.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://gj.yuexingan06.cn

TS:   // 同 JS
来源：http://mx.shxzskj.cn

Java: new Thread(() -> f()).start()
来源：http://cx.newstarts.cn

Go:   go f()
来源：http://fi.shxzskj.cn

Ruby: Thread.new { f }
来源：http://fa.yuexingan06.cn

C#:   Task.Run(() => F());
来源：http://qf.huixinmuqiang.cn

[O02] 使用线程池
来源：http://jr.chemitech.net.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://qb.nszjky.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ub.huixinmuqiang.cn

JS:   // worker_threads 线程池
来源：http://su.shtwfgs.cn

TS:   // worker_threads 线程池
来源：http://ot.muxihuayi.cn

Java: Executors.newFixedThreadPool(4)
来源：http://eo.huanxung.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ee.gzmigu.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://pb.shtwfgs.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://jp.shxzukj.cn

[O03] 加锁保护共享数据
来源：http://ea.huixiangedu.cn

Py:   with lock: shared += 1
来源：http://gr.wgjwhj.cn

PHP:  // 用 flock() 做文件锁
来源：http://rx.bookmarksfly.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wz.lnxyls.cn

TS:   // 同 JS
来源：http://pn.shxzskj.cn

Java: synchronized (this) { shared++; }
来源：http://gv.shxzukj.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ug.shtwfgs.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://dk.jianghongdianzi.cn

C#:   lock (gate) { shared++; }
来源：http://zb.huixiangedu.cn

[O04] 定义异步函数并等待
来源：http://xm.colortex.cn

Py:   async def f():⏎    await g()
来源：http://hu.lnxyls.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://gx.szsharing.cn

JS:   async function f() { await g(); }
来源：http://db.shxzukj.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ar.shtwfgs.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://zm.panjiajie.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ec.hahajie.cn

Ruby: # 用 Fiber 或 async gem
来源：http://su.jianghongdianzi.cn

C#:   async Task F() { await G(); }
来源：http://ct.lnxyls.cn

[O05] 并发执行并等待全部完成
来源：http://qz.chemitech.net.cn

Py:   asyncio.gather(*tasks)
来源：http://ke.hnjuh.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://sk.9csxet.cn

JS:   await Promise.all(tasks)
来源：http://xy.nszjky.cn

TS:   await Promise.all(tasks)
来源：http://rh.panjiajie.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://cg.nicolike.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://po.huanxung.cn

Ruby: threads.map(&:join)
来源：http://rv.shxzskj.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://sj.newstarts.cn

[O06] 使用进程池
来源：http://sk.bookmarksfly.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://bp.chemitech.net.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://jj.asd995.cn

JS:   // child_process / cluster 模块
来源：http://ph.haigaiapp.cn

TS:   // child_process / cluster 模块
来源：http://rs.521024.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wv.szsharing.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://lb.chemitech.net.cn

Ruby: // fork 块
来源：http://ai.hnjuh.cn

C#:   Parallel.For
来源：http://qy.shtwfgs.cn

================================================================================
来源：http://ub.9csxet.cn

P. 常用工具函数
来源：http://yr.lnxyls.cn

================================================================================
来源：http://pk.521024.cn

[P01] 生成 UUID
来源：http://tf.nszjky.cn

Py:   str(uuid.uuid4())
来源：http://wc.asd995.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://oo.szxytkj.cn

JS:   crypto.randomUUID()
来源：http://pu.haigaiapp.cn

TS:   crypto.randomUUID()
来源：http://nn.newstarts.cn

Java: UUID.randomUUID().toString()
来源：http://kx.chemitech.net.cn

Go:   // 用 github.com/google/uuid
来源：http://th.asd995.cn

Ruby: SecureRandom.uuid
来源：http://tk.yuntaijiaju.cn

C#:   Guid.NewGuid().ToString()
来源：http://ss.shxzskj.cn

[P02] MD5 / SHA256 摘要
来源：http://zw.szsharing.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://tu.szsharing.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://fu.chemitech.net.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://dn.521024.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://yv.huanxung.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ch.hnjuh.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://yw.asd995.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ae.521024.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://kj.shxzukj.cn

[P03] 生成短随机字符串
来源：http://ml.szxytkj.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ov.panjiajie.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://xi.shxzukj.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zr.yuntaijiaju.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hf.chemitech.net.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://nq.bookmarksfly.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://pn.hnjuh.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ri.jctech888.com.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ln.wgjwhj.cn

[P04] 求长度
来源：http://xd.huanxung.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://el.shxzukj.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://su.shxzskj.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://px.bjjhwx.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://od.9csxet.cn

Java: list.size();  map.size();  s.length()
来源：http://pt.shxzukj.cn

Go:   len(arr);  len(m)
来源：http://cb.panjiajie.cn

Ruby: x.length;  x.size
来源：http://mu.asd995.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://gs.bjjhwx.cn

[P05] 判断两个对象内容是否相等
来源：http://ep.chemitech.net.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://vn.shtwfgs.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://np.huanxung.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://xg.lnxyls.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://gg.wgjwhj.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ta.colortex.cn

Go:   reflect.DeepEqual(a, b)
来源：http://np.nicolike.cn

Ruby: a == b
来源：http://ar.jianghongdianzi.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://px.haigaiapp.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ra.wgjwhj.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://cw.huixiangedu.cn

PHP:  if (empty($x)) {}
来源：http://yv.gzmigu.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://gn.wgjwhj.cn

TS:   if (x == null) {}
来源：http://aw.asd995.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://iq.colortex.cn

Go:   if x == nil {}
来源：http://td.szxytkj.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://xz.521024.cn

C#:   if (x is null) {}
来源：http://tp.szxytkj.cn

[P07] 防抖与节流
来源：http://lq.muxihuayi.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hl.huixinmuqiang.cn

PHP:  // 手写时间戳比较
来源：http://ex.haigaiapp.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bd.panjiajie.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vj.shxzukj.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://tj.panjiajie.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://nu.szsharing.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://tp.jianghongdianzi.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ir.nszjky.cn

[P08] 处理浮点精度问题
来源：http://tz.shxzskj.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://iq.huanxung.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://vs.shtwfgs.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ab.bjjhwx.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://nm.huixinmuqiang.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://da.9csxet.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hl.gzmigu.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://yd.shxzukj.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://nf.nicolike.cn

================================================================================
来源：http://vn.lnxyls.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://zh.9csxet.cn

================================================================================
来源：http://wp.bookmarksfly.cn

[Q01] 创建表
来源：http://wg.jctech888.com.cn

CREATE TABLE users (
来源：http://jt.shxzskj.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://dt.hnjuh.cn

name VARCHAR(50) NOT NULL,
来源：http://ky.nicolike.cn

email VARCHAR(100) UNIQUE,
来源：http://yf.bookmarksfly.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://yo.yuntaijiaju.cn

);
来源：http://dl.wgjwhj.cn

[Q02] 创建带外键的表
来源：http://ku.huixiangedu.cn

CREATE TABLE orders (
来源：http://il.jctech888.com.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://fe.hnjuh.cn

user_id INT NOT NULL,
来源：http://yc.chemitech.net.cn

amount DECIMAL(10, 2),
来源：http://fm.gzmigu.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://rf.szsharing.cn

);
来源：http://qu.hnjuh.cn

[Q03] 增加列
来源：http://pq.yuntaijiaju.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://zm.shxzukj.cn

[Q04] 修改列类型
来源：http://sl.yuexingan06.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://kn.hnjuh.cn

[Q05] 重命名列
来源：http://at.9csxet.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://lk.muxihuayi.cn

[Q06] 删除列
来源：http://kt.shxzskj.cn

ALTER TABLE users DROP COLUMN age;
来源：http://rh.muxihuayi.cn

[Q07] 删除表
来源：http://tk.hnjuh.cn

DROP TABLE IF EXISTS orders;
来源：http://lb.jianghongdianzi.cn

[Q08] 创建普通索引
来源：http://la.haigaiapp.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://hg.bookmarksfly.cn

[Q09] 创建唯一索引
来源：http://mu.asd995.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://jb.shxzukj.cn

[Q10] 插入单行
来源：http://lx.shxzukj.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://vm.gzmigu.cn

[Q11] 一次插入多行
来源：http://si.szsharing.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://oq.szsharing.cn

[Q12] 插入后取自增 ID
来源：http://td.521024.cn


<!-- 参考信息 -->