代发 wailian999

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ia.wgjwhj.cn

Ruby: warn "err"
来源：http://jb.shtwfgs.cn

C#:   Console.Error.WriteLine("err")
来源：http://xq.shxzskj.cn

[M07] 判断是否为主入口
来源：http://sh.shxzskj.cn

Py:   if __name__ == "__main__":
来源：http://jv.9csxet.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://qk.521024.cn

JS:   require.main === module
来源：http://po.jctech888.com.cn

TS:   require.main === module
来源：http://jq.szsharing.cn

Java: public static void main(String[] args)
来源：http://lk.9csxet.cn

Go:   func main()
来源：http://rn.shtwfgs.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://yw.huixinmuqiang.cn

C#:   static void Main(string[] args)
来源：http://im.huanxung.cn

[M08] 获取系统与运行时信息
来源：http://mu.chemitech.net.cn

Py:   platform.system();  platform.python_version()
来源：http://nr.chemitech.net.cn

PHP:  PHP_OS;  phpversion();
来源：http://zc.hnjuh.cn

JS:   process.platform;  process.version
来源：http://lz.bookmarksfly.cn

TS:   process.platform;  process.version
来源：http://qg.9csxet.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ls.wgjwhj.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://fw.9csxet.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ca.hahajie.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://qc.521024.cn

================================================================================
来源：http://as.jianghongdianzi.cn

N. 数据结构与算法
来源：http://zs.hnjuh.cn

================================================================================
来源：http://ac.lnxyls.cn

[N01] 二分查找（有序数组）
来源：http://lf.chemitech.net.cn

Py:   bisect.bisect_left(arr, x)
来源：http://le.huanxung.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://vf.muxihuayi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ej.9csxet.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vg.shxzukj.cn

Java: Arrays.binarySearch(arr, x)
来源：http://nl.chemitech.net.cn

Go:   sort.SearchInts(arr, x)
来源：http://it.hnjuh.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://jz.bookmarksfly.cn

C#:   Array.BinarySearch(arr, x)
来源：http://jt.nszjky.cn

[N02] 排序（工程实践用内置实现）
来源：http://tq.9csxet.cn

Py:   sorted(arr);  arr.sort()
来源：http://rn.szsharing.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://tk.nicolike.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://zr.yuntaijiaju.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://kr.chemitech.net.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://pl.nicolike.cn

Go:   slices.Sort(arr)
来源：http://vu.szxytkj.cn

Ruby: arr.sort
来源：http://dr.wgjwhj.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://rp.wgjwhj.cn

[N03] 快速排序（分治示例）
来源：http://li.chemitech.net.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://bt.shxzskj.cn

PHP:  // 递归实现，或用 usort
来源：http://xf.shxzukj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pk.9csxet.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qg.muxihuayi.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ws.9csxet.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://bq.panjiajie.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ez.wgjwhj.cn

C#:   // 手写递归，或 Array.Sort
来源：http://kk.hahajie.cn

[N04] 斐波那契数列
来源：http://by.muxihuayi.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://om.haigaiapp.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ks.haigaiapp.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://da.nszjky.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sk.yuexingan06.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://qn.colortex.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ss.nszjky.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://cv.szxytkj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://gj.hnjuh.cn

[N05] 最大公约数
来源：http://tz.nicolike.cn

Py:   math.gcd(a, b)
来源：http://sd.nicolike.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://lv.shtwfgs.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lq.9csxet.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ad.lnxyls.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ze.lnxyls.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://jz.szsharing.cn

Ruby: a.gcd(b)
来源：http://nx.shxzskj.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://qs.szsharing.cn

[N06] 判断回文字符串
来源：http://wo.colortex.cn

Py:   s == s[::-1]
来源：http://rs.panjiajie.cn

PHP:  $s === strrev($s);
来源：http://xb.newstarts.cn

JS:   s === [...s].reverse().join("")
来源：http://nc.jianghongdianzi.cn

TS:   s === [...s].reverse().join("")
来源：http://xu.chemitech.net.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wi.wgjwhj.cn

Go:   // 双指针从两端比较
来源：http://qj.nicolike.cn

Ruby: s == s.reverse
来源：http://va.nszjky.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://um.huixiangedu.cn

[N07] 两数之和（返回下标）
来源：http://bx.yuntaijiaju.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://di.yuntaijiaju.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ok.wgjwhj.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://al.yuexingan06.cn

TS:   // 手写 Map<string, number>
来源：http://ik.muxihuayi.cn

Java: // 手写 HashMap
来源：http://ug.jianghongdianzi.cn

Go:   // 手写 map[int]int
来源：http://ml.bookmarksfly.cn

Ruby: // 手写 Hash
来源：http://on.jianghongdianzi.cn

C#:   // 手写 Dictionary<int, int>
来源：http://jx.jianghongdianzi.cn

[N08] 生成全排列
来源：http://wd.huanxung.cn

Py:   itertools.permutations(arr)
来源：http://eu.haigaiapp.cn

PHP:  // 手写递归交换
来源：http://xj.muxihuayi.cn

JS:   // 手写回溯递归
来源：http://rl.nicolike.cn

TS:   // 手写回溯递归
来源：http://hb.newstarts.cn

Java: // 手写回溯递归
来源：http://ll.521024.cn

Go:   // 手写回溯递归
来源：http://hg.muxihuayi.cn

Ruby: arr.permutation.to_a
来源：http://hu.lnxyls.cn

C#:   // 手写回溯递归
来源：http://qt.jctech888.com.cn

[N09] 栈与队列
来源：http://qp.bookmarksfly.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://er.szxytkj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ty.bookmarksfly.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://pz.lnxyls.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://xf.yuntaijiaju.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ns.asd995.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://sp.bjjhwx.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://yi.muxihuayi.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://tc.bjjhwx.cn

[N10] 链表节点定义
来源：http://nd.nszjky.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://us.yuntaijiaju.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://gs.huixiangedu.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://rq.szxytkj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://jo.szsharing.cn

Java: class Node { int v; Node next; }
来源：http://tv.9csxet.cn

Go:   type Node struct { V int; Next *Node }
来源：http://qn.yuexingan06.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://tz.panjiajie.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ee.newstarts.cn

[N11] 二叉树中序遍历
来源：http://ag.szxytkj.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://lx.bjjhwx.cn

PHP:  // 手写递归函数
来源：http://vx.szsharing.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cf.521024.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://df.hahajie.cn

Java: // 手写递归
来源：http://ld.shtwfgs.cn

Go:   // 手写递归
来源：http://zb.bookmarksfly.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://pm.jianghongdianzi.cn

C#:   // 手写递归
来源：http://xc.szxytkj.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://jd.nicolike.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://aq.bjjhwx.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://qd.521024.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ke.gzmigu.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ec.9csxet.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ew.colortex.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://fq.521024.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://tg.panjiajie.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://kp.521024.cn

================================================================================
来源：http://am.newstarts.cn

O. 并发与异步
来源：http://ts.lnxyls.cn

================================================================================
来源：http://gd.huixinmuqiang.cn

[O01] 启动一个线程
来源：http://lo.newstarts.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://xa.jctech888.com.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://rn.jctech888.com.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://tl.hnjuh.cn

TS:   // 同 JS
来源：http://fz.chemitech.net.cn

Java: new Thread(() -> f()).start()
来源：http://sy.asd995.cn

Go:   go f()
来源：http://ys.szsharing.cn

Ruby: Thread.new { f }
来源：http://bj.szxytkj.cn

C#:   Task.Run(() => F());
来源：http://wq.shxzskj.cn

[O02] 使用线程池
来源：http://vx.huanxung.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://fg.szxytkj.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://dk.newstarts.cn

JS:   // worker_threads 线程池
来源：http://fa.shxzukj.cn

TS:   // worker_threads 线程池
来源：http://pf.9csxet.cn

Java: Executors.newFixedThreadPool(4)
来源：http://jd.hahajie.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://pa.jianghongdianzi.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://lo.panjiajie.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ss.521024.cn

[O03] 加锁保护共享数据
来源：http://vb.haigaiapp.cn

Py:   with lock: shared += 1
来源：http://pw.gzmigu.cn

PHP:  // 用 flock() 做文件锁
来源：http://sr.521024.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://cw.asd995.cn

TS:   // 同 JS
来源：http://wc.haigaiapp.cn

Java: synchronized (this) { shared++; }
来源：http://lr.newstarts.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://uq.hahajie.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://se.muxihuayi.cn

C#:   lock (gate) { shared++; }
来源：http://rd.haigaiapp.cn

[O04] 定义异步函数并等待
来源：http://em.haigaiapp.cn

Py:   async def f():⏎    await g()
来源：http://qj.jianghongdianzi.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mc.jianghongdianzi.cn

JS:   async function f() { await g(); }
来源：http://mz.panjiajie.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://yw.huixiangedu.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://sa.panjiajie.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://zh.huixiangedu.cn

Ruby: # 用 Fiber 或 async gem
来源：http://tk.huixinmuqiang.cn

C#:   async Task F() { await G(); }
来源：http://oj.yuntaijiaju.cn

[O05] 并发执行并等待全部完成
来源：http://sa.bookmarksfly.cn

Py:   asyncio.gather(*tasks)
来源：http://py.wgjwhj.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mv.colortex.cn

JS:   await Promise.all(tasks)
来源：http://gx.nicolike.cn

TS:   await Promise.all(tasks)
来源：http://jx.szsharing.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://xl.muxihuayi.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://dy.szsharing.cn

Ruby: threads.map(&:join)
来源：http://qk.lnxyls.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ja.nicolike.cn

[O06] 使用进程池
来源：http://fl.hahajie.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://vl.521024.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ej.lnxyls.cn

JS:   // child_process / cluster 模块
来源：http://mb.szsharing.cn

TS:   // child_process / cluster 模块
来源：http://uz.chemitech.net.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ry.521024.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hg.gzmigu.cn

Ruby: // fork 块
来源：http://sg.yuexingan06.cn

C#:   Parallel.For
来源：http://vf.yuntaijiaju.cn

================================================================================
来源：http://fg.haigaiapp.cn

P. 常用工具函数
来源：http://je.newstarts.cn

================================================================================
来源：http://bu.colortex.cn

[P01] 生成 UUID
来源：http://ob.asd995.cn

Py:   str(uuid.uuid4())
来源：http://hq.asd995.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://rr.chemitech.net.cn

JS:   crypto.randomUUID()
来源：http://pp.wgjwhj.cn

TS:   crypto.randomUUID()
来源：http://iy.hahajie.cn

Java: UUID.randomUUID().toString()
来源：http://xg.szsharing.cn

Go:   // 用 github.com/google/uuid
来源：http://uo.lnxyls.cn

Ruby: SecureRandom.uuid
来源：http://io.521024.cn

C#:   Guid.NewGuid().ToString()
来源：http://ij.huixinmuqiang.cn

[P02] MD5 / SHA256 摘要
来源：http://zn.muxihuayi.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://xg.yuexingan06.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://yc.huanxung.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ea.newstarts.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://kr.asd995.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://rv.gzmigu.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://yz.huixiangedu.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wx.shxzukj.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://dj.nicolike.cn

[P03] 生成短随机字符串
来源：http://xu.521024.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ut.521024.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://qc.jianghongdianzi.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gs.jctech888.com.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://oy.huixiangedu.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://de.wgjwhj.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://bv.panjiajie.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://fy.shxzukj.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://oc.muxihuayi.cn

[P04] 求长度
来源：http://kc.shxzukj.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://pm.shxzskj.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yp.wgjwhj.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vb.jctech888.com.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tb.bookmarksfly.cn

Java: list.size();  map.size();  s.length()
来源：http://gu.shxzukj.cn

Go:   len(arr);  len(m)
来源：http://es.bjjhwx.cn

Ruby: x.length;  x.size
来源：http://tf.asd995.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://kp.yuntaijiaju.cn

[P05] 判断两个对象内容是否相等
来源：http://bo.muxihuayi.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://uy.jctech888.com.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ol.bjjhwx.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://fo.szxytkj.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ec.jianghongdianzi.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://pq.yuexingan06.cn

Go:   reflect.DeepEqual(a, b)
来源：http://kw.jianghongdianzi.cn

Ruby: a == b
来源：http://ah.yuexingan06.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://fy.szsharing.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://tl.chemitech.net.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://dl.hnjuh.cn

PHP:  if (empty($x)) {}
来源：http://ii.nszjky.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://xs.colortex.cn

TS:   if (x == null) {}
来源：http://lt.yuexingan06.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://fj.shxzskj.cn

Go:   if x == nil {}
来源：http://rj.szxytkj.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://cn.yuntaijiaju.cn

C#:   if (x is null) {}
来源：http://he.gzmigu.cn

[P07] 防抖与节流
来源：http://zt.gzmigu.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ix.hahajie.cn

PHP:  // 手写时间戳比较
来源：http://xd.huixinmuqiang.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bn.wgjwhj.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://oq.hnjuh.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://sm.colortex.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://cz.haigaiapp.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://pb.gzmigu.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://pi.yuntaijiaju.cn

[P08] 处理浮点精度问题
来源：http://ml.szsharing.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://xn.newstarts.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://vx.bookmarksfly.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://pp.colortex.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ca.shxzskj.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://rz.shxzukj.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://td.shtwfgs.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://sj.huixinmuqiang.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://fz.huixinmuqiang.cn

================================================================================
来源：http://of.asd995.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ks.lnxyls.cn

================================================================================
来源：http://hr.wgjwhj.cn

[Q01] 创建表
来源：http://vq.muxihuayi.cn

CREATE TABLE users (
来源：http://rn.gzmigu.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ea.lnxyls.cn

name VARCHAR(50) NOT NULL,
来源：http://tq.haigaiapp.cn

email VARCHAR(100) UNIQUE,
来源：http://ol.haigaiapp.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://kp.huixinmuqiang.cn

);
来源：http://qo.shxzukj.cn

[Q02] 创建带外键的表
来源：http://og.hahajie.cn

CREATE TABLE orders (
来源：http://bg.shtwfgs.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://sn.bjjhwx.cn

user_id INT NOT NULL,
来源：http://rq.wgjwhj.cn

amount DECIMAL(10, 2),
来源：http://lh.521024.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://xp.haigaiapp.cn

);
来源：http://up.bookmarksfly.cn

[Q03] 增加列
来源：http://po.shxzskj.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wa.hahajie.cn

[Q04] 修改列类型
来源：http://ng.chemitech.net.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://qh.yuntaijiaju.cn

[Q05] 重命名列
来源：http://hj.gzmigu.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hf.lnxyls.cn

[Q06] 删除列
来源：http://qr.bookmarksfly.cn

ALTER TABLE users DROP COLUMN age;
来源：http://wx.nszjky.cn

[Q07] 删除表
来源：http://aq.yuntaijiaju.cn

DROP TABLE IF EXISTS orders;
来源：http://az.gzmigu.cn

[Q08] 创建普通索引
来源：http://tk.szxytkj.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://cx.9csxet.cn

[Q09] 创建唯一索引
来源：http://yn.bjjhwx.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://sz.jianghongdianzi.cn

[Q10] 插入单行
来源：http://zt.lnxyls.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://fx.jctech888.com.cn

[Q11] 一次插入多行
来源：http://dk.wgjwhj.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://gp.haigaiapp.cn

[Q12] 插入后取自增 ID
来源：http://de.szsharing.cn


<!-- 参考信息 -->