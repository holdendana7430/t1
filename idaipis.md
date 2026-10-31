代发 wailian999

Java: public static void main(String[] args)
来源：http://ly.521024.cn

Go:   func main()
来源：http://fn.bjjhwx.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://sd.huanxung.cn

C#:   static void Main(string[] args)
来源：http://zo.9csxet.cn

[M08] 获取系统与运行时信息
来源：http://ag.gzmigu.cn

Py:   platform.system();  platform.python_version()
来源：http://ll.bjjhwx.cn

PHP:  PHP_OS;  phpversion();
来源：http://rx.521024.cn

JS:   process.platform;  process.version
来源：http://xe.shxzskj.cn

TS:   process.platform;  process.version
来源：http://en.shxzskj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://bk.nicolike.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://sz.chemitech.net.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://dy.muxihuayi.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ox.nszjky.cn

================================================================================
来源：http://wm.huixinmuqiang.cn

N. 数据结构与算法
来源：http://az.huixinmuqiang.cn

================================================================================
来源：http://lv.newstarts.cn

[N01] 二分查找（有序数组）
来源：http://tr.muxihuayi.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ki.yuntaijiaju.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://fe.nszjky.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dk.chemitech.net.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fc.gzmigu.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ne.bjjhwx.cn

Go:   sort.SearchInts(arr, x)
来源：http://qh.szxytkj.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://uu.asd995.cn

C#:   Array.BinarySearch(arr, x)
来源：http://av.haigaiapp.cn

[N02] 排序（工程实践用内置实现）
来源：http://rs.huixiangedu.cn

Py:   sorted(arr);  arr.sort()
来源：http://vj.chemitech.net.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://cv.huixinmuqiang.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://kt.bjjhwx.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://vp.bookmarksfly.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://fl.jctech888.com.cn

Go:   slices.Sort(arr)
来源：http://lu.huanxung.cn

Ruby: arr.sort
来源：http://et.yuntaijiaju.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://np.shxzukj.cn

[N03] 快速排序（分治示例）
来源：http://us.chemitech.net.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://qf.huanxung.cn

PHP:  // 递归实现，或用 usort
来源：http://gn.szxytkj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rm.lnxyls.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://iw.huixiangedu.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ov.yuntaijiaju.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://zy.shxzskj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ni.szsharing.cn

C#:   // 手写递归，或 Array.Sort
来源：http://fg.huixinmuqiang.cn

[N04] 斐波那契数列
来源：http://sv.shxzskj.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://gp.colortex.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://zj.chemitech.net.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ns.gzmigu.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bg.hahajie.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://sh.huanxung.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://xl.shtwfgs.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://or.jianghongdianzi.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://xz.szsharing.cn

[N05] 最大公约数
来源：http://ei.shtwfgs.cn

Py:   math.gcd(a, b)
来源：http://ue.chemitech.net.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://nu.shtwfgs.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cf.colortex.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bn.shxzukj.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://dz.szsharing.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ge.lnxyls.cn

Ruby: a.gcd(b)
来源：http://kw.haigaiapp.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ic.jianghongdianzi.cn

[N06] 判断回文字符串
来源：http://vj.hahajie.cn

Py:   s == s[::-1]
来源：http://qz.colortex.cn

PHP:  $s === strrev($s);
来源：http://ok.jianghongdianzi.cn

JS:   s === [...s].reverse().join("")
来源：http://kj.colortex.cn

TS:   s === [...s].reverse().join("")
来源：http://nw.huanxung.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://tg.nszjky.cn

Go:   // 双指针从两端比较
来源：http://by.asd995.cn

Ruby: s == s.reverse
来源：http://wi.colortex.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://rj.yuntaijiaju.cn

[N07] 两数之和（返回下标）
来源：http://pn.wgjwhj.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://eg.huixiangedu.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://kd.hnjuh.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://mb.haigaiapp.cn

TS:   // 手写 Map<string, number>
来源：http://ae.nicolike.cn

Java: // 手写 HashMap
来源：http://jc.yuexingan06.cn

Go:   // 手写 map[int]int
来源：http://ak.gzmigu.cn

Ruby: // 手写 Hash
来源：http://fd.panjiajie.cn

C#:   // 手写 Dictionary<int, int>
来源：http://xj.gzmigu.cn

[N08] 生成全排列
来源：http://gj.nicolike.cn

Py:   itertools.permutations(arr)
来源：http://lc.chemitech.net.cn

PHP:  // 手写递归交换
来源：http://rw.newstarts.cn

JS:   // 手写回溯递归
来源：http://ju.muxihuayi.cn

TS:   // 手写回溯递归
来源：http://mp.jctech888.com.cn

Java: // 手写回溯递归
来源：http://em.huixinmuqiang.cn

Go:   // 手写回溯递归
来源：http://kq.9csxet.cn

Ruby: arr.permutation.to_a
来源：http://kb.newstarts.cn

C#:   // 手写回溯递归
来源：http://cx.hahajie.cn

[N09] 栈与队列
来源：http://xd.jianghongdianzi.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ng.lnxyls.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://al.jctech888.com.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://bo.asd995.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://kj.huixinmuqiang.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://dr.asd995.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://xf.bjjhwx.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://by.yuntaijiaju.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ox.newstarts.cn

[N10] 链表节点定义
来源：http://hw.nicolike.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.lnxyls.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://rq.huixiangedu.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ai.huanxung.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ps.hahajie.cn

Java: class Node { int v; Node next; }
来源：http://ba.huixinmuqiang.cn

Go:   type Node struct { V int; Next *Node }
来源：http://xs.newstarts.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://im.huixinmuqiang.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://vg.haigaiapp.cn

[N11] 二叉树中序遍历
来源：http://zd.panjiajie.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mo.hahajie.cn

PHP:  // 手写递归函数
来源：http://ac.huixinmuqiang.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ab.yuexingan06.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ym.hahajie.cn

Java: // 手写递归
来源：http://te.yuexingan06.cn

Go:   // 手写递归
来源：http://pe.asd995.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://qk.hahajie.cn

C#:   // 手写递归
来源：http://gt.yuexingan06.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://zk.hahajie.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://dl.newstarts.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://cz.szxytkj.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pm.huanxung.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://us.asd995.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ic.nicolike.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://nw.shtwfgs.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://bf.haigaiapp.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://yk.panjiajie.cn

================================================================================
来源：http://yg.huixiangedu.cn

O. 并发与异步
来源：http://pz.gzmigu.cn

================================================================================
来源：http://qy.wgjwhj.cn

[O01] 启动一个线程
来源：http://kd.wgjwhj.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hq.szsharing.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://sb.szsharing.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://rk.muxihuayi.cn

TS:   // 同 JS
来源：http://cq.gzmigu.cn

Java: new Thread(() -> f()).start()
来源：http://dm.newstarts.cn

Go:   go f()
来源：http://nn.shxzskj.cn

Ruby: Thread.new { f }
来源：http://wa.chemitech.net.cn

C#:   Task.Run(() => F());
来源：http://le.asd995.cn

[O02] 使用线程池
来源：http://cq.huanxung.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://iu.jianghongdianzi.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://xu.521024.cn

JS:   // worker_threads 线程池
来源：http://wd.szxytkj.cn

TS:   // worker_threads 线程池
来源：http://lc.huixinmuqiang.cn

Java: Executors.newFixedThreadPool(4)
来源：http://xt.521024.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://yz.bookmarksfly.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://fk.huanxung.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wy.huanxung.cn

[O03] 加锁保护共享数据
来源：http://sx.szsharing.cn

Py:   with lock: shared += 1
来源：http://ms.panjiajie.cn

PHP:  // 用 flock() 做文件锁
来源：http://wo.bjjhwx.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mp.muxihuayi.cn

TS:   // 同 JS
来源：http://oc.huixinmuqiang.cn

Java: synchronized (this) { shared++; }
来源：http://qt.nicolike.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://cq.huixiangedu.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://jo.huixinmuqiang.cn

C#:   lock (gate) { shared++; }
来源：http://bn.nicolike.cn

[O04] 定义异步函数并等待
来源：http://vo.huixiangedu.cn

Py:   async def f():⏎    await g()
来源：http://dy.9csxet.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ao.huixinmuqiang.cn

JS:   async function f() { await g(); }
来源：http://tv.521024.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://pc.huanxung.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://li.yuexingan06.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ns.jctech888.com.cn

Ruby: # 用 Fiber 或 async gem
来源：http://wu.lnxyls.cn

C#:   async Task F() { await G(); }
来源：http://jb.wgjwhj.cn

[O05] 并发执行并等待全部完成
来源：http://tz.huixinmuqiang.cn

Py:   asyncio.gather(*tasks)
来源：http://vv.shtwfgs.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ip.newstarts.cn

JS:   await Promise.all(tasks)
来源：http://qd.gzmigu.cn

TS:   await Promise.all(tasks)
来源：http://pg.szsharing.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wi.jianghongdianzi.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ze.huixiangedu.cn

Ruby: threads.map(&:join)
来源：http://tk.asd995.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ut.panjiajie.cn

[O06] 使用进程池
来源：http://ej.colortex.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://rw.bjjhwx.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://mx.hnjuh.cn

JS:   // child_process / cluster 模块
来源：http://su.jctech888.com.cn

TS:   // child_process / cluster 模块
来源：http://tw.yuexingan06.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://dh.yuexingan06.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://vw.haigaiapp.cn

Ruby: // fork 块
来源：http://jb.gzmigu.cn

C#:   Parallel.For
来源：http://ez.newstarts.cn

================================================================================
来源：http://tg.jctech888.com.cn

P. 常用工具函数
来源：http://wf.muxihuayi.cn

================================================================================
来源：http://km.haigaiapp.cn

[P01] 生成 UUID
来源：http://nq.panjiajie.cn

Py:   str(uuid.uuid4())
来源：http://mq.huixinmuqiang.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://sj.bjjhwx.cn

JS:   crypto.randomUUID()
来源：http://kt.9csxet.cn

TS:   crypto.randomUUID()
来源：http://bq.chemitech.net.cn

Java: UUID.randomUUID().toString()
来源：http://an.newstarts.cn

Go:   // 用 github.com/google/uuid
来源：http://bo.huixiangedu.cn

Ruby: SecureRandom.uuid
来源：http://uy.jctech888.com.cn

C#:   Guid.NewGuid().ToString()
来源：http://rg.yuntaijiaju.cn

[P02] MD5 / SHA256 摘要
来源：http://tp.panjiajie.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://gr.muxihuayi.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://gu.bookmarksfly.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://un.szxytkj.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ay.hahajie.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ah.colortex.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://sz.shxzukj.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ge.huixiangedu.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://gv.haigaiapp.cn

[P03] 生成短随机字符串
来源：http://ey.hahajie.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://gb.newstarts.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ml.muxihuayi.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zh.9csxet.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rl.wgjwhj.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://kt.yuntaijiaju.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ax.lnxyls.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ol.haigaiapp.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://gy.haigaiapp.cn

[P04] 求长度
来源：http://pp.panjiajie.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mg.gzmigu.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cj.szxytkj.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mv.huixinmuqiang.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lw.chemitech.net.cn

Java: list.size();  map.size();  s.length()
来源：http://pk.panjiajie.cn

Go:   len(arr);  len(m)
来源：http://ln.huanxung.cn

Ruby: x.length;  x.size
来源：http://ek.colortex.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ll.bjjhwx.cn

[P05] 判断两个对象内容是否相等
来源：http://mc.shtwfgs.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://tu.muxihuayi.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://vx.panjiajie.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://iu.9csxet.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://kn.hnjuh.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://dc.9csxet.cn

Go:   reflect.DeepEqual(a, b)
来源：http://jb.newstarts.cn

Ruby: a == b
来源：http://bc.jianghongdianzi.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://lc.nicolike.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://xp.hnjuh.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://fz.haigaiapp.cn

PHP:  if (empty($x)) {}
来源：http://mj.shxzukj.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://di.nicolike.cn

TS:   if (x == null) {}
来源：http://zf.shxzskj.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://us.shtwfgs.cn

Go:   if x == nil {}
来源：http://ki.szxytkj.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://om.521024.cn

C#:   if (x is null) {}
来源：http://el.9csxet.cn

[P07] 防抖与节流
来源：http://ub.jctech888.com.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://xf.newstarts.cn

PHP:  // 手写时间戳比较
来源：http://yq.shtwfgs.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://go.lnxyls.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xc.panjiajie.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://gw.jianghongdianzi.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://xy.hahajie.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://qv.nicolike.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://qm.nicolike.cn

[P08] 处理浮点精度问题
来源：http://vt.huixinmuqiang.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hg.9csxet.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://rf.huixiangedu.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://tl.yuntaijiaju.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://oe.nszjky.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://nv.shxzskj.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://nl.shtwfgs.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ns.szsharing.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://on.muxihuayi.cn

================================================================================
来源：http://gk.jianghongdianzi.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://yu.shxzukj.cn

================================================================================
来源：http://qb.nicolike.cn

[Q01] 创建表
来源：http://wr.wgjwhj.cn

CREATE TABLE users (
来源：http://by.colortex.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://xz.huixiangedu.cn

name VARCHAR(50) NOT NULL,
来源：http://xr.panjiajie.cn

email VARCHAR(100) UNIQUE,
来源：http://gq.chemitech.net.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://yu.huanxung.cn

);
来源：http://br.nszjky.cn

[Q02] 创建带外键的表
来源：http://hg.lnxyls.cn

CREATE TABLE orders (
来源：http://pr.521024.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://xj.newstarts.cn

user_id INT NOT NULL,
来源：http://bw.bookmarksfly.cn

amount DECIMAL(10, 2),
来源：http://sg.yuntaijiaju.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://jo.lnxyls.cn

);
来源：http://wn.shxzukj.cn

[Q03] 增加列
来源：http://jk.jianghongdianzi.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://zy.chemitech.net.cn

[Q04] 修改列类型
来源：http://nc.gzmigu.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://xj.huixiangedu.cn

[Q05] 重命名列
来源：http://jo.huixinmuqiang.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://yy.shxzukj.cn

[Q06] 删除列
来源：http://cv.nicolike.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ur.szxytkj.cn

[Q07] 删除表
来源：http://pa.hnjuh.cn

DROP TABLE IF EXISTS orders;
来源：http://bc.wgjwhj.cn

[Q08] 创建普通索引
来源：http://bt.nszjky.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://qa.newstarts.cn

[Q09] 创建唯一索引
来源：http://jr.nicolike.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://qs.szsharing.cn

[Q10] 插入单行
来源：http://fj.szxytkj.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://vd.bookmarksfly.cn

[Q11] 一次插入多行
来源：http://rl.jctech888.com.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hy.shtwfgs.cn

[Q12] 插入后取自增 ID
来源：http://gw.wgjwhj.cn

INSERT INTO users (name) VALUES ('C');
来源：http://pe.shxzukj.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://rw.yuexingan06.cn

[Q13] 忽略重复插入
来源：http://cn.shxzskj.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://oo.9csxet.cn

[Q14] 存在则更新（upsert）
来源：http://lk.bjjhwx.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ub.bookmarksfly.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://uh.bookmarksfly.cn

[Q15] 查询全部
来源：http://ek.huixiangedu.cn


<!-- 参考信息 -->