代发 wailian999

PHP:  fwrite(STDERR, "err\n");
来源：http://yk.shxzukj.cn

JS:   console.error("err")
来源：http://jg.colortex.cn

TS:   console.error("err")
来源：http://zj.521024.cn

Java: System.err.println("err")
来源：http://ex.huixinmuqiang.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://rg.shxzukj.cn

Ruby: warn "err"
来源：http://zl.wgjwhj.cn

C#:   Console.Error.WriteLine("err")
来源：http://ym.yuntaijiaju.cn

[M07] 判断是否为主入口
来源：http://wb.bookmarksfly.cn

Py:   if __name__ == "__main__":
来源：http://yw.nszjky.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://te.yuexingan06.cn

JS:   require.main === module
来源：http://wo.yuntaijiaju.cn

TS:   require.main === module
来源：http://rk.shxzukj.cn

Java: public static void main(String[] args)
来源：http://wa.colortex.cn

Go:   func main()
来源：http://uv.9csxet.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hg.521024.cn

C#:   static void Main(string[] args)
来源：http://vw.colortex.cn

[M08] 获取系统与运行时信息
来源：http://rj.huixinmuqiang.cn

Py:   platform.system();  platform.python_version()
来源：http://jk.shtwfgs.cn

PHP:  PHP_OS;  phpversion();
来源：http://bp.newstarts.cn

JS:   process.platform;  process.version
来源：http://mn.szsharing.cn

TS:   process.platform;  process.version
来源：http://dz.chemitech.net.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hx.szxytkj.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://eu.hnjuh.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hk.huanxung.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://mn.nszjky.cn

================================================================================
来源：http://js.muxihuayi.cn

N. 数据结构与算法
来源：http://ua.jctech888.com.cn

================================================================================
来源：http://dv.yuntaijiaju.cn

[N01] 二分查找（有序数组）
来源：http://eh.gzmigu.cn

Py:   bisect.bisect_left(arr, x)
来源：http://tb.jctech888.com.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ux.nicolike.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hm.panjiajie.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://on.yuntaijiaju.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ix.9csxet.cn

Go:   sort.SearchInts(arr, x)
来源：http://mc.wgjwhj.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://wq.bookmarksfly.cn

C#:   Array.BinarySearch(arr, x)
来源：http://oz.chemitech.net.cn

[N02] 排序（工程实践用内置实现）
来源：http://ib.nszjky.cn

Py:   sorted(arr);  arr.sort()
来源：http://po.nszjky.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://vq.lnxyls.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://sr.shtwfgs.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://wm.hahajie.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ei.newstarts.cn

Go:   slices.Sort(arr)
来源：http://tp.521024.cn

Ruby: arr.sort
来源：http://hv.muxihuayi.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://tm.jctech888.com.cn

[N03] 快速排序（分治示例）
来源：http://fc.colortex.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://fy.jianghongdianzi.cn

PHP:  // 递归实现，或用 usort
来源：http://fk.szsharing.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nb.huixiangedu.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bm.521024.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://az.newstarts.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://am.521024.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://jp.nszjky.cn

C#:   // 手写递归，或 Array.Sort
来源：http://qh.bjjhwx.cn

[N04] 斐波那契数列
来源：http://ko.hahajie.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://kc.gzmigu.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hl.hnjuh.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kb.nszjky.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://om.jctech888.com.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://tz.9csxet.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ag.shxzskj.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://li.huixiangedu.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://fc.bookmarksfly.cn

[N05] 最大公约数
来源：http://mc.huanxung.cn

Py:   math.gcd(a, b)
来源：http://sx.bookmarksfly.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mg.huixinmuqiang.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ny.asd995.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hw.521024.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://py.hahajie.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://sa.newstarts.cn

Ruby: a.gcd(b)
来源：http://zo.bookmarksfly.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wp.szsharing.cn

[N06] 判断回文字符串
来源：http://ik.gzmigu.cn

Py:   s == s[::-1]
来源：http://jj.panjiajie.cn

PHP:  $s === strrev($s);
来源：http://za.muxihuayi.cn

JS:   s === [...s].reverse().join("")
来源：http://nt.jctech888.com.cn

TS:   s === [...s].reverse().join("")
来源：http://hc.gzmigu.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mi.jianghongdianzi.cn

Go:   // 双指针从两端比较
来源：http://xa.chemitech.net.cn

Ruby: s == s.reverse
来源：http://ix.shxzskj.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ys.shxzukj.cn

[N07] 两数之和（返回下标）
来源：http://te.huixinmuqiang.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://kr.szsharing.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://cv.bookmarksfly.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://rh.yuntaijiaju.cn

TS:   // 手写 Map<string, number>
来源：http://gd.asd995.cn

Java: // 手写 HashMap
来源：http://tw.colortex.cn

Go:   // 手写 map[int]int
来源：http://gq.lnxyls.cn

Ruby: // 手写 Hash
来源：http://tt.yuexingan06.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ae.jctech888.com.cn

[N08] 生成全排列
来源：http://qy.huixinmuqiang.cn

Py:   itertools.permutations(arr)
来源：http://ka.shtwfgs.cn

PHP:  // 手写递归交换
来源：http://fk.yuexingan06.cn

JS:   // 手写回溯递归
来源：http://ux.jianghongdianzi.cn

TS:   // 手写回溯递归
来源：http://rz.jianghongdianzi.cn

Java: // 手写回溯递归
来源：http://od.shxzskj.cn

Go:   // 手写回溯递归
来源：http://ty.panjiajie.cn

Ruby: arr.permutation.to_a
来源：http://kc.jctech888.com.cn

C#:   // 手写回溯递归
来源：http://vf.yuexingan06.cn

[N09] 栈与队列
来源：http://rv.newstarts.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://xh.hahajie.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://xv.nicolike.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://kp.jianghongdianzi.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://uf.muxihuayi.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://zd.shxzskj.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hs.chemitech.net.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://nw.haigaiapp.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://on.hahajie.cn

[N10] 链表节点定义
来源：http://fp.bjjhwx.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wo.gzmigu.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://oz.hahajie.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://lr.shxzukj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ps.shxzskj.cn

Java: class Node { int v; Node next; }
来源：http://wu.haigaiapp.cn

Go:   type Node struct { V int; Next *Node }
来源：http://zp.wgjwhj.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://wa.wgjwhj.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://qg.nicolike.cn

[N11] 二叉树中序遍历
来源：http://le.yuntaijiaju.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://cb.yuntaijiaju.cn

PHP:  // 手写递归函数
来源：http://yu.huanxung.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jl.newstarts.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vb.szsharing.cn

Java: // 手写递归
来源：http://fz.521024.cn

Go:   // 手写递归
来源：http://yc.panjiajie.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://xe.panjiajie.cn

C#:   // 手写递归
来源：http://bm.yuntaijiaju.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://pb.521024.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://gi.bjjhwx.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ek.wgjwhj.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ai.yuntaijiaju.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bx.hahajie.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ly.9csxet.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://xp.bjjhwx.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://eu.shxzskj.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://kb.yuexingan06.cn

================================================================================
来源：http://kz.yuexingan06.cn

O. 并发与异步
来源：http://yr.huixinmuqiang.cn

================================================================================
来源：http://jg.shxzskj.cn

[O01] 启动一个线程
来源：http://tj.nszjky.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://cx.nszjky.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://tm.panjiajie.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://cg.newstarts.cn

TS:   // 同 JS
来源：http://ve.muxihuayi.cn

Java: new Thread(() -> f()).start()
来源：http://yn.asd995.cn

Go:   go f()
来源：http://aw.lnxyls.cn

Ruby: Thread.new { f }
来源：http://iy.haigaiapp.cn

C#:   Task.Run(() => F());
来源：http://zf.chemitech.net.cn

[O02] 使用线程池
来源：http://fu.yuexingan06.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://uz.bjjhwx.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://lm.szsharing.cn

JS:   // worker_threads 线程池
来源：http://bx.nszjky.cn

TS:   // worker_threads 线程池
来源：http://cb.panjiajie.cn

Java: Executors.newFixedThreadPool(4)
来源：http://lc.shtwfgs.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://eg.bookmarksfly.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ak.shtwfgs.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://jz.newstarts.cn

[O03] 加锁保护共享数据
来源：http://yh.shxzskj.cn

Py:   with lock: shared += 1
来源：http://pa.huanxung.cn

PHP:  // 用 flock() 做文件锁
来源：http://ji.hnjuh.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://np.shxzskj.cn

TS:   // 同 JS
来源：http://uc.muxihuayi.cn

Java: synchronized (this) { shared++; }
来源：http://hc.chemitech.net.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://qt.colortex.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://qa.huixinmuqiang.cn

C#:   lock (gate) { shared++; }
来源：http://ka.huixiangedu.cn

[O04] 定义异步函数并等待
来源：http://tr.chemitech.net.cn

Py:   async def f():⏎    await g()
来源：http://pr.chemitech.net.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://xf.lnxyls.cn

JS:   async function f() { await g(); }
来源：http://hc.muxihuayi.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ef.szsharing.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://tc.szsharing.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://dj.shxzskj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://jq.szsharing.cn

C#:   async Task F() { await G(); }
来源：http://cj.huixiangedu.cn

[O05] 并发执行并等待全部完成
来源：http://er.colortex.cn

Py:   asyncio.gather(*tasks)
来源：http://gs.yuexingan06.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://cc.huixiangedu.cn

JS:   await Promise.all(tasks)
来源：http://vs.bjjhwx.cn

TS:   await Promise.all(tasks)
来源：http://os.lnxyls.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://tt.lnxyls.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://gf.haigaiapp.cn

Ruby: threads.map(&:join)
来源：http://nr.yuexingan06.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://xz.wgjwhj.cn

[O06] 使用进程池
来源：http://zn.9csxet.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://gl.bookmarksfly.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://da.huixinmuqiang.cn

JS:   // child_process / cluster 模块
来源：http://bn.szsharing.cn

TS:   // child_process / cluster 模块
来源：http://vv.wgjwhj.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://eh.521024.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://td.yuexingan06.cn

Ruby: // fork 块
来源：http://gp.huanxung.cn

C#:   Parallel.For
来源：http://cf.bookmarksfly.cn

================================================================================
来源：http://ym.nszjky.cn

P. 常用工具函数
来源：http://br.nicolike.cn

================================================================================
来源：http://au.muxihuayi.cn

[P01] 生成 UUID
来源：http://bl.nszjky.cn

Py:   str(uuid.uuid4())
来源：http://mj.shxzukj.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ub.shxzskj.cn

JS:   crypto.randomUUID()
来源：http://ov.521024.cn

TS:   crypto.randomUUID()
来源：http://vs.newstarts.cn

Java: UUID.randomUUID().toString()
来源：http://rm.521024.cn

Go:   // 用 github.com/google/uuid
来源：http://oi.chemitech.net.cn

Ruby: SecureRandom.uuid
来源：http://iz.szsharing.cn

C#:   Guid.NewGuid().ToString()
来源：http://dn.colortex.cn

[P02] MD5 / SHA256 摘要
来源：http://ie.bjjhwx.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ie.shxzskj.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://gx.lnxyls.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ff.huixiangedu.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://tk.haigaiapp.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://is.panjiajie.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://re.yuexingan06.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://gu.muxihuayi.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://sh.haigaiapp.cn

[P03] 生成短随机字符串
来源：http://sb.bookmarksfly.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wd.bjjhwx.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wu.521024.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://uy.yuntaijiaju.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lt.newstarts.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://xc.lnxyls.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://pc.muxihuayi.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://wh.shxzukj.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://sv.colortex.cn

[P04] 求长度
来源：http://ly.haigaiapp.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://xj.hnjuh.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://to.asd995.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://do.521024.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kc.521024.cn

Java: list.size();  map.size();  s.length()
来源：http://ci.huixinmuqiang.cn

Go:   len(arr);  len(m)
来源：http://cb.shxzskj.cn

Ruby: x.length;  x.size
来源：http://um.hnjuh.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://td.521024.cn

[P05] 判断两个对象内容是否相等
来源：http://qw.521024.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://dd.newstarts.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mm.huixiangedu.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://rs.szxytkj.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://rb.hahajie.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://xa.huixiangedu.cn

Go:   reflect.DeepEqual(a, b)
来源：http://vk.lnxyls.cn

Ruby: a == b
来源：http://xs.asd995.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://kn.shxzskj.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://lm.panjiajie.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://zc.nicolike.cn

PHP:  if (empty($x)) {}
来源：http://as.9csxet.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://pq.szsharing.cn

TS:   if (x == null) {}
来源：http://tj.shtwfgs.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://bz.huanxung.cn

Go:   if x == nil {}
来源：http://jj.huanxung.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://kn.521024.cn

C#:   if (x is null) {}
来源：http://ce.jctech888.com.cn

[P07] 防抖与节流
来源：http://ny.wgjwhj.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://xd.yuntaijiaju.cn

PHP:  // 手写时间戳比较
来源：http://ti.chemitech.net.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dw.jctech888.com.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gf.gzmigu.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://bj.haigaiapp.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://og.haigaiapp.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://kb.521024.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://bs.muxihuayi.cn

[P08] 处理浮点精度问题
来源：http://yg.huanxung.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://rn.chemitech.net.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://gt.nicolike.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://uu.huixinmuqiang.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ht.hnjuh.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://uz.shxzskj.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://yb.szxytkj.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://iy.shtwfgs.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://nr.huixinmuqiang.cn

================================================================================
来源：http://kp.yuntaijiaju.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://va.lnxyls.cn

================================================================================
来源：http://gt.nszjky.cn

[Q01] 创建表
来源：http://km.521024.cn

CREATE TABLE users (
来源：http://rn.huixinmuqiang.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://vu.colortex.cn

name VARCHAR(50) NOT NULL,
来源：http://ta.szsharing.cn

email VARCHAR(100) UNIQUE,
来源：http://rv.colortex.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://bs.9csxet.cn

);
来源：http://ct.huanxung.cn

[Q02] 创建带外键的表
来源：http://ko.colortex.cn

CREATE TABLE orders (
来源：http://gn.shxzukj.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://zm.muxihuayi.cn

user_id INT NOT NULL,
来源：http://lh.yuntaijiaju.cn

amount DECIMAL(10, 2),
来源：http://zs.shxzukj.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://kn.huanxung.cn

);
来源：http://zc.huixinmuqiang.cn

[Q03] 增加列
来源：http://oq.lnxyls.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://gn.muxihuayi.cn

[Q04] 修改列类型
来源：http://hr.chemitech.net.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://qu.gzmigu.cn

[Q05] 重命名列
来源：http://ww.chemitech.net.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://xo.szxytkj.cn

[Q06] 删除列
来源：http://og.bjjhwx.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ja.haigaiapp.cn

[Q07] 删除表
来源：http://tc.bjjhwx.cn

DROP TABLE IF EXISTS orders;
来源：http://vp.yuexingan06.cn

[Q08] 创建普通索引
来源：http://xb.haigaiapp.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://zf.shxzskj.cn

[Q09] 创建唯一索引
来源：http://sg.hahajie.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://jq.colortex.cn

[Q10] 插入单行
来源：http://fz.jctech888.com.cn


<!-- 参考信息 -->