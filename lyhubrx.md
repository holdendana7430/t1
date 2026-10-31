代发 wailian999

JS:   process.exit(1)
来源：http://zl.shxzukj.cn

TS:   process.exit(1)
来源：http://dn.jianghongdianzi.cn

Java: System.exit(1)
来源：http://sm.nicolike.cn

Go:   os.Exit(1)
来源：http://uf.huanxung.cn

Ruby: exit 1
来源：http://uf.colortex.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://rh.9csxet.cn

[M06] 向标准错误输出
来源：http://ip.muxihuayi.cn

Py:   print("err", file=sys.stderr)
来源：http://zy.hnjuh.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://jw.szxytkj.cn

JS:   console.error("err")
来源：http://ti.szxytkj.cn

TS:   console.error("err")
来源：http://mn.shxzskj.cn

Java: System.err.println("err")
来源：http://jl.colortex.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://xo.asd995.cn

Ruby: warn "err"
来源：http://pw.shxzukj.cn

C#:   Console.Error.WriteLine("err")
来源：http://wl.shxzskj.cn

[M07] 判断是否为主入口
来源：http://uz.nszjky.cn

Py:   if __name__ == "__main__":
来源：http://et.hnjuh.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://rj.newstarts.cn

JS:   require.main === module
来源：http://sy.haigaiapp.cn

TS:   require.main === module
来源：http://pl.bookmarksfly.cn

Java: public static void main(String[] args)
来源：http://pa.yuntaijiaju.cn

Go:   func main()
来源：http://wn.asd995.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ar.bookmarksfly.cn

C#:   static void Main(string[] args)
来源：http://cs.hnjuh.cn

[M08] 获取系统与运行时信息
来源：http://bv.lnxyls.cn

Py:   platform.system();  platform.python_version()
来源：http://tc.hnjuh.cn

PHP:  PHP_OS;  phpversion();
来源：http://nd.colortex.cn

JS:   process.platform;  process.version
来源：http://gv.bjjhwx.cn

TS:   process.platform;  process.version
来源：http://jt.521024.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ru.newstarts.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://rv.jctech888.com.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://dc.chemitech.net.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://yj.wgjwhj.cn

================================================================================
来源：http://ci.shtwfgs.cn

N. 数据结构与算法
来源：http://fm.jctech888.com.cn

================================================================================
来源：http://jo.chemitech.net.cn

[N01] 二分查找（有序数组）
来源：http://aa.hahajie.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ds.521024.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://rm.shxzukj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dj.gzmigu.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jn.521024.cn

Java: Arrays.binarySearch(arr, x)
来源：http://qx.lnxyls.cn

Go:   sort.SearchInts(arr, x)
来源：http://bb.panjiajie.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://iq.jctech888.com.cn

C#:   Array.BinarySearch(arr, x)
来源：http://xk.yuntaijiaju.cn

[N02] 排序（工程实践用内置实现）
来源：http://nw.shxzskj.cn

Py:   sorted(arr);  arr.sort()
来源：http://ug.shxzukj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://bs.huanxung.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://sc.newstarts.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ky.9csxet.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://pe.muxihuayi.cn

Go:   slices.Sort(arr)
来源：http://qp.jctech888.com.cn

Ruby: arr.sort
来源：http://cs.newstarts.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://yu.lnxyls.cn

[N03] 快速排序（分治示例）
来源：http://mv.9csxet.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://en.nszjky.cn

PHP:  // 递归实现，或用 usort
来源：http://ng.muxihuayi.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bu.huixinmuqiang.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qy.9csxet.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://jj.shtwfgs.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://kl.jctech888.com.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ge.bjjhwx.cn

C#:   // 手写递归，或 Array.Sort
来源：http://cl.shxzskj.cn

[N04] 斐波那契数列
来源：http://xn.chemitech.net.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ze.huixiangedu.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://yn.wgjwhj.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hd.huixinmuqiang.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://br.bookmarksfly.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://py.shxzukj.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://bj.9csxet.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ji.jianghongdianzi.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://kr.chemitech.net.cn

[N05] 最大公约数
来源：http://vr.bjjhwx.cn

Py:   math.gcd(a, b)
来源：http://zq.lnxyls.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://qz.huixinmuqiang.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kw.huixinmuqiang.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qi.jctech888.com.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wj.shxzskj.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://rv.huixinmuqiang.cn

Ruby: a.gcd(b)
来源：http://qz.bookmarksfly.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://gx.shxzukj.cn

[N06] 判断回文字符串
来源：http://tp.lnxyls.cn

Py:   s == s[::-1]
来源：http://zk.shtwfgs.cn

PHP:  $s === strrev($s);
来源：http://ad.nszjky.cn

JS:   s === [...s].reverse().join("")
来源：http://jd.shxzukj.cn

TS:   s === [...s].reverse().join("")
来源：http://mc.nicolike.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://aw.szsharing.cn

Go:   // 双指针从两端比较
来源：http://ck.huixinmuqiang.cn

Ruby: s == s.reverse
来源：http://nr.bookmarksfly.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ze.szxytkj.cn

[N07] 两数之和（返回下标）
来源：http://md.hahajie.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://gq.newstarts.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://uw.szxytkj.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://tu.colortex.cn

TS:   // 手写 Map<string, number>
来源：http://bj.huanxung.cn

Java: // 手写 HashMap
来源：http://fk.wgjwhj.cn

Go:   // 手写 map[int]int
来源：http://pl.muxihuayi.cn

Ruby: // 手写 Hash
来源：http://ub.yuexingan06.cn

C#:   // 手写 Dictionary<int, int>
来源：http://vl.panjiajie.cn

[N08] 生成全排列
来源：http://qg.shxzskj.cn

Py:   itertools.permutations(arr)
来源：http://ls.lnxyls.cn

PHP:  // 手写递归交换
来源：http://uk.huixinmuqiang.cn

JS:   // 手写回溯递归
来源：http://vy.huixiangedu.cn

TS:   // 手写回溯递归
来源：http://hk.shtwfgs.cn

Java: // 手写回溯递归
来源：http://js.shxzskj.cn

Go:   // 手写回溯递归
来源：http://mx.wgjwhj.cn

Ruby: arr.permutation.to_a
来源：http://fw.huixinmuqiang.cn

C#:   // 手写回溯递归
来源：http://se.panjiajie.cn

[N09] 栈与队列
来源：http://ne.huixinmuqiang.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://vt.9csxet.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://nc.nicolike.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ib.newstarts.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://dy.jianghongdianzi.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://py.szsharing.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://kc.colortex.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://di.shtwfgs.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://re.bjjhwx.cn

[N10] 链表节点定义
来源：http://yi.asd995.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://gm.nszjky.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ou.colortex.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://uo.gzmigu.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://rz.panjiajie.cn

Java: class Node { int v; Node next; }
来源：http://qp.shxzukj.cn

Go:   type Node struct { V int; Next *Node }
来源：http://cg.muxihuayi.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://hl.muxihuayi.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://km.newstarts.cn

[N11] 二叉树中序遍历
来源：http://rr.nszjky.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mr.szxytkj.cn

PHP:  // 手写递归函数
来源：http://gl.newstarts.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kk.chemitech.net.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xc.9csxet.cn

Java: // 手写递归
来源：http://cq.jianghongdianzi.cn

Go:   // 手写递归
来源：http://km.jctech888.com.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://vh.muxihuayi.cn

C#:   // 手写递归
来源：http://rz.colortex.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://yj.huixinmuqiang.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://yn.huixinmuqiang.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://to.shtwfgs.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pu.chemitech.net.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fs.haigaiapp.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://dn.wgjwhj.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://tk.colortex.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://bf.9csxet.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://sd.szsharing.cn

================================================================================
来源：http://wo.shxzskj.cn

O. 并发与异步
来源：http://tp.nszjky.cn

================================================================================
来源：http://bg.muxihuayi.cn

[O01] 启动一个线程
来源：http://sg.hahajie.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://of.panjiajie.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://oq.gzmigu.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://iv.huanxung.cn

TS:   // 同 JS
来源：http://fr.huixinmuqiang.cn

Java: new Thread(() -> f()).start()
来源：http://il.jianghongdianzi.cn

Go:   go f()
来源：http://ko.hahajie.cn

Ruby: Thread.new { f }
来源：http://yu.colortex.cn

C#:   Task.Run(() => F());
来源：http://he.nicolike.cn

[O02] 使用线程池
来源：http://vr.hahajie.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mj.nicolike.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ov.newstarts.cn

JS:   // worker_threads 线程池
来源：http://ob.colortex.cn

TS:   // worker_threads 线程池
来源：http://ic.newstarts.cn

Java: Executors.newFixedThreadPool(4)
来源：http://kq.asd995.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://kd.nicolike.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://qu.gzmigu.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://fl.gzmigu.cn

[O03] 加锁保护共享数据
来源：http://ua.haigaiapp.cn

Py:   with lock: shared += 1
来源：http://ip.haigaiapp.cn

PHP:  // 用 flock() 做文件锁
来源：http://bu.asd995.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://cg.nszjky.cn

TS:   // 同 JS
来源：http://rs.hahajie.cn

Java: synchronized (this) { shared++; }
来源：http://em.chemitech.net.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://yy.panjiajie.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://oy.bjjhwx.cn

C#:   lock (gate) { shared++; }
来源：http://zx.huanxung.cn

[O04] 定义异步函数并等待
来源：http://sy.colortex.cn

Py:   async def f():⏎    await g()
来源：http://uo.hahajie.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://vm.shtwfgs.cn

JS:   async function f() { await g(); }
来源：http://bw.colortex.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ew.wgjwhj.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://fg.shtwfgs.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://rl.shtwfgs.cn

Ruby: # 用 Fiber 或 async gem
来源：http://cs.gzmigu.cn

C#:   async Task F() { await G(); }
来源：http://mr.huixiangedu.cn

[O05] 并发执行并等待全部完成
来源：http://pa.huixinmuqiang.cn

Py:   asyncio.gather(*tasks)
来源：http://bs.hnjuh.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://xs.bjjhwx.cn

JS:   await Promise.all(tasks)
来源：http://kx.lnxyls.cn

TS:   await Promise.all(tasks)
来源：http://kc.panjiajie.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://zi.bookmarksfly.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://kj.asd995.cn

Ruby: threads.map(&:join)
来源：http://vc.nszjky.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://uf.9csxet.cn

[O06] 使用进程池
来源：http://fb.9csxet.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://gc.haigaiapp.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://wp.yuexingan06.cn

JS:   // child_process / cluster 模块
来源：http://ss.szxytkj.cn

TS:   // child_process / cluster 模块
来源：http://mz.colortex.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ao.wgjwhj.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mo.gzmigu.cn

Ruby: // fork 块
来源：http://zb.yuexingan06.cn

C#:   Parallel.For
来源：http://dk.szsharing.cn

================================================================================
来源：http://it.wgjwhj.cn

P. 常用工具函数
来源：http://le.shxzukj.cn

================================================================================
来源：http://sd.haigaiapp.cn

[P01] 生成 UUID
来源：http://yg.panjiajie.cn

Py:   str(uuid.uuid4())
来源：http://sn.chemitech.net.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://fq.muxihuayi.cn

JS:   crypto.randomUUID()
来源：http://li.panjiajie.cn

TS:   crypto.randomUUID()
来源：http://ru.huixinmuqiang.cn

Java: UUID.randomUUID().toString()
来源：http://bl.9csxet.cn

Go:   // 用 github.com/google/uuid
来源：http://gf.nszjky.cn

Ruby: SecureRandom.uuid
来源：http://oz.521024.cn

C#:   Guid.NewGuid().ToString()
来源：http://zf.muxihuayi.cn

[P02] MD5 / SHA256 摘要
来源：http://jt.yuntaijiaju.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://vw.huanxung.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://tc.haigaiapp.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://og.asd995.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://xg.newstarts.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://eh.bookmarksfly.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ho.hahajie.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://py.chemitech.net.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://tf.lnxyls.cn

[P03] 生成短随机字符串
来源：http://tr.shxzskj.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://cp.szsharing.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://vy.jctech888.com.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gq.521024.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://il.asd995.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://on.shxzukj.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://oc.521024.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://wb.asd995.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://se.yuntaijiaju.cn

[P04] 求长度
来源：http://qb.shxzskj.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://rt.haigaiapp.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kc.huixinmuqiang.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wu.bjjhwx.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fb.jianghongdianzi.cn

Java: list.size();  map.size();  s.length()
来源：http://is.hnjuh.cn

Go:   len(arr);  len(m)
来源：http://qq.521024.cn

Ruby: x.length;  x.size
来源：http://ts.chemitech.net.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://mr.nicolike.cn

[P05] 判断两个对象内容是否相等
来源：http://cf.shxzukj.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://gc.szxytkj.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://qh.gzmigu.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://lx.newstarts.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://co.newstarts.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://uq.shxzukj.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ev.haigaiapp.cn

Ruby: a == b
来源：http://ax.newstarts.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://uy.huixiangedu.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://oi.jianghongdianzi.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wm.jianghongdianzi.cn

PHP:  if (empty($x)) {}
来源：http://px.yuexingan06.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://dg.szsharing.cn

TS:   if (x == null) {}
来源：http://kr.huanxung.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://jg.nszjky.cn

Go:   if x == nil {}
来源：http://rs.chemitech.net.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ty.panjiajie.cn

C#:   if (x is null) {}
来源：http://ag.muxihuayi.cn

[P07] 防抖与节流
来源：http://wi.yuntaijiaju.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://aj.shxzukj.cn

PHP:  // 手写时间戳比较
来源：http://bn.wgjwhj.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qb.yuntaijiaju.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qk.huixinmuqiang.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://cl.huanxung.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://bd.szxytkj.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://yk.shxzskj.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://lk.colortex.cn

[P08] 处理浮点精度问题
来源：http://bk.wgjwhj.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://aw.muxihuayi.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mc.shxzskj.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://dp.lnxyls.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://tf.wgjwhj.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ih.panjiajie.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://yw.huixinmuqiang.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://fr.yuexingan06.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://uk.hahajie.cn

================================================================================
来源：http://in.huixinmuqiang.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://oi.panjiajie.cn

================================================================================
来源：http://oo.panjiajie.cn

[Q01] 创建表
来源：http://fr.muxihuayi.cn

CREATE TABLE users (
来源：http://gu.wgjwhj.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://yr.9csxet.cn

name VARCHAR(50) NOT NULL,
来源：http://ql.newstarts.cn

email VARCHAR(100) UNIQUE,
来源：http://zr.bjjhwx.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://pz.haigaiapp.cn

);
来源：http://xr.yuntaijiaju.cn

[Q02] 创建带外键的表
来源：http://bi.gzmigu.cn

CREATE TABLE orders (
来源：http://su.521024.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ah.wgjwhj.cn

user_id INT NOT NULL,
来源：http://cy.hahajie.cn

amount DECIMAL(10, 2),
来源：http://gm.lnxyls.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://zb.jianghongdianzi.cn

);
来源：http://ts.hahajie.cn

[Q03] 增加列
来源：http://kx.521024.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://lt.chemitech.net.cn

[Q04] 修改列类型
来源：http://my.huixinmuqiang.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ie.szsharing.cn

[Q05] 重命名列
来源：http://oj.bookmarksfly.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://oc.521024.cn

[Q06] 删除列
来源：http://km.szxytkj.cn


<!-- 参考信息 -->