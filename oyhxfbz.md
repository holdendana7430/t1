代发 wailian999

Py:   if __name__ == "__main__":
来源：http://gp.9csxet.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://gt.nicolike.cn

JS:   require.main === module
来源：http://pq.wgjwhj.cn

TS:   require.main === module
来源：http://nd.shxzukj.cn

Java: public static void main(String[] args)
来源：http://hu.lnxyls.cn

Go:   func main()
来源：http://lr.shxzukj.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://xa.chemitech.net.cn

C#:   static void Main(string[] args)
来源：http://vl.huixiangedu.cn

[M08] 获取系统与运行时信息
来源：http://rr.huixinmuqiang.cn

Py:   platform.system();  platform.python_version()
来源：http://je.bjjhwx.cn

PHP:  PHP_OS;  phpversion();
来源：http://sf.nicolike.cn

JS:   process.platform;  process.version
来源：http://ak.muxihuayi.cn

TS:   process.platform;  process.version
来源：http://rw.asd995.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://zl.yuexingan06.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://jk.asd995.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://jr.yuntaijiaju.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ck.9csxet.cn

================================================================================
来源：http://wk.haigaiapp.cn

N. 数据结构与算法
来源：http://md.jianghongdianzi.cn

================================================================================
来源：http://xp.yuexingan06.cn

[N01] 二分查找（有序数组）
来源：http://wo.nicolike.cn

Py:   bisect.bisect_left(arr, x)
来源：http://zx.szsharing.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wd.bookmarksfly.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mi.huixiangedu.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dm.bookmarksfly.cn

Java: Arrays.binarySearch(arr, x)
来源：http://dm.shtwfgs.cn

Go:   sort.SearchInts(arr, x)
来源：http://ke.shxzskj.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ja.szsharing.cn

C#:   Array.BinarySearch(arr, x)
来源：http://yd.9csxet.cn

[N02] 排序（工程实践用内置实现）
来源：http://oi.bookmarksfly.cn

Py:   sorted(arr);  arr.sort()
来源：http://nu.shtwfgs.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://xr.yuntaijiaju.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://pe.hnjuh.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ep.jianghongdianzi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hm.haigaiapp.cn

Go:   slices.Sort(arr)
来源：http://ew.wgjwhj.cn

Ruby: arr.sort
来源：http://au.huanxung.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://uk.colortex.cn

[N03] 快速排序（分治示例）
来源：http://rx.hahajie.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://zv.shxzukj.cn

PHP:  // 递归实现，或用 usort
来源：http://fp.szxytkj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qm.huanxung.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cr.lnxyls.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://lm.9csxet.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://jj.nicolike.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wr.newstarts.cn

C#:   // 手写递归，或 Array.Sort
来源：http://rw.jianghongdianzi.cn

[N04] 斐波那契数列
来源：http://rv.shxzskj.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://in.yuexingan06.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ua.bjjhwx.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hh.jianghongdianzi.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vw.gzmigu.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://dy.lnxyls.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://eo.chemitech.net.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://og.chemitech.net.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://rf.lnxyls.cn

[N05] 最大公约数
来源：http://ck.jctech888.com.cn

Py:   math.gcd(a, b)
来源：http://qg.shtwfgs.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wo.hahajie.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jc.jctech888.com.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://uz.bookmarksfly.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://po.haigaiapp.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://vy.lnxyls.cn

Ruby: a.gcd(b)
来源：http://xu.hnjuh.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://lb.asd995.cn

[N06] 判断回文字符串
来源：http://bl.jianghongdianzi.cn

Py:   s == s[::-1]
来源：http://ti.hnjuh.cn

PHP:  $s === strrev($s);
来源：http://az.lnxyls.cn

JS:   s === [...s].reverse().join("")
来源：http://il.haigaiapp.cn

TS:   s === [...s].reverse().join("")
来源：http://nm.hnjuh.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ua.lnxyls.cn

Go:   // 双指针从两端比较
来源：http://dl.yuexingan06.cn

Ruby: s == s.reverse
来源：http://lj.huixinmuqiang.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://uh.shxzukj.cn

[N07] 两数之和（返回下标）
来源：http://js.panjiajie.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ks.gzmigu.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://so.bjjhwx.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://is.521024.cn

TS:   // 手写 Map<string, number>
来源：http://eo.jianghongdianzi.cn

Java: // 手写 HashMap
来源：http://fr.wgjwhj.cn

Go:   // 手写 map[int]int
来源：http://jk.yuexingan06.cn

Ruby: // 手写 Hash
来源：http://kz.shtwfgs.cn

C#:   // 手写 Dictionary<int, int>
来源：http://jx.jianghongdianzi.cn

[N08] 生成全排列
来源：http://pv.521024.cn

Py:   itertools.permutations(arr)
来源：http://rw.nicolike.cn

PHP:  // 手写递归交换
来源：http://sg.huixinmuqiang.cn

JS:   // 手写回溯递归
来源：http://rb.hnjuh.cn

TS:   // 手写回溯递归
来源：http://on.shxzskj.cn

Java: // 手写回溯递归
来源：http://tc.521024.cn

Go:   // 手写回溯递归
来源：http://ir.521024.cn

Ruby: arr.permutation.to_a
来源：http://fn.huanxung.cn

C#:   // 手写回溯递归
来源：http://rg.colortex.cn

[N09] 栈与队列
来源：http://ti.shxzukj.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://kw.nicolike.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://xt.newstarts.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://jc.asd995.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://bl.shtwfgs.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://jw.yuntaijiaju.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://jn.shtwfgs.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://rr.9csxet.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ih.jianghongdianzi.cn

[N10] 链表节点定义
来源：http://ly.newstarts.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://rq.jianghongdianzi.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://pz.nszjky.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://nq.szxytkj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://kt.9csxet.cn

Java: class Node { int v; Node next; }
来源：http://kr.haigaiapp.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ya.nicolike.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ke.521024.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://bb.yuexingan06.cn

[N11] 二叉树中序遍历
来源：http://yx.muxihuayi.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://pj.gzmigu.cn

PHP:  // 手写递归函数
来源：http://lx.szxytkj.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qy.9csxet.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ap.szxytkj.cn

Java: // 手写递归
来源：http://cr.newstarts.cn

Go:   // 手写递归
来源：http://gp.chemitech.net.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://jb.hnjuh.cn

C#:   // 手写递归
来源：http://jj.521024.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://nj.lnxyls.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://jm.hahajie.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://sc.shtwfgs.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gf.huanxung.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mq.jianghongdianzi.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://im.newstarts.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://os.yuexingan06.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://tw.huixiangedu.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://xs.hnjuh.cn

================================================================================
来源：http://dj.bjjhwx.cn

O. 并发与异步
来源：http://lh.bookmarksfly.cn

================================================================================
来源：http://jg.521024.cn

[O01] 启动一个线程
来源：http://xp.wgjwhj.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://jv.hnjuh.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qq.huanxung.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://cc.huanxung.cn

TS:   // 同 JS
来源：http://js.wgjwhj.cn

Java: new Thread(() -> f()).start()
来源：http://vs.521024.cn

Go:   go f()
来源：http://xx.chemitech.net.cn

Ruby: Thread.new { f }
来源：http://en.asd995.cn

C#:   Task.Run(() => F());
来源：http://fe.9csxet.cn

[O02] 使用线程池
来源：http://uo.yuntaijiaju.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://kz.shtwfgs.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mz.shxzskj.cn

JS:   // worker_threads 线程池
来源：http://gi.nszjky.cn

TS:   // worker_threads 线程池
来源：http://zj.wgjwhj.cn

Java: Executors.newFixedThreadPool(4)
来源：http://fd.shtwfgs.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://sq.shxzukj.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://eo.shxzskj.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://vu.bjjhwx.cn

[O03] 加锁保护共享数据
来源：http://cf.hnjuh.cn

Py:   with lock: shared += 1
来源：http://bw.haigaiapp.cn

PHP:  // 用 flock() 做文件锁
来源：http://jk.wgjwhj.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://eo.yuexingan06.cn

TS:   // 同 JS
来源：http://zd.jianghongdianzi.cn

Java: synchronized (this) { shared++; }
来源：http://de.shtwfgs.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://kk.newstarts.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ne.szxytkj.cn

C#:   lock (gate) { shared++; }
来源：http://vk.haigaiapp.cn

[O04] 定义异步函数并等待
来源：http://iz.wgjwhj.cn

Py:   async def f():⏎    await g()
来源：http://bj.hnjuh.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://vs.newstarts.cn

JS:   async function f() { await g(); }
来源：http://qe.haigaiapp.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://vc.yuntaijiaju.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hh.lnxyls.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://br.huanxung.cn

Ruby: # 用 Fiber 或 async gem
来源：http://oc.lnxyls.cn

C#:   async Task F() { await G(); }
来源：http://nr.muxihuayi.cn

[O05] 并发执行并等待全部完成
来源：http://zb.gzmigu.cn

Py:   asyncio.gather(*tasks)
来源：http://lw.yuexingan06.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://cf.colortex.cn

JS:   await Promise.all(tasks)
来源：http://kd.yuexingan06.cn

TS:   await Promise.all(tasks)
来源：http://jo.9csxet.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://us.panjiajie.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://kq.bookmarksfly.cn

Ruby: threads.map(&:join)
来源：http://ot.colortex.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://xi.haigaiapp.cn

[O06] 使用进程池
来源：http://xl.shxzukj.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mk.panjiajie.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://lu.newstarts.cn

JS:   // child_process / cluster 模块
来源：http://qk.huanxung.cn

TS:   // child_process / cluster 模块
来源：http://tg.newstarts.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://he.wgjwhj.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://su.521024.cn

Ruby: // fork 块
来源：http://fw.asd995.cn

C#:   Parallel.For
来源：http://vk.lnxyls.cn

================================================================================
来源：http://to.9csxet.cn

P. 常用工具函数
来源：http://cr.9csxet.cn

================================================================================
来源：http://dv.hnjuh.cn

[P01] 生成 UUID
来源：http://bv.hnjuh.cn

Py:   str(uuid.uuid4())
来源：http://as.521024.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ys.shtwfgs.cn

JS:   crypto.randomUUID()
来源：http://uk.colortex.cn

TS:   crypto.randomUUID()
来源：http://nh.szxytkj.cn

Java: UUID.randomUUID().toString()
来源：http://uz.nicolike.cn

Go:   // 用 github.com/google/uuid
来源：http://ki.yuntaijiaju.cn

Ruby: SecureRandom.uuid
来源：http://ag.asd995.cn

C#:   Guid.NewGuid().ToString()
来源：http://cs.shtwfgs.cn

[P02] MD5 / SHA256 摘要
来源：http://xg.nicolike.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://iq.shxzskj.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://hg.szxytkj.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://me.jctech888.com.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://km.huixinmuqiang.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://xb.521024.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://fj.yuntaijiaju.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://so.chemitech.net.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://lg.shxzukj.cn

[P03] 生成短随机字符串
来源：http://gf.jctech888.com.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://pd.yuntaijiaju.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://dl.chemitech.net.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qo.521024.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://th.huixinmuqiang.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://el.lnxyls.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://qc.bjjhwx.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://zf.shtwfgs.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://th.lnxyls.cn

[P04] 求长度
来源：http://ee.huanxung.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ep.jctech888.com.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mj.newstarts.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://sw.asd995.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qg.jianghongdianzi.cn

Java: list.size();  map.size();  s.length()
来源：http://ls.bjjhwx.cn

Go:   len(arr);  len(m)
来源：http://do.wgjwhj.cn

Ruby: x.length;  x.size
来源：http://uw.hahajie.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://do.yuntaijiaju.cn

[P05] 判断两个对象内容是否相等
来源：http://lr.hnjuh.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://us.bjjhwx.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://fy.hahajie.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://xd.yuexingan06.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://eo.9csxet.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wx.muxihuayi.cn

Go:   reflect.DeepEqual(a, b)
来源：http://nq.hnjuh.cn

Ruby: a == b
来源：http://kg.huixiangedu.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://xf.szxytkj.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://fz.huixiangedu.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://xi.yuntaijiaju.cn

PHP:  if (empty($x)) {}
来源：http://kg.shtwfgs.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://up.muxihuayi.cn

TS:   if (x == null) {}
来源：http://le.colortex.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://qx.panjiajie.cn

Go:   if x == nil {}
来源：http://cv.huixinmuqiang.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://cv.jianghongdianzi.cn

C#:   if (x is null) {}
来源：http://fi.lnxyls.cn

[P07] 防抖与节流
来源：http://wd.szxytkj.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://rb.jctech888.com.cn

PHP:  // 手写时间戳比较
来源：http://pk.9csxet.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ze.szxytkj.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fv.huixinmuqiang.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://lz.bjjhwx.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ov.wgjwhj.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ml.huixiangedu.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ei.szxytkj.cn

[P08] 处理浮点精度问题
来源：http://be.szsharing.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ho.9csxet.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://sn.yuexingan06.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://fa.colortex.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://vu.colortex.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ic.wgjwhj.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hd.nszjky.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://xp.yuntaijiaju.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://vl.gzmigu.cn

================================================================================
来源：http://pw.colortex.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://gv.wgjwhj.cn

================================================================================
来源：http://ce.gzmigu.cn

[Q01] 创建表
来源：http://ro.newstarts.cn

CREATE TABLE users (
来源：http://ub.huanxung.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://eq.nicolike.cn

name VARCHAR(50) NOT NULL,
来源：http://lr.jctech888.com.cn

email VARCHAR(100) UNIQUE,
来源：http://gm.panjiajie.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://oq.colortex.cn

);
来源：http://nt.shtwfgs.cn

[Q02] 创建带外键的表
来源：http://bv.hahajie.cn

CREATE TABLE orders (
来源：http://uw.9csxet.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wo.colortex.cn

user_id INT NOT NULL,
来源：http://vl.huanxung.cn

amount DECIMAL(10, 2),
来源：http://fa.panjiajie.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://tp.9csxet.cn

);
来源：http://rk.bjjhwx.cn

[Q03] 增加列
来源：http://iz.521024.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hi.521024.cn

[Q04] 修改列类型
来源：http://ki.asd995.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://zj.bjjhwx.cn

[Q05] 重命名列
来源：http://pa.jctech888.com.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ar.panjiajie.cn

[Q06] 删除列
来源：http://to.bookmarksfly.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ez.yuntaijiaju.cn

[Q07] 删除表
来源：http://ay.bookmarksfly.cn

DROP TABLE IF EXISTS orders;
来源：http://cn.szxytkj.cn

[Q08] 创建普通索引
来源：http://nl.nszjky.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://sd.szxytkj.cn

[Q09] 创建唯一索引
来源：http://pa.hahajie.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://by.colortex.cn

[Q10] 插入单行
来源：http://ph.huanxung.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://gn.lnxyls.cn

[Q11] 一次插入多行
来源：http://np.muxihuayi.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://iz.jianghongdianzi.cn

[Q12] 插入后取自增 ID
来源：http://rd.nszjky.cn

INSERT INTO users (name) VALUES ('C');
来源：http://mv.gzmigu.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://zz.lnxyls.cn

[Q13] 忽略重复插入
来源：http://qe.asd995.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://fq.shxzskj.cn


<!-- 参考信息 -->