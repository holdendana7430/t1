代发 wailian999

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://yr.bookmarksfly.cn

Ruby: warn "err"
来源：http://fo.muxihuayi.cn

C#:   Console.Error.WriteLine("err")
来源：http://rh.gzmigu.cn

[M07] 判断是否为主入口
来源：http://nb.colortex.cn

Py:   if __name__ == "__main__":
来源：http://er.wgjwhj.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://si.shxzukj.cn

JS:   require.main === module
来源：http://ef.shtwfgs.cn

TS:   require.main === module
来源：http://kn.haigaiapp.cn

Java: public static void main(String[] args)
来源：http://xi.yuntaijiaju.cn

Go:   func main()
来源：http://gf.szsharing.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://xr.yuntaijiaju.cn

C#:   static void Main(string[] args)
来源：http://ru.bjjhwx.cn

[M08] 获取系统与运行时信息
来源：http://vt.gzmigu.cn

Py:   platform.system();  platform.python_version()
来源：http://ed.muxihuayi.cn

PHP:  PHP_OS;  phpversion();
来源：http://yy.jctech888.com.cn

JS:   process.platform;  process.version
来源：http://ii.gzmigu.cn

TS:   process.platform;  process.version
来源：http://rc.newstarts.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mi.nicolike.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://cc.nicolike.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hg.gzmigu.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ue.hnjuh.cn

================================================================================
来源：http://vs.shxzskj.cn

N. 数据结构与算法
来源：http://sw.bookmarksfly.cn

================================================================================
来源：http://qv.jctech888.com.cn

[N01] 二分查找（有序数组）
来源：http://qn.panjiajie.cn

Py:   bisect.bisect_left(arr, x)
来源：http://cw.lnxyls.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://bz.asd995.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vm.shxzukj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hr.nicolike.cn

Java: Arrays.binarySearch(arr, x)
来源：http://nd.huixiangedu.cn

Go:   sort.SearchInts(arr, x)
来源：http://yn.nicolike.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://cy.szsharing.cn

C#:   Array.BinarySearch(arr, x)
来源：http://hv.huanxung.cn

[N02] 排序（工程实践用内置实现）
来源：http://gj.haigaiapp.cn

Py:   sorted(arr);  arr.sort()
来源：http://np.jianghongdianzi.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://gx.wgjwhj.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://nm.wgjwhj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://nn.colortex.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://eh.nicolike.cn

Go:   slices.Sort(arr)
来源：http://tw.hahajie.cn

Ruby: arr.sort
来源：http://jq.huixiangedu.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://zy.wgjwhj.cn

[N03] 快速排序（分治示例）
来源：http://ku.521024.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://xc.nicolike.cn

PHP:  // 递归实现，或用 usort
来源：http://um.9csxet.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sf.szsharing.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ob.shxzskj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://im.huixiangedu.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://lt.bookmarksfly.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mn.hahajie.cn

C#:   // 手写递归，或 Array.Sort
来源：http://cj.bjjhwx.cn

[N04] 斐波那契数列
来源：http://ag.colortex.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://sp.hahajie.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://vj.shtwfgs.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qf.nicolike.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vh.chemitech.net.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://va.hnjuh.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://yu.gzmigu.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://rc.yuexingan06.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://gy.gzmigu.cn

[N05] 最大公约数
来源：http://kf.newstarts.cn

Py:   math.gcd(a, b)
来源：http://md.huixinmuqiang.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://xc.hnjuh.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vl.yuexingan06.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jg.jctech888.com.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://sw.hahajie.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://qu.bjjhwx.cn

Ruby: a.gcd(b)
来源：http://sf.nicolike.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://vz.9csxet.cn

[N06] 判断回文字符串
来源：http://nc.wgjwhj.cn

Py:   s == s[::-1]
来源：http://jx.colortex.cn

PHP:  $s === strrev($s);
来源：http://rr.yuntaijiaju.cn

JS:   s === [...s].reverse().join("")
来源：http://di.szxytkj.cn

TS:   s === [...s].reverse().join("")
来源：http://cj.bookmarksfly.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://jv.gzmigu.cn

Go:   // 双指针从两端比较
来源：http://br.muxihuayi.cn

Ruby: s == s.reverse
来源：http://ek.jctech888.com.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://kg.panjiajie.cn

[N07] 两数之和（返回下标）
来源：http://wg.huixinmuqiang.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://it.shtwfgs.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://si.huanxung.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://rp.yuntaijiaju.cn

TS:   // 手写 Map<string, number>
来源：http://lx.yuexingan06.cn

Java: // 手写 HashMap
来源：http://lo.9csxet.cn

Go:   // 手写 map[int]int
来源：http://gn.gzmigu.cn

Ruby: // 手写 Hash
来源：http://be.huixinmuqiang.cn

C#:   // 手写 Dictionary<int, int>
来源：http://kf.huanxung.cn

[N08] 生成全排列
来源：http://uj.9csxet.cn

Py:   itertools.permutations(arr)
来源：http://mo.newstarts.cn

PHP:  // 手写递归交换
来源：http://mx.bookmarksfly.cn

JS:   // 手写回溯递归
来源：http://ln.szxytkj.cn

TS:   // 手写回溯递归
来源：http://mz.chemitech.net.cn

Java: // 手写回溯递归
来源：http://qx.jctech888.com.cn

Go:   // 手写回溯递归
来源：http://ix.gzmigu.cn

Ruby: arr.permutation.to_a
来源：http://kg.wgjwhj.cn

C#:   // 手写回溯递归
来源：http://vi.colortex.cn

[N09] 栈与队列
来源：http://jc.muxihuayi.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://nc.yuntaijiaju.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ne.newstarts.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://bz.shxzukj.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://kk.yuexingan06.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://gf.haigaiapp.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://do.9csxet.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mh.yuntaijiaju.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wr.jianghongdianzi.cn

[N10] 链表节点定义
来源：http://uj.yuntaijiaju.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://st.nszjky.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://yn.shxzukj.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wi.yuexingan06.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ix.colortex.cn

Java: class Node { int v; Node next; }
来源：http://km.szsharing.cn

Go:   type Node struct { V int; Next *Node }
来源：http://xb.nszjky.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://zm.521024.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://bx.lnxyls.cn

[N11] 二叉树中序遍历
来源：http://ho.yuexingan06.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://tf.huixiangedu.cn

PHP:  // 手写递归函数
来源：http://qz.bjjhwx.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://co.wgjwhj.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ij.nszjky.cn

Java: // 手写递归
来源：http://dy.hahajie.cn

Go:   // 手写递归
来源：http://nj.colortex.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://pi.yuntaijiaju.cn

C#:   // 手写递归
来源：http://kv.hahajie.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://bq.panjiajie.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ne.colortex.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ua.bookmarksfly.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ht.nicolike.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://oc.colortex.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://sc.jianghongdianzi.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://kv.yuexingan06.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ov.shtwfgs.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ok.yuexingan06.cn

================================================================================
来源：http://ca.shxzukj.cn

O. 并发与异步
来源：http://iq.bjjhwx.cn

================================================================================
来源：http://kr.yuexingan06.cn

[O01] 启动一个线程
来源：http://ed.bookmarksfly.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://po.newstarts.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ae.huixinmuqiang.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://pg.colortex.cn

TS:   // 同 JS
来源：http://fm.hnjuh.cn

Java: new Thread(() -> f()).start()
来源：http://bl.newstarts.cn

Go:   go f()
来源：http://og.chemitech.net.cn

Ruby: Thread.new { f }
来源：http://tt.szsharing.cn

C#:   Task.Run(() => F());
来源：http://gw.chemitech.net.cn

[O02] 使用线程池
来源：http://hx.hnjuh.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://af.jianghongdianzi.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ej.jianghongdianzi.cn

JS:   // worker_threads 线程池
来源：http://xo.shxzukj.cn

TS:   // worker_threads 线程池
来源：http://bq.panjiajie.cn

Java: Executors.newFixedThreadPool(4)
来源：http://rt.yuntaijiaju.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://by.shxzskj.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://nk.9csxet.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://jp.haigaiapp.cn

[O03] 加锁保护共享数据
来源：http://nm.jctech888.com.cn

Py:   with lock: shared += 1
来源：http://xs.521024.cn

PHP:  // 用 flock() 做文件锁
来源：http://me.huixinmuqiang.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://rl.521024.cn

TS:   // 同 JS
来源：http://jq.haigaiapp.cn

Java: synchronized (this) { shared++; }
来源：http://kk.gzmigu.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://bz.shxzukj.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://hu.jctech888.com.cn

C#:   lock (gate) { shared++; }
来源：http://wi.yuexingan06.cn

[O04] 定义异步函数并等待
来源：http://jl.newstarts.cn

Py:   async def f():⏎    await g()
来源：http://jx.haigaiapp.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://am.nszjky.cn

JS:   async function f() { await g(); }
来源：http://sn.nszjky.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://bb.szsharing.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://iq.colortex.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://rh.huanxung.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ur.panjiajie.cn

C#:   async Task F() { await G(); }
来源：http://cs.colortex.cn

[O05] 并发执行并等待全部完成
来源：http://jw.asd995.cn

Py:   asyncio.gather(*tasks)
来源：http://yy.lnxyls.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://fv.huixinmuqiang.cn

JS:   await Promise.all(tasks)
来源：http://ux.jctech888.com.cn

TS:   await Promise.all(tasks)
来源：http://po.colortex.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://cq.gzmigu.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://uw.huixinmuqiang.cn

Ruby: threads.map(&:join)
来源：http://wz.jianghongdianzi.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ea.521024.cn

[O06] 使用进程池
来源：http://oc.bookmarksfly.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://xs.jianghongdianzi.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://jj.9csxet.cn

JS:   // child_process / cluster 模块
来源：http://gm.colortex.cn

TS:   // child_process / cluster 模块
来源：http://yg.colortex.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://oa.szsharing.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://zq.haigaiapp.cn

Ruby: // fork 块
来源：http://iz.nszjky.cn

C#:   Parallel.For
来源：http://ol.yuexingan06.cn

================================================================================
来源：http://nb.haigaiapp.cn

P. 常用工具函数
来源：http://nl.wgjwhj.cn

================================================================================
来源：http://md.bjjhwx.cn

[P01] 生成 UUID
来源：http://na.huixinmuqiang.cn

Py:   str(uuid.uuid4())
来源：http://gd.hnjuh.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://te.asd995.cn

JS:   crypto.randomUUID()
来源：http://jf.lnxyls.cn

TS:   crypto.randomUUID()
来源：http://jh.shxzskj.cn

Java: UUID.randomUUID().toString()
来源：http://mt.szxytkj.cn

Go:   // 用 github.com/google/uuid
来源：http://zw.huixiangedu.cn

Ruby: SecureRandom.uuid
来源：http://jw.asd995.cn

C#:   Guid.NewGuid().ToString()
来源：http://af.hnjuh.cn

[P02] MD5 / SHA256 摘要
来源：http://gn.szxytkj.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://qb.yuexingan06.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://qk.chemitech.net.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://yo.panjiajie.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://oc.shtwfgs.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ut.asd995.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://lt.jctech888.com.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://jn.hnjuh.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://zg.bjjhwx.cn

[P03] 生成短随机字符串
来源：http://ot.wgjwhj.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://xj.szsharing.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://to.szsharing.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://so.yuexingan06.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ef.hahajie.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wx.szxytkj.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://rl.newstarts.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://vl.szsharing.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://bt.yuexingan06.cn

[P04] 求长度
来源：http://wm.shxzskj.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://px.bookmarksfly.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ry.shxzukj.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wt.shtwfgs.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cq.hahajie.cn

Java: list.size();  map.size();  s.length()
来源：http://js.jctech888.com.cn

Go:   len(arr);  len(m)
来源：http://zl.nszjky.cn

Ruby: x.length;  x.size
来源：http://fj.wgjwhj.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://xt.shtwfgs.cn

[P05] 判断两个对象内容是否相等
来源：http://zp.asd995.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ee.lnxyls.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ik.huanxung.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hq.hahajie.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://no.haigaiapp.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://iw.chemitech.net.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ot.yuntaijiaju.cn

Ruby: a == b
来源：http://je.shxzukj.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://qx.haigaiapp.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ms.bjjhwx.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ey.muxihuayi.cn

PHP:  if (empty($x)) {}
来源：http://mc.panjiajie.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://jd.colortex.cn

TS:   if (x == null) {}
来源：http://hi.shxzskj.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://up.shtwfgs.cn

Go:   if x == nil {}
来源：http://gi.yuntaijiaju.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://za.haigaiapp.cn

C#:   if (x is null) {}
来源：http://iv.panjiajie.cn

[P07] 防抖与节流
来源：http://xa.newstarts.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ko.nszjky.cn

PHP:  // 手写时间戳比较
来源：http://hi.yuntaijiaju.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kv.yuntaijiaju.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nz.shxzukj.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://jo.newstarts.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ab.shxzukj.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://rx.shxzskj.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ow.newstarts.cn

[P08] 处理浮点精度问题
来源：http://go.nszjky.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ha.szsharing.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hn.nicolike.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://cc.szsharing.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://yr.nicolike.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://nu.hnjuh.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://us.9csxet.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://or.bjjhwx.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://sy.szxytkj.cn

================================================================================
来源：http://mn.bookmarksfly.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://cc.panjiajie.cn

================================================================================
来源：http://na.bookmarksfly.cn

[Q01] 创建表
来源：http://uo.wgjwhj.cn

CREATE TABLE users (
来源：http://jc.huixiangedu.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://qw.muxihuayi.cn

name VARCHAR(50) NOT NULL,
来源：http://ed.asd995.cn

email VARCHAR(100) UNIQUE,
来源：http://hy.huanxung.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://tb.hahajie.cn

);
来源：http://qu.muxihuayi.cn

[Q02] 创建带外键的表
来源：http://od.gzmigu.cn

CREATE TABLE orders (
来源：http://me.wgjwhj.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://qa.chemitech.net.cn

user_id INT NOT NULL,
来源：http://hh.huixiangedu.cn

amount DECIMAL(10, 2),
来源：http://iq.9csxet.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://rd.panjiajie.cn

);
来源：http://zf.nicolike.cn

[Q03] 增加列
来源：http://uo.muxihuayi.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://gs.521024.cn

[Q04] 修改列类型
来源：http://hn.huixiangedu.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ae.shxzukj.cn

[Q05] 重命名列
来源：http://ou.huanxung.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ln.nicolike.cn

[Q06] 删除列
来源：http://rb.huanxung.cn

ALTER TABLE users DROP COLUMN age;
来源：http://xk.gzmigu.cn

[Q07] 删除表
来源：http://me.nszjky.cn

DROP TABLE IF EXISTS orders;
来源：http://eg.jianghongdianzi.cn

[Q08] 创建普通索引
来源：http://ce.bjjhwx.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://yu.521024.cn

[Q09] 创建唯一索引
来源：http://ed.asd995.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://qm.huanxung.cn

[Q10] 插入单行
来源：http://df.yuexingan06.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://bx.chemitech.net.cn

[Q11] 一次插入多行
来源：http://nu.521024.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ix.wgjwhj.cn

[Q12] 插入后取自增 ID
来源：http://gq.muxihuayi.cn


<!-- 参考信息 -->