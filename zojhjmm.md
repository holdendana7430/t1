代发 wailian999

Py:   if __name__ == "__main__":
来源：http://hk.newstarts.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://si.haigaiapp.cn

JS:   require.main === module
来源：http://uy.lnxyls.cn

TS:   require.main === module
来源：http://qs.panjiajie.cn

Java: public static void main(String[] args)
来源：http://uk.shxzukj.cn

Go:   func main()
来源：http://dc.9csxet.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://bw.shxzukj.cn

C#:   static void Main(string[] args)
来源：http://fm.bjjhwx.cn

[M08] 获取系统与运行时信息
来源：http://cq.nicolike.cn

Py:   platform.system();  platform.python_version()
来源：http://zv.asd995.cn

PHP:  PHP_OS;  phpversion();
来源：http://oj.521024.cn

JS:   process.platform;  process.version
来源：http://ic.nszjky.cn

TS:   process.platform;  process.version
来源：http://qw.521024.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://jb.huixiangedu.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://vv.jctech888.com.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.huixinmuqiang.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://qm.chemitech.net.cn

================================================================================
来源：http://jm.yuexingan06.cn

N. 数据结构与算法
来源：http://ie.huixinmuqiang.cn

================================================================================
来源：http://ka.shtwfgs.cn

[N01] 二分查找（有序数组）
来源：http://jw.yuexingan06.cn

Py:   bisect.bisect_left(arr, x)
来源：http://qy.panjiajie.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://af.yuntaijiaju.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lp.9csxet.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ig.nicolike.cn

Java: Arrays.binarySearch(arr, x)
来源：http://qn.haigaiapp.cn

Go:   sort.SearchInts(arr, x)
来源：http://eo.szxytkj.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://di.szsharing.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ji.bjjhwx.cn

[N02] 排序（工程实践用内置实现）
来源：http://lh.yuntaijiaju.cn

Py:   sorted(arr);  arr.sort()
来源：http://fu.hahajie.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ps.bookmarksfly.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ev.asd995.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ao.hahajie.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://oo.lnxyls.cn

Go:   slices.Sort(arr)
来源：http://nr.asd995.cn

Ruby: arr.sort
来源：http://bh.nszjky.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://an.panjiajie.cn

[N03] 快速排序（分治示例）
来源：http://ej.shtwfgs.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://tg.huixinmuqiang.cn

PHP:  // 递归实现，或用 usort
来源：http://us.yuntaijiaju.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tl.lnxyls.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sn.shxzskj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://qw.hahajie.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://dz.shxzukj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://rr.huanxung.cn

C#:   // 手写递归，或 Array.Sort
来源：http://zl.huixinmuqiang.cn

[N04] 斐波那契数列
来源：http://el.szxytkj.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qu.yuexingan06.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://sd.lnxyls.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ka.huixiangedu.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hq.colortex.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mz.bookmarksfly.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://bd.hahajie.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://eh.bjjhwx.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://of.bjjhwx.cn

[N05] 最大公约数
来源：http://vu.panjiajie.cn

Py:   math.gcd(a, b)
来源：http://vc.panjiajie.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://in.panjiajie.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zk.newstarts.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fs.lnxyls.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://cb.muxihuayi.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ij.gzmigu.cn

Ruby: a.gcd(b)
来源：http://ka.yuexingan06.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://sk.nszjky.cn

[N06] 判断回文字符串
来源：http://ll.huixiangedu.cn

Py:   s == s[::-1]
来源：http://yf.nicolike.cn

PHP:  $s === strrev($s);
来源：http://fs.nszjky.cn

JS:   s === [...s].reverse().join("")
来源：http://xu.nszjky.cn

TS:   s === [...s].reverse().join("")
来源：http://io.colortex.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mi.chemitech.net.cn

Go:   // 双指针从两端比较
来源：http://ka.yuntaijiaju.cn

Ruby: s == s.reverse
来源：http://fk.muxihuayi.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://jy.huanxung.cn

[N07] 两数之和（返回下标）
来源：http://gy.bjjhwx.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://vk.shxzskj.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://cb.haigaiapp.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://xr.hahajie.cn

TS:   // 手写 Map<string, number>
来源：http://yr.gzmigu.cn

Java: // 手写 HashMap
来源：http://ix.muxihuayi.cn

Go:   // 手写 map[int]int
来源：http://qo.wgjwhj.cn

Ruby: // 手写 Hash
来源：http://nb.jianghongdianzi.cn

C#:   // 手写 Dictionary<int, int>
来源：http://al.huixinmuqiang.cn

[N08] 生成全排列
来源：http://re.jctech888.com.cn

Py:   itertools.permutations(arr)
来源：http://ki.jianghongdianzi.cn

PHP:  // 手写递归交换
来源：http://mb.nszjky.cn

JS:   // 手写回溯递归
来源：http://by.bookmarksfly.cn

TS:   // 手写回溯递归
来源：http://fh.shxzskj.cn

Java: // 手写回溯递归
来源：http://rd.lnxyls.cn

Go:   // 手写回溯递归
来源：http://dh.shxzskj.cn

Ruby: arr.permutation.to_a
来源：http://wu.lnxyls.cn

C#:   // 手写回溯递归
来源：http://kf.jianghongdianzi.cn

[N09] 栈与队列
来源：http://wo.bookmarksfly.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://am.nszjky.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://yl.huanxung.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://no.hahajie.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wi.chemitech.net.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ji.lnxyls.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://sz.lnxyls.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://nc.shxzskj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://iu.yuntaijiaju.cn

[N10] 链表节点定义
来源：http://rm.yuntaijiaju.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hi.lnxyls.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://rr.colortex.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qa.huanxung.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://bk.panjiajie.cn

Java: class Node { int v; Node next; }
来源：http://tv.hahajie.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ds.newstarts.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ic.yuntaijiaju.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://sf.hnjuh.cn

[N11] 二叉树中序遍历
来源：http://eh.colortex.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://kc.asd995.cn

PHP:  // 手写递归函数
来源：http://xg.jctech888.com.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fj.wgjwhj.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bx.hnjuh.cn

Java: // 手写递归
来源：http://eq.newstarts.cn

Go:   // 手写递归
来源：http://ay.jctech888.com.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://bm.huanxung.cn

C#:   // 手写递归
来源：http://sw.hnjuh.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://nr.shxzskj.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://bs.shxzskj.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://zz.nszjky.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yr.huanxung.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nd.yuntaijiaju.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://fz.huanxung.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://kv.521024.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://vd.bookmarksfly.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://gs.hahajie.cn

================================================================================
来源：http://xx.newstarts.cn

O. 并发与异步
来源：http://tw.huixiangedu.cn

================================================================================
来源：http://pd.shtwfgs.cn

[O01] 启动一个线程
来源：http://bs.huixinmuqiang.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wr.haigaiapp.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://zm.huanxung.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://yz.szsharing.cn

TS:   // 同 JS
来源：http://gv.wgjwhj.cn

Java: new Thread(() -> f()).start()
来源：http://do.yuexingan06.cn

Go:   go f()
来源：http://ti.jctech888.com.cn

Ruby: Thread.new { f }
来源：http://sr.hahajie.cn

C#:   Task.Run(() => F());
来源：http://ge.huanxung.cn

[O02] 使用线程池
来源：http://si.jianghongdianzi.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://gj.yuexingan06.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ho.haigaiapp.cn

JS:   // worker_threads 线程池
来源：http://br.yuexingan06.cn

TS:   // worker_threads 线程池
来源：http://fw.yuexingan06.cn

Java: Executors.newFixedThreadPool(4)
来源：http://gq.colortex.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://em.panjiajie.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://rx.shxzukj.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hy.nicolike.cn

[O03] 加锁保护共享数据
来源：http://sj.bjjhwx.cn

Py:   with lock: shared += 1
来源：http://hr.shxzskj.cn

PHP:  // 用 flock() 做文件锁
来源：http://ku.huixinmuqiang.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://yc.gzmigu.cn

TS:   // 同 JS
来源：http://gi.bookmarksfly.cn

Java: synchronized (this) { shared++; }
来源：http://fo.shxzskj.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://jp.nicolike.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ym.muxihuayi.cn

C#:   lock (gate) { shared++; }
来源：http://it.jctech888.com.cn

[O04] 定义异步函数并等待
来源：http://xf.huixinmuqiang.cn

Py:   async def f():⏎    await g()
来源：http://kw.muxihuayi.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://zi.nicolike.cn

JS:   async function f() { await g(); }
来源：http://iv.huixiangedu.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://qo.szsharing.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://my.yuntaijiaju.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://vw.szxytkj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://dv.nicolike.cn

C#:   async Task F() { await G(); }
来源：http://vu.szxytkj.cn

[O05] 并发执行并等待全部完成
来源：http://cq.hnjuh.cn

Py:   asyncio.gather(*tasks)
来源：http://ob.wgjwhj.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://kp.gzmigu.cn

JS:   await Promise.all(tasks)
来源：http://bn.yuexingan06.cn

TS:   await Promise.all(tasks)
来源：http://hn.szxytkj.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ol.panjiajie.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://cz.lnxyls.cn

Ruby: threads.map(&:join)
来源：http://tw.bjjhwx.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://qe.hnjuh.cn

[O06] 使用进程池
来源：http://dc.gzmigu.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://zw.yuntaijiaju.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://qo.yuexingan06.cn

JS:   // child_process / cluster 模块
来源：http://zj.yuntaijiaju.cn

TS:   // child_process / cluster 模块
来源：http://uh.bjjhwx.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mx.huanxung.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://cv.huixiangedu.cn

Ruby: // fork 块
来源：http://wn.jianghongdianzi.cn

C#:   Parallel.For
来源：http://yg.wgjwhj.cn

================================================================================
来源：http://ah.wgjwhj.cn

P. 常用工具函数
来源：http://au.muxihuayi.cn

================================================================================
来源：http://cz.wgjwhj.cn

[P01] 生成 UUID
来源：http://ej.jctech888.com.cn

Py:   str(uuid.uuid4())
来源：http://jp.shxzukj.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://lq.haigaiapp.cn

JS:   crypto.randomUUID()
来源：http://jk.wgjwhj.cn

TS:   crypto.randomUUID()
来源：http://an.asd995.cn

Java: UUID.randomUUID().toString()
来源：http://hp.szsharing.cn

Go:   // 用 github.com/google/uuid
来源：http://ax.huanxung.cn

Ruby: SecureRandom.uuid
来源：http://fs.lnxyls.cn

C#:   Guid.NewGuid().ToString()
来源：http://ek.521024.cn

[P02] MD5 / SHA256 摘要
来源：http://gc.panjiajie.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ox.hahajie.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://fc.shxzskj.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://jc.shtwfgs.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://lg.jctech888.com.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://yf.panjiajie.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://tx.newstarts.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://jx.yuntaijiaju.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://bh.521024.cn

[P03] 生成短随机字符串
来源：http://ln.yuntaijiaju.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ae.hahajie.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://zo.wgjwhj.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gl.lnxyls.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ha.lnxyls.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://zk.hnjuh.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://jc.yuexingan06.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://en.chemitech.net.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mr.bookmarksfly.cn

[P04] 求长度
来源：http://ve.wgjwhj.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://va.nicolike.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ei.huanxung.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kv.asd995.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zs.9csxet.cn

Java: list.size();  map.size();  s.length()
来源：http://mp.521024.cn

Go:   len(arr);  len(m)
来源：http://mv.shtwfgs.cn

Ruby: x.length;  x.size
来源：http://kg.huixiangedu.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://dy.wgjwhj.cn

[P05] 判断两个对象内容是否相等
来源：http://zc.haigaiapp.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://yu.colortex.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://jk.nszjky.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://bz.wgjwhj.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ea.lnxyls.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ww.bookmarksfly.cn

Go:   reflect.DeepEqual(a, b)
来源：http://fo.szxytkj.cn

Ruby: a == b
来源：http://zs.hnjuh.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://an.huixiangedu.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://zl.szxytkj.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://us.hahajie.cn

PHP:  if (empty($x)) {}
来源：http://ph.nicolike.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://vn.shxzukj.cn

TS:   if (x == null) {}
来源：http://wj.bjjhwx.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://cu.haigaiapp.cn

Go:   if x == nil {}
来源：http://zk.huixiangedu.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://il.shxzskj.cn

C#:   if (x is null) {}
来源：http://si.shxzskj.cn

[P07] 防抖与节流
来源：http://nh.panjiajie.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://qs.shxzukj.cn

PHP:  // 手写时间戳比较
来源：http://cy.szxytkj.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hw.hahajie.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fe.hahajie.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://dr.yuexingan06.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ba.newstarts.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://rk.hnjuh.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://gb.newstarts.cn

[P08] 处理浮点精度问题
来源：http://qx.huanxung.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wy.szxytkj.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://zx.panjiajie.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://de.bjjhwx.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ep.bjjhwx.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hp.lnxyls.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://do.haigaiapp.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://qx.9csxet.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://sq.yuntaijiaju.cn

================================================================================
来源：http://yb.jianghongdianzi.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://gg.huixinmuqiang.cn

================================================================================
来源：http://on.huanxung.cn

[Q01] 创建表
来源：http://hv.yuntaijiaju.cn

CREATE TABLE users (
来源：http://sk.hnjuh.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://xq.asd995.cn

name VARCHAR(50) NOT NULL,
来源：http://ig.panjiajie.cn

email VARCHAR(100) UNIQUE,
来源：http://st.bookmarksfly.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://vr.szsharing.cn

);
来源：http://jc.chemitech.net.cn

[Q02] 创建带外键的表
来源：http://sl.chemitech.net.cn

CREATE TABLE orders (
来源：http://ae.gzmigu.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ml.521024.cn

user_id INT NOT NULL,
来源：http://vz.chemitech.net.cn

amount DECIMAL(10, 2),
来源：http://vb.shtwfgs.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://vz.9csxet.cn

);
来源：http://ro.colortex.cn

[Q03] 增加列
来源：http://gt.hahajie.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ph.shxzskj.cn

[Q04] 修改列类型
来源：http://ir.bookmarksfly.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://dt.yuexingan06.cn

[Q05] 重命名列
来源：http://kr.yuexingan06.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hg.521024.cn

[Q06] 删除列
来源：http://vf.huixinmuqiang.cn

ALTER TABLE users DROP COLUMN age;
来源：http://bb.colortex.cn

[Q07] 删除表
来源：http://uh.hnjuh.cn

DROP TABLE IF EXISTS orders;
来源：http://es.haigaiapp.cn

[Q08] 创建普通索引
来源：http://po.shtwfgs.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://vg.nszjky.cn

[Q09] 创建唯一索引
来源：http://ss.newstarts.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://lc.521024.cn

[Q10] 插入单行
来源：http://qg.yuexingan06.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://qr.shxzskj.cn

[Q11] 一次插入多行
来源：http://bt.asd995.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://eh.muxihuayi.cn

[Q12] 插入后取自增 ID
来源：http://do.haigaiapp.cn

INSERT INTO users (name) VALUES ('C');
来源：http://oh.yuexingan06.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://bf.wgjwhj.cn

[Q13] 忽略重复插入
来源：http://qw.nicolike.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://su.jctech888.com.cn


<!-- 参考信息 -->