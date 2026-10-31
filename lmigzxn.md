代发 wailian999

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://cb.jctech888.com.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ez.huanxung.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ls.chemitech.net.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://qt.gzmigu.cn

[L03] 设置自定义请求头
来源：http://fv.newstarts.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://se.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ro.jctech888.com.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mi.bookmarksfly.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://si.nszjky.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://tw.hahajie.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jg.panjiajie.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://aj.huanxung.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jh.huixiangedu.cn

[L04] 设置超时
来源：http://hg.colortex.cn

Py:   requests.get(url, timeout=5)
来源：http://pc.hnjuh.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://rv.szsharing.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gp.haigaiapp.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tz.lnxyls.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://on.hnjuh.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ez.shtwfgs.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ad.huanxung.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://kt.newstarts.cn

[L05] 上传文件（multipart）
来源：http://qa.bookmarksfly.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://iu.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://fy.chemitech.net.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://np.shxzskj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://yy.lnxyls.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://sa.hahajie.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ul.jianghongdianzi.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://tw.jctech888.com.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://uc.huanxung.cn

[L06] 解析响应为 JSON
来源：http://vw.chemitech.net.cn

Py:   resp.json()
来源：http://er.shxzukj.cn

PHP:  json_decode($body, true);
来源：http://vx.colortex.cn

JS:   await resp.json()
来源：http://bk.shxzukj.cn

TS:   await resp.json()
来源：http://bl.yuexingan06.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://jg.shxzskj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://io.bjjhwx.cn

Ruby: JSON.parse(resp.body)
来源：http://ij.huixinmuqiang.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://jq.jianghongdianzi.cn

[L07] 处理 HTTP 状态码
来源：http://sj.hnjuh.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ry.hnjuh.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hc.shxzskj.cn

JS:   resp.ok;  resp.status
来源：http://vl.nicolike.cn

TS:   resp.ok;  resp.status
来源：http://vk.nicolike.cn

Java: resp.statusCode()
来源：http://qu.bookmarksfly.cn

Go:   resp.StatusCode
来源：http://ds.521024.cn

Ruby: resp.code.to_i
来源：http://qs.bjjhwx.cn

C#:   (int)resp.StatusCode
来源：http://gk.huixiangedu.cn

[L08] 并发请求多个地址
来源：http://lf.szsharing.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://cp.bjjhwx.cn

PHP:  curl_multi_init() 系列
来源：http://jo.shxzskj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wg.huanxung.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gx.haigaiapp.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ju.9csxet.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://er.bookmarksfly.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://so.szxytkj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://gl.chemitech.net.cn

================================================================================
来源：http://vw.bookmarksfly.cn

M. 命令行 / 进程 / 环境
来源：http://dr.panjiajie.cn

================================================================================
来源：http://rn.hnjuh.cn

[M01] 读取命令行参数
来源：http://jp.huanxung.cn

Py:   sys.argv[1:]
来源：http://bt.szsharing.cn

PHP:  $argv;  $argc;
来源：http://nx.panjiajie.cn

JS:   process.argv.slice(2)
来源：http://mw.szsharing.cn

TS:   process.argv.slice(2)
来源：http://st.hnjuh.cn

Java: args 数组（main 方法参数）
来源：http://dt.huanxung.cn

Go:   os.Args[1:]
来源：http://fp.asd995.cn

Ruby: ARGV
来源：http://ld.shxzukj.cn

C#:   args 数组（Main 方法参数）
来源：http://jb.shtwfgs.cn

[M02] 读取环境变量
来源：http://zd.asd995.cn

Py:   os.environ.get("HOME")
来源：http://ui.hnjuh.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wc.jctech888.com.cn

JS:   process.env.HOME
来源：http://hl.szxytkj.cn

TS:   process.env.HOME
来源：http://cs.jianghongdianzi.cn

Java: System.getenv("HOME")
来源：http://sx.muxihuayi.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mq.huixinmuqiang.cn

Ruby: ENV["HOME"]
来源：http://dq.nicolike.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://cn.gzmigu.cn

[M03] 执行外部命令
来源：http://lk.muxihuayi.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://eu.gzmigu.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://lb.9csxet.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://es.nszjky.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://aa.panjiajie.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://yi.asd995.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ax.huixiangedu.cn

Ruby: system("ls -l");  `ls -l`
来源：http://je.huixiangedu.cn

C#:   Process.Start("ls", "-l");
来源：http://iv.huanxung.cn

[M04] 获取当前工作目录
来源：http://le.haigaiapp.cn

Py:   os.getcwd()
来源：http://kn.wgjwhj.cn

PHP:  getcwd();
来源：http://iq.wgjwhj.cn

JS:   process.cwd()
来源：http://pt.huanxung.cn

TS:   process.cwd()
来源：http://kr.nicolike.cn

Java: Path.of("").toAbsolutePath()
来源：http://kp.shxzskj.cn

Go:   os.Getwd()
来源：http://gx.huixinmuqiang.cn

Ruby: Dir.pwd
来源：http://ze.asd995.cn

C#:   Directory.GetCurrentDirectory()
来源：http://hm.wgjwhj.cn

[M05] 设置退出码
来源：http://rt.yuntaijiaju.cn

Py:   sys.exit(1)
来源：http://qx.lnxyls.cn

PHP:  exit(1);
来源：http://hg.bookmarksfly.cn

JS:   process.exit(1)
来源：http://vs.nszjky.cn

TS:   process.exit(1)
来源：http://kt.nicolike.cn

Java: System.exit(1)
来源：http://aj.jctech888.com.cn

Go:   os.Exit(1)
来源：http://fu.nszjky.cn

Ruby: exit 1
来源：http://su.hahajie.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://jo.gzmigu.cn

[M06] 向标准错误输出
来源：http://gz.hahajie.cn

Py:   print("err", file=sys.stderr)
来源：http://tr.bjjhwx.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://pn.szxytkj.cn

JS:   console.error("err")
来源：http://ln.huanxung.cn

TS:   console.error("err")
来源：http://lp.shxzukj.cn

Java: System.err.println("err")
来源：http://yi.yuntaijiaju.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://lj.chemitech.net.cn

Ruby: warn "err"
来源：http://wo.yuntaijiaju.cn

C#:   Console.Error.WriteLine("err")
来源：http://ez.gzmigu.cn

[M07] 判断是否为主入口
来源：http://ou.9csxet.cn

Py:   if __name__ == "__main__":
来源：http://cc.panjiajie.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://yn.szxytkj.cn

JS:   require.main === module
来源：http://ya.9csxet.cn

TS:   require.main === module
来源：http://lj.jctech888.com.cn

Java: public static void main(String[] args)
来源：http://qc.jianghongdianzi.cn

Go:   func main()
来源：http://en.muxihuayi.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://xx.asd995.cn

C#:   static void Main(string[] args)
来源：http://hy.shxzukj.cn

[M08] 获取系统与运行时信息
来源：http://jw.asd995.cn

Py:   platform.system();  platform.python_version()
来源：http://kp.muxihuayi.cn

PHP:  PHP_OS;  phpversion();
来源：http://az.lnxyls.cn

JS:   process.platform;  process.version
来源：http://vt.haigaiapp.cn

TS:   process.platform;  process.version
来源：http://rq.nicolike.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hd.bjjhwx.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://rx.colortex.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://go.szxytkj.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ec.hnjuh.cn

================================================================================
来源：http://wg.huanxung.cn

N. 数据结构与算法
来源：http://hy.jctech888.com.cn

================================================================================
来源：http://yv.gzmigu.cn

[N01] 二分查找（有序数组）
来源：http://yp.nicolike.cn

Py:   bisect.bisect_left(arr, x)
来源：http://jr.9csxet.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mm.shtwfgs.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gx.asd995.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://am.szxytkj.cn

Java: Arrays.binarySearch(arr, x)
来源：http://sd.muxihuayi.cn

Go:   sort.SearchInts(arr, x)
来源：http://vq.hnjuh.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://hx.muxihuayi.cn

C#:   Array.BinarySearch(arr, x)
来源：http://zt.huanxung.cn

[N02] 排序（工程实践用内置实现）
来源：http://xy.521024.cn

Py:   sorted(arr);  arr.sort()
来源：http://sg.521024.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hn.521024.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://by.newstarts.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://cq.huixiangedu.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://xc.hnjuh.cn

Go:   slices.Sort(arr)
来源：http://ws.9csxet.cn

Ruby: arr.sort
来源：http://bi.yuntaijiaju.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://pl.asd995.cn

[N03] 快速排序（分治示例）
来源：http://yn.hahajie.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://je.chemitech.net.cn

PHP:  // 递归实现，或用 usort
来源：http://nc.jianghongdianzi.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ii.szxytkj.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ze.nicolike.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://tu.huanxung.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://dw.chemitech.net.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hq.shtwfgs.cn

C#:   // 手写递归，或 Array.Sort
来源：http://xz.lnxyls.cn

[N04] 斐波那契数列
来源：http://ah.szsharing.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://va.bookmarksfly.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hf.bookmarksfly.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ie.yuexingan06.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ie.lnxyls.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://iq.jctech888.com.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://oq.bookmarksfly.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://eh.shxzskj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://qo.chemitech.net.cn

[N05] 最大公约数
来源：http://lf.haigaiapp.cn

Py:   math.gcd(a, b)
来源：http://jj.nszjky.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hd.hahajie.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ri.huixiangedu.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tw.hnjuh.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wq.521024.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hw.haigaiapp.cn

Ruby: a.gcd(b)
来源：http://hp.9csxet.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://te.bjjhwx.cn

[N06] 判断回文字符串
来源：http://ck.bookmarksfly.cn

Py:   s == s[::-1]
来源：http://vd.bjjhwx.cn

PHP:  $s === strrev($s);
来源：http://tr.nszjky.cn

JS:   s === [...s].reverse().join("")
来源：http://ei.panjiajie.cn

TS:   s === [...s].reverse().join("")
来源：http://xp.huanxung.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://fw.nicolike.cn

Go:   // 双指针从两端比较
来源：http://mt.newstarts.cn

Ruby: s == s.reverse
来源：http://tp.huanxung.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://pj.9csxet.cn

[N07] 两数之和（返回下标）
来源：http://mp.asd995.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://xm.colortex.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://bo.nszjky.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://sk.hnjuh.cn

TS:   // 手写 Map<string, number>
来源：http://rh.yuexingan06.cn

Java: // 手写 HashMap
来源：http://if.jianghongdianzi.cn

Go:   // 手写 map[int]int
来源：http://kn.szsharing.cn

Ruby: // 手写 Hash
来源：http://hy.521024.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ib.9csxet.cn

[N08] 生成全排列
来源：http://lq.bookmarksfly.cn

Py:   itertools.permutations(arr)
来源：http://lb.shtwfgs.cn

PHP:  // 手写递归交换
来源：http://ge.nszjky.cn

JS:   // 手写回溯递归
来源：http://bz.huanxung.cn

TS:   // 手写回溯递归
来源：http://kj.newstarts.cn

Java: // 手写回溯递归
来源：http://ix.huixinmuqiang.cn

Go:   // 手写回溯递归
来源：http://dg.hnjuh.cn

Ruby: arr.permutation.to_a
来源：http://pp.panjiajie.cn

C#:   // 手写回溯递归
来源：http://ns.panjiajie.cn

[N09] 栈与队列
来源：http://as.panjiajie.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://rb.yuexingan06.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ty.9csxet.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://kp.521024.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mh.jctech888.com.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ah.shxzukj.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ez.hnjuh.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://jc.shxzukj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ty.chemitech.net.cn

[N10] 链表节点定义
来源：http://px.bookmarksfly.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ln.hnjuh.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://kj.bookmarksfly.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://vi.chemitech.net.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://dz.9csxet.cn

Java: class Node { int v; Node next; }
来源：http://ts.szxytkj.cn

Go:   type Node struct { V int; Next *Node }
来源：http://cg.nicolike.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ly.asd995.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://um.chemitech.net.cn

[N11] 二叉树中序遍历
来源：http://uc.wgjwhj.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wb.newstarts.cn

PHP:  // 手写递归函数
来源：http://dy.colortex.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vy.colortex.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tr.shxzukj.cn

Java: // 手写递归
来源：http://mv.asd995.cn

Go:   // 手写递归
来源：http://yf.szxytkj.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ss.muxihuayi.cn

C#:   // 手写递归
来源：http://lk.jctech888.com.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://bt.szsharing.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ks.huixinmuqiang.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://dr.colortex.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://es.colortex.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pm.jctech888.com.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://lc.chemitech.net.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://bs.huixiangedu.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://le.lnxyls.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://qm.shxzskj.cn

================================================================================
来源：http://sd.yuntaijiaju.cn

O. 并发与异步
来源：http://zz.jianghongdianzi.cn

================================================================================
来源：http://pw.hahajie.cn

[O01] 启动一个线程
来源：http://ze.muxihuayi.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://sx.muxihuayi.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mi.yuexingan06.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ry.panjiajie.cn

TS:   // 同 JS
来源：http://nc.panjiajie.cn

Java: new Thread(() -> f()).start()
来源：http://kf.muxihuayi.cn

Go:   go f()
来源：http://gr.gzmigu.cn

Ruby: Thread.new { f }
来源：http://gs.szsharing.cn

C#:   Task.Run(() => F());
来源：http://jm.huixiangedu.cn

[O02] 使用线程池
来源：http://mu.newstarts.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hj.colortex.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://nq.bookmarksfly.cn

JS:   // worker_threads 线程池
来源：http://fh.nszjky.cn

TS:   // worker_threads 线程池
来源：http://bg.szsharing.cn

Java: Executors.newFixedThreadPool(4)
来源：http://og.jianghongdianzi.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://gz.shtwfgs.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://nd.shxzskj.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://py.bjjhwx.cn

[O03] 加锁保护共享数据
来源：http://xx.huanxung.cn

Py:   with lock: shared += 1
来源：http://qy.bjjhwx.cn

PHP:  // 用 flock() 做文件锁
来源：http://ye.yuexingan06.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://cg.nicolike.cn

TS:   // 同 JS
来源：http://wl.newstarts.cn

Java: synchronized (this) { shared++; }
来源：http://mz.yuexingan06.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wh.nszjky.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://yn.jctech888.com.cn

C#:   lock (gate) { shared++; }
来源：http://vz.9csxet.cn

[O04] 定义异步函数并等待
来源：http://im.jianghongdianzi.cn

Py:   async def f():⏎    await g()
来源：http://eh.chemitech.net.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://fe.asd995.cn

JS:   async function f() { await g(); }
来源：http://wn.huanxung.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://by.huixiangedu.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://bd.colortex.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ct.jctech888.com.cn

Ruby: # 用 Fiber 或 async gem
来源：http://xs.nszjky.cn

C#:   async Task F() { await G(); }
来源：http://qs.shxzskj.cn

[O05] 并发执行并等待全部完成
来源：http://in.panjiajie.cn

Py:   asyncio.gather(*tasks)
来源：http://ly.shxzukj.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://lm.hnjuh.cn

JS:   await Promise.all(tasks)
来源：http://id.gzmigu.cn

TS:   await Promise.all(tasks)
来源：http://tk.gzmigu.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://cu.panjiajie.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://st.yuexingan06.cn

Ruby: threads.map(&:join)
来源：http://yw.shtwfgs.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ur.521024.cn

[O06] 使用进程池
来源：http://vp.jctech888.com.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://cb.panjiajie.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://bk.hnjuh.cn

JS:   // child_process / cluster 模块
来源：http://el.shtwfgs.cn

TS:   // child_process / cluster 模块
来源：http://lt.szsharing.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://uh.hnjuh.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://lr.hahajie.cn

Ruby: // fork 块
来源：http://vb.9csxet.cn


<!-- 参考信息 -->