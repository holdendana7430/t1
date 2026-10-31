代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ss.szxytkj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ud.shxzskj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://vs.yuntaijiaju.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ml.chemitech.net.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://yi.huixinmuqiang.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://zt.newstarts.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://br.bookmarksfly.cn

[L06] 解析响应为 JSON
来源：http://rt.lnxyls.cn

Py:   resp.json()
来源：http://jm.huanxung.cn

PHP:  json_decode($body, true);
来源：http://fy.yuntaijiaju.cn

JS:   await resp.json()
来源：http://pr.huanxung.cn

TS:   await resp.json()
来源：http://ix.9csxet.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ce.wgjwhj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mg.huanxung.cn

Ruby: JSON.parse(resp.body)
来源：http://kn.bookmarksfly.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://iv.9csxet.cn

[L07] 处理 HTTP 状态码
来源：http://kt.jianghongdianzi.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ht.panjiajie.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://lw.lnxyls.cn

JS:   resp.ok;  resp.status
来源：http://yk.lnxyls.cn

TS:   resp.ok;  resp.status
来源：http://fh.gzmigu.cn

Java: resp.statusCode()
来源：http://ng.jctech888.com.cn

Go:   resp.StatusCode
来源：http://jr.jctech888.com.cn

Ruby: resp.code.to_i
来源：http://dj.hnjuh.cn

C#:   (int)resp.StatusCode
来源：http://ky.shtwfgs.cn

[L08] 并发请求多个地址
来源：http://hb.lnxyls.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://jd.521024.cn

PHP:  curl_multi_init() 系列
来源：http://qq.521024.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bd.asd995.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lq.shxzskj.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://fy.jctech888.com.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://od.lnxyls.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hb.huanxung.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ll.jctech888.com.cn

================================================================================
来源：http://of.wgjwhj.cn

M. 命令行 / 进程 / 环境
来源：http://zv.asd995.cn

================================================================================
来源：http://ko.gzmigu.cn

[M01] 读取命令行参数
来源：http://ta.jianghongdianzi.cn

Py:   sys.argv[1:]
来源：http://ma.jianghongdianzi.cn

PHP:  $argv;  $argc;
来源：http://ke.yuexingan06.cn

JS:   process.argv.slice(2)
来源：http://nj.haigaiapp.cn

TS:   process.argv.slice(2)
来源：http://jw.gzmigu.cn

Java: args 数组（main 方法参数）
来源：http://br.shxzskj.cn

Go:   os.Args[1:]
来源：http://rj.muxihuayi.cn

Ruby: ARGV
来源：http://yv.jctech888.com.cn

C#:   args 数组（Main 方法参数）
来源：http://qt.huanxung.cn

[M02] 读取环境变量
来源：http://ed.nszjky.cn

Py:   os.environ.get("HOME")
来源：http://uu.shxzukj.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://iy.wgjwhj.cn

JS:   process.env.HOME
来源：http://xj.wgjwhj.cn

TS:   process.env.HOME
来源：http://yd.huixiangedu.cn

Java: System.getenv("HOME")
来源：http://zi.yuntaijiaju.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://pg.szsharing.cn

Ruby: ENV["HOME"]
来源：http://ef.hnjuh.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://zm.asd995.cn

[M03] 执行外部命令
来源：http://bv.lnxyls.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mi.bjjhwx.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://xg.shxzskj.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ti.hahajie.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://hq.shxzukj.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://jq.colortex.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://wb.muxihuayi.cn

Ruby: system("ls -l");  `ls -l`
来源：http://tw.hnjuh.cn

C#:   Process.Start("ls", "-l");
来源：http://fo.wgjwhj.cn

[M04] 获取当前工作目录
来源：http://gh.szxytkj.cn

Py:   os.getcwd()
来源：http://mi.chemitech.net.cn

PHP:  getcwd();
来源：http://md.jianghongdianzi.cn

JS:   process.cwd()
来源：http://mn.9csxet.cn

TS:   process.cwd()
来源：http://nd.hnjuh.cn

Java: Path.of("").toAbsolutePath()
来源：http://bc.bjjhwx.cn

Go:   os.Getwd()
来源：http://nu.szsharing.cn

Ruby: Dir.pwd
来源：http://cw.jianghongdianzi.cn

C#:   Directory.GetCurrentDirectory()
来源：http://hs.newstarts.cn

[M05] 设置退出码
来源：http://sn.hahajie.cn

Py:   sys.exit(1)
来源：http://jc.panjiajie.cn

PHP:  exit(1);
来源：http://hu.nszjky.cn

JS:   process.exit(1)
来源：http://fs.huixiangedu.cn

TS:   process.exit(1)
来源：http://cw.wgjwhj.cn

Java: System.exit(1)
来源：http://po.shtwfgs.cn

Go:   os.Exit(1)
来源：http://um.bjjhwx.cn

Ruby: exit 1
来源：http://ro.hnjuh.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://pq.bjjhwx.cn

[M06] 向标准错误输出
来源：http://yv.lnxyls.cn

Py:   print("err", file=sys.stderr)
来源：http://bc.yuexingan06.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ac.huixiangedu.cn

JS:   console.error("err")
来源：http://bt.nicolike.cn

TS:   console.error("err")
来源：http://ii.bookmarksfly.cn

Java: System.err.println("err")
来源：http://mz.huixiangedu.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://vu.huixinmuqiang.cn

Ruby: warn "err"
来源：http://ze.haigaiapp.cn

C#:   Console.Error.WriteLine("err")
来源：http://ue.szxytkj.cn

[M07] 判断是否为主入口
来源：http://hh.lnxyls.cn

Py:   if __name__ == "__main__":
来源：http://yn.jctech888.com.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://xn.szsharing.cn

JS:   require.main === module
来源：http://ly.szxytkj.cn

TS:   require.main === module
来源：http://lf.shtwfgs.cn

Java: public static void main(String[] args)
来源：http://xc.gzmigu.cn

Go:   func main()
来源：http://wi.yuntaijiaju.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wf.huanxung.cn

C#:   static void Main(string[] args)
来源：http://hq.panjiajie.cn

[M08] 获取系统与运行时信息
来源：http://vl.nszjky.cn

Py:   platform.system();  platform.python_version()
来源：http://oh.szxytkj.cn

PHP:  PHP_OS;  phpversion();
来源：http://ek.asd995.cn

JS:   process.platform;  process.version
来源：http://kc.huixinmuqiang.cn

TS:   process.platform;  process.version
来源：http://at.huixinmuqiang.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ag.nicolike.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://hy.hahajie.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mi.shtwfgs.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://pf.szxytkj.cn

================================================================================
来源：http://zi.asd995.cn

N. 数据结构与算法
来源：http://zr.chemitech.net.cn

================================================================================
来源：http://cm.nszjky.cn

[N01] 二分查找（有序数组）
来源：http://kj.haigaiapp.cn

Py:   bisect.bisect_left(arr, x)
来源：http://jv.hnjuh.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://lm.hahajie.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qq.szsharing.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ho.bookmarksfly.cn

Java: Arrays.binarySearch(arr, x)
来源：http://un.lnxyls.cn

Go:   sort.SearchInts(arr, x)
来源：http://hl.gzmigu.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://fh.muxihuayi.cn

C#:   Array.BinarySearch(arr, x)
来源：http://vm.huixiangedu.cn

[N02] 排序（工程实践用内置实现）
来源：http://jy.panjiajie.cn

Py:   sorted(arr);  arr.sort()
来源：http://fg.shtwfgs.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://jw.bjjhwx.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://zm.hnjuh.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://hk.jianghongdianzi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://gi.haigaiapp.cn

Go:   slices.Sort(arr)
来源：http://kh.szxytkj.cn

Ruby: arr.sort
来源：http://tw.shxzukj.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://qo.huixiangedu.cn

[N03] 快速排序（分治示例）
来源：http://mo.yuexingan06.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ne.yuntaijiaju.cn

PHP:  // 递归实现，或用 usort
来源：http://rd.szsharing.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ub.9csxet.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sj.shxzukj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://nz.yuntaijiaju.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mq.bjjhwx.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ky.nszjky.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ke.huixiangedu.cn

[N04] 斐波那契数列
来源：http://zq.szxytkj.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://we.huixiangedu.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ho.yuntaijiaju.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ew.nicolike.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rl.hahajie.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://rd.shtwfgs.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://xs.bookmarksfly.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://gp.jianghongdianzi.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://tp.jctech888.com.cn

[N05] 最大公约数
来源：http://dj.nszjky.cn

Py:   math.gcd(a, b)
来源：http://ft.huanxung.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hc.yuexingan06.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ev.lnxyls.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kd.bjjhwx.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ew.yuntaijiaju.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://jd.521024.cn

Ruby: a.gcd(b)
来源：http://mw.hnjuh.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://fo.nicolike.cn

[N06] 判断回文字符串
来源：http://zn.bjjhwx.cn

Py:   s == s[::-1]
来源：http://ad.yuexingan06.cn

PHP:  $s === strrev($s);
来源：http://wy.shxzskj.cn

JS:   s === [...s].reverse().join("")
来源：http://tb.nicolike.cn

TS:   s === [...s].reverse().join("")
来源：http://dr.muxihuayi.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://cl.shxzukj.cn

Go:   // 双指针从两端比较
来源：http://aa.bookmarksfly.cn

Ruby: s == s.reverse
来源：http://nb.hahajie.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ht.shxzukj.cn

[N07] 两数之和（返回下标）
来源：http://tt.hnjuh.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://df.wgjwhj.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://yx.chemitech.net.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://dx.asd995.cn

TS:   // 手写 Map<string, number>
来源：http://tx.jctech888.com.cn

Java: // 手写 HashMap
来源：http://dd.jianghongdianzi.cn

Go:   // 手写 map[int]int
来源：http://qo.lnxyls.cn

Ruby: // 手写 Hash
来源：http://rz.yuntaijiaju.cn

C#:   // 手写 Dictionary<int, int>
来源：http://al.asd995.cn

[N08] 生成全排列
来源：http://cr.haigaiapp.cn

Py:   itertools.permutations(arr)
来源：http://sh.szsharing.cn

PHP:  // 手写递归交换
来源：http://yu.colortex.cn

JS:   // 手写回溯递归
来源：http://nu.yuntaijiaju.cn

TS:   // 手写回溯递归
来源：http://bw.haigaiapp.cn

Java: // 手写回溯递归
来源：http://mj.szsharing.cn

Go:   // 手写回溯递归
来源：http://al.haigaiapp.cn

Ruby: arr.permutation.to_a
来源：http://yv.shxzskj.cn

C#:   // 手写回溯递归
来源：http://ig.shtwfgs.cn

[N09] 栈与队列
来源：http://lr.521024.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ps.wgjwhj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://fe.bookmarksfly.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hf.wgjwhj.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://sv.lnxyls.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://bv.shtwfgs.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://av.huanxung.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://xz.asd995.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wq.szxytkj.cn

[N10] 链表节点定义
来源：http://da.huanxung.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mb.wgjwhj.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://lz.9csxet.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://cw.newstarts.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://to.haigaiapp.cn

Java: class Node { int v; Node next; }
来源：http://cb.huixinmuqiang.cn

Go:   type Node struct { V int; Next *Node }
来源：http://oe.hnjuh.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ba.9csxet.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://gh.shtwfgs.cn

[N11] 二叉树中序遍历
来源：http://az.shtwfgs.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mm.wgjwhj.cn

PHP:  // 手写递归函数
来源：http://vu.bookmarksfly.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://uc.colortex.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xr.haigaiapp.cn

Java: // 手写递归
来源：http://oj.colortex.cn

Go:   // 手写递归
来源：http://wh.panjiajie.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://nh.muxihuayi.cn

C#:   // 手写递归
来源：http://yf.wgjwhj.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ow.bookmarksfly.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mj.huixiangedu.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ep.huixiangedu.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qt.szsharing.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://to.nszjky.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ge.lnxyls.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ya.panjiajie.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://xd.bookmarksfly.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://kx.szsharing.cn

================================================================================
来源：http://az.9csxet.cn

O. 并发与异步
来源：http://yo.jianghongdianzi.cn

================================================================================
来源：http://ht.colortex.cn

[O01] 启动一个线程
来源：http://wn.hahajie.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://zf.chemitech.net.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ee.asd995.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://xy.chemitech.net.cn

TS:   // 同 JS
来源：http://kb.nicolike.cn

Java: new Thread(() -> f()).start()
来源：http://yn.521024.cn

Go:   go f()
来源：http://vk.gzmigu.cn

Ruby: Thread.new { f }
来源：http://vm.jianghongdianzi.cn

C#:   Task.Run(() => F());
来源：http://qe.bjjhwx.cn

[O02] 使用线程池
来源：http://cz.haigaiapp.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://zw.shxzskj.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://yv.huanxung.cn

JS:   // worker_threads 线程池
来源：http://lr.9csxet.cn

TS:   // worker_threads 线程池
来源：http://ga.nszjky.cn

Java: Executors.newFixedThreadPool(4)
来源：http://lb.nicolike.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ue.nicolike.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hw.panjiajie.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ye.hahajie.cn

[O03] 加锁保护共享数据
来源：http://ng.yuntaijiaju.cn

Py:   with lock: shared += 1
来源：http://cz.szxytkj.cn

PHP:  // 用 flock() 做文件锁
来源：http://lf.huixinmuqiang.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ja.colortex.cn

TS:   // 同 JS
来源：http://qo.nszjky.cn

Java: synchronized (this) { shared++; }
来源：http://eo.yuntaijiaju.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://nf.yuntaijiaju.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://gw.jctech888.com.cn

C#:   lock (gate) { shared++; }
来源：http://le.lnxyls.cn

[O04] 定义异步函数并等待
来源：http://eo.lnxyls.cn

Py:   async def f():⏎    await g()
来源：http://ck.asd995.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://yo.asd995.cn

JS:   async function f() { await g(); }
来源：http://rj.huixiangedu.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ko.muxihuayi.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://dd.521024.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ww.shxzukj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://fa.jctech888.com.cn

C#:   async Task F() { await G(); }
来源：http://ua.nicolike.cn

[O05] 并发执行并等待全部完成
来源：http://ar.yuntaijiaju.cn

Py:   asyncio.gather(*tasks)
来源：http://by.shxzskj.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mg.colortex.cn

JS:   await Promise.all(tasks)
来源：http://su.panjiajie.cn

TS:   await Promise.all(tasks)
来源：http://vc.nicolike.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://cj.huixinmuqiang.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://yt.521024.cn

Ruby: threads.map(&:join)
来源：http://hc.nicolike.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://vk.hnjuh.cn

[O06] 使用进程池
来源：http://dc.wgjwhj.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hs.chemitech.net.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://hi.asd995.cn

JS:   // child_process / cluster 模块
来源：http://dp.hnjuh.cn

TS:   // child_process / cluster 模块
来源：http://ct.shtwfgs.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://gm.szxytkj.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ll.panjiajie.cn

Ruby: // fork 块
来源：http://rs.haigaiapp.cn

C#:   Parallel.For
来源：http://jj.jianghongdianzi.cn

================================================================================
来源：http://qi.colortex.cn

P. 常用工具函数
来源：http://vm.521024.cn

================================================================================
来源：http://vh.bjjhwx.cn

[P01] 生成 UUID
来源：http://gy.panjiajie.cn

Py:   str(uuid.uuid4())
来源：http://pv.shxzukj.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ik.yuntaijiaju.cn

JS:   crypto.randomUUID()
来源：http://ha.9csxet.cn

TS:   crypto.randomUUID()
来源：http://ec.hnjuh.cn

Java: UUID.randomUUID().toString()
来源：http://zm.lnxyls.cn

Go:   // 用 github.com/google/uuid
来源：http://nm.hahajie.cn

Ruby: SecureRandom.uuid
来源：http://zs.huanxung.cn

C#:   Guid.NewGuid().ToString()
来源：http://qd.shxzukj.cn

[P02] MD5 / SHA256 摘要
来源：http://mu.jctech888.com.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://eh.colortex.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://yl.yuexingan06.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://lj.shxzskj.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://fx.colortex.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://bb.huixinmuqiang.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://nt.hahajie.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://yj.szxytkj.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://yo.hahajie.cn

[P03] 生成短随机字符串
来源：http://go.521024.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://vz.szsharing.cn


<!-- 参考信息 -->