代发 wailian999

Go:   resp, err := http.Get(url)
来源：http://rx.shxzukj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://zr.nicolike.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://qu.newstarts.cn

[L02] 发送 POST JSON
来源：http://la.huanxung.cn

Py:   requests.post(url, json={"a": 1})
来源：http://bm.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://do.panjiajie.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ms.hnjuh.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dl.jianghongdianzi.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ki.jctech888.com.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://fk.muxihuayi.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://pd.bjjhwx.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ez.shxzukj.cn

[L03] 设置自定义请求头
来源：http://ow.huixiangedu.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ef.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://pv.muxihuayi.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qt.panjiajie.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zv.nicolike.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hx.nicolike.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mc.hahajie.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://pe.lnxyls.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://fo.shtwfgs.cn

[L04] 设置超时
来源：http://pw.chemitech.net.cn

Py:   requests.get(url, timeout=5)
来源：http://lf.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mz.hahajie.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bu.bjjhwx.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ef.shtwfgs.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://me.szxytkj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ux.huixinmuqiang.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://gi.muxihuayi.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://rw.panjiajie.cn

[L05] 上传文件（multipart）
来源：http://zj.panjiajie.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mc.haigaiapp.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://cb.panjiajie.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ah.newstarts.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://si.shxzukj.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://fw.shtwfgs.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://js.yuexingan06.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://fm.huanxung.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://at.huanxung.cn

[L06] 解析响应为 JSON
来源：http://ja.shxzukj.cn

Py:   resp.json()
来源：http://zx.szsharing.cn

PHP:  json_decode($body, true);
来源：http://wh.szsharing.cn

JS:   await resp.json()
来源：http://pu.lnxyls.cn

TS:   await resp.json()
来源：http://jy.bookmarksfly.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://lh.lnxyls.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://kp.chemitech.net.cn

Ruby: JSON.parse(resp.body)
来源：http://sr.hahajie.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://gd.shxzskj.cn

[L07] 处理 HTTP 状态码
来源：http://pe.gzmigu.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://xw.lnxyls.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://cb.huanxung.cn

JS:   resp.ok;  resp.status
来源：http://iv.lnxyls.cn

TS:   resp.ok;  resp.status
来源：http://rp.newstarts.cn

Java: resp.statusCode()
来源：http://lt.chemitech.net.cn

Go:   resp.StatusCode
来源：http://ni.chemitech.net.cn

Ruby: resp.code.to_i
来源：http://no.bookmarksfly.cn

C#:   (int)resp.StatusCode
来源：http://ou.panjiajie.cn

[L08] 并发请求多个地址
来源：http://ru.jctech888.com.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://fz.szxytkj.cn

PHP:  curl_multi_init() 系列
来源：http://ky.hnjuh.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ro.shxzskj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yw.bookmarksfly.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://fr.wgjwhj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://vf.huixiangedu.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://cm.shxzukj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xw.haigaiapp.cn

================================================================================
来源：http://ls.chemitech.net.cn

M. 命令行 / 进程 / 环境
来源：http://gi.wgjwhj.cn

================================================================================
来源：http://wp.chemitech.net.cn

[M01] 读取命令行参数
来源：http://sl.chemitech.net.cn

Py:   sys.argv[1:]
来源：http://ew.521024.cn

PHP:  $argv;  $argc;
来源：http://dt.shxzskj.cn

JS:   process.argv.slice(2)
来源：http://if.haigaiapp.cn

TS:   process.argv.slice(2)
来源：http://ka.shtwfgs.cn

Java: args 数组（main 方法参数）
来源：http://qx.newstarts.cn

Go:   os.Args[1:]
来源：http://va.jianghongdianzi.cn

Ruby: ARGV
来源：http://qz.shxzukj.cn

C#:   args 数组（Main 方法参数）
来源：http://pu.shxzskj.cn

[M02] 读取环境变量
来源：http://ow.shxzukj.cn

Py:   os.environ.get("HOME")
来源：http://yn.chemitech.net.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mc.bookmarksfly.cn

JS:   process.env.HOME
来源：http://az.521024.cn

TS:   process.env.HOME
来源：http://lj.szsharing.cn

Java: System.getenv("HOME")
来源：http://pz.wgjwhj.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://he.yuexingan06.cn

Ruby: ENV["HOME"]
来源：http://xk.newstarts.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://cc.shxzskj.cn

[M03] 执行外部命令
来源：http://uy.asd995.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://er.hahajie.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://vh.yuexingan06.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://hs.nszjky.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://io.hahajie.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://jh.shxzskj.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://bk.gzmigu.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ny.wgjwhj.cn

C#:   Process.Start("ls", "-l");
来源：http://km.huixiangedu.cn

[M04] 获取当前工作目录
来源：http://gy.hnjuh.cn

Py:   os.getcwd()
来源：http://yf.hnjuh.cn

PHP:  getcwd();
来源：http://tm.shtwfgs.cn

JS:   process.cwd()
来源：http://mp.panjiajie.cn

TS:   process.cwd()
来源：http://iw.asd995.cn

Java: Path.of("").toAbsolutePath()
来源：http://nj.szxytkj.cn

Go:   os.Getwd()
来源：http://cf.szxytkj.cn

Ruby: Dir.pwd
来源：http://pp.jctech888.com.cn

C#:   Directory.GetCurrentDirectory()
来源：http://hp.hnjuh.cn

[M05] 设置退出码
来源：http://pf.nicolike.cn

Py:   sys.exit(1)
来源：http://ca.chemitech.net.cn

PHP:  exit(1);
来源：http://xz.shxzukj.cn

JS:   process.exit(1)
来源：http://mv.yuexingan06.cn

TS:   process.exit(1)
来源：http://fd.chemitech.net.cn

Java: System.exit(1)
来源：http://yj.colortex.cn

Go:   os.Exit(1)
来源：http://ri.huixinmuqiang.cn

Ruby: exit 1
来源：http://ev.jianghongdianzi.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://qo.haigaiapp.cn

[M06] 向标准错误输出
来源：http://tj.shxzukj.cn

Py:   print("err", file=sys.stderr)
来源：http://tk.panjiajie.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://tg.lnxyls.cn

JS:   console.error("err")
来源：http://nk.yuexingan06.cn

TS:   console.error("err")
来源：http://gu.jctech888.com.cn

Java: System.err.println("err")
来源：http://tg.asd995.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ev.colortex.cn

Ruby: warn "err"
来源：http://yw.shxzskj.cn

C#:   Console.Error.WriteLine("err")
来源：http://wj.gzmigu.cn

[M07] 判断是否为主入口
来源：http://ir.newstarts.cn

Py:   if __name__ == "__main__":
来源：http://ot.hnjuh.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://om.nicolike.cn

JS:   require.main === module
来源：http://ez.szsharing.cn

TS:   require.main === module
来源：http://kr.huanxung.cn

Java: public static void main(String[] args)
来源：http://yd.bjjhwx.cn

Go:   func main()
来源：http://yl.muxihuayi.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://us.huixiangedu.cn

C#:   static void Main(string[] args)
来源：http://ku.huixinmuqiang.cn

[M08] 获取系统与运行时信息
来源：http://vz.panjiajie.cn

Py:   platform.system();  platform.python_version()
来源：http://xj.huixiangedu.cn

PHP:  PHP_OS;  phpversion();
来源：http://tq.panjiajie.cn

JS:   process.platform;  process.version
来源：http://bd.bjjhwx.cn

TS:   process.platform;  process.version
来源：http://kk.shxzukj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://zu.chemitech.net.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://je.hahajie.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://gv.gzmigu.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://fl.shtwfgs.cn

================================================================================
来源：http://zm.wgjwhj.cn

N. 数据结构与算法
来源：http://cw.shxzukj.cn

================================================================================
来源：http://ob.jctech888.com.cn

[N01] 二分查找（有序数组）
来源：http://un.huixiangedu.cn

Py:   bisect.bisect_left(arr, x)
来源：http://nn.muxihuayi.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://qz.9csxet.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jk.bjjhwx.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hg.huanxung.cn

Java: Arrays.binarySearch(arr, x)
来源：http://vn.chemitech.net.cn

Go:   sort.SearchInts(arr, x)
来源：http://ga.hnjuh.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://qh.bjjhwx.cn

C#:   Array.BinarySearch(arr, x)
来源：http://gm.asd995.cn

[N02] 排序（工程实践用内置实现）
来源：http://wr.asd995.cn

Py:   sorted(arr);  arr.sort()
来源：http://en.asd995.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://gx.szxytkj.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://lv.521024.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://hj.jctech888.com.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://tq.nicolike.cn

Go:   slices.Sort(arr)
来源：http://sw.hnjuh.cn

Ruby: arr.sort
来源：http://ry.yuntaijiaju.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://cp.hnjuh.cn

[N03] 快速排序（分治示例）
来源：http://jg.shxzskj.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ry.hahajie.cn

PHP:  // 递归实现，或用 usort
来源：http://gc.newstarts.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wk.yuntaijiaju.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://to.hahajie.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://dv.wgjwhj.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://gh.newstarts.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://cu.shxzukj.cn

C#:   // 手写递归，或 Array.Sort
来源：http://sm.9csxet.cn

[N04] 斐波那契数列
来源：http://sz.shxzskj.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ds.bjjhwx.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://me.chemitech.net.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sz.gzmigu.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jn.haigaiapp.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://lp.jianghongdianzi.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://pn.jianghongdianzi.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ua.bjjhwx.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://fa.shxzskj.cn

[N05] 最大公约数
来源：http://lh.jianghongdianzi.cn

Py:   math.gcd(a, b)
来源：http://ju.gzmigu.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://oh.haigaiapp.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cr.yuexingan06.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qy.wgjwhj.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://md.szxytkj.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://jm.szxytkj.cn

Ruby: a.gcd(b)
来源：http://mq.nszjky.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://at.yuexingan06.cn

[N06] 判断回文字符串
来源：http://ec.muxihuayi.cn

Py:   s == s[::-1]
来源：http://rj.asd995.cn

PHP:  $s === strrev($s);
来源：http://sj.jctech888.com.cn

JS:   s === [...s].reverse().join("")
来源：http://je.muxihuayi.cn

TS:   s === [...s].reverse().join("")
来源：http://qi.yuexingan06.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://yn.jianghongdianzi.cn

Go:   // 双指针从两端比较
来源：http://lv.shxzukj.cn

Ruby: s == s.reverse
来源：http://hy.asd995.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://fh.9csxet.cn

[N07] 两数之和（返回下标）
来源：http://sk.shxzukj.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ov.shxzukj.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jb.hahajie.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://jn.huixinmuqiang.cn

TS:   // 手写 Map<string, number>
来源：http://vx.huanxung.cn

Java: // 手写 HashMap
来源：http://lq.wgjwhj.cn

Go:   // 手写 map[int]int
来源：http://bt.muxihuayi.cn

Ruby: // 手写 Hash
来源：http://ko.bookmarksfly.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ux.yuexingan06.cn

[N08] 生成全排列
来源：http://wf.hnjuh.cn

Py:   itertools.permutations(arr)
来源：http://ok.colortex.cn

PHP:  // 手写递归交换
来源：http://xq.shtwfgs.cn

JS:   // 手写回溯递归
来源：http://tj.asd995.cn

TS:   // 手写回溯递归
来源：http://zi.asd995.cn

Java: // 手写回溯递归
来源：http://pj.bookmarksfly.cn

Go:   // 手写回溯递归
来源：http://ng.huixiangedu.cn

Ruby: arr.permutation.to_a
来源：http://sm.haigaiapp.cn

C#:   // 手写回溯递归
来源：http://jo.muxihuayi.cn

[N09] 栈与队列
来源：http://mo.chemitech.net.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://pb.chemitech.net.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ok.gzmigu.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://iy.yuntaijiaju.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://fw.jctech888.com.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://fp.yuntaijiaju.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://cc.bookmarksfly.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://rm.9csxet.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://jg.asd995.cn

[N10] 链表节点定义
来源：http://rg.asd995.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://pw.newstarts.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://co.bjjhwx.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ex.haigaiapp.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://nq.nicolike.cn

Java: class Node { int v; Node next; }
来源：http://hs.huixinmuqiang.cn

Go:   type Node struct { V int; Next *Node }
来源：http://dt.shxzskj.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://pt.colortex.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://rf.haigaiapp.cn

[N11] 二叉树中序遍历
来源：http://vn.gzmigu.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://il.asd995.cn

PHP:  // 手写递归函数
来源：http://vv.chemitech.net.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jq.bookmarksfly.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fx.muxihuayi.cn

Java: // 手写递归
来源：http://gu.colortex.cn

Go:   // 手写递归
来源：http://vb.asd995.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://zs.chemitech.net.cn

C#:   // 手写递归
来源：http://xg.huanxung.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ug.szsharing.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ll.lnxyls.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mb.wgjwhj.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fh.huixiangedu.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qi.huanxung.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://sl.huixinmuqiang.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://zy.nicolike.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://xl.jctech888.com.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ok.huanxung.cn

================================================================================
来源：http://pv.bjjhwx.cn

O. 并发与异步
来源：http://wj.nszjky.cn

================================================================================
来源：http://jp.chemitech.net.cn

[O01] 启动一个线程
来源：http://na.szxytkj.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ia.yuntaijiaju.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ha.panjiajie.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://vj.colortex.cn

TS:   // 同 JS
来源：http://ep.nicolike.cn

Java: new Thread(() -> f()).start()
来源：http://ia.jctech888.com.cn

Go:   go f()
来源：http://oa.yuntaijiaju.cn

Ruby: Thread.new { f }
来源：http://hr.huixiangedu.cn

C#:   Task.Run(() => F());
来源：http://ed.nszjky.cn

[O02] 使用线程池
来源：http://ym.asd995.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://vg.jianghongdianzi.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://nf.9csxet.cn

JS:   // worker_threads 线程池
来源：http://mj.hnjuh.cn

TS:   // worker_threads 线程池
来源：http://yr.lnxyls.cn

Java: Executors.newFixedThreadPool(4)
来源：http://fo.shtwfgs.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://zg.huixinmuqiang.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://dd.lnxyls.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://es.muxihuayi.cn

[O03] 加锁保护共享数据
来源：http://xw.jctech888.com.cn

Py:   with lock: shared += 1
来源：http://cf.panjiajie.cn

PHP:  // 用 flock() 做文件锁
来源：http://lb.bjjhwx.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://dn.bookmarksfly.cn

TS:   // 同 JS
来源：http://lg.9csxet.cn

Java: synchronized (this) { shared++; }
来源：http://px.jctech888.com.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hw.bjjhwx.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ca.shxzukj.cn

C#:   lock (gate) { shared++; }
来源：http://rq.shtwfgs.cn

[O04] 定义异步函数并等待
来源：http://ex.yuexingan06.cn

Py:   async def f():⏎    await g()
来源：http://xe.szxytkj.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://pk.huanxung.cn

JS:   async function f() { await g(); }
来源：http://cw.shtwfgs.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://cv.9csxet.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ct.huanxung.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://sl.nicolike.cn

Ruby: # 用 Fiber 或 async gem
来源：http://pb.nicolike.cn

C#:   async Task F() { await G(); }
来源：http://lp.colortex.cn

[O05] 并发执行并等待全部完成
来源：http://tm.huanxung.cn

Py:   asyncio.gather(*tasks)
来源：http://wk.wgjwhj.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://sq.colortex.cn

JS:   await Promise.all(tasks)
来源：http://un.szsharing.cn

TS:   await Promise.all(tasks)
来源：http://tf.521024.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://of.jianghongdianzi.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://vz.huanxung.cn

Ruby: threads.map(&:join)
来源：http://ga.shxzukj.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://bi.jctech888.com.cn


<!-- 参考信息 -->