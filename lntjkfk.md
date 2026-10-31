代发 wailian999

Py:   requests.post(url, json={"a": 1})
来源：http://ti.yuntaijiaju.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ap.9csxet.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xp.szxytkj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lc.newstarts.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://av.nszjky.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ef.haigaiapp.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://us.asd995.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ap.yuexingan06.cn

[L03] 设置自定义请求头
来源：http://rk.nszjky.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://aj.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ee.521024.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sp.bookmarksfly.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wo.hnjuh.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://lo.haigaiapp.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ki.szxytkj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://tn.bookmarksfly.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://qc.9csxet.cn

[L04] 设置超时
来源：http://ss.shtwfgs.cn

Py:   requests.get(url, timeout=5)
来源：http://vc.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ac.nszjky.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jf.nicolike.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mz.9csxet.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://sa.nszjky.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://zx.huixinmuqiang.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://fn.jctech888.com.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ih.shtwfgs.cn

[L05] 上传文件（multipart）
来源：http://hg.nszjky.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://jo.szsharing.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://oh.9csxet.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ml.colortex.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ct.hahajie.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://sr.gzmigu.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://gh.bjjhwx.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://dv.9csxet.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ly.shxzukj.cn

[L06] 解析响应为 JSON
来源：http://zc.szxytkj.cn

Py:   resp.json()
来源：http://bg.haigaiapp.cn

PHP:  json_decode($body, true);
来源：http://ed.nszjky.cn

JS:   await resp.json()
来源：http://ie.nszjky.cn

TS:   await resp.json()
来源：http://bv.shxzukj.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://an.huixinmuqiang.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://rw.nicolike.cn

Ruby: JSON.parse(resp.body)
来源：http://ss.hahajie.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://jb.yuntaijiaju.cn

[L07] 处理 HTTP 状态码
来源：http://is.huanxung.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://jg.jianghongdianzi.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://sx.jctech888.com.cn

JS:   resp.ok;  resp.status
来源：http://fg.shxzukj.cn

TS:   resp.ok;  resp.status
来源：http://ap.shxzskj.cn

Java: resp.statusCode()
来源：http://mv.huixinmuqiang.cn

Go:   resp.StatusCode
来源：http://uw.shtwfgs.cn

Ruby: resp.code.to_i
来源：http://ag.yuntaijiaju.cn

C#:   (int)resp.StatusCode
来源：http://ln.hahajie.cn

[L08] 并发请求多个地址
来源：http://dy.newstarts.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://se.hnjuh.cn

PHP:  curl_multi_init() 系列
来源：http://gp.lnxyls.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qt.lnxyls.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xz.nicolike.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://pd.nicolike.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qi.jianghongdianzi.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://gp.huixiangedu.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://lt.shxzukj.cn

================================================================================
来源：http://wn.huixiangedu.cn

M. 命令行 / 进程 / 环境
来源：http://si.nszjky.cn

================================================================================
来源：http://wh.shtwfgs.cn

[M01] 读取命令行参数
来源：http://re.shxzskj.cn

Py:   sys.argv[1:]
来源：http://yq.huixiangedu.cn

PHP:  $argv;  $argc;
来源：http://sy.newstarts.cn

JS:   process.argv.slice(2)
来源：http://qp.szsharing.cn

TS:   process.argv.slice(2)
来源：http://fk.jctech888.com.cn

Java: args 数组（main 方法参数）
来源：http://ff.szxytkj.cn

Go:   os.Args[1:]
来源：http://xz.bookmarksfly.cn

Ruby: ARGV
来源：http://pl.newstarts.cn

C#:   args 数组（Main 方法参数）
来源：http://nd.hahajie.cn

[M02] 读取环境变量
来源：http://zz.yuntaijiaju.cn

Py:   os.environ.get("HOME")
来源：http://qs.yuntaijiaju.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://bw.nszjky.cn

JS:   process.env.HOME
来源：http://xa.huixinmuqiang.cn

TS:   process.env.HOME
来源：http://wu.haigaiapp.cn

Java: System.getenv("HOME")
来源：http://ez.lnxyls.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://nz.yuntaijiaju.cn

Ruby: ENV["HOME"]
来源：http://ff.haigaiapp.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://tb.colortex.cn

[M03] 执行外部命令
来源：http://uc.9csxet.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://nv.szxytkj.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://pv.bookmarksfly.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://mk.hnjuh.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://yd.huanxung.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://az.gzmigu.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://tm.yuntaijiaju.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ts.newstarts.cn

C#:   Process.Start("ls", "-l");
来源：http://ny.bookmarksfly.cn

[M04] 获取当前工作目录
来源：http://ge.chemitech.net.cn

Py:   os.getcwd()
来源：http://ek.yuexingan06.cn

PHP:  getcwd();
来源：http://qx.shxzskj.cn

JS:   process.cwd()
来源：http://iz.haigaiapp.cn

TS:   process.cwd()
来源：http://wj.hnjuh.cn

Java: Path.of("").toAbsolutePath()
来源：http://wf.nszjky.cn

Go:   os.Getwd()
来源：http://qs.bookmarksfly.cn

Ruby: Dir.pwd
来源：http://lf.shxzskj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://gk.shxzukj.cn

[M05] 设置退出码
来源：http://st.szsharing.cn

Py:   sys.exit(1)
来源：http://cp.huixinmuqiang.cn

PHP:  exit(1);
来源：http://lw.shxzukj.cn

JS:   process.exit(1)
来源：http://aa.huixiangedu.cn

TS:   process.exit(1)
来源：http://tj.shxzukj.cn

Java: System.exit(1)
来源：http://pu.bjjhwx.cn

Go:   os.Exit(1)
来源：http://pw.shtwfgs.cn

Ruby: exit 1
来源：http://gq.colortex.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hn.hahajie.cn

[M06] 向标准错误输出
来源：http://rc.wgjwhj.cn

Py:   print("err", file=sys.stderr)
来源：http://zn.bjjhwx.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://gz.yuexingan06.cn

JS:   console.error("err")
来源：http://bg.yuexingan06.cn

TS:   console.error("err")
来源：http://vu.9csxet.cn

Java: System.err.println("err")
来源：http://ax.huixinmuqiang.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wj.9csxet.cn

Ruby: warn "err"
来源：http://bg.huixiangedu.cn

C#:   Console.Error.WriteLine("err")
来源：http://bf.wgjwhj.cn

[M07] 判断是否为主入口
来源：http://gq.panjiajie.cn

Py:   if __name__ == "__main__":
来源：http://fs.newstarts.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://nx.shxzskj.cn

JS:   require.main === module
来源：http://zn.yuexingan06.cn

TS:   require.main === module
来源：http://zs.jianghongdianzi.cn

Java: public static void main(String[] args)
来源：http://gm.yuexingan06.cn

Go:   func main()
来源：http://bw.9csxet.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://zb.hahajie.cn

C#:   static void Main(string[] args)
来源：http://di.szxytkj.cn

[M08] 获取系统与运行时信息
来源：http://ly.yuexingan06.cn

Py:   platform.system();  platform.python_version()
来源：http://qe.9csxet.cn

PHP:  PHP_OS;  phpversion();
来源：http://ks.nszjky.cn

JS:   process.platform;  process.version
来源：http://uy.521024.cn

TS:   process.platform;  process.version
来源：http://sg.9csxet.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mz.chemitech.net.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://lb.jctech888.com.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://kh.521024.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ne.nicolike.cn

================================================================================
来源：http://dc.lnxyls.cn

N. 数据结构与算法
来源：http://ov.colortex.cn

================================================================================
来源：http://my.panjiajie.cn

[N01] 二分查找（有序数组）
来源：http://sd.nszjky.cn

Py:   bisect.bisect_left(arr, x)
来源：http://pl.wgjwhj.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://je.nszjky.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rw.bjjhwx.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cs.colortex.cn

Java: Arrays.binarySearch(arr, x)
来源：http://zv.nszjky.cn

Go:   sort.SearchInts(arr, x)
来源：http://hr.yuntaijiaju.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://zb.bookmarksfly.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ql.haigaiapp.cn

[N02] 排序（工程实践用内置实现）
来源：http://gk.shtwfgs.cn

Py:   sorted(arr);  arr.sort()
来源：http://uf.shtwfgs.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://aw.521024.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://kv.huanxung.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ef.huixinmuqiang.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://kj.bookmarksfly.cn

Go:   slices.Sort(arr)
来源：http://qi.nszjky.cn

Ruby: arr.sort
来源：http://et.huixinmuqiang.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://zs.bookmarksfly.cn

[N03] 快速排序（分治示例）
来源：http://ac.jianghongdianzi.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://tb.wgjwhj.cn

PHP:  // 递归实现，或用 usort
来源：http://iv.panjiajie.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tq.hahajie.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rm.lnxyls.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hh.szsharing.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mp.jctech888.com.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://dd.szsharing.cn

C#:   // 手写递归，或 Array.Sort
来源：http://fp.wgjwhj.cn

[N04] 斐波那契数列
来源：http://li.521024.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://xn.colortex.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://nr.gzmigu.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://al.hahajie.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qt.nszjky.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wf.jianghongdianzi.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ad.bjjhwx.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://pu.gzmigu.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://gc.hnjuh.cn

[N05] 最大公约数
来源：http://wf.bjjhwx.cn

Py:   math.gcd(a, b)
来源：http://gl.newstarts.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ob.muxihuayi.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://op.hahajie.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xf.haigaiapp.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://fp.nszjky.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://xg.muxihuayi.cn

Ruby: a.gcd(b)
来源：http://xe.huixinmuqiang.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wf.szxytkj.cn

[N06] 判断回文字符串
来源：http://tc.yuexingan06.cn

Py:   s == s[::-1]
来源：http://bv.hahajie.cn

PHP:  $s === strrev($s);
来源：http://gb.huixiangedu.cn

JS:   s === [...s].reverse().join("")
来源：http://dt.hnjuh.cn

TS:   s === [...s].reverse().join("")
来源：http://zr.panjiajie.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://be.nszjky.cn

Go:   // 双指针从两端比较
来源：http://ze.shtwfgs.cn

Ruby: s == s.reverse
来源：http://xd.asd995.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://xe.yuexingan06.cn

[N07] 两数之和（返回下标）
来源：http://ln.yuntaijiaju.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://vl.newstarts.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hf.chemitech.net.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://fs.yuntaijiaju.cn

TS:   // 手写 Map<string, number>
来源：http://wb.huanxung.cn

Java: // 手写 HashMap
来源：http://ds.newstarts.cn

Go:   // 手写 map[int]int
来源：http://dw.bjjhwx.cn

Ruby: // 手写 Hash
来源：http://if.panjiajie.cn

C#:   // 手写 Dictionary<int, int>
来源：http://th.yuexingan06.cn

[N08] 生成全排列
来源：http://kx.hahajie.cn

Py:   itertools.permutations(arr)
来源：http://mr.huixiangedu.cn

PHP:  // 手写递归交换
来源：http://he.nszjky.cn

JS:   // 手写回溯递归
来源：http://mg.szsharing.cn

TS:   // 手写回溯递归
来源：http://it.bookmarksfly.cn

Java: // 手写回溯递归
来源：http://bd.521024.cn

Go:   // 手写回溯递归
来源：http://bv.bookmarksfly.cn

Ruby: arr.permutation.to_a
来源：http://oq.newstarts.cn

C#:   // 手写回溯递归
来源：http://cv.bjjhwx.cn

[N09] 栈与队列
来源：http://xe.jctech888.com.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hr.shxzukj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hm.huixinmuqiang.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wf.yuntaijiaju.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://et.nszjky.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://sy.yuexingan06.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://yp.hahajie.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://nn.bookmarksfly.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://sk.yuexingan06.cn

[N10] 链表节点定义
来源：http://za.bookmarksfly.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://no.newstarts.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://yf.shtwfgs.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ac.huixiangedu.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://dj.jianghongdianzi.cn

Java: class Node { int v; Node next; }
来源：http://cc.huixiangedu.cn

Go:   type Node struct { V int; Next *Node }
来源：http://qe.asd995.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://gh.huanxung.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ww.hahajie.cn

[N11] 二叉树中序遍历
来源：http://eu.muxihuayi.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ol.hnjuh.cn

PHP:  // 手写递归函数
来源：http://rn.shtwfgs.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ns.chemitech.net.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gy.szsharing.cn

Java: // 手写递归
来源：http://nf.jianghongdianzi.cn

Go:   // 手写递归
来源：http://fs.nszjky.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://zm.gzmigu.cn

C#:   // 手写递归
来源：http://dd.jianghongdianzi.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://or.chemitech.net.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ve.haigaiapp.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ur.colortex.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rl.szsharing.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ff.yuntaijiaju.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://nb.wgjwhj.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://cz.9csxet.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://cy.huanxung.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://vm.yuntaijiaju.cn

================================================================================
来源：http://ka.yuntaijiaju.cn

O. 并发与异步
来源：http://pl.panjiajie.cn

================================================================================
来源：http://nz.jianghongdianzi.cn

[O01] 启动一个线程
来源：http://sd.szsharing.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hb.521024.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://xf.huanxung.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://of.haigaiapp.cn

TS:   // 同 JS
来源：http://vq.chemitech.net.cn

Java: new Thread(() -> f()).start()
来源：http://ez.yuntaijiaju.cn

Go:   go f()
来源：http://pc.chemitech.net.cn

Ruby: Thread.new { f }
来源：http://gh.panjiajie.cn

C#:   Task.Run(() => F());
来源：http://lv.shtwfgs.cn

[O02] 使用线程池
来源：http://xz.huixinmuqiang.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://jm.wgjwhj.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://bf.asd995.cn

JS:   // worker_threads 线程池
来源：http://kq.wgjwhj.cn

TS:   // worker_threads 线程池
来源：http://nr.bookmarksfly.cn

Java: Executors.newFixedThreadPool(4)
来源：http://pt.szsharing.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hs.asd995.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://yu.yuntaijiaju.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mr.wgjwhj.cn

[O03] 加锁保护共享数据
来源：http://pa.haigaiapp.cn

Py:   with lock: shared += 1
来源：http://vi.gzmigu.cn

PHP:  // 用 flock() 做文件锁
来源：http://gi.chemitech.net.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://qk.huixinmuqiang.cn

TS:   // 同 JS
来源：http://gl.huanxung.cn

Java: synchronized (this) { shared++; }
来源：http://ov.yuntaijiaju.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.bjjhwx.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://hm.bjjhwx.cn

C#:   lock (gate) { shared++; }
来源：http://ar.lnxyls.cn

[O04] 定义异步函数并等待
来源：http://lo.newstarts.cn

Py:   async def f():⏎    await g()
来源：http://hn.hahajie.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://as.colortex.cn

JS:   async function f() { await g(); }
来源：http://if.jianghongdianzi.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ae.gzmigu.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://fg.jianghongdianzi.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://nz.colortex.cn

Ruby: # 用 Fiber 或 async gem
来源：http://iw.huixinmuqiang.cn

C#:   async Task F() { await G(); }
来源：http://se.bookmarksfly.cn

[O05] 并发执行并等待全部完成
来源：http://mn.panjiajie.cn

Py:   asyncio.gather(*tasks)
来源：http://vy.haigaiapp.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://cr.shxzskj.cn

JS:   await Promise.all(tasks)
来源：http://el.asd995.cn

TS:   await Promise.all(tasks)
来源：http://jv.nszjky.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ua.wgjwhj.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://kj.chemitech.net.cn

Ruby: threads.map(&:join)
来源：http://bt.newstarts.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://us.haigaiapp.cn

[O06] 使用进程池
来源：http://gf.huanxung.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://lc.panjiajie.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://xy.9csxet.cn

JS:   // child_process / cluster 模块
来源：http://tz.panjiajie.cn


<!-- 参考信息 -->