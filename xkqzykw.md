代发 wailian999

Go:   resp, err := http.Get(url)
来源：http://lt.jctech888.com.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://gq.hnjuh.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://jj.huanxung.cn

[L02] 发送 POST JSON
来源：http://ic.9csxet.cn

Py:   requests.post(url, json={"a": 1})
来源：http://yv.huixiangedu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://se.521024.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zz.9csxet.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ra.newstarts.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://gt.huixinmuqiang.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://bk.huanxung.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://uj.chemitech.net.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ip.bookmarksfly.cn

[L03] 设置自定义请求头
来源：http://vq.bookmarksfly.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://sd.haigaiapp.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://lh.nszjky.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dw.haigaiapp.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cz.yuexingan06.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ir.bjjhwx.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://kh.jianghongdianzi.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://nn.yuntaijiaju.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wv.wgjwhj.cn

[L04] 设置超时
来源：http://cj.huixinmuqiang.cn

Py:   requests.get(url, timeout=5)
来源：http://du.hnjuh.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://lp.panjiajie.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qk.jianghongdianzi.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gx.gzmigu.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ul.colortex.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fr.jctech888.com.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://vi.nszjky.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://cs.muxihuayi.cn

[L05] 上传文件（multipart）
来源：http://yj.huanxung.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://me.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://tw.jianghongdianzi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mz.shtwfgs.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ry.szxytkj.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://zb.bjjhwx.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://lq.wgjwhj.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://dj.bjjhwx.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hf.wgjwhj.cn

[L06] 解析响应为 JSON
来源：http://db.huixinmuqiang.cn

Py:   resp.json()
来源：http://es.jianghongdianzi.cn

PHP:  json_decode($body, true);
来源：http://ly.huixinmuqiang.cn

JS:   await resp.json()
来源：http://yp.chemitech.net.cn

TS:   await resp.json()
来源：http://vq.colortex.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ko.shxzskj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://pp.nicolike.cn

Ruby: JSON.parse(resp.body)
来源：http://yi.nicolike.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ny.panjiajie.cn

[L07] 处理 HTTP 状态码
来源：http://df.huixinmuqiang.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ix.haigaiapp.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://un.huixiangedu.cn

JS:   resp.ok;  resp.status
来源：http://td.shxzukj.cn

TS:   resp.ok;  resp.status
来源：http://qj.newstarts.cn

Java: resp.statusCode()
来源：http://qi.hahajie.cn

Go:   resp.StatusCode
来源：http://zu.bookmarksfly.cn

Ruby: resp.code.to_i
来源：http://sm.jctech888.com.cn

C#:   (int)resp.StatusCode
来源：http://te.colortex.cn

[L08] 并发请求多个地址
来源：http://fr.huanxung.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://gf.shxzskj.cn

PHP:  curl_multi_init() 系列
来源：http://pw.521024.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bi.hahajie.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kb.yuexingan06.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://fc.yuexingan06.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://xu.jctech888.com.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://uv.hahajie.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://fm.chemitech.net.cn

================================================================================
来源：http://hy.wgjwhj.cn

M. 命令行 / 进程 / 环境
来源：http://ca.lnxyls.cn

================================================================================
来源：http://jc.szsharing.cn

[M01] 读取命令行参数
来源：http://me.9csxet.cn

Py:   sys.argv[1:]
来源：http://wd.szsharing.cn

PHP:  $argv;  $argc;
来源：http://nf.szsharing.cn

JS:   process.argv.slice(2)
来源：http://dn.panjiajie.cn

TS:   process.argv.slice(2)
来源：http://iw.asd995.cn

Java: args 数组（main 方法参数）
来源：http://zv.521024.cn

Go:   os.Args[1:]
来源：http://eg.szsharing.cn

Ruby: ARGV
来源：http://xp.wgjwhj.cn

C#:   args 数组（Main 方法参数）
来源：http://ez.newstarts.cn

[M02] 读取环境变量
来源：http://rw.9csxet.cn

Py:   os.environ.get("HOME")
来源：http://mh.yuexingan06.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://en.521024.cn

JS:   process.env.HOME
来源：http://np.hnjuh.cn

TS:   process.env.HOME
来源：http://sz.nicolike.cn

Java: System.getenv("HOME")
来源：http://wh.shxzskj.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mt.shtwfgs.cn

Ruby: ENV["HOME"]
来源：http://mi.asd995.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://my.panjiajie.cn

[M03] 执行外部命令
来源：http://cy.huanxung.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://pf.haigaiapp.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://dy.bookmarksfly.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ep.szxytkj.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://lk.lnxyls.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ri.nszjky.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://wt.huanxung.cn

Ruby: system("ls -l");  `ls -l`
来源：http://la.panjiajie.cn

C#:   Process.Start("ls", "-l");
来源：http://sx.hnjuh.cn

[M04] 获取当前工作目录
来源：http://zr.hnjuh.cn

Py:   os.getcwd()
来源：http://hm.jianghongdianzi.cn

PHP:  getcwd();
来源：http://zr.521024.cn

JS:   process.cwd()
来源：http://ty.huixiangedu.cn

TS:   process.cwd()
来源：http://hy.yuexingan06.cn

Java: Path.of("").toAbsolutePath()
来源：http://ye.nszjky.cn

Go:   os.Getwd()
来源：http://nf.huanxung.cn

Ruby: Dir.pwd
来源：http://sp.huixinmuqiang.cn

C#:   Directory.GetCurrentDirectory()
来源：http://sc.yuexingan06.cn

[M05] 设置退出码
来源：http://if.yuntaijiaju.cn

Py:   sys.exit(1)
来源：http://dm.jianghongdianzi.cn

PHP:  exit(1);
来源：http://fo.nszjky.cn

JS:   process.exit(1)
来源：http://mn.jctech888.com.cn

TS:   process.exit(1)
来源：http://sl.shxzskj.cn

Java: System.exit(1)
来源：http://jw.newstarts.cn

Go:   os.Exit(1)
来源：http://wd.nicolike.cn

Ruby: exit 1
来源：http://oy.huixinmuqiang.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ps.huixiangedu.cn

[M06] 向标准错误输出
来源：http://nf.newstarts.cn

Py:   print("err", file=sys.stderr)
来源：http://oq.bjjhwx.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://xd.newstarts.cn

JS:   console.error("err")
来源：http://qa.wgjwhj.cn

TS:   console.error("err")
来源：http://vh.colortex.cn

Java: System.err.println("err")
来源：http://ec.szxytkj.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://jg.asd995.cn

Ruby: warn "err"
来源：http://gp.huixiangedu.cn

C#:   Console.Error.WriteLine("err")
来源：http://eh.shtwfgs.cn

[M07] 判断是否为主入口
来源：http://py.asd995.cn

Py:   if __name__ == "__main__":
来源：http://fl.huixinmuqiang.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://fw.yuexingan06.cn

JS:   require.main === module
来源：http://sb.nicolike.cn

TS:   require.main === module
来源：http://jh.huixinmuqiang.cn

Java: public static void main(String[] args)
来源：http://us.asd995.cn

Go:   func main()
来源：http://bn.shxzskj.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ee.panjiajie.cn

C#:   static void Main(string[] args)
来源：http://ep.jctech888.com.cn

[M08] 获取系统与运行时信息
来源：http://xz.panjiajie.cn

Py:   platform.system();  platform.python_version()
来源：http://vw.colortex.cn

PHP:  PHP_OS;  phpversion();
来源：http://aq.jianghongdianzi.cn

JS:   process.platform;  process.version
来源：http://yn.colortex.cn

TS:   process.platform;  process.version
来源：http://kl.yuexingan06.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ie.jianghongdianzi.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://dr.szsharing.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ef.shxzskj.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://xk.bjjhwx.cn

================================================================================
来源：http://ib.hnjuh.cn

N. 数据结构与算法
来源：http://ia.nszjky.cn

================================================================================
来源：http://zj.huixiangedu.cn

[N01] 二分查找（有序数组）
来源：http://cs.huixiangedu.cn

Py:   bisect.bisect_left(arr, x)
来源：http://aj.nicolike.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://pk.szsharing.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hw.hahajie.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mu.shxzukj.cn

Java: Arrays.binarySearch(arr, x)
来源：http://uw.muxihuayi.cn

Go:   sort.SearchInts(arr, x)
来源：http://fx.huixinmuqiang.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://fn.szxytkj.cn

C#:   Array.BinarySearch(arr, x)
来源：http://jl.gzmigu.cn

[N02] 排序（工程实践用内置实现）
来源：http://jw.panjiajie.cn

Py:   sorted(arr);  arr.sort()
来源：http://dv.9csxet.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://is.nicolike.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://jc.szxytkj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ej.shtwfgs.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://cj.yuexingan06.cn

Go:   slices.Sort(arr)
来源：http://ta.nszjky.cn

Ruby: arr.sort
来源：http://xt.newstarts.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://iw.hahajie.cn

[N03] 快速排序（分治示例）
来源：http://fx.chemitech.net.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hf.shtwfgs.cn

PHP:  // 递归实现，或用 usort
来源：http://ga.yuntaijiaju.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qa.gzmigu.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bi.huanxung.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ei.panjiajie.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ed.huixinmuqiang.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://bh.shtwfgs.cn

C#:   // 手写递归，或 Array.Sort
来源：http://wf.szsharing.cn

[N04] 斐波那契数列
来源：http://pd.haigaiapp.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://gd.yuexingan06.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://np.bjjhwx.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ev.hnjuh.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qy.lnxyls.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ph.shtwfgs.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://jc.huixinmuqiang.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://qx.shtwfgs.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://zi.hnjuh.cn

[N05] 最大公约数
来源：http://la.haigaiapp.cn

Py:   math.gcd(a, b)
来源：http://xj.szxytkj.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://zn.nszjky.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kk.bjjhwx.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dy.nicolike.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://lv.9csxet.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ia.yuntaijiaju.cn

Ruby: a.gcd(b)
来源：http://hl.huixinmuqiang.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://eg.asd995.cn

[N06] 判断回文字符串
来源：http://bj.9csxet.cn

Py:   s == s[::-1]
来源：http://ku.huixinmuqiang.cn

PHP:  $s === strrev($s);
来源：http://rs.shtwfgs.cn

JS:   s === [...s].reverse().join("")
来源：http://jd.szxytkj.cn

TS:   s === [...s].reverse().join("")
来源：http://ly.chemitech.net.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ju.hahajie.cn

Go:   // 双指针从两端比较
来源：http://un.yuntaijiaju.cn

Ruby: s == s.reverse
来源：http://al.newstarts.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://bz.wgjwhj.cn

[N07] 两数之和（返回下标）
来源：http://st.szxytkj.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ug.newstarts.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://sc.hnjuh.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://rt.szxytkj.cn

TS:   // 手写 Map<string, number>
来源：http://ix.nszjky.cn

Java: // 手写 HashMap
来源：http://fh.nszjky.cn

Go:   // 手写 map[int]int
来源：http://kg.newstarts.cn

Ruby: // 手写 Hash
来源：http://nm.chemitech.net.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ft.haigaiapp.cn

[N08] 生成全排列
来源：http://ov.hnjuh.cn

Py:   itertools.permutations(arr)
来源：http://nu.muxihuayi.cn

PHP:  // 手写递归交换
来源：http://bo.yuexingan06.cn

JS:   // 手写回溯递归
来源：http://fn.hnjuh.cn

TS:   // 手写回溯递归
来源：http://xo.huixiangedu.cn

Java: // 手写回溯递归
来源：http://kr.shxzskj.cn

Go:   // 手写回溯递归
来源：http://zm.shxzskj.cn

Ruby: arr.permutation.to_a
来源：http://ni.shtwfgs.cn

C#:   // 手写回溯递归
来源：http://ef.asd995.cn

[N09] 栈与队列
来源：http://yk.bookmarksfly.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://as.wgjwhj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mn.huixiangedu.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://yo.colortex.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://nq.szsharing.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mc.panjiajie.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://vg.9csxet.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://bb.muxihuayi.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://uj.haigaiapp.cn

[N10] 链表节点定义
来源：http://zr.colortex.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ad.hahajie.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://td.huixinmuqiang.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://go.haigaiapp.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://zl.huixinmuqiang.cn

Java: class Node { int v; Node next; }
来源：http://nx.jianghongdianzi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://nu.asd995.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://fo.huanxung.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://oh.shxzukj.cn

[N11] 二叉树中序遍历
来源：http://jt.wgjwhj.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://br.jctech888.com.cn

PHP:  // 手写递归函数
来源：http://ea.haigaiapp.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qz.bookmarksfly.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jy.lnxyls.cn

Java: // 手写递归
来源：http://gn.gzmigu.cn

Go:   // 手写递归
来源：http://bs.newstarts.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ed.hahajie.cn

C#:   // 手写递归
来源：http://nz.szxytkj.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://zf.hnjuh.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://iy.shtwfgs.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://jv.jianghongdianzi.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ap.huixinmuqiang.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kh.nicolike.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://qk.chemitech.net.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://xn.hnjuh.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://nh.haigaiapp.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://go.panjiajie.cn

================================================================================
来源：http://xv.bjjhwx.cn

O. 并发与异步
来源：http://hu.asd995.cn

================================================================================
来源：http://ap.asd995.cn

[O01] 启动一个线程
来源：http://ug.gzmigu.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hf.huixinmuqiang.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://yf.hnjuh.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ci.asd995.cn

TS:   // 同 JS
来源：http://dk.shxzukj.cn

Java: new Thread(() -> f()).start()
来源：http://tc.bjjhwx.cn

Go:   go f()
来源：http://dy.wgjwhj.cn

Ruby: Thread.new { f }
来源：http://te.521024.cn

C#:   Task.Run(() => F());
来源：http://iq.hahajie.cn

[O02] 使用线程池
来源：http://qw.wgjwhj.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://pu.hahajie.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ok.chemitech.net.cn

JS:   // worker_threads 线程池
来源：http://xw.lnxyls.cn

TS:   // worker_threads 线程池
来源：http://fb.521024.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ds.haigaiapp.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://qe.panjiajie.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://uf.huixiangedu.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://un.nszjky.cn

[O03] 加锁保护共享数据
来源：http://ig.haigaiapp.cn

Py:   with lock: shared += 1
来源：http://ar.jctech888.com.cn

PHP:  // 用 flock() 做文件锁
来源：http://gu.huanxung.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://oi.haigaiapp.cn

TS:   // 同 JS
来源：http://mf.jctech888.com.cn

Java: synchronized (this) { shared++; }
来源：http://fv.colortex.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://sl.bjjhwx.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://dw.newstarts.cn

C#:   lock (gate) { shared++; }
来源：http://xy.chemitech.net.cn

[O04] 定义异步函数并等待
来源：http://cn.bookmarksfly.cn

Py:   async def f():⏎    await g()
来源：http://qa.jianghongdianzi.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://iv.newstarts.cn

JS:   async function f() { await g(); }
来源：http://tj.9csxet.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ul.szxytkj.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://em.nicolike.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://qx.huanxung.cn

Ruby: # 用 Fiber 或 async gem
来源：http://zv.bookmarksfly.cn

C#:   async Task F() { await G(); }
来源：http://rm.newstarts.cn

[O05] 并发执行并等待全部完成
来源：http://ga.szsharing.cn

Py:   asyncio.gather(*tasks)
来源：http://lr.shxzskj.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://fc.szxytkj.cn

JS:   await Promise.all(tasks)
来源：http://ba.chemitech.net.cn

TS:   await Promise.all(tasks)
来源：http://sd.shxzskj.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://lh.haigaiapp.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hl.9csxet.cn

Ruby: threads.map(&:join)
来源：http://yn.newstarts.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ow.newstarts.cn


<!-- 参考信息 -->