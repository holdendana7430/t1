代发 wailian999

[L03] 设置自定义请求头
来源：http://md.yuntaijiaju.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://rc.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ty.lnxyls.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sj.yuntaijiaju.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ee.nszjky.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://dy.nszjky.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jz.nicolike.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://yr.nicolike.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://fx.panjiajie.cn

[L04] 设置超时
来源：http://pq.9csxet.cn

Py:   requests.get(url, timeout=5)
来源：http://qx.nszjky.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://de.szxytkj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wg.jctech888.com.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bv.newstarts.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://cq.panjiajie.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://jq.newstarts.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ir.szsharing.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://jv.haigaiapp.cn

[L05] 上传文件（multipart）
来源：http://pf.gzmigu.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://yl.yuntaijiaju.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://tr.huixiangedu.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ww.huixinmuqiang.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://em.yuexingan06.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ps.lnxyls.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://yd.yuexingan06.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://zk.wgjwhj.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://zl.colortex.cn

[L06] 解析响应为 JSON
来源：http://ih.asd995.cn

Py:   resp.json()
来源：http://pr.hnjuh.cn

PHP:  json_decode($body, true);
来源：http://vm.hnjuh.cn

JS:   await resp.json()
来源：http://xi.lnxyls.cn

TS:   await resp.json()
来源：http://nv.wgjwhj.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://zs.szsharing.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ta.szxytkj.cn

Ruby: JSON.parse(resp.body)
来源：http://zm.muxihuayi.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://dr.muxihuayi.cn

[L07] 处理 HTTP 状态码
来源：http://we.shxzukj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://pi.shtwfgs.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://yj.huixiangedu.cn

JS:   resp.ok;  resp.status
来源：http://yb.gzmigu.cn

TS:   resp.ok;  resp.status
来源：http://ih.bjjhwx.cn

Java: resp.statusCode()
来源：http://du.hnjuh.cn

Go:   resp.StatusCode
来源：http://wd.szsharing.cn

Ruby: resp.code.to_i
来源：http://hf.szxytkj.cn

C#:   (int)resp.StatusCode
来源：http://sf.panjiajie.cn

[L08] 并发请求多个地址
来源：http://px.nicolike.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ho.yuexingan06.cn

PHP:  curl_multi_init() 系列
来源：http://nx.szxytkj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rj.yuntaijiaju.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ux.yuexingan06.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://rw.nicolike.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://vo.huanxung.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://aq.lnxyls.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://kn.hnjuh.cn

================================================================================
来源：http://by.yuexingan06.cn

M. 命令行 / 进程 / 环境
来源：http://yw.huixiangedu.cn

================================================================================
来源：http://ve.hahajie.cn

[M01] 读取命令行参数
来源：http://ba.huanxung.cn

Py:   sys.argv[1:]
来源：http://em.nicolike.cn

PHP:  $argv;  $argc;
来源：http://ra.szxytkj.cn

JS:   process.argv.slice(2)
来源：http://re.hahajie.cn

TS:   process.argv.slice(2)
来源：http://on.chemitech.net.cn

Java: args 数组（main 方法参数）
来源：http://qe.panjiajie.cn

Go:   os.Args[1:]
来源：http://yl.colortex.cn

Ruby: ARGV
来源：http://cx.yuexingan06.cn

C#:   args 数组（Main 方法参数）
来源：http://it.haigaiapp.cn

[M02] 读取环境变量
来源：http://rz.huixinmuqiang.cn

Py:   os.environ.get("HOME")
来源：http://kv.bjjhwx.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hw.yuexingan06.cn

JS:   process.env.HOME
来源：http://ad.yuntaijiaju.cn

TS:   process.env.HOME
来源：http://fc.szxytkj.cn

Java: System.getenv("HOME")
来源：http://gy.shtwfgs.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://pf.huanxung.cn

Ruby: ENV["HOME"]
来源：http://gr.szxytkj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://iu.yuntaijiaju.cn

[M03] 执行外部命令
来源：http://fz.yuntaijiaju.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://bu.szsharing.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://fu.newstarts.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ei.9csxet.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://vu.bookmarksfly.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://fk.newstarts.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://us.yuntaijiaju.cn

Ruby: system("ls -l");  `ls -l`
来源：http://sv.bjjhwx.cn

C#:   Process.Start("ls", "-l");
来源：http://lq.chemitech.net.cn

[M04] 获取当前工作目录
来源：http://py.nszjky.cn

Py:   os.getcwd()
来源：http://wc.521024.cn

PHP:  getcwd();
来源：http://ze.shxzukj.cn

JS:   process.cwd()
来源：http://ja.colortex.cn

TS:   process.cwd()
来源：http://vc.panjiajie.cn

Java: Path.of("").toAbsolutePath()
来源：http://vc.shxzukj.cn

Go:   os.Getwd()
来源：http://ax.shxzukj.cn

Ruby: Dir.pwd
来源：http://ls.bjjhwx.cn

C#:   Directory.GetCurrentDirectory()
来源：http://zc.huixinmuqiang.cn

[M05] 设置退出码
来源：http://co.huanxung.cn

Py:   sys.exit(1)
来源：http://dv.haigaiapp.cn

PHP:  exit(1);
来源：http://hl.521024.cn

JS:   process.exit(1)
来源：http://kc.9csxet.cn

TS:   process.exit(1)
来源：http://ui.9csxet.cn

Java: System.exit(1)
来源：http://oo.hahajie.cn

Go:   os.Exit(1)
来源：http://fr.wgjwhj.cn

Ruby: exit 1
来源：http://ie.yuntaijiaju.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://nz.huanxung.cn

[M06] 向标准错误输出
来源：http://ef.hnjuh.cn

Py:   print("err", file=sys.stderr)
来源：http://pk.muxihuayi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://tw.huixiangedu.cn

JS:   console.error("err")
来源：http://ru.bjjhwx.cn

TS:   console.error("err")
来源：http://cv.chemitech.net.cn

Java: System.err.println("err")
来源：http://ju.newstarts.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://xk.huixiangedu.cn

Ruby: warn "err"
来源：http://ch.521024.cn

C#:   Console.Error.WriteLine("err")
来源：http://zj.newstarts.cn

[M07] 判断是否为主入口
来源：http://la.521024.cn

Py:   if __name__ == "__main__":
来源：http://vg.chemitech.net.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://tw.jctech888.com.cn

JS:   require.main === module
来源：http://qx.hnjuh.cn

TS:   require.main === module
来源：http://ym.9csxet.cn

Java: public static void main(String[] args)
来源：http://ma.huanxung.cn

Go:   func main()
来源：http://nv.521024.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://rc.yuexingan06.cn

C#:   static void Main(string[] args)
来源：http://jg.gzmigu.cn

[M08] 获取系统与运行时信息
来源：http://ue.newstarts.cn

Py:   platform.system();  platform.python_version()
来源：http://kt.muxihuayi.cn

PHP:  PHP_OS;  phpversion();
来源：http://wy.shtwfgs.cn

JS:   process.platform;  process.version
来源：http://am.panjiajie.cn

TS:   process.platform;  process.version
来源：http://rz.chemitech.net.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://tl.chemitech.net.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://fr.chemitech.net.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ps.hnjuh.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://qn.bookmarksfly.cn

================================================================================
来源：http://um.shtwfgs.cn

N. 数据结构与算法
来源：http://dc.jctech888.com.cn

================================================================================
来源：http://nx.szxytkj.cn

[N01] 二分查找（有序数组）
来源：http://oy.yuntaijiaju.cn

Py:   bisect.bisect_left(arr, x)
来源：http://kg.panjiajie.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://zu.shxzskj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://km.asd995.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ma.chemitech.net.cn

Java: Arrays.binarySearch(arr, x)
来源：http://qu.szsharing.cn

Go:   sort.SearchInts(arr, x)
来源：http://cw.bookmarksfly.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ue.jctech888.com.cn

C#:   Array.BinarySearch(arr, x)
来源：http://an.newstarts.cn

[N02] 排序（工程实践用内置实现）
来源：http://ze.muxihuayi.cn

Py:   sorted(arr);  arr.sort()
来源：http://ly.chemitech.net.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://sk.shtwfgs.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://dp.wgjwhj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://dg.bjjhwx.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://io.521024.cn

Go:   slices.Sort(arr)
来源：http://ep.bjjhwx.cn

Ruby: arr.sort
来源：http://ka.yuntaijiaju.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://cy.wgjwhj.cn

[N03] 快速排序（分治示例）
来源：http://bo.szxytkj.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://tq.9csxet.cn

PHP:  // 递归实现，或用 usort
来源：http://my.haigaiapp.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ci.bookmarksfly.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kx.shxzukj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://dh.szsharing.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://vj.panjiajie.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xu.shtwfgs.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ac.nicolike.cn

[N04] 斐波那契数列
来源：http://ox.jianghongdianzi.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://sm.shtwfgs.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://qz.panjiajie.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tm.shxzukj.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://oa.wgjwhj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://zr.gzmigu.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://fv.haigaiapp.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://kh.huixinmuqiang.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://zz.yuntaijiaju.cn

[N05] 最大公约数
来源：http://ru.jianghongdianzi.cn

Py:   math.gcd(a, b)
来源：http://ch.yuntaijiaju.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://uc.shxzskj.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tl.9csxet.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vp.chemitech.net.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mn.hahajie.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ka.haigaiapp.cn

Ruby: a.gcd(b)
来源：http://vr.huixinmuqiang.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://va.jctech888.com.cn

[N06] 判断回文字符串
来源：http://tq.9csxet.cn

Py:   s == s[::-1]
来源：http://wj.huixinmuqiang.cn

PHP:  $s === strrev($s);
来源：http://dk.jianghongdianzi.cn

JS:   s === [...s].reverse().join("")
来源：http://gs.hahajie.cn

TS:   s === [...s].reverse().join("")
来源：http://ug.huanxung.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ij.haigaiapp.cn

Go:   // 双指针从两端比较
来源：http://ye.szxytkj.cn

Ruby: s == s.reverse
来源：http://uv.haigaiapp.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://vx.newstarts.cn

[N07] 两数之和（返回下标）
来源：http://gr.huixiangedu.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://dq.panjiajie.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://oj.hnjuh.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://kz.newstarts.cn

TS:   // 手写 Map<string, number>
来源：http://es.yuntaijiaju.cn

Java: // 手写 HashMap
来源：http://ib.jianghongdianzi.cn

Go:   // 手写 map[int]int
来源：http://pg.szsharing.cn

Ruby: // 手写 Hash
来源：http://zv.jctech888.com.cn

C#:   // 手写 Dictionary<int, int>
来源：http://yx.nszjky.cn

[N08] 生成全排列
来源：http://ap.shxzskj.cn

Py:   itertools.permutations(arr)
来源：http://zb.bookmarksfly.cn

PHP:  // 手写递归交换
来源：http://mb.9csxet.cn

JS:   // 手写回溯递归
来源：http://zg.bookmarksfly.cn

TS:   // 手写回溯递归
来源：http://ow.yuexingan06.cn

Java: // 手写回溯递归
来源：http://al.jctech888.com.cn

Go:   // 手写回溯递归
来源：http://re.huixinmuqiang.cn

Ruby: arr.permutation.to_a
来源：http://rm.bjjhwx.cn

C#:   // 手写回溯递归
来源：http://zx.hahajie.cn

[N09] 栈与队列
来源：http://yv.yuntaijiaju.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://zj.jianghongdianzi.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ti.haigaiapp.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://vd.szsharing.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ey.haigaiapp.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://gr.jctech888.com.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://su.bjjhwx.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hs.huixiangedu.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://qo.newstarts.cn

[N10] 链表节点定义
来源：http://fc.521024.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://uz.haigaiapp.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ox.jctech888.com.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://sa.jctech888.com.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://pq.nicolike.cn

Java: class Node { int v; Node next; }
来源：http://po.szxytkj.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ud.huanxung.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ox.shxzukj.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://xt.asd995.cn

[N11] 二叉树中序遍历
来源：http://bb.9csxet.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://jy.bookmarksfly.cn

PHP:  // 手写递归函数
来源：http://ow.szsharing.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mw.yuexingan06.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ge.lnxyls.cn

Java: // 手写递归
来源：http://mo.shxzukj.cn

Go:   // 手写递归
来源：http://jl.gzmigu.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ry.panjiajie.cn

C#:   // 手写递归
来源：http://xu.9csxet.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ru.asd995.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://em.asd995.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://zx.haigaiapp.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://uk.hnjuh.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wv.nicolike.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://zk.huanxung.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://nw.newstarts.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://yd.hnjuh.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://yf.lnxyls.cn

================================================================================
来源：http://bq.shxzukj.cn

O. 并发与异步
来源：http://vx.huixiangedu.cn

================================================================================
来源：http://mh.nszjky.cn

[O01] 启动一个线程
来源：http://rd.muxihuayi.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ka.lnxyls.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://xi.jctech888.com.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ph.huanxung.cn

TS:   // 同 JS
来源：http://uj.huanxung.cn

Java: new Thread(() -> f()).start()
来源：http://bx.muxihuayi.cn

Go:   go f()
来源：http://vz.shxzskj.cn

Ruby: Thread.new { f }
来源：http://wq.hahajie.cn

C#:   Task.Run(() => F());
来源：http://xd.panjiajie.cn

[O02] 使用线程池
来源：http://jc.bjjhwx.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://un.huanxung.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://tw.shxzskj.cn

JS:   // worker_threads 线程池
来源：http://tn.muxihuayi.cn

TS:   // worker_threads 线程池
来源：http://yt.bjjhwx.cn

Java: Executors.newFixedThreadPool(4)
来源：http://pn.chemitech.net.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://cc.asd995.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://zg.shxzukj.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://gl.huanxung.cn

[O03] 加锁保护共享数据
来源：http://eb.hnjuh.cn

Py:   with lock: shared += 1
来源：http://hs.bookmarksfly.cn

PHP:  // 用 flock() 做文件锁
来源：http://ce.bjjhwx.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://va.yuexingan06.cn

TS:   // 同 JS
来源：http://qg.nicolike.cn

Java: synchronized (this) { shared++; }
来源：http://ed.muxihuayi.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://vs.shxzskj.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://dv.jianghongdianzi.cn

C#:   lock (gate) { shared++; }
来源：http://da.huanxung.cn

[O04] 定义异步函数并等待
来源：http://tu.jctech888.com.cn

Py:   async def f():⏎    await g()
来源：http://hu.asd995.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ld.nszjky.cn

JS:   async function f() { await g(); }
来源：http://cw.shtwfgs.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://zb.yuexingan06.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://nq.szxytkj.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://iu.bjjhwx.cn

Ruby: # 用 Fiber 或 async gem
来源：http://wa.haigaiapp.cn

C#:   async Task F() { await G(); }
来源：http://of.9csxet.cn

[O05] 并发执行并等待全部完成
来源：http://fu.521024.cn

Py:   asyncio.gather(*tasks)
来源：http://ut.shxzukj.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://tl.shtwfgs.cn

JS:   await Promise.all(tasks)
来源：http://px.huixiangedu.cn

TS:   await Promise.all(tasks)
来源：http://bx.yuexingan06.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://cv.szxytkj.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://cj.huixinmuqiang.cn

Ruby: threads.map(&:join)
来源：http://ru.huixiangedu.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ee.wgjwhj.cn

[O06] 使用进程池
来源：http://ox.huixinmuqiang.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wz.huixinmuqiang.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ps.bjjhwx.cn

JS:   // child_process / cluster 模块
来源：http://mc.huixinmuqiang.cn

TS:   // child_process / cluster 模块
来源：http://tx.bookmarksfly.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ja.huanxung.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://jd.yuntaijiaju.cn

Ruby: // fork 块
来源：http://wg.szsharing.cn

C#:   Parallel.For
来源：http://dv.bjjhwx.cn

================================================================================
来源：http://fj.colortex.cn

P. 常用工具函数
来源：http://sw.shxzskj.cn

================================================================================
来源：http://br.bjjhwx.cn


<!-- 参考信息 -->