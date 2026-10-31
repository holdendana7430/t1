代发 wailian999

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dw.yuntaijiaju.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://if.gzmigu.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://er.jctech888.com.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://cr.jctech888.com.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://zm.huixiangedu.cn

[L04] 设置超时
来源：http://uf.hahajie.cn

Py:   requests.get(url, timeout=5)
来源：http://zt.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://fz.521024.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qa.asd995.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tf.muxihuayi.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://fh.bookmarksfly.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://dg.bjjhwx.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://bw.szxytkj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://sh.huixinmuqiang.cn

[L05] 上传文件（multipart）
来源：http://xb.huixinmuqiang.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://sz.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://gz.colortex.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mc.yuexingan06.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://sk.yuexingan06.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://yl.yuexingan06.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://vq.colortex.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://tj.huanxung.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://zj.yuexingan06.cn

[L06] 解析响应为 JSON
来源：http://sc.521024.cn

Py:   resp.json()
来源：http://my.jctech888.com.cn

PHP:  json_decode($body, true);
来源：http://pi.521024.cn

JS:   await resp.json()
来源：http://wn.panjiajie.cn

TS:   await resp.json()
来源：http://ia.lnxyls.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ik.haigaiapp.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://kb.huixinmuqiang.cn

Ruby: JSON.parse(resp.body)
来源：http://sm.shxzskj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://qa.huanxung.cn

[L07] 处理 HTTP 状态码
来源：http://sq.colortex.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hw.yuexingan06.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://cf.wgjwhj.cn

JS:   resp.ok;  resp.status
来源：http://hq.szsharing.cn

TS:   resp.ok;  resp.status
来源：http://ni.lnxyls.cn

Java: resp.statusCode()
来源：http://hu.panjiajie.cn

Go:   resp.StatusCode
来源：http://cv.huixiangedu.cn

Ruby: resp.code.to_i
来源：http://fq.gzmigu.cn

C#:   (int)resp.StatusCode
来源：http://ru.nszjky.cn

[L08] 并发请求多个地址
来源：http://mo.huanxung.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://uu.nszjky.cn

PHP:  curl_multi_init() 系列
来源：http://cx.newstarts.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sh.muxihuayi.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bg.9csxet.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://za.bjjhwx.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://fl.shxzukj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ja.nszjky.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://en.chemitech.net.cn

================================================================================
来源：http://qb.bjjhwx.cn

M. 命令行 / 进程 / 环境
来源：http://gf.nszjky.cn

================================================================================
来源：http://cw.lnxyls.cn

[M01] 读取命令行参数
来源：http://ef.hnjuh.cn

Py:   sys.argv[1:]
来源：http://wm.panjiajie.cn

PHP:  $argv;  $argc;
来源：http://jv.hahajie.cn

JS:   process.argv.slice(2)
来源：http://bx.colortex.cn

TS:   process.argv.slice(2)
来源：http://ph.nszjky.cn

Java: args 数组（main 方法参数）
来源：http://kb.colortex.cn

Go:   os.Args[1:]
来源：http://al.asd995.cn

Ruby: ARGV
来源：http://sk.chemitech.net.cn

C#:   args 数组（Main 方法参数）
来源：http://jl.jctech888.com.cn

[M02] 读取环境变量
来源：http://yh.huanxung.cn

Py:   os.environ.get("HOME")
来源：http://zj.colortex.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://yp.colortex.cn

JS:   process.env.HOME
来源：http://bq.shxzukj.cn

TS:   process.env.HOME
来源：http://fr.jianghongdianzi.cn

Java: System.getenv("HOME")
来源：http://ly.bookmarksfly.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://pq.yuntaijiaju.cn

Ruby: ENV["HOME"]
来源：http://pr.nszjky.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://oj.bjjhwx.cn

[M03] 执行外部命令
来源：http://iq.521024.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ys.yuntaijiaju.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://fo.bjjhwx.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://nk.nszjky.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://sh.chemitech.net.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://fi.huanxung.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ox.haigaiapp.cn

Ruby: system("ls -l");  `ls -l`
来源：http://vu.panjiajie.cn

C#:   Process.Start("ls", "-l");
来源：http://dg.wgjwhj.cn

[M04] 获取当前工作目录
来源：http://fa.muxihuayi.cn

Py:   os.getcwd()
来源：http://eq.panjiajie.cn

PHP:  getcwd();
来源：http://gr.yuntaijiaju.cn

JS:   process.cwd()
来源：http://ac.szsharing.cn

TS:   process.cwd()
来源：http://ws.wgjwhj.cn

Java: Path.of("").toAbsolutePath()
来源：http://yz.jctech888.com.cn

Go:   os.Getwd()
来源：http://io.panjiajie.cn

Ruby: Dir.pwd
来源：http://dc.hnjuh.cn

C#:   Directory.GetCurrentDirectory()
来源：http://xm.hahajie.cn

[M05] 设置退出码
来源：http://ly.yuntaijiaju.cn

Py:   sys.exit(1)
来源：http://ak.muxihuayi.cn

PHP:  exit(1);
来源：http://ac.shtwfgs.cn

JS:   process.exit(1)
来源：http://qf.shxzukj.cn

TS:   process.exit(1)
来源：http://cv.newstarts.cn

Java: System.exit(1)
来源：http://pc.jianghongdianzi.cn

Go:   os.Exit(1)
来源：http://cn.asd995.cn

Ruby: exit 1
来源：http://se.nicolike.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://bj.nszjky.cn

[M06] 向标准错误输出
来源：http://no.hahajie.cn

Py:   print("err", file=sys.stderr)
来源：http://qg.szxytkj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://rw.hahajie.cn

JS:   console.error("err")
来源：http://fi.shxzskj.cn

TS:   console.error("err")
来源：http://nm.jctech888.com.cn

Java: System.err.println("err")
来源：http://qy.chemitech.net.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ys.panjiajie.cn

Ruby: warn "err"
来源：http://ng.shxzskj.cn

C#:   Console.Error.WriteLine("err")
来源：http://zs.nicolike.cn

[M07] 判断是否为主入口
来源：http://gl.chemitech.net.cn

Py:   if __name__ == "__main__":
来源：http://as.colortex.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://vn.colortex.cn

JS:   require.main === module
来源：http://aa.bjjhwx.cn

TS:   require.main === module
来源：http://pj.jctech888.com.cn

Java: public static void main(String[] args)
来源：http://dl.wgjwhj.cn

Go:   func main()
来源：http://xu.haigaiapp.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://fg.szsharing.cn

C#:   static void Main(string[] args)
来源：http://jn.hnjuh.cn

[M08] 获取系统与运行时信息
来源：http://gp.nszjky.cn

Py:   platform.system();  platform.python_version()
来源：http://ch.shtwfgs.cn

PHP:  PHP_OS;  phpversion();
来源：http://gd.hnjuh.cn

JS:   process.platform;  process.version
来源：http://bh.newstarts.cn

TS:   process.platform;  process.version
来源：http://wy.chemitech.net.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hd.nicolike.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://wn.shtwfgs.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://tv.hnjuh.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://sc.newstarts.cn

================================================================================
来源：http://pb.muxihuayi.cn

N. 数据结构与算法
来源：http://qu.panjiajie.cn

================================================================================
来源：http://sy.jianghongdianzi.cn

[N01] 二分查找（有序数组）
来源：http://nr.chemitech.net.cn

Py:   bisect.bisect_left(arr, x)
来源：http://bh.nszjky.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://yr.chemitech.net.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lw.hahajie.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wf.haigaiapp.cn

Java: Arrays.binarySearch(arr, x)
来源：http://js.bjjhwx.cn

Go:   sort.SearchInts(arr, x)
来源：http://vz.yuexingan06.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://oz.shxzukj.cn

C#:   Array.BinarySearch(arr, x)
来源：http://yp.gzmigu.cn

[N02] 排序（工程实践用内置实现）
来源：http://mi.bookmarksfly.cn

Py:   sorted(arr);  arr.sort()
来源：http://pd.huanxung.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mf.yuntaijiaju.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://rw.colortex.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://gj.colortex.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://it.hahajie.cn

Go:   slices.Sort(arr)
来源：http://zx.hahajie.cn

Ruby: arr.sort
来源：http://yz.colortex.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ou.521024.cn

[N03] 快速排序（分治示例）
来源：http://yd.gzmigu.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://db.hnjuh.cn

PHP:  // 递归实现，或用 usort
来源：http://xv.szsharing.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qz.bjjhwx.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fn.shxzskj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://gf.shxzskj.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://cz.shtwfgs.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://zh.yuntaijiaju.cn

C#:   // 手写递归，或 Array.Sort
来源：http://zx.yuntaijiaju.cn

[N04] 斐波那契数列
来源：http://om.gzmigu.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://nd.bookmarksfly.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://kz.lnxyls.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sg.hnjuh.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jj.yuntaijiaju.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://tf.shxzskj.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://yq.huixinmuqiang.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://xx.haigaiapp.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mz.lnxyls.cn

[N05] 最大公约数
来源：http://qg.szxytkj.cn

Py:   math.gcd(a, b)
来源：http://yu.chemitech.net.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ln.yuexingan06.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sj.huanxung.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cl.bjjhwx.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://vd.lnxyls.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ov.yuexingan06.cn

Ruby: a.gcd(b)
来源：http://vx.nicolike.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://cg.yuntaijiaju.cn

[N06] 判断回文字符串
来源：http://rl.muxihuayi.cn

Py:   s == s[::-1]
来源：http://zz.lnxyls.cn

PHP:  $s === strrev($s);
来源：http://db.chemitech.net.cn

JS:   s === [...s].reverse().join("")
来源：http://fa.bookmarksfly.cn

TS:   s === [...s].reverse().join("")
来源：http://ak.nicolike.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ry.shxzukj.cn

Go:   // 双指针从两端比较
来源：http://hf.bookmarksfly.cn

Ruby: s == s.reverse
来源：http://yx.yuexingan06.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://fw.bookmarksfly.cn

[N07] 两数之和（返回下标）
来源：http://kp.hnjuh.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://lj.lnxyls.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wm.lnxyls.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ri.chemitech.net.cn

TS:   // 手写 Map<string, number>
来源：http://ih.wgjwhj.cn

Java: // 手写 HashMap
来源：http://fs.wgjwhj.cn

Go:   // 手写 map[int]int
来源：http://fg.bookmarksfly.cn

Ruby: // 手写 Hash
来源：http://zh.huixiangedu.cn

C#:   // 手写 Dictionary<int, int>
来源：http://by.bookmarksfly.cn

[N08] 生成全排列
来源：http://zc.colortex.cn

Py:   itertools.permutations(arr)
来源：http://aj.hahajie.cn

PHP:  // 手写递归交换
来源：http://lc.huixiangedu.cn

JS:   // 手写回溯递归
来源：http://or.9csxet.cn

TS:   // 手写回溯递归
来源：http://ff.asd995.cn

Java: // 手写回溯递归
来源：http://ej.asd995.cn

Go:   // 手写回溯递归
来源：http://hu.huixiangedu.cn

Ruby: arr.permutation.to_a
来源：http://ln.nszjky.cn

C#:   // 手写回溯递归
来源：http://gz.chemitech.net.cn

[N09] 栈与队列
来源：http://aq.9csxet.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://jp.yuexingan06.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://sd.colortex.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hy.haigaiapp.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://tv.nicolike.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ni.huixinmuqiang.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://yv.huixinmuqiang.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://lf.bjjhwx.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://tu.hnjuh.cn

[N10] 链表节点定义
来源：http://lj.shxzskj.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://uv.nicolike.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://dz.hahajie.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://nq.panjiajie.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ld.bookmarksfly.cn

Java: class Node { int v; Node next; }
来源：http://xz.nicolike.cn

Go:   type Node struct { V int; Next *Node }
来源：http://oi.chemitech.net.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ox.colortex.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://gw.hnjuh.cn

[N11] 二叉树中序遍历
来源：http://hd.panjiajie.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ah.lnxyls.cn

PHP:  // 手写递归函数
来源：http://xj.szxytkj.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rl.asd995.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nb.szxytkj.cn

Java: // 手写递归
来源：http://yu.wgjwhj.cn

Go:   // 手写递归
来源：http://no.muxihuayi.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ur.shtwfgs.cn

C#:   // 手写递归
来源：http://uh.bookmarksfly.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ii.huanxung.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://vt.newstarts.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://pr.jianghongdianzi.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hm.lnxyls.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bv.panjiajie.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://dw.yuntaijiaju.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://fw.9csxet.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://kk.huixiangedu.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://cv.yuntaijiaju.cn

================================================================================
来源：http://lx.9csxet.cn

O. 并发与异步
来源：http://op.panjiajie.cn

================================================================================
来源：http://hc.jctech888.com.cn

[O01] 启动一个线程
来源：http://fi.huixinmuqiang.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://no.panjiajie.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://xy.yuexingan06.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://vm.shxzskj.cn

TS:   // 同 JS
来源：http://is.jianghongdianzi.cn

Java: new Thread(() -> f()).start()
来源：http://uu.hahajie.cn

Go:   go f()
来源：http://qi.panjiajie.cn

Ruby: Thread.new { f }
来源：http://da.colortex.cn

C#:   Task.Run(() => F());
来源：http://kd.shxzukj.cn

[O02] 使用线程池
来源：http://gc.asd995.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ct.bookmarksfly.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ur.521024.cn

JS:   // worker_threads 线程池
来源：http://ta.huixinmuqiang.cn

TS:   // worker_threads 线程池
来源：http://vm.nicolike.cn

Java: Executors.newFixedThreadPool(4)
来源：http://vw.chemitech.net.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://so.bookmarksfly.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://fv.panjiajie.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://tq.hnjuh.cn

[O03] 加锁保护共享数据
来源：http://ag.lnxyls.cn

Py:   with lock: shared += 1
来源：http://zi.huixiangedu.cn

PHP:  // 用 flock() 做文件锁
来源：http://zt.chemitech.net.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mv.haigaiapp.cn

TS:   // 同 JS
来源：http://gi.jctech888.com.cn

Java: synchronized (this) { shared++; }
来源：http://ri.bjjhwx.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://pn.nicolike.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://hx.huixinmuqiang.cn

C#:   lock (gate) { shared++; }
来源：http://bd.yuexingan06.cn

[O04] 定义异步函数并等待
来源：http://rs.bjjhwx.cn

Py:   async def f():⏎    await g()
来源：http://bt.hahajie.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://zf.szxytkj.cn

JS:   async function f() { await g(); }
来源：http://gw.nszjky.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://tx.szxytkj.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://fi.shxzukj.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://la.newstarts.cn

Ruby: # 用 Fiber 或 async gem
来源：http://uw.newstarts.cn

C#:   async Task F() { await G(); }
来源：http://ln.panjiajie.cn

[O05] 并发执行并等待全部完成
来源：http://uh.jianghongdianzi.cn

Py:   asyncio.gather(*tasks)
来源：http://py.gzmigu.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ns.yuexingan06.cn

JS:   await Promise.all(tasks)
来源：http://sv.panjiajie.cn

TS:   await Promise.all(tasks)
来源：http://iy.jctech888.com.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://nr.shxzskj.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://pm.chemitech.net.cn

Ruby: threads.map(&:join)
来源：http://wm.szsharing.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://tw.jctech888.com.cn

[O06] 使用进程池
来源：http://ni.shxzskj.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ea.yuntaijiaju.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://rg.newstarts.cn

JS:   // child_process / cluster 模块
来源：http://rh.lnxyls.cn

TS:   // child_process / cluster 模块
来源：http://ot.nicolike.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://sl.hahajie.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://vw.yuntaijiaju.cn

Ruby: // fork 块
来源：http://on.szxytkj.cn

C#:   Parallel.For
来源：http://bl.panjiajie.cn

================================================================================
来源：http://uo.jianghongdianzi.cn

P. 常用工具函数
来源：http://ig.bjjhwx.cn

================================================================================
来源：http://ft.jianghongdianzi.cn

[P01] 生成 UUID
来源：http://zn.nszjky.cn

Py:   str(uuid.uuid4())
来源：http://jy.hahajie.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://dt.jctech888.com.cn

JS:   crypto.randomUUID()
来源：http://lk.bookmarksfly.cn


<!-- 参考信息 -->