代发 wailian999

Py:   requests.post(url, json={"a": 1})
来源：http://gp.huixiangedu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wi.lnxyls.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ue.bjjhwx.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ms.shtwfgs.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://kl.nszjky.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://kt.haigaiapp.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://zn.asd995.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ne.nszjky.cn

[L03] 设置自定义请求头
来源：http://nd.521024.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ch.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://zo.nicolike.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ju.yuexingan06.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kc.szxytkj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wo.bjjhwx.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hb.yuexingan06.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ne.shxzskj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://of.yuexingan06.cn

[L04] 设置超时
来源：http://qa.jctech888.com.cn

Py:   requests.get(url, timeout=5)
来源：http://sj.panjiajie.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://jd.huanxung.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nv.hnjuh.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bq.wgjwhj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://et.huixiangedu.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mi.bookmarksfly.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hd.hahajie.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://pl.nicolike.cn

[L05] 上传文件（multipart）
来源：http://lz.lnxyls.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hw.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://oj.wgjwhj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qe.huixiangedu.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://pq.hnjuh.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://zp.asd995.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://rp.colortex.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ff.huixiangedu.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://sf.huixinmuqiang.cn

[L06] 解析响应为 JSON
来源：http://lo.hnjuh.cn

Py:   resp.json()
来源：http://uj.nszjky.cn

PHP:  json_decode($body, true);
来源：http://zk.panjiajie.cn

JS:   await resp.json()
来源：http://am.9csxet.cn

TS:   await resp.json()
来源：http://bd.huixinmuqiang.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://qg.szsharing.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ad.chemitech.net.cn

Ruby: JSON.parse(resp.body)
来源：http://of.huixiangedu.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://uj.jctech888.com.cn

[L07] 处理 HTTP 状态码
来源：http://gi.shtwfgs.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://jq.shxzukj.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://em.nszjky.cn

JS:   resp.ok;  resp.status
来源：http://ql.hnjuh.cn

TS:   resp.ok;  resp.status
来源：http://eq.chemitech.net.cn

Java: resp.statusCode()
来源：http://ne.shxzskj.cn

Go:   resp.StatusCode
来源：http://bw.colortex.cn

Ruby: resp.code.to_i
来源：http://tl.jctech888.com.cn

C#:   (int)resp.StatusCode
来源：http://og.521024.cn

[L08] 并发请求多个地址
来源：http://dm.huixiangedu.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://em.shxzukj.cn

PHP:  curl_multi_init() 系列
来源：http://zi.yuexingan06.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cm.shtwfgs.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xy.huanxung.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://lr.muxihuayi.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://yj.wgjwhj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://jd.yuexingan06.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ld.yuntaijiaju.cn

================================================================================
来源：http://mi.nicolike.cn

M. 命令行 / 进程 / 环境
来源：http://rc.shtwfgs.cn

================================================================================
来源：http://tu.nicolike.cn

[M01] 读取命令行参数
来源：http://eo.szxytkj.cn

Py:   sys.argv[1:]
来源：http://wq.asd995.cn

PHP:  $argv;  $argc;
来源：http://pv.colortex.cn

JS:   process.argv.slice(2)
来源：http://sk.hnjuh.cn

TS:   process.argv.slice(2)
来源：http://ah.bookmarksfly.cn

Java: args 数组（main 方法参数）
来源：http://oc.colortex.cn

Go:   os.Args[1:]
来源：http://ti.nicolike.cn

Ruby: ARGV
来源：http://cz.muxihuayi.cn

C#:   args 数组（Main 方法参数）
来源：http://qf.yuntaijiaju.cn

[M02] 读取环境变量
来源：http://dh.chemitech.net.cn

Py:   os.environ.get("HOME")
来源：http://hl.huixinmuqiang.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ky.chemitech.net.cn

JS:   process.env.HOME
来源：http://or.szsharing.cn

TS:   process.env.HOME
来源：http://za.521024.cn

Java: System.getenv("HOME")
来源：http://od.panjiajie.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://sb.gzmigu.cn

Ruby: ENV["HOME"]
来源：http://zf.huixinmuqiang.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://zn.nszjky.cn

[M03] 执行外部命令
来源：http://xe.yuexingan06.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://tb.bookmarksfly.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://kb.shtwfgs.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ms.521024.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://gw.jctech888.com.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ee.huixinmuqiang.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://zp.yuntaijiaju.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ue.wgjwhj.cn

C#:   Process.Start("ls", "-l");
来源：http://up.jctech888.com.cn

[M04] 获取当前工作目录
来源：http://hn.huixiangedu.cn

Py:   os.getcwd()
来源：http://ir.nszjky.cn

PHP:  getcwd();
来源：http://eu.bjjhwx.cn

JS:   process.cwd()
来源：http://zv.shxzskj.cn

TS:   process.cwd()
来源：http://on.huanxung.cn

Java: Path.of("").toAbsolutePath()
来源：http://nj.shtwfgs.cn

Go:   os.Getwd()
来源：http://km.shxzskj.cn

Ruby: Dir.pwd
来源：http://rh.bjjhwx.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ie.nszjky.cn

[M05] 设置退出码
来源：http://xq.gzmigu.cn

Py:   sys.exit(1)
来源：http://hl.asd995.cn

PHP:  exit(1);
来源：http://qf.hnjuh.cn

JS:   process.exit(1)
来源：http://ql.shxzskj.cn

TS:   process.exit(1)
来源：http://uy.muxihuayi.cn

Java: System.exit(1)
来源：http://yl.yuexingan06.cn

Go:   os.Exit(1)
来源：http://lu.panjiajie.cn

Ruby: exit 1
来源：http://qo.colortex.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://tn.asd995.cn

[M06] 向标准错误输出
来源：http://pn.chemitech.net.cn

Py:   print("err", file=sys.stderr)
来源：http://ba.nicolike.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://gg.haigaiapp.cn

JS:   console.error("err")
来源：http://so.shxzskj.cn

TS:   console.error("err")
来源：http://xv.hahajie.cn

Java: System.err.println("err")
来源：http://js.shxzskj.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://tu.szsharing.cn

Ruby: warn "err"
来源：http://uk.muxihuayi.cn

C#:   Console.Error.WriteLine("err")
来源：http://zo.bookmarksfly.cn

[M07] 判断是否为主入口
来源：http://qk.szxytkj.cn

Py:   if __name__ == "__main__":
来源：http://gd.nicolike.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://nb.shxzukj.cn

JS:   require.main === module
来源：http://wl.shxzskj.cn

TS:   require.main === module
来源：http://yz.newstarts.cn

Java: public static void main(String[] args)
来源：http://pr.bookmarksfly.cn

Go:   func main()
来源：http://aw.asd995.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://oa.gzmigu.cn

C#:   static void Main(string[] args)
来源：http://eo.9csxet.cn

[M08] 获取系统与运行时信息
来源：http://nh.jianghongdianzi.cn

Py:   platform.system();  platform.python_version()
来源：http://eq.wgjwhj.cn

PHP:  PHP_OS;  phpversion();
来源：http://ms.yuntaijiaju.cn

JS:   process.platform;  process.version
来源：http://te.hahajie.cn

TS:   process.platform;  process.version
来源：http://lh.jianghongdianzi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://dt.gzmigu.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://cf.nszjky.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ac.wgjwhj.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://pi.hahajie.cn

================================================================================
来源：http://uz.lnxyls.cn

N. 数据结构与算法
来源：http://la.shxzskj.cn

================================================================================
来源：http://fa.wgjwhj.cn

[N01] 二分查找（有序数组）
来源：http://pt.shxzukj.cn

Py:   bisect.bisect_left(arr, x)
来源：http://jz.nszjky.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://at.chemitech.net.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gb.bookmarksfly.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qc.521024.cn

Java: Arrays.binarySearch(arr, x)
来源：http://le.chemitech.net.cn

Go:   sort.SearchInts(arr, x)
来源：http://lp.szxytkj.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://hb.szxytkj.cn

C#:   Array.BinarySearch(arr, x)
来源：http://jc.yuntaijiaju.cn

[N02] 排序（工程实践用内置实现）
来源：http://mc.huixiangedu.cn

Py:   sorted(arr);  arr.sort()
来源：http://kl.shtwfgs.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ak.yuntaijiaju.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ki.shxzukj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://cw.jianghongdianzi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://cs.szxytkj.cn

Go:   slices.Sort(arr)
来源：http://ey.jctech888.com.cn

Ruby: arr.sort
来源：http://wi.nicolike.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://pc.haigaiapp.cn

[N03] 快速排序（分治示例）
来源：http://hz.huixiangedu.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://gp.shxzskj.cn

PHP:  // 递归实现，或用 usort
来源：http://of.colortex.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://at.lnxyls.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bg.nszjky.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://en.colortex.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wo.huanxung.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ou.shxzukj.cn

C#:   // 手写递归，或 Array.Sort
来源：http://yf.hnjuh.cn

[N04] 斐波那契数列
来源：http://of.bookmarksfly.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://aq.shxzskj.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://jb.shxzukj.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yt.asd995.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lo.bookmarksfly.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://fi.colortex.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://kc.colortex.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://kb.huixiangedu.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://qk.newstarts.cn

[N05] 最大公约数
来源：http://ct.huixiangedu.cn

Py:   math.gcd(a, b)
来源：http://dh.gzmigu.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://qn.haigaiapp.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pw.panjiajie.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pk.muxihuayi.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://pw.gzmigu.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://lj.nszjky.cn

Ruby: a.gcd(b)
来源：http://xw.hahajie.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://tu.chemitech.net.cn

[N06] 判断回文字符串
来源：http://ip.nicolike.cn

Py:   s == s[::-1]
来源：http://lr.bookmarksfly.cn

PHP:  $s === strrev($s);
来源：http://bh.szxytkj.cn

JS:   s === [...s].reverse().join("")
来源：http://xh.huanxung.cn

TS:   s === [...s].reverse().join("")
来源：http://lo.huixiangedu.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://eu.521024.cn

Go:   // 双指针从两端比较
来源：http://am.muxihuayi.cn

Ruby: s == s.reverse
来源：http://gs.chemitech.net.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ms.shtwfgs.cn

[N07] 两数之和（返回下标）
来源：http://zp.bookmarksfly.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://uj.shxzskj.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ps.nicolike.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://pd.wgjwhj.cn

TS:   // 手写 Map<string, number>
来源：http://zt.szxytkj.cn

Java: // 手写 HashMap
来源：http://mo.shxzukj.cn

Go:   // 手写 map[int]int
来源：http://xb.yuexingan06.cn

Ruby: // 手写 Hash
来源：http://yp.szsharing.cn

C#:   // 手写 Dictionary<int, int>
来源：http://zw.haigaiapp.cn

[N08] 生成全排列
来源：http://hg.huixinmuqiang.cn

Py:   itertools.permutations(arr)
来源：http://eu.nicolike.cn

PHP:  // 手写递归交换
来源：http://lf.bjjhwx.cn

JS:   // 手写回溯递归
来源：http://wa.jianghongdianzi.cn

TS:   // 手写回溯递归
来源：http://oo.asd995.cn

Java: // 手写回溯递归
来源：http://mh.huanxung.cn

Go:   // 手写回溯递归
来源：http://wu.huixinmuqiang.cn

Ruby: arr.permutation.to_a
来源：http://vz.9csxet.cn

C#:   // 手写回溯递归
来源：http://lu.jctech888.com.cn

[N09] 栈与队列
来源：http://ux.asd995.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://nk.jctech888.com.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://zo.newstarts.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://el.chemitech.net.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://fu.bjjhwx.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://le.panjiajie.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ad.muxihuayi.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://uq.chemitech.net.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ry.huanxung.cn

[N10] 链表节点定义
来源：http://jk.lnxyls.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hr.hahajie.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://jt.nicolike.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ey.shtwfgs.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ip.colortex.cn

Java: class Node { int v; Node next; }
来源：http://ee.wgjwhj.cn

Go:   type Node struct { V int; Next *Node }
来源：http://vp.hnjuh.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://zu.asd995.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://zj.gzmigu.cn

[N11] 二叉树中序遍历
来源：http://pu.wgjwhj.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ki.yuexingan06.cn

PHP:  // 手写递归函数
来源：http://ux.wgjwhj.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kf.shtwfgs.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zd.muxihuayi.cn

Java: // 手写递归
来源：http://rk.bjjhwx.cn

Go:   // 手写递归
来源：http://pm.gzmigu.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://yt.bookmarksfly.cn

C#:   // 手写递归
来源：http://mb.asd995.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://lp.wgjwhj.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://zt.shxzukj.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://as.gzmigu.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hb.asd995.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pq.bjjhwx.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ec.huixinmuqiang.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://zv.haigaiapp.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ey.chemitech.net.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://fv.muxihuayi.cn

================================================================================
来源：http://sg.wgjwhj.cn

O. 并发与异步
来源：http://yy.huanxung.cn

================================================================================
来源：http://ue.9csxet.cn

[O01] 启动一个线程
来源：http://xm.asd995.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ag.panjiajie.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://fq.lnxyls.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://dd.wgjwhj.cn

TS:   // 同 JS
来源：http://ij.panjiajie.cn

Java: new Thread(() -> f()).start()
来源：http://wo.huanxung.cn

Go:   go f()
来源：http://uw.szxytkj.cn

Ruby: Thread.new { f }
来源：http://ze.nicolike.cn

C#:   Task.Run(() => F());
来源：http://ry.muxihuayi.cn

[O02] 使用线程池
来源：http://fb.521024.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://oz.wgjwhj.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://zd.bjjhwx.cn

JS:   // worker_threads 线程池
来源：http://yh.hahajie.cn

TS:   // worker_threads 线程池
来源：http://mg.hahajie.cn

Java: Executors.newFixedThreadPool(4)
来源：http://yb.wgjwhj.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://zy.gzmigu.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://yl.shtwfgs.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ty.chemitech.net.cn

[O03] 加锁保护共享数据
来源：http://gg.jianghongdianzi.cn

Py:   with lock: shared += 1
来源：http://hf.nicolike.cn

PHP:  // 用 flock() 做文件锁
来源：http://ab.haigaiapp.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://yw.szsharing.cn

TS:   // 同 JS
来源：http://bl.521024.cn

Java: synchronized (this) { shared++; }
来源：http://dn.shxzukj.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wt.yuntaijiaju.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://br.newstarts.cn

C#:   lock (gate) { shared++; }
来源：http://pn.szxytkj.cn

[O04] 定义异步函数并等待
来源：http://jv.gzmigu.cn

Py:   async def f():⏎    await g()
来源：http://ou.9csxet.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ri.yuntaijiaju.cn

JS:   async function f() { await g(); }
来源：http://dl.shtwfgs.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://nm.huanxung.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://xv.szsharing.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://bo.szsharing.cn

Ruby: # 用 Fiber 或 async gem
来源：http://sy.yuexingan06.cn

C#:   async Task F() { await G(); }
来源：http://fp.jianghongdianzi.cn

[O05] 并发执行并等待全部完成
来源：http://xb.9csxet.cn

Py:   asyncio.gather(*tasks)
来源：http://ma.gzmigu.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://nf.shxzskj.cn

JS:   await Promise.all(tasks)
来源：http://um.hnjuh.cn

TS:   await Promise.all(tasks)
来源：http://yp.colortex.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://zy.hnjuh.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://xf.bookmarksfly.cn

Ruby: threads.map(&:join)
来源：http://oj.shtwfgs.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://zi.panjiajie.cn

[O06] 使用进程池
来源：http://mt.muxihuayi.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://gs.shxzukj.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ig.yuexingan06.cn

JS:   // child_process / cluster 模块
来源：http://us.shtwfgs.cn


<!-- 参考信息 -->