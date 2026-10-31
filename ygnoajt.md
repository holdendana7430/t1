代发 wailian999

Go:   resp, err := http.Get(url)
来源：http://xy.gzmigu.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ie.jianghongdianzi.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://re.shxzukj.cn

[L02] 发送 POST JSON
来源：http://bb.shxzskj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ax.nszjky.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://gy.colortex.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://uh.hahajie.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://uw.hahajie.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://kd.huixinmuqiang.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qw.jianghongdianzi.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xz.521024.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ys.yuntaijiaju.cn

[L03] 设置自定义请求头
来源：http://db.huixinmuqiang.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://yl.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://jv.shtwfgs.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pl.yuexingan06.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mx.shxzukj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://oh.nicolike.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://qg.muxihuayi.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://si.szsharing.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://kp.haigaiapp.cn

[L04] 设置超时
来源：http://hq.haigaiapp.cn

Py:   requests.get(url, timeout=5)
来源：http://tp.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://nv.bjjhwx.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cd.hahajie.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pe.panjiajie.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://tu.jianghongdianzi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://tx.panjiajie.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hb.bjjhwx.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://xu.jctech888.com.cn

[L05] 上传文件（multipart）
来源：http://gw.shxzukj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://um.shtwfgs.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://xq.yuntaijiaju.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://bk.szxytkj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://uh.newstarts.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ak.muxihuayi.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://gt.muxihuayi.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://um.panjiajie.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://tv.lnxyls.cn

[L06] 解析响应为 JSON
来源：http://ak.nszjky.cn

Py:   resp.json()
来源：http://gg.hahajie.cn

PHP:  json_decode($body, true);
来源：http://sg.bjjhwx.cn

JS:   await resp.json()
来源：http://al.lnxyls.cn

TS:   await resp.json()
来源：http://xv.huixinmuqiang.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://bw.chemitech.net.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://uo.gzmigu.cn

Ruby: JSON.parse(resp.body)
来源：http://ig.gzmigu.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hs.hahajie.cn

[L07] 处理 HTTP 状态码
来源：http://dc.nicolike.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ih.huixinmuqiang.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qo.huixinmuqiang.cn

JS:   resp.ok;  resp.status
来源：http://ml.chemitech.net.cn

TS:   resp.ok;  resp.status
来源：http://bh.szsharing.cn

Java: resp.statusCode()
来源：http://re.jianghongdianzi.cn

Go:   resp.StatusCode
来源：http://cf.muxihuayi.cn

Ruby: resp.code.to_i
来源：http://bw.huixinmuqiang.cn

C#:   (int)resp.StatusCode
来源：http://ig.hnjuh.cn

[L08] 并发请求多个地址
来源：http://ct.gzmigu.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://eg.bookmarksfly.cn

PHP:  curl_multi_init() 系列
来源：http://rv.hahajie.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xy.yuexingan06.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zd.521024.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://na.jianghongdianzi.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://fd.huanxung.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://lv.huixiangedu.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://oj.panjiajie.cn

================================================================================
来源：http://na.newstarts.cn

M. 命令行 / 进程 / 环境
来源：http://jf.chemitech.net.cn

================================================================================
来源：http://jc.hahajie.cn

[M01] 读取命令行参数
来源：http://te.newstarts.cn

Py:   sys.argv[1:]
来源：http://cd.colortex.cn

PHP:  $argv;  $argc;
来源：http://ok.gzmigu.cn

JS:   process.argv.slice(2)
来源：http://hx.panjiajie.cn

TS:   process.argv.slice(2)
来源：http://fa.lnxyls.cn

Java: args 数组（main 方法参数）
来源：http://gd.bookmarksfly.cn

Go:   os.Args[1:]
来源：http://hf.asd995.cn

Ruby: ARGV
来源：http://yz.muxihuayi.cn

C#:   args 数组（Main 方法参数）
来源：http://nr.panjiajie.cn

[M02] 读取环境变量
来源：http://jb.wgjwhj.cn

Py:   os.environ.get("HOME")
来源：http://hx.szxytkj.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://xh.wgjwhj.cn

JS:   process.env.HOME
来源：http://eb.huixinmuqiang.cn

TS:   process.env.HOME
来源：http://zw.asd995.cn

Java: System.getenv("HOME")
来源：http://tr.nicolike.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ui.huixiangedu.cn

Ruby: ENV["HOME"]
来源：http://ar.chemitech.net.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wm.panjiajie.cn

[M03] 执行外部命令
来源：http://bj.jctech888.com.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://lg.szxytkj.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://rf.nszjky.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://kn.shxzskj.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://iy.wgjwhj.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://zz.shtwfgs.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://qk.yuntaijiaju.cn

Ruby: system("ls -l");  `ls -l`
来源：http://uo.panjiajie.cn

C#:   Process.Start("ls", "-l");
来源：http://lv.bjjhwx.cn

[M04] 获取当前工作目录
来源：http://pl.yuntaijiaju.cn

Py:   os.getcwd()
来源：http://uq.newstarts.cn

PHP:  getcwd();
来源：http://ci.shxzukj.cn

JS:   process.cwd()
来源：http://an.szsharing.cn

TS:   process.cwd()
来源：http://ow.nszjky.cn

Java: Path.of("").toAbsolutePath()
来源：http://kq.asd995.cn

Go:   os.Getwd()
来源：http://xh.yuntaijiaju.cn

Ruby: Dir.pwd
来源：http://pp.bookmarksfly.cn

C#:   Directory.GetCurrentDirectory()
来源：http://td.huixinmuqiang.cn

[M05] 设置退出码
来源：http://fi.nszjky.cn

Py:   sys.exit(1)
来源：http://gv.nszjky.cn

PHP:  exit(1);
来源：http://dc.huixinmuqiang.cn

JS:   process.exit(1)
来源：http://yq.colortex.cn

TS:   process.exit(1)
来源：http://wy.shxzskj.cn

Java: System.exit(1)
来源：http://bx.nicolike.cn

Go:   os.Exit(1)
来源：http://gd.huixinmuqiang.cn

Ruby: exit 1
来源：http://vx.chemitech.net.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://bb.jianghongdianzi.cn

[M06] 向标准错误输出
来源：http://er.521024.cn

Py:   print("err", file=sys.stderr)
来源：http://au.jctech888.com.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://hs.huixinmuqiang.cn

JS:   console.error("err")
来源：http://rf.huanxung.cn

TS:   console.error("err")
来源：http://mz.szsharing.cn

Java: System.err.println("err")
来源：http://tu.colortex.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://xt.nszjky.cn

Ruby: warn "err"
来源：http://fi.jianghongdianzi.cn

C#:   Console.Error.WriteLine("err")
来源：http://ny.9csxet.cn

[M07] 判断是否为主入口
来源：http://rp.huanxung.cn

Py:   if __name__ == "__main__":
来源：http://ef.huixiangedu.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ho.szsharing.cn

JS:   require.main === module
来源：http://ga.huixinmuqiang.cn

TS:   require.main === module
来源：http://gk.newstarts.cn

Java: public static void main(String[] args)
来源：http://xz.haigaiapp.cn

Go:   func main()
来源：http://sh.hnjuh.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://rf.colortex.cn

C#:   static void Main(string[] args)
来源：http://fp.nszjky.cn

[M08] 获取系统与运行时信息
来源：http://lq.gzmigu.cn

Py:   platform.system();  platform.python_version()
来源：http://vn.colortex.cn

PHP:  PHP_OS;  phpversion();
来源：http://nv.haigaiapp.cn

JS:   process.platform;  process.version
来源：http://xp.huixinmuqiang.cn

TS:   process.platform;  process.version
来源：http://oo.bookmarksfly.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://br.bookmarksfly.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://on.hahajie.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ne.shxzukj.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://fq.hnjuh.cn

================================================================================
来源：http://sv.bjjhwx.cn

N. 数据结构与算法
来源：http://qz.huixinmuqiang.cn

================================================================================
来源：http://pb.hahajie.cn

[N01] 二分查找（有序数组）
来源：http://fx.gzmigu.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ub.szsharing.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://iu.muxihuayi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sy.huixinmuqiang.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qs.szsharing.cn

Java: Arrays.binarySearch(arr, x)
来源：http://rw.newstarts.cn

Go:   sort.SearchInts(arr, x)
来源：http://fy.lnxyls.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://qv.huixinmuqiang.cn

C#:   Array.BinarySearch(arr, x)
来源：http://pw.asd995.cn

[N02] 排序（工程实践用内置实现）
来源：http://af.huixinmuqiang.cn

Py:   sorted(arr);  arr.sort()
来源：http://vx.lnxyls.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://dc.yuntaijiaju.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ed.bjjhwx.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://yi.panjiajie.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ns.yuexingan06.cn

Go:   slices.Sort(arr)
来源：http://il.gzmigu.cn

Ruby: arr.sort
来源：http://vb.szxytkj.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://cl.521024.cn

[N03] 快速排序（分治示例）
来源：http://rb.yuexingan06.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://gj.panjiajie.cn

PHP:  // 递归实现，或用 usort
来源：http://as.muxihuayi.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fo.colortex.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://va.colortex.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://bp.muxihuayi.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://pw.bookmarksfly.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wv.chemitech.net.cn

C#:   // 手写递归，或 Array.Sort
来源：http://jx.huixinmuqiang.cn

[N04] 斐波那契数列
来源：http://bx.shtwfgs.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://iz.nszjky.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ri.jctech888.com.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://uw.colortex.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://uv.lnxyls.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://vm.shtwfgs.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://bj.szsharing.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://os.shtwfgs.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://lu.shtwfgs.cn

[N05] 最大公约数
来源：http://vg.szsharing.cn

Py:   math.gcd(a, b)
来源：http://jl.huixiangedu.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ub.9csxet.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pc.shxzukj.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lo.lnxyls.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://nx.9csxet.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://io.asd995.cn

Ruby: a.gcd(b)
来源：http://cr.gzmigu.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://kl.hahajie.cn

[N06] 判断回文字符串
来源：http://zn.yuexingan06.cn

Py:   s == s[::-1]
来源：http://kl.colortex.cn

PHP:  $s === strrev($s);
来源：http://dh.bjjhwx.cn

JS:   s === [...s].reverse().join("")
来源：http://et.chemitech.net.cn

TS:   s === [...s].reverse().join("")
来源：http://te.9csxet.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://bg.9csxet.cn

Go:   // 双指针从两端比较
来源：http://gr.shxzskj.cn

Ruby: s == s.reverse
来源：http://eh.bjjhwx.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://an.shtwfgs.cn

[N07] 两数之和（返回下标）
来源：http://tg.huanxung.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://xa.lnxyls.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://lb.colortex.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ms.newstarts.cn

TS:   // 手写 Map<string, number>
来源：http://ha.yuexingan06.cn

Java: // 手写 HashMap
来源：http://lr.nicolike.cn

Go:   // 手写 map[int]int
来源：http://ei.colortex.cn

Ruby: // 手写 Hash
来源：http://wl.szxytkj.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ow.jctech888.com.cn

[N08] 生成全排列
来源：http://ih.huixinmuqiang.cn

Py:   itertools.permutations(arr)
来源：http://go.huanxung.cn

PHP:  // 手写递归交换
来源：http://ki.colortex.cn

JS:   // 手写回溯递归
来源：http://vb.wgjwhj.cn

TS:   // 手写回溯递归
来源：http://nz.huanxung.cn

Java: // 手写回溯递归
来源：http://ac.colortex.cn

Go:   // 手写回溯递归
来源：http://ts.521024.cn

Ruby: arr.permutation.to_a
来源：http://pj.gzmigu.cn

C#:   // 手写回溯递归
来源：http://pk.shxzukj.cn

[N09] 栈与队列
来源：http://xn.yuntaijiaju.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://pi.chemitech.net.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://jy.wgjwhj.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hj.521024.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ge.huixinmuqiang.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ah.521024.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://oo.lnxyls.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ht.shtwfgs.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://qw.nicolike.cn

[N10] 链表节点定义
来源：http://xx.jctech888.com.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://is.chemitech.net.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://rx.wgjwhj.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ye.muxihuayi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://sl.bookmarksfly.cn

Java: class Node { int v; Node next; }
来源：http://gy.haigaiapp.cn

Go:   type Node struct { V int; Next *Node }
来源：http://if.yuntaijiaju.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://tp.shxzskj.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ax.colortex.cn

[N11] 二叉树中序遍历
来源：http://lt.chemitech.net.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://rl.colortex.cn

PHP:  // 手写递归函数
来源：http://bs.bjjhwx.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wp.jianghongdianzi.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zk.panjiajie.cn

Java: // 手写递归
来源：http://vf.panjiajie.cn

Go:   // 手写递归
来源：http://qf.hahajie.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://xd.521024.cn

C#:   // 手写递归
来源：http://br.huixinmuqiang.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://sw.bookmarksfly.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hc.hnjuh.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://uy.hnjuh.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dp.hnjuh.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fk.chemitech.net.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://is.lnxyls.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://vd.chemitech.net.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://uw.szsharing.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hg.shxzukj.cn

================================================================================
来源：http://op.shxzukj.cn

O. 并发与异步
来源：http://bh.9csxet.cn

================================================================================
来源：http://gf.muxihuayi.cn

[O01] 启动一个线程
来源：http://ip.bjjhwx.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://qb.huixinmuqiang.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qs.jctech888.com.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://xx.panjiajie.cn

TS:   // 同 JS
来源：http://ch.shxzukj.cn

Java: new Thread(() -> f()).start()
来源：http://ge.huixiangedu.cn

Go:   go f()
来源：http://vi.jianghongdianzi.cn

Ruby: Thread.new { f }
来源：http://wq.shtwfgs.cn

C#:   Task.Run(() => F());
来源：http://xs.bjjhwx.cn

[O02] 使用线程池
来源：http://jz.9csxet.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://sa.9csxet.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hb.muxihuayi.cn

JS:   // worker_threads 线程池
来源：http://jh.shtwfgs.cn

TS:   // worker_threads 线程池
来源：http://hc.szsharing.cn

Java: Executors.newFixedThreadPool(4)
来源：http://nr.asd995.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://rp.wgjwhj.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ek.hnjuh.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://je.shxzukj.cn

[O03] 加锁保护共享数据
来源：http://pl.szxytkj.cn

Py:   with lock: shared += 1
来源：http://mp.hahajie.cn

PHP:  // 用 flock() 做文件锁
来源：http://nv.lnxyls.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://xy.muxihuayi.cn

TS:   // 同 JS
来源：http://rk.9csxet.cn

Java: synchronized (this) { shared++; }
来源：http://py.lnxyls.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://um.yuntaijiaju.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://uv.yuntaijiaju.cn

C#:   lock (gate) { shared++; }
来源：http://wv.wgjwhj.cn

[O04] 定义异步函数并等待
来源：http://gm.shxzskj.cn

Py:   async def f():⏎    await g()
来源：http://ap.huixinmuqiang.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ni.panjiajie.cn

JS:   async function f() { await g(); }
来源：http://ll.muxihuayi.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://wg.gzmigu.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mw.szxytkj.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://zn.shxzukj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://qz.nicolike.cn

C#:   async Task F() { await G(); }
来源：http://rt.nicolike.cn

[O05] 并发执行并等待全部完成
来源：http://qa.521024.cn

Py:   asyncio.gather(*tasks)
来源：http://kk.muxihuayi.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://sf.wgjwhj.cn

JS:   await Promise.all(tasks)
来源：http://mr.chemitech.net.cn

TS:   await Promise.all(tasks)
来源：http://tj.chemitech.net.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://vm.hahajie.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ah.nicolike.cn

Ruby: threads.map(&:join)
来源：http://lq.yuntaijiaju.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://lu.chemitech.net.cn


<!-- 参考信息 -->