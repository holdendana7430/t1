代发 wailian999

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://gg.asd995.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://rm.bjjhwx.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://tz.9csxet.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://vh.huixinmuqiang.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hx.szxytkj.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://xz.nicolike.cn

Ruby: system("ls -l");  `ls -l`
来源：http://dv.wgjwhj.cn

C#:   Process.Start("ls", "-l");
来源：http://ko.521024.cn

[M04] 获取当前工作目录
来源：http://fm.nicolike.cn

Py:   os.getcwd()
来源：http://gh.asd995.cn

PHP:  getcwd();
来源：http://fc.jctech888.com.cn

JS:   process.cwd()
来源：http://mi.panjiajie.cn

TS:   process.cwd()
来源：http://pk.newstarts.cn

Java: Path.of("").toAbsolutePath()
来源：http://oz.gzmigu.cn

Go:   os.Getwd()
来源：http://sl.shxzskj.cn

Ruby: Dir.pwd
来源：http://cw.jctech888.com.cn

C#:   Directory.GetCurrentDirectory()
来源：http://cx.hnjuh.cn

[M05] 设置退出码
来源：http://sv.haigaiapp.cn

Py:   sys.exit(1)
来源：http://ll.521024.cn

PHP:  exit(1);
来源：http://vx.szsharing.cn

JS:   process.exit(1)
来源：http://wx.haigaiapp.cn

TS:   process.exit(1)
来源：http://zt.huixinmuqiang.cn

Java: System.exit(1)
来源：http://kv.yuntaijiaju.cn

Go:   os.Exit(1)
来源：http://ql.panjiajie.cn

Ruby: exit 1
来源：http://sz.huixiangedu.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://iz.newstarts.cn

[M06] 向标准错误输出
来源：http://dp.chemitech.net.cn

Py:   print("err", file=sys.stderr)
来源：http://oi.shtwfgs.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://oo.colortex.cn

JS:   console.error("err")
来源：http://qb.szxytkj.cn

TS:   console.error("err")
来源：http://zj.gzmigu.cn

Java: System.err.println("err")
来源：http://hm.haigaiapp.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ck.newstarts.cn

Ruby: warn "err"
来源：http://va.asd995.cn

C#:   Console.Error.WriteLine("err")
来源：http://my.hahajie.cn

[M07] 判断是否为主入口
来源：http://ys.nicolike.cn

Py:   if __name__ == "__main__":
来源：http://hz.jctech888.com.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ez.yuexingan06.cn

JS:   require.main === module
来源：http://pw.wgjwhj.cn

TS:   require.main === module
来源：http://ry.bjjhwx.cn

Java: public static void main(String[] args)
来源：http://cj.muxihuayi.cn

Go:   func main()
来源：http://af.gzmigu.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://do.521024.cn

C#:   static void Main(string[] args)
来源：http://an.szsharing.cn

[M08] 获取系统与运行时信息
来源：http://pq.shxzskj.cn

Py:   platform.system();  platform.python_version()
来源：http://fb.shxzukj.cn

PHP:  PHP_OS;  phpversion();
来源：http://av.9csxet.cn

JS:   process.platform;  process.version
来源：http://wr.521024.cn

TS:   process.platform;  process.version
来源：http://pj.muxihuayi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://nv.nicolike.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://yq.shxzukj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://vx.muxihuayi.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://dh.colortex.cn

================================================================================
来源：http://jq.jctech888.com.cn

N. 数据结构与算法
来源：http://ng.panjiajie.cn

================================================================================
来源：http://jr.shxzskj.cn

[N01] 二分查找（有序数组）
来源：http://nx.bjjhwx.cn

Py:   bisect.bisect_left(arr, x)
来源：http://gg.huanxung.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://fo.bjjhwx.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wr.jianghongdianzi.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jp.bookmarksfly.cn

Java: Arrays.binarySearch(arr, x)
来源：http://bc.asd995.cn

Go:   sort.SearchInts(arr, x)
来源：http://hr.panjiajie.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://nx.muxihuayi.cn

C#:   Array.BinarySearch(arr, x)
来源：http://og.nicolike.cn

[N02] 排序（工程实践用内置实现）
来源：http://jk.lnxyls.cn

Py:   sorted(arr);  arr.sort()
来源：http://kl.nszjky.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ud.jianghongdianzi.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://xv.hnjuh.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://yw.szsharing.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ex.huixinmuqiang.cn

Go:   slices.Sort(arr)
来源：http://xg.newstarts.cn

Ruby: arr.sort
来源：http://ec.newstarts.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ki.hahajie.cn

[N03] 快速排序（分治示例）
来源：http://ya.shxzskj.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://up.hnjuh.cn

PHP:  // 递归实现，或用 usort
来源：http://ka.jianghongdianzi.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jb.521024.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ls.wgjwhj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://jt.huixiangedu.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://af.shxzukj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ua.shxzukj.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ix.huixiangedu.cn

[N04] 斐波那契数列
来源：http://er.bjjhwx.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://lc.521024.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://xx.shxzskj.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fu.hahajie.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zx.szsharing.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://so.gzmigu.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://vd.muxihuayi.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://vd.nszjky.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://yz.panjiajie.cn

[N05] 最大公约数
来源：http://pg.asd995.cn

Py:   math.gcd(a, b)
来源：http://hp.wgjwhj.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ip.asd995.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ir.huixiangedu.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gt.huixinmuqiang.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://gh.shxzukj.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://gg.huixiangedu.cn

Ruby: a.gcd(b)
来源：http://fb.jianghongdianzi.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://jl.panjiajie.cn

[N06] 判断回文字符串
来源：http://tq.9csxet.cn

Py:   s == s[::-1]
来源：http://kv.shxzukj.cn

PHP:  $s === strrev($s);
来源：http://sg.lnxyls.cn

JS:   s === [...s].reverse().join("")
来源：http://ir.huixiangedu.cn

TS:   s === [...s].reverse().join("")
来源：http://sv.jianghongdianzi.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://kv.9csxet.cn

Go:   // 双指针从两端比较
来源：http://ee.asd995.cn

Ruby: s == s.reverse
来源：http://lc.wgjwhj.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://zi.haigaiapp.cn

[N07] 两数之和（返回下标）
来源：http://na.newstarts.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://zl.gzmigu.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://xa.colortex.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ev.hnjuh.cn

TS:   // 手写 Map<string, number>
来源：http://sh.yuexingan06.cn

Java: // 手写 HashMap
来源：http://yx.haigaiapp.cn

Go:   // 手写 map[int]int
来源：http://sq.huanxung.cn

Ruby: // 手写 Hash
来源：http://ur.gzmigu.cn

C#:   // 手写 Dictionary<int, int>
来源：http://pq.hnjuh.cn

[N08] 生成全排列
来源：http://gg.szsharing.cn

Py:   itertools.permutations(arr)
来源：http://gu.gzmigu.cn

PHP:  // 手写递归交换
来源：http://ct.szsharing.cn

JS:   // 手写回溯递归
来源：http://hm.jianghongdianzi.cn

TS:   // 手写回溯递归
来源：http://yc.bjjhwx.cn

Java: // 手写回溯递归
来源：http://fp.haigaiapp.cn

Go:   // 手写回溯递归
来源：http://yu.chemitech.net.cn

Ruby: arr.permutation.to_a
来源：http://ql.panjiajie.cn

C#:   // 手写回溯递归
来源：http://tl.haigaiapp.cn

[N09] 栈与队列
来源：http://rt.gzmigu.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://bj.chemitech.net.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://fv.jctech888.com.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://qs.hnjuh.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://sq.chemitech.net.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://rf.nicolike.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://jo.hahajie.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://tu.szxytkj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ea.huanxung.cn

[N10] 链表节点定义
来源：http://fj.chemitech.net.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wv.jctech888.com.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://oo.bjjhwx.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://kz.hahajie.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ag.haigaiapp.cn

Java: class Node { int v; Node next; }
来源：http://af.shtwfgs.cn

Go:   type Node struct { V int; Next *Node }
来源：http://up.haigaiapp.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://kf.shxzskj.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://oj.nicolike.cn

[N11] 二叉树中序遍历
来源：http://ex.yuntaijiaju.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://lv.huixinmuqiang.cn

PHP:  // 手写递归函数
来源：http://qt.hnjuh.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tz.szsharing.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ys.colortex.cn

Java: // 手写递归
来源：http://nt.bjjhwx.cn

Go:   // 手写递归
来源：http://fd.shxzukj.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mf.yuntaijiaju.cn

C#:   // 手写递归
来源：http://du.hnjuh.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://yf.yuexingan06.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://qb.newstarts.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mj.chemitech.net.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yd.panjiajie.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ht.haigaiapp.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wr.newstarts.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hi.yuexingan06.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://do.muxihuayi.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wh.yuexingan06.cn

================================================================================
来源：http://ok.shtwfgs.cn

O. 并发与异步
来源：http://dv.huanxung.cn

================================================================================
来源：http://hb.yuexingan06.cn

[O01] 启动一个线程
来源：http://qr.huanxung.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://kx.shxzskj.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://do.szsharing.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ql.panjiajie.cn

TS:   // 同 JS
来源：http://jv.huanxung.cn

Java: new Thread(() -> f()).start()
来源：http://wx.9csxet.cn

Go:   go f()
来源：http://rz.shxzskj.cn

Ruby: Thread.new { f }
来源：http://id.haigaiapp.cn

C#:   Task.Run(() => F());
来源：http://fv.nicolike.cn

[O02] 使用线程池
来源：http://eu.lnxyls.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://gf.jianghongdianzi.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ub.bookmarksfly.cn

JS:   // worker_threads 线程池
来源：http://er.yuntaijiaju.cn

TS:   // worker_threads 线程池
来源：http://wd.nicolike.cn

Java: Executors.newFixedThreadPool(4)
来源：http://sd.shxzskj.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://fz.szsharing.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ql.nicolike.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://sw.shxzukj.cn

[O03] 加锁保护共享数据
来源：http://rl.nicolike.cn

Py:   with lock: shared += 1
来源：http://ur.9csxet.cn

PHP:  // 用 flock() 做文件锁
来源：http://mr.bjjhwx.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://yv.panjiajie.cn

TS:   // 同 JS
来源：http://sk.shxzukj.cn

Java: synchronized (this) { shared++; }
来源：http://mu.gzmigu.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ha.gzmigu.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://hk.haigaiapp.cn

C#:   lock (gate) { shared++; }
来源：http://zu.asd995.cn

[O04] 定义异步函数并等待
来源：http://dn.yuexingan06.cn

Py:   async def f():⏎    await g()
来源：http://ft.yuexingan06.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://lw.shxzukj.cn

JS:   async function f() { await g(); }
来源：http://jy.nicolike.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://wn.yuexingan06.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mt.szsharing.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ea.lnxyls.cn

Ruby: # 用 Fiber 或 async gem
来源：http://re.haigaiapp.cn

C#:   async Task F() { await G(); }
来源：http://rr.lnxyls.cn

[O05] 并发执行并等待全部完成
来源：http://xc.huixiangedu.cn

Py:   asyncio.gather(*tasks)
来源：http://mk.lnxyls.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://fb.jianghongdianzi.cn

JS:   await Promise.all(tasks)
来源：http://tg.gzmigu.cn

TS:   await Promise.all(tasks)
来源：http://pc.huixiangedu.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://vv.panjiajie.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://fy.muxihuayi.cn

Ruby: threads.map(&:join)
来源：http://fe.521024.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://gv.521024.cn

[O06] 使用进程池
来源：http://tl.huixiangedu.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ok.panjiajie.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://pa.chemitech.net.cn

JS:   // child_process / cluster 模块
来源：http://py.nicolike.cn

TS:   // child_process / cluster 模块
来源：http://fp.gzmigu.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://nx.shtwfgs.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://zq.jctech888.com.cn

Ruby: // fork 块
来源：http://ri.shtwfgs.cn

C#:   Parallel.For
来源：http://gd.nicolike.cn

================================================================================
来源：http://vw.yuntaijiaju.cn

P. 常用工具函数
来源：http://re.9csxet.cn

================================================================================
来源：http://ih.chemitech.net.cn

[P01] 生成 UUID
来源：http://qu.newstarts.cn

Py:   str(uuid.uuid4())
来源：http://yq.lnxyls.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://fa.muxihuayi.cn

JS:   crypto.randomUUID()
来源：http://uz.hahajie.cn

TS:   crypto.randomUUID()
来源：http://bg.wgjwhj.cn

Java: UUID.randomUUID().toString()
来源：http://zq.wgjwhj.cn

Go:   // 用 github.com/google/uuid
来源：http://gn.nicolike.cn

Ruby: SecureRandom.uuid
来源：http://id.huixinmuqiang.cn

C#:   Guid.NewGuid().ToString()
来源：http://ii.haigaiapp.cn

[P02] MD5 / SHA256 摘要
来源：http://ch.chemitech.net.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://pr.nszjky.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://av.yuntaijiaju.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://xp.huixiangedu.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://qe.newstarts.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://bt.huixiangedu.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://vh.shxzukj.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ys.muxihuayi.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://gu.huixiangedu.cn

[P03] 生成短随机字符串
来源：http://kj.521024.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://qq.lnxyls.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://yl.bookmarksfly.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vm.jianghongdianzi.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pm.hnjuh.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://zq.shxzukj.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://xo.haigaiapp.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://mx.jianghongdianzi.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ce.panjiajie.cn

[P04] 求长度
来源：http://ko.huixinmuqiang.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mx.bookmarksfly.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ko.szsharing.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qf.lnxyls.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cd.521024.cn

Java: list.size();  map.size();  s.length()
来源：http://fd.yuexingan06.cn

Go:   len(arr);  len(m)
来源：http://wh.jctech888.com.cn

Ruby: x.length;  x.size
来源：http://fv.hahajie.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://hw.jianghongdianzi.cn

[P05] 判断两个对象内容是否相等
来源：http://ez.shxzskj.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://di.yuexingan06.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://um.muxihuayi.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://xg.bookmarksfly.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://me.newstarts.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://jp.huanxung.cn

Go:   reflect.DeepEqual(a, b)
来源：http://qt.huixinmuqiang.cn

Ruby: a == b
来源：http://ca.wgjwhj.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://vk.nszjky.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://tu.bjjhwx.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://pe.hnjuh.cn

PHP:  if (empty($x)) {}
来源：http://sy.bookmarksfly.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://dh.szxytkj.cn

TS:   if (x == null) {}
来源：http://ho.szsharing.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ie.shxzskj.cn

Go:   if x == nil {}
来源：http://oz.szxytkj.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://gb.9csxet.cn

C#:   if (x is null) {}
来源：http://dh.huixiangedu.cn

[P07] 防抖与节流
来源：http://qu.huixiangedu.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mk.chemitech.net.cn

PHP:  // 手写时间戳比较
来源：http://up.wgjwhj.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cj.szsharing.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nr.lnxyls.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://aq.colortex.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://as.szsharing.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://kb.hahajie.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://zf.bjjhwx.cn

[P08] 处理浮点精度问题
来源：http://jf.yuntaijiaju.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ar.gzmigu.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://kw.yuntaijiaju.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://no.hnjuh.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://dw.newstarts.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://uh.yuntaijiaju.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ip.szxytkj.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://fo.shtwfgs.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://vu.9csxet.cn

================================================================================
来源：http://jm.shtwfgs.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://eg.shxzukj.cn

================================================================================
来源：http://oa.wgjwhj.cn

[Q01] 创建表
来源：http://oo.newstarts.cn


<!-- 参考信息 -->