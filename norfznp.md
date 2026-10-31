代发 wailian999

Go:   resp, err := http.Get(url)
来源：http://dr.chemitech.net.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://je.panjiajie.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://fl.hahajie.cn

[L02] 发送 POST JSON
来源：http://ob.panjiajie.cn

Py:   requests.post(url, json={"a": 1})
来源：http://yx.panjiajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://nd.szxytkj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sy.hnjuh.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kf.hnjuh.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vz.muxihuayi.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://bm.huanxung.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ra.shxzukj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://df.szxytkj.cn

[L03] 设置自定义请求头
来源：http://sr.jianghongdianzi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://nc.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://fe.huixiangedu.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://df.yuexingan06.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pl.newstarts.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://gk.shtwfgs.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mz.szsharing.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://sg.bjjhwx.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ys.shxzskj.cn

[L04] 设置超时
来源：http://ur.szxytkj.cn

Py:   requests.get(url, timeout=5)
来源：http://og.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xf.panjiajie.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tk.yuntaijiaju.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vq.9csxet.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://xk.muxihuayi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://jy.jianghongdianzi.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://qb.bjjhwx.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://im.chemitech.net.cn

[L05] 上传文件（multipart）
来源：http://nd.wgjwhj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://dr.szsharing.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://os.asd995.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://zo.szsharing.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://un.gzmigu.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://jl.shtwfgs.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://qn.yuexingan06.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://bh.panjiajie.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://iv.shxzskj.cn

[L06] 解析响应为 JSON
来源：http://ud.szsharing.cn

Py:   resp.json()
来源：http://kc.gzmigu.cn

PHP:  json_decode($body, true);
来源：http://bw.jianghongdianzi.cn

JS:   await resp.json()
来源：http://az.haigaiapp.cn

TS:   await resp.json()
来源：http://nu.bookmarksfly.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://rw.muxihuayi.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://gp.jctech888.com.cn

Ruby: JSON.parse(resp.body)
来源：http://uf.wgjwhj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wg.huixiangedu.cn

[L07] 处理 HTTP 状态码
来源：http://wk.gzmigu.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://or.yuexingan06.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://zq.muxihuayi.cn

JS:   resp.ok;  resp.status
来源：http://qs.huixiangedu.cn

TS:   resp.ok;  resp.status
来源：http://fn.lnxyls.cn

Java: resp.statusCode()
来源：http://xc.bookmarksfly.cn

Go:   resp.StatusCode
来源：http://yk.shxzukj.cn

Ruby: resp.code.to_i
来源：http://vn.shtwfgs.cn

C#:   (int)resp.StatusCode
来源：http://oz.haigaiapp.cn

[L08] 并发请求多个地址
来源：http://ex.hahajie.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://uf.asd995.cn

PHP:  curl_multi_init() 系列
来源：http://jg.shxzskj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jw.szxytkj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://me.szsharing.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mw.haigaiapp.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://zv.nicolike.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hd.asd995.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://zs.hahajie.cn

================================================================================
来源：http://jc.haigaiapp.cn

M. 命令行 / 进程 / 环境
来源：http://ir.521024.cn

================================================================================
来源：http://ao.muxihuayi.cn

[M01] 读取命令行参数
来源：http://kb.gzmigu.cn

Py:   sys.argv[1:]
来源：http://kd.hahajie.cn

PHP:  $argv;  $argc;
来源：http://en.bookmarksfly.cn

JS:   process.argv.slice(2)
来源：http://gq.yuntaijiaju.cn

TS:   process.argv.slice(2)
来源：http://nv.muxihuayi.cn

Java: args 数组（main 方法参数）
来源：http://nw.jianghongdianzi.cn

Go:   os.Args[1:]
来源：http://nc.lnxyls.cn

Ruby: ARGV
来源：http://qn.panjiajie.cn

C#:   args 数组（Main 方法参数）
来源：http://qm.lnxyls.cn

[M02] 读取环境变量
来源：http://es.newstarts.cn

Py:   os.environ.get("HOME")
来源：http://gb.huixiangedu.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hb.newstarts.cn

JS:   process.env.HOME
来源：http://dd.wgjwhj.cn

TS:   process.env.HOME
来源：http://en.asd995.cn

Java: System.getenv("HOME")
来源：http://qi.huixiangedu.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://pi.panjiajie.cn

Ruby: ENV["HOME"]
来源：http://tr.szsharing.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ys.szxytkj.cn

[M03] 执行外部命令
来源：http://le.bookmarksfly.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://cm.bjjhwx.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://pj.szsharing.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://xe.huanxung.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://jb.nszjky.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://lt.jianghongdianzi.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ev.hahajie.cn

Ruby: system("ls -l");  `ls -l`
来源：http://fp.muxihuayi.cn

C#:   Process.Start("ls", "-l");
来源：http://or.chemitech.net.cn

[M04] 获取当前工作目录
来源：http://pn.9csxet.cn

Py:   os.getcwd()
来源：http://fw.huixiangedu.cn

PHP:  getcwd();
来源：http://rv.asd995.cn

JS:   process.cwd()
来源：http://vg.shtwfgs.cn

TS:   process.cwd()
来源：http://se.521024.cn

Java: Path.of("").toAbsolutePath()
来源：http://jc.haigaiapp.cn

Go:   os.Getwd()
来源：http://ey.shxzskj.cn

Ruby: Dir.pwd
来源：http://nr.9csxet.cn

C#:   Directory.GetCurrentDirectory()
来源：http://qg.huixiangedu.cn

[M05] 设置退出码
来源：http://dg.yuntaijiaju.cn

Py:   sys.exit(1)
来源：http://yf.bjjhwx.cn

PHP:  exit(1);
来源：http://ia.hahajie.cn

JS:   process.exit(1)
来源：http://xy.yuexingan06.cn

TS:   process.exit(1)
来源：http://nz.asd995.cn

Java: System.exit(1)
来源：http://qz.yuexingan06.cn

Go:   os.Exit(1)
来源：http://ho.wgjwhj.cn

Ruby: exit 1
来源：http://bi.panjiajie.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://jh.muxihuayi.cn

[M06] 向标准错误输出
来源：http://ek.shxzskj.cn

Py:   print("err", file=sys.stderr)
来源：http://jp.9csxet.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://yj.hnjuh.cn

JS:   console.error("err")
来源：http://sn.newstarts.cn

TS:   console.error("err")
来源：http://nb.shxzukj.cn

Java: System.err.println("err")
来源：http://xl.asd995.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ca.huanxung.cn

Ruby: warn "err"
来源：http://av.shtwfgs.cn

C#:   Console.Error.WriteLine("err")
来源：http://in.jctech888.com.cn

[M07] 判断是否为主入口
来源：http://lz.jctech888.com.cn

Py:   if __name__ == "__main__":
来源：http://pj.yuexingan06.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ne.chemitech.net.cn

JS:   require.main === module
来源：http://km.yuexingan06.cn

TS:   require.main === module
来源：http://sy.gzmigu.cn

Java: public static void main(String[] args)
来源：http://kx.9csxet.cn

Go:   func main()
来源：http://ci.9csxet.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ya.chemitech.net.cn

C#:   static void Main(string[] args)
来源：http://vc.hnjuh.cn

[M08] 获取系统与运行时信息
来源：http://mv.yuntaijiaju.cn

Py:   platform.system();  platform.python_version()
来源：http://ro.yuexingan06.cn

PHP:  PHP_OS;  phpversion();
来源：http://ju.9csxet.cn

JS:   process.platform;  process.version
来源：http://nu.huixiangedu.cn

TS:   process.platform;  process.version
来源：http://np.szsharing.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://vn.haigaiapp.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://va.nszjky.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wq.szsharing.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://sr.jianghongdianzi.cn

================================================================================
来源：http://mj.lnxyls.cn

N. 数据结构与算法
来源：http://zr.huixinmuqiang.cn

================================================================================
来源：http://gk.nszjky.cn

[N01] 二分查找（有序数组）
来源：http://zi.huanxung.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ze.asd995.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mn.yuntaijiaju.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dv.gzmigu.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kl.hahajie.cn

Java: Arrays.binarySearch(arr, x)
来源：http://dr.asd995.cn

Go:   sort.SearchInts(arr, x)
来源：http://ml.huanxung.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://xf.huanxung.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ut.asd995.cn

[N02] 排序（工程实践用内置实现）
来源：http://av.huanxung.cn

Py:   sorted(arr);  arr.sort()
来源：http://js.nicolike.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://jz.szxytkj.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://du.yuntaijiaju.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://yc.jctech888.com.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://cf.colortex.cn

Go:   slices.Sort(arr)
来源：http://oq.nicolike.cn

Ruby: arr.sort
来源：http://re.jctech888.com.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ip.panjiajie.cn

[N03] 快速排序（分治示例）
来源：http://ho.wgjwhj.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://sr.szsharing.cn

PHP:  // 递归实现，或用 usort
来源：http://zw.bjjhwx.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gh.shxzskj.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kq.asd995.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://tz.9csxet.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://if.9csxet.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://yc.huixinmuqiang.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ax.gzmigu.cn

[N04] 斐波那契数列
来源：http://hp.huixiangedu.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://vd.szxytkj.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://do.muxihuayi.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lu.yuntaijiaju.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pq.haigaiapp.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://cv.hnjuh.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://zx.szsharing.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://tc.shxzukj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://fb.lnxyls.cn

[N05] 最大公约数
来源：http://mx.panjiajie.cn

Py:   math.gcd(a, b)
来源：http://rf.shxzskj.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ju.muxihuayi.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://px.huixinmuqiang.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cf.shxzukj.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mo.shxzukj.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://fu.panjiajie.cn

Ruby: a.gcd(b)
来源：http://lm.bookmarksfly.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://os.gzmigu.cn

[N06] 判断回文字符串
来源：http://bb.panjiajie.cn

Py:   s == s[::-1]
来源：http://vh.yuexingan06.cn

PHP:  $s === strrev($s);
来源：http://jn.bjjhwx.cn

JS:   s === [...s].reverse().join("")
来源：http://tz.szsharing.cn

TS:   s === [...s].reverse().join("")
来源：http://as.gzmigu.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wf.huixinmuqiang.cn

Go:   // 双指针从两端比较
来源：http://fi.9csxet.cn

Ruby: s == s.reverse
来源：http://bt.haigaiapp.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://je.colortex.cn

[N07] 两数之和（返回下标）
来源：http://aa.asd995.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ik.nszjky.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://dy.shtwfgs.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://wt.yuntaijiaju.cn

TS:   // 手写 Map<string, number>
来源：http://st.muxihuayi.cn

Java: // 手写 HashMap
来源：http://cf.521024.cn

Go:   // 手写 map[int]int
来源：http://kn.bookmarksfly.cn

Ruby: // 手写 Hash
来源：http://cx.bjjhwx.cn

C#:   // 手写 Dictionary<int, int>
来源：http://vl.521024.cn

[N08] 生成全排列
来源：http://zc.hahajie.cn

Py:   itertools.permutations(arr)
来源：http://fp.shxzskj.cn

PHP:  // 手写递归交换
来源：http://yi.colortex.cn

JS:   // 手写回溯递归
来源：http://ln.wgjwhj.cn

TS:   // 手写回溯递归
来源：http://ez.9csxet.cn

Java: // 手写回溯递归
来源：http://vw.gzmigu.cn

Go:   // 手写回溯递归
来源：http://ds.jctech888.com.cn

Ruby: arr.permutation.to_a
来源：http://ww.521024.cn

C#:   // 手写回溯递归
来源：http://yf.bjjhwx.cn

[N09] 栈与队列
来源：http://xm.bjjhwx.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://qi.yuntaijiaju.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://gv.9csxet.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://gn.yuntaijiaju.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wz.9csxet.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://bw.szsharing.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://sa.lnxyls.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://cz.bookmarksfly.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://md.hnjuh.cn

[N10] 链表节点定义
来源：http://kp.shxzskj.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://nf.jctech888.com.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://pp.colortex.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://uk.shxzskj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://tz.hnjuh.cn

Java: class Node { int v; Node next; }
来源：http://hh.haigaiapp.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ya.asd995.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://hm.szxytkj.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://jj.nszjky.cn

[N11] 二叉树中序遍历
来源：http://gs.huanxung.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://na.shxzskj.cn

PHP:  // 手写递归函数
来源：http://th.nicolike.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lp.shtwfgs.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gd.gzmigu.cn

Java: // 手写递归
来源：http://ct.szsharing.cn

Go:   // 手写递归
来源：http://ci.panjiajie.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ky.lnxyls.cn

C#:   // 手写递归
来源：http://hx.bjjhwx.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://rm.szsharing.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wn.shxzukj.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://bc.muxihuayi.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vw.chemitech.net.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sr.lnxyls.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hf.muxihuayi.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://jv.hnjuh.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wf.huixinmuqiang.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://lg.9csxet.cn

================================================================================
来源：http://gk.panjiajie.cn

O. 并发与异步
来源：http://rk.huixiangedu.cn

================================================================================
来源：http://zt.hahajie.cn

[O01] 启动一个线程
来源：http://es.hahajie.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://oy.hahajie.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://sk.yuntaijiaju.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://gi.wgjwhj.cn

TS:   // 同 JS
来源：http://eh.huanxung.cn

Java: new Thread(() -> f()).start()
来源：http://hw.shtwfgs.cn

Go:   go f()
来源：http://cu.chemitech.net.cn

Ruby: Thread.new { f }
来源：http://yc.shxzskj.cn

C#:   Task.Run(() => F());
来源：http://jw.gzmigu.cn

[O02] 使用线程池
来源：http://hi.9csxet.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://yw.muxihuayi.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://vq.shtwfgs.cn

JS:   // worker_threads 线程池
来源：http://xs.shxzukj.cn

TS:   // worker_threads 线程池
来源：http://kn.haigaiapp.cn

Java: Executors.newFixedThreadPool(4)
来源：http://zq.9csxet.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://bw.colortex.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://na.shxzskj.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ph.huanxung.cn

[O03] 加锁保护共享数据
来源：http://bs.newstarts.cn

Py:   with lock: shared += 1
来源：http://eh.haigaiapp.cn

PHP:  // 用 flock() 做文件锁
来源：http://ed.panjiajie.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://dh.huanxung.cn

TS:   // 同 JS
来源：http://ae.szsharing.cn

Java: synchronized (this) { shared++; }
来源：http://xt.jianghongdianzi.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ee.shxzskj.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://bs.chemitech.net.cn

C#:   lock (gate) { shared++; }
来源：http://iu.hnjuh.cn

[O04] 定义异步函数并等待
来源：http://of.muxihuayi.cn

Py:   async def f():⏎    await g()
来源：http://pc.hnjuh.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://fw.huanxung.cn

JS:   async function f() { await g(); }
来源：http://fq.lnxyls.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://hv.yuntaijiaju.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://cs.gzmigu.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://da.shtwfgs.cn

Ruby: # 用 Fiber 或 async gem
来源：http://jq.nszjky.cn

C#:   async Task F() { await G(); }
来源：http://dp.hnjuh.cn

[O05] 并发执行并等待全部完成
来源：http://mc.yuexingan06.cn

Py:   asyncio.gather(*tasks)
来源：http://ui.hnjuh.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://we.muxihuayi.cn

JS:   await Promise.all(tasks)
来源：http://up.shtwfgs.cn

TS:   await Promise.all(tasks)
来源：http://uu.huixinmuqiang.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://go.haigaiapp.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://sh.hahajie.cn

Ruby: threads.map(&:join)
来源：http://qn.shxzukj.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://jj.9csxet.cn


<!-- 参考信息 -->