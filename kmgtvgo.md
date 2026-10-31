代发 wailian999

Go:   resp, err := http.Get(url)
来源：http://gh.bookmarksfly.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ab.hnjuh.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://xx.nszjky.cn

[L02] 发送 POST JSON
来源：http://ir.huixiangedu.cn

Py:   requests.post(url, json={"a": 1})
来源：http://rs.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://nt.gzmigu.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qg.gzmigu.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mp.hnjuh.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://yq.hnjuh.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://gv.huixinmuqiang.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ak.lnxyls.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hk.newstarts.cn

[L03] 设置自定义请求头
来源：http://hy.hnjuh.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://kv.panjiajie.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://kd.colortex.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ep.yuexingan06.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qc.bookmarksfly.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://id.jctech888.com.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://pb.bookmarksfly.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ac.hahajie.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://zo.yuntaijiaju.cn

[L04] 设置超时
来源：http://ce.szxytkj.cn

Py:   requests.get(url, timeout=5)
来源：http://zp.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://so.huanxung.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ti.newstarts.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pe.jianghongdianzi.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://zn.huanxung.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://gf.521024.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://dz.szxytkj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://yl.haigaiapp.cn

[L05] 上传文件（multipart）
来源：http://qz.nszjky.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://yo.nicolike.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://na.asd995.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://dx.jianghongdianzi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://jr.newstarts.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://nb.nicolike.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://jy.szsharing.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://sa.hahajie.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://md.wgjwhj.cn

[L06] 解析响应为 JSON
来源：http://nc.nicolike.cn

Py:   resp.json()
来源：http://xi.jianghongdianzi.cn

PHP:  json_decode($body, true);
来源：http://gl.shxzukj.cn

JS:   await resp.json()
来源：http://po.yuexingan06.cn

TS:   await resp.json()
来源：http://is.shxzukj.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://vk.haigaiapp.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mn.colortex.cn

Ruby: JSON.parse(resp.body)
来源：http://qb.hahajie.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://aw.gzmigu.cn

[L07] 处理 HTTP 状态码
来源：http://th.hnjuh.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://rn.nicolike.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://bi.huixiangedu.cn

JS:   resp.ok;  resp.status
来源：http://zi.colortex.cn

TS:   resp.ok;  resp.status
来源：http://zy.shxzskj.cn

Java: resp.statusCode()
来源：http://an.szxytkj.cn

Go:   resp.StatusCode
来源：http://ph.nicolike.cn

Ruby: resp.code.to_i
来源：http://xz.muxihuayi.cn

C#:   (int)resp.StatusCode
来源：http://ok.asd995.cn

[L08] 并发请求多个地址
来源：http://xu.9csxet.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://on.bjjhwx.cn

PHP:  curl_multi_init() 系列
来源：http://ub.bookmarksfly.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vi.colortex.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rn.szsharing.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://td.panjiajie.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ff.wgjwhj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://du.wgjwhj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://qu.yuexingan06.cn

================================================================================
来源：http://gq.panjiajie.cn

M. 命令行 / 进程 / 环境
来源：http://fr.bjjhwx.cn

================================================================================
来源：http://ba.bjjhwx.cn

[M01] 读取命令行参数
来源：http://ez.colortex.cn

Py:   sys.argv[1:]
来源：http://rn.bjjhwx.cn

PHP:  $argv;  $argc;
来源：http://pz.hahajie.cn

JS:   process.argv.slice(2)
来源：http://ri.bookmarksfly.cn

TS:   process.argv.slice(2)
来源：http://la.panjiajie.cn

Java: args 数组（main 方法参数）
来源：http://kh.bjjhwx.cn

Go:   os.Args[1:]
来源：http://wv.huixiangedu.cn

Ruby: ARGV
来源：http://nz.hnjuh.cn

C#:   args 数组（Main 方法参数）
来源：http://ob.yuexingan06.cn

[M02] 读取环境变量
来源：http://xz.lnxyls.cn

Py:   os.environ.get("HOME")
来源：http://ez.bjjhwx.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://gx.bjjhwx.cn

JS:   process.env.HOME
来源：http://sm.nicolike.cn

TS:   process.env.HOME
来源：http://wm.chemitech.net.cn

Java: System.getenv("HOME")
来源：http://bk.jctech888.com.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://qa.9csxet.cn

Ruby: ENV["HOME"]
来源：http://uz.huanxung.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://oa.521024.cn

[M03] 执行外部命令
来源：http://wm.hnjuh.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://aj.bookmarksfly.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://iv.yuexingan06.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://rm.jianghongdianzi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://xe.panjiajie.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.shxzskj.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://lo.haigaiapp.cn

Ruby: system("ls -l");  `ls -l`
来源：http://lk.colortex.cn

C#:   Process.Start("ls", "-l");
来源：http://uq.haigaiapp.cn

[M04] 获取当前工作目录
来源：http://qa.gzmigu.cn

Py:   os.getcwd()
来源：http://fb.hahajie.cn

PHP:  getcwd();
来源：http://pz.lnxyls.cn

JS:   process.cwd()
来源：http://se.hnjuh.cn

TS:   process.cwd()
来源：http://tr.huanxung.cn

Java: Path.of("").toAbsolutePath()
来源：http://ue.huixinmuqiang.cn

Go:   os.Getwd()
来源：http://ip.colortex.cn

Ruby: Dir.pwd
来源：http://fq.shxzukj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://eq.521024.cn

[M05] 设置退出码
来源：http://pb.colortex.cn

Py:   sys.exit(1)
来源：http://wk.szxytkj.cn

PHP:  exit(1);
来源：http://sf.9csxet.cn

JS:   process.exit(1)
来源：http://tv.hahajie.cn

TS:   process.exit(1)
来源：http://xw.nicolike.cn

Java: System.exit(1)
来源：http://qd.lnxyls.cn

Go:   os.Exit(1)
来源：http://zi.shxzskj.cn

Ruby: exit 1
来源：http://ko.muxihuayi.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://md.shtwfgs.cn

[M06] 向标准错误输出
来源：http://hw.yuexingan06.cn

Py:   print("err", file=sys.stderr)
来源：http://tu.nicolike.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://qz.bjjhwx.cn

JS:   console.error("err")
来源：http://cs.huixinmuqiang.cn

TS:   console.error("err")
来源：http://tn.asd995.cn

Java: System.err.println("err")
来源：http://xh.haigaiapp.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://sm.huixiangedu.cn

Ruby: warn "err"
来源：http://rd.gzmigu.cn

C#:   Console.Error.WriteLine("err")
来源：http://nt.bjjhwx.cn

[M07] 判断是否为主入口
来源：http://zz.nszjky.cn

Py:   if __name__ == "__main__":
来源：http://jw.newstarts.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hd.jianghongdianzi.cn

JS:   require.main === module
来源：http://pw.lnxyls.cn

TS:   require.main === module
来源：http://jy.shxzskj.cn

Java: public static void main(String[] args)
来源：http://fi.asd995.cn

Go:   func main()
来源：http://an.gzmigu.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://xg.huixiangedu.cn

C#:   static void Main(string[] args)
来源：http://nj.szxytkj.cn

[M08] 获取系统与运行时信息
来源：http://dd.szsharing.cn

Py:   platform.system();  platform.python_version()
来源：http://bg.yuexingan06.cn

PHP:  PHP_OS;  phpversion();
来源：http://zr.muxihuayi.cn

JS:   process.platform;  process.version
来源：http://jt.lnxyls.cn

TS:   process.platform;  process.version
来源：http://sj.huixinmuqiang.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mb.bookmarksfly.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ms.huanxung.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ma.lnxyls.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://wx.shxzukj.cn

================================================================================
来源：http://tc.shtwfgs.cn

N. 数据结构与算法
来源：http://tr.chemitech.net.cn

================================================================================
来源：http://xw.bjjhwx.cn

[N01] 二分查找（有序数组）
来源：http://vt.szxytkj.cn

Py:   bisect.bisect_left(arr, x)
来源：http://bu.yuntaijiaju.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://af.9csxet.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wm.nszjky.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ey.panjiajie.cn

Java: Arrays.binarySearch(arr, x)
来源：http://kx.panjiajie.cn

Go:   sort.SearchInts(arr, x)
来源：http://io.bjjhwx.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://yz.muxihuayi.cn

C#:   Array.BinarySearch(arr, x)
来源：http://vh.asd995.cn

[N02] 排序（工程实践用内置实现）
来源：http://ck.bjjhwx.cn

Py:   sorted(arr);  arr.sort()
来源：http://pe.yuntaijiaju.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ja.huixiangedu.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://tt.bjjhwx.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://hi.huixiangedu.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://tp.shxzskj.cn

Go:   slices.Sort(arr)
来源：http://vt.lnxyls.cn

Ruby: arr.sort
来源：http://vy.jianghongdianzi.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://vq.chemitech.net.cn

[N03] 快速排序（分治示例）
来源：http://dc.newstarts.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://dm.hahajie.cn

PHP:  // 递归实现，或用 usort
来源：http://es.szsharing.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dd.panjiajie.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zq.shxzskj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mv.hnjuh.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://sy.muxihuayi.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xa.gzmigu.cn

C#:   // 手写递归，或 Array.Sort
来源：http://rn.hnjuh.cn

[N04] 斐波那契数列
来源：http://oc.yuexingan06.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://vk.hnjuh.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://kj.jianghongdianzi.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ko.nszjky.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xm.panjiajie.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://gf.yuexingan06.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://bh.hnjuh.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://dn.newstarts.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wv.bookmarksfly.cn

[N05] 最大公约数
来源：http://oq.shxzukj.cn

Py:   math.gcd(a, b)
来源：http://fr.jianghongdianzi.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://yr.yuntaijiaju.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vh.colortex.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ai.hahajie.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://bd.szxytkj.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://tw.bjjhwx.cn

Ruby: a.gcd(b)
来源：http://qi.bookmarksfly.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://up.bookmarksfly.cn

[N06] 判断回文字符串
来源：http://vw.yuntaijiaju.cn

Py:   s == s[::-1]
来源：http://xi.nicolike.cn

PHP:  $s === strrev($s);
来源：http://ar.521024.cn

JS:   s === [...s].reverse().join("")
来源：http://ru.nicolike.cn

TS:   s === [...s].reverse().join("")
来源：http://os.chemitech.net.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://lk.muxihuayi.cn

Go:   // 双指针从两端比较
来源：http://zp.bjjhwx.cn

Ruby: s == s.reverse
来源：http://uh.panjiajie.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ic.chemitech.net.cn

[N07] 两数之和（返回下标）
来源：http://tq.yuexingan06.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://pp.nicolike.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://gi.9csxet.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://zw.wgjwhj.cn

TS:   // 手写 Map<string, number>
来源：http://ue.muxihuayi.cn

Java: // 手写 HashMap
来源：http://ly.hahajie.cn

Go:   // 手写 map[int]int
来源：http://qf.szxytkj.cn

Ruby: // 手写 Hash
来源：http://wi.huixinmuqiang.cn

C#:   // 手写 Dictionary<int, int>
来源：http://qe.lnxyls.cn

[N08] 生成全排列
来源：http://wf.chemitech.net.cn

Py:   itertools.permutations(arr)
来源：http://dg.jianghongdianzi.cn

PHP:  // 手写递归交换
来源：http://fe.yuexingan06.cn

JS:   // 手写回溯递归
来源：http://cm.hahajie.cn

TS:   // 手写回溯递归
来源：http://bl.asd995.cn

Java: // 手写回溯递归
来源：http://ne.gzmigu.cn

Go:   // 手写回溯递归
来源：http://fu.huixinmuqiang.cn

Ruby: arr.permutation.to_a
来源：http://nd.asd995.cn

C#:   // 手写回溯递归
来源：http://ly.bjjhwx.cn

[N09] 栈与队列
来源：http://sd.huixiangedu.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://tt.shxzukj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://zb.huanxung.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://eq.wgjwhj.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://zs.shxzskj.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://bg.521024.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://tv.nszjky.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://sp.huixinmuqiang.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ri.asd995.cn

[N10] 链表节点定义
来源：http://cg.hahajie.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://bb.shxzskj.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://bl.muxihuayi.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://kg.shxzukj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://fr.wgjwhj.cn

Java: class Node { int v; Node next; }
来源：http://mr.yuntaijiaju.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ex.shtwfgs.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://rg.521024.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://sq.yuntaijiaju.cn

[N11] 二叉树中序遍历
来源：http://zc.521024.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://zi.jianghongdianzi.cn

PHP:  // 手写递归函数
来源：http://ty.szsharing.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ml.asd995.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://iu.9csxet.cn

Java: // 手写递归
来源：http://rh.nicolike.cn

Go:   // 手写递归
来源：http://ii.hnjuh.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://bt.huixinmuqiang.cn

C#:   // 手写递归
来源：http://st.gzmigu.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ge.wgjwhj.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://fj.bjjhwx.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://oj.yuntaijiaju.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://df.bookmarksfly.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sv.nszjky.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://iw.yuexingan06.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://rw.nicolike.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://oj.lnxyls.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://xm.nszjky.cn

================================================================================
来源：http://td.shxzskj.cn

O. 并发与异步
来源：http://tl.9csxet.cn

================================================================================
来源：http://bj.bjjhwx.cn

[O01] 启动一个线程
来源：http://mo.bookmarksfly.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://dd.haigaiapp.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://gq.haigaiapp.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wy.nszjky.cn

TS:   // 同 JS
来源：http://rh.shxzukj.cn

Java: new Thread(() -> f()).start()
来源：http://aj.shxzskj.cn

Go:   go f()
来源：http://lu.chemitech.net.cn

Ruby: Thread.new { f }
来源：http://ob.yuntaijiaju.cn

C#:   Task.Run(() => F());
来源：http://fu.hnjuh.cn

[O02] 使用线程池
来源：http://ng.huixinmuqiang.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://sx.gzmigu.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ay.asd995.cn

JS:   // worker_threads 线程池
来源：http://lj.muxihuayi.cn

TS:   // worker_threads 线程池
来源：http://qu.huixiangedu.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ke.lnxyls.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ju.huixinmuqiang.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://kr.521024.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://nx.chemitech.net.cn

[O03] 加锁保护共享数据
来源：http://ez.hahajie.cn

Py:   with lock: shared += 1
来源：http://ca.huixinmuqiang.cn

PHP:  // 用 flock() 做文件锁
来源：http://ni.chemitech.net.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://kq.bookmarksfly.cn

TS:   // 同 JS
来源：http://xi.panjiajie.cn

Java: synchronized (this) { shared++; }
来源：http://oh.szsharing.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ek.panjiajie.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://nl.haigaiapp.cn

C#:   lock (gate) { shared++; }
来源：http://sp.lnxyls.cn

[O04] 定义异步函数并等待
来源：http://su.chemitech.net.cn

Py:   async def f():⏎    await g()
来源：http://rz.lnxyls.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://bg.shtwfgs.cn

JS:   async function f() { await g(); }
来源：http://yr.newstarts.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://xm.shtwfgs.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://yu.huanxung.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://vz.shxzskj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://kp.haigaiapp.cn

C#:   async Task F() { await G(); }
来源：http://li.colortex.cn

[O05] 并发执行并等待全部完成
来源：http://pn.haigaiapp.cn

Py:   asyncio.gather(*tasks)
来源：http://df.shtwfgs.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://dy.colortex.cn

JS:   await Promise.all(tasks)
来源：http://cg.bookmarksfly.cn

TS:   await Promise.all(tasks)
来源：http://ca.shtwfgs.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mw.nicolike.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ts.jianghongdianzi.cn

Ruby: threads.map(&:join)
来源：http://ak.huixinmuqiang.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://hw.huixinmuqiang.cn


<!-- 参考信息 -->