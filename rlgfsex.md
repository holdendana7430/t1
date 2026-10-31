代发 wailian999

Ruby: exit 1
来源：http://ri.huixinmuqiang.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://nx.hahajie.cn

[M06] 向标准错误输出
来源：http://in.gzmigu.cn

Py:   print("err", file=sys.stderr)
来源：http://tl.haigaiapp.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://vd.yuexingan06.cn

JS:   console.error("err")
来源：http://ux.hahajie.cn

TS:   console.error("err")
来源：http://mj.yuexingan06.cn

Java: System.err.println("err")
来源：http://oe.hnjuh.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://yz.hnjuh.cn

Ruby: warn "err"
来源：http://qs.hnjuh.cn

C#:   Console.Error.WriteLine("err")
来源：http://zi.huixinmuqiang.cn

[M07] 判断是否为主入口
来源：http://dw.hahajie.cn

Py:   if __name__ == "__main__":
来源：http://zk.szsharing.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ep.bjjhwx.cn

JS:   require.main === module
来源：http://rc.shxzukj.cn

TS:   require.main === module
来源：http://an.lnxyls.cn

Java: public static void main(String[] args)
来源：http://hn.jctech888.com.cn

Go:   func main()
来源：http://bh.bookmarksfly.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ef.szxytkj.cn

C#:   static void Main(string[] args)
来源：http://rc.muxihuayi.cn

[M08] 获取系统与运行时信息
来源：http://ts.jianghongdianzi.cn

Py:   platform.system();  platform.python_version()
来源：http://iv.shxzskj.cn

PHP:  PHP_OS;  phpversion();
来源：http://ix.bookmarksfly.cn

JS:   process.platform;  process.version
来源：http://dc.haigaiapp.cn

TS:   process.platform;  process.version
来源：http://df.9csxet.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://bi.9csxet.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://id.nszjky.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://bq.nicolike.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://qv.bjjhwx.cn

================================================================================
来源：http://xn.wgjwhj.cn

N. 数据结构与算法
来源：http://fo.wgjwhj.cn

================================================================================
来源：http://dd.gzmigu.cn

[N01] 二分查找（有序数组）
来源：http://qf.hnjuh.cn

Py:   bisect.bisect_left(arr, x)
来源：http://qe.nicolike.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://eq.hnjuh.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://te.szxytkj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ok.bookmarksfly.cn

Java: Arrays.binarySearch(arr, x)
来源：http://aq.shxzskj.cn

Go:   sort.SearchInts(arr, x)
来源：http://ng.chemitech.net.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://wo.newstarts.cn

C#:   Array.BinarySearch(arr, x)
来源：http://kj.521024.cn

[N02] 排序（工程实践用内置实现）
来源：http://ma.szsharing.cn

Py:   sorted(arr);  arr.sort()
来源：http://sx.chemitech.net.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://kb.huanxung.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://go.gzmigu.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://rf.asd995.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://cx.colortex.cn

Go:   slices.Sort(arr)
来源：http://de.521024.cn

Ruby: arr.sort
来源：http://gh.lnxyls.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://kr.asd995.cn

[N03] 快速排序（分治示例）
来源：http://ql.jianghongdianzi.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://qs.jianghongdianzi.cn

PHP:  // 递归实现，或用 usort
来源：http://da.panjiajie.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cg.shxzskj.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://oo.521024.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://bl.jctech888.com.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://pd.huanxung.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://lu.newstarts.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ec.shtwfgs.cn

[N04] 斐波那契数列
来源：http://wj.yuntaijiaju.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://pd.panjiajie.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://kg.hnjuh.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://er.muxihuayi.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://th.gzmigu.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://yd.hahajie.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ps.huixiangedu.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://qr.szxytkj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://dm.9csxet.cn

[N05] 最大公约数
来源：http://sj.panjiajie.cn

Py:   math.gcd(a, b)
来源：http://xo.haigaiapp.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://pc.szsharing.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ay.newstarts.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://uw.yuntaijiaju.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ix.bookmarksfly.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://jr.colortex.cn

Ruby: a.gcd(b)
来源：http://ub.chemitech.net.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://kg.asd995.cn

[N06] 判断回文字符串
来源：http://hi.colortex.cn

Py:   s == s[::-1]
来源：http://cb.panjiajie.cn

PHP:  $s === strrev($s);
来源：http://ad.lnxyls.cn

JS:   s === [...s].reverse().join("")
来源：http://we.hnjuh.cn

TS:   s === [...s].reverse().join("")
来源：http://bd.lnxyls.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ji.nszjky.cn

Go:   // 双指针从两端比较
来源：http://tz.bjjhwx.cn

Ruby: s == s.reverse
来源：http://lo.szsharing.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ny.521024.cn

[N07] 两数之和（返回下标）
来源：http://ud.bjjhwx.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hv.huanxung.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ao.521024.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://zi.hnjuh.cn

TS:   // 手写 Map<string, number>
来源：http://ji.huanxung.cn

Java: // 手写 HashMap
来源：http://sw.shxzskj.cn

Go:   // 手写 map[int]int
来源：http://yi.szsharing.cn

Ruby: // 手写 Hash
来源：http://js.huanxung.cn

C#:   // 手写 Dictionary<int, int>
来源：http://vb.hnjuh.cn

[N08] 生成全排列
来源：http://eg.wgjwhj.cn

Py:   itertools.permutations(arr)
来源：http://os.szxytkj.cn

PHP:  // 手写递归交换
来源：http://nx.jctech888.com.cn

JS:   // 手写回溯递归
来源：http://qt.9csxet.cn

TS:   // 手写回溯递归
来源：http://hv.lnxyls.cn

Java: // 手写回溯递归
来源：http://zp.szxytkj.cn

Go:   // 手写回溯递归
来源：http://kb.nicolike.cn

Ruby: arr.permutation.to_a
来源：http://nl.panjiajie.cn

C#:   // 手写回溯递归
来源：http://ee.yuexingan06.cn

[N09] 栈与队列
来源：http://tp.newstarts.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://rf.haigaiapp.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://is.panjiajie.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://jw.lnxyls.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://xh.szxytkj.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://pf.hnjuh.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://iy.hahajie.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://yu.wgjwhj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://qi.newstarts.cn

[N10] 链表节点定义
来源：http://ry.wgjwhj.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ei.chemitech.net.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://hk.colortex.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://nz.colortex.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://tz.asd995.cn

Java: class Node { int v; Node next; }
来源：http://nb.nicolike.cn

Go:   type Node struct { V int; Next *Node }
来源：http://yn.huixiangedu.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://cl.yuntaijiaju.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://yw.nicolike.cn

[N11] 二叉树中序遍历
来源：http://dn.muxihuayi.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://rz.jctech888.com.cn

PHP:  // 手写递归函数
来源：http://oc.yuexingan06.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mr.gzmigu.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jw.bjjhwx.cn

Java: // 手写递归
来源：http://of.shxzukj.cn

Go:   // 手写递归
来源：http://so.asd995.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://jk.huixinmuqiang.cn

C#:   // 手写递归
来源：http://ny.haigaiapp.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://om.chemitech.net.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://nl.nicolike.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://oe.lnxyls.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vj.shxzskj.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ip.yuexingan06.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://zl.yuntaijiaju.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://jr.521024.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://iz.chemitech.net.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://jr.shxzskj.cn

================================================================================
来源：http://ed.panjiajie.cn

O. 并发与异步
来源：http://kp.panjiajie.cn

================================================================================
来源：http://ca.nszjky.cn

[O01] 启动一个线程
来源：http://kj.hnjuh.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://yn.shtwfgs.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ck.yuexingan06.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://fy.huixiangedu.cn

TS:   // 同 JS
来源：http://ol.huixiangedu.cn

Java: new Thread(() -> f()).start()
来源：http://dd.hnjuh.cn

Go:   go f()
来源：http://ia.huixinmuqiang.cn

Ruby: Thread.new { f }
来源：http://el.asd995.cn

C#:   Task.Run(() => F());
来源：http://tp.521024.cn

[O02] 使用线程池
来源：http://pd.colortex.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://sj.nszjky.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://yv.hahajie.cn

JS:   // worker_threads 线程池
来源：http://tz.bookmarksfly.cn

TS:   // worker_threads 线程池
来源：http://qn.asd995.cn

Java: Executors.newFixedThreadPool(4)
来源：http://dh.huanxung.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://zg.shxzukj.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://pu.hahajie.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wh.nicolike.cn

[O03] 加锁保护共享数据
来源：http://bo.bookmarksfly.cn

Py:   with lock: shared += 1
来源：http://fq.shxzskj.cn

PHP:  // 用 flock() 做文件锁
来源：http://vt.shtwfgs.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://sg.panjiajie.cn

TS:   // 同 JS
来源：http://lo.shxzukj.cn

Java: synchronized (this) { shared++; }
来源：http://hj.521024.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://at.yuntaijiaju.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://oo.shxzukj.cn

C#:   lock (gate) { shared++; }
来源：http://lk.shxzukj.cn

[O04] 定义异步函数并等待
来源：http://js.jianghongdianzi.cn

Py:   async def f():⏎    await g()
来源：http://xu.chemitech.net.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mw.nszjky.cn

JS:   async function f() { await g(); }
来源：http://nb.huixiangedu.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://id.9csxet.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://cj.lnxyls.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ac.521024.cn

Ruby: # 用 Fiber 或 async gem
来源：http://xu.gzmigu.cn

C#:   async Task F() { await G(); }
来源：http://ez.shxzskj.cn

[O05] 并发执行并等待全部完成
来源：http://yy.bjjhwx.cn

Py:   asyncio.gather(*tasks)
来源：http://it.newstarts.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://eh.nicolike.cn

JS:   await Promise.all(tasks)
来源：http://om.9csxet.cn

TS:   await Promise.all(tasks)
来源：http://jv.nszjky.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://il.colortex.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://jf.9csxet.cn

Ruby: threads.map(&:join)
来源：http://qp.hnjuh.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://cs.huixinmuqiang.cn

[O06] 使用进程池
来源：http://tx.panjiajie.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://sa.shxzskj.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://sv.shxzukj.cn

JS:   // child_process / cluster 模块
来源：http://hy.shxzukj.cn

TS:   // child_process / cluster 模块
来源：http://dm.jianghongdianzi.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://xx.muxihuayi.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ow.hnjuh.cn

Ruby: // fork 块
来源：http://ll.shxzukj.cn

C#:   Parallel.For
来源：http://qa.jctech888.com.cn

================================================================================
来源：http://pc.9csxet.cn

P. 常用工具函数
来源：http://nj.gzmigu.cn

================================================================================
来源：http://yd.jctech888.com.cn

[P01] 生成 UUID
来源：http://vc.shxzukj.cn

Py:   str(uuid.uuid4())
来源：http://aa.jctech888.com.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://kq.nszjky.cn

JS:   crypto.randomUUID()
来源：http://ku.bookmarksfly.cn

TS:   crypto.randomUUID()
来源：http://ls.newstarts.cn

Java: UUID.randomUUID().toString()
来源：http://ch.chemitech.net.cn

Go:   // 用 github.com/google/uuid
来源：http://pn.huixinmuqiang.cn

Ruby: SecureRandom.uuid
来源：http://vf.huixinmuqiang.cn

C#:   Guid.NewGuid().ToString()
来源：http://sm.lnxyls.cn

[P02] MD5 / SHA256 摘要
来源：http://xx.hahajie.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://bz.yuntaijiaju.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://aa.jctech888.com.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wk.colortex.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://xu.jianghongdianzi.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://cd.nicolike.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://fn.521024.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://gl.bookmarksfly.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://sl.yuexingan06.cn

[P03] 生成短随机字符串
来源：http://wr.gzmigu.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wz.panjiajie.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://gv.huixinmuqiang.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://it.gzmigu.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wl.shxzukj.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://if.colortex.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://tc.colortex.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://oa.jctech888.com.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://xn.muxihuayi.cn

[P04] 求长度
来源：http://jm.colortex.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://dp.nszjky.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qa.newstarts.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://uv.newstarts.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yr.jctech888.com.cn

Java: list.size();  map.size();  s.length()
来源：http://rp.newstarts.cn

Go:   len(arr);  len(m)
来源：http://hy.hahajie.cn

Ruby: x.length;  x.size
来源：http://ua.asd995.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://zn.huixinmuqiang.cn

[P05] 判断两个对象内容是否相等
来源：http://mf.hnjuh.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://uc.szxytkj.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://nw.hnjuh.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://kw.yuntaijiaju.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hk.yuexingan06.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ny.newstarts.cn

Go:   reflect.DeepEqual(a, b)
来源：http://kt.shxzukj.cn

Ruby: a == b
来源：http://ak.lnxyls.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://zd.shtwfgs.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.szxytkj.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://cl.panjiajie.cn

PHP:  if (empty($x)) {}
来源：http://ap.huanxung.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://vs.9csxet.cn

TS:   if (x == null) {}
来源：http://og.szxytkj.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://cg.nszjky.cn

Go:   if x == nil {}
来源：http://ko.521024.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://xw.nszjky.cn

C#:   if (x is null) {}
来源：http://tt.szxytkj.cn

[P07] 防抖与节流
来源：http://tr.hnjuh.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ps.asd995.cn

PHP:  // 手写时间戳比较
来源：http://ax.asd995.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://of.panjiajie.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rc.gzmigu.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://is.9csxet.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://oz.huixiangedu.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://bf.chemitech.net.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mj.hahajie.cn

[P08] 处理浮点精度问题
来源：http://ms.haigaiapp.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://fc.shxzskj.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://lw.shtwfgs.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ti.nicolike.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://fd.huixinmuqiang.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://lo.yuntaijiaju.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ir.hahajie.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://sb.newstarts.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://qi.shxzskj.cn

================================================================================
来源：http://jo.shxzskj.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://qx.newstarts.cn

================================================================================
来源：http://gz.asd995.cn

[Q01] 创建表
来源：http://wl.nszjky.cn

CREATE TABLE users (
来源：http://sa.huixinmuqiang.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://vm.huixiangedu.cn

name VARCHAR(50) NOT NULL,
来源：http://cq.shtwfgs.cn

email VARCHAR(100) UNIQUE,
来源：http://tk.asd995.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ne.jianghongdianzi.cn

);
来源：http://kt.haigaiapp.cn

[Q02] 创建带外键的表
来源：http://bd.newstarts.cn

CREATE TABLE orders (
来源：http://wv.nszjky.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ah.huanxung.cn

user_id INT NOT NULL,
来源：http://mk.panjiajie.cn

amount DECIMAL(10, 2),
来源：http://ll.szxytkj.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://sb.huixiangedu.cn

);
来源：http://kv.wgjwhj.cn

[Q03] 增加列
来源：http://id.gzmigu.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ue.gzmigu.cn

[Q04] 修改列类型
来源：http://ck.colortex.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://gs.9csxet.cn

[Q05] 重命名列
来源：http://gr.lnxyls.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://pe.colortex.cn

[Q06] 删除列
来源：http://zj.panjiajie.cn

ALTER TABLE users DROP COLUMN age;
来源：http://yr.nicolike.cn

[Q07] 删除表
来源：http://rq.yuexingan06.cn

DROP TABLE IF EXISTS orders;
来源：http://wl.asd995.cn

[Q08] 创建普通索引
来源：http://vl.huixinmuqiang.cn


<!-- 参考信息 -->