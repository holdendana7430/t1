代发 wailian999

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://pk.lnxyls.cn

JS:   await fetch(url)
来源：http://ln.muxihuayi.cn

TS:   await fetch(url)
来源：http://gd.bjjhwx.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ng.9csxet.cn

Go:   resp, err := http.Get(url)
来源：http://gq.shtwfgs.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://uu.nicolike.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://rz.hahajie.cn

[L02] 发送 POST JSON
来源：http://gl.gzmigu.cn

Py:   requests.post(url, json={"a": 1})
来源：http://sa.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://tr.521024.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sd.nszjky.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rm.shtwfgs.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ga.shtwfgs.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://uc.huixiangedu.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://fo.huixiangedu.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://zv.yuntaijiaju.cn

[L03] 设置自定义请求头
来源：http://cq.521024.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://lf.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ba.shxzukj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sw.nszjky.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ju.shxzskj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://bo.szxytkj.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wk.panjiajie.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://xh.gzmigu.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://tb.asd995.cn

[L04] 设置超时
来源：http://vq.nszjky.cn

Py:   requests.get(url, timeout=5)
来源：http://yp.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ug.521024.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://db.huixiangedu.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uw.wgjwhj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://rv.panjiajie.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://yy.muxihuayi.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://in.gzmigu.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hw.lnxyls.cn

[L05] 上传文件（multipart）
来源：http://au.jianghongdianzi.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://sx.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://cf.lnxyls.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://bz.shxzskj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ko.chemitech.net.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hx.szsharing.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://iz.hnjuh.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vw.hahajie.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://lt.colortex.cn

[L06] 解析响应为 JSON
来源：http://bb.nicolike.cn

Py:   resp.json()
来源：http://md.bjjhwx.cn

PHP:  json_decode($body, true);
来源：http://eh.huixiangedu.cn

JS:   await resp.json()
来源：http://af.haigaiapp.cn

TS:   await resp.json()
来源：http://ac.colortex.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mp.nicolike.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://jz.wgjwhj.cn

Ruby: JSON.parse(resp.body)
来源：http://ek.jianghongdianzi.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://br.szxytkj.cn

[L07] 处理 HTTP 状态码
来源：http://cc.panjiajie.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://bi.hahajie.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://nk.bjjhwx.cn

JS:   resp.ok;  resp.status
来源：http://ex.muxihuayi.cn

TS:   resp.ok;  resp.status
来源：http://lc.hnjuh.cn

Java: resp.statusCode()
来源：http://wk.bookmarksfly.cn

Go:   resp.StatusCode
来源：http://yw.huixinmuqiang.cn

Ruby: resp.code.to_i
来源：http://sb.szsharing.cn

C#:   (int)resp.StatusCode
来源：http://tr.jianghongdianzi.cn

[L08] 并发请求多个地址
来源：http://gr.newstarts.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://pp.bookmarksfly.cn

PHP:  curl_multi_init() 系列
来源：http://zu.shtwfgs.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xe.jctech888.com.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xj.bjjhwx.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://qe.chemitech.net.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ur.szsharing.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ki.bjjhwx.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://rb.jctech888.com.cn

================================================================================
来源：http://vo.szsharing.cn

M. 命令行 / 进程 / 环境
来源：http://yg.szsharing.cn

================================================================================
来源：http://cz.hnjuh.cn

[M01] 读取命令行参数
来源：http://ab.panjiajie.cn

Py:   sys.argv[1:]
来源：http://ua.shtwfgs.cn

PHP:  $argv;  $argc;
来源：http://hw.hahajie.cn

JS:   process.argv.slice(2)
来源：http://ts.colortex.cn

TS:   process.argv.slice(2)
来源：http://cg.521024.cn

Java: args 数组（main 方法参数）
来源：http://er.hahajie.cn

Go:   os.Args[1:]
来源：http://rl.shxzskj.cn

Ruby: ARGV
来源：http://uq.jianghongdianzi.cn

C#:   args 数组（Main 方法参数）
来源：http://lp.lnxyls.cn

[M02] 读取环境变量
来源：http://wp.wgjwhj.cn

Py:   os.environ.get("HOME")
来源：http://ui.asd995.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://fx.shxzskj.cn

JS:   process.env.HOME
来源：http://an.huixiangedu.cn

TS:   process.env.HOME
来源：http://az.szxytkj.cn

Java: System.getenv("HOME")
来源：http://db.bjjhwx.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://oa.bjjhwx.cn

Ruby: ENV["HOME"]
来源：http://vr.szxytkj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://kp.shxzskj.cn

[M03] 执行外部命令
来源：http://wz.chemitech.net.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://op.colortex.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mk.521024.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://qf.newstarts.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://za.yuexingan06.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://eq.bookmarksfly.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ox.jianghongdianzi.cn

Ruby: system("ls -l");  `ls -l`
来源：http://oa.jctech888.com.cn

C#:   Process.Start("ls", "-l");
来源：http://xh.yuexingan06.cn

[M04] 获取当前工作目录
来源：http://gv.yuexingan06.cn

Py:   os.getcwd()
来源：http://hg.muxihuayi.cn

PHP:  getcwd();
来源：http://hx.asd995.cn

JS:   process.cwd()
来源：http://eq.jctech888.com.cn

TS:   process.cwd()
来源：http://jt.szsharing.cn

Java: Path.of("").toAbsolutePath()
来源：http://vs.shtwfgs.cn

Go:   os.Getwd()
来源：http://cl.muxihuayi.cn

Ruby: Dir.pwd
来源：http://fn.nicolike.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ua.hnjuh.cn

[M05] 设置退出码
来源：http://vr.panjiajie.cn

Py:   sys.exit(1)
来源：http://qx.szxytkj.cn

PHP:  exit(1);
来源：http://ft.nicolike.cn

JS:   process.exit(1)
来源：http://gk.muxihuayi.cn

TS:   process.exit(1)
来源：http://rk.gzmigu.cn

Java: System.exit(1)
来源：http://na.muxihuayi.cn

Go:   os.Exit(1)
来源：http://xx.asd995.cn

Ruby: exit 1
来源：http://mb.wgjwhj.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://pb.shxzukj.cn

[M06] 向标准错误输出
来源：http://wb.shxzukj.cn

Py:   print("err", file=sys.stderr)
来源：http://hj.huanxung.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://at.shtwfgs.cn

JS:   console.error("err")
来源：http://re.huixiangedu.cn

TS:   console.error("err")
来源：http://px.shxzskj.cn

Java: System.err.println("err")
来源：http://nv.huixiangedu.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://xu.shtwfgs.cn

Ruby: warn "err"
来源：http://cy.wgjwhj.cn

C#:   Console.Error.WriteLine("err")
来源：http://mi.gzmigu.cn

[M07] 判断是否为主入口
来源：http://kx.shxzskj.cn

Py:   if __name__ == "__main__":
来源：http://qv.asd995.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://dh.lnxyls.cn

JS:   require.main === module
来源：http://qu.jctech888.com.cn

TS:   require.main === module
来源：http://pd.shxzukj.cn

Java: public static void main(String[] args)
来源：http://za.gzmigu.cn

Go:   func main()
来源：http://ac.jctech888.com.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wk.jianghongdianzi.cn

C#:   static void Main(string[] args)
来源：http://ur.colortex.cn

[M08] 获取系统与运行时信息
来源：http://xa.huixiangedu.cn

Py:   platform.system();  platform.python_version()
来源：http://ii.lnxyls.cn

PHP:  PHP_OS;  phpversion();
来源：http://ul.huanxung.cn

JS:   process.platform;  process.version
来源：http://kb.huixiangedu.cn

TS:   process.platform;  process.version
来源：http://gc.9csxet.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://up.jctech888.com.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://pr.gzmigu.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://eq.shxzukj.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://lp.huixinmuqiang.cn

================================================================================
来源：http://ok.hnjuh.cn

N. 数据结构与算法
来源：http://tf.haigaiapp.cn

================================================================================
来源：http://vd.nicolike.cn

[N01] 二分查找（有序数组）
来源：http://eu.szxytkj.cn

Py:   bisect.bisect_left(arr, x)
来源：http://rw.lnxyls.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ql.jctech888.com.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hj.wgjwhj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ee.shtwfgs.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ul.nszjky.cn

Go:   sort.SearchInts(arr, x)
来源：http://gq.huanxung.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://qh.jianghongdianzi.cn

C#:   Array.BinarySearch(arr, x)
来源：http://jj.9csxet.cn

[N02] 排序（工程实践用内置实现）
来源：http://og.bjjhwx.cn

Py:   sorted(arr);  arr.sort()
来源：http://yg.chemitech.net.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://av.huixinmuqiang.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ob.bjjhwx.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://pv.lnxyls.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://xw.bjjhwx.cn

Go:   slices.Sort(arr)
来源：http://eq.bookmarksfly.cn

Ruby: arr.sort
来源：http://vs.yuexingan06.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ua.bjjhwx.cn

[N03] 快速排序（分治示例）
来源：http://yg.huixiangedu.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ue.huanxung.cn

PHP:  // 递归实现，或用 usort
来源：http://oa.szsharing.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vt.shxzskj.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://da.colortex.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://bh.shtwfgs.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mk.szxytkj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://gy.shxzskj.cn

C#:   // 手写递归，或 Array.Sort
来源：http://sw.colortex.cn

[N04] 斐波那契数列
来源：http://bq.shxzskj.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://rv.jctech888.com.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://rm.shxzukj.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qe.shxzskj.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qu.bookmarksfly.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://pa.nicolike.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://bu.jctech888.com.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://pn.9csxet.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://fl.hnjuh.cn

[N05] 最大公约数
来源：http://na.huanxung.cn

Py:   math.gcd(a, b)
来源：http://kv.9csxet.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://vf.jianghongdianzi.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yg.huixinmuqiang.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fq.9csxet.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wg.521024.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://dq.bjjhwx.cn

Ruby: a.gcd(b)
来源：http://ig.huanxung.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://rf.hnjuh.cn

[N06] 判断回文字符串
来源：http://uc.colortex.cn

Py:   s == s[::-1]
来源：http://dy.hnjuh.cn

PHP:  $s === strrev($s);
来源：http://jz.szsharing.cn

JS:   s === [...s].reverse().join("")
来源：http://iz.huixiangedu.cn

TS:   s === [...s].reverse().join("")
来源：http://gm.szxytkj.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xl.wgjwhj.cn

Go:   // 双指针从两端比较
来源：http://vd.gzmigu.cn

Ruby: s == s.reverse
来源：http://mr.bjjhwx.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://uw.yuexingan06.cn

[N07] 两数之和（返回下标）
来源：http://ww.hahajie.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://kz.szxytkj.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ks.szxytkj.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://sl.shtwfgs.cn

TS:   // 手写 Map<string, number>
来源：http://lm.colortex.cn

Java: // 手写 HashMap
来源：http://nz.gzmigu.cn

Go:   // 手写 map[int]int
来源：http://kb.newstarts.cn

Ruby: // 手写 Hash
来源：http://wu.haigaiapp.cn

C#:   // 手写 Dictionary<int, int>
来源：http://nv.yuexingan06.cn

[N08] 生成全排列
来源：http://nv.jianghongdianzi.cn

Py:   itertools.permutations(arr)
来源：http://qj.newstarts.cn

PHP:  // 手写递归交换
来源：http://nv.shxzskj.cn

JS:   // 手写回溯递归
来源：http://hs.huixinmuqiang.cn

TS:   // 手写回溯递归
来源：http://bw.shxzskj.cn

Java: // 手写回溯递归
来源：http://lr.shtwfgs.cn

Go:   // 手写回溯递归
来源：http://di.huanxung.cn

Ruby: arr.permutation.to_a
来源：http://ed.gzmigu.cn

C#:   // 手写回溯递归
来源：http://so.hahajie.cn

[N09] 栈与队列
来源：http://dr.hnjuh.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ns.yuntaijiaju.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://fm.lnxyls.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://bs.chemitech.net.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ae.asd995.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://bw.bjjhwx.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://eb.szxytkj.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wn.haigaiapp.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://vm.huanxung.cn

[N10] 链表节点定义
来源：http://sh.haigaiapp.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://zx.shxzskj.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ju.huixinmuqiang.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://pq.jianghongdianzi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://yb.haigaiapp.cn

Java: class Node { int v; Node next; }
来源：http://am.yuntaijiaju.cn

Go:   type Node struct { V int; Next *Node }
来源：http://dn.szxytkj.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ik.shtwfgs.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://th.huanxung.cn

[N11] 二叉树中序遍历
来源：http://zc.szsharing.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://oj.szsharing.cn

PHP:  // 手写递归函数
来源：http://tk.yuexingan06.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yn.hnjuh.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qd.9csxet.cn

Java: // 手写递归
来源：http://bt.nszjky.cn

Go:   // 手写递归
来源：http://jj.nicolike.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://jo.yuexingan06.cn

C#:   // 手写递归
来源：http://gc.521024.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://do.nszjky.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://tz.asd995.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ds.szxytkj.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tf.bjjhwx.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wq.huixiangedu.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://sg.lnxyls.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://rx.521024.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://tv.huixinmuqiang.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ta.9csxet.cn

================================================================================
来源：http://sa.shxzskj.cn

O. 并发与异步
来源：http://di.bjjhwx.cn

================================================================================
来源：http://an.chemitech.net.cn

[O01] 启动一个线程
来源：http://yw.wgjwhj.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://yn.muxihuayi.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://fv.szxytkj.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://an.yuntaijiaju.cn

TS:   // 同 JS
来源：http://bt.nszjky.cn

Java: new Thread(() -> f()).start()
来源：http://bv.hnjuh.cn

Go:   go f()
来源：http://kw.gzmigu.cn

Ruby: Thread.new { f }
来源：http://rs.szxytkj.cn

C#:   Task.Run(() => F());
来源：http://vf.nszjky.cn

[O02] 使用线程池
来源：http://or.asd995.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://nv.lnxyls.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://sk.521024.cn

JS:   // worker_threads 线程池
来源：http://jj.bjjhwx.cn

TS:   // worker_threads 线程池
来源：http://do.shtwfgs.cn

Java: Executors.newFixedThreadPool(4)
来源：http://kg.huixinmuqiang.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://po.9csxet.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://yg.panjiajie.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://bb.gzmigu.cn

[O03] 加锁保护共享数据
来源：http://ou.shtwfgs.cn

Py:   with lock: shared += 1
来源：http://ks.szxytkj.cn

PHP:  // 用 flock() 做文件锁
来源：http://wk.shtwfgs.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ht.szsharing.cn

TS:   // 同 JS
来源：http://gy.huanxung.cn

Java: synchronized (this) { shared++; }
来源：http://wd.asd995.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://jg.9csxet.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://kg.haigaiapp.cn

C#:   lock (gate) { shared++; }
来源：http://nm.gzmigu.cn

[O04] 定义异步函数并等待
来源：http://qs.bjjhwx.cn

Py:   async def f():⏎    await g()
来源：http://xb.huixinmuqiang.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://av.panjiajie.cn

JS:   async function f() { await g(); }
来源：http://lu.hahajie.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ob.szsharing.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ta.haigaiapp.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ck.huixinmuqiang.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ju.szxytkj.cn

C#:   async Task F() { await G(); }
来源：http://ru.hahajie.cn

[O05] 并发执行并等待全部完成
来源：http://vc.bookmarksfly.cn

Py:   asyncio.gather(*tasks)
来源：http://ym.szxytkj.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wc.szsharing.cn

JS:   await Promise.all(tasks)
来源：http://uv.nszjky.cn

TS:   await Promise.all(tasks)
来源：http://ll.szsharing.cn


<!-- 参考信息 -->