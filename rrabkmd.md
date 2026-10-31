代发 wailian999

L. 网络请求
来源：http://em.szsharing.cn

================================================================================
来源：http://nt.521024.cn

[L01] 发送 GET 请求
来源：http://ms.521024.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://fc.nicolike.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vq.huixiangedu.cn

JS:   await fetch(url)
来源：http://mm.muxihuayi.cn

TS:   await fetch(url)
来源：http://lt.szxytkj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://gh.panjiajie.cn

Go:   resp, err := http.Get(url)
来源：http://us.haigaiapp.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://tb.jctech888.com.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://vi.shtwfgs.cn

[L02] 发送 POST JSON
来源：http://xp.yuexingan06.cn

Py:   requests.post(url, json={"a": 1})
来源：http://oh.yuntaijiaju.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://fe.huixiangedu.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ge.bookmarksfly.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ud.nszjky.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://xp.jctech888.com.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ow.asd995.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ak.muxihuayi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://rr.jctech888.com.cn

[L03] 设置自定义请求头
来源：http://le.gzmigu.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ku.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://qi.hahajie.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fh.bookmarksfly.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://iz.wgjwhj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://kk.lnxyls.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://sw.yuntaijiaju.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ea.haigaiapp.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://cs.asd995.cn

[L04] 设置超时
来源：http://vr.colortex.cn

Py:   requests.get(url, timeout=5)
来源：http://zm.yuntaijiaju.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://su.nszjky.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vt.521024.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fr.wgjwhj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://my.hnjuh.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ns.hahajie.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://co.shxzukj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://xx.newstarts.cn

[L05] 上传文件（multipart）
来源：http://kw.bookmarksfly.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://sm.wgjwhj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://lb.gzmigu.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hu.jianghongdianzi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://nu.huixiangedu.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://qa.bookmarksfly.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://fv.hahajie.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://lg.nszjky.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://nd.szxytkj.cn

[L06] 解析响应为 JSON
来源：http://jl.nicolike.cn

Py:   resp.json()
来源：http://er.yuntaijiaju.cn

PHP:  json_decode($body, true);
来源：http://fg.hnjuh.cn

JS:   await resp.json()
来源：http://ag.yuntaijiaju.cn

TS:   await resp.json()
来源：http://kq.szsharing.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://fb.haigaiapp.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ui.asd995.cn

Ruby: JSON.parse(resp.body)
来源：http://mx.hahajie.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ah.lnxyls.cn

[L07] 处理 HTTP 状态码
来源：http://kj.shxzukj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://fi.shxzukj.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ot.panjiajie.cn

JS:   resp.ok;  resp.status
来源：http://oe.yuexingan06.cn

TS:   resp.ok;  resp.status
来源：http://mk.yuexingan06.cn

Java: resp.statusCode()
来源：http://ms.chemitech.net.cn

Go:   resp.StatusCode
来源：http://wn.huixinmuqiang.cn

Ruby: resp.code.to_i
来源：http://fk.bookmarksfly.cn

C#:   (int)resp.StatusCode
来源：http://we.huanxung.cn

[L08] 并发请求多个地址
来源：http://kz.shxzskj.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://eh.shtwfgs.cn

PHP:  curl_multi_init() 系列
来源：http://vf.bookmarksfly.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rp.bjjhwx.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mm.newstarts.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://zk.yuexingan06.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://uq.asd995.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://au.yuexingan06.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://we.yuntaijiaju.cn

================================================================================
来源：http://nn.hnjuh.cn

M. 命令行 / 进程 / 环境
来源：http://jc.shxzskj.cn

================================================================================
来源：http://kv.chemitech.net.cn

[M01] 读取命令行参数
来源：http://ls.shxzukj.cn

Py:   sys.argv[1:]
来源：http://ms.hahajie.cn

PHP:  $argv;  $argc;
来源：http://tx.yuntaijiaju.cn

JS:   process.argv.slice(2)
来源：http://us.bjjhwx.cn

TS:   process.argv.slice(2)
来源：http://tf.huanxung.cn

Java: args 数组（main 方法参数）
来源：http://mn.szsharing.cn

Go:   os.Args[1:]
来源：http://ay.yuntaijiaju.cn

Ruby: ARGV
来源：http://mq.szxytkj.cn

C#:   args 数组（Main 方法参数）
来源：http://hu.hahajie.cn

[M02] 读取环境变量
来源：http://uj.huixiangedu.cn

Py:   os.environ.get("HOME")
来源：http://gv.wgjwhj.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://cc.hnjuh.cn

JS:   process.env.HOME
来源：http://yn.szxytkj.cn

TS:   process.env.HOME
来源：http://av.yuexingan06.cn

Java: System.getenv("HOME")
来源：http://wb.shxzukj.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://nj.gzmigu.cn

Ruby: ENV["HOME"]
来源：http://bd.9csxet.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ay.jctech888.com.cn

[M03] 执行外部命令
来源：http://we.nszjky.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wm.shxzskj.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ui.jianghongdianzi.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://lj.jianghongdianzi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://fa.gzmigu.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ze.jianghongdianzi.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://wz.lnxyls.cn

Ruby: system("ls -l");  `ls -l`
来源：http://xd.lnxyls.cn

C#:   Process.Start("ls", "-l");
来源：http://vg.jianghongdianzi.cn

[M04] 获取当前工作目录
来源：http://zn.asd995.cn

Py:   os.getcwd()
来源：http://im.521024.cn

PHP:  getcwd();
来源：http://xd.szsharing.cn

JS:   process.cwd()
来源：http://lr.panjiajie.cn

TS:   process.cwd()
来源：http://fc.wgjwhj.cn

Java: Path.of("").toAbsolutePath()
来源：http://ck.huanxung.cn

Go:   os.Getwd()
来源：http://gq.jctech888.com.cn

Ruby: Dir.pwd
来源：http://ck.hnjuh.cn

C#:   Directory.GetCurrentDirectory()
来源：http://js.bookmarksfly.cn

[M05] 设置退出码
来源：http://ic.huanxung.cn

Py:   sys.exit(1)
来源：http://ot.nicolike.cn

PHP:  exit(1);
来源：http://bi.shxzukj.cn

JS:   process.exit(1)
来源：http://kd.yuexingan06.cn

TS:   process.exit(1)
来源：http://if.hnjuh.cn

Java: System.exit(1)
来源：http://fp.shxzukj.cn

Go:   os.Exit(1)
来源：http://wn.nicolike.cn

Ruby: exit 1
来源：http://ot.szsharing.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://gq.jctech888.com.cn

[M06] 向标准错误输出
来源：http://vi.haigaiapp.cn

Py:   print("err", file=sys.stderr)
来源：http://dw.gzmigu.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://nr.9csxet.cn

JS:   console.error("err")
来源：http://fp.colortex.cn

TS:   console.error("err")
来源：http://tk.jianghongdianzi.cn

Java: System.err.println("err")
来源：http://ga.lnxyls.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://oc.yuntaijiaju.cn

Ruby: warn "err"
来源：http://ah.shtwfgs.cn

C#:   Console.Error.WriteLine("err")
来源：http://zl.hahajie.cn

[M07] 判断是否为主入口
来源：http://um.nszjky.cn

Py:   if __name__ == "__main__":
来源：http://gx.lnxyls.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://pi.hnjuh.cn

JS:   require.main === module
来源：http://up.yuexingan06.cn

TS:   require.main === module
来源：http://wi.huixiangedu.cn

Java: public static void main(String[] args)
来源：http://lt.bookmarksfly.cn

Go:   func main()
来源：http://fq.bookmarksfly.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wz.gzmigu.cn

C#:   static void Main(string[] args)
来源：http://hg.yuntaijiaju.cn

[M08] 获取系统与运行时信息
来源：http://fh.521024.cn

Py:   platform.system();  platform.python_version()
来源：http://oq.chemitech.net.cn

PHP:  PHP_OS;  phpversion();
来源：http://so.asd995.cn

JS:   process.platform;  process.version
来源：http://nz.lnxyls.cn

TS:   process.platform;  process.version
来源：http://gi.colortex.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xu.huixiangedu.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://py.521024.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://dr.asd995.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ke.bjjhwx.cn

================================================================================
来源：http://af.nszjky.cn

N. 数据结构与算法
来源：http://tk.newstarts.cn

================================================================================
来源：http://ql.huanxung.cn

[N01] 二分查找（有序数组）
来源：http://dj.shtwfgs.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ol.9csxet.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://bv.nicolike.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ys.shxzukj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dq.panjiajie.cn

Java: Arrays.binarySearch(arr, x)
来源：http://wv.jctech888.com.cn

Go:   sort.SearchInts(arr, x)
来源：http://uj.gzmigu.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://pl.lnxyls.cn

C#:   Array.BinarySearch(arr, x)
来源：http://hs.shxzskj.cn

[N02] 排序（工程实践用内置实现）
来源：http://cl.huixiangedu.cn

Py:   sorted(arr);  arr.sort()
来源：http://ze.shtwfgs.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://nc.hnjuh.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://bw.haigaiapp.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://fb.nszjky.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://sq.jctech888.com.cn

Go:   slices.Sort(arr)
来源：http://vf.haigaiapp.cn

Ruby: arr.sort
来源：http://fg.muxihuayi.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://jk.huanxung.cn

[N03] 快速排序（分治示例）
来源：http://te.muxihuayi.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://dz.muxihuayi.cn

PHP:  // 递归实现，或用 usort
来源：http://ss.chemitech.net.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rk.yuexingan06.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ef.chemitech.net.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://dk.haigaiapp.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://nh.colortex.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://vt.gzmigu.cn

C#:   // 手写递归，或 Array.Sort
来源：http://vf.lnxyls.cn

[N04] 斐波那契数列
来源：http://xh.wgjwhj.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mm.jctech888.com.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wx.panjiajie.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tq.nszjky.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://oq.shxzskj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://dd.hahajie.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://tw.bookmarksfly.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://rb.chemitech.net.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://cs.shxzskj.cn

[N05] 最大公约数
来源：http://qf.szxytkj.cn

Py:   math.gcd(a, b)
来源：http://iw.shxzukj.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://xt.jctech888.com.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ls.shxzskj.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nv.lnxyls.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://nz.newstarts.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ls.shxzskj.cn

Ruby: a.gcd(b)
来源：http://xd.panjiajie.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://tl.szxytkj.cn

[N06] 判断回文字符串
来源：http://nx.jianghongdianzi.cn

Py:   s == s[::-1]
来源：http://og.bookmarksfly.cn

PHP:  $s === strrev($s);
来源：http://zy.bookmarksfly.cn

JS:   s === [...s].reverse().join("")
来源：http://sl.huanxung.cn

TS:   s === [...s].reverse().join("")
来源：http://ga.hnjuh.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://pd.shxzskj.cn

Go:   // 双指针从两端比较
来源：http://ho.jianghongdianzi.cn

Ruby: s == s.reverse
来源：http://jb.szxytkj.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ur.521024.cn

[N07] 两数之和（返回下标）
来源：http://dl.huixinmuqiang.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://kt.huanxung.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wa.colortex.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://jj.colortex.cn

TS:   // 手写 Map<string, number>
来源：http://pr.9csxet.cn

Java: // 手写 HashMap
来源：http://ou.bjjhwx.cn

Go:   // 手写 map[int]int
来源：http://nz.shxzukj.cn

Ruby: // 手写 Hash
来源：http://wi.panjiajie.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ba.asd995.cn

[N08] 生成全排列
来源：http://mb.jctech888.com.cn

Py:   itertools.permutations(arr)
来源：http://ih.szsharing.cn

PHP:  // 手写递归交换
来源：http://qw.huixiangedu.cn

JS:   // 手写回溯递归
来源：http://aq.bookmarksfly.cn

TS:   // 手写回溯递归
来源：http://ga.hahajie.cn

Java: // 手写回溯递归
来源：http://tk.nicolike.cn

Go:   // 手写回溯递归
来源：http://rr.bjjhwx.cn

Ruby: arr.permutation.to_a
来源：http://xj.newstarts.cn

C#:   // 手写回溯递归
来源：http://lg.9csxet.cn

[N09] 栈与队列
来源：http://xq.lnxyls.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hw.szxytkj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://jk.shxzskj.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://og.muxihuayi.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://fl.huixinmuqiang.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ro.huixiangedu.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://xe.szxytkj.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://vs.shxzukj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://fj.shxzskj.cn

[N10] 链表节点定义
来源：http://wx.lnxyls.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ck.shxzskj.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ha.szsharing.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qw.wgjwhj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://nm.jctech888.com.cn

Java: class Node { int v; Node next; }
来源：http://kz.gzmigu.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ja.9csxet.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://fh.szsharing.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://an.jianghongdianzi.cn

[N11] 二叉树中序遍历
来源：http://oa.521024.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://bz.chemitech.net.cn

PHP:  // 手写递归函数
来源：http://zt.shxzukj.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bh.nszjky.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qs.yuexingan06.cn

Java: // 手写递归
来源：http://kf.szsharing.cn

Go:   // 手写递归
来源：http://bs.jctech888.com.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://fp.9csxet.cn

C#:   // 手写递归
来源：http://dk.wgjwhj.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://fb.haigaiapp.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://om.haigaiapp.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://io.jctech888.com.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.szxytkj.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://om.hahajie.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ku.gzmigu.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ni.shxzukj.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://re.szxytkj.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ok.nszjky.cn

================================================================================
来源：http://jy.huixiangedu.cn

O. 并发与异步
来源：http://px.9csxet.cn

================================================================================
来源：http://vc.haigaiapp.cn

[O01] 启动一个线程
来源：http://mt.hahajie.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mw.hahajie.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hs.huanxung.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ix.yuntaijiaju.cn

TS:   // 同 JS
来源：http://fo.nicolike.cn

Java: new Thread(() -> f()).start()
来源：http://ku.jctech888.com.cn

Go:   go f()
来源：http://wy.szsharing.cn

Ruby: Thread.new { f }
来源：http://lm.hnjuh.cn

C#:   Task.Run(() => F());
来源：http://tq.521024.cn

[O02] 使用线程池
来源：http://ny.lnxyls.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://uf.bookmarksfly.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ay.szsharing.cn

JS:   // worker_threads 线程池
来源：http://uz.huanxung.cn

TS:   // worker_threads 线程池
来源：http://nk.nszjky.cn

Java: Executors.newFixedThreadPool(4)
来源：http://sn.hnjuh.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://dy.haigaiapp.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://lo.huixinmuqiang.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://nb.muxihuayi.cn

[O03] 加锁保护共享数据
来源：http://wv.shtwfgs.cn

Py:   with lock: shared += 1
来源：http://ru.gzmigu.cn

PHP:  // 用 flock() 做文件锁
来源：http://ws.huixinmuqiang.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ye.panjiajie.cn

TS:   // 同 JS
来源：http://zl.panjiajie.cn

Java: synchronized (this) { shared++; }
来源：http://gg.shxzskj.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wf.nszjky.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://qj.szxytkj.cn

C#:   lock (gate) { shared++; }
来源：http://wf.newstarts.cn

[O04] 定义异步函数并等待
来源：http://tu.gzmigu.cn

Py:   async def f():⏎    await g()
来源：http://pr.huixiangedu.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://lc.lnxyls.cn

JS:   async function f() { await g(); }
来源：http://pi.shxzskj.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://kt.gzmigu.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ag.jianghongdianzi.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://jc.chemitech.net.cn

Ruby: # 用 Fiber 或 async gem
来源：http://pf.nicolike.cn

C#:   async Task F() { await G(); }
来源：http://cy.jctech888.com.cn

[O05] 并发执行并等待全部完成
来源：http://fa.lnxyls.cn


<!-- 参考信息 -->