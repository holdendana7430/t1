代发 wailian999

Go:   resp, err := http.Get(url)
来源：http://rf.521024.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://mz.muxihuayi.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://jy.muxihuayi.cn

[L02] 发送 POST JSON
来源：http://vj.nicolike.cn

Py:   requests.post(url, json={"a": 1})
来源：http://wm.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://sj.hnjuh.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kx.521024.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dg.lnxyls.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://xk.huixiangedu.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://zh.gzmigu.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ha.shxzskj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://pl.jianghongdianzi.cn

[L03] 设置自定义请求头
来源：http://bu.chemitech.net.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://dr.asd995.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://gw.nicolike.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://px.panjiajie.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://or.newstarts.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ke.muxihuayi.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://fo.nszjky.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mj.muxihuayi.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://yj.9csxet.cn

[L04] 设置超时
来源：http://ls.shtwfgs.cn

Py:   requests.get(url, timeout=5)
来源：http://td.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://kz.huixinmuqiang.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tg.bjjhwx.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xk.bjjhwx.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ua.hnjuh.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://bq.nicolike.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://zn.haigaiapp.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://vl.huanxung.cn

[L05] 上传文件（multipart）
来源：http://tv.haigaiapp.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mf.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://jm.shtwfgs.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://sp.asd995.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://qb.9csxet.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://bk.jctech888.com.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://rb.colortex.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://df.huanxung.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hj.huanxung.cn

[L06] 解析响应为 JSON
来源：http://up.shxzskj.cn

Py:   resp.json()
来源：http://dc.521024.cn

PHP:  json_decode($body, true);
来源：http://jv.nicolike.cn

JS:   await resp.json()
来源：http://lt.huixiangedu.cn

TS:   await resp.json()
来源：http://rd.nszjky.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://or.shtwfgs.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://cr.chemitech.net.cn

Ruby: JSON.parse(resp.body)
来源：http://ei.hahajie.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mz.lnxyls.cn

[L07] 处理 HTTP 状态码
来源：http://mv.yuntaijiaju.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://um.colortex.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://eo.yuntaijiaju.cn

JS:   resp.ok;  resp.status
来源：http://jk.shxzukj.cn

TS:   resp.ok;  resp.status
来源：http://dp.colortex.cn

Java: resp.statusCode()
来源：http://rp.huixiangedu.cn

Go:   resp.StatusCode
来源：http://xv.huixiangedu.cn

Ruby: resp.code.to_i
来源：http://qa.jctech888.com.cn

C#:   (int)resp.StatusCode
来源：http://yy.newstarts.cn

[L08] 并发请求多个地址
来源：http://ke.hahajie.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://tv.hnjuh.cn

PHP:  curl_multi_init() 系列
来源：http://ju.shxzukj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pn.shxzukj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sg.shxzukj.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://xb.hahajie.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://cz.muxihuayi.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://oe.jctech888.com.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hc.asd995.cn

================================================================================
来源：http://jl.muxihuayi.cn

M. 命令行 / 进程 / 环境
来源：http://tg.hnjuh.cn

================================================================================
来源：http://be.newstarts.cn

[M01] 读取命令行参数
来源：http://ws.huanxung.cn

Py:   sys.argv[1:]
来源：http://qs.panjiajie.cn

PHP:  $argv;  $argc;
来源：http://qf.colortex.cn

JS:   process.argv.slice(2)
来源：http://tp.nszjky.cn

TS:   process.argv.slice(2)
来源：http://jk.nicolike.cn

Java: args 数组（main 方法参数）
来源：http://al.szxytkj.cn

Go:   os.Args[1:]
来源：http://zm.shxzukj.cn

Ruby: ARGV
来源：http://qf.yuexingan06.cn

C#:   args 数组（Main 方法参数）
来源：http://zd.nicolike.cn

[M02] 读取环境变量
来源：http://ys.nicolike.cn

Py:   os.environ.get("HOME")
来源：http://gp.yuntaijiaju.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hv.nicolike.cn

JS:   process.env.HOME
来源：http://os.bookmarksfly.cn

TS:   process.env.HOME
来源：http://qw.yuntaijiaju.cn

Java: System.getenv("HOME")
来源：http://ch.chemitech.net.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://at.bookmarksfly.cn

Ruby: ENV["HOME"]
来源：http://dm.yuntaijiaju.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://yg.shtwfgs.cn

[M03] 执行外部命令
来源：http://nc.wgjwhj.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://pp.asd995.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://my.colortex.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://mo.panjiajie.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://mj.newstarts.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hl.yuexingan06.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://db.asd995.cn

Ruby: system("ls -l");  `ls -l`
来源：http://vf.jianghongdianzi.cn

C#:   Process.Start("ls", "-l");
来源：http://zk.nicolike.cn

[M04] 获取当前工作目录
来源：http://yg.hahajie.cn

Py:   os.getcwd()
来源：http://qz.newstarts.cn

PHP:  getcwd();
来源：http://mo.szsharing.cn

JS:   process.cwd()
来源：http://rq.bookmarksfly.cn

TS:   process.cwd()
来源：http://wn.nszjky.cn

Java: Path.of("").toAbsolutePath()
来源：http://an.9csxet.cn

Go:   os.Getwd()
来源：http://ql.chemitech.net.cn

Ruby: Dir.pwd
来源：http://rv.colortex.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ca.haigaiapp.cn

[M05] 设置退出码
来源：http://gs.panjiajie.cn

Py:   sys.exit(1)
来源：http://hf.muxihuayi.cn

PHP:  exit(1);
来源：http://gm.szxytkj.cn

JS:   process.exit(1)
来源：http://ja.panjiajie.cn

TS:   process.exit(1)
来源：http://ts.wgjwhj.cn

Java: System.exit(1)
来源：http://zl.szxytkj.cn

Go:   os.Exit(1)
来源：http://ib.shxzskj.cn

Ruby: exit 1
来源：http://om.shxzskj.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://tj.lnxyls.cn

[M06] 向标准错误输出
来源：http://rf.shtwfgs.cn

Py:   print("err", file=sys.stderr)
来源：http://ag.yuexingan06.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://wk.yuntaijiaju.cn

JS:   console.error("err")
来源：http://ku.szxytkj.cn

TS:   console.error("err")
来源：http://de.wgjwhj.cn

Java: System.err.println("err")
来源：http://kz.gzmigu.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://eb.newstarts.cn

Ruby: warn "err"
来源：http://iq.nicolike.cn

C#:   Console.Error.WriteLine("err")
来源：http://km.yuexingan06.cn

[M07] 判断是否为主入口
来源：http://bu.9csxet.cn

Py:   if __name__ == "__main__":
来源：http://pu.nicolike.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://rm.521024.cn

JS:   require.main === module
来源：http://py.szxytkj.cn

TS:   require.main === module
来源：http://pj.szxytkj.cn

Java: public static void main(String[] args)
来源：http://hp.huanxung.cn

Go:   func main()
来源：http://tb.yuexingan06.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wf.szxytkj.cn

C#:   static void Main(string[] args)
来源：http://dg.huixinmuqiang.cn

[M08] 获取系统与运行时信息
来源：http://od.szxytkj.cn

Py:   platform.system();  platform.python_version()
来源：http://yx.yuexingan06.cn

PHP:  PHP_OS;  phpversion();
来源：http://ql.nicolike.cn

JS:   process.platform;  process.version
来源：http://fz.9csxet.cn

TS:   process.platform;  process.version
来源：http://fo.yuntaijiaju.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xi.colortex.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://dr.bjjhwx.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://nu.colortex.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://eh.colortex.cn

================================================================================
来源：http://ol.gzmigu.cn

N. 数据结构与算法
来源：http://ag.huixiangedu.cn

================================================================================
来源：http://cq.bookmarksfly.cn

[N01] 二分查找（有序数组）
来源：http://xf.shxzukj.cn

Py:   bisect.bisect_left(arr, x)
来源：http://tc.gzmigu.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://uy.haigaiapp.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sz.haigaiapp.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xd.chemitech.net.cn

Java: Arrays.binarySearch(arr, x)
来源：http://nj.colortex.cn

Go:   sort.SearchInts(arr, x)
来源：http://zd.9csxet.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://fi.huixinmuqiang.cn

C#:   Array.BinarySearch(arr, x)
来源：http://lw.jctech888.com.cn

[N02] 排序（工程实践用内置实现）
来源：http://lu.yuexingan06.cn

Py:   sorted(arr);  arr.sort()
来源：http://bv.nicolike.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://su.colortex.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://rd.colortex.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://vt.bookmarksfly.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://xg.nicolike.cn

Go:   slices.Sort(arr)
来源：http://py.asd995.cn

Ruby: arr.sort
来源：http://ik.huixinmuqiang.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://xa.huixiangedu.cn

[N03] 快速排序（分治示例）
来源：http://cw.chemitech.net.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ou.muxihuayi.cn

PHP:  // 递归实现，或用 usort
来源：http://ef.shxzukj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yw.asd995.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://em.wgjwhj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://kg.hahajie.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://fr.huanxung.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ei.szxytkj.cn

C#:   // 手写递归，或 Array.Sort
来源：http://va.521024.cn

[N04] 斐波那契数列
来源：http://fw.nszjky.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ih.shxzskj.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ns.szsharing.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hc.521024.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ed.jianghongdianzi.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://uu.hnjuh.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ry.gzmigu.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://pe.huixiangedu.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://we.bookmarksfly.cn

[N05] 最大公约数
来源：http://wd.gzmigu.cn

Py:   math.gcd(a, b)
来源：http://sb.chemitech.net.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ts.huixiangedu.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wt.hnjuh.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bz.521024.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://gw.gzmigu.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ld.bjjhwx.cn

Ruby: a.gcd(b)
来源：http://hg.szxytkj.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://lr.shxzukj.cn

[N06] 判断回文字符串
来源：http://ee.huixiangedu.cn

Py:   s == s[::-1]
来源：http://fh.nszjky.cn

PHP:  $s === strrev($s);
来源：http://vc.9csxet.cn

JS:   s === [...s].reverse().join("")
来源：http://dy.colortex.cn

TS:   s === [...s].reverse().join("")
来源：http://wy.nszjky.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://of.muxihuayi.cn

Go:   // 双指针从两端比较
来源：http://br.huixiangedu.cn

Ruby: s == s.reverse
来源：http://gr.jctech888.com.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ky.jianghongdianzi.cn

[N07] 两数之和（返回下标）
来源：http://wv.chemitech.net.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://gi.haigaiapp.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://aw.9csxet.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://cw.shxzukj.cn

TS:   // 手写 Map<string, number>
来源：http://vv.asd995.cn

Java: // 手写 HashMap
来源：http://gv.asd995.cn

Go:   // 手写 map[int]int
来源：http://bo.wgjwhj.cn

Ruby: // 手写 Hash
来源：http://uc.521024.cn

C#:   // 手写 Dictionary<int, int>
来源：http://up.hahajie.cn

[N08] 生成全排列
来源：http://dd.szsharing.cn

Py:   itertools.permutations(arr)
来源：http://bl.jctech888.com.cn

PHP:  // 手写递归交换
来源：http://bg.lnxyls.cn

JS:   // 手写回溯递归
来源：http://dy.szsharing.cn

TS:   // 手写回溯递归
来源：http://er.9csxet.cn

Java: // 手写回溯递归
来源：http://ah.lnxyls.cn

Go:   // 手写回溯递归
来源：http://hg.chemitech.net.cn

Ruby: arr.permutation.to_a
来源：http://mp.huixiangedu.cn

C#:   // 手写回溯递归
来源：http://yu.nszjky.cn

[N09] 栈与队列
来源：http://xs.colortex.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mh.jianghongdianzi.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://yb.yuexingan06.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://rm.szxytkj.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://od.huixiangedu.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://an.9csxet.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ro.gzmigu.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ba.szxytkj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ik.huixiangedu.cn

[N10] 链表节点定义
来源：http://hy.huixinmuqiang.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://yd.gzmigu.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ug.asd995.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://kf.shxzukj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://yr.gzmigu.cn

Java: class Node { int v; Node next; }
来源：http://qv.haigaiapp.cn

Go:   type Node struct { V int; Next *Node }
来源：http://te.shxzukj.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://qu.lnxyls.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://mf.colortex.cn

[N11] 二叉树中序遍历
来源：http://re.nicolike.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://vt.panjiajie.cn

PHP:  // 手写递归函数
来源：http://ut.szsharing.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hn.jctech888.com.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://am.chemitech.net.cn

Java: // 手写递归
来源：http://zs.nszjky.cn

Go:   // 手写递归
来源：http://fv.asd995.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://pk.panjiajie.cn

C#:   // 手写递归
来源：http://jb.huixinmuqiang.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://gt.huixinmuqiang.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://kz.bookmarksfly.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://fx.nicolike.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vl.huanxung.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lv.hahajie.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://kx.huixiangedu.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://de.9csxet.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://no.huanxung.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://bm.gzmigu.cn

================================================================================
来源：http://rw.huanxung.cn

O. 并发与异步
来源：http://it.gzmigu.cn

================================================================================
来源：http://vs.jianghongdianzi.cn

[O01] 启动一个线程
来源：http://nq.yuntaijiaju.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mx.jctech888.com.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ni.haigaiapp.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://xn.szxytkj.cn

TS:   // 同 JS
来源：http://hi.bookmarksfly.cn

Java: new Thread(() -> f()).start()
来源：http://mk.jianghongdianzi.cn

Go:   go f()
来源：http://dn.gzmigu.cn

Ruby: Thread.new { f }
来源：http://vk.lnxyls.cn

C#:   Task.Run(() => F());
来源：http://mi.muxihuayi.cn

[O02] 使用线程池
来源：http://gz.shxzskj.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ov.hahajie.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://fh.shtwfgs.cn

JS:   // worker_threads 线程池
来源：http://hv.jianghongdianzi.cn

TS:   // worker_threads 线程池
来源：http://ea.nszjky.cn

Java: Executors.newFixedThreadPool(4)
来源：http://bv.huixiangedu.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://bb.521024.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ee.lnxyls.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://cb.bjjhwx.cn

[O03] 加锁保护共享数据
来源：http://ul.gzmigu.cn

Py:   with lock: shared += 1
来源：http://tm.lnxyls.cn

PHP:  // 用 flock() 做文件锁
来源：http://yi.hahajie.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ez.shtwfgs.cn

TS:   // 同 JS
来源：http://jr.jianghongdianzi.cn

Java: synchronized (this) { shared++; }
来源：http://dg.nicolike.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://cj.huanxung.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ye.hnjuh.cn

C#:   lock (gate) { shared++; }
来源：http://ty.haigaiapp.cn

[O04] 定义异步函数并等待
来源：http://pk.nicolike.cn

Py:   async def f():⏎    await g()
来源：http://sz.jctech888.com.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://uu.jianghongdianzi.cn

JS:   async function f() { await g(); }
来源：http://cw.yuexingan06.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://zo.huanxung.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://pr.nicolike.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ax.huanxung.cn

Ruby: # 用 Fiber 或 async gem
来源：http://zl.asd995.cn

C#:   async Task F() { await G(); }
来源：http://bv.muxihuayi.cn

[O05] 并发执行并等待全部完成
来源：http://gp.hahajie.cn

Py:   asyncio.gather(*tasks)
来源：http://yx.huixinmuqiang.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ao.nszjky.cn

JS:   await Promise.all(tasks)
来源：http://mz.huanxung.cn

TS:   await Promise.all(tasks)
来源：http://zs.yuntaijiaju.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ww.bjjhwx.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://rk.shxzukj.cn

Ruby: threads.map(&:join)
来源：http://wq.nicolike.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://qg.jianghongdianzi.cn


<!-- 参考信息 -->