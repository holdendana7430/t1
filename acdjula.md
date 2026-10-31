代发 wailian999

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://bc.shtwfgs.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://pg.521024.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mb.lnxyls.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://kz.lnxyls.cn

[L03] 设置自定义请求头
来源：http://vp.shxzskj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://rt.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://uy.szsharing.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dr.colortex.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fk.newstarts.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ld.jianghongdianzi.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://sa.jianghongdianzi.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ga.huanxung.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://yt.nszjky.cn

[L04] 设置超时
来源：http://ok.yuntaijiaju.cn

Py:   requests.get(url, timeout=5)
来源：http://ru.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://qx.yuexingan06.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gm.nszjky.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uc.szxytkj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://to.panjiajie.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ox.9csxet.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://yz.bookmarksfly.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://xa.hahajie.cn

[L05] 上传文件（multipart）
来源：http://zs.shtwfgs.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ff.gzmigu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ay.haigaiapp.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://xw.521024.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://st.hahajie.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://oq.bjjhwx.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://lx.jianghongdianzi.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ud.huanxung.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://fl.colortex.cn

[L06] 解析响应为 JSON
来源：http://un.chemitech.net.cn

Py:   resp.json()
来源：http://ma.szsharing.cn

PHP:  json_decode($body, true);
来源：http://rj.szsharing.cn

JS:   await resp.json()
来源：http://ve.haigaiapp.cn

TS:   await resp.json()
来源：http://uu.yuntaijiaju.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://fz.bookmarksfly.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://sx.newstarts.cn

Ruby: JSON.parse(resp.body)
来源：http://ac.jctech888.com.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://au.jctech888.com.cn

[L07] 处理 HTTP 状态码
来源：http://bi.szsharing.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://pi.haigaiapp.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://sn.hahajie.cn

JS:   resp.ok;  resp.status
来源：http://qc.haigaiapp.cn

TS:   resp.ok;  resp.status
来源：http://gt.shtwfgs.cn

Java: resp.statusCode()
来源：http://lh.521024.cn

Go:   resp.StatusCode
来源：http://pq.wgjwhj.cn

Ruby: resp.code.to_i
来源：http://nd.huixinmuqiang.cn

C#:   (int)resp.StatusCode
来源：http://oq.muxihuayi.cn

[L08] 并发请求多个地址
来源：http://fu.newstarts.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hu.hahajie.cn

PHP:  curl_multi_init() 系列
来源：http://gj.wgjwhj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pq.shtwfgs.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qo.chemitech.net.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://gg.huixiangedu.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://cn.colortex.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://yn.muxihuayi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://sa.haigaiapp.cn

================================================================================
来源：http://wj.shtwfgs.cn

M. 命令行 / 进程 / 环境
来源：http://cq.bookmarksfly.cn

================================================================================
来源：http://el.yuexingan06.cn

[M01] 读取命令行参数
来源：http://gl.bookmarksfly.cn

Py:   sys.argv[1:]
来源：http://iv.bjjhwx.cn

PHP:  $argv;  $argc;
来源：http://fi.newstarts.cn

JS:   process.argv.slice(2)
来源：http://aj.huixiangedu.cn

TS:   process.argv.slice(2)
来源：http://ep.szxytkj.cn

Java: args 数组（main 方法参数）
来源：http://cy.huanxung.cn

Go:   os.Args[1:]
来源：http://rw.asd995.cn

Ruby: ARGV
来源：http://qm.huixiangedu.cn

C#:   args 数组（Main 方法参数）
来源：http://cc.shxzskj.cn

[M02] 读取环境变量
来源：http://og.shtwfgs.cn

Py:   os.environ.get("HOME")
来源：http://wy.bjjhwx.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hw.jianghongdianzi.cn

JS:   process.env.HOME
来源：http://rs.jianghongdianzi.cn

TS:   process.env.HOME
来源：http://md.yuntaijiaju.cn

Java: System.getenv("HOME")
来源：http://kj.shtwfgs.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://xe.huanxung.cn

Ruby: ENV["HOME"]
来源：http://zi.newstarts.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://sd.nszjky.cn

[M03] 执行外部命令
来源：http://kg.huanxung.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wg.shtwfgs.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://pz.bookmarksfly.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ee.panjiajie.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://hs.asd995.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ly.colortex.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ld.yuntaijiaju.cn

Ruby: system("ls -l");  `ls -l`
来源：http://yd.szxytkj.cn

C#:   Process.Start("ls", "-l");
来源：http://cw.huanxung.cn

[M04] 获取当前工作目录
来源：http://wi.yuexingan06.cn

Py:   os.getcwd()
来源：http://ig.shxzskj.cn

PHP:  getcwd();
来源：http://kg.panjiajie.cn

JS:   process.cwd()
来源：http://ip.szxytkj.cn

TS:   process.cwd()
来源：http://kw.huixinmuqiang.cn

Java: Path.of("").toAbsolutePath()
来源：http://ul.hahajie.cn

Go:   os.Getwd()
来源：http://mn.haigaiapp.cn

Ruby: Dir.pwd
来源：http://co.bjjhwx.cn

C#:   Directory.GetCurrentDirectory()
来源：http://vy.bjjhwx.cn

[M05] 设置退出码
来源：http://kg.huanxung.cn

Py:   sys.exit(1)
来源：http://jj.huixinmuqiang.cn

PHP:  exit(1);
来源：http://dd.yuntaijiaju.cn

JS:   process.exit(1)
来源：http://mr.szxytkj.cn

TS:   process.exit(1)
来源：http://nf.hnjuh.cn

Java: System.exit(1)
来源：http://ov.szxytkj.cn

Go:   os.Exit(1)
来源：http://ox.colortex.cn

Ruby: exit 1
来源：http://ou.nicolike.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ko.yuntaijiaju.cn

[M06] 向标准错误输出
来源：http://fw.haigaiapp.cn

Py:   print("err", file=sys.stderr)
来源：http://hn.jianghongdianzi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://bd.huixinmuqiang.cn

JS:   console.error("err")
来源：http://yu.newstarts.cn

TS:   console.error("err")
来源：http://xs.yuntaijiaju.cn

Java: System.err.println("err")
来源：http://ko.yuexingan06.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://xj.nicolike.cn

Ruby: warn "err"
来源：http://ch.chemitech.net.cn

C#:   Console.Error.WriteLine("err")
来源：http://hi.huixiangedu.cn

[M07] 判断是否为主入口
来源：http://pq.asd995.cn

Py:   if __name__ == "__main__":
来源：http://rq.9csxet.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://jp.9csxet.cn

JS:   require.main === module
来源：http://fk.bookmarksfly.cn

TS:   require.main === module
来源：http://wk.szxytkj.cn

Java: public static void main(String[] args)
来源：http://sh.huixiangedu.cn

Go:   func main()
来源：http://lg.9csxet.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://bg.asd995.cn

C#:   static void Main(string[] args)
来源：http://my.shxzskj.cn

[M08] 获取系统与运行时信息
来源：http://tw.wgjwhj.cn

Py:   platform.system();  platform.python_version()
来源：http://sd.lnxyls.cn

PHP:  PHP_OS;  phpversion();
来源：http://hb.szxytkj.cn

JS:   process.platform;  process.version
来源：http://wv.jianghongdianzi.cn

TS:   process.platform;  process.version
来源：http://de.asd995.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://vd.hahajie.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://dg.panjiajie.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://rd.panjiajie.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ws.bjjhwx.cn

================================================================================
来源：http://bd.panjiajie.cn

N. 数据结构与算法
来源：http://xr.jianghongdianzi.cn

================================================================================
来源：http://zu.shxzskj.cn

[N01] 二分查找（有序数组）
来源：http://em.huanxung.cn

Py:   bisect.bisect_left(arr, x)
来源：http://na.hnjuh.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wx.shtwfgs.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ib.colortex.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mr.chemitech.net.cn

Java: Arrays.binarySearch(arr, x)
来源：http://jj.jctech888.com.cn

Go:   sort.SearchInts(arr, x)
来源：http://ua.shtwfgs.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ay.szsharing.cn

C#:   Array.BinarySearch(arr, x)
来源：http://jl.hahajie.cn

[N02] 排序（工程实践用内置实现）
来源：http://jm.wgjwhj.cn

Py:   sorted(arr);  arr.sort()
来源：http://dm.bookmarksfly.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://jb.colortex.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://vu.lnxyls.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://mf.shxzukj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ew.jctech888.com.cn

Go:   slices.Sort(arr)
来源：http://wx.huixinmuqiang.cn

Ruby: arr.sort
来源：http://vo.hnjuh.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://db.lnxyls.cn

[N03] 快速排序（分治示例）
来源：http://po.jianghongdianzi.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ql.yuntaijiaju.cn

PHP:  // 递归实现，或用 usort
来源：http://pp.521024.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dp.yuntaijiaju.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qm.hahajie.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://qm.huixinmuqiang.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://pp.asd995.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wg.jianghongdianzi.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ha.jianghongdianzi.cn

[N04] 斐波那契数列
来源：http://vw.yuntaijiaju.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://fm.haigaiapp.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wn.gzmigu.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://st.jctech888.com.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://si.nicolike.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://pd.yuexingan06.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://uw.bookmarksfly.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://db.yuexingan06.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ah.wgjwhj.cn

[N05] 最大公约数
来源：http://qf.szxytkj.cn

Py:   math.gcd(a, b)
来源：http://sd.shxzukj.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ob.yuntaijiaju.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gn.hnjuh.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sl.chemitech.net.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zk.9csxet.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://xl.huanxung.cn

Ruby: a.gcd(b)
来源：http://uy.jctech888.com.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://lk.nicolike.cn

[N06] 判断回文字符串
来源：http://ob.muxihuayi.cn

Py:   s == s[::-1]
来源：http://wa.hahajie.cn

PHP:  $s === strrev($s);
来源：http://li.shxzukj.cn

JS:   s === [...s].reverse().join("")
来源：http://ov.szsharing.cn

TS:   s === [...s].reverse().join("")
来源：http://qz.newstarts.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://zm.521024.cn

Go:   // 双指针从两端比较
来源：http://oi.asd995.cn

Ruby: s == s.reverse
来源：http://lc.hahajie.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://wo.9csxet.cn

[N07] 两数之和（返回下标）
来源：http://vc.huixinmuqiang.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://dn.szxytkj.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://br.bookmarksfly.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://bo.huixinmuqiang.cn

TS:   // 手写 Map<string, number>
来源：http://sa.hnjuh.cn

Java: // 手写 HashMap
来源：http://gn.huixiangedu.cn

Go:   // 手写 map[int]int
来源：http://jf.muxihuayi.cn

Ruby: // 手写 Hash
来源：http://jn.9csxet.cn

C#:   // 手写 Dictionary<int, int>
来源：http://dc.shxzukj.cn

[N08] 生成全排列
来源：http://lk.colortex.cn

Py:   itertools.permutations(arr)
来源：http://nr.shtwfgs.cn

PHP:  // 手写递归交换
来源：http://qf.chemitech.net.cn

JS:   // 手写回溯递归
来源：http://pe.jianghongdianzi.cn

TS:   // 手写回溯递归
来源：http://cg.wgjwhj.cn

Java: // 手写回溯递归
来源：http://ki.haigaiapp.cn

Go:   // 手写回溯递归
来源：http://ak.gzmigu.cn

Ruby: arr.permutation.to_a
来源：http://el.9csxet.cn

C#:   // 手写回溯递归
来源：http://jw.9csxet.cn

[N09] 栈与队列
来源：http://qw.lnxyls.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wb.bookmarksfly.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://as.hnjuh.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://aw.nicolike.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ag.szxytkj.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ro.bookmarksfly.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://tu.yuntaijiaju.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://sy.jctech888.com.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://su.szxytkj.cn

[N10] 链表节点定义
来源：http://nc.yuexingan06.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://rf.jianghongdianzi.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://qw.yuntaijiaju.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://zu.chemitech.net.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://sq.hahajie.cn

Java: class Node { int v; Node next; }
来源：http://ri.asd995.cn

Go:   type Node struct { V int; Next *Node }
来源：http://qf.jctech888.com.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://fp.szsharing.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://wt.nszjky.cn

[N11] 二叉树中序遍历
来源：http://bg.huixiangedu.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://pz.lnxyls.cn

PHP:  // 手写递归函数
来源：http://dw.nicolike.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qq.huixiangedu.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ha.nicolike.cn

Java: // 手写递归
来源：http://bc.9csxet.cn

Go:   // 手写递归
来源：http://fw.nszjky.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://lz.gzmigu.cn

C#:   // 手写递归
来源：http://ve.jianghongdianzi.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://od.bjjhwx.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ha.huixinmuqiang.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://qj.bjjhwx.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vd.panjiajie.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fi.nszjky.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://sh.hnjuh.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://xu.huanxung.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://fl.bjjhwx.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ej.jctech888.com.cn

================================================================================
来源：http://ff.huanxung.cn

O. 并发与异步
来源：http://vm.9csxet.cn

================================================================================
来源：http://yn.jctech888.com.cn

[O01] 启动一个线程
来源：http://rl.jianghongdianzi.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://jw.wgjwhj.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://fv.nicolike.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://uf.nicolike.cn

TS:   // 同 JS
来源：http://gq.muxihuayi.cn

Java: new Thread(() -> f()).start()
来源：http://nl.bjjhwx.cn

Go:   go f()
来源：http://aw.asd995.cn

Ruby: Thread.new { f }
来源：http://xu.jctech888.com.cn

C#:   Task.Run(() => F());
来源：http://fp.nicolike.cn

[O02] 使用线程池
来源：http://on.shxzskj.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://pr.nszjky.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://lt.bjjhwx.cn

JS:   // worker_threads 线程池
来源：http://mf.muxihuayi.cn

TS:   // worker_threads 线程池
来源：http://za.huixinmuqiang.cn

Java: Executors.newFixedThreadPool(4)
来源：http://sp.hnjuh.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://yx.chemitech.net.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://sq.gzmigu.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://jh.muxihuayi.cn

[O03] 加锁保护共享数据
来源：http://co.shxzukj.cn

Py:   with lock: shared += 1
来源：http://ni.huixiangedu.cn

PHP:  // 用 flock() 做文件锁
来源：http://pb.haigaiapp.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://pa.nicolike.cn

TS:   // 同 JS
来源：http://yv.hahajie.cn

Java: synchronized (this) { shared++; }
来源：http://rh.muxihuayi.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://cq.shxzskj.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://zs.nszjky.cn

C#:   lock (gate) { shared++; }
来源：http://qk.yuexingan06.cn

[O04] 定义异步函数并等待
来源：http://yn.yuntaijiaju.cn

Py:   async def f():⏎    await g()
来源：http://gm.jctech888.com.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://gd.huixiangedu.cn

JS:   async function f() { await g(); }
来源：http://ps.yuntaijiaju.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ra.gzmigu.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ga.chemitech.net.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mf.bjjhwx.cn

Ruby: # 用 Fiber 或 async gem
来源：http://kx.lnxyls.cn

C#:   async Task F() { await G(); }
来源：http://rx.muxihuayi.cn

[O05] 并发执行并等待全部完成
来源：http://wt.muxihuayi.cn

Py:   asyncio.gather(*tasks)
来源：http://em.bookmarksfly.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://nq.shtwfgs.cn

JS:   await Promise.all(tasks)
来源：http://hw.huixiangedu.cn

TS:   await Promise.all(tasks)
来源：http://rj.chemitech.net.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ox.szxytkj.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ri.haigaiapp.cn

Ruby: threads.map(&:join)
来源：http://ln.jianghongdianzi.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://yq.hnjuh.cn

[O06] 使用进程池
来源：http://ok.bookmarksfly.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://xu.asd995.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://yx.nszjky.cn

JS:   // child_process / cluster 模块
来源：http://ln.haigaiapp.cn

TS:   // child_process / cluster 模块
来源：http://hm.shxzskj.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://jr.asd995.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ue.9csxet.cn

Ruby: // fork 块
来源：http://zx.bjjhwx.cn


<!-- 参考信息 -->