代发 wailian999

Go:   resp, err := http.Get(url)
来源：http://xw.lnxyls.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://zw.bookmarksfly.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://aq.hnjuh.cn

[L02] 发送 POST JSON
来源：http://fb.lnxyls.cn

Py:   requests.post(url, json={"a": 1})
来源：http://le.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ft.nszjky.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qn.jctech888.com.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ue.chemitech.net.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ok.huanxung.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ak.panjiajie.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ib.nszjky.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://cm.jianghongdianzi.cn

[L03] 设置自定义请求头
来源：http://pe.szsharing.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ge.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ws.nicolike.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nq.huanxung.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ge.nszjky.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://kr.szsharing.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mb.yuntaijiaju.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://dx.521024.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://qa.muxihuayi.cn

[L04] 设置超时
来源：http://jm.hahajie.cn

Py:   requests.get(url, timeout=5)
来源：http://hh.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://zn.wgjwhj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://sy.yuntaijiaju.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dj.newstarts.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://iw.shxzskj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://dx.haigaiapp.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://kl.shxzukj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://eg.colortex.cn

[L05] 上传文件（multipart）
来源：http://ym.szxytkj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://at.nicolike.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://uf.9csxet.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ba.521024.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://pt.gzmigu.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://gd.hahajie.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://zf.yuntaijiaju.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ve.asd995.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://sy.haigaiapp.cn

[L06] 解析响应为 JSON
来源：http://cs.hahajie.cn

Py:   resp.json()
来源：http://wp.nszjky.cn

PHP:  json_decode($body, true);
来源：http://ve.asd995.cn

JS:   await resp.json()
来源：http://yu.newstarts.cn

TS:   await resp.json()
来源：http://sy.9csxet.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://nl.521024.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://fp.shxzukj.cn

Ruby: JSON.parse(resp.body)
来源：http://um.nicolike.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ao.szxytkj.cn

[L07] 处理 HTTP 状态码
来源：http://em.huixinmuqiang.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://yg.wgjwhj.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://zf.huixinmuqiang.cn

JS:   resp.ok;  resp.status
来源：http://bd.bookmarksfly.cn

TS:   resp.ok;  resp.status
来源：http://qb.newstarts.cn

Java: resp.statusCode()
来源：http://tr.9csxet.cn

Go:   resp.StatusCode
来源：http://pj.yuntaijiaju.cn

Ruby: resp.code.to_i
来源：http://ye.shxzskj.cn

C#:   (int)resp.StatusCode
来源：http://rf.521024.cn

[L08] 并发请求多个地址
来源：http://op.gzmigu.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wf.shxzukj.cn

PHP:  curl_multi_init() 系列
来源：http://ej.panjiajie.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gz.huixiangedu.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pd.bookmarksfly.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://za.huixinmuqiang.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ww.gzmigu.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wy.wgjwhj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://pt.newstarts.cn

================================================================================
来源：http://ru.9csxet.cn

M. 命令行 / 进程 / 环境
来源：http://us.haigaiapp.cn

================================================================================
来源：http://gd.9csxet.cn

[M01] 读取命令行参数
来源：http://cu.yuexingan06.cn

Py:   sys.argv[1:]
来源：http://vh.huixiangedu.cn

PHP:  $argv;  $argc;
来源：http://vt.huixiangedu.cn

JS:   process.argv.slice(2)
来源：http://fg.huixiangedu.cn

TS:   process.argv.slice(2)
来源：http://dh.huixinmuqiang.cn

Java: args 数组（main 方法参数）
来源：http://fh.shxzukj.cn

Go:   os.Args[1:]
来源：http://bf.gzmigu.cn

Ruby: ARGV
来源：http://mq.nicolike.cn

C#:   args 数组（Main 方法参数）
来源：http://th.wgjwhj.cn

[M02] 读取环境变量
来源：http://ft.panjiajie.cn

Py:   os.environ.get("HOME")
来源：http://ja.szsharing.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://jh.huixinmuqiang.cn

JS:   process.env.HOME
来源：http://pe.muxihuayi.cn

TS:   process.env.HOME
来源：http://qg.bookmarksfly.cn

Java: System.getenv("HOME")
来源：http://xo.szxytkj.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://rk.nicolike.cn

Ruby: ENV["HOME"]
来源：http://xn.newstarts.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://oc.szxytkj.cn

[M03] 执行外部命令
来源：http://er.huixiangedu.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://cx.huixiangedu.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mu.muxihuayi.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://sv.szxytkj.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://sl.newstarts.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://uv.newstarts.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://lg.jianghongdianzi.cn

Ruby: system("ls -l");  `ls -l`
来源：http://al.huixinmuqiang.cn

C#:   Process.Start("ls", "-l");
来源：http://bz.yuexingan06.cn

[M04] 获取当前工作目录
来源：http://pr.haigaiapp.cn

Py:   os.getcwd()
来源：http://eo.nicolike.cn

PHP:  getcwd();
来源：http://gn.colortex.cn

JS:   process.cwd()
来源：http://ru.colortex.cn

TS:   process.cwd()
来源：http://cs.yuexingan06.cn

Java: Path.of("").toAbsolutePath()
来源：http://xq.hnjuh.cn

Go:   os.Getwd()
来源：http://px.lnxyls.cn

Ruby: Dir.pwd
来源：http://sa.szsharing.cn

C#:   Directory.GetCurrentDirectory()
来源：http://cg.asd995.cn

[M05] 设置退出码
来源：http://fv.9csxet.cn

Py:   sys.exit(1)
来源：http://bk.hahajie.cn

PHP:  exit(1);
来源：http://ju.jianghongdianzi.cn

JS:   process.exit(1)
来源：http://tt.shxzskj.cn

TS:   process.exit(1)
来源：http://xr.shtwfgs.cn

Java: System.exit(1)
来源：http://pc.colortex.cn

Go:   os.Exit(1)
来源：http://cr.huixinmuqiang.cn

Ruby: exit 1
来源：http://dg.yuexingan06.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hh.jianghongdianzi.cn

[M06] 向标准错误输出
来源：http://es.jctech888.com.cn

Py:   print("err", file=sys.stderr)
来源：http://db.muxihuayi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ea.colortex.cn

JS:   console.error("err")
来源：http://os.shxzukj.cn

TS:   console.error("err")
来源：http://bg.szxytkj.cn

Java: System.err.println("err")
来源：http://pm.colortex.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://av.colortex.cn

Ruby: warn "err"
来源：http://gr.yuntaijiaju.cn

C#:   Console.Error.WriteLine("err")
来源：http://qv.shxzukj.cn

[M07] 判断是否为主入口
来源：http://sd.haigaiapp.cn

Py:   if __name__ == "__main__":
来源：http://kk.shtwfgs.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ul.hnjuh.cn

JS:   require.main === module
来源：http://zq.yuntaijiaju.cn

TS:   require.main === module
来源：http://vx.szsharing.cn

Java: public static void main(String[] args)
来源：http://gb.panjiajie.cn

Go:   func main()
来源：http://at.jctech888.com.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://so.asd995.cn

C#:   static void Main(string[] args)
来源：http://tg.shxzskj.cn

[M08] 获取系统与运行时信息
来源：http://kh.nszjky.cn

Py:   platform.system();  platform.python_version()
来源：http://ml.bjjhwx.cn

PHP:  PHP_OS;  phpversion();
来源：http://pr.shtwfgs.cn

JS:   process.platform;  process.version
来源：http://di.yuexingan06.cn

TS:   process.platform;  process.version
来源：http://qe.shxzukj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://am.9csxet.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://mp.wgjwhj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://kr.panjiajie.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://vw.lnxyls.cn

================================================================================
来源：http://vv.szsharing.cn

N. 数据结构与算法
来源：http://de.521024.cn

================================================================================
来源：http://lu.huixiangedu.cn

[N01] 二分查找（有序数组）
来源：http://ls.yuexingan06.cn

Py:   bisect.bisect_left(arr, x)
来源：http://pm.hnjuh.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://qd.huanxung.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hm.jianghongdianzi.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dn.asd995.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ir.hahajie.cn

Go:   sort.SearchInts(arr, x)
来源：http://sd.shtwfgs.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://xy.yuntaijiaju.cn

C#:   Array.BinarySearch(arr, x)
来源：http://du.panjiajie.cn

[N02] 排序（工程实践用内置实现）
来源：http://mj.lnxyls.cn

Py:   sorted(arr);  arr.sort()
来源：http://dz.colortex.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ar.lnxyls.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://sw.szxytkj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://zg.hahajie.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://dg.nicolike.cn

Go:   slices.Sort(arr)
来源：http://yh.wgjwhj.cn

Ruby: arr.sort
来源：http://hx.wgjwhj.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://bu.jctech888.com.cn

[N03] 快速排序（分治示例）
来源：http://zs.huanxung.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ua.521024.cn

PHP:  // 递归实现，或用 usort
来源：http://iw.521024.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fc.jctech888.com.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xv.newstarts.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://rp.nicolike.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wx.hahajie.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ph.huixiangedu.cn

C#:   // 手写递归，或 Array.Sort
来源：http://qv.panjiajie.cn

[N04] 斐波那契数列
来源：http://vk.muxihuayi.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://tl.huanxung.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://nb.gzmigu.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mb.newstarts.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://to.bookmarksfly.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ag.jctech888.com.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://pf.muxihuayi.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://bl.jianghongdianzi.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://oa.szxytkj.cn

[N05] 最大公约数
来源：http://aa.colortex.cn

Py:   math.gcd(a, b)
来源：http://ce.asd995.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mb.shtwfgs.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://re.muxihuayi.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nq.szsharing.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zd.shxzukj.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://zy.huanxung.cn

Ruby: a.gcd(b)
来源：http://wu.nszjky.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://xz.newstarts.cn

[N06] 判断回文字符串
来源：http://di.jianghongdianzi.cn

Py:   s == s[::-1]
来源：http://mj.shxzukj.cn

PHP:  $s === strrev($s);
来源：http://cl.panjiajie.cn

JS:   s === [...s].reverse().join("")
来源：http://yi.colortex.cn

TS:   s === [...s].reverse().join("")
来源：http://jx.huanxung.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://tm.lnxyls.cn

Go:   // 双指针从两端比较
来源：http://fz.lnxyls.cn

Ruby: s == s.reverse
来源：http://zt.gzmigu.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://nu.hnjuh.cn

[N07] 两数之和（返回下标）
来源：http://tv.shxzskj.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://im.wgjwhj.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ak.shxzskj.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://qa.haigaiapp.cn

TS:   // 手写 Map<string, number>
来源：http://ok.shtwfgs.cn

Java: // 手写 HashMap
来源：http://yk.bookmarksfly.cn

Go:   // 手写 map[int]int
来源：http://ue.newstarts.cn

Ruby: // 手写 Hash
来源：http://fl.hnjuh.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ba.yuntaijiaju.cn

[N08] 生成全排列
来源：http://gh.huanxung.cn

Py:   itertools.permutations(arr)
来源：http://ht.yuntaijiaju.cn

PHP:  // 手写递归交换
来源：http://xe.haigaiapp.cn

JS:   // 手写回溯递归
来源：http://nr.muxihuayi.cn

TS:   // 手写回溯递归
来源：http://jy.haigaiapp.cn

Java: // 手写回溯递归
来源：http://ng.nicolike.cn

Go:   // 手写回溯递归
来源：http://us.huanxung.cn

Ruby: arr.permutation.to_a
来源：http://ir.9csxet.cn

C#:   // 手写回溯递归
来源：http://ml.szsharing.cn

[N09] 栈与队列
来源：http://ps.bjjhwx.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://tn.panjiajie.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ye.colortex.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wj.huanxung.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://zp.bjjhwx.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://nm.nicolike.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://fj.colortex.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wq.bookmarksfly.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://qw.lnxyls.cn

[N10] 链表节点定义
来源：http://qz.gzmigu.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://yw.shxzskj.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://bu.huixinmuqiang.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://us.shxzskj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://tk.shxzukj.cn

Java: class Node { int v; Node next; }
来源：http://me.9csxet.cn

Go:   type Node struct { V int; Next *Node }
来源：http://fy.huanxung.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ar.huixinmuqiang.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://cp.panjiajie.cn

[N11] 二叉树中序遍历
来源：http://kg.shxzskj.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://av.shtwfgs.cn

PHP:  // 手写递归函数
来源：http://ic.szsharing.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ql.gzmigu.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xb.jctech888.com.cn

Java: // 手写递归
来源：http://ms.yuntaijiaju.cn

Go:   // 手写递归
来源：http://vb.nicolike.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://jz.colortex.cn

C#:   // 手写递归
来源：http://ne.nicolike.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://tu.hnjuh.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ky.hnjuh.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://rn.hnjuh.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xs.huixiangedu.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zs.huanxung.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mk.huixiangedu.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://bo.lnxyls.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://eu.9csxet.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://xp.shxzukj.cn

================================================================================
来源：http://oo.szxytkj.cn

O. 并发与异步
来源：http://ek.521024.cn

================================================================================
来源：http://oh.shxzukj.cn

[O01] 启动一个线程
来源：http://cn.jianghongdianzi.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://uq.hnjuh.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://er.shxzskj.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://rd.9csxet.cn

TS:   // 同 JS
来源：http://fs.asd995.cn

Java: new Thread(() -> f()).start()
来源：http://gs.huixiangedu.cn

Go:   go f()
来源：http://ra.newstarts.cn

Ruby: Thread.new { f }
来源：http://hs.hnjuh.cn

C#:   Task.Run(() => F());
来源：http://im.yuntaijiaju.cn

[O02] 使用线程池
来源：http://wb.bjjhwx.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://fp.bookmarksfly.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://pv.bookmarksfly.cn

JS:   // worker_threads 线程池
来源：http://hq.jianghongdianzi.cn

TS:   // worker_threads 线程池
来源：http://ey.yuexingan06.cn

Java: Executors.newFixedThreadPool(4)
来源：http://mz.colortex.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ly.chemitech.net.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://fl.nicolike.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://lp.gzmigu.cn

[O03] 加锁保护共享数据
来源：http://vx.bjjhwx.cn

Py:   with lock: shared += 1
来源：http://om.9csxet.cn

PHP:  // 用 flock() 做文件锁
来源：http://hn.lnxyls.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://zp.yuexingan06.cn

TS:   // 同 JS
来源：http://ta.szsharing.cn

Java: synchronized (this) { shared++; }
来源：http://yc.huixiangedu.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://yj.jianghongdianzi.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://bh.chemitech.net.cn

C#:   lock (gate) { shared++; }
来源：http://oe.hnjuh.cn

[O04] 定义异步函数并等待
来源：http://pf.bjjhwx.cn

Py:   async def f():⏎    await g()
来源：http://lc.hahajie.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://rq.521024.cn

JS:   async function f() { await g(); }
来源：http://np.asd995.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ex.hnjuh.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://rj.hnjuh.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mj.szsharing.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ny.huanxung.cn

C#:   async Task F() { await G(); }
来源：http://zg.jctech888.com.cn

[O05] 并发执行并等待全部完成
来源：http://oi.hahajie.cn

Py:   asyncio.gather(*tasks)
来源：http://cn.9csxet.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://zg.hnjuh.cn

JS:   await Promise.all(tasks)
来源：http://dy.bookmarksfly.cn

TS:   await Promise.all(tasks)
来源：http://qe.huixiangedu.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://kc.yuexingan06.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://id.521024.cn

Ruby: threads.map(&:join)
来源：http://ck.bookmarksfly.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://li.huixiangedu.cn


<!-- 参考信息 -->