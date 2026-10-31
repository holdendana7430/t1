代发 wailian999

L. 网络请求
来源：http://dg.shxzukj.cn

================================================================================
来源：http://rd.huixiangedu.cn

[L01] 发送 GET 请求
来源：http://nb.asd995.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://bk.yuexingan06.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://uf.huixinmuqiang.cn

JS:   await fetch(url)
来源：http://tu.jianghongdianzi.cn

TS:   await fetch(url)
来源：http://kb.hnjuh.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ku.bookmarksfly.cn

Go:   resp, err := http.Get(url)
来源：http://qd.yuexingan06.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://es.szxytkj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hy.szxytkj.cn

[L02] 发送 POST JSON
来源：http://ui.newstarts.cn

Py:   requests.post(url, json={"a": 1})
来源：http://wj.yuntaijiaju.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://az.hnjuh.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://be.shtwfgs.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gx.lnxyls.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ux.colortex.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://sm.bjjhwx.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://yk.gzmigu.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://rw.gzmigu.cn

[L03] 设置自定义请求头
来源：http://wv.shxzskj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://cz.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ih.asd995.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fi.hahajie.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xk.asd995.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ce.chemitech.net.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ak.9csxet.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ic.bookmarksfly.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://dn.nszjky.cn

[L04] 设置超时
来源：http://bw.huixinmuqiang.cn

Py:   requests.get(url, timeout=5)
来源：http://hk.yuntaijiaju.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://fb.bookmarksfly.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jn.bjjhwx.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rf.chemitech.net.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://nn.shtwfgs.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://oo.huixiangedu.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://so.szsharing.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://vx.yuexingan06.cn

[L05] 上传文件（multipart）
来源：http://lu.shxzukj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://fx.gzmigu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://dg.shtwfgs.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://si.yuexingan06.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://fl.haigaiapp.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ff.huixinmuqiang.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://aj.521024.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ij.bookmarksfly.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ys.shtwfgs.cn

[L06] 解析响应为 JSON
来源：http://kh.asd995.cn

Py:   resp.json()
来源：http://pc.bjjhwx.cn

PHP:  json_decode($body, true);
来源：http://qm.bookmarksfly.cn

JS:   await resp.json()
来源：http://ke.shtwfgs.cn

TS:   await resp.json()
来源：http://qo.chemitech.net.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://no.521024.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mr.bookmarksfly.cn

Ruby: JSON.parse(resp.body)
来源：http://ve.newstarts.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ua.hnjuh.cn

[L07] 处理 HTTP 状态码
来源：http://sz.shxzskj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://xr.nszjky.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://aa.huanxung.cn

JS:   resp.ok;  resp.status
来源：http://uy.jianghongdianzi.cn

TS:   resp.ok;  resp.status
来源：http://pd.colortex.cn

Java: resp.statusCode()
来源：http://rl.szsharing.cn

Go:   resp.StatusCode
来源：http://vh.shtwfgs.cn

Ruby: resp.code.to_i
来源：http://yj.panjiajie.cn

C#:   (int)resp.StatusCode
来源：http://xa.newstarts.cn

[L08] 并发请求多个地址
来源：http://zb.huixinmuqiang.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://rt.hnjuh.cn

PHP:  curl_multi_init() 系列
来源：http://xn.nszjky.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gy.nicolike.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zy.colortex.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ak.asd995.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://gq.lnxyls.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://cn.panjiajie.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://my.lnxyls.cn

================================================================================
来源：http://uo.shxzukj.cn

M. 命令行 / 进程 / 环境
来源：http://fz.chemitech.net.cn

================================================================================
来源：http://zz.521024.cn

[M01] 读取命令行参数
来源：http://um.nicolike.cn

Py:   sys.argv[1:]
来源：http://ut.shxzskj.cn

PHP:  $argv;  $argc;
来源：http://ab.shxzskj.cn

JS:   process.argv.slice(2)
来源：http://mh.nicolike.cn

TS:   process.argv.slice(2)
来源：http://nr.hahajie.cn

Java: args 数组（main 方法参数）
来源：http://mt.bjjhwx.cn

Go:   os.Args[1:]
来源：http://fn.nszjky.cn

Ruby: ARGV
来源：http://aq.521024.cn

C#:   args 数组（Main 方法参数）
来源：http://ye.nicolike.cn

[M02] 读取环境变量
来源：http://jj.gzmigu.cn

Py:   os.environ.get("HOME")
来源：http://ur.huixiangedu.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ol.hahajie.cn

JS:   process.env.HOME
来源：http://bw.shxzukj.cn

TS:   process.env.HOME
来源：http://ud.colortex.cn

Java: System.getenv("HOME")
来源：http://yd.huanxung.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://dc.yuntaijiaju.cn

Ruby: ENV["HOME"]
来源：http://kq.hnjuh.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://fh.szxytkj.cn

[M03] 执行外部命令
来源：http://gv.lnxyls.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://zh.wgjwhj.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://bd.szsharing.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://oe.521024.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://xi.jctech888.com.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hr.lnxyls.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://zf.bookmarksfly.cn

Ruby: system("ls -l");  `ls -l`
来源：http://tf.shxzukj.cn

C#:   Process.Start("ls", "-l");
来源：http://dn.haigaiapp.cn

[M04] 获取当前工作目录
来源：http://ov.muxihuayi.cn

Py:   os.getcwd()
来源：http://el.9csxet.cn

PHP:  getcwd();
来源：http://zb.huixiangedu.cn

JS:   process.cwd()
来源：http://su.colortex.cn

TS:   process.cwd()
来源：http://tz.hahajie.cn

Java: Path.of("").toAbsolutePath()
来源：http://av.haigaiapp.cn

Go:   os.Getwd()
来源：http://gn.521024.cn

Ruby: Dir.pwd
来源：http://rx.yuexingan06.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ev.wgjwhj.cn

[M05] 设置退出码
来源：http://jv.jianghongdianzi.cn

Py:   sys.exit(1)
来源：http://iw.szsharing.cn

PHP:  exit(1);
来源：http://cr.chemitech.net.cn

JS:   process.exit(1)
来源：http://mi.bookmarksfly.cn

TS:   process.exit(1)
来源：http://wi.yuntaijiaju.cn

Java: System.exit(1)
来源：http://td.huixiangedu.cn

Go:   os.Exit(1)
来源：http://rt.shtwfgs.cn

Ruby: exit 1
来源：http://qg.shxzukj.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://cp.nicolike.cn

[M06] 向标准错误输出
来源：http://wm.hahajie.cn

Py:   print("err", file=sys.stderr)
来源：http://tq.bjjhwx.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://qq.szsharing.cn

JS:   console.error("err")
来源：http://lv.lnxyls.cn

TS:   console.error("err")
来源：http://ql.asd995.cn

Java: System.err.println("err")
来源：http://qx.huanxung.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://sx.huixiangedu.cn

Ruby: warn "err"
来源：http://bi.yuntaijiaju.cn

C#:   Console.Error.WriteLine("err")
来源：http://va.muxihuayi.cn

[M07] 判断是否为主入口
来源：http://fd.hahajie.cn

Py:   if __name__ == "__main__":
来源：http://gj.shxzskj.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://qk.muxihuayi.cn

JS:   require.main === module
来源：http://jh.chemitech.net.cn

TS:   require.main === module
来源：http://jx.jctech888.com.cn

Java: public static void main(String[] args)
来源：http://fn.nicolike.cn

Go:   func main()
来源：http://im.shxzukj.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://yj.521024.cn

C#:   static void Main(string[] args)
来源：http://vq.nszjky.cn

[M08] 获取系统与运行时信息
来源：http://mp.panjiajie.cn

Py:   platform.system();  platform.python_version()
来源：http://fa.bjjhwx.cn

PHP:  PHP_OS;  phpversion();
来源：http://dr.jctech888.com.cn

JS:   process.platform;  process.version
来源：http://ld.bookmarksfly.cn

TS:   process.platform;  process.version
来源：http://sr.panjiajie.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://bu.lnxyls.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ux.szsharing.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ov.bjjhwx.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://nw.haigaiapp.cn

================================================================================
来源：http://ke.yuntaijiaju.cn

N. 数据结构与算法
来源：http://tq.szxytkj.cn

================================================================================
来源：http://et.gzmigu.cn

[N01] 二分查找（有序数组）
来源：http://ek.shxzskj.cn

Py:   bisect.bisect_left(arr, x)
来源：http://bj.nicolike.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://la.muxihuayi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kn.huixiangedu.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yt.huanxung.cn

Java: Arrays.binarySearch(arr, x)
来源：http://mv.jctech888.com.cn

Go:   sort.SearchInts(arr, x)
来源：http://xh.shtwfgs.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://xa.yuexingan06.cn

C#:   Array.BinarySearch(arr, x)
来源：http://oz.gzmigu.cn

[N02] 排序（工程实践用内置实现）
来源：http://bs.newstarts.cn

Py:   sorted(arr);  arr.sort()
来源：http://oj.szsharing.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ij.shxzskj.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ly.muxihuayi.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://jt.panjiajie.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://dt.muxihuayi.cn

Go:   slices.Sort(arr)
来源：http://tl.shxzukj.cn

Ruby: arr.sort
来源：http://jf.nicolike.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://za.shtwfgs.cn

[N03] 快速排序（分治示例）
来源：http://wq.yuntaijiaju.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://gb.hnjuh.cn

PHP:  // 递归实现，或用 usort
来源：http://zl.panjiajie.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zc.huixinmuqiang.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xb.jianghongdianzi.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://gd.521024.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://fi.yuexingan06.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://dv.nicolike.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ej.colortex.cn

[N04] 斐波那契数列
来源：http://wp.shtwfgs.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://fc.yuexingan06.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://yi.nszjky.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xq.yuexingan06.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qb.bjjhwx.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://re.colortex.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://qb.9csxet.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://pg.shtwfgs.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://cq.bjjhwx.cn

[N05] 最大公约数
来源：http://ww.lnxyls.cn

Py:   math.gcd(a, b)
来源：http://eb.nicolike.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://uv.hnjuh.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wr.hnjuh.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ux.bookmarksfly.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://og.muxihuayi.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://zd.huixinmuqiang.cn

Ruby: a.gcd(b)
来源：http://gk.huixiangedu.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://qe.muxihuayi.cn

[N06] 判断回文字符串
来源：http://mk.bookmarksfly.cn

Py:   s == s[::-1]
来源：http://zl.huanxung.cn

PHP:  $s === strrev($s);
来源：http://im.hahajie.cn

JS:   s === [...s].reverse().join("")
来源：http://qp.asd995.cn

TS:   s === [...s].reverse().join("")
来源：http://pg.chemitech.net.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xu.panjiajie.cn

Go:   // 双指针从两端比较
来源：http://nt.huanxung.cn

Ruby: s == s.reverse
来源：http://qb.asd995.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://hs.bookmarksfly.cn

[N07] 两数之和（返回下标）
来源：http://ov.huixiangedu.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ya.bookmarksfly.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ww.bjjhwx.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://uu.hahajie.cn

TS:   // 手写 Map<string, number>
来源：http://ni.lnxyls.cn

Java: // 手写 HashMap
来源：http://lf.gzmigu.cn

Go:   // 手写 map[int]int
来源：http://dn.haigaiapp.cn

Ruby: // 手写 Hash
来源：http://fi.gzmigu.cn

C#:   // 手写 Dictionary<int, int>
来源：http://hc.panjiajie.cn

[N08] 生成全排列
来源：http://mk.shxzukj.cn

Py:   itertools.permutations(arr)
来源：http://op.hahajie.cn

PHP:  // 手写递归交换
来源：http://kh.asd995.cn

JS:   // 手写回溯递归
来源：http://zf.bjjhwx.cn

TS:   // 手写回溯递归
来源：http://yh.szxytkj.cn

Java: // 手写回溯递归
来源：http://dn.hnjuh.cn

Go:   // 手写回溯递归
来源：http://fi.lnxyls.cn

Ruby: arr.permutation.to_a
来源：http://sc.bjjhwx.cn

C#:   // 手写回溯递归
来源：http://ra.panjiajie.cn

[N09] 栈与队列
来源：http://wo.nszjky.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://au.nicolike.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://nt.shxzskj.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://kt.szxytkj.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://pc.nicolike.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://di.shtwfgs.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://qs.hnjuh.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://zk.nicolike.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mm.haigaiapp.cn

[N10] 链表节点定义
来源：http://so.newstarts.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://kx.newstarts.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ha.szsharing.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://xn.huanxung.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ql.yuexingan06.cn

Java: class Node { int v; Node next; }
来源：http://fp.szsharing.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ik.bookmarksfly.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ux.szxytkj.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ep.lnxyls.cn

[N11] 二叉树中序遍历
来源：http://mp.haigaiapp.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ck.hahajie.cn

PHP:  // 手写递归函数
来源：http://oq.yuntaijiaju.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qk.huanxung.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://my.huixiangedu.cn

Java: // 手写递归
来源：http://qp.jianghongdianzi.cn

Go:   // 手写递归
来源：http://ug.newstarts.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://un.haigaiapp.cn

C#:   // 手写递归
来源：http://ku.521024.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://qt.huanxung.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://fp.huixinmuqiang.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://tx.jianghongdianzi.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://il.lnxyls.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qc.huixiangedu.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://tl.szsharing.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://qo.asd995.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wf.huixiangedu.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://me.huixinmuqiang.cn

================================================================================
来源：http://pq.bjjhwx.cn

O. 并发与异步
来源：http://bk.panjiajie.cn

================================================================================
来源：http://qh.jianghongdianzi.cn

[O01] 启动一个线程
来源：http://lw.nicolike.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ms.nicolike.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wq.shxzskj.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ff.wgjwhj.cn

TS:   // 同 JS
来源：http://su.szxytkj.cn

Java: new Thread(() -> f()).start()
来源：http://vu.newstarts.cn

Go:   go f()
来源：http://qi.jctech888.com.cn

Ruby: Thread.new { f }
来源：http://sl.muxihuayi.cn

C#:   Task.Run(() => F());
来源：http://dm.bookmarksfly.cn

[O02] 使用线程池
来源：http://wc.yuntaijiaju.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ng.huixinmuqiang.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://jr.jianghongdianzi.cn

JS:   // worker_threads 线程池
来源：http://pe.yuntaijiaju.cn

TS:   // worker_threads 线程池
来源：http://od.521024.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ki.lnxyls.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://yi.yuntaijiaju.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://qa.colortex.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://lu.huixiangedu.cn

[O03] 加锁保护共享数据
来源：http://bt.szxytkj.cn

Py:   with lock: shared += 1
来源：http://ja.huixinmuqiang.cn

PHP:  // 用 flock() 做文件锁
来源：http://lo.shtwfgs.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://go.haigaiapp.cn

TS:   // 同 JS
来源：http://sz.hahajie.cn

Java: synchronized (this) { shared++; }
来源：http://ph.nszjky.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ne.szxytkj.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://rs.nszjky.cn

C#:   lock (gate) { shared++; }
来源：http://as.muxihuayi.cn

[O04] 定义异步函数并等待
来源：http://ml.nicolike.cn

Py:   async def f():⏎    await g()
来源：http://bl.colortex.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://pv.huixiangedu.cn

JS:   async function f() { await g(); }
来源：http://su.shxzukj.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://aw.muxihuayi.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://sb.colortex.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://yw.chemitech.net.cn

Ruby: # 用 Fiber 或 async gem
来源：http://oy.asd995.cn

C#:   async Task F() { await G(); }
来源：http://ij.chemitech.net.cn

[O05] 并发执行并等待全部完成
来源：http://ni.521024.cn


<!-- 参考信息 -->