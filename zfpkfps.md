代发 wailian999

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://tk.shxzskj.cn

JS:   await fetch(url)
来源：http://sf.9csxet.cn

TS:   await fetch(url)
来源：http://ey.szsharing.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://bp.asd995.cn

Go:   resp, err := http.Get(url)
来源：http://sf.haigaiapp.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://nj.yuntaijiaju.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mr.yuexingan06.cn

[L02] 发送 POST JSON
来源：http://se.shxzskj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ep.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ff.yuexingan06.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://el.huixinmuqiang.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xu.newstarts.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://lo.521024.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qm.newstarts.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://yl.hnjuh.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://oy.szsharing.cn

[L03] 设置自定义请求头
来源：http://uy.bookmarksfly.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://qb.nszjky.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://uq.huanxung.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ug.colortex.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ff.hahajie.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://he.huixinmuqiang.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://xm.huixiangedu.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://fs.jctech888.com.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://db.nszjky.cn

[L04] 设置超时
来源：http://bg.huanxung.cn

Py:   requests.get(url, timeout=5)
来源：http://da.yuntaijiaju.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ss.szsharing.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fk.asd995.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://os.panjiajie.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://yh.szsharing.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://vm.hnjuh.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mn.nszjky.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://zf.panjiajie.cn

[L05] 上传文件（multipart）
来源：http://mi.hahajie.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://av.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://zt.521024.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://oz.muxihuayi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xt.newstarts.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://rk.yuexingan06.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://fc.huixinmuqiang.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wd.bookmarksfly.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ck.9csxet.cn

[L06] 解析响应为 JSON
来源：http://bi.newstarts.cn

Py:   resp.json()
来源：http://zn.chemitech.net.cn

PHP:  json_decode($body, true);
来源：http://xx.jctech888.com.cn

JS:   await resp.json()
来源：http://sj.shxzukj.cn

TS:   await resp.json()
来源：http://vq.shxzskj.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://yl.9csxet.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ou.shxzskj.cn

Ruby: JSON.parse(resp.body)
来源：http://hs.gzmigu.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://pa.521024.cn

[L07] 处理 HTTP 状态码
来源：http://pi.asd995.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mn.bookmarksfly.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://gs.muxihuayi.cn

JS:   resp.ok;  resp.status
来源：http://qv.huixiangedu.cn

TS:   resp.ok;  resp.status
来源：http://uh.huixiangedu.cn

Java: resp.statusCode()
来源：http://qd.chemitech.net.cn

Go:   resp.StatusCode
来源：http://jo.colortex.cn

Ruby: resp.code.to_i
来源：http://ti.newstarts.cn

C#:   (int)resp.StatusCode
来源：http://du.shxzskj.cn

[L08] 并发请求多个地址
来源：http://wy.szsharing.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://kz.wgjwhj.cn

PHP:  curl_multi_init() 系列
来源：http://dm.chemitech.net.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ts.colortex.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://eq.yuntaijiaju.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://bs.hnjuh.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://he.muxihuayi.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://xx.asd995.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://fg.9csxet.cn

================================================================================
来源：http://do.nicolike.cn

M. 命令行 / 进程 / 环境
来源：http://aa.newstarts.cn

================================================================================
来源：http://xy.huixinmuqiang.cn

[M01] 读取命令行参数
来源：http://yk.colortex.cn

Py:   sys.argv[1:]
来源：http://vl.yuexingan06.cn

PHP:  $argv;  $argc;
来源：http://mk.jianghongdianzi.cn

JS:   process.argv.slice(2)
来源：http://gf.muxihuayi.cn

TS:   process.argv.slice(2)
来源：http://jv.bjjhwx.cn

Java: args 数组（main 方法参数）
来源：http://fn.bjjhwx.cn

Go:   os.Args[1:]
来源：http://ph.lnxyls.cn

Ruby: ARGV
来源：http://sx.bjjhwx.cn

C#:   args 数组（Main 方法参数）
来源：http://px.521024.cn

[M02] 读取环境变量
来源：http://ut.gzmigu.cn

Py:   os.environ.get("HOME")
来源：http://fd.shxzskj.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zb.muxihuayi.cn

JS:   process.env.HOME
来源：http://qe.shtwfgs.cn

TS:   process.env.HOME
来源：http://ay.haigaiapp.cn

Java: System.getenv("HOME")
来源：http://bf.yuexingan06.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ek.shtwfgs.cn

Ruby: ENV["HOME"]
来源：http://jb.chemitech.net.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://jl.hnjuh.cn

[M03] 执行外部命令
来源：http://ks.szxytkj.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://rt.gzmigu.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wu.colortex.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://lp.colortex.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://vi.jctech888.com.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ee.chemitech.net.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://el.nszjky.cn

Ruby: system("ls -l");  `ls -l`
来源：http://iu.gzmigu.cn

C#:   Process.Start("ls", "-l");
来源：http://az.hnjuh.cn

[M04] 获取当前工作目录
来源：http://mm.9csxet.cn

Py:   os.getcwd()
来源：http://vr.yuexingan06.cn

PHP:  getcwd();
来源：http://qs.jianghongdianzi.cn

JS:   process.cwd()
来源：http://gk.jctech888.com.cn

TS:   process.cwd()
来源：http://qf.colortex.cn

Java: Path.of("").toAbsolutePath()
来源：http://lh.haigaiapp.cn

Go:   os.Getwd()
来源：http://be.yuexingan06.cn

Ruby: Dir.pwd
来源：http://ej.haigaiapp.cn

C#:   Directory.GetCurrentDirectory()
来源：http://uu.wgjwhj.cn

[M05] 设置退出码
来源：http://do.shtwfgs.cn

Py:   sys.exit(1)
来源：http://yr.muxihuayi.cn

PHP:  exit(1);
来源：http://xg.asd995.cn

JS:   process.exit(1)
来源：http://iw.hahajie.cn

TS:   process.exit(1)
来源：http://lq.yuexingan06.cn

Java: System.exit(1)
来源：http://fq.yuexingan06.cn

Go:   os.Exit(1)
来源：http://uj.hnjuh.cn

Ruby: exit 1
来源：http://wr.lnxyls.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mf.lnxyls.cn

[M06] 向标准错误输出
来源：http://lj.521024.cn

Py:   print("err", file=sys.stderr)
来源：http://pz.shtwfgs.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://nf.colortex.cn

JS:   console.error("err")
来源：http://se.huanxung.cn

TS:   console.error("err")
来源：http://ky.bookmarksfly.cn

Java: System.err.println("err")
来源：http://rm.hahajie.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ej.lnxyls.cn

Ruby: warn "err"
来源：http://vn.yuexingan06.cn

C#:   Console.Error.WriteLine("err")
来源：http://yz.bjjhwx.cn

[M07] 判断是否为主入口
来源：http://tu.haigaiapp.cn

Py:   if __name__ == "__main__":
来源：http://ya.wgjwhj.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://tc.szxytkj.cn

JS:   require.main === module
来源：http://qy.chemitech.net.cn

TS:   require.main === module
来源：http://uk.haigaiapp.cn

Java: public static void main(String[] args)
来源：http://nc.hnjuh.cn

Go:   func main()
来源：http://mw.gzmigu.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ks.shxzukj.cn

C#:   static void Main(string[] args)
来源：http://xz.yuexingan06.cn

[M08] 获取系统与运行时信息
来源：http://aa.nszjky.cn

Py:   platform.system();  platform.python_version()
来源：http://zu.newstarts.cn

PHP:  PHP_OS;  phpversion();
来源：http://ul.muxihuayi.cn

JS:   process.platform;  process.version
来源：http://ca.9csxet.cn

TS:   process.platform;  process.version
来源：http://vb.muxihuayi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://dc.nszjky.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://yx.521024.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://on.muxihuayi.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://es.huanxung.cn

================================================================================
来源：http://vc.9csxet.cn

N. 数据结构与算法
来源：http://sj.jctech888.com.cn

================================================================================
来源：http://gm.hnjuh.cn

[N01] 二分查找（有序数组）
来源：http://ol.jianghongdianzi.cn

Py:   bisect.bisect_left(arr, x)
来源：http://qp.huanxung.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://dy.shxzukj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lo.huixinmuqiang.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rr.colortex.cn

Java: Arrays.binarySearch(arr, x)
来源：http://rh.yuexingan06.cn

Go:   sort.SearchInts(arr, x)
来源：http://qe.asd995.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://hb.bookmarksfly.cn

C#:   Array.BinarySearch(arr, x)
来源：http://nm.gzmigu.cn

[N02] 排序（工程实践用内置实现）
来源：http://is.nszjky.cn

Py:   sorted(arr);  arr.sort()
来源：http://el.bookmarksfly.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hl.szxytkj.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://dj.szsharing.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://yw.jianghongdianzi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://cd.panjiajie.cn

Go:   slices.Sort(arr)
来源：http://lz.chemitech.net.cn

Ruby: arr.sort
来源：http://pz.gzmigu.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://rx.wgjwhj.cn

[N03] 快速排序（分治示例）
来源：http://yt.newstarts.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.huixinmuqiang.cn

PHP:  // 递归实现，或用 usort
来源：http://pn.colortex.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ur.shxzskj.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hi.huanxung.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wx.jianghongdianzi.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ff.huixinmuqiang.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://qm.haigaiapp.cn

C#:   // 手写递归，或 Array.Sort
来源：http://hq.shtwfgs.cn

[N04] 斐波那契数列
来源：http://an.szxytkj.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://lr.colortex.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://yl.shxzukj.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gn.asd995.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qf.shtwfgs.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://qc.9csxet.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://dp.szsharing.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://db.shtwfgs.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://pq.9csxet.cn

[N05] 最大公约数
来源：http://vx.szsharing.cn

Py:   math.gcd(a, b)
来源：http://fw.huanxung.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://jl.huanxung.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tv.yuntaijiaju.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zd.panjiajie.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://pp.colortex.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://qb.huixiangedu.cn

Ruby: a.gcd(b)
来源：http://zd.521024.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ey.szsharing.cn

[N06] 判断回文字符串
来源：http://mj.lnxyls.cn

Py:   s == s[::-1]
来源：http://ge.szsharing.cn

PHP:  $s === strrev($s);
来源：http://mn.asd995.cn

JS:   s === [...s].reverse().join("")
来源：http://mf.huixiangedu.cn

TS:   s === [...s].reverse().join("")
来源：http://ji.bjjhwx.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://pe.shxzukj.cn

Go:   // 双指针从两端比较
来源：http://vh.muxihuayi.cn

Ruby: s == s.reverse
来源：http://vr.nicolike.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://gy.jctech888.com.cn

[N07] 两数之和（返回下标）
来源：http://lc.nicolike.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wo.huanxung.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://bs.yuexingan06.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://as.haigaiapp.cn

TS:   // 手写 Map<string, number>
来源：http://mk.hahajie.cn

Java: // 手写 HashMap
来源：http://zv.newstarts.cn

Go:   // 手写 map[int]int
来源：http://jt.bjjhwx.cn

Ruby: // 手写 Hash
来源：http://pn.shxzukj.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ms.jctech888.com.cn

[N08] 生成全排列
来源：http://nc.jianghongdianzi.cn

Py:   itertools.permutations(arr)
来源：http://jz.colortex.cn

PHP:  // 手写递归交换
来源：http://ks.yuntaijiaju.cn

JS:   // 手写回溯递归
来源：http://ut.nszjky.cn

TS:   // 手写回溯递归
来源：http://cf.gzmigu.cn

Java: // 手写回溯递归
来源：http://it.huixinmuqiang.cn

Go:   // 手写回溯递归
来源：http://og.shtwfgs.cn

Ruby: arr.permutation.to_a
来源：http://zd.panjiajie.cn

C#:   // 手写回溯递归
来源：http://sj.gzmigu.cn

[N09] 栈与队列
来源：http://kk.hnjuh.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://el.huixinmuqiang.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ae.huanxung.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://oq.asd995.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://re.yuexingan06.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://kw.huixinmuqiang.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://de.gzmigu.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hd.chemitech.net.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://qo.asd995.cn

[N10] 链表节点定义
来源：http://ka.bjjhwx.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://rb.shxzskj.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://sy.muxihuayi.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://rb.hnjuh.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://fq.haigaiapp.cn

Java: class Node { int v; Node next; }
来源：http://qu.jctech888.com.cn

Go:   type Node struct { V int; Next *Node }
来源：http://rh.asd995.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://td.haigaiapp.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ze.gzmigu.cn

[N11] 二叉树中序遍历
来源：http://wp.9csxet.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://bb.newstarts.cn

PHP:  // 手写递归函数
来源：http://uj.yuexingan06.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://og.gzmigu.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://se.asd995.cn

Java: // 手写递归
来源：http://mz.muxihuayi.cn

Go:   // 手写递归
来源：http://gi.yuntaijiaju.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wj.jianghongdianzi.cn

C#:   // 手写递归
来源：http://sp.lnxyls.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://vm.szxytkj.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://cq.haigaiapp.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://km.hahajie.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ps.newstarts.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zk.hnjuh.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://uy.wgjwhj.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://zo.asd995.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://eg.colortex.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://lm.521024.cn

================================================================================
来源：http://ot.nszjky.cn

O. 并发与异步
来源：http://xk.huixiangedu.cn

================================================================================
来源：http://ea.newstarts.cn

[O01] 启动一个线程
来源：http://ul.newstarts.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wz.jctech888.com.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://lw.nicolike.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://tb.jianghongdianzi.cn

TS:   // 同 JS
来源：http://wo.nszjky.cn

Java: new Thread(() -> f()).start()
来源：http://uu.huanxung.cn

Go:   go f()
来源：http://ly.haigaiapp.cn

Ruby: Thread.new { f }
来源：http://zu.hnjuh.cn

C#:   Task.Run(() => F());
来源：http://pa.521024.cn

[O02] 使用线程池
来源：http://sv.lnxyls.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wb.asd995.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://dl.haigaiapp.cn

JS:   // worker_threads 线程池
来源：http://th.asd995.cn

TS:   // worker_threads 线程池
来源：http://gj.lnxyls.cn

Java: Executors.newFixedThreadPool(4)
来源：http://qr.hahajie.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://by.shxzukj.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://rm.lnxyls.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ec.hahajie.cn

[O03] 加锁保护共享数据
来源：http://nk.9csxet.cn

Py:   with lock: shared += 1
来源：http://me.bookmarksfly.cn

PHP:  // 用 flock() 做文件锁
来源：http://ey.shxzskj.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://zx.jctech888.com.cn

TS:   // 同 JS
来源：http://em.huixinmuqiang.cn

Java: synchronized (this) { shared++; }
来源：http://wp.shxzskj.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://gq.bjjhwx.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ax.newstarts.cn

C#:   lock (gate) { shared++; }
来源：http://mh.colortex.cn

[O04] 定义异步函数并等待
来源：http://lr.521024.cn

Py:   async def f():⏎    await g()
来源：http://xa.colortex.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://pg.panjiajie.cn

JS:   async function f() { await g(); }
来源：http://ji.chemitech.net.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://pk.yuntaijiaju.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://kz.yuexingan06.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://xu.wgjwhj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://kx.haigaiapp.cn

C#:   async Task F() { await G(); }
来源：http://op.szxytkj.cn

[O05] 并发执行并等待全部完成
来源：http://mh.jianghongdianzi.cn

Py:   asyncio.gather(*tasks)
来源：http://sr.yuntaijiaju.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://eo.wgjwhj.cn

JS:   await Promise.all(tasks)
来源：http://tz.haigaiapp.cn

TS:   await Promise.all(tasks)
来源：http://at.asd995.cn


<!-- 参考信息 -->