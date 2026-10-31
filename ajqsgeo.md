代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ae.panjiajie.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://un.jianghongdianzi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wp.gzmigu.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://zv.jianghongdianzi.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://rz.hahajie.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://zu.hnjuh.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ww.gzmigu.cn

[L06] 解析响应为 JSON
来源：http://jv.lnxyls.cn

Py:   resp.json()
来源：http://tk.nicolike.cn

PHP:  json_decode($body, true);
来源：http://ks.haigaiapp.cn

JS:   await resp.json()
来源：http://qe.nszjky.cn

TS:   await resp.json()
来源：http://dh.szsharing.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://cm.panjiajie.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://yo.9csxet.cn

Ruby: JSON.parse(resp.body)
来源：http://sx.9csxet.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://du.lnxyls.cn

[L07] 处理 HTTP 状态码
来源：http://gk.521024.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://rn.nicolike.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://dm.jctech888.com.cn

JS:   resp.ok;  resp.status
来源：http://ot.asd995.cn

TS:   resp.ok;  resp.status
来源：http://nx.521024.cn

Java: resp.statusCode()
来源：http://dv.chemitech.net.cn

Go:   resp.StatusCode
来源：http://cb.chemitech.net.cn

Ruby: resp.code.to_i
来源：http://id.chemitech.net.cn

C#:   (int)resp.StatusCode
来源：http://lz.wgjwhj.cn

[L08] 并发请求多个地址
来源：http://bh.panjiajie.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://un.lnxyls.cn

PHP:  curl_multi_init() 系列
来源：http://vw.bookmarksfly.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qy.jctech888.com.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://so.huanxung.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://zu.521024.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://az.9csxet.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://gi.jctech888.com.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://kf.szxytkj.cn

================================================================================
来源：http://yw.szxytkj.cn

M. 命令行 / 进程 / 环境
来源：http://xe.shxzskj.cn

================================================================================
来源：http://uu.yuexingan06.cn

[M01] 读取命令行参数
来源：http://wd.huixiangedu.cn

Py:   sys.argv[1:]
来源：http://cz.muxihuayi.cn

PHP:  $argv;  $argc;
来源：http://hs.haigaiapp.cn

JS:   process.argv.slice(2)
来源：http://tm.huanxung.cn

TS:   process.argv.slice(2)
来源：http://pv.bjjhwx.cn

Java: args 数组（main 方法参数）
来源：http://ou.bjjhwx.cn

Go:   os.Args[1:]
来源：http://fg.hahajie.cn

Ruby: ARGV
来源：http://qf.shxzskj.cn

C#:   args 数组（Main 方法参数）
来源：http://fu.huanxung.cn

[M02] 读取环境变量
来源：http://hk.bjjhwx.cn

Py:   os.environ.get("HOME")
来源：http://ne.panjiajie.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://xl.szsharing.cn

JS:   process.env.HOME
来源：http://tp.wgjwhj.cn

TS:   process.env.HOME
来源：http://bp.jctech888.com.cn

Java: System.getenv("HOME")
来源：http://tg.hahajie.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://lo.nicolike.cn

Ruby: ENV["HOME"]
来源：http://zm.lnxyls.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://sr.szsharing.cn

[M03] 执行外部命令
来源：http://dz.chemitech.net.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://uc.asd995.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://pz.hnjuh.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ga.chemitech.net.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://gr.shxzukj.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://nu.szxytkj.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://wf.chemitech.net.cn

Ruby: system("ls -l");  `ls -l`
来源：http://yw.huixiangedu.cn

C#:   Process.Start("ls", "-l");
来源：http://gq.hahajie.cn

[M04] 获取当前工作目录
来源：http://yu.muxihuayi.cn

Py:   os.getcwd()
来源：http://aq.nszjky.cn

PHP:  getcwd();
来源：http://ou.jianghongdianzi.cn

JS:   process.cwd()
来源：http://kj.wgjwhj.cn

TS:   process.cwd()
来源：http://qi.hnjuh.cn

Java: Path.of("").toAbsolutePath()
来源：http://lf.panjiajie.cn

Go:   os.Getwd()
来源：http://ds.hahajie.cn

Ruby: Dir.pwd
来源：http://cw.shxzskj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://oy.shxzukj.cn

[M05] 设置退出码
来源：http://wi.szxytkj.cn

Py:   sys.exit(1)
来源：http://xk.huixiangedu.cn

PHP:  exit(1);
来源：http://hl.haigaiapp.cn

JS:   process.exit(1)
来源：http://hl.bjjhwx.cn

TS:   process.exit(1)
来源：http://fu.wgjwhj.cn

Java: System.exit(1)
来源：http://jh.yuntaijiaju.cn

Go:   os.Exit(1)
来源：http://xi.asd995.cn

Ruby: exit 1
来源：http://ml.nszjky.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://cq.szsharing.cn

[M06] 向标准错误输出
来源：http://by.huixiangedu.cn

Py:   print("err", file=sys.stderr)
来源：http://ar.lnxyls.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://gg.panjiajie.cn

JS:   console.error("err")
来源：http://bw.gzmigu.cn

TS:   console.error("err")
来源：http://dl.haigaiapp.cn

Java: System.err.println("err")
来源：http://no.9csxet.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://yw.jctech888.com.cn

Ruby: warn "err"
来源：http://oi.hnjuh.cn

C#:   Console.Error.WriteLine("err")
来源：http://oi.colortex.cn

[M07] 判断是否为主入口
来源：http://sh.panjiajie.cn

Py:   if __name__ == "__main__":
来源：http://fq.yuntaijiaju.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://vu.bookmarksfly.cn

JS:   require.main === module
来源：http://rk.hnjuh.cn

TS:   require.main === module
来源：http://lz.panjiajie.cn

Java: public static void main(String[] args)
来源：http://nw.wgjwhj.cn

Go:   func main()
来源：http://ws.bjjhwx.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://oz.newstarts.cn

C#:   static void Main(string[] args)
来源：http://am.panjiajie.cn

[M08] 获取系统与运行时信息
来源：http://eg.bjjhwx.cn

Py:   platform.system();  platform.python_version()
来源：http://if.jianghongdianzi.cn

PHP:  PHP_OS;  phpversion();
来源：http://km.lnxyls.cn

JS:   process.platform;  process.version
来源：http://nz.bookmarksfly.cn

TS:   process.platform;  process.version
来源：http://qc.bjjhwx.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://cb.bjjhwx.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ce.gzmigu.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://cx.shxzukj.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://gu.huanxung.cn

================================================================================
来源：http://rm.hnjuh.cn

N. 数据结构与算法
来源：http://xb.jianghongdianzi.cn

================================================================================
来源：http://ye.haigaiapp.cn

[N01] 二分查找（有序数组）
来源：http://rh.nicolike.cn

Py:   bisect.bisect_left(arr, x)
来源：http://qw.hahajie.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://no.yuexingan06.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qz.bookmarksfly.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rp.panjiajie.cn

Java: Arrays.binarySearch(arr, x)
来源：http://xg.9csxet.cn

Go:   sort.SearchInts(arr, x)
来源：http://jf.jianghongdianzi.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://nu.colortex.cn

C#:   Array.BinarySearch(arr, x)
来源：http://zw.yuexingan06.cn

[N02] 排序（工程实践用内置实现）
来源：http://kk.bjjhwx.cn

Py:   sorted(arr);  arr.sort()
来源：http://lm.shxzukj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://zm.huixinmuqiang.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://nq.nicolike.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://qm.bjjhwx.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ek.huixinmuqiang.cn

Go:   slices.Sort(arr)
来源：http://ws.jctech888.com.cn

Ruby: arr.sort
来源：http://va.521024.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://xf.chemitech.net.cn

[N03] 快速排序（分治示例）
来源：http://ku.jctech888.com.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://cg.shtwfgs.cn

PHP:  // 递归实现，或用 usort
来源：http://eq.shxzukj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xc.shtwfgs.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qg.wgjwhj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ps.521024.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://cj.gzmigu.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ze.huixinmuqiang.cn

C#:   // 手写递归，或 Array.Sort
来源：http://kj.bjjhwx.cn

[N04] 斐波那契数列
来源：http://yk.panjiajie.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://af.huixinmuqiang.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://cf.gzmigu.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sa.nicolike.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ew.bjjhwx.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://dj.shxzukj.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://fc.szxytkj.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://bd.szxytkj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://lw.lnxyls.cn

[N05] 最大公约数
来源：http://of.shtwfgs.cn

Py:   math.gcd(a, b)
来源：http://kw.lnxyls.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://nz.asd995.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xe.shtwfgs.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ho.gzmigu.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://jm.huanxung.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://tz.jctech888.com.cn

Ruby: a.gcd(b)
来源：http://ta.panjiajie.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://cg.haigaiapp.cn

[N06] 判断回文字符串
来源：http://lx.yuntaijiaju.cn

Py:   s == s[::-1]
来源：http://zi.haigaiapp.cn

PHP:  $s === strrev($s);
来源：http://ii.asd995.cn

JS:   s === [...s].reverse().join("")
来源：http://mc.jianghongdianzi.cn

TS:   s === [...s].reverse().join("")
来源：http://gn.yuntaijiaju.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://kr.521024.cn

Go:   // 双指针从两端比较
来源：http://xw.nicolike.cn

Ruby: s == s.reverse
来源：http://fb.shxzskj.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://aw.haigaiapp.cn

[N07] 两数之和（返回下标）
来源：http://lz.hnjuh.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ig.szxytkj.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wy.nicolike.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://mj.521024.cn

TS:   // 手写 Map<string, number>
来源：http://cz.asd995.cn

Java: // 手写 HashMap
来源：http://rf.szxytkj.cn

Go:   // 手写 map[int]int
来源：http://ha.chemitech.net.cn

Ruby: // 手写 Hash
来源：http://og.521024.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ph.gzmigu.cn

[N08] 生成全排列
来源：http://vo.hnjuh.cn

Py:   itertools.permutations(arr)
来源：http://ck.nszjky.cn

PHP:  // 手写递归交换
来源：http://mg.lnxyls.cn

JS:   // 手写回溯递归
来源：http://bv.shxzukj.cn

TS:   // 手写回溯递归
来源：http://fl.hnjuh.cn

Java: // 手写回溯递归
来源：http://ga.szsharing.cn

Go:   // 手写回溯递归
来源：http://zj.gzmigu.cn

Ruby: arr.permutation.to_a
来源：http://vi.huixiangedu.cn

C#:   // 手写回溯递归
来源：http://cg.9csxet.cn

[N09] 栈与队列
来源：http://tc.huanxung.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://by.yuntaijiaju.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://jk.shtwfgs.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://uf.521024.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://en.muxihuayi.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://tn.huixinmuqiang.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://zw.newstarts.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://nq.wgjwhj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ru.asd995.cn

[N10] 链表节点定义
来源：http://km.wgjwhj.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://et.shxzskj.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://vn.asd995.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://vm.521024.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://xk.yuntaijiaju.cn

Java: class Node { int v; Node next; }
来源：http://di.szxytkj.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ws.huixinmuqiang.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://hr.huixiangedu.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://mi.jianghongdianzi.cn

[N11] 二叉树中序遍历
来源：http://fn.bookmarksfly.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://rl.hahajie.cn

PHP:  // 手写递归函数
来源：http://kn.szxytkj.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lv.521024.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://oh.szxytkj.cn

Java: // 手写递归
来源：http://gz.bookmarksfly.cn

Go:   // 手写递归
来源：http://ey.colortex.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ry.bookmarksfly.cn

C#:   // 手写递归
来源：http://xn.szsharing.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ej.nicolike.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://gd.yuntaijiaju.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://lo.yuexingan06.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sf.chemitech.net.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hk.haigaiapp.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ws.shxzukj.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://rc.shxzukj.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://rs.huixiangedu.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ok.bookmarksfly.cn

================================================================================
来源：http://wm.521024.cn

O. 并发与异步
来源：http://cs.chemitech.net.cn

================================================================================
来源：http://ul.panjiajie.cn

[O01] 启动一个线程
来源：http://ld.gzmigu.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://jm.chemitech.net.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://nt.hnjuh.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://fq.nszjky.cn

TS:   // 同 JS
来源：http://cq.bjjhwx.cn

Java: new Thread(() -> f()).start()
来源：http://jh.521024.cn

Go:   go f()
来源：http://oi.shxzukj.cn

Ruby: Thread.new { f }
来源：http://vj.gzmigu.cn

C#:   Task.Run(() => F());
来源：http://pr.szxytkj.cn

[O02] 使用线程池
来源：http://xh.shxzskj.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://aq.szxytkj.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hv.nszjky.cn

JS:   // worker_threads 线程池
来源：http://gd.colortex.cn

TS:   // worker_threads 线程池
来源：http://uu.9csxet.cn

Java: Executors.newFixedThreadPool(4)
来源：http://yj.bjjhwx.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://sz.9csxet.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://al.jianghongdianzi.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://lj.newstarts.cn

[O03] 加锁保护共享数据
来源：http://vv.gzmigu.cn

Py:   with lock: shared += 1
来源：http://ud.szxytkj.cn

PHP:  // 用 flock() 做文件锁
来源：http://dk.szsharing.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://pn.panjiajie.cn

TS:   // 同 JS
来源：http://qp.hnjuh.cn

Java: synchronized (this) { shared++; }
来源：http://lb.wgjwhj.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ty.yuntaijiaju.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://pz.szxytkj.cn

C#:   lock (gate) { shared++; }
来源：http://ub.bookmarksfly.cn

[O04] 定义异步函数并等待
来源：http://md.szsharing.cn

Py:   async def f():⏎    await g()
来源：http://of.bjjhwx.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://rn.shtwfgs.cn

JS:   async function f() { await g(); }
来源：http://nl.asd995.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://qu.szxytkj.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://xj.chemitech.net.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hh.bookmarksfly.cn

Ruby: # 用 Fiber 或 async gem
来源：http://jx.shtwfgs.cn

C#:   async Task F() { await G(); }
来源：http://sx.haigaiapp.cn

[O05] 并发执行并等待全部完成
来源：http://cn.jianghongdianzi.cn

Py:   asyncio.gather(*tasks)
来源：http://ke.huanxung.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://zz.szsharing.cn

JS:   await Promise.all(tasks)
来源：http://jg.asd995.cn

TS:   await Promise.all(tasks)
来源：http://fd.bookmarksfly.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ls.chemitech.net.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ca.9csxet.cn

Ruby: threads.map(&:join)
来源：http://jr.shxzukj.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://iy.jctech888.com.cn

[O06] 使用进程池
来源：http://ce.jctech888.com.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://is.huixinmuqiang.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://el.huixinmuqiang.cn

JS:   // child_process / cluster 模块
来源：http://zn.gzmigu.cn

TS:   // child_process / cluster 模块
来源：http://nb.gzmigu.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://iq.shtwfgs.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://bd.yuexingan06.cn

Ruby: // fork 块
来源：http://lu.chemitech.net.cn

C#:   Parallel.For
来源：http://sr.bjjhwx.cn

================================================================================
来源：http://sv.muxihuayi.cn

P. 常用工具函数
来源：http://cn.huixinmuqiang.cn

================================================================================
来源：http://ck.yuexingan06.cn

[P01] 生成 UUID
来源：http://qw.nszjky.cn

Py:   str(uuid.uuid4())
来源：http://mp.jianghongdianzi.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://fm.bjjhwx.cn

JS:   crypto.randomUUID()
来源：http://ex.szxytkj.cn

TS:   crypto.randomUUID()
来源：http://ap.asd995.cn

Java: UUID.randomUUID().toString()
来源：http://kq.newstarts.cn

Go:   // 用 github.com/google/uuid
来源：http://na.bjjhwx.cn

Ruby: SecureRandom.uuid
来源：http://gb.shtwfgs.cn

C#:   Guid.NewGuid().ToString()
来源：http://kq.yuexingan06.cn

[P02] MD5 / SHA256 摘要
来源：http://fr.yuexingan06.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://bh.colortex.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://yr.panjiajie.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://kv.szxytkj.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://co.lnxyls.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://qb.shxzskj.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://kq.szsharing.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ug.lnxyls.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://jx.colortex.cn

[P03] 生成短随机字符串
来源：http://lm.newstarts.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://bh.lnxyls.cn


<!-- 参考信息 -->