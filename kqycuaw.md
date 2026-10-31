代发 wailian999

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://tv.shxzskj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://vp.gzmigu.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ms.jianghongdianzi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://rp.hahajie.cn

[L03] 设置自定义请求头
来源：http://se.521024.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://zl.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://av.shtwfgs.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zs.shxzskj.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fd.shxzskj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://sf.huixinmuqiang.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://qq.yuexingan06.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://op.hnjuh.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ut.muxihuayi.cn

[L04] 设置超时
来源：http://zp.shxzskj.cn

Py:   requests.get(url, timeout=5)
来源：http://od.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://su.colortex.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://np.hahajie.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cw.colortex.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://jo.muxihuayi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fw.colortex.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://rl.newstarts.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://zy.lnxyls.cn

[L05] 上传文件（multipart）
来源：http://qw.szxytkj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://nw.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://yy.9csxet.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://nq.panjiajie.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xe.huixiangedu.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://zg.shxzskj.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://au.yuntaijiaju.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://bu.huixiangedu.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wa.yuexingan06.cn

[L06] 解析响应为 JSON
来源：http://aj.newstarts.cn

Py:   resp.json()
来源：http://fy.colortex.cn

PHP:  json_decode($body, true);
来源：http://iy.hahajie.cn

JS:   await resp.json()
来源：http://pk.chemitech.net.cn

TS:   await resp.json()
来源：http://zw.bookmarksfly.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://eq.asd995.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://bs.bookmarksfly.cn

Ruby: JSON.parse(resp.body)
来源：http://rz.9csxet.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://oj.bjjhwx.cn

[L07] 处理 HTTP 状态码
来源：http://yc.wgjwhj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://er.yuntaijiaju.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://cn.wgjwhj.cn

JS:   resp.ok;  resp.status
来源：http://tt.szxytkj.cn

TS:   resp.ok;  resp.status
来源：http://sx.9csxet.cn

Java: resp.statusCode()
来源：http://iq.lnxyls.cn

Go:   resp.StatusCode
来源：http://qx.colortex.cn

Ruby: resp.code.to_i
来源：http://yf.bookmarksfly.cn

C#:   (int)resp.StatusCode
来源：http://ay.huanxung.cn

[L08] 并发请求多个地址
来源：http://by.shxzskj.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://bj.jctech888.com.cn

PHP:  curl_multi_init() 系列
来源：http://ed.huanxung.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pg.newstarts.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://um.shtwfgs.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://cn.gzmigu.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://vi.asd995.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vs.chemitech.net.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ez.shtwfgs.cn

================================================================================
来源：http://xx.nszjky.cn

M. 命令行 / 进程 / 环境
来源：http://qc.muxihuayi.cn

================================================================================
来源：http://jo.panjiajie.cn

[M01] 读取命令行参数
来源：http://yu.huixiangedu.cn

Py:   sys.argv[1:]
来源：http://ud.asd995.cn

PHP:  $argv;  $argc;
来源：http://bg.jctech888.com.cn

JS:   process.argv.slice(2)
来源：http://yp.lnxyls.cn

TS:   process.argv.slice(2)
来源：http://sc.yuexingan06.cn

Java: args 数组（main 方法参数）
来源：http://ug.shxzskj.cn

Go:   os.Args[1:]
来源：http://lw.panjiajie.cn

Ruby: ARGV
来源：http://iy.asd995.cn

C#:   args 数组（Main 方法参数）
来源：http://lr.haigaiapp.cn

[M02] 读取环境变量
来源：http://nr.jianghongdianzi.cn

Py:   os.environ.get("HOME")
来源：http://tw.jianghongdianzi.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://tt.chemitech.net.cn

JS:   process.env.HOME
来源：http://mv.shxzukj.cn

TS:   process.env.HOME
来源：http://aa.wgjwhj.cn

Java: System.getenv("HOME")
来源：http://vj.jianghongdianzi.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://yr.huixiangedu.cn

Ruby: ENV["HOME"]
来源：http://om.nicolike.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://pw.9csxet.cn

[M03] 执行外部命令
来源：http://he.nszjky.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://my.szsharing.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mq.chemitech.net.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://bg.huixiangedu.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://lo.asd995.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://si.chemitech.net.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://mi.chemitech.net.cn

Ruby: system("ls -l");  `ls -l`
来源：http://xp.huixiangedu.cn

C#:   Process.Start("ls", "-l");
来源：http://ay.szsharing.cn

[M04] 获取当前工作目录
来源：http://xe.panjiajie.cn

Py:   os.getcwd()
来源：http://fs.jianghongdianzi.cn

PHP:  getcwd();
来源：http://rz.muxihuayi.cn

JS:   process.cwd()
来源：http://vy.shxzskj.cn

TS:   process.cwd()
来源：http://ue.colortex.cn

Java: Path.of("").toAbsolutePath()
来源：http://cf.gzmigu.cn

Go:   os.Getwd()
来源：http://fz.jianghongdianzi.cn

Ruby: Dir.pwd
来源：http://sl.521024.cn

C#:   Directory.GetCurrentDirectory()
来源：http://gi.chemitech.net.cn

[M05] 设置退出码
来源：http://ty.gzmigu.cn

Py:   sys.exit(1)
来源：http://bq.shxzskj.cn

PHP:  exit(1);
来源：http://hd.huixiangedu.cn

JS:   process.exit(1)
来源：http://qo.hahajie.cn

TS:   process.exit(1)
来源：http://tk.huixinmuqiang.cn

Java: System.exit(1)
来源：http://hg.bookmarksfly.cn

Go:   os.Exit(1)
来源：http://uj.hnjuh.cn

Ruby: exit 1
来源：http://ih.huixinmuqiang.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://nh.bookmarksfly.cn

[M06] 向标准错误输出
来源：http://bn.gzmigu.cn

Py:   print("err", file=sys.stderr)
来源：http://rf.szsharing.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://hd.colortex.cn

JS:   console.error("err")
来源：http://jv.jctech888.com.cn

TS:   console.error("err")
来源：http://ck.9csxet.cn

Java: System.err.println("err")
来源：http://so.yuexingan06.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://zp.9csxet.cn

Ruby: warn "err"
来源：http://tf.bookmarksfly.cn

C#:   Console.Error.WriteLine("err")
来源：http://cz.shtwfgs.cn

[M07] 判断是否为主入口
来源：http://ut.bookmarksfly.cn

Py:   if __name__ == "__main__":
来源：http://un.hnjuh.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://zk.newstarts.cn

JS:   require.main === module
来源：http://tx.nicolike.cn

TS:   require.main === module
来源：http://ha.9csxet.cn

Java: public static void main(String[] args)
来源：http://dg.panjiajie.cn

Go:   func main()
来源：http://wj.bjjhwx.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://zh.wgjwhj.cn

C#:   static void Main(string[] args)
来源：http://hg.hahajie.cn

[M08] 获取系统与运行时信息
来源：http://xr.panjiajie.cn

Py:   platform.system();  platform.python_version()
来源：http://gz.nicolike.cn

PHP:  PHP_OS;  phpversion();
来源：http://rk.huixinmuqiang.cn

JS:   process.platform;  process.version
来源：http://ur.521024.cn

TS:   process.platform;  process.version
来源：http://vi.huixiangedu.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://eu.hahajie.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ct.shxzukj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ba.asd995.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://xj.chemitech.net.cn

================================================================================
来源：http://ra.jctech888.com.cn

N. 数据结构与算法
来源：http://gb.nszjky.cn

================================================================================
来源：http://to.bjjhwx.cn

[N01] 二分查找（有序数组）
来源：http://cr.jctech888.com.cn

Py:   bisect.bisect_left(arr, x)
来源：http://tc.bjjhwx.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://am.nszjky.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qq.chemitech.net.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qx.szsharing.cn

Java: Arrays.binarySearch(arr, x)
来源：http://to.chemitech.net.cn

Go:   sort.SearchInts(arr, x)
来源：http://fp.hahajie.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://xl.shxzskj.cn

C#:   Array.BinarySearch(arr, x)
来源：http://gr.yuntaijiaju.cn

[N02] 排序（工程实践用内置实现）
来源：http://xh.bookmarksfly.cn

Py:   sorted(arr);  arr.sort()
来源：http://lh.521024.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ka.newstarts.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://jj.shxzskj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://mn.jctech888.com.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://sc.jctech888.com.cn

Go:   slices.Sort(arr)
来源：http://em.jianghongdianzi.cn

Ruby: arr.sort
来源：http://de.huixinmuqiang.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ku.chemitech.net.cn

[N03] 快速排序（分治示例）
来源：http://tz.gzmigu.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://eb.wgjwhj.cn

PHP:  // 递归实现，或用 usort
来源：http://jl.wgjwhj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lp.muxihuayi.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cv.hnjuh.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://os.bookmarksfly.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://gz.shtwfgs.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://fs.jianghongdianzi.cn

C#:   // 手写递归，或 Array.Sort
来源：http://vn.yuexingan06.cn

[N04] 斐波那契数列
来源：http://ld.521024.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://kp.nszjky.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wz.jianghongdianzi.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://de.szxytkj.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xs.9csxet.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ic.wgjwhj.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://cj.haigaiapp.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://sg.huanxung.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://yo.wgjwhj.cn

[N05] 最大公约数
来源：http://pt.wgjwhj.cn

Py:   math.gcd(a, b)
来源：http://wx.wgjwhj.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://gh.chemitech.net.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://uk.9csxet.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lr.nszjky.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://oa.nicolike.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://go.newstarts.cn

Ruby: a.gcd(b)
来源：http://ur.bookmarksfly.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://gy.muxihuayi.cn

[N06] 判断回文字符串
来源：http://lq.hahajie.cn

Py:   s == s[::-1]
来源：http://re.szxytkj.cn

PHP:  $s === strrev($s);
来源：http://mh.haigaiapp.cn

JS:   s === [...s].reverse().join("")
来源：http://mu.9csxet.cn

TS:   s === [...s].reverse().join("")
来源：http://vq.jianghongdianzi.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xs.nicolike.cn

Go:   // 双指针从两端比较
来源：http://wk.lnxyls.cn

Ruby: s == s.reverse
来源：http://rm.huixinmuqiang.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://qe.wgjwhj.cn

[N07] 两数之和（返回下标）
来源：http://gt.bookmarksfly.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://nb.huixinmuqiang.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://fh.lnxyls.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://hi.huixiangedu.cn

TS:   // 手写 Map<string, number>
来源：http://vy.lnxyls.cn

Java: // 手写 HashMap
来源：http://fr.huanxung.cn

Go:   // 手写 map[int]int
来源：http://gf.asd995.cn

Ruby: // 手写 Hash
来源：http://sj.yuntaijiaju.cn

C#:   // 手写 Dictionary<int, int>
来源：http://pr.hnjuh.cn

[N08] 生成全排列
来源：http://dk.lnxyls.cn

Py:   itertools.permutations(arr)
来源：http://ry.nicolike.cn

PHP:  // 手写递归交换
来源：http://yg.szsharing.cn

JS:   // 手写回溯递归
来源：http://tv.huixinmuqiang.cn

TS:   // 手写回溯递归
来源：http://fp.wgjwhj.cn

Java: // 手写回溯递归
来源：http://ts.jianghongdianzi.cn

Go:   // 手写回溯递归
来源：http://mm.panjiajie.cn

Ruby: arr.permutation.to_a
来源：http://xp.chemitech.net.cn

C#:   // 手写回溯递归
来源：http://ea.jctech888.com.cn

[N09] 栈与队列
来源：http://ic.asd995.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://lf.newstarts.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://qm.szxytkj.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://qv.panjiajie.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ij.nicolike.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://aa.muxihuayi.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wm.haigaiapp.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ke.huanxung.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://dg.lnxyls.cn

[N10] 链表节点定义
来源：http://oi.huanxung.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://dy.yuntaijiaju.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://il.yuntaijiaju.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://sp.bjjhwx.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://dd.bjjhwx.cn

Java: class Node { int v; Node next; }
来源：http://vs.gzmigu.cn

Go:   type Node struct { V int; Next *Node }
来源：http://bj.nicolike.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://kr.muxihuayi.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ge.shxzskj.cn

[N11] 二叉树中序遍历
来源：http://sd.hnjuh.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ah.nszjky.cn

PHP:  // 手写递归函数
来源：http://xj.yuntaijiaju.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tb.muxihuayi.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hv.huixinmuqiang.cn

Java: // 手写递归
来源：http://zo.521024.cn

Go:   // 手写递归
来源：http://gd.panjiajie.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://xn.bjjhwx.cn

C#:   // 手写递归
来源：http://kg.shxzskj.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://dn.colortex.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://zy.gzmigu.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wd.huixinmuqiang.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rd.newstarts.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vu.521024.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ky.haigaiapp.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://sr.muxihuayi.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ng.hnjuh.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://zd.shxzskj.cn

================================================================================
来源：http://qn.jctech888.com.cn

O. 并发与异步
来源：http://rj.panjiajie.cn

================================================================================
来源：http://ic.asd995.cn

[O01] 启动一个线程
来源：http://on.jianghongdianzi.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://be.panjiajie.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://le.huixinmuqiang.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://rv.colortex.cn

TS:   // 同 JS
来源：http://ho.asd995.cn

Java: new Thread(() -> f()).start()
来源：http://gt.shxzukj.cn

Go:   go f()
来源：http://tt.jctech888.com.cn

Ruby: Thread.new { f }
来源：http://jg.9csxet.cn

C#:   Task.Run(() => F());
来源：http://wk.9csxet.cn

[O02] 使用线程池
来源：http://oh.shtwfgs.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://yh.bjjhwx.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://aq.haigaiapp.cn

JS:   // worker_threads 线程池
来源：http://kv.huixinmuqiang.cn

TS:   // worker_threads 线程池
来源：http://dj.chemitech.net.cn

Java: Executors.newFixedThreadPool(4)
来源：http://uk.shxzskj.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://th.bookmarksfly.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://rg.szsharing.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wv.huanxung.cn

[O03] 加锁保护共享数据
来源：http://zk.chemitech.net.cn

Py:   with lock: shared += 1
来源：http://sd.huixinmuqiang.cn

PHP:  // 用 flock() 做文件锁
来源：http://ox.9csxet.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://bf.yuntaijiaju.cn

TS:   // 同 JS
来源：http://ya.shxzukj.cn

Java: synchronized (this) { shared++; }
来源：http://nl.jctech888.com.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://jx.shtwfgs.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://lu.yuexingan06.cn

C#:   lock (gate) { shared++; }
来源：http://nh.newstarts.cn

[O04] 定义异步函数并等待
来源：http://lc.asd995.cn

Py:   async def f():⏎    await g()
来源：http://kx.9csxet.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://gm.nicolike.cn

JS:   async function f() { await g(); }
来源：http://ig.yuntaijiaju.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ve.nszjky.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://gh.bookmarksfly.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://vd.jctech888.com.cn

Ruby: # 用 Fiber 或 async gem
来源：http://yv.szsharing.cn

C#:   async Task F() { await G(); }
来源：http://zi.yuntaijiaju.cn

[O05] 并发执行并等待全部完成
来源：http://no.hnjuh.cn

Py:   asyncio.gather(*tasks)
来源：http://ri.colortex.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://oi.huixiangedu.cn

JS:   await Promise.all(tasks)
来源：http://hl.lnxyls.cn

TS:   await Promise.all(tasks)
来源：http://xl.szxytkj.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://qm.lnxyls.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ke.huixiangedu.cn

Ruby: threads.map(&:join)
来源：http://uh.szsharing.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://hq.shxzukj.cn

[O06] 使用进程池
来源：http://pc.bjjhwx.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://fc.shxzukj.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://oh.muxihuayi.cn

JS:   // child_process / cluster 模块
来源：http://mt.lnxyls.cn

TS:   // child_process / cluster 模块
来源：http://ve.lnxyls.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://st.521024.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://pp.nszjky.cn

Ruby: // fork 块
来源：http://em.nszjky.cn


<!-- 参考信息 -->