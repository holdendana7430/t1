代发 wailian999

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://st.muxihuayi.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://tl.newstarts.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://xb.nszjky.cn

[L06] 解析响应为 JSON
来源：http://lp.yuntaijiaju.cn

Py:   resp.json()
来源：http://ev.shxzskj.cn

PHP:  json_decode($body, true);
来源：http://no.colortex.cn

JS:   await resp.json()
来源：http://je.521024.cn

TS:   await resp.json()
来源：http://qh.szsharing.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://rg.shxzskj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://nx.huixinmuqiang.cn

Ruby: JSON.parse(resp.body)
来源：http://vm.hnjuh.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://aj.newstarts.cn

[L07] 处理 HTTP 状态码
来源：http://fv.szxytkj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://xd.bjjhwx.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://dm.nszjky.cn

JS:   resp.ok;  resp.status
来源：http://om.shtwfgs.cn

TS:   resp.ok;  resp.status
来源：http://jm.bookmarksfly.cn

Java: resp.statusCode()
来源：http://kw.521024.cn

Go:   resp.StatusCode
来源：http://ob.jianghongdianzi.cn

Ruby: resp.code.to_i
来源：http://po.asd995.cn

C#:   (int)resp.StatusCode
来源：http://xm.panjiajie.cn

[L08] 并发请求多个地址
来源：http://ca.muxihuayi.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hn.colortex.cn

PHP:  curl_multi_init() 系列
来源：http://wj.jctech888.com.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://so.yuntaijiaju.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bz.gzmigu.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://qw.nicolike.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ye.wgjwhj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ji.hahajie.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://iv.szxytkj.cn

================================================================================
来源：http://wx.521024.cn

M. 命令行 / 进程 / 环境
来源：http://qn.bjjhwx.cn

================================================================================
来源：http://zt.jctech888.com.cn

[M01] 读取命令行参数
来源：http://bo.bjjhwx.cn

Py:   sys.argv[1:]
来源：http://kh.9csxet.cn

PHP:  $argv;  $argc;
来源：http://pc.nicolike.cn

JS:   process.argv.slice(2)
来源：http://nf.shxzukj.cn

TS:   process.argv.slice(2)
来源：http://wi.huanxung.cn

Java: args 数组（main 方法参数）
来源：http://qp.shxzskj.cn

Go:   os.Args[1:]
来源：http://hv.wgjwhj.cn

Ruby: ARGV
来源：http://vx.chemitech.net.cn

C#:   args 数组（Main 方法参数）
来源：http://of.huixinmuqiang.cn

[M02] 读取环境变量
来源：http://eg.shxzukj.cn

Py:   os.environ.get("HOME")
来源：http://ds.wgjwhj.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wo.huanxung.cn

JS:   process.env.HOME
来源：http://by.panjiajie.cn

TS:   process.env.HOME
来源：http://gc.szsharing.cn

Java: System.getenv("HOME")
来源：http://qr.hnjuh.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://fl.shtwfgs.cn

Ruby: ENV["HOME"]
来源：http://zy.hnjuh.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://er.hnjuh.cn

[M03] 执行外部命令
来源：http://ds.shxzskj.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://uz.jctech888.com.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://vn.bookmarksfly.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://gs.shxzskj.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://vu.haigaiapp.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ih.jianghongdianzi.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://lx.yuexingan06.cn

Ruby: system("ls -l");  `ls -l`
来源：http://we.nszjky.cn

C#:   Process.Start("ls", "-l");
来源：http://db.gzmigu.cn

[M04] 获取当前工作目录
来源：http://hu.huanxung.cn

Py:   os.getcwd()
来源：http://bp.asd995.cn

PHP:  getcwd();
来源：http://zi.jctech888.com.cn

JS:   process.cwd()
来源：http://ig.nszjky.cn

TS:   process.cwd()
来源：http://ha.yuexingan06.cn

Java: Path.of("").toAbsolutePath()
来源：http://gl.bookmarksfly.cn

Go:   os.Getwd()
来源：http://mo.9csxet.cn

Ruby: Dir.pwd
来源：http://oe.521024.cn

C#:   Directory.GetCurrentDirectory()
来源：http://fx.bookmarksfly.cn

[M05] 设置退出码
来源：http://bq.huixinmuqiang.cn

Py:   sys.exit(1)
来源：http://cz.yuntaijiaju.cn

PHP:  exit(1);
来源：http://el.nszjky.cn

JS:   process.exit(1)
来源：http://ca.huanxung.cn

TS:   process.exit(1)
来源：http://ke.521024.cn

Java: System.exit(1)
来源：http://uy.newstarts.cn

Go:   os.Exit(1)
来源：http://ze.jianghongdianzi.cn

Ruby: exit 1
来源：http://ki.chemitech.net.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://bz.haigaiapp.cn

[M06] 向标准错误输出
来源：http://ni.chemitech.net.cn

Py:   print("err", file=sys.stderr)
来源：http://vi.shxzukj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://du.muxihuayi.cn

JS:   console.error("err")
来源：http://rm.lnxyls.cn

TS:   console.error("err")
来源：http://uk.nszjky.cn

Java: System.err.println("err")
来源：http://su.9csxet.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hs.lnxyls.cn

Ruby: warn "err"
来源：http://zc.panjiajie.cn

C#:   Console.Error.WriteLine("err")
来源：http://qv.9csxet.cn

[M07] 判断是否为主入口
来源：http://au.panjiajie.cn

Py:   if __name__ == "__main__":
来源：http://kn.shtwfgs.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://nd.521024.cn

JS:   require.main === module
来源：http://vn.szsharing.cn

TS:   require.main === module
来源：http://dc.gzmigu.cn

Java: public static void main(String[] args)
来源：http://yk.yuexingan06.cn

Go:   func main()
来源：http://gk.haigaiapp.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://py.yuexingan06.cn

C#:   static void Main(string[] args)
来源：http://cv.wgjwhj.cn

[M08] 获取系统与运行时信息
来源：http://oh.panjiajie.cn

Py:   platform.system();  platform.python_version()
来源：http://js.yuexingan06.cn

PHP:  PHP_OS;  phpversion();
来源：http://ge.asd995.cn

JS:   process.platform;  process.version
来源：http://kn.gzmigu.cn

TS:   process.platform;  process.version
来源：http://pt.shxzukj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hj.yuntaijiaju.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://mv.yuexingan06.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wn.newstarts.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ry.colortex.cn

================================================================================
来源：http://lb.hahajie.cn

N. 数据结构与算法
来源：http://yw.gzmigu.cn

================================================================================
来源：http://yi.newstarts.cn

[N01] 二分查找（有序数组）
来源：http://zq.yuntaijiaju.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ns.hnjuh.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://uu.hnjuh.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sf.huixiangedu.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rt.hahajie.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ih.muxihuayi.cn

Go:   sort.SearchInts(arr, x)
来源：http://rk.panjiajie.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ee.yuntaijiaju.cn

C#:   Array.BinarySearch(arr, x)
来源：http://hk.gzmigu.cn

[N02] 排序（工程实践用内置实现）
来源：http://ni.jianghongdianzi.cn

Py:   sorted(arr);  arr.sort()
来源：http://tt.szxytkj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://tu.gzmigu.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://lr.nszjky.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ww.shxzskj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://lc.bjjhwx.cn

Go:   slices.Sort(arr)
来源：http://zh.panjiajie.cn

Ruby: arr.sort
来源：http://gd.chemitech.net.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://wx.huixiangedu.cn

[N03] 快速排序（分治示例）
来源：http://dm.huixiangedu.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://zc.huixiangedu.cn

PHP:  // 递归实现，或用 usort
来源：http://lu.bjjhwx.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://az.shxzukj.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ab.nicolike.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ay.asd995.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://cm.521024.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://nv.bookmarksfly.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ua.shtwfgs.cn

[N04] 斐波那契数列
来源：http://jm.asd995.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://yq.huixinmuqiang.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://gs.huanxung.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lf.szxytkj.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vw.jctech888.com.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://lf.haigaiapp.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://pr.shxzskj.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://qo.jianghongdianzi.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://kn.huanxung.cn

[N05] 最大公约数
来源：http://le.szxytkj.cn

Py:   math.gcd(a, b)
来源：http://tc.521024.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mn.jianghongdianzi.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hi.huanxung.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tn.jctech888.com.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://sr.szsharing.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://du.asd995.cn

Ruby: a.gcd(b)
来源：http://co.9csxet.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://zb.shxzskj.cn

[N06] 判断回文字符串
来源：http://bk.jctech888.com.cn

Py:   s == s[::-1]
来源：http://qr.newstarts.cn

PHP:  $s === strrev($s);
来源：http://xi.bjjhwx.cn

JS:   s === [...s].reverse().join("")
来源：http://mf.yuexingan06.cn

TS:   s === [...s].reverse().join("")
来源：http://bk.nicolike.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://lq.szxytkj.cn

Go:   // 双指针从两端比较
来源：http://kr.bjjhwx.cn

Ruby: s == s.reverse
来源：http://pv.yuntaijiaju.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://sn.bjjhwx.cn

[N07] 两数之和（返回下标）
来源：http://pv.yuntaijiaju.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://nk.chemitech.net.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://pr.panjiajie.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://fb.bjjhwx.cn

TS:   // 手写 Map<string, number>
来源：http://ui.shtwfgs.cn

Java: // 手写 HashMap
来源：http://da.asd995.cn

Go:   // 手写 map[int]int
来源：http://dr.shxzukj.cn

Ruby: // 手写 Hash
来源：http://bl.nszjky.cn

C#:   // 手写 Dictionary<int, int>
来源：http://wp.yuexingan06.cn

[N08] 生成全排列
来源：http://pu.521024.cn

Py:   itertools.permutations(arr)
来源：http://mb.hahajie.cn

PHP:  // 手写递归交换
来源：http://fn.9csxet.cn

JS:   // 手写回溯递归
来源：http://om.bookmarksfly.cn

TS:   // 手写回溯递归
来源：http://fe.shxzskj.cn

Java: // 手写回溯递归
来源：http://ql.hahajie.cn

Go:   // 手写回溯递归
来源：http://lo.newstarts.cn

Ruby: arr.permutation.to_a
来源：http://sc.colortex.cn

C#:   // 手写回溯递归
来源：http://sh.bookmarksfly.cn

[N09] 栈与队列
来源：http://xw.521024.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ah.chemitech.net.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://gl.jianghongdianzi.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://xe.jianghongdianzi.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ap.newstarts.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mw.wgjwhj.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ig.yuexingan06.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://db.szxytkj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://aa.bookmarksfly.cn

[N10] 链表节点定义
来源：http://wl.bjjhwx.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://uv.newstarts.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://md.jctech888.com.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://jq.jianghongdianzi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://um.gzmigu.cn

Java: class Node { int v; Node next; }
来源：http://vi.haigaiapp.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ne.shxzukj.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://lv.nicolike.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://oz.gzmigu.cn

[N11] 二叉树中序遍历
来源：http://bd.newstarts.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hp.hahajie.cn

PHP:  // 手写递归函数
来源：http://kj.lnxyls.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://up.colortex.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ct.shxzukj.cn

Java: // 手写递归
来源：http://pm.yuntaijiaju.cn

Go:   // 手写递归
来源：http://fv.colortex.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://fz.jctech888.com.cn

C#:   // 手写递归
来源：http://by.yuexingan06.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ad.hnjuh.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://bh.asd995.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://uc.nszjky.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xn.yuntaijiaju.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qe.asd995.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://tu.haigaiapp.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ze.bookmarksfly.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://zu.nicolike.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://oa.yuexingan06.cn

================================================================================
来源：http://qd.nicolike.cn

O. 并发与异步
来源：http://qq.colortex.cn

================================================================================
来源：http://pu.bjjhwx.cn

[O01] 启动一个线程
来源：http://wj.bookmarksfly.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://pe.panjiajie.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mb.szxytkj.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ir.jctech888.com.cn

TS:   // 同 JS
来源：http://kg.chemitech.net.cn

Java: new Thread(() -> f()).start()
来源：http://sa.chemitech.net.cn

Go:   go f()
来源：http://lr.521024.cn

Ruby: Thread.new { f }
来源：http://zb.wgjwhj.cn

C#:   Task.Run(() => F());
来源：http://ue.shxzukj.cn

[O02] 使用线程池
来源：http://ih.colortex.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://rs.haigaiapp.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ku.colortex.cn

JS:   // worker_threads 线程池
来源：http://ma.jianghongdianzi.cn

TS:   // worker_threads 线程池
来源：http://ie.shxzskj.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ml.521024.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ys.nszjky.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://he.muxihuayi.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://un.lnxyls.cn

[O03] 加锁保护共享数据
来源：http://ur.521024.cn

Py:   with lock: shared += 1
来源：http://ul.yuexingan06.cn

PHP:  // 用 flock() 做文件锁
来源：http://kj.jctech888.com.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://nl.lnxyls.cn

TS:   // 同 JS
来源：http://sj.bjjhwx.cn

Java: synchronized (this) { shared++; }
来源：http://ta.yuntaijiaju.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://bq.colortex.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://fr.521024.cn

C#:   lock (gate) { shared++; }
来源：http://qo.nszjky.cn

[O04] 定义异步函数并等待
来源：http://rb.shtwfgs.cn

Py:   async def f():⏎    await g()
来源：http://po.nszjky.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://zr.bookmarksfly.cn

JS:   async function f() { await g(); }
来源：http://rb.muxihuayi.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://gu.colortex.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://st.colortex.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://cd.jianghongdianzi.cn

Ruby: # 用 Fiber 或 async gem
来源：http://az.shxzukj.cn

C#:   async Task F() { await G(); }
来源：http://zg.huixinmuqiang.cn

[O05] 并发执行并等待全部完成
来源：http://sf.haigaiapp.cn

Py:   asyncio.gather(*tasks)
来源：http://ks.szsharing.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://fz.shxzukj.cn

JS:   await Promise.all(tasks)
来源：http://im.asd995.cn

TS:   await Promise.all(tasks)
来源：http://cu.nszjky.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://dm.gzmigu.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wr.gzmigu.cn

Ruby: threads.map(&:join)
来源：http://vs.shtwfgs.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://uv.yuntaijiaju.cn

[O06] 使用进程池
来源：http://te.nszjky.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://gh.hnjuh.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://mm.panjiajie.cn

JS:   // child_process / cluster 模块
来源：http://wh.huanxung.cn

TS:   // child_process / cluster 模块
来源：http://ku.huanxung.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ld.gzmigu.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://yc.huixiangedu.cn

Ruby: // fork 块
来源：http://yd.lnxyls.cn

C#:   Parallel.For
来源：http://ip.panjiajie.cn

================================================================================
来源：http://lz.lnxyls.cn

P. 常用工具函数
来源：http://ks.newstarts.cn

================================================================================
来源：http://am.haigaiapp.cn

[P01] 生成 UUID
来源：http://xe.nicolike.cn

Py:   str(uuid.uuid4())
来源：http://vc.muxihuayi.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://nk.lnxyls.cn

JS:   crypto.randomUUID()
来源：http://qo.hahajie.cn

TS:   crypto.randomUUID()
来源：http://sd.huixinmuqiang.cn

Java: UUID.randomUUID().toString()
来源：http://rm.wgjwhj.cn

Go:   // 用 github.com/google/uuid
来源：http://co.asd995.cn

Ruby: SecureRandom.uuid
来源：http://mp.chemitech.net.cn

C#:   Guid.NewGuid().ToString()
来源：http://tq.shxzskj.cn

[P02] MD5 / SHA256 摘要
来源：http://jj.panjiajie.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://zu.bjjhwx.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://nu.szsharing.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://vb.bookmarksfly.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://xq.jctech888.com.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mj.huixinmuqiang.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://es.panjiajie.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://lg.shxzukj.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hl.shxzskj.cn

[P03] 生成短随机字符串
来源：http://hi.yuntaijiaju.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://jo.wgjwhj.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://la.haigaiapp.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ye.nszjky.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://sw.yuntaijiaju.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://bc.shxzskj.cn


<!-- 参考信息 -->