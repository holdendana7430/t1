代发 wailian999

Py:   if __name__ == "__main__":
来源：http://xc.huanxung.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://lu.bjjhwx.cn

JS:   require.main === module
来源：http://et.nszjky.cn

TS:   require.main === module
来源：http://sq.bjjhwx.cn

Java: public static void main(String[] args)
来源：http://dr.panjiajie.cn

Go:   func main()
来源：http://im.szsharing.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://eb.jctech888.com.cn

C#:   static void Main(string[] args)
来源：http://li.huixiangedu.cn

[M08] 获取系统与运行时信息
来源：http://to.huixiangedu.cn

Py:   platform.system();  platform.python_version()
来源：http://yc.huixinmuqiang.cn

PHP:  PHP_OS;  phpversion();
来源：http://nr.colortex.cn

JS:   process.platform;  process.version
来源：http://an.haigaiapp.cn

TS:   process.platform;  process.version
来源：http://uc.muxihuayi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ny.asd995.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://gr.nicolike.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://uj.huixinmuqiang.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://lv.huixiangedu.cn

================================================================================
来源：http://ok.shxzskj.cn

N. 数据结构与算法
来源：http://oe.lnxyls.cn

================================================================================
来源：http://dj.shxzskj.cn

[N01] 二分查找（有序数组）
来源：http://ba.jctech888.com.cn

Py:   bisect.bisect_left(arr, x)
来源：http://sr.panjiajie.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://jw.shxzskj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hh.9csxet.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kd.shtwfgs.cn

Java: Arrays.binarySearch(arr, x)
来源：http://lu.huanxung.cn

Go:   sort.SearchInts(arr, x)
来源：http://cj.wgjwhj.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://jh.panjiajie.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ww.jianghongdianzi.cn

[N02] 排序（工程实践用内置实现）
来源：http://mq.newstarts.cn

Py:   sorted(arr);  arr.sort()
来源：http://hz.wgjwhj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://qm.huixinmuqiang.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://uf.yuexingan06.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://gd.nicolike.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://qp.szsharing.cn

Go:   slices.Sort(arr)
来源：http://lt.nszjky.cn

Ruby: arr.sort
来源：http://sf.lnxyls.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://hi.szxytkj.cn

[N03] 快速排序（分治示例）
来源：http://wv.bookmarksfly.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://sn.haigaiapp.cn

PHP:  // 递归实现，或用 usort
来源：http://vs.hahajie.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mm.szxytkj.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qi.nicolike.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://cf.yuntaijiaju.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://vt.panjiajie.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://bu.wgjwhj.cn

C#:   // 手写递归，或 Array.Sort
来源：http://jm.szxytkj.cn

[N04] 斐波那契数列
来源：http://am.haigaiapp.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wx.colortex.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://cv.nszjky.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rs.hahajie.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sh.yuexingan06.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mu.muxihuayi.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://li.bookmarksfly.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wz.colortex.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ye.521024.cn

[N05] 最大公约数
来源：http://wy.9csxet.cn

Py:   math.gcd(a, b)
来源：http://vo.9csxet.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://co.521024.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cj.hnjuh.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xm.shxzukj.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://jy.hnjuh.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://gr.521024.cn

Ruby: a.gcd(b)
来源：http://cm.bookmarksfly.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://vl.szxytkj.cn

[N06] 判断回文字符串
来源：http://hn.gzmigu.cn

Py:   s == s[::-1]
来源：http://fd.szsharing.cn

PHP:  $s === strrev($s);
来源：http://sz.nicolike.cn

JS:   s === [...s].reverse().join("")
来源：http://ef.colortex.cn

TS:   s === [...s].reverse().join("")
来源：http://tj.yuntaijiaju.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xb.haigaiapp.cn

Go:   // 双指针从两端比较
来源：http://un.muxihuayi.cn

Ruby: s == s.reverse
来源：http://yy.nszjky.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://mt.panjiajie.cn

[N07] 两数之和（返回下标）
来源：http://vw.haigaiapp.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://it.shxzukj.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mg.huixiangedu.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://vv.chemitech.net.cn

TS:   // 手写 Map<string, number>
来源：http://tn.shxzskj.cn

Java: // 手写 HashMap
来源：http://bv.bookmarksfly.cn

Go:   // 手写 map[int]int
来源：http://fs.muxihuayi.cn

Ruby: // 手写 Hash
来源：http://fj.asd995.cn

C#:   // 手写 Dictionary<int, int>
来源：http://bh.huixinmuqiang.cn

[N08] 生成全排列
来源：http://rm.yuexingan06.cn

Py:   itertools.permutations(arr)
来源：http://za.jianghongdianzi.cn

PHP:  // 手写递归交换
来源：http://qr.hahajie.cn

JS:   // 手写回溯递归
来源：http://yz.huixiangedu.cn

TS:   // 手写回溯递归
来源：http://un.szxytkj.cn

Java: // 手写回溯递归
来源：http://cf.haigaiapp.cn

Go:   // 手写回溯递归
来源：http://hx.yuntaijiaju.cn

Ruby: arr.permutation.to_a
来源：http://gs.newstarts.cn

C#:   // 手写回溯递归
来源：http://kf.lnxyls.cn

[N09] 栈与队列
来源：http://ov.nszjky.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://yk.huixiangedu.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://dc.nicolike.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://km.bjjhwx.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ou.shxzskj.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://gl.szxytkj.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ko.nicolike.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mm.jctech888.com.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://qc.shxzukj.cn

[N10] 链表节点定义
来源：http://fo.szxytkj.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://zg.szsharing.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://zs.yuexingan06.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://oo.bjjhwx.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://fm.muxihuayi.cn

Java: class Node { int v; Node next; }
来源：http://fw.muxihuayi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://gn.nicolike.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://bk.haigaiapp.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ad.lnxyls.cn

[N11] 二叉树中序遍历
来源：http://ri.nicolike.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://qn.colortex.cn

PHP:  // 手写递归函数
来源：http://bt.gzmigu.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://na.wgjwhj.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pr.gzmigu.cn

Java: // 手写递归
来源：http://et.huixiangedu.cn

Go:   // 手写递归
来源：http://vu.shxzskj.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://jt.nicolike.cn

C#:   // 手写递归
来源：http://yz.shxzukj.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://nu.hnjuh.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mz.newstarts.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://id.9csxet.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wu.panjiajie.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://my.asd995.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ht.shxzskj.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://bt.jctech888.com.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://pd.muxihuayi.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://xd.hahajie.cn

================================================================================
来源：http://mb.gzmigu.cn

O. 并发与异步
来源：http://ip.nszjky.cn

================================================================================
来源：http://rs.yuntaijiaju.cn

[O01] 启动一个线程
来源：http://fj.chemitech.net.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://iv.hnjuh.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://pt.newstarts.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://vq.9csxet.cn

TS:   // 同 JS
来源：http://mw.521024.cn

Java: new Thread(() -> f()).start()
来源：http://mh.panjiajie.cn

Go:   go f()
来源：http://yo.yuexingan06.cn

Ruby: Thread.new { f }
来源：http://ur.hnjuh.cn

C#:   Task.Run(() => F());
来源：http://ql.521024.cn

[O02] 使用线程池
来源：http://ac.shtwfgs.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ag.shxzskj.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://kr.bookmarksfly.cn

JS:   // worker_threads 线程池
来源：http://ut.521024.cn

TS:   // worker_threads 线程池
来源：http://rr.bjjhwx.cn

Java: Executors.newFixedThreadPool(4)
来源：http://sg.yuntaijiaju.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://vr.muxihuayi.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://lu.shxzskj.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://vi.szsharing.cn

[O03] 加锁保护共享数据
来源：http://kq.szsharing.cn

Py:   with lock: shared += 1
来源：http://px.gzmigu.cn

PHP:  // 用 flock() 做文件锁
来源：http://ky.huixinmuqiang.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ur.haigaiapp.cn

TS:   // 同 JS
来源：http://qi.yuntaijiaju.cn

Java: synchronized (this) { shared++; }
来源：http://kt.shtwfgs.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://fu.yuntaijiaju.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://df.yuntaijiaju.cn

C#:   lock (gate) { shared++; }
来源：http://zh.hahajie.cn

[O04] 定义异步函数并等待
来源：http://pi.shxzukj.cn

Py:   async def f():⏎    await g()
来源：http://ai.panjiajie.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://an.521024.cn

JS:   async function f() { await g(); }
来源：http://xu.colortex.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://od.9csxet.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://rj.jctech888.com.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://eb.szxytkj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://pb.szsharing.cn

C#:   async Task F() { await G(); }
来源：http://sm.wgjwhj.cn

[O05] 并发执行并等待全部完成
来源：http://am.huixinmuqiang.cn

Py:   asyncio.gather(*tasks)
来源：http://ho.jianghongdianzi.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://xl.shxzukj.cn

JS:   await Promise.all(tasks)
来源：http://iu.colortex.cn

TS:   await Promise.all(tasks)
来源：http://ex.haigaiapp.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://bj.newstarts.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://sj.haigaiapp.cn

Ruby: threads.map(&:join)
来源：http://wy.yuexingan06.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ad.asd995.cn

[O06] 使用进程池
来源：http://zo.chemitech.net.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://pv.jianghongdianzi.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ev.hahajie.cn

JS:   // child_process / cluster 模块
来源：http://gx.jctech888.com.cn

TS:   // child_process / cluster 模块
来源：http://to.colortex.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ns.shxzukj.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://uy.haigaiapp.cn

Ruby: // fork 块
来源：http://tn.szsharing.cn

C#:   Parallel.For
来源：http://rt.huanxung.cn

================================================================================
来源：http://vt.jctech888.com.cn

P. 常用工具函数
来源：http://si.jianghongdianzi.cn

================================================================================
来源：http://cs.newstarts.cn

[P01] 生成 UUID
来源：http://oj.bookmarksfly.cn

Py:   str(uuid.uuid4())
来源：http://bt.huanxung.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://pw.521024.cn

JS:   crypto.randomUUID()
来源：http://lm.huixiangedu.cn

TS:   crypto.randomUUID()
来源：http://sr.muxihuayi.cn

Java: UUID.randomUUID().toString()
来源：http://oh.yuexingan06.cn

Go:   // 用 github.com/google/uuid
来源：http://vu.hnjuh.cn

Ruby: SecureRandom.uuid
来源：http://nl.9csxet.cn

C#:   Guid.NewGuid().ToString()
来源：http://ul.bookmarksfly.cn

[P02] MD5 / SHA256 摘要
来源：http://st.szxytkj.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://rb.szsharing.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://vl.huixiangedu.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://zr.hahajie.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://qq.newstarts.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://uu.hahajie.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://im.yuntaijiaju.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://jw.shxzskj.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://oz.panjiajie.cn

[P03] 生成短随机字符串
来源：http://pp.bjjhwx.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ui.asd995.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://lg.yuntaijiaju.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tp.haigaiapp.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jv.huixinmuqiang.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ag.bjjhwx.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://np.colortex.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://vn.szxytkj.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ru.shtwfgs.cn

[P04] 求长度
来源：http://ce.nicolike.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hx.521024.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jn.nicolike.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zq.9csxet.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ar.bookmarksfly.cn

Java: list.size();  map.size();  s.length()
来源：http://er.shxzskj.cn

Go:   len(arr);  len(m)
来源：http://gx.hahajie.cn

Ruby: x.length;  x.size
来源：http://zi.jctech888.com.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://bt.9csxet.cn

[P05] 判断两个对象内容是否相等
来源：http://pf.shtwfgs.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ys.muxihuayi.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://kl.lnxyls.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ug.huixiangedu.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://lk.jctech888.com.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://dc.muxihuayi.cn

Go:   reflect.DeepEqual(a, b)
来源：http://lb.huanxung.cn

Ruby: a == b
来源：http://ys.jianghongdianzi.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://xs.szsharing.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hd.chemitech.net.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://md.yuexingan06.cn

PHP:  if (empty($x)) {}
来源：http://mw.shtwfgs.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wt.yuntaijiaju.cn

TS:   if (x == null) {}
来源：http://je.yuntaijiaju.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://eu.szsharing.cn

Go:   if x == nil {}
来源：http://lc.huixiangedu.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ff.9csxet.cn

C#:   if (x is null) {}
来源：http://je.jianghongdianzi.cn

[P07] 防抖与节流
来源：http://mh.bjjhwx.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://jv.hnjuh.cn

PHP:  // 手写时间戳比较
来源：http://rq.muxihuayi.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sl.lnxyls.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mj.wgjwhj.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://jq.huixinmuqiang.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mr.jianghongdianzi.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://bg.szxytkj.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wt.huixiangedu.cn

[P08] 处理浮点精度问题
来源：http://oe.jianghongdianzi.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://nh.shxzukj.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://io.hnjuh.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ep.chemitech.net.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://tw.yuntaijiaju.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://uy.szxytkj.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://lz.shtwfgs.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ka.9csxet.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://gt.colortex.cn

================================================================================
来源：http://sh.szxytkj.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ix.lnxyls.cn

================================================================================
来源：http://bw.huixiangedu.cn

[Q01] 创建表
来源：http://sr.newstarts.cn

CREATE TABLE users (
来源：http://vq.newstarts.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://zh.521024.cn

name VARCHAR(50) NOT NULL,
来源：http://ve.muxihuayi.cn

email VARCHAR(100) UNIQUE,
来源：http://fe.szxytkj.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wa.bookmarksfly.cn

);
来源：http://zs.nicolike.cn

[Q02] 创建带外键的表
来源：http://as.wgjwhj.cn

CREATE TABLE orders (
来源：http://cr.hahajie.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ck.shxzskj.cn

user_id INT NOT NULL,
来源：http://ah.yuntaijiaju.cn

amount DECIMAL(10, 2),
来源：http://er.colortex.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://sl.yuexingan06.cn

);
来源：http://xw.haigaiapp.cn

[Q03] 增加列
来源：http://xc.521024.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ga.muxihuayi.cn

[Q04] 修改列类型
来源：http://fn.gzmigu.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://kd.asd995.cn

[Q05] 重命名列
来源：http://fm.colortex.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://lc.colortex.cn

[Q06] 删除列
来源：http://ay.gzmigu.cn

ALTER TABLE users DROP COLUMN age;
来源：http://rm.huixiangedu.cn

[Q07] 删除表
来源：http://dg.yuntaijiaju.cn

DROP TABLE IF EXISTS orders;
来源：http://ht.hahajie.cn

[Q08] 创建普通索引
来源：http://jv.9csxet.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://wq.yuexingan06.cn

[Q09] 创建唯一索引
来源：http://uj.szxytkj.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ne.jianghongdianzi.cn

[Q10] 插入单行
来源：http://xu.szxytkj.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ts.bookmarksfly.cn

[Q11] 一次插入多行
来源：http://wm.huixiangedu.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://dv.shxzskj.cn

[Q12] 插入后取自增 ID
来源：http://qq.nicolike.cn

INSERT INTO users (name) VALUES ('C');
来源：http://xf.muxihuayi.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://sp.nszjky.cn

[Q13] 忽略重复插入
来源：http://tc.yuntaijiaju.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wq.gzmigu.cn


<!-- 参考信息 -->