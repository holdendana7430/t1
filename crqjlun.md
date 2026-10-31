代发 wailian999

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://js.chemitech.net.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ih.panjiajie.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://jw.jctech888.com.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ro.521024.cn

[L03] 设置自定义请求头
来源：http://ac.nszjky.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mu.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://sf.newstarts.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kx.shtwfgs.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dy.9csxet.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://qq.haigaiapp.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://vc.newstarts.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://zw.nicolike.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ay.yuexingan06.cn

[L04] 设置超时
来源：http://wp.szxytkj.cn

Py:   requests.get(url, timeout=5)
来源：http://qd.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://qu.huanxung.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lw.huanxung.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hi.nicolike.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ty.jctech888.com.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://td.bjjhwx.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ou.hnjuh.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://id.yuexingan06.cn

[L05] 上传文件（multipart）
来源：http://wy.bookmarksfly.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://sr.yuntaijiaju.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://xb.colortex.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://eo.newstarts.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ml.muxihuayi.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ui.nszjky.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://oq.521024.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://av.newstarts.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://lw.shtwfgs.cn

[L06] 解析响应为 JSON
来源：http://wl.lnxyls.cn

Py:   resp.json()
来源：http://nd.colortex.cn

PHP:  json_decode($body, true);
来源：http://rc.yuexingan06.cn

JS:   await resp.json()
来源：http://lj.9csxet.cn

TS:   await resp.json()
来源：http://fb.shxzukj.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://gu.yuntaijiaju.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://yf.huixinmuqiang.cn

Ruby: JSON.parse(resp.body)
来源：http://kk.asd995.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://vp.yuexingan06.cn

[L07] 处理 HTTP 状态码
来源：http://qs.szsharing.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://sq.newstarts.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://yd.hnjuh.cn

JS:   resp.ok;  resp.status
来源：http://la.asd995.cn

TS:   resp.ok;  resp.status
来源：http://qx.asd995.cn

Java: resp.statusCode()
来源：http://bt.huanxung.cn

Go:   resp.StatusCode
来源：http://ck.colortex.cn

Ruby: resp.code.to_i
来源：http://ps.lnxyls.cn

C#:   (int)resp.StatusCode
来源：http://wj.haigaiapp.cn

[L08] 并发请求多个地址
来源：http://gg.gzmigu.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://sv.bookmarksfly.cn

PHP:  curl_multi_init() 系列
来源：http://ek.bjjhwx.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gr.szsharing.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://py.haigaiapp.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://pg.wgjwhj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ix.hahajie.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://st.newstarts.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://nn.gzmigu.cn

================================================================================
来源：http://lb.shtwfgs.cn

M. 命令行 / 进程 / 环境
来源：http://qt.wgjwhj.cn

================================================================================
来源：http://zn.521024.cn

[M01] 读取命令行参数
来源：http://kl.yuntaijiaju.cn

Py:   sys.argv[1:]
来源：http://lr.nszjky.cn

PHP:  $argv;  $argc;
来源：http://wr.bjjhwx.cn

JS:   process.argv.slice(2)
来源：http://mh.haigaiapp.cn

TS:   process.argv.slice(2)
来源：http://in.bjjhwx.cn

Java: args 数组（main 方法参数）
来源：http://at.nicolike.cn

Go:   os.Args[1:]
来源：http://sx.huixiangedu.cn

Ruby: ARGV
来源：http://lo.shxzukj.cn

C#:   args 数组（Main 方法参数）
来源：http://tt.521024.cn

[M02] 读取环境变量
来源：http://qw.huixiangedu.cn

Py:   os.environ.get("HOME")
来源：http://tf.shtwfgs.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://pb.chemitech.net.cn

JS:   process.env.HOME
来源：http://wz.gzmigu.cn

TS:   process.env.HOME
来源：http://ih.gzmigu.cn

Java: System.getenv("HOME")
来源：http://di.szsharing.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hk.yuntaijiaju.cn

Ruby: ENV["HOME"]
来源：http://bx.jianghongdianzi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ai.bjjhwx.cn

[M03] 执行外部命令
来源：http://uz.muxihuayi.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://bo.chemitech.net.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wt.panjiajie.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ss.wgjwhj.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://dj.shxzukj.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://qw.huixinmuqiang.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://wd.nicolike.cn

Ruby: system("ls -l");  `ls -l`
来源：http://gh.newstarts.cn

C#:   Process.Start("ls", "-l");
来源：http://qs.szsharing.cn

[M04] 获取当前工作目录
来源：http://pl.huixiangedu.cn

Py:   os.getcwd()
来源：http://lv.szsharing.cn

PHP:  getcwd();
来源：http://yx.9csxet.cn

JS:   process.cwd()
来源：http://ou.chemitech.net.cn

TS:   process.cwd()
来源：http://id.9csxet.cn

Java: Path.of("").toAbsolutePath()
来源：http://tl.panjiajie.cn

Go:   os.Getwd()
来源：http://tw.shtwfgs.cn

Ruby: Dir.pwd
来源：http://mm.shtwfgs.cn

C#:   Directory.GetCurrentDirectory()
来源：http://oz.yuntaijiaju.cn

[M05] 设置退出码
来源：http://ef.hnjuh.cn

Py:   sys.exit(1)
来源：http://xx.szsharing.cn

PHP:  exit(1);
来源：http://hd.lnxyls.cn

JS:   process.exit(1)
来源：http://qu.hnjuh.cn

TS:   process.exit(1)
来源：http://kb.szxytkj.cn

Java: System.exit(1)
来源：http://lu.bjjhwx.cn

Go:   os.Exit(1)
来源：http://rb.jianghongdianzi.cn

Ruby: exit 1
来源：http://el.newstarts.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ey.muxihuayi.cn

[M06] 向标准错误输出
来源：http://yw.wgjwhj.cn

Py:   print("err", file=sys.stderr)
来源：http://mt.muxihuayi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://st.nicolike.cn

JS:   console.error("err")
来源：http://ia.hnjuh.cn

TS:   console.error("err")
来源：http://ag.shtwfgs.cn

Java: System.err.println("err")
来源：http://gx.hahajie.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mr.shxzskj.cn

Ruby: warn "err"
来源：http://mb.szxytkj.cn

C#:   Console.Error.WriteLine("err")
来源：http://nq.newstarts.cn

[M07] 判断是否为主入口
来源：http://sy.szsharing.cn

Py:   if __name__ == "__main__":
来源：http://np.gzmigu.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://lu.wgjwhj.cn

JS:   require.main === module
来源：http://ki.wgjwhj.cn

TS:   require.main === module
来源：http://sx.szxytkj.cn

Java: public static void main(String[] args)
来源：http://kh.nicolike.cn

Go:   func main()
来源：http://zv.wgjwhj.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ff.jianghongdianzi.cn

C#:   static void Main(string[] args)
来源：http://hg.jctech888.com.cn

[M08] 获取系统与运行时信息
来源：http://nn.nicolike.cn

Py:   platform.system();  platform.python_version()
来源：http://bl.huixiangedu.cn

PHP:  PHP_OS;  phpversion();
来源：http://en.yuexingan06.cn

JS:   process.platform;  process.version
来源：http://br.gzmigu.cn

TS:   process.platform;  process.version
来源：http://dh.gzmigu.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://nu.szsharing.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ux.muxihuayi.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://dc.bookmarksfly.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://cz.colortex.cn

================================================================================
来源：http://tq.colortex.cn

N. 数据结构与算法
来源：http://mc.jctech888.com.cn

================================================================================
来源：http://id.nszjky.cn

[N01] 二分查找（有序数组）
来源：http://nf.chemitech.net.cn

Py:   bisect.bisect_left(arr, x)
来源：http://zk.yuntaijiaju.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://nt.huanxung.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wz.huixinmuqiang.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ay.haigaiapp.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ww.hnjuh.cn

Go:   sort.SearchInts(arr, x)
来源：http://ch.shxzskj.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://qv.9csxet.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ux.wgjwhj.cn

[N02] 排序（工程实践用内置实现）
来源：http://vc.9csxet.cn

Py:   sorted(arr);  arr.sort()
来源：http://ak.521024.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://sg.9csxet.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://sq.yuntaijiaju.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://cx.szxytkj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://cn.nicolike.cn

Go:   slices.Sort(arr)
来源：http://tu.chemitech.net.cn

Ruby: arr.sort
来源：http://vs.huixiangedu.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://dc.huixiangedu.cn

[N03] 快速排序（分治示例）
来源：http://nu.szsharing.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://bs.shxzukj.cn

PHP:  // 递归实现，或用 usort
来源：http://yz.szsharing.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sk.chemitech.net.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://so.huixiangedu.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://dy.yuntaijiaju.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hm.bjjhwx.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://qn.hahajie.cn

C#:   // 手写递归，或 Array.Sort
来源：http://tl.chemitech.net.cn

[N04] 斐波那契数列
来源：http://og.yuexingan06.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://rv.huixinmuqiang.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://jj.szsharing.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://od.shxzukj.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hx.nicolike.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://sg.wgjwhj.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ay.szsharing.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ju.colortex.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://qx.shxzskj.cn

[N05] 最大公约数
来源：http://tz.yuntaijiaju.cn

Py:   math.gcd(a, b)
来源：http://gg.nicolike.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hu.huanxung.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mm.szxytkj.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kc.9csxet.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://an.bookmarksfly.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://bl.wgjwhj.cn

Ruby: a.gcd(b)
来源：http://hf.521024.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://aq.gzmigu.cn

[N06] 判断回文字符串
来源：http://nm.jctech888.com.cn

Py:   s == s[::-1]
来源：http://ou.chemitech.net.cn

PHP:  $s === strrev($s);
来源：http://ou.szsharing.cn

JS:   s === [...s].reverse().join("")
来源：http://ur.bookmarksfly.cn

TS:   s === [...s].reverse().join("")
来源：http://sj.huixiangedu.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://sk.shxzukj.cn

Go:   // 双指针从两端比较
来源：http://gu.huanxung.cn

Ruby: s == s.reverse
来源：http://ay.521024.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://mv.lnxyls.cn

[N07] 两数之和（返回下标）
来源：http://cx.nicolike.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://tw.hnjuh.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://xy.chemitech.net.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://sa.muxihuayi.cn

TS:   // 手写 Map<string, number>
来源：http://yh.huixinmuqiang.cn

Java: // 手写 HashMap
来源：http://dj.shxzskj.cn

Go:   // 手写 map[int]int
来源：http://ch.jctech888.com.cn

Ruby: // 手写 Hash
来源：http://ps.bookmarksfly.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ya.chemitech.net.cn

[N08] 生成全排列
来源：http://yn.szsharing.cn

Py:   itertools.permutations(arr)
来源：http://ji.nszjky.cn

PHP:  // 手写递归交换
来源：http://gh.9csxet.cn

JS:   // 手写回溯递归
来源：http://zh.newstarts.cn

TS:   // 手写回溯递归
来源：http://bx.shxzskj.cn

Java: // 手写回溯递归
来源：http://fk.shxzskj.cn

Go:   // 手写回溯递归
来源：http://vs.shxzukj.cn

Ruby: arr.permutation.to_a
来源：http://xa.panjiajie.cn

C#:   // 手写回溯递归
来源：http://vb.newstarts.cn

[N09] 栈与队列
来源：http://gq.chemitech.net.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ht.521024.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ix.huixinmuqiang.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://vu.muxihuayi.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://cb.521024.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://xu.shxzskj.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://is.szsharing.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://rs.lnxyls.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://lq.colortex.cn

[N10] 链表节点定义
来源：http://en.521024.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://un.bookmarksfly.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://vq.szsharing.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://cc.hnjuh.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://nb.jianghongdianzi.cn

Java: class Node { int v; Node next; }
来源：http://wy.panjiajie.cn

Go:   type Node struct { V int; Next *Node }
来源：http://fg.szsharing.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://fk.9csxet.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://wg.newstarts.cn

[N11] 二叉树中序遍历
来源：http://wa.bjjhwx.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://pr.yuntaijiaju.cn

PHP:  // 手写递归函数
来源：http://sm.newstarts.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vr.jianghongdianzi.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fm.asd995.cn

Java: // 手写递归
来源：http://yv.huixinmuqiang.cn

Go:   // 手写递归
来源：http://hq.shxzskj.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://qe.colortex.cn

C#:   // 手写递归
来源：http://lk.shxzskj.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://gr.jctech888.com.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ma.yuexingan06.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://lt.nszjky.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ih.asd995.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sj.shtwfgs.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://uu.lnxyls.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://bg.nszjky.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://km.huixiangedu.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://og.shxzskj.cn

================================================================================
来源：http://xf.shxzskj.cn

O. 并发与异步
来源：http://qa.colortex.cn

================================================================================
来源：http://qu.521024.cn

[O01] 启动一个线程
来源：http://bv.jctech888.com.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://gd.yuexingan06.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qn.shxzskj.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hb.nicolike.cn

TS:   // 同 JS
来源：http://nf.muxihuayi.cn

Java: new Thread(() -> f()).start()
来源：http://vh.jianghongdianzi.cn

Go:   go f()
来源：http://kd.jctech888.com.cn

Ruby: Thread.new { f }
来源：http://gl.wgjwhj.cn

C#:   Task.Run(() => F());
来源：http://gl.jctech888.com.cn

[O02] 使用线程池
来源：http://fo.shxzukj.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mx.huixiangedu.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://fs.panjiajie.cn

JS:   // worker_threads 线程池
来源：http://nm.colortex.cn

TS:   // worker_threads 线程池
来源：http://ja.huanxung.cn

Java: Executors.newFixedThreadPool(4)
来源：http://wn.nszjky.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mw.newstarts.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hp.asd995.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://xa.szxytkj.cn

[O03] 加锁保护共享数据
来源：http://pp.huanxung.cn

Py:   with lock: shared += 1
来源：http://aa.jctech888.com.cn

PHP:  // 用 flock() 做文件锁
来源：http://ja.huixiangedu.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://st.521024.cn

TS:   // 同 JS
来源：http://wr.newstarts.cn

Java: synchronized (this) { shared++; }
来源：http://us.jctech888.com.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://sr.lnxyls.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://tf.yuexingan06.cn

C#:   lock (gate) { shared++; }
来源：http://tn.huixinmuqiang.cn

[O04] 定义异步函数并等待
来源：http://sc.muxihuayi.cn

Py:   async def f():⏎    await g()
来源：http://ii.bookmarksfly.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://xn.shxzukj.cn

JS:   async function f() { await g(); }
来源：http://mr.haigaiapp.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://pr.wgjwhj.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://lc.haigaiapp.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ao.huanxung.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ko.yuntaijiaju.cn

C#:   async Task F() { await G(); }
来源：http://px.huanxung.cn

[O05] 并发执行并等待全部完成
来源：http://ut.muxihuayi.cn

Py:   asyncio.gather(*tasks)
来源：http://cv.yuntaijiaju.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ka.szsharing.cn

JS:   await Promise.all(tasks)
来源：http://qt.yuexingan06.cn

TS:   await Promise.all(tasks)
来源：http://pt.szsharing.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://rg.gzmigu.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://qr.nszjky.cn

Ruby: threads.map(&:join)
来源：http://uc.huixinmuqiang.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://dd.newstarts.cn

[O06] 使用进程池
来源：http://kz.bookmarksfly.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://tf.chemitech.net.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://hw.panjiajie.cn

JS:   // child_process / cluster 模块
来源：http://wu.huixiangedu.cn

TS:   // child_process / cluster 模块
来源：http://ig.9csxet.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://uv.haigaiapp.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://el.shxzukj.cn

Ruby: // fork 块
来源：http://tu.lnxyls.cn


<!-- 参考信息 -->