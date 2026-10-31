代发 wailian999

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://as.muxihuayi.cn

JS:   await fetch(url)
来源：http://ie.hahajie.cn

TS:   await fetch(url)
来源：http://wm.chemitech.net.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://xi.chemitech.net.cn

Go:   resp, err := http.Get(url)
来源：http://fc.szsharing.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://nx.chemitech.net.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://lm.huanxung.cn

[L02] 发送 POST JSON
来源：http://pl.haigaiapp.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ok.hnjuh.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://be.shtwfgs.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gm.szxytkj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://no.muxihuayi.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://lb.chemitech.net.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://bg.gzmigu.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://vf.bookmarksfly.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://kl.9csxet.cn

[L03] 设置自定义请求头
来源：http://pc.colortex.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://cw.szxytkj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://rx.lnxyls.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ya.gzmigu.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ui.haigaiapp.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://th.shxzskj.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://lm.nszjky.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://vh.bjjhwx.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://zl.jianghongdianzi.cn

[L04] 设置超时
来源：http://zv.shxzskj.cn

Py:   requests.get(url, timeout=5)
来源：http://vx.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://px.shtwfgs.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wi.yuntaijiaju.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kq.haigaiapp.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mt.9csxet.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ok.haigaiapp.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://cw.hahajie.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://nn.asd995.cn

[L05] 上传文件（multipart）
来源：http://yk.nicolike.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://qh.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://or.panjiajie.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://zt.nszjky.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://fx.szsharing.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hb.lnxyls.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://rg.hahajie.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://tg.haigaiapp.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ww.haigaiapp.cn

[L06] 解析响应为 JSON
来源：http://ex.hnjuh.cn

Py:   resp.json()
来源：http://gb.asd995.cn

PHP:  json_decode($body, true);
来源：http://hh.asd995.cn

JS:   await resp.json()
来源：http://cn.gzmigu.cn

TS:   await resp.json()
来源：http://xg.panjiajie.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://qk.yuexingan06.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://xv.muxihuayi.cn

Ruby: JSON.parse(resp.body)
来源：http://js.panjiajie.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://re.hnjuh.cn

[L07] 处理 HTTP 状态码
来源：http://yt.asd995.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://cd.panjiajie.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ct.chemitech.net.cn

JS:   resp.ok;  resp.status
来源：http://ez.521024.cn

TS:   resp.ok;  resp.status
来源：http://co.huanxung.cn

Java: resp.statusCode()
来源：http://ti.haigaiapp.cn

Go:   resp.StatusCode
来源：http://tx.jianghongdianzi.cn

Ruby: resp.code.to_i
来源：http://nf.yuntaijiaju.cn

C#:   (int)resp.StatusCode
来源：http://ml.szxytkj.cn

[L08] 并发请求多个地址
来源：http://ul.nicolike.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ce.yuntaijiaju.cn

PHP:  curl_multi_init() 系列
来源：http://ht.shxzukj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vj.szsharing.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ao.shtwfgs.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://lp.szsharing.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ua.haigaiapp.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://yc.colortex.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://he.gzmigu.cn

================================================================================
来源：http://qo.nicolike.cn

M. 命令行 / 进程 / 环境
来源：http://vq.muxihuayi.cn

================================================================================
来源：http://js.nicolike.cn

[M01] 读取命令行参数
来源：http://tn.szxytkj.cn

Py:   sys.argv[1:]
来源：http://bu.newstarts.cn

PHP:  $argv;  $argc;
来源：http://an.shxzskj.cn

JS:   process.argv.slice(2)
来源：http://qm.hahajie.cn

TS:   process.argv.slice(2)
来源：http://ea.huixiangedu.cn

Java: args 数组（main 方法参数）
来源：http://xz.newstarts.cn

Go:   os.Args[1:]
来源：http://dn.bookmarksfly.cn

Ruby: ARGV
来源：http://oh.muxihuayi.cn

C#:   args 数组（Main 方法参数）
来源：http://gh.521024.cn

[M02] 读取环境变量
来源：http://jo.wgjwhj.cn

Py:   os.environ.get("HOME")
来源：http://pt.521024.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hc.nszjky.cn

JS:   process.env.HOME
来源：http://fo.bookmarksfly.cn

TS:   process.env.HOME
来源：http://im.shtwfgs.cn

Java: System.getenv("HOME")
来源：http://ml.yuexingan06.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://cx.yuntaijiaju.cn

Ruby: ENV["HOME"]
来源：http://kj.521024.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ls.shxzukj.cn

[M03] 执行外部命令
来源：http://ro.nszjky.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://od.shxzskj.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://sw.muxihuayi.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://dj.bookmarksfly.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://dr.huanxung.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mp.asd995.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://oj.9csxet.cn

Ruby: system("ls -l");  `ls -l`
来源：http://gn.newstarts.cn

C#:   Process.Start("ls", "-l");
来源：http://po.shxzukj.cn

[M04] 获取当前工作目录
来源：http://tf.bjjhwx.cn

Py:   os.getcwd()
来源：http://fx.lnxyls.cn

PHP:  getcwd();
来源：http://qv.huixinmuqiang.cn

JS:   process.cwd()
来源：http://to.521024.cn

TS:   process.cwd()
来源：http://wg.szxytkj.cn

Java: Path.of("").toAbsolutePath()
来源：http://mv.huanxung.cn

Go:   os.Getwd()
来源：http://mg.haigaiapp.cn

Ruby: Dir.pwd
来源：http://du.shxzskj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://iq.szxytkj.cn

[M05] 设置退出码
来源：http://qc.jianghongdianzi.cn

Py:   sys.exit(1)
来源：http://ol.shtwfgs.cn

PHP:  exit(1);
来源：http://fc.panjiajie.cn

JS:   process.exit(1)
来源：http://xq.lnxyls.cn

TS:   process.exit(1)
来源：http://xv.asd995.cn

Java: System.exit(1)
来源：http://ld.wgjwhj.cn

Go:   os.Exit(1)
来源：http://pz.szxytkj.cn

Ruby: exit 1
来源：http://rp.hnjuh.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://fa.shtwfgs.cn

[M06] 向标准错误输出
来源：http://xn.colortex.cn

Py:   print("err", file=sys.stderr)
来源：http://iv.newstarts.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ko.jctech888.com.cn

JS:   console.error("err")
来源：http://in.9csxet.cn

TS:   console.error("err")
来源：http://sr.asd995.cn

Java: System.err.println("err")
来源：http://sv.jianghongdianzi.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://rm.panjiajie.cn

Ruby: warn "err"
来源：http://th.chemitech.net.cn

C#:   Console.Error.WriteLine("err")
来源：http://hy.newstarts.cn

[M07] 判断是否为主入口
来源：http://ul.szsharing.cn

Py:   if __name__ == "__main__":
来源：http://ib.hnjuh.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://qn.bjjhwx.cn

JS:   require.main === module
来源：http://su.shtwfgs.cn

TS:   require.main === module
来源：http://fp.bjjhwx.cn

Java: public static void main(String[] args)
来源：http://ul.huanxung.cn

Go:   func main()
来源：http://vx.yuexingan06.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://lq.gzmigu.cn

C#:   static void Main(string[] args)
来源：http://sv.nszjky.cn

[M08] 获取系统与运行时信息
来源：http://mk.hnjuh.cn

Py:   platform.system();  platform.python_version()
来源：http://cy.szsharing.cn

PHP:  PHP_OS;  phpversion();
来源：http://sf.yuntaijiaju.cn

JS:   process.platform;  process.version
来源：http://xt.9csxet.cn

TS:   process.platform;  process.version
来源：http://me.hahajie.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://zo.gzmigu.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://js.bjjhwx.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://br.shtwfgs.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://fu.bookmarksfly.cn

================================================================================
来源：http://tg.muxihuayi.cn

N. 数据结构与算法
来源：http://tu.bjjhwx.cn

================================================================================
来源：http://dh.hahajie.cn

[N01] 二分查找（有序数组）
来源：http://ie.haigaiapp.cn

Py:   bisect.bisect_left(arr, x)
来源：http://fm.hnjuh.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://lq.colortex.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://uf.szxytkj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ta.yuntaijiaju.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ul.shxzskj.cn

Go:   sort.SearchInts(arr, x)
来源：http://lq.521024.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://vr.newstarts.cn

C#:   Array.BinarySearch(arr, x)
来源：http://gn.colortex.cn

[N02] 排序（工程实践用内置实现）
来源：http://sb.huixiangedu.cn

Py:   sorted(arr);  arr.sort()
来源：http://jx.shxzukj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://gk.nicolike.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://zr.szxytkj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://xc.521024.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://la.lnxyls.cn

Go:   slices.Sort(arr)
来源：http://xz.shxzskj.cn

Ruby: arr.sort
来源：http://ws.gzmigu.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://uw.lnxyls.cn

[N03] 快速排序（分治示例）
来源：http://lq.haigaiapp.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://tp.gzmigu.cn

PHP:  // 递归实现，或用 usort
来源：http://qm.shtwfgs.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sf.nicolike.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pu.chemitech.net.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ba.asd995.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ti.chemitech.net.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://if.nszjky.cn

C#:   // 手写递归，或 Array.Sort
来源：http://td.wgjwhj.cn

[N04] 斐波那契数列
来源：http://rd.asd995.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://yn.shxzukj.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://is.yuexingan06.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tj.jctech888.com.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fw.huixinmuqiang.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://cs.szsharing.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ps.gzmigu.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://uh.bookmarksfly.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://nx.huanxung.cn

[N05] 最大公约数
来源：http://am.bookmarksfly.cn

Py:   math.gcd(a, b)
来源：http://cn.huanxung.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ms.nszjky.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zy.chemitech.net.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pn.colortex.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://kn.yuntaijiaju.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://dp.521024.cn

Ruby: a.gcd(b)
来源：http://ia.nszjky.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ur.chemitech.net.cn

[N06] 判断回文字符串
来源：http://bh.huixiangedu.cn

Py:   s == s[::-1]
来源：http://qi.yuexingan06.cn

PHP:  $s === strrev($s);
来源：http://st.huixiangedu.cn

JS:   s === [...s].reverse().join("")
来源：http://cj.jianghongdianzi.cn

TS:   s === [...s].reverse().join("")
来源：http://pz.jctech888.com.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://at.shxzukj.cn

Go:   // 双指针从两端比较
来源：http://kw.jctech888.com.cn

Ruby: s == s.reverse
来源：http://tl.gzmigu.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://tx.huixiangedu.cn

[N07] 两数之和（返回下标）
来源：http://ue.hnjuh.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hd.shxzukj.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://lo.haigaiapp.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://cc.lnxyls.cn

TS:   // 手写 Map<string, number>
来源：http://jm.jianghongdianzi.cn

Java: // 手写 HashMap
来源：http://ae.huixiangedu.cn

Go:   // 手写 map[int]int
来源：http://rs.hnjuh.cn

Ruby: // 手写 Hash
来源：http://th.chemitech.net.cn

C#:   // 手写 Dictionary<int, int>
来源：http://nk.yuexingan06.cn

[N08] 生成全排列
来源：http://eg.9csxet.cn

Py:   itertools.permutations(arr)
来源：http://yn.bookmarksfly.cn

PHP:  // 手写递归交换
来源：http://ta.hahajie.cn

JS:   // 手写回溯递归
来源：http://ry.muxihuayi.cn

TS:   // 手写回溯递归
来源：http://sy.jctech888.com.cn

Java: // 手写回溯递归
来源：http://ws.shxzukj.cn

Go:   // 手写回溯递归
来源：http://km.jctech888.com.cn

Ruby: arr.permutation.to_a
来源：http://vs.nicolike.cn

C#:   // 手写回溯递归
来源：http://rq.yuntaijiaju.cn

[N09] 栈与队列
来源：http://yr.yuexingan06.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hq.gzmigu.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://sj.chemitech.net.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ps.newstarts.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://jh.lnxyls.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mf.szsharing.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://uw.szsharing.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ah.huixiangedu.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wl.yuexingan06.cn

[N10] 链表节点定义
来源：http://mn.bookmarksfly.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://jb.nicolike.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://wz.yuexingan06.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ft.lnxyls.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://so.huixinmuqiang.cn

Java: class Node { int v; Node next; }
来源：http://ko.colortex.cn

Go:   type Node struct { V int; Next *Node }
来源：http://wt.nszjky.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://wp.bjjhwx.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://kb.bjjhwx.cn

[N11] 二叉树中序遍历
来源：http://fa.colortex.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ti.huixinmuqiang.cn

PHP:  // 手写递归函数
来源：http://qz.9csxet.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jg.hahajie.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rf.gzmigu.cn

Java: // 手写递归
来源：http://kv.haigaiapp.cn

Go:   // 手写递归
来源：http://zj.newstarts.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ta.newstarts.cn

C#:   // 手写递归
来源：http://ov.muxihuayi.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://qi.chemitech.net.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://lq.muxihuayi.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://iy.hnjuh.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gy.wgjwhj.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fx.jctech888.com.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://dk.asd995.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://tu.shxzukj.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ns.jctech888.com.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ol.9csxet.cn

================================================================================
来源：http://pk.lnxyls.cn

O. 并发与异步
来源：http://xs.asd995.cn

================================================================================
来源：http://ep.bookmarksfly.cn

[O01] 启动一个线程
来源：http://vj.9csxet.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ag.szsharing.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://lb.bjjhwx.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://cl.521024.cn

TS:   // 同 JS
来源：http://rf.huanxung.cn

Java: new Thread(() -> f()).start()
来源：http://wt.9csxet.cn

Go:   go f()
来源：http://bd.bookmarksfly.cn

Ruby: Thread.new { f }
来源：http://bu.szxytkj.cn

C#:   Task.Run(() => F());
来源：http://hp.9csxet.cn

[O02] 使用线程池
来源：http://fz.shtwfgs.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://uz.shxzskj.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://lj.jctech888.com.cn

JS:   // worker_threads 线程池
来源：http://ao.nicolike.cn

TS:   // worker_threads 线程池
来源：http://sq.huixinmuqiang.cn

Java: Executors.newFixedThreadPool(4)
来源：http://vo.shtwfgs.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://jz.lnxyls.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://qd.bookmarksfly.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://as.shxzskj.cn

[O03] 加锁保护共享数据
来源：http://ch.521024.cn

Py:   with lock: shared += 1
来源：http://sd.newstarts.cn

PHP:  // 用 flock() 做文件锁
来源：http://zd.yuexingan06.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ld.yuexingan06.cn

TS:   // 同 JS
来源：http://es.gzmigu.cn

Java: synchronized (this) { shared++; }
来源：http://ya.lnxyls.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://tt.huixinmuqiang.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ho.521024.cn

C#:   lock (gate) { shared++; }
来源：http://ng.jctech888.com.cn

[O04] 定义异步函数并等待
来源：http://in.newstarts.cn

Py:   async def f():⏎    await g()
来源：http://ky.bjjhwx.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://rh.shxzskj.cn

JS:   async function f() { await g(); }
来源：http://gb.9csxet.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://xl.lnxyls.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ec.colortex.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://im.jianghongdianzi.cn

Ruby: # 用 Fiber 或 async gem
来源：http://qu.huixiangedu.cn

C#:   async Task F() { await G(); }
来源：http://fv.nszjky.cn

[O05] 并发执行并等待全部完成
来源：http://fl.jctech888.com.cn

Py:   asyncio.gather(*tasks)
来源：http://xz.asd995.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://cm.chemitech.net.cn

JS:   await Promise.all(tasks)
来源：http://qp.hnjuh.cn

TS:   await Promise.all(tasks)
来源：http://rq.521024.cn


<!-- 参考信息 -->