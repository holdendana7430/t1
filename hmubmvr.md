代发 wailian999

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ma.szsharing.cn

JS:   await fetch(url)
来源：http://pu.asd995.cn

TS:   await fetch(url)
来源：http://kz.nszjky.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://au.szxytkj.cn

Go:   resp, err := http.Get(url)
来源：http://nl.hahajie.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://bh.chemitech.net.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://qo.hahajie.cn

[L02] 发送 POST JSON
来源：http://oq.newstarts.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ym.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://yc.muxihuayi.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zs.wgjwhj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://uk.shtwfgs.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://rv.asd995.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://tz.jianghongdianzi.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://zi.yuntaijiaju.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://nc.nicolike.cn

[L03] 设置自定义请求头
来源：http://oa.haigaiapp.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ed.haigaiapp.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://no.nszjky.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jo.newstarts.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ug.shxzskj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ln.nszjky.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://of.bookmarksfly.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ey.panjiajie.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ib.muxihuayi.cn

[L04] 设置超时
来源：http://ri.szsharing.cn

Py:   requests.get(url, timeout=5)
来源：http://pe.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ia.hahajie.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jd.nszjky.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zd.colortex.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ao.521024.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://vq.shtwfgs.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ky.wgjwhj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://kz.haigaiapp.cn

[L05] 上传文件（multipart）
来源：http://aw.szsharing.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ho.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wr.yuntaijiaju.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://av.panjiajie.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ae.shxzskj.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ql.nicolike.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://vm.asd995.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://kt.hnjuh.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://nb.newstarts.cn

[L06] 解析响应为 JSON
来源：http://ge.szxytkj.cn

Py:   resp.json()
来源：http://ek.shtwfgs.cn

PHP:  json_decode($body, true);
来源：http://fy.huixiangedu.cn

JS:   await resp.json()
来源：http://yr.shxzukj.cn

TS:   await resp.json()
来源：http://nl.asd995.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://nm.shxzukj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://bf.shtwfgs.cn

Ruby: JSON.parse(resp.body)
来源：http://vp.nicolike.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ux.asd995.cn

[L07] 处理 HTTP 状态码
来源：http://af.bjjhwx.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://iv.szxytkj.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://or.shxzukj.cn

JS:   resp.ok;  resp.status
来源：http://lq.szxytkj.cn

TS:   resp.ok;  resp.status
来源：http://ri.yuexingan06.cn

Java: resp.statusCode()
来源：http://rt.huixiangedu.cn

Go:   resp.StatusCode
来源：http://up.hahajie.cn

Ruby: resp.code.to_i
来源：http://gn.hahajie.cn

C#:   (int)resp.StatusCode
来源：http://su.wgjwhj.cn

[L08] 并发请求多个地址
来源：http://ks.shxzskj.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://yk.huixiangedu.cn

PHP:  curl_multi_init() 系列
来源：http://ou.szsharing.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tg.haigaiapp.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://du.chemitech.net.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://uz.colortex.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ev.panjiajie.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://km.huanxung.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://at.wgjwhj.cn

================================================================================
来源：http://bl.nicolike.cn

M. 命令行 / 进程 / 环境
来源：http://fl.hahajie.cn

================================================================================
来源：http://jd.gzmigu.cn

[M01] 读取命令行参数
来源：http://nq.lnxyls.cn

Py:   sys.argv[1:]
来源：http://gu.lnxyls.cn

PHP:  $argv;  $argc;
来源：http://mi.yuntaijiaju.cn

JS:   process.argv.slice(2)
来源：http://iq.nicolike.cn

TS:   process.argv.slice(2)
来源：http://xk.asd995.cn

Java: args 数组（main 方法参数）
来源：http://fb.colortex.cn

Go:   os.Args[1:]
来源：http://hg.huixiangedu.cn

Ruby: ARGV
来源：http://ws.yuexingan06.cn

C#:   args 数组（Main 方法参数）
来源：http://ow.haigaiapp.cn

[M02] 读取环境变量
来源：http://gn.newstarts.cn

Py:   os.environ.get("HOME")
来源：http://hh.lnxyls.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zr.asd995.cn

JS:   process.env.HOME
来源：http://qi.muxihuayi.cn

TS:   process.env.HOME
来源：http://pc.huanxung.cn

Java: System.getenv("HOME")
来源：http://fg.huixiangedu.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://gd.bookmarksfly.cn

Ruby: ENV["HOME"]
来源：http://cs.lnxyls.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://rk.szsharing.cn

[M03] 执行外部命令
来源：http://qo.asd995.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://lt.nicolike.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wd.gzmigu.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://gy.asd995.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://tu.jianghongdianzi.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://dr.huixiangedu.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://nz.huixiangedu.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ot.wgjwhj.cn

C#:   Process.Start("ls", "-l");
来源：http://ks.lnxyls.cn

[M04] 获取当前工作目录
来源：http://ag.chemitech.net.cn

Py:   os.getcwd()
来源：http://ug.panjiajie.cn

PHP:  getcwd();
来源：http://jb.nszjky.cn

JS:   process.cwd()
来源：http://wa.wgjwhj.cn

TS:   process.cwd()
来源：http://cq.jctech888.com.cn

Java: Path.of("").toAbsolutePath()
来源：http://ul.shxzukj.cn

Go:   os.Getwd()
来源：http://pu.muxihuayi.cn

Ruby: Dir.pwd
来源：http://nr.lnxyls.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ub.chemitech.net.cn

[M05] 设置退出码
来源：http://xz.bjjhwx.cn

Py:   sys.exit(1)
来源：http://ra.gzmigu.cn

PHP:  exit(1);
来源：http://hg.huixinmuqiang.cn

JS:   process.exit(1)
来源：http://bx.hahajie.cn

TS:   process.exit(1)
来源：http://gv.yuexingan06.cn

Java: System.exit(1)
来源：http://bv.shxzskj.cn

Go:   os.Exit(1)
来源：http://jj.haigaiapp.cn

Ruby: exit 1
来源：http://ey.panjiajie.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mu.asd995.cn

[M06] 向标准错误输出
来源：http://ok.lnxyls.cn

Py:   print("err", file=sys.stderr)
来源：http://xb.chemitech.net.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://zf.wgjwhj.cn

JS:   console.error("err")
来源：http://cr.lnxyls.cn

TS:   console.error("err")
来源：http://zq.yuntaijiaju.cn

Java: System.err.println("err")
来源：http://co.yuexingan06.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://qc.haigaiapp.cn

Ruby: warn "err"
来源：http://kx.yuntaijiaju.cn

C#:   Console.Error.WriteLine("err")
来源：http://ma.szsharing.cn

[M07] 判断是否为主入口
来源：http://fg.jianghongdianzi.cn

Py:   if __name__ == "__main__":
来源：http://pr.shxzskj.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://fr.wgjwhj.cn

JS:   require.main === module
来源：http://ff.lnxyls.cn

TS:   require.main === module
来源：http://gl.yuexingan06.cn

Java: public static void main(String[] args)
来源：http://zv.szxytkj.cn

Go:   func main()
来源：http://mf.colortex.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mz.nicolike.cn

C#:   static void Main(string[] args)
来源：http://th.nicolike.cn

[M08] 获取系统与运行时信息
来源：http://vb.lnxyls.cn

Py:   platform.system();  platform.python_version()
来源：http://bi.521024.cn

PHP:  PHP_OS;  phpversion();
来源：http://sn.haigaiapp.cn

JS:   process.platform;  process.version
来源：http://sp.huanxung.cn

TS:   process.platform;  process.version
来源：http://vv.yuexingan06.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ns.521024.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ne.yuexingan06.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ym.jianghongdianzi.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ss.muxihuayi.cn

================================================================================
来源：http://cg.szxytkj.cn

N. 数据结构与算法
来源：http://ku.nicolike.cn

================================================================================
来源：http://gg.nicolike.cn

[N01] 二分查找（有序数组）
来源：http://ii.panjiajie.cn

Py:   bisect.bisect_left(arr, x)
来源：http://jk.wgjwhj.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ri.szsharing.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gv.bjjhwx.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ny.muxihuayi.cn

Java: Arrays.binarySearch(arr, x)
来源：http://dk.panjiajie.cn

Go:   sort.SearchInts(arr, x)
来源：http://ko.jctech888.com.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://xp.hahajie.cn

C#:   Array.BinarySearch(arr, x)
来源：http://fr.shxzskj.cn

[N02] 排序（工程实践用内置实现）
来源：http://gg.huixiangedu.cn

Py:   sorted(arr);  arr.sort()
来源：http://va.hnjuh.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://rt.shxzukj.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://yz.szxytkj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://qg.asd995.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wk.yuexingan06.cn

Go:   slices.Sort(arr)
来源：http://nn.521024.cn

Ruby: arr.sort
来源：http://ca.chemitech.net.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://nm.9csxet.cn

[N03] 快速排序（分治示例）
来源：http://eg.haigaiapp.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://yn.lnxyls.cn

PHP:  // 递归实现，或用 usort
来源：http://ha.huixinmuqiang.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lz.shxzukj.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ua.huanxung.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://bm.shtwfgs.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://qn.nicolike.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://te.szxytkj.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ek.9csxet.cn

[N04] 斐波那契数列
来源：http://es.panjiajie.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://dx.colortex.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://cy.521024.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yu.szxytkj.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vr.huixinmuqiang.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hh.panjiajie.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mi.yuexingan06.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wv.newstarts.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://rn.szsharing.cn

[N05] 最大公约数
来源：http://tn.yuexingan06.cn

Py:   math.gcd(a, b)
来源：http://lb.haigaiapp.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://fh.huixinmuqiang.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lo.shxzukj.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fp.nszjky.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://kw.chemitech.net.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://zk.521024.cn

Ruby: a.gcd(b)
来源：http://ho.chemitech.net.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mh.yuexingan06.cn

[N06] 判断回文字符串
来源：http://nu.jianghongdianzi.cn

Py:   s == s[::-1]
来源：http://rr.jctech888.com.cn

PHP:  $s === strrev($s);
来源：http://jc.huixinmuqiang.cn

JS:   s === [...s].reverse().join("")
来源：http://mt.newstarts.cn

TS:   s === [...s].reverse().join("")
来源：http://nn.hnjuh.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://qg.shxzukj.cn

Go:   // 双指针从两端比较
来源：http://iu.9csxet.cn

Ruby: s == s.reverse
来源：http://ab.szsharing.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://cw.colortex.cn

[N07] 两数之和（返回下标）
来源：http://gq.hnjuh.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wq.huanxung.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://zf.hnjuh.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://kv.huixiangedu.cn

TS:   // 手写 Map<string, number>
来源：http://yc.jctech888.com.cn

Java: // 手写 HashMap
来源：http://zv.huixiangedu.cn

Go:   // 手写 map[int]int
来源：http://uw.hahajie.cn

Ruby: // 手写 Hash
来源：http://fg.hnjuh.cn

C#:   // 手写 Dictionary<int, int>
来源：http://np.huixiangedu.cn

[N08] 生成全排列
来源：http://qs.9csxet.cn

Py:   itertools.permutations(arr)
来源：http://it.shxzukj.cn

PHP:  // 手写递归交换
来源：http://mw.jianghongdianzi.cn

JS:   // 手写回溯递归
来源：http://gv.hahajie.cn

TS:   // 手写回溯递归
来源：http://zx.szsharing.cn

Java: // 手写回溯递归
来源：http://ku.jianghongdianzi.cn

Go:   // 手写回溯递归
来源：http://lq.szxytkj.cn

Ruby: arr.permutation.to_a
来源：http://gp.shxzskj.cn

C#:   // 手写回溯递归
来源：http://ns.shxzskj.cn

[N09] 栈与队列
来源：http://vq.jianghongdianzi.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ku.9csxet.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://bz.colortex.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://zf.bjjhwx.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://rm.haigaiapp.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://kq.szsharing.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wp.hnjuh.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://nx.shtwfgs.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://vq.shxzskj.cn

[N10] 链表节点定义
来源：http://xu.nicolike.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://sd.chemitech.net.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ij.chemitech.net.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://tv.panjiajie.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://dh.shxzskj.cn

Java: class Node { int v; Node next; }
来源：http://qu.yuexingan06.cn

Go:   type Node struct { V int; Next *Node }
来源：http://oj.huixiangedu.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ol.muxihuayi.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://vb.nicolike.cn

[N11] 二叉树中序遍历
来源：http://tf.asd995.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://lz.szsharing.cn

PHP:  // 手写递归函数
来源：http://pn.panjiajie.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bu.newstarts.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ra.521024.cn

Java: // 手写递归
来源：http://cq.yuntaijiaju.cn

Go:   // 手写递归
来源：http://ks.shxzskj.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://uu.jianghongdianzi.cn

C#:   // 手写递归
来源：http://fv.bookmarksfly.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://uq.hahajie.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://bn.huixinmuqiang.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://gn.shtwfgs.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qv.chemitech.net.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sz.gzmigu.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mk.hnjuh.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://cr.huanxung.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://bk.szsharing.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ya.shxzskj.cn

================================================================================
来源：http://nf.huixiangedu.cn

O. 并发与异步
来源：http://jc.nszjky.cn

================================================================================
来源：http://sg.jctech888.com.cn

[O01] 启动一个线程
来源：http://kf.newstarts.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://yi.gzmigu.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://sj.huixiangedu.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ra.jctech888.com.cn

TS:   // 同 JS
来源：http://mc.huanxung.cn

Java: new Thread(() -> f()).start()
来源：http://wo.colortex.cn

Go:   go f()
来源：http://tu.shxzskj.cn

Ruby: Thread.new { f }
来源：http://ur.gzmigu.cn

C#:   Task.Run(() => F());
来源：http://jc.chemitech.net.cn

[O02] 使用线程池
来源：http://fz.huixinmuqiang.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://cr.jianghongdianzi.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ep.521024.cn

JS:   // worker_threads 线程池
来源：http://im.panjiajie.cn

TS:   // worker_threads 线程池
来源：http://ok.shxzskj.cn

Java: Executors.newFixedThreadPool(4)
来源：http://xw.asd995.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://po.chemitech.net.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://nz.jctech888.com.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ya.hnjuh.cn

[O03] 加锁保护共享数据
来源：http://sa.muxihuayi.cn

Py:   with lock: shared += 1
来源：http://rl.yuexingan06.cn

PHP:  // 用 flock() 做文件锁
来源：http://wp.9csxet.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://pf.gzmigu.cn

TS:   // 同 JS
来源：http://rb.asd995.cn

Java: synchronized (this) { shared++; }
来源：http://bs.lnxyls.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://xo.haigaiapp.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://hu.chemitech.net.cn

C#:   lock (gate) { shared++; }
来源：http://fz.muxihuayi.cn

[O04] 定义异步函数并等待
来源：http://hf.shxzukj.cn

Py:   async def f():⏎    await g()
来源：http://xz.521024.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://pz.521024.cn

JS:   async function f() { await g(); }
来源：http://ta.panjiajie.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://fy.hnjuh.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://pi.szxytkj.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://kh.bookmarksfly.cn

Ruby: # 用 Fiber 或 async gem
来源：http://lp.9csxet.cn

C#:   async Task F() { await G(); }
来源：http://gi.521024.cn

[O05] 并发执行并等待全部完成
来源：http://bj.521024.cn

Py:   asyncio.gather(*tasks)
来源：http://bo.huanxung.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ks.jctech888.com.cn

JS:   await Promise.all(tasks)
来源：http://sn.shxzskj.cn

TS:   await Promise.all(tasks)
来源：http://jo.gzmigu.cn


<!-- 参考信息 -->