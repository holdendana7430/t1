代发 wailian999

[L03] 设置自定义请求头
来源：http://md.szsharing.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://je.szxytkj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ma.gzmigu.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ti.nicolike.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zo.szxytkj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ee.jctech888.com.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://xp.hahajie.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://dv.lnxyls.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://zr.chemitech.net.cn

[L04] 设置超时
来源：http://hf.lnxyls.cn

Py:   requests.get(url, timeout=5)
来源：http://av.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://yg.asd995.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://aq.hahajie.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gj.wgjwhj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://gu.bjjhwx.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://rx.gzmigu.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://pi.colortex.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://yx.newstarts.cn

[L05] 上传文件（multipart）
来源：http://lb.panjiajie.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://dy.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://gf.bookmarksfly.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://jb.asd995.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://iz.hahajie.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vk.muxihuayi.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://li.shxzukj.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://yr.panjiajie.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://vu.haigaiapp.cn

[L06] 解析响应为 JSON
来源：http://yy.bookmarksfly.cn

Py:   resp.json()
来源：http://ex.wgjwhj.cn

PHP:  json_decode($body, true);
来源：http://ii.9csxet.cn

JS:   await resp.json()
来源：http://pn.nicolike.cn

TS:   await resp.json()
来源：http://an.yuexingan06.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://sd.hahajie.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mn.shtwfgs.cn

Ruby: JSON.parse(resp.body)
来源：http://uj.jctech888.com.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://zj.shxzukj.cn

[L07] 处理 HTTP 状态码
来源：http://ar.gzmigu.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://gy.yuexingan06.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://kc.bjjhwx.cn

JS:   resp.ok;  resp.status
来源：http://vf.asd995.cn

TS:   resp.ok;  resp.status
来源：http://es.haigaiapp.cn

Java: resp.statusCode()
来源：http://va.haigaiapp.cn

Go:   resp.StatusCode
来源：http://ec.jianghongdianzi.cn

Ruby: resp.code.to_i
来源：http://lo.asd995.cn

C#:   (int)resp.StatusCode
来源：http://yt.gzmigu.cn

[L08] 并发请求多个地址
来源：http://tq.jctech888.com.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://zz.asd995.cn

PHP:  curl_multi_init() 系列
来源：http://xc.newstarts.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ns.nicolike.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fa.9csxet.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://pa.hahajie.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://eu.nicolike.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://qt.shtwfgs.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://qz.newstarts.cn

================================================================================
来源：http://hd.nszjky.cn

M. 命令行 / 进程 / 环境
来源：http://fd.hahajie.cn

================================================================================
来源：http://tf.huixinmuqiang.cn

[M01] 读取命令行参数
来源：http://nf.jctech888.com.cn

Py:   sys.argv[1:]
来源：http://xi.yuntaijiaju.cn

PHP:  $argv;  $argc;
来源：http://ni.asd995.cn

JS:   process.argv.slice(2)
来源：http://dp.colortex.cn

TS:   process.argv.slice(2)
来源：http://yv.newstarts.cn

Java: args 数组（main 方法参数）
来源：http://uq.bookmarksfly.cn

Go:   os.Args[1:]
来源：http://xg.jctech888.com.cn

Ruby: ARGV
来源：http://pr.yuntaijiaju.cn

C#:   args 数组（Main 方法参数）
来源：http://ey.gzmigu.cn

[M02] 读取环境变量
来源：http://ma.szxytkj.cn

Py:   os.environ.get("HOME")
来源：http://ki.chemitech.net.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://qi.bookmarksfly.cn

JS:   process.env.HOME
来源：http://lx.colortex.cn

TS:   process.env.HOME
来源：http://ns.521024.cn

Java: System.getenv("HOME")
来源：http://ol.huixiangedu.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mg.panjiajie.cn

Ruby: ENV["HOME"]
来源：http://ky.chemitech.net.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ej.jianghongdianzi.cn

[M03] 执行外部命令
来源：http://ys.shtwfgs.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://rh.haigaiapp.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://dp.nicolike.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://sa.newstarts.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://az.yuntaijiaju.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://nt.huixinmuqiang.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://db.newstarts.cn

Ruby: system("ls -l");  `ls -l`
来源：http://xy.bookmarksfly.cn

C#:   Process.Start("ls", "-l");
来源：http://vf.newstarts.cn

[M04] 获取当前工作目录
来源：http://eo.bookmarksfly.cn

Py:   os.getcwd()
来源：http://gy.nszjky.cn

PHP:  getcwd();
来源：http://nv.muxihuayi.cn

JS:   process.cwd()
来源：http://zl.yuexingan06.cn

TS:   process.cwd()
来源：http://oj.jctech888.com.cn

Java: Path.of("").toAbsolutePath()
来源：http://gr.asd995.cn

Go:   os.Getwd()
来源：http://oj.jctech888.com.cn

Ruby: Dir.pwd
来源：http://ox.bjjhwx.cn

C#:   Directory.GetCurrentDirectory()
来源：http://od.huixiangedu.cn

[M05] 设置退出码
来源：http://se.hahajie.cn

Py:   sys.exit(1)
来源：http://kj.hnjuh.cn

PHP:  exit(1);
来源：http://px.yuntaijiaju.cn

JS:   process.exit(1)
来源：http://wt.jctech888.com.cn

TS:   process.exit(1)
来源：http://mx.nszjky.cn

Java: System.exit(1)
来源：http://lq.colortex.cn

Go:   os.Exit(1)
来源：http://sl.colortex.cn

Ruby: exit 1
来源：http://xm.colortex.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://nx.colortex.cn

[M06] 向标准错误输出
来源：http://ut.shtwfgs.cn

Py:   print("err", file=sys.stderr)
来源：http://pv.huixiangedu.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://hx.chemitech.net.cn

JS:   console.error("err")
来源：http://da.shxzukj.cn

TS:   console.error("err")
来源：http://gi.521024.cn

Java: System.err.println("err")
来源：http://ps.huanxung.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://td.hnjuh.cn

Ruby: warn "err"
来源：http://kk.jctech888.com.cn

C#:   Console.Error.WriteLine("err")
来源：http://yp.yuntaijiaju.cn

[M07] 判断是否为主入口
来源：http://kj.jctech888.com.cn

Py:   if __name__ == "__main__":
来源：http://js.panjiajie.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://uk.haigaiapp.cn

JS:   require.main === module
来源：http://jw.colortex.cn

TS:   require.main === module
来源：http://lt.chemitech.net.cn

Java: public static void main(String[] args)
来源：http://fo.hnjuh.cn

Go:   func main()
来源：http://ne.gzmigu.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://yb.colortex.cn

C#:   static void Main(string[] args)
来源：http://wc.shxzukj.cn

[M08] 获取系统与运行时信息
来源：http://bn.bookmarksfly.cn

Py:   platform.system();  platform.python_version()
来源：http://ug.nszjky.cn

PHP:  PHP_OS;  phpversion();
来源：http://cr.lnxyls.cn

JS:   process.platform;  process.version
来源：http://kh.huixiangedu.cn

TS:   process.platform;  process.version
来源：http://jq.colortex.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://et.9csxet.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ms.huanxung.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ga.huixiangedu.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://zu.colortex.cn

================================================================================
来源：http://dy.hahajie.cn

N. 数据结构与算法
来源：http://vz.jctech888.com.cn

================================================================================
来源：http://ib.yuntaijiaju.cn

[N01] 二分查找（有序数组）
来源：http://yi.shtwfgs.cn

Py:   bisect.bisect_left(arr, x)
来源：http://zz.shtwfgs.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://gi.nicolike.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pc.9csxet.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pz.szsharing.cn

Java: Arrays.binarySearch(arr, x)
来源：http://qb.9csxet.cn

Go:   sort.SearchInts(arr, x)
来源：http://ey.huanxung.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://rv.szsharing.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ig.huanxung.cn

[N02] 排序（工程实践用内置实现）
来源：http://mi.shxzukj.cn

Py:   sorted(arr);  arr.sort()
来源：http://hi.chemitech.net.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://gi.bjjhwx.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ed.hnjuh.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://lf.huanxung.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://td.shxzukj.cn

Go:   slices.Sort(arr)
来源：http://vc.panjiajie.cn

Ruby: arr.sort
来源：http://bj.shxzukj.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://md.wgjwhj.cn

[N03] 快速排序（分治示例）
来源：http://uw.hnjuh.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://od.szxytkj.cn

PHP:  // 递归实现，或用 usort
来源：http://xs.yuntaijiaju.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qg.muxihuayi.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lk.wgjwhj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wb.huanxung.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wn.newstarts.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://fx.jctech888.com.cn

C#:   // 手写递归，或 Array.Sort
来源：http://xc.wgjwhj.cn

[N04] 斐波那契数列
来源：http://ln.shxzskj.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://be.gzmigu.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://nt.panjiajie.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ou.hahajie.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hb.hahajie.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://io.gzmigu.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ka.newstarts.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ot.bjjhwx.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ue.jianghongdianzi.cn

[N05] 最大公约数
来源：http://vm.nicolike.cn

Py:   math.gcd(a, b)
来源：http://sp.hahajie.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wk.panjiajie.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pi.shtwfgs.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ct.bjjhwx.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://sr.jctech888.com.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://il.shxzukj.cn

Ruby: a.gcd(b)
来源：http://hq.huixiangedu.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wm.bookmarksfly.cn

[N06] 判断回文字符串
来源：http://uh.muxihuayi.cn

Py:   s == s[::-1]
来源：http://pz.huixinmuqiang.cn

PHP:  $s === strrev($s);
来源：http://mw.521024.cn

JS:   s === [...s].reverse().join("")
来源：http://tq.hahajie.cn

TS:   s === [...s].reverse().join("")
来源：http://cg.shxzukj.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mv.yuexingan06.cn

Go:   // 双指针从两端比较
来源：http://jw.szsharing.cn

Ruby: s == s.reverse
来源：http://ab.huixiangedu.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://gh.shxzukj.cn

[N07] 两数之和（返回下标）
来源：http://mk.panjiajie.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://sg.asd995.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ru.9csxet.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://sz.shxzukj.cn

TS:   // 手写 Map<string, number>
来源：http://uf.bjjhwx.cn

Java: // 手写 HashMap
来源：http://ip.yuexingan06.cn

Go:   // 手写 map[int]int
来源：http://di.colortex.cn

Ruby: // 手写 Hash
来源：http://xn.gzmigu.cn

C#:   // 手写 Dictionary<int, int>
来源：http://bd.szxytkj.cn

[N08] 生成全排列
来源：http://fk.muxihuayi.cn

Py:   itertools.permutations(arr)
来源：http://oe.yuntaijiaju.cn

PHP:  // 手写递归交换
来源：http://yy.wgjwhj.cn

JS:   // 手写回溯递归
来源：http://rq.shxzskj.cn

TS:   // 手写回溯递归
来源：http://iw.huixiangedu.cn

Java: // 手写回溯递归
来源：http://un.jctech888.com.cn

Go:   // 手写回溯递归
来源：http://cn.521024.cn

Ruby: arr.permutation.to_a
来源：http://ar.hnjuh.cn

C#:   // 手写回溯递归
来源：http://wv.yuexingan06.cn

[N09] 栈与队列
来源：http://ue.lnxyls.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://vx.bjjhwx.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://kf.jctech888.com.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ye.huixiangedu.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mv.bjjhwx.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ue.gzmigu.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ey.chemitech.net.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://eh.shxzukj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://pj.colortex.cn

[N10] 链表节点定义
来源：http://ww.jctech888.com.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://kt.asd995.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://if.nszjky.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hc.gzmigu.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://qf.shxzukj.cn

Java: class Node { int v; Node next; }
来源：http://ii.hnjuh.cn

Go:   type Node struct { V int; Next *Node }
来源：http://mq.jianghongdianzi.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://mj.bookmarksfly.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://lu.haigaiapp.cn

[N11] 二叉树中序遍历
来源：http://kx.gzmigu.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://vk.9csxet.cn

PHP:  // 手写递归函数
来源：http://jm.huanxung.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://za.bjjhwx.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://uz.colortex.cn

Java: // 手写递归
来源：http://ay.jianghongdianzi.cn

Go:   // 手写递归
来源：http://md.521024.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://zv.colortex.cn

C#:   // 手写递归
来源：http://pk.haigaiapp.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ko.muxihuayi.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ld.colortex.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://kp.jianghongdianzi.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mk.9csxet.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://iw.jianghongdianzi.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://qq.shtwfgs.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://gy.huixiangedu.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://fj.wgjwhj.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://dd.haigaiapp.cn

================================================================================
来源：http://ee.chemitech.net.cn

O. 并发与异步
来源：http://ld.lnxyls.cn

================================================================================
来源：http://em.hnjuh.cn

[O01] 启动一个线程
来源：http://tj.chemitech.net.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ea.hahajie.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://vf.szsharing.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://nr.shxzukj.cn

TS:   // 同 JS
来源：http://fa.bookmarksfly.cn

Java: new Thread(() -> f()).start()
来源：http://yx.yuexingan06.cn

Go:   go f()
来源：http://ym.lnxyls.cn

Ruby: Thread.new { f }
来源：http://ck.521024.cn

C#:   Task.Run(() => F());
来源：http://sx.colortex.cn

[O02] 使用线程池
来源：http://dj.huanxung.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ig.nszjky.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://jp.jctech888.com.cn

JS:   // worker_threads 线程池
来源：http://nt.yuntaijiaju.cn

TS:   // worker_threads 线程池
来源：http://qb.colortex.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ey.panjiajie.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://gx.wgjwhj.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ne.gzmigu.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://zz.9csxet.cn

[O03] 加锁保护共享数据
来源：http://jw.wgjwhj.cn

Py:   with lock: shared += 1
来源：http://ea.huanxung.cn

PHP:  // 用 flock() 做文件锁
来源：http://ph.szsharing.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://bg.bjjhwx.cn

TS:   // 同 JS
来源：http://bb.yuntaijiaju.cn

Java: synchronized (this) { shared++; }
来源：http://zz.asd995.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://bv.jianghongdianzi.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ri.bjjhwx.cn

C#:   lock (gate) { shared++; }
来源：http://xr.jctech888.com.cn

[O04] 定义异步函数并等待
来源：http://ri.huanxung.cn

Py:   async def f():⏎    await g()
来源：http://wv.wgjwhj.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://kp.wgjwhj.cn

JS:   async function f() { await g(); }
来源：http://xp.shtwfgs.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ei.shxzskj.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://go.muxihuayi.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://kx.nicolike.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ik.szxytkj.cn

C#:   async Task F() { await G(); }
来源：http://sx.newstarts.cn

[O05] 并发执行并等待全部完成
来源：http://rz.jianghongdianzi.cn

Py:   asyncio.gather(*tasks)
来源：http://kf.hnjuh.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://jd.huanxung.cn

JS:   await Promise.all(tasks)
来源：http://ah.panjiajie.cn

TS:   await Promise.all(tasks)
来源：http://oq.shxzukj.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wz.shxzukj.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://tz.chemitech.net.cn

Ruby: threads.map(&:join)
来源：http://cb.haigaiapp.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://qi.szsharing.cn

[O06] 使用进程池
来源：http://dz.shxzukj.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mg.huixinmuqiang.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://sm.hahajie.cn

JS:   // child_process / cluster 模块
来源：http://ur.nicolike.cn

TS:   // child_process / cluster 模块
来源：http://xi.huixinmuqiang.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://uf.colortex.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://da.haigaiapp.cn

Ruby: // fork 块
来源：http://zv.wgjwhj.cn

C#:   Parallel.For
来源：http://em.yuexingan06.cn

================================================================================
来源：http://cp.nszjky.cn

P. 常用工具函数
来源：http://we.shxzskj.cn

================================================================================
来源：http://kn.shxzskj.cn


<!-- 参考信息 -->