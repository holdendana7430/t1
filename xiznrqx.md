代发 wailian999

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jv.hahajie.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://lw.colortex.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://vq.bjjhwx.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://kr.panjiajie.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://qj.huanxung.cn

[L04] 设置超时
来源：http://oz.jctech888.com.cn

Py:   requests.get(url, timeout=5)
来源：http://ac.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ul.bookmarksfly.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zo.yuexingan06.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nx.hnjuh.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://do.521024.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://rq.521024.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://in.hahajie.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://fu.muxihuayi.cn

[L05] 上传文件（multipart）
来源：http://mu.nszjky.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wt.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://nv.yuexingan06.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://oq.9csxet.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xy.huixiangedu.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ia.chemitech.net.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://xg.lnxyls.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://eb.szsharing.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ub.bjjhwx.cn

[L06] 解析响应为 JSON
来源：http://gt.shtwfgs.cn

Py:   resp.json()
来源：http://oq.huixinmuqiang.cn

PHP:  json_decode($body, true);
来源：http://fp.szsharing.cn

JS:   await resp.json()
来源：http://jt.shxzskj.cn

TS:   await resp.json()
来源：http://eh.nszjky.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://dv.9csxet.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://rs.jctech888.com.cn

Ruby: JSON.parse(resp.body)
来源：http://ij.chemitech.net.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ug.wgjwhj.cn

[L07] 处理 HTTP 状态码
来源：http://ut.colortex.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ix.lnxyls.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://jc.haigaiapp.cn

JS:   resp.ok;  resp.status
来源：http://dx.yuexingan06.cn

TS:   resp.ok;  resp.status
来源：http://au.colortex.cn

Java: resp.statusCode()
来源：http://gc.szxytkj.cn

Go:   resp.StatusCode
来源：http://cn.chemitech.net.cn

Ruby: resp.code.to_i
来源：http://zs.shtwfgs.cn

C#:   (int)resp.StatusCode
来源：http://lp.bjjhwx.cn

[L08] 并发请求多个地址
来源：http://kv.wgjwhj.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://zr.panjiajie.cn

PHP:  curl_multi_init() 系列
来源：http://hz.nicolike.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qj.shxzskj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tc.shxzskj.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://nn.chemitech.net.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://bf.yuexingan06.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://xu.colortex.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://yf.huixinmuqiang.cn

================================================================================
来源：http://cs.shxzskj.cn

M. 命令行 / 进程 / 环境
来源：http://mh.nszjky.cn

================================================================================
来源：http://px.lnxyls.cn

[M01] 读取命令行参数
来源：http://dy.shtwfgs.cn

Py:   sys.argv[1:]
来源：http://ae.muxihuayi.cn

PHP:  $argv;  $argc;
来源：http://pt.nszjky.cn

JS:   process.argv.slice(2)
来源：http://fc.yuexingan06.cn

TS:   process.argv.slice(2)
来源：http://tg.panjiajie.cn

Java: args 数组（main 方法参数）
来源：http://pd.bjjhwx.cn

Go:   os.Args[1:]
来源：http://by.521024.cn

Ruby: ARGV
来源：http://vk.521024.cn

C#:   args 数组（Main 方法参数）
来源：http://ge.shxzukj.cn

[M02] 读取环境变量
来源：http://nc.newstarts.cn

Py:   os.environ.get("HOME")
来源：http://yd.9csxet.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://va.yuntaijiaju.cn

JS:   process.env.HOME
来源：http://re.huanxung.cn

TS:   process.env.HOME
来源：http://en.lnxyls.cn

Java: System.getenv("HOME")
来源：http://xh.nszjky.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://nw.szsharing.cn

Ruby: ENV["HOME"]
来源：http://ah.yuntaijiaju.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://xt.huanxung.cn

[M03] 执行外部命令
来源：http://ka.haigaiapp.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://le.muxihuayi.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://xi.muxihuayi.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://gr.jctech888.com.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ht.yuexingan06.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://zu.shxzukj.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://tb.jctech888.com.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ur.shtwfgs.cn

C#:   Process.Start("ls", "-l");
来源：http://zl.wgjwhj.cn

[M04] 获取当前工作目录
来源：http://ql.lnxyls.cn

Py:   os.getcwd()
来源：http://ku.newstarts.cn

PHP:  getcwd();
来源：http://pm.lnxyls.cn

JS:   process.cwd()
来源：http://sg.bjjhwx.cn

TS:   process.cwd()
来源：http://ts.huanxung.cn

Java: Path.of("").toAbsolutePath()
来源：http://cc.jctech888.com.cn

Go:   os.Getwd()
来源：http://wb.9csxet.cn

Ruby: Dir.pwd
来源：http://jp.wgjwhj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://lc.huixiangedu.cn

[M05] 设置退出码
来源：http://cs.jianghongdianzi.cn

Py:   sys.exit(1)
来源：http://cw.jctech888.com.cn

PHP:  exit(1);
来源：http://au.yuntaijiaju.cn

JS:   process.exit(1)
来源：http://fi.huixinmuqiang.cn

TS:   process.exit(1)
来源：http://lq.huixiangedu.cn

Java: System.exit(1)
来源：http://sn.yuntaijiaju.cn

Go:   os.Exit(1)
来源：http://qq.lnxyls.cn

Ruby: exit 1
来源：http://so.szxytkj.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://qu.newstarts.cn

[M06] 向标准错误输出
来源：http://ff.gzmigu.cn

Py:   print("err", file=sys.stderr)
来源：http://tt.shxzukj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ce.hahajie.cn

JS:   console.error("err")
来源：http://ge.hnjuh.cn

TS:   console.error("err")
来源：http://sh.szxytkj.cn

Java: System.err.println("err")
来源：http://gu.szxytkj.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://gd.muxihuayi.cn

Ruby: warn "err"
来源：http://si.asd995.cn

C#:   Console.Error.WriteLine("err")
来源：http://mi.shtwfgs.cn

[M07] 判断是否为主入口
来源：http://kw.szsharing.cn

Py:   if __name__ == "__main__":
来源：http://pl.shxzukj.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://lh.jianghongdianzi.cn

JS:   require.main === module
来源：http://ul.shtwfgs.cn

TS:   require.main === module
来源：http://qq.szsharing.cn

Java: public static void main(String[] args)
来源：http://ox.colortex.cn

Go:   func main()
来源：http://yc.shxzukj.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://pc.hahajie.cn

C#:   static void Main(string[] args)
来源：http://zb.jianghongdianzi.cn

[M08] 获取系统与运行时信息
来源：http://eb.hahajie.cn

Py:   platform.system();  platform.python_version()
来源：http://ay.yuexingan06.cn

PHP:  PHP_OS;  phpversion();
来源：http://nb.colortex.cn

JS:   process.platform;  process.version
来源：http://zd.jctech888.com.cn

TS:   process.platform;  process.version
来源：http://qx.gzmigu.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ex.shxzskj.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://bu.bjjhwx.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://aq.huanxung.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://dd.shxzskj.cn

================================================================================
来源：http://kn.shtwfgs.cn

N. 数据结构与算法
来源：http://ds.nicolike.cn

================================================================================
来源：http://ya.9csxet.cn

[N01] 二分查找（有序数组）
来源：http://ul.shxzskj.cn

Py:   bisect.bisect_left(arr, x)
来源：http://de.huixiangedu.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://tc.nicolike.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://st.muxihuayi.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sl.yuexingan06.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ug.huixinmuqiang.cn

Go:   sort.SearchInts(arr, x)
来源：http://nx.shtwfgs.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://hx.muxihuayi.cn

C#:   Array.BinarySearch(arr, x)
来源：http://mo.yuexingan06.cn

[N02] 排序（工程实践用内置实现）
来源：http://fj.haigaiapp.cn

Py:   sorted(arr);  arr.sort()
来源：http://gx.wgjwhj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://bo.bookmarksfly.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://co.521024.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://jj.huanxung.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://bv.yuexingan06.cn

Go:   slices.Sort(arr)
来源：http://uk.muxihuayi.cn

Ruby: arr.sort
来源：http://ys.huixinmuqiang.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://vb.newstarts.cn

[N03] 快速排序（分治示例）
来源：http://qk.jianghongdianzi.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://xt.hahajie.cn

PHP:  // 递归实现，或用 usort
来源：http://ou.wgjwhj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zy.jctech888.com.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://op.hnjuh.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://qz.lnxyls.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ic.szxytkj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ku.shxzskj.cn

C#:   // 手写递归，或 Array.Sort
来源：http://xn.chemitech.net.cn

[N04] 斐波那契数列
来源：http://sr.shtwfgs.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://gx.yuexingan06.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://xp.gzmigu.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ok.jctech888.com.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ig.huixiangedu.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mo.asd995.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ts.szxytkj.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ai.szsharing.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://gv.shxzukj.cn

[N05] 最大公约数
来源：http://cm.shxzskj.cn

Py:   math.gcd(a, b)
来源：http://gx.hnjuh.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mc.521024.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cy.lnxyls.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mw.hahajie.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://us.szxytkj.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://kj.panjiajie.cn

Ruby: a.gcd(b)
来源：http://gg.hahajie.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://pl.szsharing.cn

[N06] 判断回文字符串
来源：http://jg.haigaiapp.cn

Py:   s == s[::-1]
来源：http://qk.lnxyls.cn

PHP:  $s === strrev($s);
来源：http://rt.newstarts.cn

JS:   s === [...s].reverse().join("")
来源：http://ya.hnjuh.cn

TS:   s === [...s].reverse().join("")
来源：http://xw.asd995.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mz.yuntaijiaju.cn

Go:   // 双指针从两端比较
来源：http://fo.9csxet.cn

Ruby: s == s.reverse
来源：http://zc.nicolike.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ak.shxzskj.cn

[N07] 两数之和（返回下标）
来源：http://jj.shtwfgs.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://qi.szxytkj.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://nk.yuexingan06.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://zz.huanxung.cn

TS:   // 手写 Map<string, number>
来源：http://pc.shxzukj.cn

Java: // 手写 HashMap
来源：http://hm.yuexingan06.cn

Go:   // 手写 map[int]int
来源：http://cw.haigaiapp.cn

Ruby: // 手写 Hash
来源：http://qz.521024.cn

C#:   // 手写 Dictionary<int, int>
来源：http://yz.jctech888.com.cn

[N08] 生成全排列
来源：http://vr.jianghongdianzi.cn

Py:   itertools.permutations(arr)
来源：http://vg.colortex.cn

PHP:  // 手写递归交换
来源：http://gy.gzmigu.cn

JS:   // 手写回溯递归
来源：http://ml.nicolike.cn

TS:   // 手写回溯递归
来源：http://bp.shxzskj.cn

Java: // 手写回溯递归
来源：http://wr.yuntaijiaju.cn

Go:   // 手写回溯递归
来源：http://co.panjiajie.cn

Ruby: arr.permutation.to_a
来源：http://qs.jctech888.com.cn

C#:   // 手写回溯递归
来源：http://om.nszjky.cn

[N09] 栈与队列
来源：http://is.521024.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://zr.yuntaijiaju.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mv.jctech888.com.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wd.bookmarksfly.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://io.bookmarksfly.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://im.chemitech.net.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://bq.shxzukj.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mm.nicolike.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wf.huanxung.cn

[N10] 链表节点定义
来源：http://sl.newstarts.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://gc.huixiangedu.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://to.newstarts.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://vl.asd995.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://gm.shtwfgs.cn

Java: class Node { int v; Node next; }
来源：http://yc.shxzskj.cn

Go:   type Node struct { V int; Next *Node }
来源：http://wj.jctech888.com.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://mk.asd995.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ex.yuntaijiaju.cn

[N11] 二叉树中序遍历
来源：http://qy.nicolike.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hm.shtwfgs.cn

PHP:  // 手写递归函数
来源：http://dh.nicolike.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bs.shtwfgs.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kh.9csxet.cn

Java: // 手写递归
来源：http://tm.panjiajie.cn

Go:   // 手写递归
来源：http://wm.yuntaijiaju.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ns.shxzukj.cn

C#:   // 手写递归
来源：http://ff.lnxyls.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://eq.gzmigu.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://pt.lnxyls.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ao.huixinmuqiang.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sq.yuntaijiaju.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xk.shxzskj.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://kl.shtwfgs.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://tl.huanxung.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://lo.szxytkj.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://yq.jianghongdianzi.cn

================================================================================
来源：http://uw.newstarts.cn

O. 并发与异步
来源：http://uh.huanxung.cn

================================================================================
来源：http://de.nicolike.cn

[O01] 启动一个线程
来源：http://iu.9csxet.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://jx.bjjhwx.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://lm.shxzukj.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hb.hahajie.cn

TS:   // 同 JS
来源：http://lk.muxihuayi.cn

Java: new Thread(() -> f()).start()
来源：http://br.lnxyls.cn

Go:   go f()
来源：http://my.huixinmuqiang.cn

Ruby: Thread.new { f }
来源：http://oq.huixiangedu.cn

C#:   Task.Run(() => F());
来源：http://cv.szsharing.cn

[O02] 使用线程池
来源：http://fe.bookmarksfly.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://va.szsharing.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mn.szxytkj.cn

JS:   // worker_threads 线程池
来源：http://qt.bjjhwx.cn

TS:   // worker_threads 线程池
来源：http://oi.jctech888.com.cn

Java: Executors.newFixedThreadPool(4)
来源：http://su.shxzukj.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://qm.shxzskj.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://je.haigaiapp.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ji.asd995.cn

[O03] 加锁保护共享数据
来源：http://sm.newstarts.cn

Py:   with lock: shared += 1
来源：http://gz.nszjky.cn

PHP:  // 用 flock() 做文件锁
来源：http://hi.asd995.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://lz.shtwfgs.cn

TS:   // 同 JS
来源：http://yl.521024.cn

Java: synchronized (this) { shared++; }
来源：http://rn.colortex.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://if.huanxung.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ge.521024.cn

C#:   lock (gate) { shared++; }
来源：http://la.jctech888.com.cn

[O04] 定义异步函数并等待
来源：http://ke.gzmigu.cn

Py:   async def f():⏎    await g()
来源：http://jh.chemitech.net.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://sf.szxytkj.cn

JS:   async function f() { await g(); }
来源：http://ak.huanxung.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://fw.nszjky.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://sl.yuntaijiaju.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://vg.hahajie.cn

Ruby: # 用 Fiber 或 async gem
来源：http://tv.521024.cn

C#:   async Task F() { await G(); }
来源：http://yx.hahajie.cn

[O05] 并发执行并等待全部完成
来源：http://oi.shxzskj.cn

Py:   asyncio.gather(*tasks)
来源：http://kb.gzmigu.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://pp.shxzukj.cn

JS:   await Promise.all(tasks)
来源：http://rl.bjjhwx.cn

TS:   await Promise.all(tasks)
来源：http://jf.haigaiapp.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://xa.bookmarksfly.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hc.szsharing.cn

Ruby: threads.map(&:join)
来源：http://zd.asd995.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ck.bjjhwx.cn

[O06] 使用进程池
来源：http://dd.muxihuayi.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ym.hahajie.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ds.yuexingan06.cn

JS:   // child_process / cluster 模块
来源：http://zn.shtwfgs.cn

TS:   // child_process / cluster 模块
来源：http://dj.colortex.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://sj.nicolike.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ot.shtwfgs.cn

Ruby: // fork 块
来源：http://uz.chemitech.net.cn

C#:   Parallel.For
来源：http://ys.jctech888.com.cn

================================================================================
来源：http://dw.panjiajie.cn

P. 常用工具函数
来源：http://hl.shxzskj.cn

================================================================================
来源：http://ci.newstarts.cn

[P01] 生成 UUID
来源：http://jc.jctech888.com.cn

Py:   str(uuid.uuid4())
来源：http://mg.asd995.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://po.szsharing.cn

JS:   crypto.randomUUID()
来源：http://hg.nszjky.cn


<!-- 参考信息 -->