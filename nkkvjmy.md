代发 wailian999

Ruby: exit 1
来源：http://ir.jianghongdianzi.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://tv.gzmigu.cn

[M06] 向标准错误输出
来源：http://kp.hnjuh.cn

Py:   print("err", file=sys.stderr)
来源：http://uu.gzmigu.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://uj.gzmigu.cn

JS:   console.error("err")
来源：http://hv.yuntaijiaju.cn

TS:   console.error("err")
来源：http://dm.newstarts.cn

Java: System.err.println("err")
来源：http://kq.hnjuh.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://li.huanxung.cn

Ruby: warn "err"
来源：http://ls.yuexingan06.cn

C#:   Console.Error.WriteLine("err")
来源：http://xc.jianghongdianzi.cn

[M07] 判断是否为主入口
来源：http://vv.panjiajie.cn

Py:   if __name__ == "__main__":
来源：http://av.szsharing.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://rr.shxzukj.cn

JS:   require.main === module
来源：http://an.muxihuayi.cn

TS:   require.main === module
来源：http://ux.bjjhwx.cn

Java: public static void main(String[] args)
来源：http://vx.bjjhwx.cn

Go:   func main()
来源：http://wb.gzmigu.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://fk.nicolike.cn

C#:   static void Main(string[] args)
来源：http://si.bookmarksfly.cn

[M08] 获取系统与运行时信息
来源：http://nm.bookmarksfly.cn

Py:   platform.system();  platform.python_version()
来源：http://bn.shxzukj.cn

PHP:  PHP_OS;  phpversion();
来源：http://sz.yuexingan06.cn

JS:   process.platform;  process.version
来源：http://ld.szsharing.cn

TS:   process.platform;  process.version
来源：http://hv.huixiangedu.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://zh.hnjuh.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ln.shxzskj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mv.colortex.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://lp.shxzskj.cn

================================================================================
来源：http://kx.jctech888.com.cn

N. 数据结构与算法
来源：http://rp.shxzskj.cn

================================================================================
来源：http://wm.hnjuh.cn

[N01] 二分查找（有序数组）
来源：http://te.jctech888.com.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ni.nicolike.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wn.gzmigu.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sy.bookmarksfly.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gz.nicolike.cn

Java: Arrays.binarySearch(arr, x)
来源：http://hx.9csxet.cn

Go:   sort.SearchInts(arr, x)
来源：http://ty.521024.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://yg.bjjhwx.cn

C#:   Array.BinarySearch(arr, x)
来源：http://sl.shxzukj.cn

[N02] 排序（工程实践用内置实现）
来源：http://ha.jctech888.com.cn

Py:   sorted(arr);  arr.sort()
来源：http://ey.jianghongdianzi.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://fd.hahajie.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://fn.shxzukj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ge.newstarts.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://uv.panjiajie.cn

Go:   slices.Sort(arr)
来源：http://sz.521024.cn

Ruby: arr.sort
来源：http://up.szxytkj.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://oo.hahajie.cn

[N03] 快速排序（分治示例）
来源：http://wv.9csxet.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ce.wgjwhj.cn

PHP:  // 递归实现，或用 usort
来源：http://cq.jctech888.com.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ni.huixiangedu.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pl.shxzukj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://fk.hnjuh.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ks.asd995.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://qz.huixiangedu.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ln.nicolike.cn

[N04] 斐波那契数列
来源：http://hg.yuexingan06.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ri.newstarts.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://tb.panjiajie.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kd.wgjwhj.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cu.bjjhwx.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://de.panjiajie.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://sn.muxihuayi.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ks.hnjuh.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ht.jianghongdianzi.cn

[N05] 最大公约数
来源：http://no.wgjwhj.cn

Py:   math.gcd(a, b)
来源：http://zw.newstarts.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ds.wgjwhj.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://br.9csxet.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dj.jianghongdianzi.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zz.jctech888.com.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://fo.wgjwhj.cn

Ruby: a.gcd(b)
来源：http://ba.hahajie.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://xv.yuexingan06.cn

[N06] 判断回文字符串
来源：http://gd.nicolike.cn

Py:   s == s[::-1]
来源：http://yy.huixiangedu.cn

PHP:  $s === strrev($s);
来源：http://uj.jianghongdianzi.cn

JS:   s === [...s].reverse().join("")
来源：http://jj.asd995.cn

TS:   s === [...s].reverse().join("")
来源：http://po.huixinmuqiang.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://qz.huixiangedu.cn

Go:   // 双指针从两端比较
来源：http://kr.chemitech.net.cn

Ruby: s == s.reverse
来源：http://um.nszjky.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://wp.szxytkj.cn

[N07] 两数之和（返回下标）
来源：http://eg.gzmigu.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://uc.521024.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wh.szsharing.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://dt.huixiangedu.cn

TS:   // 手写 Map<string, number>
来源：http://jv.lnxyls.cn

Java: // 手写 HashMap
来源：http://ci.shxzukj.cn

Go:   // 手写 map[int]int
来源：http://gc.yuntaijiaju.cn

Ruby: // 手写 Hash
来源：http://pq.hahajie.cn

C#:   // 手写 Dictionary<int, int>
来源：http://id.521024.cn

[N08] 生成全排列
来源：http://bd.panjiajie.cn

Py:   itertools.permutations(arr)
来源：http://ga.huanxung.cn

PHP:  // 手写递归交换
来源：http://mi.shxzukj.cn

JS:   // 手写回溯递归
来源：http://dy.jctech888.com.cn

TS:   // 手写回溯递归
来源：http://wk.bookmarksfly.cn

Java: // 手写回溯递归
来源：http://hx.9csxet.cn

Go:   // 手写回溯递归
来源：http://mb.colortex.cn

Ruby: arr.permutation.to_a
来源：http://im.lnxyls.cn

C#:   // 手写回溯递归
来源：http://yq.wgjwhj.cn

[N09] 栈与队列
来源：http://cv.chemitech.net.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://so.nicolike.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://yb.wgjwhj.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://af.muxihuayi.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://bf.haigaiapp.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://cx.panjiajie.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://dy.huixinmuqiang.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ni.chemitech.net.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://td.muxihuayi.cn

[N10] 链表节点定义
来源：http://lv.newstarts.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://lp.hnjuh.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://uu.yuntaijiaju.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://eq.yuexingan06.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hx.yuexingan06.cn

Java: class Node { int v; Node next; }
来源：http://do.muxihuayi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://lr.asd995.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://lo.chemitech.net.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://bv.jianghongdianzi.cn

[N11] 二叉树中序遍历
来源：http://gn.shxzukj.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://qz.nicolike.cn

PHP:  // 手写递归函数
来源：http://tx.huixinmuqiang.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yi.hnjuh.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yi.muxihuayi.cn

Java: // 手写递归
来源：http://mh.colortex.cn

Go:   // 手写递归
来源：http://vr.lnxyls.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://lq.yuexingan06.cn

C#:   // 手写递归
来源：http://oq.nicolike.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://gr.newstarts.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://cx.huanxung.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://om.521024.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://az.newstarts.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kg.huanxung.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hb.jianghongdianzi.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mp.huixinmuqiang.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://sg.shtwfgs.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://jk.shxzskj.cn

================================================================================
来源：http://ib.wgjwhj.cn

O. 并发与异步
来源：http://jg.chemitech.net.cn

================================================================================
来源：http://kq.bookmarksfly.cn

[O01] 启动一个线程
来源：http://ig.szsharing.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ma.szsharing.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://xc.nszjky.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://qn.asd995.cn

TS:   // 同 JS
来源：http://uj.shtwfgs.cn

Java: new Thread(() -> f()).start()
来源：http://xd.szsharing.cn

Go:   go f()
来源：http://oo.huanxung.cn

Ruby: Thread.new { f }
来源：http://zo.gzmigu.cn

C#:   Task.Run(() => F());
来源：http://ix.shxzskj.cn

[O02] 使用线程池
来源：http://fk.muxihuayi.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ic.huanxung.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://oc.shtwfgs.cn

JS:   // worker_threads 线程池
来源：http://xm.colortex.cn

TS:   // worker_threads 线程池
来源：http://si.newstarts.cn

Java: Executors.newFixedThreadPool(4)
来源：http://wb.jianghongdianzi.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ng.szxytkj.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://rj.wgjwhj.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://vm.521024.cn

[O03] 加锁保护共享数据
来源：http://yk.huixiangedu.cn

Py:   with lock: shared += 1
来源：http://sc.chemitech.net.cn

PHP:  // 用 flock() 做文件锁
来源：http://xs.szsharing.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://vc.szsharing.cn

TS:   // 同 JS
来源：http://rk.shxzukj.cn

Java: synchronized (this) { shared++; }
来源：http://vh.shtwfgs.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://td.shtwfgs.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://bg.newstarts.cn

C#:   lock (gate) { shared++; }
来源：http://hg.chemitech.net.cn

[O04] 定义异步函数并等待
来源：http://yi.hnjuh.cn

Py:   async def f():⏎    await g()
来源：http://fm.colortex.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://qf.gzmigu.cn

JS:   async function f() { await g(); }
来源：http://mw.shxzukj.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://in.jctech888.com.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://sr.nszjky.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://oc.shxzukj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://bx.shtwfgs.cn

C#:   async Task F() { await G(); }
来源：http://ok.newstarts.cn

[O05] 并发执行并等待全部完成
来源：http://ep.huanxung.cn

Py:   asyncio.gather(*tasks)
来源：http://ow.jctech888.com.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hk.jianghongdianzi.cn

JS:   await Promise.all(tasks)
来源：http://mg.haigaiapp.cn

TS:   await Promise.all(tasks)
来源：http://ob.9csxet.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hy.panjiajie.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ci.huixinmuqiang.cn

Ruby: threads.map(&:join)
来源：http://dw.chemitech.net.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://rx.asd995.cn

[O06] 使用进程池
来源：http://ci.hahajie.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://su.jianghongdianzi.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://gl.521024.cn

JS:   // child_process / cluster 模块
来源：http://ts.9csxet.cn

TS:   // child_process / cluster 模块
来源：http://xf.huanxung.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ye.nszjky.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://pj.yuntaijiaju.cn

Ruby: // fork 块
来源：http://yk.huanxung.cn

C#:   Parallel.For
来源：http://dl.huanxung.cn

================================================================================
来源：http://ej.panjiajie.cn

P. 常用工具函数
来源：http://kc.huixiangedu.cn

================================================================================
来源：http://rn.521024.cn

[P01] 生成 UUID
来源：http://lp.szxytkj.cn

Py:   str(uuid.uuid4())
来源：http://ir.hnjuh.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://pw.hnjuh.cn

JS:   crypto.randomUUID()
来源：http://wp.bookmarksfly.cn

TS:   crypto.randomUUID()
来源：http://qn.huanxung.cn

Java: UUID.randomUUID().toString()
来源：http://np.asd995.cn

Go:   // 用 github.com/google/uuid
来源：http://rv.panjiajie.cn

Ruby: SecureRandom.uuid
来源：http://ow.wgjwhj.cn

C#:   Guid.NewGuid().ToString()
来源：http://yd.huixinmuqiang.cn

[P02] MD5 / SHA256 摘要
来源：http://ik.jctech888.com.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://tn.muxihuayi.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ix.newstarts.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mf.huanxung.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://qj.huanxung.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ly.colortex.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://bd.521024.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://gw.newstarts.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ff.huixinmuqiang.cn

[P03] 生成短随机字符串
来源：http://vc.szxytkj.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mq.nicolike.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://bq.huanxung.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qz.huixinmuqiang.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://el.huixiangedu.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://rq.haigaiapp.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ap.jianghongdianzi.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://au.newstarts.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://os.shxzukj.cn

[P04] 求长度
来源：http://qe.asd995.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://nx.haigaiapp.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://in.521024.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cp.chemitech.net.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ul.lnxyls.cn

Java: list.size();  map.size();  s.length()
来源：http://cx.yuntaijiaju.cn

Go:   len(arr);  len(m)
来源：http://mq.szxytkj.cn

Ruby: x.length;  x.size
来源：http://yc.colortex.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ui.shtwfgs.cn

[P05] 判断两个对象内容是否相等
来源：http://fk.wgjwhj.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://dx.wgjwhj.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://qa.lnxyls.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://du.jctech888.com.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://dq.lnxyls.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://iq.panjiajie.cn

Go:   reflect.DeepEqual(a, b)
来源：http://am.yuntaijiaju.cn

Ruby: a == b
来源：http://mw.yuntaijiaju.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://zi.colortex.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://xo.huanxung.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://rm.shtwfgs.cn

PHP:  if (empty($x)) {}
来源：http://zf.shtwfgs.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hb.521024.cn

TS:   if (x == null) {}
来源：http://uo.asd995.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://uf.asd995.cn

Go:   if x == nil {}
来源：http://sn.newstarts.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wk.jianghongdianzi.cn

C#:   if (x is null) {}
来源：http://ke.jctech888.com.cn

[P07] 防抖与节流
来源：http://kn.newstarts.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://zm.wgjwhj.cn

PHP:  // 手写时间戳比较
来源：http://yo.bjjhwx.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wn.huixiangedu.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uv.huixinmuqiang.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://xx.hahajie.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://bx.shtwfgs.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://wj.bjjhwx.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ft.nicolike.cn

[P08] 处理浮点精度问题
来源：http://hh.yuexingan06.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://gl.jctech888.com.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://nh.lnxyls.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://yc.shtwfgs.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://xq.huixiangedu.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://th.chemitech.net.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://sx.521024.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://tz.521024.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://bi.chemitech.net.cn

================================================================================
来源：http://dp.yuexingan06.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://dn.huanxung.cn

================================================================================
来源：http://oz.shxzskj.cn

[Q01] 创建表
来源：http://xy.colortex.cn

CREATE TABLE users (
来源：http://xf.nicolike.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ch.gzmigu.cn

name VARCHAR(50) NOT NULL,
来源：http://cm.nszjky.cn

email VARCHAR(100) UNIQUE,
来源：http://uz.szxytkj.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://qv.haigaiapp.cn

);
来源：http://pq.muxihuayi.cn

[Q02] 创建带外键的表
来源：http://ah.chemitech.net.cn

CREATE TABLE orders (
来源：http://ps.gzmigu.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://qq.9csxet.cn

user_id INT NOT NULL,
来源：http://ny.gzmigu.cn

amount DECIMAL(10, 2),
来源：http://xj.huixinmuqiang.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://xv.colortex.cn

);
来源：http://ov.muxihuayi.cn

[Q03] 增加列
来源：http://pk.huixinmuqiang.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ag.hnjuh.cn

[Q04] 修改列类型
来源：http://rg.bjjhwx.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://cy.panjiajie.cn

[Q05] 重命名列
来源：http://sm.szsharing.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ey.asd995.cn

[Q06] 删除列
来源：http://zx.muxihuayi.cn

ALTER TABLE users DROP COLUMN age;
来源：http://co.szsharing.cn

[Q07] 删除表
来源：http://hm.haigaiapp.cn

DROP TABLE IF EXISTS orders;
来源：http://xr.haigaiapp.cn

[Q08] 创建普通索引
来源：http://zg.bjjhwx.cn


<!-- 参考信息 -->