代发 wailian999

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ey.huanxung.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ze.jctech888.com.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://cq.colortex.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wb.jctech888.com.cn

[L03] 设置自定义请求头
来源：http://no.yuexingan06.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://dv.huixiangedu.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://sn.yuexingan06.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lp.shtwfgs.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ju.huanxung.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://pu.lnxyls.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hs.shxzukj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ie.szxytkj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://pm.nszjky.cn

[L04] 设置超时
来源：http://kn.szxytkj.cn

Py:   requests.get(url, timeout=5)
来源：http://ou.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://oj.yuntaijiaju.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ew.jctech888.com.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rp.szxytkj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://fc.bjjhwx.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://eq.shxzskj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://su.newstarts.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ac.newstarts.cn

[L05] 上传文件（multipart）
来源：http://eb.chemitech.net.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://oc.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://qz.wgjwhj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://xt.asd995.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ki.colortex.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://te.shxzskj.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://gw.jianghongdianzi.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ls.szsharing.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wo.newstarts.cn

[L06] 解析响应为 JSON
来源：http://vo.haigaiapp.cn

Py:   resp.json()
来源：http://bq.panjiajie.cn

PHP:  json_decode($body, true);
来源：http://zq.szxytkj.cn

JS:   await resp.json()
来源：http://fp.asd995.cn

TS:   await resp.json()
来源：http://lc.szsharing.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://nc.yuexingan06.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://jp.bookmarksfly.cn

Ruby: JSON.parse(resp.body)
来源：http://hr.shxzukj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://sm.panjiajie.cn

[L07] 处理 HTTP 状态码
来源：http://rn.huanxung.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://tv.lnxyls.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://il.hahajie.cn

JS:   resp.ok;  resp.status
来源：http://at.panjiajie.cn

TS:   resp.ok;  resp.status
来源：http://dg.hnjuh.cn

Java: resp.statusCode()
来源：http://jj.panjiajie.cn

Go:   resp.StatusCode
来源：http://tk.jctech888.com.cn

Ruby: resp.code.to_i
来源：http://yp.521024.cn

C#:   (int)resp.StatusCode
来源：http://lj.shtwfgs.cn

[L08] 并发请求多个地址
来源：http://wj.szsharing.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://vm.bjjhwx.cn

PHP:  curl_multi_init() 系列
来源：http://sh.huixinmuqiang.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vt.hnjuh.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://db.521024.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://cx.colortex.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mn.yuntaijiaju.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://qm.colortex.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ff.nszjky.cn

================================================================================
来源：http://fl.newstarts.cn

M. 命令行 / 进程 / 环境
来源：http://fg.muxihuayi.cn

================================================================================
来源：http://tw.9csxet.cn

[M01] 读取命令行参数
来源：http://tx.muxihuayi.cn

Py:   sys.argv[1:]
来源：http://fh.nicolike.cn

PHP:  $argv;  $argc;
来源：http://xk.muxihuayi.cn

JS:   process.argv.slice(2)
来源：http://oe.shxzukj.cn

TS:   process.argv.slice(2)
来源：http://hr.muxihuayi.cn

Java: args 数组（main 方法参数）
来源：http://vz.jianghongdianzi.cn

Go:   os.Args[1:]
来源：http://hz.hnjuh.cn

Ruby: ARGV
来源：http://ay.gzmigu.cn

C#:   args 数组（Main 方法参数）
来源：http://hb.huixiangedu.cn

[M02] 读取环境变量
来源：http://kr.huixinmuqiang.cn

Py:   os.environ.get("HOME")
来源：http://yr.nicolike.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://cg.gzmigu.cn

JS:   process.env.HOME
来源：http://vu.szsharing.cn

TS:   process.env.HOME
来源：http://hc.chemitech.net.cn

Java: System.getenv("HOME")
来源：http://lt.panjiajie.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://bc.haigaiapp.cn

Ruby: ENV["HOME"]
来源：http://ck.asd995.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://by.yuntaijiaju.cn

[M03] 执行外部命令
来源：http://om.nicolike.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://le.wgjwhj.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://xo.muxihuayi.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://df.shxzukj.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://pe.bjjhwx.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://cn.newstarts.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://no.521024.cn

Ruby: system("ls -l");  `ls -l`
来源：http://og.wgjwhj.cn

C#:   Process.Start("ls", "-l");
来源：http://at.szsharing.cn

[M04] 获取当前工作目录
来源：http://zt.colortex.cn

Py:   os.getcwd()
来源：http://yz.szxytkj.cn

PHP:  getcwd();
来源：http://wx.huixinmuqiang.cn

JS:   process.cwd()
来源：http://tf.gzmigu.cn

TS:   process.cwd()
来源：http://vb.huixinmuqiang.cn

Java: Path.of("").toAbsolutePath()
来源：http://qj.lnxyls.cn

Go:   os.Getwd()
来源：http://zs.521024.cn

Ruby: Dir.pwd
来源：http://hf.nicolike.cn

C#:   Directory.GetCurrentDirectory()
来源：http://zp.lnxyls.cn

[M05] 设置退出码
来源：http://wa.521024.cn

Py:   sys.exit(1)
来源：http://md.wgjwhj.cn

PHP:  exit(1);
来源：http://hj.szsharing.cn

JS:   process.exit(1)
来源：http://fc.haigaiapp.cn

TS:   process.exit(1)
来源：http://bb.lnxyls.cn

Java: System.exit(1)
来源：http://ow.yuntaijiaju.cn

Go:   os.Exit(1)
来源：http://dy.colortex.cn

Ruby: exit 1
来源：http://fo.panjiajie.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://kx.lnxyls.cn

[M06] 向标准错误输出
来源：http://qg.yuexingan06.cn

Py:   print("err", file=sys.stderr)
来源：http://xs.hahajie.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://xs.lnxyls.cn

JS:   console.error("err")
来源：http://ac.nszjky.cn

TS:   console.error("err")
来源：http://vt.huanxung.cn

Java: System.err.println("err")
来源：http://pl.szsharing.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ci.yuexingan06.cn

Ruby: warn "err"
来源：http://vt.shxzukj.cn

C#:   Console.Error.WriteLine("err")
来源：http://bv.panjiajie.cn

[M07] 判断是否为主入口
来源：http://cb.chemitech.net.cn

Py:   if __name__ == "__main__":
来源：http://zg.nszjky.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://bp.lnxyls.cn

JS:   require.main === module
来源：http://wj.nicolike.cn

TS:   require.main === module
来源：http://ew.shxzukj.cn

Java: public static void main(String[] args)
来源：http://sc.521024.cn

Go:   func main()
来源：http://ca.asd995.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://kw.huixinmuqiang.cn

C#:   static void Main(string[] args)
来源：http://nx.9csxet.cn

[M08] 获取系统与运行时信息
来源：http://vy.nszjky.cn

Py:   platform.system();  platform.python_version()
来源：http://uh.szxytkj.cn

PHP:  PHP_OS;  phpversion();
来源：http://mv.muxihuayi.cn

JS:   process.platform;  process.version
来源：http://pa.muxihuayi.cn

TS:   process.platform;  process.version
来源：http://kk.newstarts.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://he.yuntaijiaju.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://et.yuexingan06.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://fh.hnjuh.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://sb.huixinmuqiang.cn

================================================================================
来源：http://nc.szxytkj.cn

N. 数据结构与算法
来源：http://jd.yuexingan06.cn

================================================================================
来源：http://zk.newstarts.cn

[N01] 二分查找（有序数组）
来源：http://jt.shxzskj.cn

Py:   bisect.bisect_left(arr, x)
来源：http://yr.wgjwhj.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mi.yuexingan06.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wh.haigaiapp.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tq.haigaiapp.cn

Java: Arrays.binarySearch(arr, x)
来源：http://wn.9csxet.cn

Go:   sort.SearchInts(arr, x)
来源：http://km.shtwfgs.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://iq.jianghongdianzi.cn

C#:   Array.BinarySearch(arr, x)
来源：http://am.shxzskj.cn

[N02] 排序（工程实践用内置实现）
来源：http://ey.jctech888.com.cn

Py:   sorted(arr);  arr.sort()
来源：http://iv.shtwfgs.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://zf.panjiajie.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://xk.521024.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://lb.shxzukj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://yo.bookmarksfly.cn

Go:   slices.Sort(arr)
来源：http://xh.521024.cn

Ruby: arr.sort
来源：http://rl.nszjky.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://uj.521024.cn

[N03] 快速排序（分治示例）
来源：http://ok.szsharing.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://gk.nszjky.cn

PHP:  // 递归实现，或用 usort
来源：http://ct.gzmigu.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ol.hnjuh.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cd.gzmigu.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://gf.bjjhwx.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mn.jctech888.com.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://zu.colortex.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ad.shtwfgs.cn

[N04] 斐波那契数列
来源：http://sc.szxytkj.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://cg.muxihuayi.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://bh.nicolike.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ye.muxihuayi.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qr.szxytkj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wm.hahajie.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://og.muxihuayi.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://jl.gzmigu.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://og.szxytkj.cn

[N05] 最大公约数
来源：http://uw.jianghongdianzi.cn

Py:   math.gcd(a, b)
来源：http://vw.szxytkj.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://xh.chemitech.net.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gd.haigaiapp.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ju.huixinmuqiang.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://gs.muxihuayi.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://jt.shtwfgs.cn

Ruby: a.gcd(b)
来源：http://nt.gzmigu.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://pe.nicolike.cn

[N06] 判断回文字符串
来源：http://ax.yuexingan06.cn

Py:   s == s[::-1]
来源：http://ga.chemitech.net.cn

PHP:  $s === strrev($s);
来源：http://yk.szxytkj.cn

JS:   s === [...s].reverse().join("")
来源：http://sx.bookmarksfly.cn

TS:   s === [...s].reverse().join("")
来源：http://lj.521024.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xp.bjjhwx.cn

Go:   // 双指针从两端比较
来源：http://tr.hahajie.cn

Ruby: s == s.reverse
来源：http://yf.huixinmuqiang.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://vo.huanxung.cn

[N07] 两数之和（返回下标）
来源：http://xb.bjjhwx.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://la.shxzskj.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://bw.hnjuh.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ob.hnjuh.cn

TS:   // 手写 Map<string, number>
来源：http://yu.shtwfgs.cn

Java: // 手写 HashMap
来源：http://vf.szsharing.cn

Go:   // 手写 map[int]int
来源：http://zw.shxzskj.cn

Ruby: // 手写 Hash
来源：http://zt.yuexingan06.cn

C#:   // 手写 Dictionary<int, int>
来源：http://vu.yuexingan06.cn

[N08] 生成全排列
来源：http://qb.shxzskj.cn

Py:   itertools.permutations(arr)
来源：http://qf.wgjwhj.cn

PHP:  // 手写递归交换
来源：http://jj.nszjky.cn

JS:   // 手写回溯递归
来源：http://pg.yuexingan06.cn

TS:   // 手写回溯递归
来源：http://fn.chemitech.net.cn

Java: // 手写回溯递归
来源：http://au.nicolike.cn

Go:   // 手写回溯递归
来源：http://dw.yuntaijiaju.cn

Ruby: arr.permutation.to_a
来源：http://tf.colortex.cn

C#:   // 手写回溯递归
来源：http://dg.chemitech.net.cn

[N09] 栈与队列
来源：http://yz.jianghongdianzi.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hx.yuexingan06.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://nb.bjjhwx.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://zn.newstarts.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://pe.lnxyls.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://pi.muxihuayi.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://go.lnxyls.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://fd.hnjuh.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://lq.muxihuayi.cn

[N10] 链表节点定义
来源：http://vz.szsharing.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://yy.nicolike.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://kb.yuexingan06.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qa.huanxung.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://kl.521024.cn

Java: class Node { int v; Node next; }
来源：http://ax.huanxung.cn

Go:   type Node struct { V int; Next *Node }
来源：http://oc.9csxet.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://tu.yuntaijiaju.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://qv.colortex.cn

[N11] 二叉树中序遍历
来源：http://fd.yuntaijiaju.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://sf.lnxyls.cn

PHP:  // 手写递归函数
来源：http://ll.jianghongdianzi.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sg.lnxyls.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kt.shxzukj.cn

Java: // 手写递归
来源：http://th.colortex.cn

Go:   // 手写递归
来源：http://ia.newstarts.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://rx.yuexingan06.cn

C#:   // 手写递归
来源：http://vg.521024.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://em.lnxyls.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://xf.panjiajie.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ik.hahajie.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ro.newstarts.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yh.jianghongdianzi.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://pc.jctech888.com.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://qu.szsharing.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ho.yuexingan06.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ko.newstarts.cn

================================================================================
来源：http://ki.9csxet.cn

O. 并发与异步
来源：http://oo.newstarts.cn

================================================================================
来源：http://ce.szsharing.cn

[O01] 启动一个线程
来源：http://sc.newstarts.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://sb.panjiajie.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ie.huixinmuqiang.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://nt.bookmarksfly.cn

TS:   // 同 JS
来源：http://fn.newstarts.cn

Java: new Thread(() -> f()).start()
来源：http://di.huanxung.cn

Go:   go f()
来源：http://za.shxzskj.cn

Ruby: Thread.new { f }
来源：http://sx.huixiangedu.cn

C#:   Task.Run(() => F());
来源：http://ik.hnjuh.cn

[O02] 使用线程池
来源：http://ly.jianghongdianzi.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://sy.jctech888.com.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://vx.bookmarksfly.cn

JS:   // worker_threads 线程池
来源：http://az.shxzukj.cn

TS:   // worker_threads 线程池
来源：http://xw.bookmarksfly.cn

Java: Executors.newFixedThreadPool(4)
来源：http://zd.huixiangedu.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://rm.lnxyls.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://tt.shxzskj.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://cv.shtwfgs.cn

[O03] 加锁保护共享数据
来源：http://ee.jctech888.com.cn

Py:   with lock: shared += 1
来源：http://oq.nszjky.cn

PHP:  // 用 flock() 做文件锁
来源：http://aj.hnjuh.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://kv.szxytkj.cn

TS:   // 同 JS
来源：http://zr.huixinmuqiang.cn

Java: synchronized (this) { shared++; }
来源：http://ky.haigaiapp.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://kk.szxytkj.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ke.521024.cn

C#:   lock (gate) { shared++; }
来源：http://es.bookmarksfly.cn

[O04] 定义异步函数并等待
来源：http://ta.bjjhwx.cn

Py:   async def f():⏎    await g()
来源：http://ur.panjiajie.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://im.yuexingan06.cn

JS:   async function f() { await g(); }
来源：http://jb.hnjuh.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://wn.shxzukj.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://oj.bookmarksfly.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hx.szxytkj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://uf.hahajie.cn

C#:   async Task F() { await G(); }
来源：http://eq.jctech888.com.cn

[O05] 并发执行并等待全部完成
来源：http://ie.colortex.cn

Py:   asyncio.gather(*tasks)
来源：http://vc.hahajie.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ok.szsharing.cn

JS:   await Promise.all(tasks)
来源：http://ea.panjiajie.cn

TS:   await Promise.all(tasks)
来源：http://ws.jctech888.com.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ae.nszjky.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://nz.chemitech.net.cn

Ruby: threads.map(&:join)
来源：http://ho.nszjky.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ui.nszjky.cn

[O06] 使用进程池
来源：http://jl.yuntaijiaju.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hx.bjjhwx.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://df.huixinmuqiang.cn

JS:   // child_process / cluster 模块
来源：http://le.chemitech.net.cn

TS:   // child_process / cluster 模块
来源：http://sm.szsharing.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ev.wgjwhj.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hu.huanxung.cn

Ruby: // fork 块
来源：http://jk.chemitech.net.cn


<!-- 参考信息 -->