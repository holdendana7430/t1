代发 wailian999

Py:   if __name__ == "__main__":
来源：http://su.hahajie.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://vn.bjjhwx.cn

JS:   require.main === module
来源：http://xv.wgjwhj.cn

TS:   require.main === module
来源：http://wy.panjiajie.cn

Java: public static void main(String[] args)
来源：http://bw.huixinmuqiang.cn

Go:   func main()
来源：http://vc.nszjky.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://fx.bjjhwx.cn

C#:   static void Main(string[] args)
来源：http://yd.colortex.cn

[M08] 获取系统与运行时信息
来源：http://fl.nszjky.cn

Py:   platform.system();  platform.python_version()
来源：http://yq.9csxet.cn

PHP:  PHP_OS;  phpversion();
来源：http://eb.jctech888.com.cn

JS:   process.platform;  process.version
来源：http://pl.jctech888.com.cn

TS:   process.platform;  process.version
来源：http://xp.bjjhwx.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hr.hnjuh.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://yq.521024.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://np.gzmigu.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ns.haigaiapp.cn

================================================================================
来源：http://we.szsharing.cn

N. 数据结构与算法
来源：http://zw.newstarts.cn

================================================================================
来源：http://zu.wgjwhj.cn

[N01] 二分查找（有序数组）
来源：http://gq.yuntaijiaju.cn

Py:   bisect.bisect_left(arr, x)
来源：http://dz.9csxet.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://lu.bookmarksfly.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jo.szsharing.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vb.yuntaijiaju.cn

Java: Arrays.binarySearch(arr, x)
来源：http://od.bookmarksfly.cn

Go:   sort.SearchInts(arr, x)
来源：http://sd.huixinmuqiang.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ia.shxzskj.cn

C#:   Array.BinarySearch(arr, x)
来源：http://qz.9csxet.cn

[N02] 排序（工程实践用内置实现）
来源：http://ba.chemitech.net.cn

Py:   sorted(arr);  arr.sort()
来源：http://ny.bookmarksfly.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ia.nszjky.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://td.huixiangedu.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://bo.newstarts.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://gr.wgjwhj.cn

Go:   slices.Sort(arr)
来源：http://fz.jianghongdianzi.cn

Ruby: arr.sort
来源：http://hv.huixinmuqiang.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://uq.9csxet.cn

[N03] 快速排序（分治示例）
来源：http://ld.lnxyls.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hs.shtwfgs.cn

PHP:  // 递归实现，或用 usort
来源：http://jn.huixinmuqiang.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wk.yuexingan06.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zy.bjjhwx.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ur.bjjhwx.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://bs.jctech888.com.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ec.haigaiapp.cn

C#:   // 手写递归，或 Array.Sort
来源：http://gb.wgjwhj.cn

[N04] 斐波那契数列
来源：http://dr.shtwfgs.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://cl.gzmigu.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://pt.haigaiapp.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hl.szsharing.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ap.muxihuayi.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://dm.shxzskj.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://vg.nszjky.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://dx.shxzskj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://eo.haigaiapp.cn

[N05] 最大公约数
来源：http://tb.jctech888.com.cn

Py:   math.gcd(a, b)
来源：http://xp.nszjky.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://op.haigaiapp.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vi.haigaiapp.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dt.jianghongdianzi.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://uh.wgjwhj.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://tt.newstarts.cn

Ruby: a.gcd(b)
来源：http://ha.nicolike.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://uy.szsharing.cn

[N06] 判断回文字符串
来源：http://be.shtwfgs.cn

Py:   s == s[::-1]
来源：http://yi.bjjhwx.cn

PHP:  $s === strrev($s);
来源：http://zs.shtwfgs.cn

JS:   s === [...s].reverse().join("")
来源：http://fp.yuexingan06.cn

TS:   s === [...s].reverse().join("")
来源：http://xt.wgjwhj.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wa.bjjhwx.cn

Go:   // 双指针从两端比较
来源：http://au.hnjuh.cn

Ruby: s == s.reverse
来源：http://pq.szsharing.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://dm.hahajie.cn

[N07] 两数之和（返回下标）
来源：http://qd.shxzskj.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ud.muxihuayi.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://qv.huanxung.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://wd.jctech888.com.cn

TS:   // 手写 Map<string, number>
来源：http://mg.yuntaijiaju.cn

Java: // 手写 HashMap
来源：http://nq.bjjhwx.cn

Go:   // 手写 map[int]int
来源：http://sy.yuntaijiaju.cn

Ruby: // 手写 Hash
来源：http://pr.lnxyls.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ux.bjjhwx.cn

[N08] 生成全排列
来源：http://au.gzmigu.cn

Py:   itertools.permutations(arr)
来源：http://tf.bjjhwx.cn

PHP:  // 手写递归交换
来源：http://nk.hahajie.cn

JS:   // 手写回溯递归
来源：http://dm.chemitech.net.cn

TS:   // 手写回溯递归
来源：http://nr.yuntaijiaju.cn

Java: // 手写回溯递归
来源：http://ki.nicolike.cn

Go:   // 手写回溯递归
来源：http://os.asd995.cn

Ruby: arr.permutation.to_a
来源：http://hm.huixinmuqiang.cn

C#:   // 手写回溯递归
来源：http://ff.asd995.cn

[N09] 栈与队列
来源：http://yj.shxzskj.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ve.muxihuayi.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://sp.jianghongdianzi.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://fd.huixinmuqiang.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://vb.newstarts.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://rj.wgjwhj.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://qb.hahajie.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://gi.shxzukj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wr.nszjky.cn

[N10] 链表节点定义
来源：http://ok.521024.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ww.haigaiapp.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://tc.nicolike.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://fs.chemitech.net.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mx.colortex.cn

Java: class Node { int v; Node next; }
来源：http://vz.shtwfgs.cn

Go:   type Node struct { V int; Next *Node }
来源：http://bp.asd995.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://cy.shxzskj.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://tg.newstarts.cn

[N11] 二叉树中序遍历
来源：http://mr.huixinmuqiang.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://xx.yuntaijiaju.cn

PHP:  // 手写递归函数
来源：http://ux.bookmarksfly.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pg.shxzskj.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://oo.panjiajie.cn

Java: // 手写递归
来源：http://ov.muxihuayi.cn

Go:   // 手写递归
来源：http://tr.bookmarksfly.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ma.bookmarksfly.cn

C#:   // 手写递归
来源：http://js.huixinmuqiang.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://qf.gzmigu.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mn.chemitech.net.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://sj.gzmigu.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jy.huixiangedu.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gk.szxytkj.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://tu.jianghongdianzi.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://aw.nszjky.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://gp.shxzskj.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://fd.huanxung.cn

================================================================================
来源：http://if.bookmarksfly.cn

O. 并发与异步
来源：http://mg.521024.cn

================================================================================
来源：http://sz.wgjwhj.cn

[O01] 启动一个线程
来源：http://lj.gzmigu.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://aa.wgjwhj.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://uv.hnjuh.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://lf.9csxet.cn

TS:   // 同 JS
来源：http://je.muxihuayi.cn

Java: new Thread(() -> f()).start()
来源：http://zq.hnjuh.cn

Go:   go f()
来源：http://tg.yuexingan06.cn

Ruby: Thread.new { f }
来源：http://hy.9csxet.cn

C#:   Task.Run(() => F());
来源：http://dh.colortex.cn

[O02] 使用线程池
来源：http://by.newstarts.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ty.jianghongdianzi.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://sl.jianghongdianzi.cn

JS:   // worker_threads 线程池
来源：http://oh.shxzskj.cn

TS:   // worker_threads 线程池
来源：http://pt.hnjuh.cn

Java: Executors.newFixedThreadPool(4)
来源：http://jt.shxzukj.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ya.bookmarksfly.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://qm.hahajie.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wf.colortex.cn

[O03] 加锁保护共享数据
来源：http://do.chemitech.net.cn

Py:   with lock: shared += 1
来源：http://dz.9csxet.cn

PHP:  // 用 flock() 做文件锁
来源：http://rc.asd995.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://dn.yuntaijiaju.cn

TS:   // 同 JS
来源：http://oi.hnjuh.cn

Java: synchronized (this) { shared++; }
来源：http://rm.shtwfgs.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ro.hnjuh.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://gb.colortex.cn

C#:   lock (gate) { shared++; }
来源：http://ph.jianghongdianzi.cn

[O04] 定义异步函数并等待
来源：http://mu.shxzukj.cn

Py:   async def f():⏎    await g()
来源：http://ti.shxzukj.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://an.muxihuayi.cn

JS:   async function f() { await g(); }
来源：http://ze.haigaiapp.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://px.panjiajie.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://fe.haigaiapp.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://tq.szxytkj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://qa.jctech888.com.cn

C#:   async Task F() { await G(); }
来源：http://nf.szxytkj.cn

[O05] 并发执行并等待全部完成
来源：http://tn.jianghongdianzi.cn

Py:   asyncio.gather(*tasks)
来源：http://oi.huixinmuqiang.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wb.gzmigu.cn

JS:   await Promise.all(tasks)
来源：http://ef.huanxung.cn

TS:   await Promise.all(tasks)
来源：http://ts.jianghongdianzi.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://xn.bjjhwx.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://bp.yuexingan06.cn

Ruby: threads.map(&:join)
来源：http://ms.nicolike.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://cj.nszjky.cn

[O06] 使用进程池
来源：http://di.bjjhwx.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mc.shtwfgs.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://vz.bjjhwx.cn

JS:   // child_process / cluster 模块
来源：http://sr.panjiajie.cn

TS:   // child_process / cluster 模块
来源：http://dd.panjiajie.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ve.szxytkj.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ay.szxytkj.cn

Ruby: // fork 块
来源：http://xr.9csxet.cn

C#:   Parallel.For
来源：http://az.nszjky.cn

================================================================================
来源：http://be.bjjhwx.cn

P. 常用工具函数
来源：http://sj.newstarts.cn

================================================================================
来源：http://ph.nicolike.cn

[P01] 生成 UUID
来源：http://ie.yuexingan06.cn

Py:   str(uuid.uuid4())
来源：http://tu.lnxyls.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://bo.shtwfgs.cn

JS:   crypto.randomUUID()
来源：http://gj.yuntaijiaju.cn

TS:   crypto.randomUUID()
来源：http://dc.panjiajie.cn

Java: UUID.randomUUID().toString()
来源：http://xv.jctech888.com.cn

Go:   // 用 github.com/google/uuid
来源：http://pb.nszjky.cn

Ruby: SecureRandom.uuid
来源：http://np.huixiangedu.cn

C#:   Guid.NewGuid().ToString()
来源：http://uy.wgjwhj.cn

[P02] MD5 / SHA256 摘要
来源：http://ux.huixinmuqiang.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://fx.huixinmuqiang.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://qz.wgjwhj.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://bd.shxzskj.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://el.huanxung.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://qz.asd995.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://bb.nicolike.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ll.lnxyls.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://fr.chemitech.net.cn

[P03] 生成短随机字符串
来源：http://tc.jianghongdianzi.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://qn.huixinmuqiang.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://fb.yuntaijiaju.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xu.colortex.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vx.szxytkj.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://vp.521024.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hx.huanxung.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://cd.huixinmuqiang.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://yc.jctech888.com.cn

[P04] 求长度
来源：http://rj.jianghongdianzi.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://qb.haigaiapp.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sc.nszjky.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bn.shxzukj.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://on.bookmarksfly.cn

Java: list.size();  map.size();  s.length()
来源：http://kd.colortex.cn

Go:   len(arr);  len(m)
来源：http://sv.lnxyls.cn

Ruby: x.length;  x.size
来源：http://ct.nicolike.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://sy.nicolike.cn

[P05] 判断两个对象内容是否相等
来源：http://cy.newstarts.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://sz.huixiangedu.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://jl.hnjuh.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://uw.nszjky.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://sp.jctech888.com.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ff.newstarts.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ev.shtwfgs.cn

Ruby: a == b
来源：http://ja.yuntaijiaju.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://jb.shxzukj.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://es.wgjwhj.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ui.chemitech.net.cn

PHP:  if (empty($x)) {}
来源：http://ii.yuexingan06.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://vx.521024.cn

TS:   if (x == null) {}
来源：http://zd.newstarts.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://cd.jctech888.com.cn

Go:   if x == nil {}
来源：http://cg.lnxyls.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://lo.yuntaijiaju.cn

C#:   if (x is null) {}
来源：http://ed.lnxyls.cn

[P07] 防抖与节流
来源：http://rh.nszjky.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://vv.newstarts.cn

PHP:  // 手写时间戳比较
来源：http://uj.9csxet.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rd.lnxyls.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ac.huixinmuqiang.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://fs.lnxyls.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ok.szsharing.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://hs.panjiajie.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://bb.nszjky.cn

[P08] 处理浮点精度问题
来源：http://qk.shxzskj.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://iu.bjjhwx.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://rm.newstarts.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://tc.panjiajie.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://fi.nszjky.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://bl.nicolike.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ej.shxzukj.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://vy.szsharing.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://cv.nszjky.cn

================================================================================
来源：http://gg.huixiangedu.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://yn.haigaiapp.cn

================================================================================
来源：http://gl.9csxet.cn

[Q01] 创建表
来源：http://rl.lnxyls.cn

CREATE TABLE users (
来源：http://py.huixinmuqiang.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://gf.yuntaijiaju.cn

name VARCHAR(50) NOT NULL,
来源：http://ux.newstarts.cn

email VARCHAR(100) UNIQUE,
来源：http://dw.shtwfgs.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://bg.newstarts.cn

);
来源：http://wc.nszjky.cn

[Q02] 创建带外键的表
来源：http://ie.panjiajie.cn

CREATE TABLE orders (
来源：http://rs.huixinmuqiang.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://pp.muxihuayi.cn

user_id INT NOT NULL,
来源：http://qi.nszjky.cn

amount DECIMAL(10, 2),
来源：http://ds.chemitech.net.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://zv.colortex.cn

);
来源：http://fp.lnxyls.cn

[Q03] 增加列
来源：http://oy.huanxung.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://xj.gzmigu.cn

[Q04] 修改列类型
来源：http://xh.nszjky.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ak.9csxet.cn

[Q05] 重命名列
来源：http://sx.szxytkj.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://tv.lnxyls.cn

[Q06] 删除列
来源：http://ik.asd995.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ic.521024.cn

[Q07] 删除表
来源：http://cv.gzmigu.cn

DROP TABLE IF EXISTS orders;
来源：http://kl.muxihuayi.cn

[Q08] 创建普通索引
来源：http://cj.lnxyls.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://yk.521024.cn

[Q09] 创建唯一索引
来源：http://yi.yuntaijiaju.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ja.panjiajie.cn

[Q10] 插入单行
来源：http://td.lnxyls.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hp.shxzskj.cn

[Q11] 一次插入多行
来源：http://vo.shxzukj.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://im.colortex.cn

[Q12] 插入后取自增 ID
来源：http://ha.haigaiapp.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ql.huixiangedu.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hs.huixinmuqiang.cn

[Q13] 忽略重复插入
来源：http://hf.jctech888.com.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://xs.hahajie.cn


<!-- 参考信息 -->