代发 wailian999

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://up.jianghongdianzi.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://pm.shtwfgs.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://js.jctech888.com.cn

[L06] 解析响应为 JSON
来源：http://wn.jctech888.com.cn

Py:   resp.json()
来源：http://fu.jianghongdianzi.cn

PHP:  json_decode($body, true);
来源：http://ix.huixinmuqiang.cn

JS:   await resp.json()
来源：http://ed.newstarts.cn

TS:   await resp.json()
来源：http://sv.shtwfgs.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://on.panjiajie.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://vz.panjiajie.cn

Ruby: JSON.parse(resp.body)
来源：http://yt.jianghongdianzi.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://dk.yuexingan06.cn

[L07] 处理 HTTP 状态码
来源：http://ei.nszjky.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ww.hnjuh.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://yi.huixiangedu.cn

JS:   resp.ok;  resp.status
来源：http://bi.jianghongdianzi.cn

TS:   resp.ok;  resp.status
来源：http://wr.szsharing.cn

Java: resp.statusCode()
来源：http://ja.shxzukj.cn

Go:   resp.StatusCode
来源：http://ty.panjiajie.cn

Ruby: resp.code.to_i
来源：http://db.hahajie.cn

C#:   (int)resp.StatusCode
来源：http://bu.wgjwhj.cn

[L08] 并发请求多个地址
来源：http://rx.jianghongdianzi.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://va.huanxung.cn

PHP:  curl_multi_init() 系列
来源：http://th.chemitech.net.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ru.shxzukj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jt.521024.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://jf.huanxung.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://lh.asd995.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hl.huanxung.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://zi.9csxet.cn

================================================================================
来源：http://tm.asd995.cn

M. 命令行 / 进程 / 环境
来源：http://qk.jctech888.com.cn

================================================================================
来源：http://vn.asd995.cn

[M01] 读取命令行参数
来源：http://pr.haigaiapp.cn

Py:   sys.argv[1:]
来源：http://kh.bjjhwx.cn

PHP:  $argv;  $argc;
来源：http://ww.newstarts.cn

JS:   process.argv.slice(2)
来源：http://sj.haigaiapp.cn

TS:   process.argv.slice(2)
来源：http://il.yuexingan06.cn

Java: args 数组（main 方法参数）
来源：http://kk.521024.cn

Go:   os.Args[1:]
来源：http://rp.lnxyls.cn

Ruby: ARGV
来源：http://yb.hahajie.cn

C#:   args 数组（Main 方法参数）
来源：http://yq.lnxyls.cn

[M02] 读取环境变量
来源：http://ds.yuexingan06.cn

Py:   os.environ.get("HOME")
来源：http://mj.jctech888.com.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ac.chemitech.net.cn

JS:   process.env.HOME
来源：http://yu.haigaiapp.cn

TS:   process.env.HOME
来源：http://ar.gzmigu.cn

Java: System.getenv("HOME")
来源：http://qj.lnxyls.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://jy.huixiangedu.cn

Ruby: ENV["HOME"]
来源：http://bi.hnjuh.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://nf.yuexingan06.cn

[M03] 执行外部命令
来源：http://dk.hnjuh.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://dt.newstarts.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://tm.bjjhwx.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://kh.panjiajie.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://rb.newstarts.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://rl.huixinmuqiang.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://pc.colortex.cn

Ruby: system("ls -l");  `ls -l`
来源：http://bh.hahajie.cn

C#:   Process.Start("ls", "-l");
来源：http://gs.asd995.cn

[M04] 获取当前工作目录
来源：http://kc.szxytkj.cn

Py:   os.getcwd()
来源：http://oz.521024.cn

PHP:  getcwd();
来源：http://bb.szxytkj.cn

JS:   process.cwd()
来源：http://xj.huanxung.cn

TS:   process.cwd()
来源：http://lq.colortex.cn

Java: Path.of("").toAbsolutePath()
来源：http://oa.lnxyls.cn

Go:   os.Getwd()
来源：http://sv.hnjuh.cn

Ruby: Dir.pwd
来源：http://jx.wgjwhj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://by.szxytkj.cn

[M05] 设置退出码
来源：http://ou.szxytkj.cn

Py:   sys.exit(1)
来源：http://zg.lnxyls.cn

PHP:  exit(1);
来源：http://uq.hnjuh.cn

JS:   process.exit(1)
来源：http://lw.9csxet.cn

TS:   process.exit(1)
来源：http://fn.panjiajie.cn

Java: System.exit(1)
来源：http://rp.huixiangedu.cn

Go:   os.Exit(1)
来源：http://cs.521024.cn

Ruby: exit 1
来源：http://uf.shtwfgs.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://uy.colortex.cn

[M06] 向标准错误输出
来源：http://zf.jianghongdianzi.cn

Py:   print("err", file=sys.stderr)
来源：http://lk.huixiangedu.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://bs.521024.cn

JS:   console.error("err")
来源：http://wf.521024.cn

TS:   console.error("err")
来源：http://km.bookmarksfly.cn

Java: System.err.println("err")
来源：http://es.szxytkj.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://zf.lnxyls.cn

Ruby: warn "err"
来源：http://oo.nszjky.cn

C#:   Console.Error.WriteLine("err")
来源：http://bt.bjjhwx.cn

[M07] 判断是否为主入口
来源：http://op.wgjwhj.cn

Py:   if __name__ == "__main__":
来源：http://am.hnjuh.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hg.huixinmuqiang.cn

JS:   require.main === module
来源：http://yg.bookmarksfly.cn

TS:   require.main === module
来源：http://us.nszjky.cn

Java: public static void main(String[] args)
来源：http://wx.nszjky.cn

Go:   func main()
来源：http://uu.panjiajie.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://vr.chemitech.net.cn

C#:   static void Main(string[] args)
来源：http://do.jctech888.com.cn

[M08] 获取系统与运行时信息
来源：http://yv.asd995.cn

Py:   platform.system();  platform.python_version()
来源：http://av.shxzukj.cn

PHP:  PHP_OS;  phpversion();
来源：http://nd.hahajie.cn

JS:   process.platform;  process.version
来源：http://zo.haigaiapp.cn

TS:   process.platform;  process.version
来源：http://hg.bjjhwx.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://bb.panjiajie.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://te.colortex.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://zj.chemitech.net.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://kw.shxzukj.cn

================================================================================
来源：http://yh.shtwfgs.cn

N. 数据结构与算法
来源：http://ri.bjjhwx.cn

================================================================================
来源：http://om.jianghongdianzi.cn

[N01] 二分查找（有序数组）
来源：http://lb.jctech888.com.cn

Py:   bisect.bisect_left(arr, x)
来源：http://zg.jianghongdianzi.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://vj.nszjky.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ry.yuntaijiaju.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rz.lnxyls.cn

Java: Arrays.binarySearch(arr, x)
来源：http://fm.shtwfgs.cn

Go:   sort.SearchInts(arr, x)
来源：http://ha.wgjwhj.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://tt.huanxung.cn

C#:   Array.BinarySearch(arr, x)
来源：http://tv.hnjuh.cn

[N02] 排序（工程实践用内置实现）
来源：http://qr.lnxyls.cn

Py:   sorted(arr);  arr.sort()
来源：http://qk.hahajie.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://cm.huanxung.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://qr.yuntaijiaju.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://rv.jctech888.com.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://qg.bookmarksfly.cn

Go:   slices.Sort(arr)
来源：http://go.hahajie.cn

Ruby: arr.sort
来源：http://tq.hahajie.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://im.lnxyls.cn

[N03] 快速排序（分治示例）
来源：http://cn.huixiangedu.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://xl.gzmigu.cn

PHP:  // 递归实现，或用 usort
来源：http://oj.yuexingan06.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vq.521024.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pk.nszjky.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://lg.521024.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://pa.bookmarksfly.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://bo.chemitech.net.cn

C#:   // 手写递归，或 Array.Sort
来源：http://vu.haigaiapp.cn

[N04] 斐波那契数列
来源：http://zk.shxzukj.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://fz.panjiajie.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://me.newstarts.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ce.521024.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://uo.newstarts.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://sv.bjjhwx.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ze.colortex.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://gd.shxzukj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://my.huixinmuqiang.cn

[N05] 最大公约数
来源：http://eh.shtwfgs.cn

Py:   math.gcd(a, b)
来源：http://ti.panjiajie.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://qk.haigaiapp.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pq.colortex.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bl.hahajie.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zs.colortex.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://cz.chemitech.net.cn

Ruby: a.gcd(b)
来源：http://zm.huixiangedu.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://fw.hahajie.cn

[N06] 判断回文字符串
来源：http://lh.szsharing.cn

Py:   s == s[::-1]
来源：http://oj.wgjwhj.cn

PHP:  $s === strrev($s);
来源：http://cm.nszjky.cn

JS:   s === [...s].reverse().join("")
来源：http://bp.yuntaijiaju.cn

TS:   s === [...s].reverse().join("")
来源：http://sq.huixiangedu.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://vz.shxzskj.cn

Go:   // 双指针从两端比较
来源：http://xd.yuntaijiaju.cn

Ruby: s == s.reverse
来源：http://wr.muxihuayi.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://tu.szsharing.cn

[N07] 两数之和（返回下标）
来源：http://fu.haigaiapp.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://oi.chemitech.net.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://xb.nicolike.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://jb.szsharing.cn

TS:   // 手写 Map<string, number>
来源：http://xv.9csxet.cn

Java: // 手写 HashMap
来源：http://vr.huixinmuqiang.cn

Go:   // 手写 map[int]int
来源：http://dt.huixinmuqiang.cn

Ruby: // 手写 Hash
来源：http://ym.colortex.cn

C#:   // 手写 Dictionary<int, int>
来源：http://xy.9csxet.cn

[N08] 生成全排列
来源：http://nv.nicolike.cn

Py:   itertools.permutations(arr)
来源：http://eb.shxzskj.cn

PHP:  // 手写递归交换
来源：http://yo.gzmigu.cn

JS:   // 手写回溯递归
来源：http://om.szsharing.cn

TS:   // 手写回溯递归
来源：http://ab.nicolike.cn

Java: // 手写回溯递归
来源：http://cr.9csxet.cn

Go:   // 手写回溯递归
来源：http://dt.hnjuh.cn

Ruby: arr.permutation.to_a
来源：http://rd.huixiangedu.cn

C#:   // 手写回溯递归
来源：http://gf.huixiangedu.cn

[N09] 栈与队列
来源：http://yt.jianghongdianzi.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://bs.colortex.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://de.521024.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://xh.muxihuayi.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://st.nszjky.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://og.chemitech.net.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://md.9csxet.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mj.colortex.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://di.jctech888.com.cn

[N10] 链表节点定义
来源：http://ha.newstarts.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://io.colortex.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ag.nszjky.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://pb.chemitech.net.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://py.hahajie.cn

Java: class Node { int v; Node next; }
来源：http://qg.shxzskj.cn

Go:   type Node struct { V int; Next *Node }
来源：http://wq.lnxyls.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://bu.yuexingan06.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://is.shtwfgs.cn

[N11] 二叉树中序遍历
来源：http://wp.huixinmuqiang.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://pb.jctech888.com.cn

PHP:  // 手写递归函数
来源：http://ui.hahajie.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xp.haigaiapp.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kz.wgjwhj.cn

Java: // 手写递归
来源：http://we.huixiangedu.cn

Go:   // 手写递归
来源：http://rw.wgjwhj.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://kf.muxihuayi.cn

C#:   // 手写递归
来源：http://yy.shxzukj.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ql.szxytkj.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://lg.jianghongdianzi.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wx.colortex.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sq.shtwfgs.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://si.huixinmuqiang.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://jg.bjjhwx.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://oi.asd995.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://yk.bookmarksfly.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ql.haigaiapp.cn

================================================================================
来源：http://au.yuntaijiaju.cn

O. 并发与异步
来源：http://yn.521024.cn

================================================================================
来源：http://xd.521024.cn

[O01] 启动一个线程
来源：http://xi.shxzukj.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://bb.hnjuh.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hm.panjiajie.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://lh.huixinmuqiang.cn

TS:   // 同 JS
来源：http://ay.bjjhwx.cn

Java: new Thread(() -> f()).start()
来源：http://zp.9csxet.cn

Go:   go f()
来源：http://qd.asd995.cn

Ruby: Thread.new { f }
来源：http://bv.yuexingan06.cn

C#:   Task.Run(() => F());
来源：http://oh.hnjuh.cn

[O02] 使用线程池
来源：http://xm.hahajie.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wr.haigaiapp.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wl.hnjuh.cn

JS:   // worker_threads 线程池
来源：http://ym.bjjhwx.cn

TS:   // worker_threads 线程池
来源：http://ku.nszjky.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ov.szxytkj.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://th.panjiajie.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://am.hnjuh.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ve.haigaiapp.cn

[O03] 加锁保护共享数据
来源：http://fn.colortex.cn

Py:   with lock: shared += 1
来源：http://fo.nicolike.cn

PHP:  // 用 flock() 做文件锁
来源：http://fu.shxzskj.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://fp.nicolike.cn

TS:   // 同 JS
来源：http://dm.hahajie.cn

Java: synchronized (this) { shared++; }
来源：http://aj.asd995.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ub.jianghongdianzi.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://mh.shtwfgs.cn

C#:   lock (gate) { shared++; }
来源：http://xv.jianghongdianzi.cn

[O04] 定义异步函数并等待
来源：http://it.yuntaijiaju.cn

Py:   async def f():⏎    await g()
来源：http://um.chemitech.net.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ci.muxihuayi.cn

JS:   async function f() { await g(); }
来源：http://jr.lnxyls.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://re.muxihuayi.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://xd.gzmigu.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://tj.panjiajie.cn

Ruby: # 用 Fiber 或 async gem
来源：http://sb.jctech888.com.cn

C#:   async Task F() { await G(); }
来源：http://yl.huixinmuqiang.cn

[O05] 并发执行并等待全部完成
来源：http://em.nszjky.cn

Py:   asyncio.gather(*tasks)
来源：http://ge.huixinmuqiang.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://xc.muxihuayi.cn

JS:   await Promise.all(tasks)
来源：http://gy.huixinmuqiang.cn

TS:   await Promise.all(tasks)
来源：http://nq.nicolike.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ql.bjjhwx.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mt.panjiajie.cn

Ruby: threads.map(&:join)
来源：http://dj.521024.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://lv.szsharing.cn

[O06] 使用进程池
来源：http://ay.panjiajie.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://rs.muxihuayi.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://og.9csxet.cn

JS:   // child_process / cluster 模块
来源：http://jf.chemitech.net.cn

TS:   // child_process / cluster 模块
来源：http://lb.lnxyls.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mw.muxihuayi.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://lf.jianghongdianzi.cn

Ruby: // fork 块
来源：http://kn.colortex.cn

C#:   Parallel.For
来源：http://af.bjjhwx.cn

================================================================================
来源：http://bp.chemitech.net.cn

P. 常用工具函数
来源：http://sy.haigaiapp.cn

================================================================================
来源：http://xb.newstarts.cn

[P01] 生成 UUID
来源：http://lj.hahajie.cn

Py:   str(uuid.uuid4())
来源：http://oz.jianghongdianzi.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ba.chemitech.net.cn

JS:   crypto.randomUUID()
来源：http://wg.szsharing.cn

TS:   crypto.randomUUID()
来源：http://ps.colortex.cn

Java: UUID.randomUUID().toString()
来源：http://hs.colortex.cn

Go:   // 用 github.com/google/uuid
来源：http://ub.chemitech.net.cn

Ruby: SecureRandom.uuid
来源：http://cx.shxzskj.cn

C#:   Guid.NewGuid().ToString()
来源：http://ey.jctech888.com.cn

[P02] MD5 / SHA256 摘要
来源：http://ds.lnxyls.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://vx.colortex.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://xv.colortex.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ij.shxzskj.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://xr.hahajie.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://co.lnxyls.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://nz.bookmarksfly.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wy.huixinmuqiang.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://fl.huixiangedu.cn

[P03] 生成短随机字符串
来源：http://wb.lnxyls.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ip.jctech888.com.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ix.muxihuayi.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ko.huanxung.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gh.huanxung.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://rj.nszjky.cn


<!-- 参考信息 -->