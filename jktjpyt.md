代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ix.yuntaijiaju.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://re.hnjuh.cn

[L05] 上传文件（multipart）
来源：http://vu.chemitech.net.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ew.asd995.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ru.chemitech.net.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ho.huixiangedu.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mp.wgjwhj.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://jp.nszjky.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://yb.szxytkj.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://zv.jctech888.com.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://zc.panjiajie.cn

[L06] 解析响应为 JSON
来源：http://eo.newstarts.cn

Py:   resp.json()
来源：http://am.chemitech.net.cn

PHP:  json_decode($body, true);
来源：http://qh.huixinmuqiang.cn

JS:   await resp.json()
来源：http://qd.huixiangedu.cn

TS:   await resp.json()
来源：http://ss.muxihuayi.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://vh.colortex.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://kr.wgjwhj.cn

Ruby: JSON.parse(resp.body)
来源：http://vf.9csxet.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hd.wgjwhj.cn

[L07] 处理 HTTP 状态码
来源：http://fs.lnxyls.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://yv.panjiajie.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://vg.521024.cn

JS:   resp.ok;  resp.status
来源：http://ug.szxytkj.cn

TS:   resp.ok;  resp.status
来源：http://bg.huanxung.cn

Java: resp.statusCode()
来源：http://pc.huanxung.cn

Go:   resp.StatusCode
来源：http://ok.yuexingan06.cn

Ruby: resp.code.to_i
来源：http://gc.nszjky.cn

C#:   (int)resp.StatusCode
来源：http://on.huixinmuqiang.cn

[L08] 并发请求多个地址
来源：http://ty.jianghongdianzi.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wb.lnxyls.cn

PHP:  curl_multi_init() 系列
来源：http://kw.gzmigu.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://op.gzmigu.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sj.jctech888.com.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://qx.newstarts.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://yb.yuexingan06.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://lm.newstarts.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://cf.haigaiapp.cn

================================================================================
来源：http://rs.szsharing.cn

M. 命令行 / 进程 / 环境
来源：http://ws.lnxyls.cn

================================================================================
来源：http://hz.haigaiapp.cn

[M01] 读取命令行参数
来源：http://nn.hahajie.cn

Py:   sys.argv[1:]
来源：http://ar.bookmarksfly.cn

PHP:  $argv;  $argc;
来源：http://bc.asd995.cn

JS:   process.argv.slice(2)
来源：http://cy.9csxet.cn

TS:   process.argv.slice(2)
来源：http://ft.jianghongdianzi.cn

Java: args 数组（main 方法参数）
来源：http://md.jianghongdianzi.cn

Go:   os.Args[1:]
来源：http://gn.bjjhwx.cn

Ruby: ARGV
来源：http://wy.huixiangedu.cn

C#:   args 数组（Main 方法参数）
来源：http://cr.panjiajie.cn

[M02] 读取环境变量
来源：http://bl.nszjky.cn

Py:   os.environ.get("HOME")
来源：http://xm.hahajie.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://cm.gzmigu.cn

JS:   process.env.HOME
来源：http://mr.jianghongdianzi.cn

TS:   process.env.HOME
来源：http://pg.shxzskj.cn

Java: System.getenv("HOME")
来源：http://gy.colortex.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ot.hahajie.cn

Ruby: ENV["HOME"]
来源：http://ys.hahajie.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://kv.gzmigu.cn

[M03] 执行外部命令
来源：http://gq.gzmigu.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mt.lnxyls.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://tk.muxihuayi.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://pc.haigaiapp.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://rl.bjjhwx.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://fm.nszjky.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://qr.muxihuayi.cn

Ruby: system("ls -l");  `ls -l`
来源：http://jw.huixinmuqiang.cn

C#:   Process.Start("ls", "-l");
来源：http://uw.haigaiapp.cn

[M04] 获取当前工作目录
来源：http://yk.chemitech.net.cn

Py:   os.getcwd()
来源：http://rj.bookmarksfly.cn

PHP:  getcwd();
来源：http://ze.hahajie.cn

JS:   process.cwd()
来源：http://uk.bjjhwx.cn

TS:   process.cwd()
来源：http://kl.9csxet.cn

Java: Path.of("").toAbsolutePath()
来源：http://gt.chemitech.net.cn

Go:   os.Getwd()
来源：http://jj.shtwfgs.cn

Ruby: Dir.pwd
来源：http://ra.haigaiapp.cn

C#:   Directory.GetCurrentDirectory()
来源：http://sz.nszjky.cn

[M05] 设置退出码
来源：http://bx.nszjky.cn

Py:   sys.exit(1)
来源：http://nw.jianghongdianzi.cn

PHP:  exit(1);
来源：http://ot.haigaiapp.cn

JS:   process.exit(1)
来源：http://qn.wgjwhj.cn

TS:   process.exit(1)
来源：http://pv.chemitech.net.cn

Java: System.exit(1)
来源：http://zy.panjiajie.cn

Go:   os.Exit(1)
来源：http://tl.yuexingan06.cn

Ruby: exit 1
来源：http://ms.asd995.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ez.nicolike.cn

[M06] 向标准错误输出
来源：http://mf.huixiangedu.cn

Py:   print("err", file=sys.stderr)
来源：http://mp.lnxyls.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://qk.huanxung.cn

JS:   console.error("err")
来源：http://oi.colortex.cn

TS:   console.error("err")
来源：http://ig.9csxet.cn

Java: System.err.println("err")
来源：http://xn.chemitech.net.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ze.hnjuh.cn

Ruby: warn "err"
来源：http://xz.jianghongdianzi.cn

C#:   Console.Error.WriteLine("err")
来源：http://ny.nszjky.cn

[M07] 判断是否为主入口
来源：http://qw.muxihuayi.cn

Py:   if __name__ == "__main__":
来源：http://hd.lnxyls.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://fc.colortex.cn

JS:   require.main === module
来源：http://uf.nszjky.cn

TS:   require.main === module
来源：http://xt.panjiajie.cn

Java: public static void main(String[] args)
来源：http://yv.asd995.cn

Go:   func main()
来源：http://lk.shxzskj.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://pr.szxytkj.cn

C#:   static void Main(string[] args)
来源：http://kw.nszjky.cn

[M08] 获取系统与运行时信息
来源：http://gm.asd995.cn

Py:   platform.system();  platform.python_version()
来源：http://nt.shxzskj.cn

PHP:  PHP_OS;  phpversion();
来源：http://wt.gzmigu.cn

JS:   process.platform;  process.version
来源：http://fs.yuntaijiaju.cn

TS:   process.platform;  process.version
来源：http://ry.521024.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://sx.jctech888.com.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://gf.colortex.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://cs.panjiajie.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://uu.huanxung.cn

================================================================================
来源：http://jd.hahajie.cn

N. 数据结构与算法
来源：http://dl.521024.cn

================================================================================
来源：http://cw.panjiajie.cn

[N01] 二分查找（有序数组）
来源：http://rp.nicolike.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ul.lnxyls.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ac.shxzskj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gy.nicolike.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tq.yuexingan06.cn

Java: Arrays.binarySearch(arr, x)
来源：http://zx.bookmarksfly.cn

Go:   sort.SearchInts(arr, x)
来源：http://nr.haigaiapp.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://pl.huixinmuqiang.cn

C#:   Array.BinarySearch(arr, x)
来源：http://xp.gzmigu.cn

[N02] 排序（工程实践用内置实现）
来源：http://lo.muxihuayi.cn

Py:   sorted(arr);  arr.sort()
来源：http://nh.shxzukj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://cj.bjjhwx.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://gn.shxzskj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://jd.lnxyls.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ol.jianghongdianzi.cn

Go:   slices.Sort(arr)
来源：http://do.wgjwhj.cn

Ruby: arr.sort
来源：http://bs.shxzskj.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://nz.jctech888.com.cn

[N03] 快速排序（分治示例）
来源：http://tj.9csxet.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://vk.jctech888.com.cn

PHP:  // 递归实现，或用 usort
来源：http://fn.szsharing.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dl.colortex.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ub.shxzskj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://rl.9csxet.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ul.521024.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.huixiangedu.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ym.gzmigu.cn

[N04] 斐波那契数列
来源：http://xm.521024.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ss.asd995.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://db.szsharing.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ad.jianghongdianzi.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ou.nszjky.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://qd.lnxyls.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://br.jianghongdianzi.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ru.lnxyls.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://tx.jianghongdianzi.cn

[N05] 最大公约数
来源：http://bb.hnjuh.cn

Py:   math.gcd(a, b)
来源：http://tj.newstarts.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wg.panjiajie.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cw.hnjuh.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://uf.nszjky.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://bl.gzmigu.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://fc.nicolike.cn

Ruby: a.gcd(b)
来源：http://ca.newstarts.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://vn.521024.cn

[N06] 判断回文字符串
来源：http://si.jctech888.com.cn

Py:   s == s[::-1]
来源：http://mm.colortex.cn

PHP:  $s === strrev($s);
来源：http://rp.szsharing.cn

JS:   s === [...s].reverse().join("")
来源：http://lw.nicolike.cn

TS:   s === [...s].reverse().join("")
来源：http://rp.521024.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://uj.hnjuh.cn

Go:   // 双指针从两端比较
来源：http://ge.wgjwhj.cn

Ruby: s == s.reverse
来源：http://xt.muxihuayi.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://pa.szsharing.cn

[N07] 两数之和（返回下标）
来源：http://ke.panjiajie.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://sr.hnjuh.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mj.newstarts.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ux.huanxung.cn

TS:   // 手写 Map<string, number>
来源：http://yy.9csxet.cn

Java: // 手写 HashMap
来源：http://fw.chemitech.net.cn

Go:   // 手写 map[int]int
来源：http://wh.521024.cn

Ruby: // 手写 Hash
来源：http://vv.nicolike.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ju.9csxet.cn

[N08] 生成全排列
来源：http://tv.hahajie.cn

Py:   itertools.permutations(arr)
来源：http://mb.lnxyls.cn

PHP:  // 手写递归交换
来源：http://ts.szxytkj.cn

JS:   // 手写回溯递归
来源：http://ie.nszjky.cn

TS:   // 手写回溯递归
来源：http://zu.szxytkj.cn

Java: // 手写回溯递归
来源：http://zi.gzmigu.cn

Go:   // 手写回溯递归
来源：http://hd.jianghongdianzi.cn

Ruby: arr.permutation.to_a
来源：http://yi.shtwfgs.cn

C#:   // 手写回溯递归
来源：http://rq.wgjwhj.cn

[N09] 栈与队列
来源：http://jc.521024.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://sv.nicolike.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hh.huixinmuqiang.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://zg.wgjwhj.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://dx.huanxung.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://qc.colortex.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://db.bookmarksfly.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://oz.yuexingan06.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://dv.huixinmuqiang.cn

[N10] 链表节点定义
来源：http://yl.yuexingan06.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qk.szxytkj.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://dc.gzmigu.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://cu.colortex.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://sg.hnjuh.cn

Java: class Node { int v; Node next; }
来源：http://iu.wgjwhj.cn

Go:   type Node struct { V int; Next *Node }
来源：http://fm.haigaiapp.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://bz.hahajie.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://xi.gzmigu.cn

[N11] 二叉树中序遍历
来源：http://xd.szxytkj.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://xa.jctech888.com.cn

PHP:  // 手写递归函数
来源：http://pv.asd995.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xv.shtwfgs.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hh.nszjky.cn

Java: // 手写递归
来源：http://xh.521024.cn

Go:   // 手写递归
来源：http://ek.nicolike.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://gb.nszjky.cn

C#:   // 手写递归
来源：http://ow.yuntaijiaju.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://dc.huanxung.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://vz.szxytkj.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://nl.yuexingan06.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sf.huixinmuqiang.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ud.bookmarksfly.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://xv.szsharing.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ak.shtwfgs.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://zt.9csxet.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://nk.muxihuayi.cn

================================================================================
来源：http://oa.lnxyls.cn

O. 并发与异步
来源：http://zn.asd995.cn

================================================================================
来源：http://mr.jianghongdianzi.cn

[O01] 启动一个线程
来源：http://ob.jianghongdianzi.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://rd.nicolike.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://eo.shxzukj.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://vz.nszjky.cn

TS:   // 同 JS
来源：http://xa.jctech888.com.cn

Java: new Thread(() -> f()).start()
来源：http://hd.muxihuayi.cn

Go:   go f()
来源：http://iy.jianghongdianzi.cn

Ruby: Thread.new { f }
来源：http://rw.bookmarksfly.cn

C#:   Task.Run(() => F());
来源：http://an.nicolike.cn

[O02] 使用线程池
来源：http://zr.hnjuh.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mh.shtwfgs.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://oz.bjjhwx.cn

JS:   // worker_threads 线程池
来源：http://ag.chemitech.net.cn

TS:   // worker_threads 线程池
来源：http://tr.yuntaijiaju.cn

Java: Executors.newFixedThreadPool(4)
来源：http://dw.chemitech.net.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ot.szxytkj.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ks.szxytkj.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://dl.shxzskj.cn

[O03] 加锁保护共享数据
来源：http://ko.yuexingan06.cn

Py:   with lock: shared += 1
来源：http://nf.szsharing.cn

PHP:  // 用 flock() 做文件锁
来源：http://pm.521024.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://yf.shtwfgs.cn

TS:   // 同 JS
来源：http://hm.9csxet.cn

Java: synchronized (this) { shared++; }
来源：http://ny.shtwfgs.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://cq.shxzukj.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://at.newstarts.cn

C#:   lock (gate) { shared++; }
来源：http://wy.huixinmuqiang.cn

[O04] 定义异步函数并等待
来源：http://dh.szsharing.cn

Py:   async def f():⏎    await g()
来源：http://sr.nicolike.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ps.nszjky.cn

JS:   async function f() { await g(); }
来源：http://ue.szsharing.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://oa.colortex.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://tm.bjjhwx.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ch.asd995.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ep.jianghongdianzi.cn

C#:   async Task F() { await G(); }
来源：http://ym.9csxet.cn

[O05] 并发执行并等待全部完成
来源：http://cq.jianghongdianzi.cn

Py:   asyncio.gather(*tasks)
来源：http://pq.szxytkj.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://qn.huanxung.cn

JS:   await Promise.all(tasks)
来源：http://xv.jianghongdianzi.cn

TS:   await Promise.all(tasks)
来源：http://xx.jianghongdianzi.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://zw.haigaiapp.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://qb.9csxet.cn

Ruby: threads.map(&:join)
来源：http://ig.panjiajie.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://dz.521024.cn

[O06] 使用进程池
来源：http://bz.9csxet.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://yn.huanxung.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://qi.chemitech.net.cn

JS:   // child_process / cluster 模块
来源：http://pf.huanxung.cn

TS:   // child_process / cluster 模块
来源：http://gt.wgjwhj.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://rh.jianghongdianzi.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hb.hnjuh.cn

Ruby: // fork 块
来源：http://we.bjjhwx.cn

C#:   Parallel.For
来源：http://ng.huixiangedu.cn

================================================================================
来源：http://dn.colortex.cn

P. 常用工具函数
来源：http://gd.newstarts.cn

================================================================================
来源：http://py.huixinmuqiang.cn

[P01] 生成 UUID
来源：http://hz.gzmigu.cn

Py:   str(uuid.uuid4())
来源：http://zx.szxytkj.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://tt.szxytkj.cn

JS:   crypto.randomUUID()
来源：http://px.gzmigu.cn

TS:   crypto.randomUUID()
来源：http://zs.nicolike.cn

Java: UUID.randomUUID().toString()
来源：http://gp.bjjhwx.cn

Go:   // 用 github.com/google/uuid
来源：http://jz.lnxyls.cn

Ruby: SecureRandom.uuid
来源：http://ye.521024.cn

C#:   Guid.NewGuid().ToString()
来源：http://ex.huixinmuqiang.cn

[P02] MD5 / SHA256 摘要
来源：http://zp.chemitech.net.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://fv.chemitech.net.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://um.bookmarksfly.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://zm.nszjky.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://yl.lnxyls.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ti.panjiajie.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mh.panjiajie.cn


<!-- 参考信息 -->