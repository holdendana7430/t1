代发 wailian999

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ff.panjiajie.cn

JS:   await fetch(url)
来源：http://ck.huixinmuqiang.cn

TS:   await fetch(url)
来源：http://kx.chemitech.net.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ob.shtwfgs.cn

Go:   resp, err := http.Get(url)
来源：http://uk.bjjhwx.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://tn.nicolike.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://pz.bjjhwx.cn

[L02] 发送 POST JSON
来源：http://dd.nicolike.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ee.shtwfgs.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://aq.521024.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://eh.yuexingan06.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mh.chemitech.net.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://re.shxzskj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mq.szsharing.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://vz.asd995.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ob.szsharing.cn

[L03] 设置自定义请求头
来源：http://mv.wgjwhj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ze.yuntaijiaju.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://vn.wgjwhj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vx.9csxet.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://er.hnjuh.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ay.muxihuayi.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wq.gzmigu.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://su.huanxung.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://rz.bjjhwx.cn

[L04] 设置超时
来源：http://gx.lnxyls.cn

Py:   requests.get(url, timeout=5)
来源：http://rb.szsharing.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hq.jianghongdianzi.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ag.yuexingan06.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qb.huixiangedu.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://pz.huixiangedu.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ex.jianghongdianzi.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://co.asd995.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hu.nicolike.cn

[L05] 上传文件（multipart）
来源：http://be.huixinmuqiang.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://sc.panjiajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://fc.panjiajie.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://pd.9csxet.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ly.gzmigu.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ge.colortex.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://rd.yuexingan06.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mu.muxihuayi.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ty.hnjuh.cn

[L06] 解析响应为 JSON
来源：http://ga.lnxyls.cn

Py:   resp.json()
来源：http://aw.huixiangedu.cn

PHP:  json_decode($body, true);
来源：http://ji.gzmigu.cn

JS:   await resp.json()
来源：http://tw.bookmarksfly.cn

TS:   await resp.json()
来源：http://qm.9csxet.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://us.huanxung.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://pn.huixiangedu.cn

Ruby: JSON.parse(resp.body)
来源：http://rl.newstarts.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://jb.9csxet.cn

[L07] 处理 HTTP 状态码
来源：http://gb.asd995.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://uc.gzmigu.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://kq.yuexingan06.cn

JS:   resp.ok;  resp.status
来源：http://zj.newstarts.cn

TS:   resp.ok;  resp.status
来源：http://em.hahajie.cn

Java: resp.statusCode()
来源：http://lu.shxzukj.cn

Go:   resp.StatusCode
来源：http://jj.nicolike.cn

Ruby: resp.code.to_i
来源：http://xf.lnxyls.cn

C#:   (int)resp.StatusCode
来源：http://if.nszjky.cn

[L08] 并发请求多个地址
来源：http://fy.huanxung.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://bs.szxytkj.cn

PHP:  curl_multi_init() 系列
来源：http://bp.shxzskj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mi.yuexingan06.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sc.szsharing.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://qq.yuexingan06.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ye.colortex.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wp.shxzskj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://qr.shtwfgs.cn

================================================================================
来源：http://mh.colortex.cn

M. 命令行 / 进程 / 环境
来源：http://mn.colortex.cn

================================================================================
来源：http://kp.jianghongdianzi.cn

[M01] 读取命令行参数
来源：http://rr.bookmarksfly.cn

Py:   sys.argv[1:]
来源：http://bg.colortex.cn

PHP:  $argv;  $argc;
来源：http://es.colortex.cn

JS:   process.argv.slice(2)
来源：http://nq.haigaiapp.cn

TS:   process.argv.slice(2)
来源：http://ka.bjjhwx.cn

Java: args 数组（main 方法参数）
来源：http://vl.lnxyls.cn

Go:   os.Args[1:]
来源：http://dg.panjiajie.cn

Ruby: ARGV
来源：http://yr.hnjuh.cn

C#:   args 数组（Main 方法参数）
来源：http://vv.lnxyls.cn

[M02] 读取环境变量
来源：http://pm.colortex.cn

Py:   os.environ.get("HOME")
来源：http://kv.yuexingan06.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://le.haigaiapp.cn

JS:   process.env.HOME
来源：http://ez.shxzukj.cn

TS:   process.env.HOME
来源：http://pv.panjiajie.cn

Java: System.getenv("HOME")
来源：http://ui.chemitech.net.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://pu.wgjwhj.cn

Ruby: ENV["HOME"]
来源：http://nd.521024.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wu.yuexingan06.cn

[M03] 执行外部命令
来源：http://ob.wgjwhj.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ux.huanxung.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://gt.lnxyls.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ft.9csxet.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://oz.bookmarksfly.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://lo.shtwfgs.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://zp.szsharing.cn

Ruby: system("ls -l");  `ls -l`
来源：http://vs.huanxung.cn

C#:   Process.Start("ls", "-l");
来源：http://gm.yuntaijiaju.cn

[M04] 获取当前工作目录
来源：http://ih.lnxyls.cn

Py:   os.getcwd()
来源：http://bj.bookmarksfly.cn

PHP:  getcwd();
来源：http://nz.shtwfgs.cn

JS:   process.cwd()
来源：http://cu.lnxyls.cn

TS:   process.cwd()
来源：http://zl.9csxet.cn

Java: Path.of("").toAbsolutePath()
来源：http://rq.hnjuh.cn

Go:   os.Getwd()
来源：http://tj.haigaiapp.cn

Ruby: Dir.pwd
来源：http://wc.colortex.cn

C#:   Directory.GetCurrentDirectory()
来源：http://vy.gzmigu.cn

[M05] 设置退出码
来源：http://bg.nszjky.cn

Py:   sys.exit(1)
来源：http://zb.newstarts.cn

PHP:  exit(1);
来源：http://uh.yuexingan06.cn

JS:   process.exit(1)
来源：http://fj.hnjuh.cn

TS:   process.exit(1)
来源：http://dj.szxytkj.cn

Java: System.exit(1)
来源：http://dp.521024.cn

Go:   os.Exit(1)
来源：http://qx.hahajie.cn

Ruby: exit 1
来源：http://ae.colortex.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://zb.shtwfgs.cn

[M06] 向标准错误输出
来源：http://yu.521024.cn

Py:   print("err", file=sys.stderr)
来源：http://sl.shtwfgs.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ah.hahajie.cn

JS:   console.error("err")
来源：http://ym.newstarts.cn

TS:   console.error("err")
来源：http://vf.jctech888.com.cn

Java: System.err.println("err")
来源：http://xg.huixinmuqiang.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://rq.haigaiapp.cn

Ruby: warn "err"
来源：http://hf.nszjky.cn

C#:   Console.Error.WriteLine("err")
来源：http://qj.gzmigu.cn

[M07] 判断是否为主入口
来源：http://jl.huixiangedu.cn

Py:   if __name__ == "__main__":
来源：http://xm.lnxyls.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://fk.hnjuh.cn

JS:   require.main === module
来源：http://ol.asd995.cn

TS:   require.main === module
来源：http://zf.bookmarksfly.cn

Java: public static void main(String[] args)
来源：http://no.newstarts.cn

Go:   func main()
来源：http://qv.chemitech.net.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://bp.yuntaijiaju.cn

C#:   static void Main(string[] args)
来源：http://im.huixiangedu.cn

[M08] 获取系统与运行时信息
来源：http://wf.shxzskj.cn

Py:   platform.system();  platform.python_version()
来源：http://nk.gzmigu.cn

PHP:  PHP_OS;  phpversion();
来源：http://fg.bookmarksfly.cn

JS:   process.platform;  process.version
来源：http://ex.lnxyls.cn

TS:   process.platform;  process.version
来源：http://eq.521024.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://vo.9csxet.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ah.wgjwhj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://uz.huixiangedu.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://fs.nicolike.cn

================================================================================
来源：http://jq.jctech888.com.cn

N. 数据结构与算法
来源：http://wn.hahajie.cn

================================================================================
来源：http://sg.9csxet.cn

[N01] 二分查找（有序数组）
来源：http://bm.yuexingan06.cn

Py:   bisect.bisect_left(arr, x)
来源：http://cl.huixiangedu.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wl.huixiangedu.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ov.bookmarksfly.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ji.nicolike.cn

Java: Arrays.binarySearch(arr, x)
来源：http://iv.huixinmuqiang.cn

Go:   sort.SearchInts(arr, x)
来源：http://rm.haigaiapp.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://zw.gzmigu.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ti.chemitech.net.cn

[N02] 排序（工程实践用内置实现）
来源：http://su.521024.cn

Py:   sorted(arr);  arr.sort()
来源：http://dx.szxytkj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://xw.newstarts.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://gz.hnjuh.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://tm.gzmigu.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://lz.521024.cn

Go:   slices.Sort(arr)
来源：http://vp.lnxyls.cn

Ruby: arr.sort
来源：http://lk.jianghongdianzi.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ca.szxytkj.cn

[N03] 快速排序（分治示例）
来源：http://it.asd995.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://aw.chemitech.net.cn

PHP:  // 递归实现，或用 usort
来源：http://jc.lnxyls.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bu.shxzukj.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rq.wgjwhj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://gq.muxihuayi.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://fr.lnxyls.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://zn.bjjhwx.cn

C#:   // 手写递归，或 Array.Sort
来源：http://bk.newstarts.cn

[N04] 斐波那契数列
来源：http://jw.szxytkj.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://td.huanxung.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://kj.haigaiapp.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hr.521024.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xr.szsharing.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ft.chemitech.net.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://my.shtwfgs.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ss.nszjky.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://fc.521024.cn

[N05] 最大公约数
来源：http://yq.asd995.cn

Py:   math.gcd(a, b)
来源：http://il.nszjky.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://lz.panjiajie.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bb.yuexingan06.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fz.yuntaijiaju.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ua.huixinmuqiang.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://nm.shxzskj.cn

Ruby: a.gcd(b)
来源：http://rj.szxytkj.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://av.szxytkj.cn

[N06] 判断回文字符串
来源：http://tg.muxihuayi.cn

Py:   s == s[::-1]
来源：http://gv.jianghongdianzi.cn

PHP:  $s === strrev($s);
来源：http://ls.huixinmuqiang.cn

JS:   s === [...s].reverse().join("")
来源：http://zv.shxzukj.cn

TS:   s === [...s].reverse().join("")
来源：http://xn.521024.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xc.gzmigu.cn

Go:   // 双指针从两端比较
来源：http://fq.jianghongdianzi.cn

Ruby: s == s.reverse
来源：http://ra.jianghongdianzi.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://xr.bjjhwx.cn

[N07] 两数之和（返回下标）
来源：http://cf.jianghongdianzi.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://vl.shtwfgs.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ap.shtwfgs.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://kv.newstarts.cn

TS:   // 手写 Map<string, number>
来源：http://mj.hnjuh.cn

Java: // 手写 HashMap
来源：http://xi.nicolike.cn

Go:   // 手写 map[int]int
来源：http://xj.lnxyls.cn

Ruby: // 手写 Hash
来源：http://we.asd995.cn

C#:   // 手写 Dictionary<int, int>
来源：http://um.bjjhwx.cn

[N08] 生成全排列
来源：http://bh.huanxung.cn

Py:   itertools.permutations(arr)
来源：http://rh.nicolike.cn

PHP:  // 手写递归交换
来源：http://bf.bjjhwx.cn

JS:   // 手写回溯递归
来源：http://et.wgjwhj.cn

TS:   // 手写回溯递归
来源：http://xq.wgjwhj.cn

Java: // 手写回溯递归
来源：http://ii.9csxet.cn

Go:   // 手写回溯递归
来源：http://yw.huanxung.cn

Ruby: arr.permutation.to_a
来源：http://dc.wgjwhj.cn

C#:   // 手写回溯递归
来源：http://zf.521024.cn

[N09] 栈与队列
来源：http://pr.huixiangedu.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://il.huixiangedu.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://uz.panjiajie.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://km.yuexingan06.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ma.szxytkj.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://gv.yuntaijiaju.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://sr.shtwfgs.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://oc.newstarts.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ff.hnjuh.cn

[N10] 链表节点定义
来源：http://wj.panjiajie.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://tw.gzmigu.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://nk.szsharing.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://xr.huixiangedu.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://js.huixiangedu.cn

Java: class Node { int v; Node next; }
来源：http://yg.muxihuayi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://gl.hnjuh.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://kj.lnxyls.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://dv.jctech888.com.cn

[N11] 二叉树中序遍历
来源：http://pv.asd995.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://yq.521024.cn

PHP:  // 手写递归函数
来源：http://pg.shtwfgs.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://iq.gzmigu.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://la.yuntaijiaju.cn

Java: // 手写递归
来源：http://zz.lnxyls.cn

Go:   // 手写递归
来源：http://kq.wgjwhj.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://px.szsharing.cn

C#:   // 手写递归
来源：http://xs.lnxyls.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://xm.shxzukj.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://fj.haigaiapp.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hm.nszjky.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pa.bjjhwx.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rh.bjjhwx.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://oe.jctech888.com.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://an.muxihuayi.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://op.asd995.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://dc.jctech888.com.cn

================================================================================
来源：http://ok.newstarts.cn

O. 并发与异步
来源：http://ys.wgjwhj.cn

================================================================================
来源：http://ma.yuntaijiaju.cn

[O01] 启动一个线程
来源：http://ug.colortex.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ff.panjiajie.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ef.wgjwhj.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://cs.jctech888.com.cn

TS:   // 同 JS
来源：http://ew.jctech888.com.cn

Java: new Thread(() -> f()).start()
来源：http://cl.huanxung.cn

Go:   go f()
来源：http://fc.shxzskj.cn

Ruby: Thread.new { f }
来源：http://oc.gzmigu.cn

C#:   Task.Run(() => F());
来源：http://ho.chemitech.net.cn

[O02] 使用线程池
来源：http://ck.huanxung.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://kg.shxzskj.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://fb.bjjhwx.cn

JS:   // worker_threads 线程池
来源：http://av.bookmarksfly.cn

TS:   // worker_threads 线程池
来源：http://dj.jctech888.com.cn

Java: Executors.newFixedThreadPool(4)
来源：http://nf.huanxung.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://xt.huanxung.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://fd.shxzukj.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://jk.yuntaijiaju.cn

[O03] 加锁保护共享数据
来源：http://wp.jianghongdianzi.cn

Py:   with lock: shared += 1
来源：http://mz.yuexingan06.cn

PHP:  // 用 flock() 做文件锁
来源：http://js.yuexingan06.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ev.chemitech.net.cn

TS:   // 同 JS
来源：http://lc.wgjwhj.cn

Java: synchronized (this) { shared++; }
来源：http://vr.jianghongdianzi.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://pf.huixinmuqiang.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://jh.jianghongdianzi.cn

C#:   lock (gate) { shared++; }
来源：http://lg.yuntaijiaju.cn

[O04] 定义异步函数并等待
来源：http://zq.shxzskj.cn

Py:   async def f():⏎    await g()
来源：http://fz.lnxyls.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://zu.shtwfgs.cn

JS:   async function f() { await g(); }
来源：http://em.szsharing.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ec.hahajie.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://bj.szxytkj.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://nj.9csxet.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ns.hahajie.cn

C#:   async Task F() { await G(); }
来源：http://si.asd995.cn

[O05] 并发执行并等待全部完成
来源：http://th.huixinmuqiang.cn

Py:   asyncio.gather(*tasks)
来源：http://xc.haigaiapp.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://dx.yuntaijiaju.cn

JS:   await Promise.all(tasks)
来源：http://pw.huanxung.cn

TS:   await Promise.all(tasks)
来源：http://ey.nszjky.cn


<!-- 参考信息 -->