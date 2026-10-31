代发 wailian999

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://bs.shxzskj.cn

JS:   await fetch(url)
来源：http://lg.shxzskj.cn

TS:   await fetch(url)
来源：http://dk.lnxyls.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://pm.nszjky.cn

Go:   resp, err := http.Get(url)
来源：http://rq.szxytkj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ix.jianghongdianzi.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://vk.chemitech.net.cn

[L02] 发送 POST JSON
来源：http://rq.shtwfgs.cn

Py:   requests.post(url, json={"a": 1})
来源：http://jp.panjiajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hy.nszjky.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yh.yuexingan06.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wr.newstarts.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://od.nicolike.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://kl.jctech888.com.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://jm.panjiajie.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://qp.panjiajie.cn

[L03] 设置自定义请求头
来源：http://yq.521024.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ut.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://of.shtwfgs.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://te.jctech888.com.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://do.colortex.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://or.shtwfgs.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://lu.bjjhwx.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://en.huixinmuqiang.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://se.szsharing.cn

[L04] 设置超时
来源：http://ds.jctech888.com.cn

Py:   requests.get(url, timeout=5)
来源：http://pw.gzmigu.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://se.bjjhwx.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ka.nicolike.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xn.huixiangedu.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://zp.nicolike.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://nv.wgjwhj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://sj.hnjuh.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ke.huixiangedu.cn

[L05] 上传文件（multipart）
来源：http://dv.bjjhwx.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://vl.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://sk.asd995.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ic.jianghongdianzi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://yx.szsharing.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ji.jianghongdianzi.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://qh.gzmigu.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://gg.panjiajie.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://uv.hnjuh.cn

[L06] 解析响应为 JSON
来源：http://sv.hnjuh.cn

Py:   resp.json()
来源：http://uw.9csxet.cn

PHP:  json_decode($body, true);
来源：http://hn.yuntaijiaju.cn

JS:   await resp.json()
来源：http://hg.szxytkj.cn

TS:   await resp.json()
来源：http://ic.yuexingan06.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://st.chemitech.net.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://cq.bookmarksfly.cn

Ruby: JSON.parse(resp.body)
来源：http://su.jianghongdianzi.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ai.9csxet.cn

[L07] 处理 HTTP 状态码
来源：http://yi.9csxet.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://at.nicolike.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://pf.huixinmuqiang.cn

JS:   resp.ok;  resp.status
来源：http://rl.wgjwhj.cn

TS:   resp.ok;  resp.status
来源：http://rl.haigaiapp.cn

Java: resp.statusCode()
来源：http://eu.hnjuh.cn

Go:   resp.StatusCode
来源：http://ia.hahajie.cn

Ruby: resp.code.to_i
来源：http://em.szsharing.cn

C#:   (int)resp.StatusCode
来源：http://rl.bjjhwx.cn

[L08] 并发请求多个地址
来源：http://sx.huixiangedu.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://cs.9csxet.cn

PHP:  curl_multi_init() 系列
来源：http://wz.yuexingan06.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gp.haigaiapp.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sx.wgjwhj.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://dq.nicolike.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qg.chemitech.net.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ng.yuntaijiaju.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://fi.gzmigu.cn

================================================================================
来源：http://hh.shxzskj.cn

M. 命令行 / 进程 / 环境
来源：http://oy.asd995.cn

================================================================================
来源：http://fc.yuexingan06.cn

[M01] 读取命令行参数
来源：http://ps.9csxet.cn

Py:   sys.argv[1:]
来源：http://rb.yuexingan06.cn

PHP:  $argv;  $argc;
来源：http://ce.haigaiapp.cn

JS:   process.argv.slice(2)
来源：http://wr.asd995.cn

TS:   process.argv.slice(2)
来源：http://ad.szxytkj.cn

Java: args 数组（main 方法参数）
来源：http://lf.jianghongdianzi.cn

Go:   os.Args[1:]
来源：http://rq.nszjky.cn

Ruby: ARGV
来源：http://tj.asd995.cn

C#:   args 数组（Main 方法参数）
来源：http://in.hahajie.cn

[M02] 读取环境变量
来源：http://je.wgjwhj.cn

Py:   os.environ.get("HOME")
来源：http://rz.huixinmuqiang.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://tr.haigaiapp.cn

JS:   process.env.HOME
来源：http://xz.wgjwhj.cn

TS:   process.env.HOME
来源：http://hi.jianghongdianzi.cn

Java: System.getenv("HOME")
来源：http://bh.yuexingan06.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://uw.yuntaijiaju.cn

Ruby: ENV["HOME"]
来源：http://ht.jctech888.com.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://li.521024.cn

[M03] 执行外部命令
来源：http://bh.colortex.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://tv.bookmarksfly.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://jj.9csxet.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://sr.asd995.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://dt.hnjuh.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://tf.jctech888.com.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://eh.lnxyls.cn

Ruby: system("ls -l");  `ls -l`
来源：http://xq.wgjwhj.cn

C#:   Process.Start("ls", "-l");
来源：http://yh.panjiajie.cn

[M04] 获取当前工作目录
来源：http://qv.huixinmuqiang.cn

Py:   os.getcwd()
来源：http://vw.shtwfgs.cn

PHP:  getcwd();
来源：http://sm.haigaiapp.cn

JS:   process.cwd()
来源：http://sh.gzmigu.cn

TS:   process.cwd()
来源：http://xm.yuexingan06.cn

Java: Path.of("").toAbsolutePath()
来源：http://rj.shtwfgs.cn

Go:   os.Getwd()
来源：http://tm.huixiangedu.cn

Ruby: Dir.pwd
来源：http://gn.huixinmuqiang.cn

C#:   Directory.GetCurrentDirectory()
来源：http://rj.muxihuayi.cn

[M05] 设置退出码
来源：http://wj.nicolike.cn

Py:   sys.exit(1)
来源：http://jy.chemitech.net.cn

PHP:  exit(1);
来源：http://zs.lnxyls.cn

JS:   process.exit(1)
来源：http://ok.asd995.cn

TS:   process.exit(1)
来源：http://sz.szxytkj.cn

Java: System.exit(1)
来源：http://go.shxzskj.cn

Go:   os.Exit(1)
来源：http://pj.huixiangedu.cn

Ruby: exit 1
来源：http://rv.colortex.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://qx.bookmarksfly.cn

[M06] 向标准错误输出
来源：http://yg.shxzukj.cn

Py:   print("err", file=sys.stderr)
来源：http://sm.colortex.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://bq.huixinmuqiang.cn

JS:   console.error("err")
来源：http://we.bookmarksfly.cn

TS:   console.error("err")
来源：http://gt.yuntaijiaju.cn

Java: System.err.println("err")
来源：http://at.newstarts.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://za.bookmarksfly.cn

Ruby: warn "err"
来源：http://tm.yuexingan06.cn

C#:   Console.Error.WriteLine("err")
来源：http://su.jctech888.com.cn

[M07] 判断是否为主入口
来源：http://yg.shtwfgs.cn

Py:   if __name__ == "__main__":
来源：http://yw.colortex.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ub.colortex.cn

JS:   require.main === module
来源：http://px.hnjuh.cn

TS:   require.main === module
来源：http://ff.szsharing.cn

Java: public static void main(String[] args)
来源：http://fa.huixinmuqiang.cn

Go:   func main()
来源：http://uz.wgjwhj.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://jh.nszjky.cn

C#:   static void Main(string[] args)
来源：http://wm.lnxyls.cn

[M08] 获取系统与运行时信息
来源：http://lh.gzmigu.cn

Py:   platform.system();  platform.python_version()
来源：http://jh.wgjwhj.cn

PHP:  PHP_OS;  phpversion();
来源：http://aw.jianghongdianzi.cn

JS:   process.platform;  process.version
来源：http://sh.hnjuh.cn

TS:   process.platform;  process.version
来源：http://di.lnxyls.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://rt.chemitech.net.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://hw.hnjuh.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://eg.shxzskj.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://dg.chemitech.net.cn

================================================================================
来源：http://ol.panjiajie.cn

N. 数据结构与算法
来源：http://jy.newstarts.cn

================================================================================
来源：http://fs.asd995.cn

[N01] 二分查找（有序数组）
来源：http://lx.lnxyls.cn

Py:   bisect.bisect_left(arr, x)
来源：http://mb.jianghongdianzi.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://gk.lnxyls.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kr.hnjuh.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://oh.yuntaijiaju.cn

Java: Arrays.binarySearch(arr, x)
来源：http://xi.chemitech.net.cn

Go:   sort.SearchInts(arr, x)
来源：http://tz.nszjky.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://as.nicolike.cn

C#:   Array.BinarySearch(arr, x)
来源：http://jf.szsharing.cn

[N02] 排序（工程实践用内置实现）
来源：http://rp.huixinmuqiang.cn

Py:   sorted(arr);  arr.sort()
来源：http://wl.9csxet.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://gw.muxihuayi.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://lk.asd995.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://tj.jctech888.com.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://jj.shxzukj.cn

Go:   slices.Sort(arr)
来源：http://sq.shxzskj.cn

Ruby: arr.sort
来源：http://kp.wgjwhj.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://wk.wgjwhj.cn

[N03] 快速排序（分治示例）
来源：http://qz.hnjuh.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hq.huixinmuqiang.cn

PHP:  // 递归实现，或用 usort
来源：http://yh.szxytkj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://oi.jctech888.com.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gx.colortex.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://rj.521024.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://em.szsharing.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://jk.bjjhwx.cn

C#:   // 手写递归，或 Array.Sort
来源：http://yg.hahajie.cn

[N04] 斐波那契数列
来源：http://tc.haigaiapp.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://cx.chemitech.net.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ck.panjiajie.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mu.colortex.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ji.panjiajie.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://sx.bookmarksfly.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ck.huixinmuqiang.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://kd.yuntaijiaju.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://we.szxytkj.cn

[N05] 最大公约数
来源：http://vg.bookmarksfly.cn

Py:   math.gcd(a, b)
来源：http://bq.gzmigu.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://zu.nszjky.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ci.shtwfgs.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://an.newstarts.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://dy.bjjhwx.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://gd.521024.cn

Ruby: a.gcd(b)
来源：http://xe.jianghongdianzi.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://vc.9csxet.cn

[N06] 判断回文字符串
来源：http://fl.521024.cn

Py:   s == s[::-1]
来源：http://dr.9csxet.cn

PHP:  $s === strrev($s);
来源：http://bb.9csxet.cn

JS:   s === [...s].reverse().join("")
来源：http://hz.haigaiapp.cn

TS:   s === [...s].reverse().join("")
来源：http://vn.muxihuayi.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://pi.bjjhwx.cn

Go:   // 双指针从两端比较
来源：http://uh.nszjky.cn

Ruby: s == s.reverse
来源：http://cu.jianghongdianzi.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://vz.shxzskj.cn

[N07] 两数之和（返回下标）
来源：http://dm.szxytkj.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://xb.szsharing.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ua.haigaiapp.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://bi.gzmigu.cn

TS:   // 手写 Map<string, number>
来源：http://uh.panjiajie.cn

Java: // 手写 HashMap
来源：http://ir.lnxyls.cn

Go:   // 手写 map[int]int
来源：http://mh.521024.cn

Ruby: // 手写 Hash
来源：http://tq.yuexingan06.cn

C#:   // 手写 Dictionary<int, int>
来源：http://dt.haigaiapp.cn

[N08] 生成全排列
来源：http://xn.shxzskj.cn

Py:   itertools.permutations(arr)
来源：http://mf.nszjky.cn

PHP:  // 手写递归交换
来源：http://um.hnjuh.cn

JS:   // 手写回溯递归
来源：http://bj.jianghongdianzi.cn

TS:   // 手写回溯递归
来源：http://id.yuntaijiaju.cn

Java: // 手写回溯递归
来源：http://yl.yuexingan06.cn

Go:   // 手写回溯递归
来源：http://za.yuexingan06.cn

Ruby: arr.permutation.to_a
来源：http://ti.newstarts.cn

C#:   // 手写回溯递归
来源：http://ca.jctech888.com.cn

[N09] 栈与队列
来源：http://er.bjjhwx.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wa.lnxyls.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://yz.panjiajie.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://it.shxzskj.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://pj.muxihuayi.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ex.bookmarksfly.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://uj.newstarts.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://sj.shxzskj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://gh.bookmarksfly.cn

[N10] 链表节点定义
来源：http://uu.9csxet.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://yf.newstarts.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://tf.lnxyls.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://yg.nszjky.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://oh.yuntaijiaju.cn

Java: class Node { int v; Node next; }
来源：http://kg.newstarts.cn

Go:   type Node struct { V int; Next *Node }
来源：http://vi.chemitech.net.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ke.nicolike.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://vi.huixinmuqiang.cn

[N11] 二叉树中序遍历
来源：http://nj.nicolike.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://rd.yuexingan06.cn

PHP:  // 手写递归函数
来源：http://hg.hahajie.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bj.lnxyls.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dm.shxzukj.cn

Java: // 手写递归
来源：http://fc.newstarts.cn

Go:   // 手写递归
来源：http://mi.jctech888.com.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://md.szxytkj.cn

C#:   // 手写递归
来源：http://sa.szxytkj.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://yc.yuexingan06.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://il.huixiangedu.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://zd.bjjhwx.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bg.jctech888.com.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bv.gzmigu.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wv.shtwfgs.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://oa.shxzukj.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://op.szxytkj.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://zk.bookmarksfly.cn

================================================================================
来源：http://tm.shxzukj.cn

O. 并发与异步
来源：http://fi.nszjky.cn

================================================================================
来源：http://op.nszjky.cn

[O01] 启动一个线程
来源：http://im.jctech888.com.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://fy.newstarts.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://uo.muxihuayi.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wf.shxzukj.cn

TS:   // 同 JS
来源：http://rg.9csxet.cn

Java: new Thread(() -> f()).start()
来源：http://xv.szxytkj.cn

Go:   go f()
来源：http://aq.nszjky.cn

Ruby: Thread.new { f }
来源：http://xl.huanxung.cn

C#:   Task.Run(() => F());
来源：http://ku.muxihuayi.cn

[O02] 使用线程池
来源：http://nb.521024.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ra.wgjwhj.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ex.yuntaijiaju.cn

JS:   // worker_threads 线程池
来源：http://zp.colortex.cn

TS:   // worker_threads 线程池
来源：http://ql.shtwfgs.cn

Java: Executors.newFixedThreadPool(4)
来源：http://rr.haigaiapp.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://yd.szxytkj.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mk.asd995.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://qh.szsharing.cn

[O03] 加锁保护共享数据
来源：http://pg.huixinmuqiang.cn

Py:   with lock: shared += 1
来源：http://jr.panjiajie.cn

PHP:  // 用 flock() 做文件锁
来源：http://ug.shxzskj.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ma.shtwfgs.cn

TS:   // 同 JS
来源：http://uz.bookmarksfly.cn

Java: synchronized (this) { shared++; }
来源：http://dq.yuexingan06.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://do.muxihuayi.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://un.bjjhwx.cn

C#:   lock (gate) { shared++; }
来源：http://nu.shxzskj.cn

[O04] 定义异步函数并等待
来源：http://my.jianghongdianzi.cn

Py:   async def f():⏎    await g()
来源：http://fn.szxytkj.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://il.huanxung.cn

JS:   async function f() { await g(); }
来源：http://bb.hahajie.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://wv.shxzskj.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://fs.521024.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://pv.shtwfgs.cn

Ruby: # 用 Fiber 或 async gem
来源：http://bt.521024.cn

C#:   async Task F() { await G(); }
来源：http://qf.jianghongdianzi.cn

[O05] 并发执行并等待全部完成
来源：http://ml.521024.cn

Py:   asyncio.gather(*tasks)
来源：http://ox.haigaiapp.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://jd.panjiajie.cn

JS:   await Promise.all(tasks)
来源：http://vp.nszjky.cn

TS:   await Promise.all(tasks)
来源：http://wc.521024.cn


<!-- 参考信息 -->