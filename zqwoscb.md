代发 wailian999

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qf.asd995.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qk.chemitech.net.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://bt.shxzskj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wy.panjiajie.cn

[L03] 设置自定义请求头
来源：http://ws.shtwfgs.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://yj.nszjky.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hn.szxytkj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://so.shxzskj.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mu.huixiangedu.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ts.huixinmuqiang.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://kg.gzmigu.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://fg.huanxung.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://kh.newstarts.cn

[L04] 设置超时
来源：http://zz.newstarts.cn

Py:   requests.get(url, timeout=5)
来源：http://hc.521024.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xj.asd995.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fy.gzmigu.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://du.gzmigu.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wt.jctech888.com.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wq.chemitech.net.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://da.nszjky.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://it.521024.cn

[L05] 上传文件（multipart）
来源：http://kw.panjiajie.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://bk.wgjwhj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ad.huanxung.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://eb.yuexingan06.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://to.haigaiapp.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://if.haigaiapp.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://eh.bookmarksfly.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://uc.hahajie.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://nb.bjjhwx.cn

[L06] 解析响应为 JSON
来源：http://tu.9csxet.cn

Py:   resp.json()
来源：http://op.wgjwhj.cn

PHP:  json_decode($body, true);
来源：http://on.huixinmuqiang.cn

JS:   await resp.json()
来源：http://rr.yuntaijiaju.cn

TS:   await resp.json()
来源：http://qp.wgjwhj.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mw.asd995.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://bj.521024.cn

Ruby: JSON.parse(resp.body)
来源：http://gb.yuexingan06.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://up.asd995.cn

[L07] 处理 HTTP 状态码
来源：http://xc.panjiajie.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://zf.wgjwhj.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wj.chemitech.net.cn

JS:   resp.ok;  resp.status
来源：http://rn.yuexingan06.cn

TS:   resp.ok;  resp.status
来源：http://mj.nicolike.cn

Java: resp.statusCode()
来源：http://bt.szsharing.cn

Go:   resp.StatusCode
来源：http://zg.hahajie.cn

Ruby: resp.code.to_i
来源：http://ic.bjjhwx.cn

C#:   (int)resp.StatusCode
来源：http://np.shxzukj.cn

[L08] 并发请求多个地址
来源：http://bd.huixinmuqiang.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://gp.wgjwhj.cn

PHP:  curl_multi_init() 系列
来源：http://bi.chemitech.net.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://oc.bookmarksfly.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hb.newstarts.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://yh.haigaiapp.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mg.yuexingan06.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vi.yuexingan06.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://pf.shxzskj.cn

================================================================================
来源：http://ah.wgjwhj.cn

M. 命令行 / 进程 / 环境
来源：http://fh.shxzukj.cn

================================================================================
来源：http://oa.lnxyls.cn

[M01] 读取命令行参数
来源：http://vc.hnjuh.cn

Py:   sys.argv[1:]
来源：http://tl.asd995.cn

PHP:  $argv;  $argc;
来源：http://ls.chemitech.net.cn

JS:   process.argv.slice(2)
来源：http://bc.chemitech.net.cn

TS:   process.argv.slice(2)
来源：http://pe.yuntaijiaju.cn

Java: args 数组（main 方法参数）
来源：http://cq.jianghongdianzi.cn

Go:   os.Args[1:]
来源：http://vr.bookmarksfly.cn

Ruby: ARGV
来源：http://sc.szsharing.cn

C#:   args 数组（Main 方法参数）
来源：http://my.szxytkj.cn

[M02] 读取环境变量
来源：http://yx.jctech888.com.cn

Py:   os.environ.get("HOME")
来源：http://fc.muxihuayi.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://yn.huixiangedu.cn

JS:   process.env.HOME
来源：http://cq.jctech888.com.cn

TS:   process.env.HOME
来源：http://we.gzmigu.cn

Java: System.getenv("HOME")
来源：http://cx.huanxung.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://um.wgjwhj.cn

Ruby: ENV["HOME"]
来源：http://sf.yuntaijiaju.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hy.muxihuayi.cn

[M03] 执行外部命令
来源：http://xl.gzmigu.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://no.jctech888.com.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zd.gzmigu.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://jj.jianghongdianzi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://vk.huixiangedu.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://gt.gzmigu.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://dc.shxzukj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ce.jctech888.com.cn

C#:   Process.Start("ls", "-l");
来源：http://ym.shtwfgs.cn

[M04] 获取当前工作目录
来源：http://rt.bjjhwx.cn

Py:   os.getcwd()
来源：http://nk.yuntaijiaju.cn

PHP:  getcwd();
来源：http://uq.haigaiapp.cn

JS:   process.cwd()
来源：http://as.chemitech.net.cn

TS:   process.cwd()
来源：http://ec.asd995.cn

Java: Path.of("").toAbsolutePath()
来源：http://iz.panjiajie.cn

Go:   os.Getwd()
来源：http://wn.asd995.cn

Ruby: Dir.pwd
来源：http://ci.shxzskj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://qq.shxzskj.cn

[M05] 设置退出码
来源：http://ki.chemitech.net.cn

Py:   sys.exit(1)
来源：http://ip.colortex.cn

PHP:  exit(1);
来源：http://tk.jianghongdianzi.cn

JS:   process.exit(1)
来源：http://uq.szsharing.cn

TS:   process.exit(1)
来源：http://ed.yuexingan06.cn

Java: System.exit(1)
来源：http://kr.hahajie.cn

Go:   os.Exit(1)
来源：http://bl.chemitech.net.cn

Ruby: exit 1
来源：http://ax.shxzukj.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://gq.wgjwhj.cn

[M06] 向标准错误输出
来源：http://dh.shtwfgs.cn

Py:   print("err", file=sys.stderr)
来源：http://rw.muxihuayi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://xx.szsharing.cn

JS:   console.error("err")
来源：http://xx.nicolike.cn

TS:   console.error("err")
来源：http://io.gzmigu.cn

Java: System.err.println("err")
来源：http://nz.asd995.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hx.bjjhwx.cn

Ruby: warn "err"
来源：http://yx.jctech888.com.cn

C#:   Console.Error.WriteLine("err")
来源：http://bg.shxzskj.cn

[M07] 判断是否为主入口
来源：http://up.szxytkj.cn

Py:   if __name__ == "__main__":
来源：http://kb.bookmarksfly.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wx.9csxet.cn

JS:   require.main === module
来源：http://wi.haigaiapp.cn

TS:   require.main === module
来源：http://is.lnxyls.cn

Java: public static void main(String[] args)
来源：http://tf.nicolike.cn

Go:   func main()
来源：http://jn.newstarts.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://kj.nszjky.cn

C#:   static void Main(string[] args)
来源：http://gz.shtwfgs.cn

[M08] 获取系统与运行时信息
来源：http://ib.9csxet.cn

Py:   platform.system();  platform.python_version()
来源：http://le.shxzskj.cn

PHP:  PHP_OS;  phpversion();
来源：http://en.huanxung.cn

JS:   process.platform;  process.version
来源：http://bc.nicolike.cn

TS:   process.platform;  process.version
来源：http://qk.colortex.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ug.shtwfgs.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://lp.jctech888.com.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://an.hnjuh.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://jj.lnxyls.cn

================================================================================
来源：http://er.9csxet.cn

N. 数据结构与算法
来源：http://zx.huixinmuqiang.cn

================================================================================
来源：http://zc.colortex.cn

[N01] 二分查找（有序数组）
来源：http://yp.yuntaijiaju.cn

Py:   bisect.bisect_left(arr, x)
来源：http://te.colortex.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://eh.521024.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ar.yuexingan06.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bv.lnxyls.cn

Java: Arrays.binarySearch(arr, x)
来源：http://vm.newstarts.cn

Go:   sort.SearchInts(arr, x)
来源：http://de.hahajie.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://yx.wgjwhj.cn

C#:   Array.BinarySearch(arr, x)
来源：http://kj.yuntaijiaju.cn

[N02] 排序（工程实践用内置实现）
来源：http://ok.yuexingan06.cn

Py:   sorted(arr);  arr.sort()
来源：http://xf.hnjuh.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hx.panjiajie.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://he.huanxung.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://oj.wgjwhj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ga.haigaiapp.cn

Go:   slices.Sort(arr)
来源：http://iw.yuexingan06.cn

Ruby: arr.sort
来源：http://uo.yuexingan06.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://uu.nicolike.cn

[N03] 快速排序（分治示例）
来源：http://kw.huixinmuqiang.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://yv.szxytkj.cn

PHP:  // 递归实现，或用 usort
来源：http://lc.haigaiapp.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://eg.szsharing.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lx.hahajie.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://yz.huixiangedu.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://sl.shxzukj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://jx.jianghongdianzi.cn

C#:   // 手写递归，或 Array.Sort
来源：http://jx.bookmarksfly.cn

[N04] 斐波那契数列
来源：http://zs.szxytkj.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ne.hahajie.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://iq.bookmarksfly.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xm.nszjky.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dg.szsharing.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://lk.huanxung.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hv.szsharing.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://rt.lnxyls.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://lv.yuexingan06.cn

[N05] 最大公约数
来源：http://kp.shtwfgs.cn

Py:   math.gcd(a, b)
来源：http://sv.wgjwhj.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://sr.muxihuayi.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mm.shtwfgs.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kl.bookmarksfly.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://nj.9csxet.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://lt.haigaiapp.cn

Ruby: a.gcd(b)
来源：http://gb.bookmarksfly.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://cu.yuntaijiaju.cn

[N06] 判断回文字符串
来源：http://mh.huixiangedu.cn

Py:   s == s[::-1]
来源：http://th.bookmarksfly.cn

PHP:  $s === strrev($s);
来源：http://by.shxzukj.cn

JS:   s === [...s].reverse().join("")
来源：http://zm.shxzukj.cn

TS:   s === [...s].reverse().join("")
来源：http://js.bjjhwx.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://tt.521024.cn

Go:   // 双指针从两端比较
来源：http://dk.shxzskj.cn

Ruby: s == s.reverse
来源：http://dl.shxzukj.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://sf.shxzukj.cn

[N07] 两数之和（返回下标）
来源：http://up.lnxyls.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mz.muxihuayi.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://oz.yuntaijiaju.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://dg.wgjwhj.cn

TS:   // 手写 Map<string, number>
来源：http://jd.jianghongdianzi.cn

Java: // 手写 HashMap
来源：http://po.nicolike.cn

Go:   // 手写 map[int]int
来源：http://pg.shxzskj.cn

Ruby: // 手写 Hash
来源：http://ah.panjiajie.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ig.szsharing.cn

[N08] 生成全排列
来源：http://aq.hahajie.cn

Py:   itertools.permutations(arr)
来源：http://ih.shxzskj.cn

PHP:  // 手写递归交换
来源：http://ti.panjiajie.cn

JS:   // 手写回溯递归
来源：http://rp.panjiajie.cn

TS:   // 手写回溯递归
来源：http://zz.wgjwhj.cn

Java: // 手写回溯递归
来源：http://tf.wgjwhj.cn

Go:   // 手写回溯递归
来源：http://iv.asd995.cn

Ruby: arr.permutation.to_a
来源：http://vh.jianghongdianzi.cn

C#:   // 手写回溯递归
来源：http://vp.jianghongdianzi.cn

[N09] 栈与队列
来源：http://ix.bookmarksfly.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://vg.hnjuh.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://et.yuexingan06.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wz.nicolike.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hi.chemitech.net.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ai.chemitech.net.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://bs.jianghongdianzi.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://yq.yuexingan06.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mg.szsharing.cn

[N10] 链表节点定义
来源：http://jo.huanxung.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://bq.huixiangedu.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://al.huanxung.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mn.yuntaijiaju.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://it.huixiangedu.cn

Java: class Node { int v; Node next; }
来源：http://lj.muxihuayi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://xi.shxzukj.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://rk.9csxet.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://sx.chemitech.net.cn

[N11] 二叉树中序遍历
来源：http://qu.szsharing.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://zi.nicolike.cn

PHP:  // 手写递归函数
来源：http://zl.asd995.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ls.shxzskj.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jj.yuntaijiaju.cn

Java: // 手写递归
来源：http://ur.haigaiapp.cn

Go:   // 手写递归
来源：http://zo.nszjky.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://uj.muxihuayi.cn

C#:   // 手写递归
来源：http://mp.haigaiapp.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://pf.hnjuh.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://qo.asd995.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://gm.gzmigu.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sa.szsharing.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gh.szxytkj.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hu.521024.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ay.newstarts.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://gp.shxzskj.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://dk.haigaiapp.cn

================================================================================
来源：http://ms.hnjuh.cn

O. 并发与异步
来源：http://ds.bookmarksfly.cn

================================================================================
来源：http://ti.muxihuayi.cn

[O01] 启动一个线程
来源：http://xh.newstarts.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://no.colortex.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://fc.jianghongdianzi.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://zt.nicolike.cn

TS:   // 同 JS
来源：http://ud.chemitech.net.cn

Java: new Thread(() -> f()).start()
来源：http://bb.jctech888.com.cn

Go:   go f()
来源：http://fj.panjiajie.cn

Ruby: Thread.new { f }
来源：http://wz.lnxyls.cn

C#:   Task.Run(() => F());
来源：http://ud.szxytkj.cn

[O02] 使用线程池
来源：http://rn.hahajie.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://rj.szsharing.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://rn.newstarts.cn

JS:   // worker_threads 线程池
来源：http://uq.jctech888.com.cn

TS:   // worker_threads 线程池
来源：http://hz.shtwfgs.cn

Java: Executors.newFixedThreadPool(4)
来源：http://wb.huixinmuqiang.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://sr.hnjuh.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://yx.shxzskj.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://tx.jianghongdianzi.cn

[O03] 加锁保护共享数据
来源：http://wt.bjjhwx.cn

Py:   with lock: shared += 1
来源：http://yn.wgjwhj.cn

PHP:  // 用 flock() 做文件锁
来源：http://ev.wgjwhj.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ct.chemitech.net.cn

TS:   // 同 JS
来源：http://kt.bookmarksfly.cn

Java: synchronized (this) { shared++; }
来源：http://fk.hnjuh.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://pu.bjjhwx.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://bl.asd995.cn

C#:   lock (gate) { shared++; }
来源：http://tw.jctech888.com.cn

[O04] 定义异步函数并等待
来源：http://qi.521024.cn

Py:   async def f():⏎    await g()
来源：http://mn.panjiajie.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wt.colortex.cn

JS:   async function f() { await g(); }
来源：http://zz.jianghongdianzi.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ly.gzmigu.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wy.shtwfgs.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ao.hahajie.cn

Ruby: # 用 Fiber 或 async gem
来源：http://mp.wgjwhj.cn

C#:   async Task F() { await G(); }
来源：http://ey.hnjuh.cn

[O05] 并发执行并等待全部完成
来源：http://lo.jctech888.com.cn

Py:   asyncio.gather(*tasks)
来源：http://ne.hahajie.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wg.chemitech.net.cn

JS:   await Promise.all(tasks)
来源：http://ua.szsharing.cn

TS:   await Promise.all(tasks)
来源：http://vg.huanxung.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://tu.yuexingan06.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://nv.jianghongdianzi.cn

Ruby: threads.map(&:join)
来源：http://aj.huixinmuqiang.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://vx.jctech888.com.cn

[O06] 使用进程池
来源：http://ib.9csxet.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://nk.shxzskj.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://rd.shxzukj.cn

JS:   // child_process / cluster 模块
来源：http://ed.muxihuayi.cn

TS:   // child_process / cluster 模块
来源：http://yz.bjjhwx.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://oo.bookmarksfly.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://rd.colortex.cn

Ruby: // fork 块
来源：http://rw.huixiangedu.cn


<!-- 参考信息 -->