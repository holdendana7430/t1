代发 wailian999

L. 网络请求
来源：http://ak.shtwfgs.cn

================================================================================
来源：http://ik.hahajie.cn

[L01] 发送 GET 请求
来源：http://xt.colortex.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ru.haigaiapp.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://kd.jctech888.com.cn

JS:   await fetch(url)
来源：http://ps.shtwfgs.cn

TS:   await fetch(url)
来源：http://zr.muxihuayi.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ms.huanxung.cn

Go:   resp, err := http.Get(url)
来源：http://qa.hnjuh.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://fh.muxihuayi.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://xv.shtwfgs.cn

[L02] 发送 POST JSON
来源：http://lk.lnxyls.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ro.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://da.gzmigu.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://el.lnxyls.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ar.lnxyls.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ou.9csxet.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://di.shtwfgs.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mu.jctech888.com.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ly.yuntaijiaju.cn

[L03] 设置自定义请求头
来源：http://vg.muxihuayi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hr.shtwfgs.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ty.9csxet.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ih.shtwfgs.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jj.muxihuayi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://eb.yuexingan06.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://dp.hnjuh.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://uh.muxihuayi.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mi.panjiajie.cn

[L04] 设置超时
来源：http://ns.jctech888.com.cn

Py:   requests.get(url, timeout=5)
来源：http://hs.nicolike.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://im.521024.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nw.nszjky.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fl.shtwfgs.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://cf.jianghongdianzi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ln.yuexingan06.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://al.shtwfgs.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://pb.panjiajie.cn

[L05] 上传文件（multipart）
来源：http://yd.asd995.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ex.hnjuh.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://yv.9csxet.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://zg.bookmarksfly.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://nb.gzmigu.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://lz.lnxyls.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://jh.hahajie.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://kl.huixinmuqiang.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://lk.szsharing.cn

[L06] 解析响应为 JSON
来源：http://pi.asd995.cn

Py:   resp.json()
来源：http://mb.szsharing.cn

PHP:  json_decode($body, true);
来源：http://rf.huixinmuqiang.cn

JS:   await resp.json()
来源：http://xi.szsharing.cn

TS:   await resp.json()
来源：http://ck.bookmarksfly.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://nf.shxzskj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://oq.jianghongdianzi.cn

Ruby: JSON.parse(resp.body)
来源：http://yy.yuexingan06.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://es.haigaiapp.cn

[L07] 处理 HTTP 状态码
来源：http://hn.szxytkj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mg.colortex.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://sp.yuntaijiaju.cn

JS:   resp.ok;  resp.status
来源：http://ji.shxzskj.cn

TS:   resp.ok;  resp.status
来源：http://we.szsharing.cn

Java: resp.statusCode()
来源：http://fn.jianghongdianzi.cn

Go:   resp.StatusCode
来源：http://mc.newstarts.cn

Ruby: resp.code.to_i
来源：http://zy.521024.cn

C#:   (int)resp.StatusCode
来源：http://ci.asd995.cn

[L08] 并发请求多个地址
来源：http://yw.hahajie.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://sf.gzmigu.cn

PHP:  curl_multi_init() 系列
来源：http://ka.colortex.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ki.yuntaijiaju.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ym.shtwfgs.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://dk.shxzukj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qo.huixinmuqiang.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ya.szsharing.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://bx.nicolike.cn

================================================================================
来源：http://wz.szxytkj.cn

M. 命令行 / 进程 / 环境
来源：http://zb.jctech888.com.cn

================================================================================
来源：http://yz.huanxung.cn

[M01] 读取命令行参数
来源：http://tz.bookmarksfly.cn

Py:   sys.argv[1:]
来源：http://wr.yuntaijiaju.cn

PHP:  $argv;  $argc;
来源：http://ij.haigaiapp.cn

JS:   process.argv.slice(2)
来源：http://bn.panjiajie.cn

TS:   process.argv.slice(2)
来源：http://zs.521024.cn

Java: args 数组（main 方法参数）
来源：http://mu.bookmarksfly.cn

Go:   os.Args[1:]
来源：http://ba.wgjwhj.cn

Ruby: ARGV
来源：http://rb.bjjhwx.cn

C#:   args 数组（Main 方法参数）
来源：http://ax.chemitech.net.cn

[M02] 读取环境变量
来源：http://zj.colortex.cn

Py:   os.environ.get("HOME")
来源：http://ik.szsharing.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://qp.gzmigu.cn

JS:   process.env.HOME
来源：http://li.gzmigu.cn

TS:   process.env.HOME
来源：http://zu.wgjwhj.cn

Java: System.getenv("HOME")
来源：http://jj.nszjky.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://fk.szxytkj.cn

Ruby: ENV["HOME"]
来源：http://rh.szxytkj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mx.huixiangedu.cn

[M03] 执行外部命令
来源：http://wk.colortex.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wl.nszjky.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://yc.hahajie.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://nm.haigaiapp.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://us.shtwfgs.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://yc.huixinmuqiang.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://nt.gzmigu.cn

Ruby: system("ls -l");  `ls -l`
来源：http://pc.newstarts.cn

C#:   Process.Start("ls", "-l");
来源：http://dg.huixinmuqiang.cn

[M04] 获取当前工作目录
来源：http://vw.colortex.cn

Py:   os.getcwd()
来源：http://ou.hnjuh.cn

PHP:  getcwd();
来源：http://og.jctech888.com.cn

JS:   process.cwd()
来源：http://jg.bjjhwx.cn

TS:   process.cwd()
来源：http://lh.bjjhwx.cn

Java: Path.of("").toAbsolutePath()
来源：http://ef.szxytkj.cn

Go:   os.Getwd()
来源：http://om.jctech888.com.cn

Ruby: Dir.pwd
来源：http://cs.hnjuh.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ta.yuntaijiaju.cn

[M05] 设置退出码
来源：http://tf.wgjwhj.cn

Py:   sys.exit(1)
来源：http://mt.nszjky.cn

PHP:  exit(1);
来源：http://nu.colortex.cn

JS:   process.exit(1)
来源：http://yf.gzmigu.cn

TS:   process.exit(1)
来源：http://zl.panjiajie.cn

Java: System.exit(1)
来源：http://fk.asd995.cn

Go:   os.Exit(1)
来源：http://oi.szxytkj.cn

Ruby: exit 1
来源：http://rx.newstarts.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://du.hahajie.cn

[M06] 向标准错误输出
来源：http://qj.newstarts.cn

Py:   print("err", file=sys.stderr)
来源：http://av.nszjky.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://sr.shxzukj.cn

JS:   console.error("err")
来源：http://zs.gzmigu.cn

TS:   console.error("err")
来源：http://nm.jctech888.com.cn

Java: System.err.println("err")
来源：http://ii.nicolike.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://gf.huixiangedu.cn

Ruby: warn "err"
来源：http://yu.gzmigu.cn

C#:   Console.Error.WriteLine("err")
来源：http://cg.nicolike.cn

[M07] 判断是否为主入口
来源：http://cn.asd995.cn

Py:   if __name__ == "__main__":
来源：http://fd.szxytkj.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://pj.jianghongdianzi.cn

JS:   require.main === module
来源：http://kq.gzmigu.cn

TS:   require.main === module
来源：http://dp.shtwfgs.cn

Java: public static void main(String[] args)
来源：http://nd.hahajie.cn

Go:   func main()
来源：http://ja.shxzskj.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://uv.shxzskj.cn

C#:   static void Main(string[] args)
来源：http://wu.huixiangedu.cn

[M08] 获取系统与运行时信息
来源：http://th.nicolike.cn

Py:   platform.system();  platform.python_version()
来源：http://zj.yuexingan06.cn

PHP:  PHP_OS;  phpversion();
来源：http://pr.gzmigu.cn

JS:   process.platform;  process.version
来源：http://hh.shtwfgs.cn

TS:   process.platform;  process.version
来源：http://gy.wgjwhj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://fo.shxzukj.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://xw.szxytkj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ju.huanxung.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://hg.bookmarksfly.cn

================================================================================
来源：http://jn.yuexingan06.cn

N. 数据结构与算法
来源：http://ev.colortex.cn

================================================================================
来源：http://da.panjiajie.cn

[N01] 二分查找（有序数组）
来源：http://ru.muxihuayi.cn

Py:   bisect.bisect_left(arr, x)
来源：http://xh.newstarts.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ie.shxzukj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bs.gzmigu.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cb.shtwfgs.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ye.huanxung.cn

Go:   sort.SearchInts(arr, x)
来源：http://gb.huixiangedu.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ms.nszjky.cn

C#:   Array.BinarySearch(arr, x)
来源：http://nx.muxihuayi.cn

[N02] 排序（工程实践用内置实现）
来源：http://bb.shtwfgs.cn

Py:   sorted(arr);  arr.sort()
来源：http://zu.muxihuayi.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://zj.hnjuh.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://tu.lnxyls.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://cn.chemitech.net.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ui.jctech888.com.cn

Go:   slices.Sort(arr)
来源：http://ol.hahajie.cn

Ruby: arr.sort
来源：http://ew.hahajie.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://fo.shxzskj.cn

[N03] 快速排序（分治示例）
来源：http://mv.lnxyls.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://pn.huixinmuqiang.cn

PHP:  // 递归实现，或用 usort
来源：http://ea.shxzukj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nf.huixinmuqiang.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bi.shtwfgs.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://xp.hahajie.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://bl.asd995.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://sn.huixinmuqiang.cn

C#:   // 手写递归，或 Array.Sort
来源：http://gq.bjjhwx.cn

[N04] 斐波那契数列
来源：http://wa.yuntaijiaju.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zv.shxzskj.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ls.colortex.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://br.huixiangedu.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wg.huanxung.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://uh.bookmarksfly.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://oj.521024.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ts.chemitech.net.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://id.bookmarksfly.cn

[N05] 最大公约数
来源：http://cg.bookmarksfly.cn

Py:   math.gcd(a, b)
来源：http://ih.asd995.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ux.shxzukj.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://si.szsharing.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ik.huixinmuqiang.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://jl.lnxyls.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://dz.nszjky.cn

Ruby: a.gcd(b)
来源：http://xy.shxzukj.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://zo.521024.cn

[N06] 判断回文字符串
来源：http://ry.wgjwhj.cn

Py:   s == s[::-1]
来源：http://wt.szsharing.cn

PHP:  $s === strrev($s);
来源：http://gh.jctech888.com.cn

JS:   s === [...s].reverse().join("")
来源：http://nv.jctech888.com.cn

TS:   s === [...s].reverse().join("")
来源：http://dp.haigaiapp.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ni.chemitech.net.cn

Go:   // 双指针从两端比较
来源：http://dt.gzmigu.cn

Ruby: s == s.reverse
来源：http://il.wgjwhj.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://iy.shxzskj.cn

[N07] 两数之和（返回下标）
来源：http://qt.chemitech.net.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://zw.chemitech.net.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://gh.huanxung.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ah.szsharing.cn

TS:   // 手写 Map<string, number>
来源：http://xe.bjjhwx.cn

Java: // 手写 HashMap
来源：http://nj.shtwfgs.cn

Go:   // 手写 map[int]int
来源：http://oz.521024.cn

Ruby: // 手写 Hash
来源：http://vk.asd995.cn

C#:   // 手写 Dictionary<int, int>
来源：http://tp.newstarts.cn

[N08] 生成全排列
来源：http://dp.shxzskj.cn

Py:   itertools.permutations(arr)
来源：http://ws.yuntaijiaju.cn

PHP:  // 手写递归交换
来源：http://ko.wgjwhj.cn

JS:   // 手写回溯递归
来源：http://oj.shxzukj.cn

TS:   // 手写回溯递归
来源：http://hs.hahajie.cn

Java: // 手写回溯递归
来源：http://ig.asd995.cn

Go:   // 手写回溯递归
来源：http://bz.wgjwhj.cn

Ruby: arr.permutation.to_a
来源：http://pu.panjiajie.cn

C#:   // 手写回溯递归
来源：http://bg.bjjhwx.cn

[N09] 栈与队列
来源：http://mo.shtwfgs.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://sy.asd995.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://tj.bjjhwx.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://oy.huixiangedu.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://zd.szsharing.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://sr.lnxyls.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ec.gzmigu.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://yl.bjjhwx.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://st.jianghongdianzi.cn

[N10] 链表节点定义
来源：http://eb.newstarts.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://rc.jctech888.com.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://hm.asd995.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://dy.jianghongdianzi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://eo.yuntaijiaju.cn

Java: class Node { int v; Node next; }
来源：http://ws.szxytkj.cn

Go:   type Node struct { V int; Next *Node }
来源：http://iv.panjiajie.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://yc.jianghongdianzi.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://kg.gzmigu.cn

[N11] 二叉树中序遍历
来源：http://pk.newstarts.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://km.jctech888.com.cn

PHP:  // 手写递归函数
来源：http://js.colortex.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zz.chemitech.net.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dm.9csxet.cn

Java: // 手写递归
来源：http://lz.szsharing.cn

Go:   // 手写递归
来源：http://yl.gzmigu.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://zf.newstarts.cn

C#:   // 手写递归
来源：http://nj.szxytkj.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://is.newstarts.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://by.nszjky.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://uh.chemitech.net.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ys.nszjky.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nx.jianghongdianzi.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://eu.haigaiapp.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://gj.shxzskj.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://gk.9csxet.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://dp.chemitech.net.cn

================================================================================
来源：http://ns.bjjhwx.cn

O. 并发与异步
来源：http://ac.szsharing.cn

================================================================================
来源：http://hz.nicolike.cn

[O01] 启动一个线程
来源：http://ox.hahajie.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ia.jianghongdianzi.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://xl.bookmarksfly.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://gw.huixiangedu.cn

TS:   // 同 JS
来源：http://ck.lnxyls.cn

Java: new Thread(() -> f()).start()
来源：http://kw.huixiangedu.cn

Go:   go f()
来源：http://lt.jctech888.com.cn

Ruby: Thread.new { f }
来源：http://qp.szxytkj.cn

C#:   Task.Run(() => F());
来源：http://lw.huixinmuqiang.cn

[O02] 使用线程池
来源：http://pl.huanxung.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://vq.haigaiapp.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://gp.yuexingan06.cn

JS:   // worker_threads 线程池
来源：http://nf.huanxung.cn

TS:   // worker_threads 线程池
来源：http://cz.szxytkj.cn

Java: Executors.newFixedThreadPool(4)
来源：http://nz.asd995.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://of.muxihuayi.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://zp.shtwfgs.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://xf.bjjhwx.cn

[O03] 加锁保护共享数据
来源：http://nd.yuntaijiaju.cn

Py:   with lock: shared += 1
来源：http://fj.huanxung.cn

PHP:  // 用 flock() 做文件锁
来源：http://sr.colortex.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://pr.muxihuayi.cn

TS:   // 同 JS
来源：http://gj.asd995.cn

Java: synchronized (this) { shared++; }
来源：http://cq.huixiangedu.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://vn.yuexingan06.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://kd.yuexingan06.cn

C#:   lock (gate) { shared++; }
来源：http://vc.szxytkj.cn

[O04] 定义异步函数并等待
来源：http://qn.9csxet.cn

Py:   async def f():⏎    await g()
来源：http://nq.hahajie.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wa.nszjky.cn

JS:   async function f() { await g(); }
来源：http://qe.yuexingan06.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://dt.hahajie.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://na.hahajie.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://bf.wgjwhj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://wy.yuntaijiaju.cn

C#:   async Task F() { await G(); }
来源：http://sd.wgjwhj.cn

[O05] 并发执行并等待全部完成
来源：http://qu.yuntaijiaju.cn


<!-- 参考信息 -->