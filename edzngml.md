代发 wailian999

[L03] 设置自定义请求头
来源：http://ih.shxzukj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://uh.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wx.lnxyls.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bs.wgjwhj.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dv.hnjuh.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ei.shxzskj.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://cn.shtwfgs.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://er.asd995.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://uy.szxytkj.cn

[L04] 设置超时
来源：http://lc.wgjwhj.cn

Py:   requests.get(url, timeout=5)
来源：http://kr.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://as.bookmarksfly.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fd.panjiajie.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jl.jctech888.com.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ki.szsharing.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://kg.bookmarksfly.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://of.yuntaijiaju.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ts.huanxung.cn

[L05] 上传文件（multipart）
来源：http://us.szsharing.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://xo.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://xx.yuntaijiaju.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://co.nicolike.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://qt.hahajie.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mf.huanxung.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://rl.yuexingan06.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://xm.panjiajie.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://nb.hnjuh.cn

[L06] 解析响应为 JSON
来源：http://vi.9csxet.cn

Py:   resp.json()
来源：http://ny.hahajie.cn

PHP:  json_decode($body, true);
来源：http://dr.huixiangedu.cn

JS:   await resp.json()
来源：http://ar.newstarts.cn

TS:   await resp.json()
来源：http://cj.wgjwhj.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ke.huanxung.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://gu.szxytkj.cn

Ruby: JSON.parse(resp.body)
来源：http://ll.yuexingan06.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://qc.jctech888.com.cn

[L07] 处理 HTTP 状态码
来源：http://ee.huanxung.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://eg.9csxet.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hs.huixiangedu.cn

JS:   resp.ok;  resp.status
来源：http://yo.szsharing.cn

TS:   resp.ok;  resp.status
来源：http://bf.asd995.cn

Java: resp.statusCode()
来源：http://uw.colortex.cn

Go:   resp.StatusCode
来源：http://hv.hnjuh.cn

Ruby: resp.code.to_i
来源：http://zt.bookmarksfly.cn

C#:   (int)resp.StatusCode
来源：http://bs.haigaiapp.cn

[L08] 并发请求多个地址
来源：http://dd.hahajie.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hu.521024.cn

PHP:  curl_multi_init() 系列
来源：http://mi.shxzukj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gd.hahajie.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qw.huixiangedu.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://kv.huixinmuqiang.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ff.colortex.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://st.panjiajie.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://db.huixinmuqiang.cn

================================================================================
来源：http://hf.shtwfgs.cn

M. 命令行 / 进程 / 环境
来源：http://co.colortex.cn

================================================================================
来源：http://uh.haigaiapp.cn

[M01] 读取命令行参数
来源：http://ge.shxzukj.cn

Py:   sys.argv[1:]
来源：http://cp.521024.cn

PHP:  $argv;  $argc;
来源：http://ak.jctech888.com.cn

JS:   process.argv.slice(2)
来源：http://fp.shtwfgs.cn

TS:   process.argv.slice(2)
来源：http://cx.jctech888.com.cn

Java: args 数组（main 方法参数）
来源：http://eo.szxytkj.cn

Go:   os.Args[1:]
来源：http://un.jctech888.com.cn

Ruby: ARGV
来源：http://bv.huixiangedu.cn

C#:   args 数组（Main 方法参数）
来源：http://ru.nszjky.cn

[M02] 读取环境变量
来源：http://lj.shxzskj.cn

Py:   os.environ.get("HOME")
来源：http://dz.bjjhwx.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://oi.bookmarksfly.cn

JS:   process.env.HOME
来源：http://mz.haigaiapp.cn

TS:   process.env.HOME
来源：http://st.shtwfgs.cn

Java: System.getenv("HOME")
来源：http://qz.panjiajie.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://pn.colortex.cn

Ruby: ENV["HOME"]
来源：http://sy.shtwfgs.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://vi.shtwfgs.cn

[M03] 执行外部命令
来源：http://ln.hahajie.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://gm.muxihuayi.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ee.bookmarksfly.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://cw.bjjhwx.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ii.jianghongdianzi.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://tc.jianghongdianzi.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://mo.colortex.cn

Ruby: system("ls -l");  `ls -l`
来源：http://is.hahajie.cn

C#:   Process.Start("ls", "-l");
来源：http://us.nicolike.cn

[M04] 获取当前工作目录
来源：http://xi.panjiajie.cn

Py:   os.getcwd()
来源：http://wh.asd995.cn

PHP:  getcwd();
来源：http://zc.asd995.cn

JS:   process.cwd()
来源：http://kp.asd995.cn

TS:   process.cwd()
来源：http://do.yuntaijiaju.cn

Java: Path.of("").toAbsolutePath()
来源：http://re.9csxet.cn

Go:   os.Getwd()
来源：http://yg.shtwfgs.cn

Ruby: Dir.pwd
来源：http://rq.huixiangedu.cn

C#:   Directory.GetCurrentDirectory()
来源：http://zo.shtwfgs.cn

[M05] 设置退出码
来源：http://ox.9csxet.cn

Py:   sys.exit(1)
来源：http://hk.nszjky.cn

PHP:  exit(1);
来源：http://ae.huixiangedu.cn

JS:   process.exit(1)
来源：http://vq.bookmarksfly.cn

TS:   process.exit(1)
来源：http://wb.jctech888.com.cn

Java: System.exit(1)
来源：http://zj.huixiangedu.cn

Go:   os.Exit(1)
来源：http://qo.shxzukj.cn

Ruby: exit 1
来源：http://wd.hnjuh.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wz.nszjky.cn

[M06] 向标准错误输出
来源：http://zs.lnxyls.cn

Py:   print("err", file=sys.stderr)
来源：http://ry.shxzukj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://wq.521024.cn

JS:   console.error("err")
来源：http://vm.asd995.cn

TS:   console.error("err")
来源：http://xa.yuexingan06.cn

Java: System.err.println("err")
来源：http://hq.bookmarksfly.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ty.huixinmuqiang.cn

Ruby: warn "err"
来源：http://og.jianghongdianzi.cn

C#:   Console.Error.WriteLine("err")
来源：http://cp.wgjwhj.cn

[M07] 判断是否为主入口
来源：http://av.asd995.cn

Py:   if __name__ == "__main__":
来源：http://fe.shxzukj.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://dg.huixinmuqiang.cn

JS:   require.main === module
来源：http://nr.szxytkj.cn

TS:   require.main === module
来源：http://fu.chemitech.net.cn

Java: public static void main(String[] args)
来源：http://vy.nszjky.cn

Go:   func main()
来源：http://du.szxytkj.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://kz.panjiajie.cn

C#:   static void Main(string[] args)
来源：http://lh.jctech888.com.cn

[M08] 获取系统与运行时信息
来源：http://oi.9csxet.cn

Py:   platform.system();  platform.python_version()
来源：http://ta.jctech888.com.cn

PHP:  PHP_OS;  phpversion();
来源：http://hm.gzmigu.cn

JS:   process.platform;  process.version
来源：http://dp.shtwfgs.cn

TS:   process.platform;  process.version
来源：http://xz.yuexingan06.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://bn.huanxung.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ri.yuntaijiaju.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://kn.jctech888.com.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://tw.yuexingan06.cn

================================================================================
来源：http://jx.9csxet.cn

N. 数据结构与算法
来源：http://nx.521024.cn

================================================================================
来源：http://mc.nicolike.cn

[N01] 二分查找（有序数组）
来源：http://fn.bjjhwx.cn

Py:   bisect.bisect_left(arr, x)
来源：http://cm.wgjwhj.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://da.yuexingan06.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ig.lnxyls.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://te.yuexingan06.cn

Java: Arrays.binarySearch(arr, x)
来源：http://cd.nszjky.cn

Go:   sort.SearchInts(arr, x)
来源：http://zn.huanxung.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://xd.wgjwhj.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ks.haigaiapp.cn

[N02] 排序（工程实践用内置实现）
来源：http://hi.szsharing.cn

Py:   sorted(arr);  arr.sort()
来源：http://ui.muxihuayi.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wb.colortex.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://vq.lnxyls.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ar.huixinmuqiang.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://fl.szsharing.cn

Go:   slices.Sort(arr)
来源：http://td.lnxyls.cn

Ruby: arr.sort
来源：http://fn.gzmigu.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ir.bookmarksfly.cn

[N03] 快速排序（分治示例）
来源：http://bu.gzmigu.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://na.colortex.cn

PHP:  // 递归实现，或用 usort
来源：http://hi.szxytkj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dn.bookmarksfly.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ak.gzmigu.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://kr.jianghongdianzi.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ox.521024.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ib.haigaiapp.cn

C#:   // 手写递归，或 Array.Sort
来源：http://on.bookmarksfly.cn

[N04] 斐波那契数列
来源：http://fe.yuexingan06.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://nb.newstarts.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://xi.hnjuh.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cs.haigaiapp.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fj.yuntaijiaju.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://nt.9csxet.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://eo.shxzskj.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://le.haigaiapp.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://zi.colortex.cn

[N05] 最大公约数
来源：http://lv.haigaiapp.cn

Py:   math.gcd(a, b)
来源：http://bs.colortex.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ul.bookmarksfly.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rp.hnjuh.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ou.nicolike.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ze.szxytkj.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://gu.shxzukj.cn

Ruby: a.gcd(b)
来源：http://aw.lnxyls.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://oy.9csxet.cn

[N06] 判断回文字符串
来源：http://fc.9csxet.cn

Py:   s == s[::-1]
来源：http://mv.newstarts.cn

PHP:  $s === strrev($s);
来源：http://an.bjjhwx.cn

JS:   s === [...s].reverse().join("")
来源：http://bc.huanxung.cn

TS:   s === [...s].reverse().join("")
来源：http://sb.szsharing.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mt.gzmigu.cn

Go:   // 双指针从两端比较
来源：http://zl.nicolike.cn

Ruby: s == s.reverse
来源：http://ox.wgjwhj.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://jx.bjjhwx.cn

[N07] 两数之和（返回下标）
来源：http://ja.szxytkj.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://qi.bookmarksfly.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://lj.szsharing.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://zj.panjiajie.cn

TS:   // 手写 Map<string, number>
来源：http://tl.nszjky.cn

Java: // 手写 HashMap
来源：http://cb.9csxet.cn

Go:   // 手写 map[int]int
来源：http://ee.jctech888.com.cn

Ruby: // 手写 Hash
来源：http://xz.wgjwhj.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ub.521024.cn

[N08] 生成全排列
来源：http://oq.shxzukj.cn

Py:   itertools.permutations(arr)
来源：http://ul.chemitech.net.cn

PHP:  // 手写递归交换
来源：http://ra.newstarts.cn

JS:   // 手写回溯递归
来源：http://nl.yuntaijiaju.cn

TS:   // 手写回溯递归
来源：http://st.jianghongdianzi.cn

Java: // 手写回溯递归
来源：http://he.hnjuh.cn

Go:   // 手写回溯递归
来源：http://ik.yuntaijiaju.cn

Ruby: arr.permutation.to_a
来源：http://tb.haigaiapp.cn

C#:   // 手写回溯递归
来源：http://vp.shxzukj.cn

[N09] 栈与队列
来源：http://nd.lnxyls.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://vo.chemitech.net.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://sy.colortex.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://xf.szsharing.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://gr.shtwfgs.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wq.bjjhwx.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://fd.haigaiapp.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ov.szsharing.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ar.bookmarksfly.cn

[N10] 链表节点定义
来源：http://sa.jianghongdianzi.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://fw.colortex.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://wi.bookmarksfly.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wn.wgjwhj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://cv.panjiajie.cn

Java: class Node { int v; Node next; }
来源：http://sc.wgjwhj.cn

Go:   type Node struct { V int; Next *Node }
来源：http://wy.wgjwhj.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://av.shxzukj.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://kr.asd995.cn

[N11] 二叉树中序遍历
来源：http://bw.hahajie.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://sh.newstarts.cn

PHP:  // 手写递归函数
来源：http://gi.521024.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sv.hahajie.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lh.yuntaijiaju.cn

Java: // 手写递归
来源：http://qu.yuexingan06.cn

Go:   // 手写递归
来源：http://bt.chemitech.net.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://qk.nszjky.cn

C#:   // 手写递归
来源：http://dc.bookmarksfly.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wk.szsharing.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ng.lnxyls.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://yo.lnxyls.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wr.huixinmuqiang.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sz.haigaiapp.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mc.9csxet.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://gh.wgjwhj.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ow.lnxyls.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wh.gzmigu.cn

================================================================================
来源：http://tu.huixinmuqiang.cn

O. 并发与异步
来源：http://bd.shtwfgs.cn

================================================================================
来源：http://ek.jianghongdianzi.cn

[O01] 启动一个线程
来源：http://yl.nszjky.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ey.muxihuayi.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://xq.szsharing.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://pi.huixiangedu.cn

TS:   // 同 JS
来源：http://xt.newstarts.cn

Java: new Thread(() -> f()).start()
来源：http://tw.521024.cn

Go:   go f()
来源：http://km.szsharing.cn

Ruby: Thread.new { f }
来源：http://hw.shxzskj.cn

C#:   Task.Run(() => F());
来源：http://et.muxihuayi.cn

[O02] 使用线程池
来源：http://yt.yuexingan06.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://xu.wgjwhj.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ip.panjiajie.cn

JS:   // worker_threads 线程池
来源：http://cj.nszjky.cn

TS:   // worker_threads 线程池
来源：http://ao.lnxyls.cn

Java: Executors.newFixedThreadPool(4)
来源：http://yx.shxzskj.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://bo.colortex.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://rf.muxihuayi.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://jl.hahajie.cn

[O03] 加锁保护共享数据
来源：http://st.huanxung.cn

Py:   with lock: shared += 1
来源：http://fd.nszjky.cn

PHP:  // 用 flock() 做文件锁
来源：http://jc.yuntaijiaju.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://rp.lnxyls.cn

TS:   // 同 JS
来源：http://id.shxzukj.cn

Java: synchronized (this) { shared++; }
来源：http://dy.yuexingan06.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://pv.hahajie.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://hv.szxytkj.cn

C#:   lock (gate) { shared++; }
来源：http://fp.haigaiapp.cn

[O04] 定义异步函数并等待
来源：http://ss.shxzukj.cn

Py:   async def f():⏎    await g()
来源：http://gi.gzmigu.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://kw.haigaiapp.cn

JS:   async function f() { await g(); }
来源：http://hm.huixiangedu.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://om.jctech888.com.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://xk.gzmigu.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://zj.9csxet.cn

Ruby: # 用 Fiber 或 async gem
来源：http://nh.jianghongdianzi.cn

C#:   async Task F() { await G(); }
来源：http://qo.huixiangedu.cn

[O05] 并发执行并等待全部完成
来源：http://zi.chemitech.net.cn

Py:   asyncio.gather(*tasks)
来源：http://hy.huixinmuqiang.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://yz.newstarts.cn

JS:   await Promise.all(tasks)
来源：http://vl.shtwfgs.cn

TS:   await Promise.all(tasks)
来源：http://uy.shxzukj.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ih.bjjhwx.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://yz.colortex.cn

Ruby: threads.map(&:join)
来源：http://wc.chemitech.net.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://og.9csxet.cn

[O06] 使用进程池
来源：http://uy.shxzskj.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://bm.chemitech.net.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://kd.wgjwhj.cn

JS:   // child_process / cluster 模块
来源：http://nt.wgjwhj.cn

TS:   // child_process / cluster 模块
来源：http://cv.bookmarksfly.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ut.lnxyls.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wo.nicolike.cn

Ruby: // fork 块
来源：http://yw.muxihuayi.cn

C#:   Parallel.For
来源：http://vz.huanxung.cn

================================================================================
来源：http://on.newstarts.cn

P. 常用工具函数
来源：http://wh.colortex.cn

================================================================================
来源：http://on.gzmigu.cn


<!-- 参考信息 -->