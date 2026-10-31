代发 wailian999

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nr.huanxung.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://zy.haigaiapp.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jj.muxihuayi.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://uf.jctech888.com.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://rx.jctech888.com.cn

[L04] 设置超时
来源：http://qu.lnxyls.cn

Py:   requests.get(url, timeout=5)
来源：http://os.hnjuh.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hj.yuntaijiaju.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zc.muxihuayi.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cu.521024.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://pb.shxzskj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ho.szsharing.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ea.asd995.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://jk.hahajie.cn

[L05] 上传文件（multipart）
来源：http://rb.shxzskj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://dc.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://qx.newstarts.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hm.bookmarksfly.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://zh.huixiangedu.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://lf.panjiajie.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://vr.yuexingan06.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ui.haigaiapp.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://zs.haigaiapp.cn

[L06] 解析响应为 JSON
来源：http://aj.huixiangedu.cn

Py:   resp.json()
来源：http://ts.bookmarksfly.cn

PHP:  json_decode($body, true);
来源：http://om.wgjwhj.cn

JS:   await resp.json()
来源：http://so.9csxet.cn

TS:   await resp.json()
来源：http://pn.colortex.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ek.shtwfgs.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ae.bookmarksfly.cn

Ruby: JSON.parse(resp.body)
来源：http://kr.shtwfgs.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://tu.gzmigu.cn

[L07] 处理 HTTP 状态码
来源：http://jz.asd995.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://nr.muxihuayi.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://jr.huixinmuqiang.cn

JS:   resp.ok;  resp.status
来源：http://zk.lnxyls.cn

TS:   resp.ok;  resp.status
来源：http://oq.nicolike.cn

Java: resp.statusCode()
来源：http://kn.chemitech.net.cn

Go:   resp.StatusCode
来源：http://bj.huixinmuqiang.cn

Ruby: resp.code.to_i
来源：http://rl.hahajie.cn

C#:   (int)resp.StatusCode
来源：http://bp.huixinmuqiang.cn

[L08] 并发请求多个地址
来源：http://vh.shxzukj.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://rh.shtwfgs.cn

PHP:  curl_multi_init() 系列
来源：http://xa.bookmarksfly.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://td.nicolike.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tl.gzmigu.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://jn.shxzukj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://kz.hnjuh.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://bm.lnxyls.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://nu.yuexingan06.cn

================================================================================
来源：http://jc.huixinmuqiang.cn

M. 命令行 / 进程 / 环境
来源：http://st.bookmarksfly.cn

================================================================================
来源：http://mt.shtwfgs.cn

[M01] 读取命令行参数
来源：http://cx.huanxung.cn

Py:   sys.argv[1:]
来源：http://bk.huixinmuqiang.cn

PHP:  $argv;  $argc;
来源：http://wb.yuntaijiaju.cn

JS:   process.argv.slice(2)
来源：http://bp.asd995.cn

TS:   process.argv.slice(2)
来源：http://ih.panjiajie.cn

Java: args 数组（main 方法参数）
来源：http://gd.huanxung.cn

Go:   os.Args[1:]
来源：http://cr.bjjhwx.cn

Ruby: ARGV
来源：http://vn.9csxet.cn

C#:   args 数组（Main 方法参数）
来源：http://jd.nicolike.cn

[M02] 读取环境变量
来源：http://kt.shxzukj.cn

Py:   os.environ.get("HOME")
来源：http://cp.jianghongdianzi.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rx.haigaiapp.cn

JS:   process.env.HOME
来源：http://wo.yuntaijiaju.cn

TS:   process.env.HOME
来源：http://rp.yuntaijiaju.cn

Java: System.getenv("HOME")
来源：http://vw.lnxyls.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://em.shxzskj.cn

Ruby: ENV["HOME"]
来源：http://gj.bookmarksfly.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://xa.shxzukj.cn

[M03] 执行外部命令
来源：http://hg.nszjky.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hy.chemitech.net.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://fs.huixiangedu.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://lp.huixiangedu.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://jx.yuntaijiaju.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wa.521024.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://vn.9csxet.cn

Ruby: system("ls -l");  `ls -l`
来源：http://yz.bjjhwx.cn

C#:   Process.Start("ls", "-l");
来源：http://jz.szxytkj.cn

[M04] 获取当前工作目录
来源：http://ie.shxzukj.cn

Py:   os.getcwd()
来源：http://aq.yuexingan06.cn

PHP:  getcwd();
来源：http://fy.bookmarksfly.cn

JS:   process.cwd()
来源：http://wa.nszjky.cn

TS:   process.cwd()
来源：http://oe.jctech888.com.cn

Java: Path.of("").toAbsolutePath()
来源：http://lm.huanxung.cn

Go:   os.Getwd()
来源：http://qm.asd995.cn

Ruby: Dir.pwd
来源：http://nl.nicolike.cn

C#:   Directory.GetCurrentDirectory()
来源：http://jx.yuexingan06.cn

[M05] 设置退出码
来源：http://hx.521024.cn

Py:   sys.exit(1)
来源：http://fp.colortex.cn

PHP:  exit(1);
来源：http://ep.yuexingan06.cn

JS:   process.exit(1)
来源：http://rg.lnxyls.cn

TS:   process.exit(1)
来源：http://sx.huixiangedu.cn

Java: System.exit(1)
来源：http://xu.huixiangedu.cn

Go:   os.Exit(1)
来源：http://ks.hnjuh.cn

Ruby: exit 1
来源：http://mq.panjiajie.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://nu.yuntaijiaju.cn

[M06] 向标准错误输出
来源：http://bo.bookmarksfly.cn

Py:   print("err", file=sys.stderr)
来源：http://kq.lnxyls.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://zd.muxihuayi.cn

JS:   console.error("err")
来源：http://to.szxytkj.cn

TS:   console.error("err")
来源：http://gf.shxzukj.cn

Java: System.err.println("err")
来源：http://et.bjjhwx.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://sr.shxzukj.cn

Ruby: warn "err"
来源：http://xm.shxzskj.cn

C#:   Console.Error.WriteLine("err")
来源：http://qy.szsharing.cn

[M07] 判断是否为主入口
来源：http://bf.bjjhwx.cn

Py:   if __name__ == "__main__":
来源：http://yj.nszjky.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://qg.bookmarksfly.cn

JS:   require.main === module
来源：http://ls.chemitech.net.cn

TS:   require.main === module
来源：http://om.huixinmuqiang.cn

Java: public static void main(String[] args)
来源：http://qr.wgjwhj.cn

Go:   func main()
来源：http://kp.nszjky.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://og.hahajie.cn

C#:   static void Main(string[] args)
来源：http://xy.wgjwhj.cn

[M08] 获取系统与运行时信息
来源：http://xg.wgjwhj.cn

Py:   platform.system();  platform.python_version()
来源：http://oc.gzmigu.cn

PHP:  PHP_OS;  phpversion();
来源：http://fz.bookmarksfly.cn

JS:   process.platform;  process.version
来源：http://xg.chemitech.net.cn

TS:   process.platform;  process.version
来源：http://tr.panjiajie.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://fv.newstarts.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://um.huanxung.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://jy.huanxung.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://jo.wgjwhj.cn

================================================================================
来源：http://hx.shxzskj.cn

N. 数据结构与算法
来源：http://nt.hnjuh.cn

================================================================================
来源：http://he.bookmarksfly.cn

[N01] 二分查找（有序数组）
来源：http://pm.lnxyls.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ly.hnjuh.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://nh.haigaiapp.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fl.newstarts.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://il.bjjhwx.cn

Java: Arrays.binarySearch(arr, x)
来源：http://fm.newstarts.cn

Go:   sort.SearchInts(arr, x)
来源：http://yt.wgjwhj.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://lc.nszjky.cn

C#:   Array.BinarySearch(arr, x)
来源：http://rd.szxytkj.cn

[N02] 排序（工程实践用内置实现）
来源：http://gg.newstarts.cn

Py:   sorted(arr);  arr.sort()
来源：http://ai.panjiajie.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ne.nicolike.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ax.szxytkj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ul.haigaiapp.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://xi.jctech888.com.cn

Go:   slices.Sort(arr)
来源：http://qu.yuexingan06.cn

Ruby: arr.sort
来源：http://de.huanxung.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ng.bjjhwx.cn

[N03] 快速排序（分治示例）
来源：http://nw.bjjhwx.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://zg.colortex.cn

PHP:  // 递归实现，或用 usort
来源：http://mo.hnjuh.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sc.muxihuayi.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uw.muxihuayi.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://dp.nszjky.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ey.haigaiapp.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xb.szsharing.cn

C#:   // 手写递归，或 Array.Sort
来源：http://lf.huixinmuqiang.cn

[N04] 斐波那契数列
来源：http://ba.521024.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://bc.lnxyls.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://di.521024.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://iu.chemitech.net.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://so.panjiajie.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://qk.jctech888.com.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://xq.chemitech.net.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hi.lnxyls.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://yz.9csxet.cn

[N05] 最大公约数
来源：http://as.jctech888.com.cn

Py:   math.gcd(a, b)
来源：http://tc.nszjky.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://up.9csxet.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://oe.bjjhwx.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://aq.yuexingan06.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://af.chemitech.net.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://tj.9csxet.cn

Ruby: a.gcd(b)
来源：http://lo.521024.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://oa.szsharing.cn

[N06] 判断回文字符串
来源：http://ky.colortex.cn

Py:   s == s[::-1]
来源：http://wo.chemitech.net.cn

PHP:  $s === strrev($s);
来源：http://kd.haigaiapp.cn

JS:   s === [...s].reverse().join("")
来源：http://xp.gzmigu.cn

TS:   s === [...s].reverse().join("")
来源：http://si.yuexingan06.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://lj.huixiangedu.cn

Go:   // 双指针从两端比较
来源：http://nu.yuntaijiaju.cn

Ruby: s == s.reverse
来源：http://gz.newstarts.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://zu.shxzukj.cn

[N07] 两数之和（返回下标）
来源：http://bc.521024.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://dg.shxzskj.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://cr.shtwfgs.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://mi.jctech888.com.cn

TS:   // 手写 Map<string, number>
来源：http://go.9csxet.cn

Java: // 手写 HashMap
来源：http://fs.muxihuayi.cn

Go:   // 手写 map[int]int
来源：http://hg.panjiajie.cn

Ruby: // 手写 Hash
来源：http://ck.9csxet.cn

C#:   // 手写 Dictionary<int, int>
来源：http://gk.huixinmuqiang.cn

[N08] 生成全排列
来源：http://ss.huixinmuqiang.cn

Py:   itertools.permutations(arr)
来源：http://xn.shxzukj.cn

PHP:  // 手写递归交换
来源：http://ce.shxzukj.cn

JS:   // 手写回溯递归
来源：http://km.newstarts.cn

TS:   // 手写回溯递归
来源：http://ug.panjiajie.cn

Java: // 手写回溯递归
来源：http://vv.shxzskj.cn

Go:   // 手写回溯递归
来源：http://yx.haigaiapp.cn

Ruby: arr.permutation.to_a
来源：http://jn.yuexingan06.cn

C#:   // 手写回溯递归
来源：http://le.panjiajie.cn

[N09] 栈与队列
来源：http://qd.hahajie.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ap.shxzukj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hd.lnxyls.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://no.panjiajie.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://zu.jianghongdianzi.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://qs.bjjhwx.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://cs.jctech888.com.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://om.huixiangedu.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://eh.yuexingan06.cn

[N10] 链表节点定义
来源：http://bs.szsharing.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://xd.gzmigu.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://jw.shxzukj.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://kb.panjiajie.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://zh.newstarts.cn

Java: class Node { int v; Node next; }
来源：http://zw.colortex.cn

Go:   type Node struct { V int; Next *Node }
来源：http://dp.shtwfgs.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ai.asd995.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://mp.colortex.cn

[N11] 二叉树中序遍历
来源：http://ri.shxzukj.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://si.shtwfgs.cn

PHP:  // 手写递归函数
来源：http://aa.shxzskj.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://uh.9csxet.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gy.shxzukj.cn

Java: // 手写递归
来源：http://ra.huixiangedu.cn

Go:   // 手写递归
来源：http://ht.jianghongdianzi.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ex.9csxet.cn

C#:   // 手写递归
来源：http://zh.lnxyls.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://cv.bookmarksfly.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ih.asd995.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://tx.asd995.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://do.jctech888.com.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wm.chemitech.net.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ng.hnjuh.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ow.szxytkj.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://fs.jianghongdianzi.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://kj.colortex.cn

================================================================================
来源：http://nv.nszjky.cn

O. 并发与异步
来源：http://ty.nszjky.cn

================================================================================
来源：http://lk.lnxyls.cn

[O01] 启动一个线程
来源：http://st.hnjuh.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://dl.huixinmuqiang.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://uo.jctech888.com.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wf.yuexingan06.cn

TS:   // 同 JS
来源：http://it.yuntaijiaju.cn

Java: new Thread(() -> f()).start()
来源：http://fc.newstarts.cn

Go:   go f()
来源：http://ct.yuexingan06.cn

Ruby: Thread.new { f }
来源：http://xt.nszjky.cn

C#:   Task.Run(() => F());
来源：http://ot.bjjhwx.cn

[O02] 使用线程池
来源：http://hr.yuntaijiaju.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://kb.asd995.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://tc.szsharing.cn

JS:   // worker_threads 线程池
来源：http://ai.bookmarksfly.cn

TS:   // worker_threads 线程池
来源：http://bc.chemitech.net.cn

Java: Executors.newFixedThreadPool(4)
来源：http://rn.muxihuayi.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://cd.hnjuh.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ro.nszjky.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://bf.nszjky.cn

[O03] 加锁保护共享数据
来源：http://jx.bjjhwx.cn

Py:   with lock: shared += 1
来源：http://uo.newstarts.cn

PHP:  // 用 flock() 做文件锁
来源：http://bs.lnxyls.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://zz.9csxet.cn

TS:   // 同 JS
来源：http://cy.bjjhwx.cn

Java: synchronized (this) { shared++; }
来源：http://hd.hnjuh.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mx.521024.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://bt.wgjwhj.cn

C#:   lock (gate) { shared++; }
来源：http://vg.muxihuayi.cn

[O04] 定义异步函数并等待
来源：http://da.521024.cn

Py:   async def f():⏎    await g()
来源：http://qj.newstarts.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://dj.haigaiapp.cn

JS:   async function f() { await g(); }
来源：http://bc.colortex.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://uq.shxzskj.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://qp.shxzskj.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://jw.newstarts.cn

Ruby: # 用 Fiber 或 async gem
来源：http://qr.yuntaijiaju.cn

C#:   async Task F() { await G(); }
来源：http://em.nszjky.cn

[O05] 并发执行并等待全部完成
来源：http://ke.shtwfgs.cn

Py:   asyncio.gather(*tasks)
来源：http://xl.9csxet.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://cd.colortex.cn

JS:   await Promise.all(tasks)
来源：http://uf.hahajie.cn

TS:   await Promise.all(tasks)
来源：http://ke.nszjky.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://nr.panjiajie.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ll.jctech888.com.cn

Ruby: threads.map(&:join)
来源：http://lf.bjjhwx.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://wb.asd995.cn

[O06] 使用进程池
来源：http://gc.asd995.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://gp.haigaiapp.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ah.colortex.cn

JS:   // child_process / cluster 模块
来源：http://no.hahajie.cn

TS:   // child_process / cluster 模块
来源：http://pk.huixinmuqiang.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://be.muxihuayi.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://xp.muxihuayi.cn

Ruby: // fork 块
来源：http://gv.huixinmuqiang.cn

C#:   Parallel.For
来源：http://kq.huixiangedu.cn

================================================================================
来源：http://lv.hnjuh.cn

P. 常用工具函数
来源：http://jc.shxzukj.cn

================================================================================
来源：http://mf.huanxung.cn

[P01] 生成 UUID
来源：http://km.yuexingan06.cn

Py:   str(uuid.uuid4())
来源：http://zn.asd995.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ij.hnjuh.cn

JS:   crypto.randomUUID()
来源：http://tv.panjiajie.cn


<!-- 参考信息 -->