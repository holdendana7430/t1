代发 wailian999

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vj.panjiajie.cn

JS:   await fetch(url)
来源：http://pw.muxihuayi.cn

TS:   await fetch(url)
来源：http://ov.wgjwhj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://gi.nicolike.cn

Go:   resp, err := http.Get(url)
来源：http://xe.hahajie.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ya.shxzskj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ay.newstarts.cn

[L02] 发送 POST JSON
来源：http://us.jianghongdianzi.cn

Py:   requests.post(url, json={"a": 1})
来源：http://nj.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ce.huixinmuqiang.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xn.bookmarksfly.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pr.shxzskj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://op.huixiangedu.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://op.gzmigu.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://gn.haigaiapp.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ou.jianghongdianzi.cn

[L03] 设置自定义请求头
来源：http://hf.panjiajie.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://dn.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://qw.asd995.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mf.szsharing.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gl.9csxet.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hg.panjiajie.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ug.shxzskj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://kb.lnxyls.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://cs.panjiajie.cn

[L04] 设置超时
来源：http://jh.shxzukj.cn

Py:   requests.get(url, timeout=5)
来源：http://wv.panjiajie.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://be.shtwfgs.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ui.jianghongdianzi.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ad.lnxyls.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ib.jctech888.com.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://oo.hnjuh.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://eu.shxzskj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ar.huixiangedu.cn

[L05] 上传文件（multipart）
来源：http://kt.szxytkj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ae.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://qs.yuntaijiaju.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://fm.huixinmuqiang.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://np.wgjwhj.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vq.521024.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://zn.panjiajie.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://cg.bookmarksfly.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://oe.lnxyls.cn

[L06] 解析响应为 JSON
来源：http://ki.huixinmuqiang.cn

Py:   resp.json()
来源：http://xd.nicolike.cn

PHP:  json_decode($body, true);
来源：http://pr.haigaiapp.cn

JS:   await resp.json()
来源：http://je.gzmigu.cn

TS:   await resp.json()
来源：http://nh.huixiangedu.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://zc.shxzskj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://of.9csxet.cn

Ruby: JSON.parse(resp.body)
来源：http://ws.shtwfgs.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://uu.9csxet.cn

[L07] 处理 HTTP 状态码
来源：http://km.hnjuh.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ik.yuexingan06.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hs.panjiajie.cn

JS:   resp.ok;  resp.status
来源：http://qc.hnjuh.cn

TS:   resp.ok;  resp.status
来源：http://ep.asd995.cn

Java: resp.statusCode()
来源：http://jj.shxzukj.cn

Go:   resp.StatusCode
来源：http://to.shtwfgs.cn

Ruby: resp.code.to_i
来源：http://of.521024.cn

C#:   (int)resp.StatusCode
来源：http://wx.nicolike.cn

[L08] 并发请求多个地址
来源：http://xe.huanxung.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://il.haigaiapp.cn

PHP:  curl_multi_init() 系列
来源：http://ds.huixiangedu.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ug.gzmigu.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nf.shtwfgs.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://pk.huixinmuqiang.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://kr.wgjwhj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://di.asd995.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://im.wgjwhj.cn

================================================================================
来源：http://ju.shxzskj.cn

M. 命令行 / 进程 / 环境
来源：http://it.hahajie.cn

================================================================================
来源：http://nx.bjjhwx.cn

[M01] 读取命令行参数
来源：http://ed.huixiangedu.cn

Py:   sys.argv[1:]
来源：http://yv.shxzskj.cn

PHP:  $argv;  $argc;
来源：http://ep.shxzskj.cn

JS:   process.argv.slice(2)
来源：http://dm.yuntaijiaju.cn

TS:   process.argv.slice(2)
来源：http://tj.jianghongdianzi.cn

Java: args 数组（main 方法参数）
来源：http://sf.nszjky.cn

Go:   os.Args[1:]
来源：http://yp.wgjwhj.cn

Ruby: ARGV
来源：http://mk.gzmigu.cn

C#:   args 数组（Main 方法参数）
来源：http://yg.gzmigu.cn

[M02] 读取环境变量
来源：http://ov.newstarts.cn

Py:   os.environ.get("HOME")
来源：http://kr.521024.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zq.bookmarksfly.cn

JS:   process.env.HOME
来源：http://zd.shxzskj.cn

TS:   process.env.HOME
来源：http://jf.lnxyls.cn

Java: System.getenv("HOME")
来源：http://qm.wgjwhj.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://am.hahajie.cn

Ruby: ENV["HOME"]
来源：http://bi.jianghongdianzi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ql.chemitech.net.cn

[M03] 执行外部命令
来源：http://sd.shxzukj.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://my.colortex.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://uf.chemitech.net.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ub.bjjhwx.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://qb.huixiangedu.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://da.hahajie.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://po.yuntaijiaju.cn

Ruby: system("ls -l");  `ls -l`
来源：http://nt.asd995.cn

C#:   Process.Start("ls", "-l");
来源：http://pj.huixinmuqiang.cn

[M04] 获取当前工作目录
来源：http://rd.huixiangedu.cn

Py:   os.getcwd()
来源：http://dy.hahajie.cn

PHP:  getcwd();
来源：http://di.9csxet.cn

JS:   process.cwd()
来源：http://us.newstarts.cn

TS:   process.cwd()
来源：http://if.haigaiapp.cn

Java: Path.of("").toAbsolutePath()
来源：http://sa.hnjuh.cn

Go:   os.Getwd()
来源：http://kr.asd995.cn

Ruby: Dir.pwd
来源：http://cs.haigaiapp.cn

C#:   Directory.GetCurrentDirectory()
来源：http://za.haigaiapp.cn

[M05] 设置退出码
来源：http://vr.chemitech.net.cn

Py:   sys.exit(1)
来源：http://gx.9csxet.cn

PHP:  exit(1);
来源：http://cr.panjiajie.cn

JS:   process.exit(1)
来源：http://au.nicolike.cn

TS:   process.exit(1)
来源：http://ij.muxihuayi.cn

Java: System.exit(1)
来源：http://aq.panjiajie.cn

Go:   os.Exit(1)
来源：http://gr.jctech888.com.cn

Ruby: exit 1
来源：http://at.muxihuayi.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://zl.jianghongdianzi.cn

[M06] 向标准错误输出
来源：http://hr.yuntaijiaju.cn

Py:   print("err", file=sys.stderr)
来源：http://ot.hahajie.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://za.wgjwhj.cn

JS:   console.error("err")
来源：http://dc.huixiangedu.cn

TS:   console.error("err")
来源：http://ni.panjiajie.cn

Java: System.err.println("err")
来源：http://xg.yuexingan06.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ty.521024.cn

Ruby: warn "err"
来源：http://nv.chemitech.net.cn

C#:   Console.Error.WriteLine("err")
来源：http://dc.shxzskj.cn

[M07] 判断是否为主入口
来源：http://nv.gzmigu.cn

Py:   if __name__ == "__main__":
来源：http://qo.colortex.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://qh.huanxung.cn

JS:   require.main === module
来源：http://oe.9csxet.cn

TS:   require.main === module
来源：http://zd.nicolike.cn

Java: public static void main(String[] args)
来源：http://xs.jctech888.com.cn

Go:   func main()
来源：http://pf.chemitech.net.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://qr.shxzukj.cn

C#:   static void Main(string[] args)
来源：http://ws.hnjuh.cn

[M08] 获取系统与运行时信息
来源：http://tm.lnxyls.cn

Py:   platform.system();  platform.python_version()
来源：http://eo.hahajie.cn

PHP:  PHP_OS;  phpversion();
来源：http://zj.jianghongdianzi.cn

JS:   process.platform;  process.version
来源：http://nt.szsharing.cn

TS:   process.platform;  process.version
来源：http://bh.lnxyls.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://nr.colortex.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://yd.muxihuayi.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://vc.yuexingan06.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://yt.hahajie.cn

================================================================================
来源：http://bi.newstarts.cn

N. 数据结构与算法
来源：http://om.nszjky.cn

================================================================================
来源：http://ti.nszjky.cn

[N01] 二分查找（有序数组）
来源：http://mf.hahajie.cn

Py:   bisect.bisect_left(arr, x)
来源：http://hw.haigaiapp.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ri.szsharing.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vi.9csxet.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gs.521024.cn

Java: Arrays.binarySearch(arr, x)
来源：http://oj.jctech888.com.cn

Go:   sort.SearchInts(arr, x)
来源：http://bw.wgjwhj.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://dn.nicolike.cn

C#:   Array.BinarySearch(arr, x)
来源：http://pi.szsharing.cn

[N02] 排序（工程实践用内置实现）
来源：http://ov.haigaiapp.cn

Py:   sorted(arr);  arr.sort()
来源：http://nv.hnjuh.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://en.asd995.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ns.chemitech.net.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ay.shxzskj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://td.9csxet.cn

Go:   slices.Sort(arr)
来源：http://ol.jianghongdianzi.cn

Ruby: arr.sort
来源：http://re.huixinmuqiang.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://wf.yuexingan06.cn

[N03] 快速排序（分治示例）
来源：http://rb.jctech888.com.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://pd.521024.cn

PHP:  // 递归实现，或用 usort
来源：http://ev.yuexingan06.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bu.panjiajie.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fm.bjjhwx.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://tf.huixinmuqiang.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://xd.bjjhwx.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://yk.panjiajie.cn

C#:   // 手写递归，或 Array.Sort
来源：http://jy.wgjwhj.cn

[N04] 斐波那契数列
来源：http://hb.gzmigu.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://gi.yuexingan06.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ze.wgjwhj.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vs.wgjwhj.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qm.shtwfgs.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://tr.asd995.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://gk.jctech888.com.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://nm.9csxet.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://af.nicolike.cn

[N05] 最大公约数
来源：http://fr.szsharing.cn

Py:   math.gcd(a, b)
来源：http://vd.nicolike.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://dk.chemitech.net.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hn.panjiajie.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bi.haigaiapp.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ki.nszjky.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://fb.szsharing.cn

Ruby: a.gcd(b)
来源：http://bo.muxihuayi.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://kb.hnjuh.cn

[N06] 判断回文字符串
来源：http://if.shtwfgs.cn

Py:   s == s[::-1]
来源：http://ar.521024.cn

PHP:  $s === strrev($s);
来源：http://lz.muxihuayi.cn

JS:   s === [...s].reverse().join("")
来源：http://td.shxzskj.cn

TS:   s === [...s].reverse().join("")
来源：http://pb.chemitech.net.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://tk.szsharing.cn

Go:   // 双指针从两端比较
来源：http://ew.gzmigu.cn

Ruby: s == s.reverse
来源：http://dc.shxzukj.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://su.shxzukj.cn

[N07] 两数之和（返回下标）
来源：http://cs.shtwfgs.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://pe.hahajie.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wt.hahajie.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://bc.bjjhwx.cn

TS:   // 手写 Map<string, number>
来源：http://rl.shxzskj.cn

Java: // 手写 HashMap
来源：http://xl.szxytkj.cn

Go:   // 手写 map[int]int
来源：http://rm.shxzskj.cn

Ruby: // 手写 Hash
来源：http://fu.szxytkj.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ve.huanxung.cn

[N08] 生成全排列
来源：http://dw.asd995.cn

Py:   itertools.permutations(arr)
来源：http://kz.chemitech.net.cn

PHP:  // 手写递归交换
来源：http://ig.bjjhwx.cn

JS:   // 手写回溯递归
来源：http://zc.521024.cn

TS:   // 手写回溯递归
来源：http://ja.szsharing.cn

Java: // 手写回溯递归
来源：http://ol.panjiajie.cn

Go:   // 手写回溯递归
来源：http://rd.szsharing.cn

Ruby: arr.permutation.to_a
来源：http://pt.chemitech.net.cn

C#:   // 手写回溯递归
来源：http://zi.hahajie.cn

[N09] 栈与队列
来源：http://bh.huanxung.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ct.colortex.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ob.colortex.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://oz.huixiangedu.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hd.yuexingan06.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://kp.jianghongdianzi.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://tk.asd995.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ni.huixiangedu.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ws.bjjhwx.cn

[N10] 链表节点定义
来源：http://jh.hnjuh.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ea.newstarts.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ey.szsharing.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://zu.szxytkj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://vv.haigaiapp.cn

Java: class Node { int v; Node next; }
来源：http://bg.bjjhwx.cn

Go:   type Node struct { V int; Next *Node }
来源：http://bw.gzmigu.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://hp.asd995.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://nc.9csxet.cn

[N11] 二叉树中序遍历
来源：http://qa.huixinmuqiang.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://vl.nicolike.cn

PHP:  // 手写递归函数
来源：http://mr.shxzukj.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vl.bookmarksfly.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fi.colortex.cn

Java: // 手写递归
来源：http://pm.bjjhwx.cn

Go:   // 手写递归
来源：http://bz.shxzukj.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://vz.shxzukj.cn

C#:   // 手写递归
来源：http://ki.szsharing.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://cj.9csxet.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wl.9csxet.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://sp.szsharing.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xo.9csxet.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mk.huanxung.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://js.asd995.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://dd.shxzskj.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ym.bjjhwx.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://zv.9csxet.cn

================================================================================
来源：http://qo.szsharing.cn

O. 并发与异步
来源：http://le.nszjky.cn

================================================================================
来源：http://kn.jctech888.com.cn

[O01] 启动一个线程
来源：http://oy.chemitech.net.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://fh.yuexingan06.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://dq.chemitech.net.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://oy.gzmigu.cn

TS:   // 同 JS
来源：http://gp.hahajie.cn

Java: new Thread(() -> f()).start()
来源：http://ud.jctech888.com.cn

Go:   go f()
来源：http://gl.nszjky.cn

Ruby: Thread.new { f }
来源：http://ti.lnxyls.cn

C#:   Task.Run(() => F());
来源：http://nr.asd995.cn

[O02] 使用线程池
来源：http://fp.yuntaijiaju.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mu.szsharing.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://xr.jctech888.com.cn

JS:   // worker_threads 线程池
来源：http://wb.huixiangedu.cn

TS:   // worker_threads 线程池
来源：http://rx.haigaiapp.cn

Java: Executors.newFixedThreadPool(4)
来源：http://hb.shtwfgs.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://xv.9csxet.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://oo.colortex.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://vf.yuntaijiaju.cn

[O03] 加锁保护共享数据
来源：http://ix.huixinmuqiang.cn

Py:   with lock: shared += 1
来源：http://ew.szxytkj.cn

PHP:  // 用 flock() 做文件锁
来源：http://cc.yuntaijiaju.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://pf.chemitech.net.cn

TS:   // 同 JS
来源：http://je.szsharing.cn

Java: synchronized (this) { shared++; }
来源：http://ti.panjiajie.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://sx.gzmigu.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ms.huixiangedu.cn

C#:   lock (gate) { shared++; }
来源：http://sw.yuexingan06.cn

[O04] 定义异步函数并等待
来源：http://nw.shtwfgs.cn

Py:   async def f():⏎    await g()
来源：http://nf.asd995.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://jd.szxytkj.cn

JS:   async function f() { await g(); }
来源：http://bh.gzmigu.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://xo.9csxet.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://vp.huixiangedu.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://fd.panjiajie.cn

Ruby: # 用 Fiber 或 async gem
来源：http://mq.bookmarksfly.cn

C#:   async Task F() { await G(); }
来源：http://ng.newstarts.cn

[O05] 并发执行并等待全部完成
来源：http://yi.muxihuayi.cn

Py:   asyncio.gather(*tasks)
来源：http://iq.bjjhwx.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ti.newstarts.cn

JS:   await Promise.all(tasks)
来源：http://ix.nicolike.cn

TS:   await Promise.all(tasks)
来源：http://fs.shxzukj.cn


<!-- 参考信息 -->