代发 wailian999

[L03] 设置自定义请求头
来源：http://qu.jctech888.com.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://qi.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://sh.521024.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mq.haigaiapp.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://oq.chemitech.net.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://pe.yuexingan06.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://oc.shxzskj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ka.asd995.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://vi.szxytkj.cn

[L04] 设置超时
来源：http://dr.yuntaijiaju.cn

Py:   requests.get(url, timeout=5)
来源：http://hr.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://nk.szsharing.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://on.9csxet.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pw.nicolike.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qt.haigaiapp.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fj.huanxung.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ba.nszjky.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ny.521024.cn

[L05] 上传文件（multipart）
来源：http://bl.asd995.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://yv.shtwfgs.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mc.szsharing.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://tu.hahajie.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://jj.gzmigu.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ca.lnxyls.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://jr.panjiajie.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://tm.szsharing.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://rv.asd995.cn

[L06] 解析响应为 JSON
来源：http://da.szsharing.cn

Py:   resp.json()
来源：http://wt.panjiajie.cn

PHP:  json_decode($body, true);
来源：http://pg.bjjhwx.cn

JS:   await resp.json()
来源：http://og.chemitech.net.cn

TS:   await resp.json()
来源：http://rt.haigaiapp.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ah.huixinmuqiang.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://kv.wgjwhj.cn

Ruby: JSON.parse(resp.body)
来源：http://zb.haigaiapp.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://yi.521024.cn

[L07] 处理 HTTP 状态码
来源：http://qu.huixiangedu.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://is.szxytkj.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://sx.bjjhwx.cn

JS:   resp.ok;  resp.status
来源：http://xf.muxihuayi.cn

TS:   resp.ok;  resp.status
来源：http://uu.hnjuh.cn

Java: resp.statusCode()
来源：http://pz.newstarts.cn

Go:   resp.StatusCode
来源：http://dc.yuntaijiaju.cn

Ruby: resp.code.to_i
来源：http://sv.bookmarksfly.cn

C#:   (int)resp.StatusCode
来源：http://wf.panjiajie.cn

[L08] 并发请求多个地址
来源：http://ty.huixinmuqiang.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://vs.shxzskj.cn

PHP:  curl_multi_init() 系列
来源：http://yf.bjjhwx.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cs.hahajie.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kq.521024.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://pj.hnjuh.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://gv.jctech888.com.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://kv.colortex.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ug.huixiangedu.cn

================================================================================
来源：http://om.muxihuayi.cn

M. 命令行 / 进程 / 环境
来源：http://xl.jianghongdianzi.cn

================================================================================
来源：http://ky.521024.cn

[M01] 读取命令行参数
来源：http://be.9csxet.cn

Py:   sys.argv[1:]
来源：http://fr.huixiangedu.cn

PHP:  $argv;  $argc;
来源：http://fk.huanxung.cn

JS:   process.argv.slice(2)
来源：http://ak.huanxung.cn

TS:   process.argv.slice(2)
来源：http://pf.szsharing.cn

Java: args 数组（main 方法参数）
来源：http://kr.shtwfgs.cn

Go:   os.Args[1:]
来源：http://cx.521024.cn

Ruby: ARGV
来源：http://fv.bjjhwx.cn

C#:   args 数组（Main 方法参数）
来源：http://hl.newstarts.cn

[M02] 读取环境变量
来源：http://zp.panjiajie.cn

Py:   os.environ.get("HOME")
来源：http://nn.colortex.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ov.shtwfgs.cn

JS:   process.env.HOME
来源：http://vs.jctech888.com.cn

TS:   process.env.HOME
来源：http://vi.chemitech.net.cn

Java: System.getenv("HOME")
来源：http://ti.asd995.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://kn.haigaiapp.cn

Ruby: ENV["HOME"]
来源：http://hp.chemitech.net.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://if.yuexingan06.cn

[M03] 执行外部命令
来源：http://nl.nszjky.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://if.hahajie.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://yn.9csxet.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://na.nszjky.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://jw.haigaiapp.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://gq.wgjwhj.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ss.szxytkj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://qn.shtwfgs.cn

C#:   Process.Start("ls", "-l");
来源：http://mk.chemitech.net.cn

[M04] 获取当前工作目录
来源：http://zb.haigaiapp.cn

Py:   os.getcwd()
来源：http://va.jctech888.com.cn

PHP:  getcwd();
来源：http://fc.shxzukj.cn

JS:   process.cwd()
来源：http://yx.haigaiapp.cn

TS:   process.cwd()
来源：http://ex.nszjky.cn

Java: Path.of("").toAbsolutePath()
来源：http://ev.nszjky.cn

Go:   os.Getwd()
来源：http://cl.jianghongdianzi.cn

Ruby: Dir.pwd
来源：http://oa.yuntaijiaju.cn

C#:   Directory.GetCurrentDirectory()
来源：http://nh.colortex.cn

[M05] 设置退出码
来源：http://gw.bookmarksfly.cn

Py:   sys.exit(1)
来源：http://zz.szsharing.cn

PHP:  exit(1);
来源：http://ai.haigaiapp.cn

JS:   process.exit(1)
来源：http://ev.shxzukj.cn

TS:   process.exit(1)
来源：http://ms.521024.cn

Java: System.exit(1)
来源：http://ey.shxzskj.cn

Go:   os.Exit(1)
来源：http://ru.yuntaijiaju.cn

Ruby: exit 1
来源：http://va.nszjky.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ez.yuntaijiaju.cn

[M06] 向标准错误输出
来源：http://st.szxytkj.cn

Py:   print("err", file=sys.stderr)
来源：http://uk.lnxyls.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://jk.hahajie.cn

JS:   console.error("err")
来源：http://jr.521024.cn

TS:   console.error("err")
来源：http://zp.huanxung.cn

Java: System.err.println("err")
来源：http://go.asd995.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ia.newstarts.cn

Ruby: warn "err"
来源：http://dg.nicolike.cn

C#:   Console.Error.WriteLine("err")
来源：http://wz.jianghongdianzi.cn

[M07] 判断是否为主入口
来源：http://gk.shtwfgs.cn

Py:   if __name__ == "__main__":
来源：http://sq.colortex.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://uf.chemitech.net.cn

JS:   require.main === module
来源：http://wr.9csxet.cn

TS:   require.main === module
来源：http://if.hnjuh.cn

Java: public static void main(String[] args)
来源：http://su.shtwfgs.cn

Go:   func main()
来源：http://ns.szxytkj.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://xu.shtwfgs.cn

C#:   static void Main(string[] args)
来源：http://wf.colortex.cn

[M08] 获取系统与运行时信息
来源：http://wx.nicolike.cn

Py:   platform.system();  platform.python_version()
来源：http://yq.nszjky.cn

PHP:  PHP_OS;  phpversion();
来源：http://lw.9csxet.cn

JS:   process.platform;  process.version
来源：http://tn.jctech888.com.cn

TS:   process.platform;  process.version
来源：http://bm.bjjhwx.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://sl.newstarts.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ap.szsharing.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ue.jianghongdianzi.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://al.jianghongdianzi.cn

================================================================================
来源：http://hp.yuexingan06.cn

N. 数据结构与算法
来源：http://wr.newstarts.cn

================================================================================
来源：http://sd.lnxyls.cn

[N01] 二分查找（有序数组）
来源：http://pf.gzmigu.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ws.asd995.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ka.bjjhwx.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zu.szsharing.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fu.chemitech.net.cn

Java: Arrays.binarySearch(arr, x)
来源：http://wg.521024.cn

Go:   sort.SearchInts(arr, x)
来源：http://du.panjiajie.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://up.colortex.cn

C#:   Array.BinarySearch(arr, x)
来源：http://dr.9csxet.cn

[N02] 排序（工程实践用内置实现）
来源：http://wj.jianghongdianzi.cn

Py:   sorted(arr);  arr.sort()
来源：http://mx.yuntaijiaju.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://jw.chemitech.net.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://qm.huanxung.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://de.szsharing.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://dd.9csxet.cn

Go:   slices.Sort(arr)
来源：http://hl.9csxet.cn

Ruby: arr.sort
来源：http://ug.shxzskj.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://pp.hnjuh.cn

[N03] 快速排序（分治示例）
来源：http://xk.muxihuayi.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://vo.huanxung.cn

PHP:  // 递归实现，或用 usort
来源：http://qz.9csxet.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tp.shxzukj.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://al.9csxet.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ez.huanxung.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://jt.hnjuh.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://vq.9csxet.cn

C#:   // 手写递归，或 Array.Sort
来源：http://gj.szsharing.cn

[N04] 斐波那契数列
来源：http://ta.521024.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ls.colortex.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ir.huixiangedu.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ir.yuntaijiaju.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ks.shtwfgs.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://sv.yuntaijiaju.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://if.shtwfgs.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://cu.yuntaijiaju.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://zx.nszjky.cn

[N05] 最大公约数
来源：http://to.shtwfgs.cn

Py:   math.gcd(a, b)
来源：http://cm.asd995.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://lm.hnjuh.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://un.huixinmuqiang.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yg.wgjwhj.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://tr.9csxet.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://zs.huixinmuqiang.cn

Ruby: a.gcd(b)
来源：http://fp.haigaiapp.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hf.shtwfgs.cn

[N06] 判断回文字符串
来源：http://la.chemitech.net.cn

Py:   s == s[::-1]
来源：http://wt.nicolike.cn

PHP:  $s === strrev($s);
来源：http://ev.shtwfgs.cn

JS:   s === [...s].reverse().join("")
来源：http://zg.wgjwhj.cn

TS:   s === [...s].reverse().join("")
来源：http://xz.muxihuayi.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ca.newstarts.cn

Go:   // 双指针从两端比较
来源：http://ka.panjiajie.cn

Ruby: s == s.reverse
来源：http://ev.szxytkj.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://rb.newstarts.cn

[N07] 两数之和（返回下标）
来源：http://lp.bookmarksfly.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://iu.nszjky.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://bd.yuexingan06.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://co.jianghongdianzi.cn

TS:   // 手写 Map<string, number>
来源：http://kx.newstarts.cn

Java: // 手写 HashMap
来源：http://uf.yuexingan06.cn

Go:   // 手写 map[int]int
来源：http://yt.jctech888.com.cn

Ruby: // 手写 Hash
来源：http://vx.newstarts.cn

C#:   // 手写 Dictionary<int, int>
来源：http://pi.huixiangedu.cn

[N08] 生成全排列
来源：http://tp.nicolike.cn

Py:   itertools.permutations(arr)
来源：http://tu.yuexingan06.cn

PHP:  // 手写递归交换
来源：http://rc.hahajie.cn

JS:   // 手写回溯递归
来源：http://in.szsharing.cn

TS:   // 手写回溯递归
来源：http://zi.nszjky.cn

Java: // 手写回溯递归
来源：http://qa.jianghongdianzi.cn

Go:   // 手写回溯递归
来源：http://df.bookmarksfly.cn

Ruby: arr.permutation.to_a
来源：http://wq.bookmarksfly.cn

C#:   // 手写回溯递归
来源：http://cb.szsharing.cn

[N09] 栈与队列
来源：http://lx.hnjuh.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hy.shxzskj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://st.jianghongdianzi.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://lc.nszjky.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://nb.9csxet.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wz.colortex.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ym.bookmarksfly.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ms.huixiangedu.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://qt.shtwfgs.cn

[N10] 链表节点定义
来源：http://ex.asd995.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ly.colortex.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ew.asd995.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ru.jianghongdianzi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://jb.bjjhwx.cn

Java: class Node { int v; Node next; }
来源：http://rx.huixinmuqiang.cn

Go:   type Node struct { V int; Next *Node }
来源：http://bh.colortex.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://hg.asd995.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://lu.szsharing.cn

[N11] 二叉树中序遍历
来源：http://yk.huixinmuqiang.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://zv.shxzukj.cn

PHP:  // 手写递归函数
来源：http://ah.hahajie.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ad.chemitech.net.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rd.hahajie.cn

Java: // 手写递归
来源：http://by.haigaiapp.cn

Go:   // 手写递归
来源：http://rv.muxihuayi.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://sv.huixiangedu.cn

C#:   // 手写递归
来源：http://vi.jctech888.com.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://sy.chemitech.net.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://fg.wgjwhj.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ki.bjjhwx.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lr.yuntaijiaju.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://in.nicolike.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://fw.nszjky.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://yh.jctech888.com.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://fv.shtwfgs.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hu.haigaiapp.cn

================================================================================
来源：http://ep.szsharing.cn

O. 并发与异步
来源：http://hs.szsharing.cn

================================================================================
来源：http://bm.wgjwhj.cn

[O01] 启动一个线程
来源：http://ky.lnxyls.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://kc.szxytkj.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://uc.521024.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://je.shxzukj.cn

TS:   // 同 JS
来源：http://ut.szsharing.cn

Java: new Thread(() -> f()).start()
来源：http://xs.521024.cn

Go:   go f()
来源：http://xy.jianghongdianzi.cn

Ruby: Thread.new { f }
来源：http://bg.bjjhwx.cn

C#:   Task.Run(() => F());
来源：http://pu.newstarts.cn

[O02] 使用线程池
来源：http://lk.haigaiapp.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://en.yuntaijiaju.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://dl.muxihuayi.cn

JS:   // worker_threads 线程池
来源：http://xt.haigaiapp.cn

TS:   // worker_threads 线程池
来源：http://bd.huixiangedu.cn

Java: Executors.newFixedThreadPool(4)
来源：http://lt.colortex.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://pc.colortex.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://bn.chemitech.net.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://if.hahajie.cn

[O03] 加锁保护共享数据
来源：http://iv.gzmigu.cn

Py:   with lock: shared += 1
来源：http://qz.9csxet.cn

PHP:  // 用 flock() 做文件锁
来源：http://fx.yuntaijiaju.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://js.asd995.cn

TS:   // 同 JS
来源：http://vs.huanxung.cn

Java: synchronized (this) { shared++; }
来源：http://lq.nicolike.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wr.szsharing.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://uv.yuntaijiaju.cn

C#:   lock (gate) { shared++; }
来源：http://dl.bjjhwx.cn

[O04] 定义异步函数并等待
来源：http://xl.shxzskj.cn

Py:   async def f():⏎    await g()
来源：http://md.jianghongdianzi.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://kl.nicolike.cn

JS:   async function f() { await g(); }
来源：http://cb.bjjhwx.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://vq.huixiangedu.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://br.newstarts.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://sb.yuexingan06.cn

Ruby: # 用 Fiber 或 async gem
来源：http://uj.szsharing.cn

C#:   async Task F() { await G(); }
来源：http://pf.shtwfgs.cn

[O05] 并发执行并等待全部完成
来源：http://ql.9csxet.cn

Py:   asyncio.gather(*tasks)
来源：http://vh.521024.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ur.jctech888.com.cn

JS:   await Promise.all(tasks)
来源：http://kq.nicolike.cn

TS:   await Promise.all(tasks)
来源：http://if.huixinmuqiang.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ia.jianghongdianzi.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://rv.yuntaijiaju.cn

Ruby: threads.map(&:join)
来源：http://td.nszjky.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://jn.jctech888.com.cn

[O06] 使用进程池
来源：http://sr.huanxung.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://sk.shtwfgs.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://oc.shxzukj.cn

JS:   // child_process / cluster 模块
来源：http://xr.huanxung.cn

TS:   // child_process / cluster 模块
来源：http://bu.shtwfgs.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://dy.muxihuayi.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ta.yuexingan06.cn

Ruby: // fork 块
来源：http://vh.bjjhwx.cn

C#:   Parallel.For
来源：http://lh.yuexingan06.cn

================================================================================
来源：http://in.gzmigu.cn

P. 常用工具函数
来源：http://lj.shtwfgs.cn

================================================================================
来源：http://zp.hnjuh.cn


<!-- 参考信息 -->