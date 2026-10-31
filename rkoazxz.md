代发 wailian999

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://am.lnxyls.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yq.hahajie.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://jp.panjiajie.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://gg.wgjwhj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hk.yuntaijiaju.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://fm.asd995.cn

[L05] 上传文件（multipart）
来源：http://ap.lnxyls.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://gq.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ti.hahajie.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ir.jianghongdianzi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://kj.colortex.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://gq.nszjky.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://qh.muxihuayi.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://rw.9csxet.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://uv.huanxung.cn

[L06] 解析响应为 JSON
来源：http://rj.yuexingan06.cn

Py:   resp.json()
来源：http://oc.521024.cn

PHP:  json_decode($body, true);
来源：http://ld.jctech888.com.cn

JS:   await resp.json()
来源：http://wh.colortex.cn

TS:   await resp.json()
来源：http://yt.yuntaijiaju.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://fy.asd995.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://lk.huixiangedu.cn

Ruby: JSON.parse(resp.body)
来源：http://vj.huixinmuqiang.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://zi.bjjhwx.cn

[L07] 处理 HTTP 状态码
来源：http://lh.yuexingan06.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://zv.bookmarksfly.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://tm.huanxung.cn

JS:   resp.ok;  resp.status
来源：http://is.asd995.cn

TS:   resp.ok;  resp.status
来源：http://qz.bookmarksfly.cn

Java: resp.statusCode()
来源：http://hw.nicolike.cn

Go:   resp.StatusCode
来源：http://pi.chemitech.net.cn

Ruby: resp.code.to_i
来源：http://lw.szsharing.cn

C#:   (int)resp.StatusCode
来源：http://do.haigaiapp.cn

[L08] 并发请求多个地址
来源：http://yi.jianghongdianzi.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ez.jianghongdianzi.cn

PHP:  curl_multi_init() 系列
来源：http://xw.hahajie.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://np.huixiangedu.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ha.nszjky.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://dj.szsharing.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://it.yuexingan06.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ut.hahajie.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hf.yuexingan06.cn

================================================================================
来源：http://gx.lnxyls.cn

M. 命令行 / 进程 / 环境
来源：http://wh.yuexingan06.cn

================================================================================
来源：http://og.haigaiapp.cn

[M01] 读取命令行参数
来源：http://vu.colortex.cn

Py:   sys.argv[1:]
来源：http://xn.yuexingan06.cn

PHP:  $argv;  $argc;
来源：http://yj.shxzskj.cn

JS:   process.argv.slice(2)
来源：http://xi.haigaiapp.cn

TS:   process.argv.slice(2)
来源：http://eg.bookmarksfly.cn

Java: args 数组（main 方法参数）
来源：http://iq.nicolike.cn

Go:   os.Args[1:]
来源：http://ee.shxzskj.cn

Ruby: ARGV
来源：http://cd.muxihuayi.cn

C#:   args 数组（Main 方法参数）
来源：http://fv.szxytkj.cn

[M02] 读取环境变量
来源：http://qf.huanxung.cn

Py:   os.environ.get("HOME")
来源：http://ef.nicolike.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mk.panjiajie.cn

JS:   process.env.HOME
来源：http://jk.bjjhwx.cn

TS:   process.env.HOME
来源：http://ft.nszjky.cn

Java: System.getenv("HOME")
来源：http://fm.yuexingan06.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mr.muxihuayi.cn

Ruby: ENV["HOME"]
来源：http://vd.huixiangedu.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://tb.yuntaijiaju.cn

[M03] 执行外部命令
来源：http://sm.szxytkj.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mv.haigaiapp.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://lb.hahajie.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://kp.chemitech.net.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://zv.gzmigu.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://nz.huixiangedu.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://xo.wgjwhj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ar.shxzukj.cn

C#:   Process.Start("ls", "-l");
来源：http://hk.asd995.cn

[M04] 获取当前工作目录
来源：http://kj.9csxet.cn

Py:   os.getcwd()
来源：http://ns.521024.cn

PHP:  getcwd();
来源：http://ja.huixinmuqiang.cn

JS:   process.cwd()
来源：http://cd.jctech888.com.cn

TS:   process.cwd()
来源：http://uu.bjjhwx.cn

Java: Path.of("").toAbsolutePath()
来源：http://xy.yuexingan06.cn

Go:   os.Getwd()
来源：http://sd.panjiajie.cn

Ruby: Dir.pwd
来源：http://xn.nszjky.cn

C#:   Directory.GetCurrentDirectory()
来源：http://eo.asd995.cn

[M05] 设置退出码
来源：http://at.hahajie.cn

Py:   sys.exit(1)
来源：http://lo.yuexingan06.cn

PHP:  exit(1);
来源：http://mq.shxzukj.cn

JS:   process.exit(1)
来源：http://ht.gzmigu.cn

TS:   process.exit(1)
来源：http://lg.bjjhwx.cn

Java: System.exit(1)
来源：http://tc.nszjky.cn

Go:   os.Exit(1)
来源：http://fr.yuexingan06.cn

Ruby: exit 1
来源：http://xq.szsharing.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ky.yuntaijiaju.cn

[M06] 向标准错误输出
来源：http://zv.szsharing.cn

Py:   print("err", file=sys.stderr)
来源：http://wp.nicolike.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://wz.nicolike.cn

JS:   console.error("err")
来源：http://id.nszjky.cn

TS:   console.error("err")
来源：http://xp.lnxyls.cn

Java: System.err.println("err")
来源：http://ey.newstarts.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hi.hahajie.cn

Ruby: warn "err"
来源：http://fa.huixiangedu.cn

C#:   Console.Error.WriteLine("err")
来源：http://yp.chemitech.net.cn

[M07] 判断是否为主入口
来源：http://vx.521024.cn

Py:   if __name__ == "__main__":
来源：http://ej.jianghongdianzi.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://fd.huanxung.cn

JS:   require.main === module
来源：http://aq.yuntaijiaju.cn

TS:   require.main === module
来源：http://ez.lnxyls.cn

Java: public static void main(String[] args)
来源：http://gp.huixinmuqiang.cn

Go:   func main()
来源：http://vk.szsharing.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://yr.jianghongdianzi.cn

C#:   static void Main(string[] args)
来源：http://fg.bjjhwx.cn

[M08] 获取系统与运行时信息
来源：http://ga.shxzskj.cn

Py:   platform.system();  platform.python_version()
来源：http://db.szxytkj.cn

PHP:  PHP_OS;  phpversion();
来源：http://ko.szsharing.cn

JS:   process.platform;  process.version
来源：http://dn.shxzskj.cn

TS:   process.platform;  process.version
来源：http://sv.huixiangedu.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://qz.jianghongdianzi.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://zx.huixiangedu.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://st.chemitech.net.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://rx.huixinmuqiang.cn

================================================================================
来源：http://rc.szsharing.cn

N. 数据结构与算法
来源：http://zp.yuexingan06.cn

================================================================================
来源：http://uf.nicolike.cn

[N01] 二分查找（有序数组）
来源：http://mj.9csxet.cn

Py:   bisect.bisect_left(arr, x)
来源：http://bj.hahajie.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://gn.nszjky.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mi.jctech888.com.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yi.asd995.cn

Java: Arrays.binarySearch(arr, x)
来源：http://gu.nicolike.cn

Go:   sort.SearchInts(arr, x)
来源：http://bx.9csxet.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ia.haigaiapp.cn

C#:   Array.BinarySearch(arr, x)
来源：http://hi.shxzukj.cn

[N02] 排序（工程实践用内置实现）
来源：http://xt.lnxyls.cn

Py:   sorted(arr);  arr.sort()
来源：http://cd.szxytkj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://gh.hahajie.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://jn.shxzskj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://bj.shxzukj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://bw.lnxyls.cn

Go:   slices.Sort(arr)
来源：http://rx.bookmarksfly.cn

Ruby: arr.sort
来源：http://ra.lnxyls.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://yl.gzmigu.cn

[N03] 快速排序（分治示例）
来源：http://bl.szsharing.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ln.bookmarksfly.cn

PHP:  // 递归实现，或用 usort
来源：http://lc.asd995.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ky.hnjuh.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ua.huanxung.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://yi.muxihuayi.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://sn.szsharing.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://lh.bjjhwx.cn

C#:   // 手写递归，或 Array.Sort
来源：http://pj.nszjky.cn

[N04] 斐波那契数列
来源：http://zo.newstarts.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qj.jianghongdianzi.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://qj.shtwfgs.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://id.bjjhwx.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xh.newstarts.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://la.shxzskj.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://st.huixiangedu.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://yx.nszjky.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://au.hnjuh.cn

[N05] 最大公约数
来源：http://jf.shxzskj.cn

Py:   math.gcd(a, b)
来源：http://hv.hahajie.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://au.shtwfgs.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qx.gzmigu.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://eh.nicolike.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://lv.9csxet.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://kv.jctech888.com.cn

Ruby: a.gcd(b)
来源：http://tj.shxzskj.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://yt.asd995.cn

[N06] 判断回文字符串
来源：http://ys.szxytkj.cn

Py:   s == s[::-1]
来源：http://hr.hnjuh.cn

PHP:  $s === strrev($s);
来源：http://dj.yuexingan06.cn

JS:   s === [...s].reverse().join("")
来源：http://ig.szxytkj.cn

TS:   s === [...s].reverse().join("")
来源：http://mg.asd995.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ou.huanxung.cn

Go:   // 双指针从两端比较
来源：http://jd.colortex.cn

Ruby: s == s.reverse
来源：http://al.huixiangedu.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://cp.hahajie.cn

[N07] 两数之和（返回下标）
来源：http://dj.huixinmuqiang.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ky.jctech888.com.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://gk.muxihuayi.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://vd.shtwfgs.cn

TS:   // 手写 Map<string, number>
来源：http://en.yuntaijiaju.cn

Java: // 手写 HashMap
来源：http://qz.huixinmuqiang.cn

Go:   // 手写 map[int]int
来源：http://se.shxzukj.cn

Ruby: // 手写 Hash
来源：http://hd.haigaiapp.cn

C#:   // 手写 Dictionary<int, int>
来源：http://uf.gzmigu.cn

[N08] 生成全排列
来源：http://uy.huixiangedu.cn

Py:   itertools.permutations(arr)
来源：http://vk.bookmarksfly.cn

PHP:  // 手写递归交换
来源：http://yy.lnxyls.cn

JS:   // 手写回溯递归
来源：http://fi.szxytkj.cn

TS:   // 手写回溯递归
来源：http://un.yuntaijiaju.cn

Java: // 手写回溯递归
来源：http://wv.shxzskj.cn

Go:   // 手写回溯递归
来源：http://gu.huixiangedu.cn

Ruby: arr.permutation.to_a
来源：http://ih.shtwfgs.cn

C#:   // 手写回溯递归
来源：http://oy.shxzukj.cn

[N09] 栈与队列
来源：http://ls.huixiangedu.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://gs.521024.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ag.nicolike.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ib.huixiangedu.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://vf.jctech888.com.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://uw.9csxet.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://yx.shtwfgs.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://de.bookmarksfly.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ut.yuexingan06.cn

[N10] 链表节点定义
来源：http://qn.jctech888.com.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://un.colortex.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://kt.nszjky.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://iq.asd995.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://pw.colortex.cn

Java: class Node { int v; Node next; }
来源：http://ig.bookmarksfly.cn

Go:   type Node struct { V int; Next *Node }
来源：http://mc.jianghongdianzi.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://xi.hahajie.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://at.szsharing.cn

[N11] 二叉树中序遍历
来源：http://cq.yuexingan06.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ec.yuexingan06.cn

PHP:  // 手写递归函数
来源：http://ar.haigaiapp.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ct.huanxung.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ah.haigaiapp.cn

Java: // 手写递归
来源：http://hp.colortex.cn

Go:   // 手写递归
来源：http://tr.huixinmuqiang.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://vm.hahajie.cn

C#:   // 手写递归
来源：http://gp.bookmarksfly.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mz.chemitech.net.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wd.huixiangedu.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://tv.nszjky.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lg.hahajie.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zc.shxzukj.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://tm.shxzukj.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://bi.asd995.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ys.asd995.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://vx.huanxung.cn

================================================================================
来源：http://aj.huanxung.cn

O. 并发与异步
来源：http://qa.newstarts.cn

================================================================================
来源：http://bx.bookmarksfly.cn

[O01] 启动一个线程
来源：http://xh.hnjuh.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://rg.szsharing.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://dh.yuexingan06.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://nv.shtwfgs.cn

TS:   // 同 JS
来源：http://hm.hnjuh.cn

Java: new Thread(() -> f()).start()
来源：http://le.wgjwhj.cn

Go:   go f()
来源：http://zt.panjiajie.cn

Ruby: Thread.new { f }
来源：http://dc.chemitech.net.cn

C#:   Task.Run(() => F());
来源：http://we.jianghongdianzi.cn

[O02] 使用线程池
来源：http://ub.hnjuh.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ue.bjjhwx.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ym.9csxet.cn

JS:   // worker_threads 线程池
来源：http://sp.muxihuayi.cn

TS:   // worker_threads 线程池
来源：http://zg.9csxet.cn

Java: Executors.newFixedThreadPool(4)
来源：http://wj.szsharing.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://gs.nicolike.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ra.huixinmuqiang.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://dc.huixinmuqiang.cn

[O03] 加锁保护共享数据
来源：http://xt.521024.cn

Py:   with lock: shared += 1
来源：http://hi.panjiajie.cn

PHP:  // 用 flock() 做文件锁
来源：http://be.bjjhwx.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://rq.bookmarksfly.cn

TS:   // 同 JS
来源：http://sb.shxzskj.cn

Java: synchronized (this) { shared++; }
来源：http://me.9csxet.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ph.shxzukj.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ob.huanxung.cn

C#:   lock (gate) { shared++; }
来源：http://vy.huixiangedu.cn

[O04] 定义异步函数并等待
来源：http://bc.bookmarksfly.cn

Py:   async def f():⏎    await g()
来源：http://xw.wgjwhj.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hd.newstarts.cn

JS:   async function f() { await g(); }
来源：http://va.jianghongdianzi.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://tg.szsharing.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://xc.9csxet.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://qe.muxihuayi.cn

Ruby: # 用 Fiber 或 async gem
来源：http://iw.szxytkj.cn

C#:   async Task F() { await G(); }
来源：http://vr.wgjwhj.cn

[O05] 并发执行并等待全部完成
来源：http://ow.muxihuayi.cn

Py:   asyncio.gather(*tasks)
来源：http://qv.hahajie.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://fr.haigaiapp.cn

JS:   await Promise.all(tasks)
来源：http://hl.shxzukj.cn

TS:   await Promise.all(tasks)
来源：http://xu.shtwfgs.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wy.shxzskj.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://va.lnxyls.cn

Ruby: threads.map(&:join)
来源：http://tz.szxytkj.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://jl.szxytkj.cn

[O06] 使用进程池
来源：http://by.yuexingan06.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wr.hahajie.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://pa.shxzukj.cn

JS:   // child_process / cluster 模块
来源：http://zq.wgjwhj.cn

TS:   // child_process / cluster 模块
来源：http://dm.asd995.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ic.bookmarksfly.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://fs.hnjuh.cn

Ruby: // fork 块
来源：http://iv.jctech888.com.cn

C#:   Parallel.For
来源：http://wt.szsharing.cn

================================================================================
来源：http://ln.wgjwhj.cn

P. 常用工具函数
来源：http://jj.lnxyls.cn

================================================================================
来源：http://kd.huixinmuqiang.cn

[P01] 生成 UUID
来源：http://cm.asd995.cn

Py:   str(uuid.uuid4())
来源：http://dy.wgjwhj.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://em.muxihuayi.cn

JS:   crypto.randomUUID()
来源：http://rg.jianghongdianzi.cn

TS:   crypto.randomUUID()
来源：http://wy.colortex.cn

Java: UUID.randomUUID().toString()
来源：http://gc.shtwfgs.cn

Go:   // 用 github.com/google/uuid
来源：http://dv.521024.cn

Ruby: SecureRandom.uuid
来源：http://eh.shtwfgs.cn

C#:   Guid.NewGuid().ToString()
来源：http://yd.jianghongdianzi.cn

[P02] MD5 / SHA256 摘要
来源：http://ds.panjiajie.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://pd.huanxung.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://in.hahajie.cn


<!-- 参考信息 -->