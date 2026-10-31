代发 wailian999

Py:   requests.post(url, json={"a": 1})
来源：http://mr.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://gq.nicolike.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rj.haigaiapp.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qn.chemitech.net.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://of.wgjwhj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://gb.chemitech.net.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ez.shtwfgs.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xs.gzmigu.cn

[L03] 设置自定义请求头
来源：http://km.wgjwhj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://xp.nicolike.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wq.wgjwhj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bl.szxytkj.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ep.szxytkj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ls.huixiangedu.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://gs.colortex.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wf.lnxyls.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://kp.szsharing.cn

[L04] 设置超时
来源：http://kr.huixiangedu.cn

Py:   requests.get(url, timeout=5)
来源：http://te.yuntaijiaju.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ae.chemitech.net.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ry.yuntaijiaju.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nk.hnjuh.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mn.huixinmuqiang.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://nz.huixiangedu.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ie.bjjhwx.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://oi.colortex.cn

[L05] 上传文件（multipart）
来源：http://ft.bookmarksfly.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://na.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://bv.yuexingan06.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://dw.bookmarksfly.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://vs.hnjuh.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://of.9csxet.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ji.yuexingan06.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://xs.chemitech.net.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://fz.nicolike.cn

[L06] 解析响应为 JSON
来源：http://kr.bjjhwx.cn

Py:   resp.json()
来源：http://pm.lnxyls.cn

PHP:  json_decode($body, true);
来源：http://mf.nicolike.cn

JS:   await resp.json()
来源：http://ml.huanxung.cn

TS:   await resp.json()
来源：http://sq.gzmigu.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://kq.newstarts.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://cv.jctech888.com.cn

Ruby: JSON.parse(resp.body)
来源：http://ur.shtwfgs.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://cc.nszjky.cn

[L07] 处理 HTTP 状态码
来源：http://ji.hnjuh.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ji.nszjky.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qi.hnjuh.cn

JS:   resp.ok;  resp.status
来源：http://ib.shxzukj.cn

TS:   resp.ok;  resp.status
来源：http://ou.bjjhwx.cn

Java: resp.statusCode()
来源：http://vb.colortex.cn

Go:   resp.StatusCode
来源：http://ik.lnxyls.cn

Ruby: resp.code.to_i
来源：http://zc.yuntaijiaju.cn

C#:   (int)resp.StatusCode
来源：http://dd.shtwfgs.cn

[L08] 并发请求多个地址
来源：http://ra.lnxyls.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://zb.yuntaijiaju.cn

PHP:  curl_multi_init() 系列
来源：http://ok.colortex.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lp.shxzskj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kr.huanxung.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://jw.gzmigu.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://fi.huixinmuqiang.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://dn.huixinmuqiang.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://gj.haigaiapp.cn

================================================================================
来源：http://do.huixinmuqiang.cn

M. 命令行 / 进程 / 环境
来源：http://lm.shxzskj.cn

================================================================================
来源：http://dw.nicolike.cn

[M01] 读取命令行参数
来源：http://wf.asd995.cn

Py:   sys.argv[1:]
来源：http://xi.huixiangedu.cn

PHP:  $argv;  $argc;
来源：http://lw.szxytkj.cn

JS:   process.argv.slice(2)
来源：http://cg.jctech888.com.cn

TS:   process.argv.slice(2)
来源：http://bm.colortex.cn

Java: args 数组（main 方法参数）
来源：http://tr.newstarts.cn

Go:   os.Args[1:]
来源：http://rj.szxytkj.cn

Ruby: ARGV
来源：http://tz.yuexingan06.cn

C#:   args 数组（Main 方法参数）
来源：http://kv.9csxet.cn

[M02] 读取环境变量
来源：http://al.yuexingan06.cn

Py:   os.environ.get("HOME")
来源：http://wd.colortex.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://sq.gzmigu.cn

JS:   process.env.HOME
来源：http://gy.huanxung.cn

TS:   process.env.HOME
来源：http://yk.lnxyls.cn

Java: System.getenv("HOME")
来源：http://cz.huixiangedu.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hx.huanxung.cn

Ruby: ENV["HOME"]
来源：http://gx.huixiangedu.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://gv.huixinmuqiang.cn

[M03] 执行外部命令
来源：http://qa.chemitech.net.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://uu.haigaiapp.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://pf.521024.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://py.bookmarksfly.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://dc.gzmigu.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://sr.szsharing.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://jf.yuntaijiaju.cn

Ruby: system("ls -l");  `ls -l`
来源：http://zu.panjiajie.cn

C#:   Process.Start("ls", "-l");
来源：http://vo.gzmigu.cn

[M04] 获取当前工作目录
来源：http://lu.newstarts.cn

Py:   os.getcwd()
来源：http://kl.shxzskj.cn

PHP:  getcwd();
来源：http://vt.huanxung.cn

JS:   process.cwd()
来源：http://ia.szxytkj.cn

TS:   process.cwd()
来源：http://ak.shtwfgs.cn

Java: Path.of("").toAbsolutePath()
来源：http://uv.jianghongdianzi.cn

Go:   os.Getwd()
来源：http://bv.9csxet.cn

Ruby: Dir.pwd
来源：http://kz.bjjhwx.cn

C#:   Directory.GetCurrentDirectory()
来源：http://nz.szsharing.cn

[M05] 设置退出码
来源：http://vp.huixiangedu.cn

Py:   sys.exit(1)
来源：http://vu.asd995.cn

PHP:  exit(1);
来源：http://gk.shtwfgs.cn

JS:   process.exit(1)
来源：http://iz.nszjky.cn

TS:   process.exit(1)
来源：http://zp.wgjwhj.cn

Java: System.exit(1)
来源：http://qz.lnxyls.cn

Go:   os.Exit(1)
来源：http://dy.huanxung.cn

Ruby: exit 1
来源：http://nj.panjiajie.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://my.shxzskj.cn

[M06] 向标准错误输出
来源：http://lq.jctech888.com.cn

Py:   print("err", file=sys.stderr)
来源：http://vx.9csxet.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ja.huixiangedu.cn

JS:   console.error("err")
来源：http://fx.shxzukj.cn

TS:   console.error("err")
来源：http://he.bjjhwx.cn

Java: System.err.println("err")
来源：http://ec.chemitech.net.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://it.bjjhwx.cn

Ruby: warn "err"
来源：http://yv.yuntaijiaju.cn

C#:   Console.Error.WriteLine("err")
来源：http://re.shtwfgs.cn

[M07] 判断是否为主入口
来源：http://br.haigaiapp.cn

Py:   if __name__ == "__main__":
来源：http://qh.9csxet.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ya.gzmigu.cn

JS:   require.main === module
来源：http://lq.jctech888.com.cn

TS:   require.main === module
来源：http://ge.wgjwhj.cn

Java: public static void main(String[] args)
来源：http://fr.szxytkj.cn

Go:   func main()
来源：http://eq.asd995.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mz.hnjuh.cn

C#:   static void Main(string[] args)
来源：http://ur.newstarts.cn

[M08] 获取系统与运行时信息
来源：http://ky.jianghongdianzi.cn

Py:   platform.system();  platform.python_version()
来源：http://uu.szxytkj.cn

PHP:  PHP_OS;  phpversion();
来源：http://vo.colortex.cn

JS:   process.platform;  process.version
来源：http://gg.bookmarksfly.cn

TS:   process.platform;  process.version
来源：http://tz.muxihuayi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://jr.muxihuayi.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://tk.panjiajie.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://oa.shxzskj.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://rg.colortex.cn

================================================================================
来源：http://xp.yuexingan06.cn

N. 数据结构与算法
来源：http://jd.yuntaijiaju.cn

================================================================================
来源：http://ar.wgjwhj.cn

[N01] 二分查找（有序数组）
来源：http://qo.shtwfgs.cn

Py:   bisect.bisect_left(arr, x)
来源：http://hh.colortex.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://oe.panjiajie.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://th.jianghongdianzi.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dq.shxzskj.cn

Java: Arrays.binarySearch(arr, x)
来源：http://tt.colortex.cn

Go:   sort.SearchInts(arr, x)
来源：http://wm.shxzskj.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ng.bookmarksfly.cn

C#:   Array.BinarySearch(arr, x)
来源：http://aj.huanxung.cn

[N02] 排序（工程实践用内置实现）
来源：http://az.yuntaijiaju.cn

Py:   sorted(arr);  arr.sort()
来源：http://zl.hnjuh.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://te.bookmarksfly.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://fn.wgjwhj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://df.bookmarksfly.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hp.asd995.cn

Go:   slices.Sort(arr)
来源：http://os.colortex.cn

Ruby: arr.sort
来源：http://iv.521024.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://bs.nszjky.cn

[N03] 快速排序（分治示例）
来源：http://vu.nicolike.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://xm.huanxung.cn

PHP:  // 递归实现，或用 usort
来源：http://iv.nicolike.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cj.huanxung.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nt.wgjwhj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ug.shtwfgs.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ln.panjiajie.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ao.hahajie.cn

C#:   // 手写递归，或 Array.Sort
来源：http://sh.nicolike.cn

[N04] 斐波那契数列
来源：http://qf.yuexingan06.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hl.bjjhwx.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://tz.bookmarksfly.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gq.asd995.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fk.nicolike.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mi.shxzukj.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://va.szxytkj.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://nz.shtwfgs.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://rm.gzmigu.cn

[N05] 最大公约数
来源：http://ln.huanxung.cn

Py:   math.gcd(a, b)
来源：http://xw.hnjuh.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://om.huanxung.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xw.muxihuayi.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cb.yuexingan06.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ry.lnxyls.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ol.huanxung.cn

Ruby: a.gcd(b)
来源：http://sk.huixinmuqiang.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://za.huixinmuqiang.cn

[N06] 判断回文字符串
来源：http://zi.huanxung.cn

Py:   s == s[::-1]
来源：http://ge.asd995.cn

PHP:  $s === strrev($s);
来源：http://mh.nszjky.cn

JS:   s === [...s].reverse().join("")
来源：http://yt.yuexingan06.cn

TS:   s === [...s].reverse().join("")
来源：http://xo.9csxet.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mc.gzmigu.cn

Go:   // 双指针从两端比较
来源：http://vj.lnxyls.cn

Ruby: s == s.reverse
来源：http://fj.panjiajie.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://er.yuexingan06.cn

[N07] 两数之和（返回下标）
来源：http://ol.muxihuayi.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ge.shxzskj.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://tv.muxihuayi.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://oh.shtwfgs.cn

TS:   // 手写 Map<string, number>
来源：http://pw.asd995.cn

Java: // 手写 HashMap
来源：http://bu.hahajie.cn

Go:   // 手写 map[int]int
来源：http://hn.asd995.cn

Ruby: // 手写 Hash
来源：http://hg.asd995.cn

C#:   // 手写 Dictionary<int, int>
来源：http://rf.yuntaijiaju.cn

[N08] 生成全排列
来源：http://xu.panjiajie.cn

Py:   itertools.permutations(arr)
来源：http://ne.yuntaijiaju.cn

PHP:  // 手写递归交换
来源：http://dr.shxzskj.cn

JS:   // 手写回溯递归
来源：http://pm.hahajie.cn

TS:   // 手写回溯递归
来源：http://jo.wgjwhj.cn

Java: // 手写回溯递归
来源：http://cj.asd995.cn

Go:   // 手写回溯递归
来源：http://ch.lnxyls.cn

Ruby: arr.permutation.to_a
来源：http://ce.wgjwhj.cn

C#:   // 手写回溯递归
来源：http://lq.nicolike.cn

[N09] 栈与队列
来源：http://fg.9csxet.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hd.panjiajie.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://bd.lnxyls.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://fc.newstarts.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://vw.haigaiapp.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ea.newstarts.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ig.gzmigu.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ea.jianghongdianzi.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://pp.shtwfgs.cn

[N10] 链表节点定义
来源：http://zm.9csxet.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://of.szsharing.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ap.lnxyls.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://dq.panjiajie.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ig.jianghongdianzi.cn

Java: class Node { int v; Node next; }
来源：http://tj.jctech888.com.cn

Go:   type Node struct { V int; Next *Node }
来源：http://am.521024.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://sm.bjjhwx.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://cc.lnxyls.cn

[N11] 二叉树中序遍历
来源：http://qx.huanxung.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ni.shtwfgs.cn

PHP:  // 手写递归函数
来源：http://qk.hnjuh.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://am.yuexingan06.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://le.lnxyls.cn

Java: // 手写递归
来源：http://um.muxihuayi.cn

Go:   // 手写递归
来源：http://xl.wgjwhj.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wx.yuntaijiaju.cn

C#:   // 手写递归
来源：http://xb.nicolike.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ne.bjjhwx.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://xv.szxytkj.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://io.bookmarksfly.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vk.nszjky.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://it.chemitech.net.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://pj.wgjwhj.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ea.panjiajie.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ax.9csxet.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ag.jctech888.com.cn

================================================================================
来源：http://qk.bjjhwx.cn

O. 并发与异步
来源：http://ny.jctech888.com.cn

================================================================================
来源：http://eu.521024.cn

[O01] 启动一个线程
来源：http://yo.wgjwhj.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ba.muxihuayi.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hg.nszjky.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://rs.panjiajie.cn

TS:   // 同 JS
来源：http://da.haigaiapp.cn

Java: new Thread(() -> f()).start()
来源：http://ow.lnxyls.cn

Go:   go f()
来源：http://no.bjjhwx.cn

Ruby: Thread.new { f }
来源：http://nz.asd995.cn

C#:   Task.Run(() => F());
来源：http://ar.muxihuayi.cn

[O02] 使用线程池
来源：http://qm.yuexingan06.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://zu.szsharing.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://gq.bjjhwx.cn

JS:   // worker_threads 线程池
来源：http://md.szxytkj.cn

TS:   // worker_threads 线程池
来源：http://td.panjiajie.cn

Java: Executors.newFixedThreadPool(4)
来源：http://or.9csxet.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://vi.shxzukj.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ep.huixinmuqiang.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://pi.gzmigu.cn

[O03] 加锁保护共享数据
来源：http://bl.yuexingan06.cn

Py:   with lock: shared += 1
来源：http://hc.wgjwhj.cn

PHP:  // 用 flock() 做文件锁
来源：http://ed.newstarts.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://uv.shxzskj.cn

TS:   // 同 JS
来源：http://wt.jctech888.com.cn

Java: synchronized (this) { shared++; }
来源：http://xh.jianghongdianzi.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://du.nszjky.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://qp.panjiajie.cn

C#:   lock (gate) { shared++; }
来源：http://cv.panjiajie.cn

[O04] 定义异步函数并等待
来源：http://ga.haigaiapp.cn

Py:   async def f():⏎    await g()
来源：http://hg.jianghongdianzi.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://gd.newstarts.cn

JS:   async function f() { await g(); }
来源：http://uw.lnxyls.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ki.9csxet.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://cd.haigaiapp.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://no.9csxet.cn

Ruby: # 用 Fiber 或 async gem
来源：http://yh.colortex.cn

C#:   async Task F() { await G(); }
来源：http://cu.szxytkj.cn

[O05] 并发执行并等待全部完成
来源：http://qb.haigaiapp.cn

Py:   asyncio.gather(*tasks)
来源：http://se.lnxyls.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ci.9csxet.cn

JS:   await Promise.all(tasks)
来源：http://bt.huixiangedu.cn

TS:   await Promise.all(tasks)
来源：http://ut.szxytkj.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wy.shtwfgs.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://td.shxzskj.cn

Ruby: threads.map(&:join)
来源：http://qh.szxytkj.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://nl.gzmigu.cn

[O06] 使用进程池
来源：http://tp.colortex.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://zr.huanxung.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://yc.shxzukj.cn

JS:   // child_process / cluster 模块
来源：http://sr.newstarts.cn


<!-- 参考信息 -->