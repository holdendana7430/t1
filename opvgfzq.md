代发 wailian999

Py:   requests.post(url, json={"a": 1})
来源：http://ns.gzmigu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ir.newstarts.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ws.newstarts.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nq.chemitech.net.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vr.nszjky.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ii.yuntaijiaju.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://zd.panjiajie.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://vg.huixinmuqiang.cn

[L03] 设置自定义请求头
来源：http://wm.yuntaijiaju.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ch.hnjuh.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ql.hahajie.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jf.nszjky.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jk.huanxung.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://kw.huanxung.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wu.muxihuayi.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://uz.yuntaijiaju.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://rl.bookmarksfly.cn

[L04] 设置超时
来源：http://kf.9csxet.cn

Py:   requests.get(url, timeout=5)
来源：http://br.gzmigu.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xh.jctech888.com.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lj.yuexingan06.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ml.bookmarksfly.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://uf.shxzskj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://dp.hnjuh.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ox.shxzukj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://gy.huanxung.cn

[L05] 上传文件（multipart）
来源：http://po.jctech888.com.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://uf.szsharing.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ua.yuexingan06.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ew.yuexingan06.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://pa.bjjhwx.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://tf.jctech888.com.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mi.jianghongdianzi.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ej.521024.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://eb.yuntaijiaju.cn

[L06] 解析响应为 JSON
来源：http://ps.bookmarksfly.cn

Py:   resp.json()
来源：http://sk.szxytkj.cn

PHP:  json_decode($body, true);
来源：http://se.shxzukj.cn

JS:   await resp.json()
来源：http://zc.panjiajie.cn

TS:   await resp.json()
来源：http://dv.bjjhwx.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://bj.hahajie.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ri.huixinmuqiang.cn

Ruby: JSON.parse(resp.body)
来源：http://ny.panjiajie.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://au.panjiajie.cn

[L07] 处理 HTTP 状态码
来源：http://im.shtwfgs.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://sc.wgjwhj.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ze.jianghongdianzi.cn

JS:   resp.ok;  resp.status
来源：http://sf.newstarts.cn

TS:   resp.ok;  resp.status
来源：http://lx.bjjhwx.cn

Java: resp.statusCode()
来源：http://aq.bjjhwx.cn

Go:   resp.StatusCode
来源：http://zj.colortex.cn

Ruby: resp.code.to_i
来源：http://bd.panjiajie.cn

C#:   (int)resp.StatusCode
来源：http://ox.lnxyls.cn

[L08] 并发请求多个地址
来源：http://we.haigaiapp.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://bu.bookmarksfly.cn

PHP:  curl_multi_init() 系列
来源：http://af.jctech888.com.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tp.szsharing.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ba.yuntaijiaju.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ib.huanxung.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hk.nicolike.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://fm.bookmarksfly.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ci.nszjky.cn

================================================================================
来源：http://pl.colortex.cn

M. 命令行 / 进程 / 环境
来源：http://cl.bookmarksfly.cn

================================================================================
来源：http://vm.asd995.cn

[M01] 读取命令行参数
来源：http://bb.wgjwhj.cn

Py:   sys.argv[1:]
来源：http://jk.huixinmuqiang.cn

PHP:  $argv;  $argc;
来源：http://yj.huixinmuqiang.cn

JS:   process.argv.slice(2)
来源：http://wm.hahajie.cn

TS:   process.argv.slice(2)
来源：http://py.muxihuayi.cn

Java: args 数组（main 方法参数）
来源：http://vu.521024.cn

Go:   os.Args[1:]
来源：http://ug.asd995.cn

Ruby: ARGV
来源：http://ko.colortex.cn

C#:   args 数组（Main 方法参数）
来源：http://kd.yuexingan06.cn

[M02] 读取环境变量
来源：http://dz.huixiangedu.cn

Py:   os.environ.get("HOME")
来源：http://cc.9csxet.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://pz.yuexingan06.cn

JS:   process.env.HOME
来源：http://oc.szsharing.cn

TS:   process.env.HOME
来源：http://to.bookmarksfly.cn

Java: System.getenv("HOME")
来源：http://mp.yuntaijiaju.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://uw.szsharing.cn

Ruby: ENV["HOME"]
来源：http://mb.hnjuh.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ln.nicolike.cn

[M03] 执行外部命令
来源：http://dy.huixinmuqiang.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://xe.shxzskj.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ox.jctech888.com.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://qo.huixiangedu.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://um.panjiajie.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://zm.bookmarksfly.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://vv.shtwfgs.cn

Ruby: system("ls -l");  `ls -l`
来源：http://gh.nszjky.cn

C#:   Process.Start("ls", "-l");
来源：http://cv.jianghongdianzi.cn

[M04] 获取当前工作目录
来源：http://js.muxihuayi.cn

Py:   os.getcwd()
来源：http://xy.asd995.cn

PHP:  getcwd();
来源：http://ek.nicolike.cn

JS:   process.cwd()
来源：http://ym.muxihuayi.cn

TS:   process.cwd()
来源：http://ut.521024.cn

Java: Path.of("").toAbsolutePath()
来源：http://wd.haigaiapp.cn

Go:   os.Getwd()
来源：http://yq.hnjuh.cn

Ruby: Dir.pwd
来源：http://cj.huixinmuqiang.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ls.chemitech.net.cn

[M05] 设置退出码
来源：http://rt.9csxet.cn

Py:   sys.exit(1)
来源：http://bi.shxzskj.cn

PHP:  exit(1);
来源：http://ux.panjiajie.cn

JS:   process.exit(1)
来源：http://yu.panjiajie.cn

TS:   process.exit(1)
来源：http://zh.asd995.cn

Java: System.exit(1)
来源：http://fu.shxzskj.cn

Go:   os.Exit(1)
来源：http://ha.huixinmuqiang.cn

Ruby: exit 1
来源：http://ma.szsharing.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ve.muxihuayi.cn

[M06] 向标准错误输出
来源：http://wg.haigaiapp.cn

Py:   print("err", file=sys.stderr)
来源：http://rn.chemitech.net.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ih.haigaiapp.cn

JS:   console.error("err")
来源：http://hz.nicolike.cn

TS:   console.error("err")
来源：http://cf.huixinmuqiang.cn

Java: System.err.println("err")
来源：http://rl.huanxung.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://es.521024.cn

Ruby: warn "err"
来源：http://tw.shtwfgs.cn

C#:   Console.Error.WriteLine("err")
来源：http://ve.nszjky.cn

[M07] 判断是否为主入口
来源：http://qi.yuexingan06.cn

Py:   if __name__ == "__main__":
来源：http://qz.muxihuayi.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://nl.bjjhwx.cn

JS:   require.main === module
来源：http://xy.shtwfgs.cn

TS:   require.main === module
来源：http://jr.colortex.cn

Java: public static void main(String[] args)
来源：http://vb.huixiangedu.cn

Go:   func main()
来源：http://sn.shxzukj.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mv.asd995.cn

C#:   static void Main(string[] args)
来源：http://sz.jctech888.com.cn

[M08] 获取系统与运行时信息
来源：http://ww.jianghongdianzi.cn

Py:   platform.system();  platform.python_version()
来源：http://ss.panjiajie.cn

PHP:  PHP_OS;  phpversion();
来源：http://ci.yuntaijiaju.cn

JS:   process.platform;  process.version
来源：http://dl.nicolike.cn

TS:   process.platform;  process.version
来源：http://af.shxzskj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://cy.bookmarksfly.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ax.yuntaijiaju.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://qt.huanxung.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://bb.bookmarksfly.cn

================================================================================
来源：http://xg.muxihuayi.cn

N. 数据结构与算法
来源：http://bp.colortex.cn

================================================================================
来源：http://hz.hahajie.cn

[N01] 二分查找（有序数组）
来源：http://da.newstarts.cn

Py:   bisect.bisect_left(arr, x)
来源：http://nh.szsharing.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://nw.szxytkj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cu.huixiangedu.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mw.panjiajie.cn

Java: Arrays.binarySearch(arr, x)
来源：http://kx.shxzukj.cn

Go:   sort.SearchInts(arr, x)
来源：http://rd.asd995.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ly.yuntaijiaju.cn

C#:   Array.BinarySearch(arr, x)
来源：http://hy.szsharing.cn

[N02] 排序（工程实践用内置实现）
来源：http://uw.nicolike.cn

Py:   sorted(arr);  arr.sort()
来源：http://ho.gzmigu.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://iy.yuexingan06.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://uo.szxytkj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://oq.bookmarksfly.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ec.colortex.cn

Go:   slices.Sort(arr)
来源：http://mv.9csxet.cn

Ruby: arr.sort
来源：http://ov.colortex.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://fo.colortex.cn

[N03] 快速排序（分治示例）
来源：http://yy.szxytkj.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://tn.shtwfgs.cn

PHP:  // 递归实现，或用 usort
来源：http://bl.shxzukj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vq.chemitech.net.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yv.shtwfgs.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://eh.huixinmuqiang.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://bx.hnjuh.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://kc.muxihuayi.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ld.chemitech.net.cn

[N04] 斐波那契数列
来源：http://xm.hahajie.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://cg.hahajie.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ip.colortex.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qx.shxzukj.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sa.wgjwhj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://lb.asd995.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://zi.huanxung.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://xz.shtwfgs.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://st.jctech888.com.cn

[N05] 最大公约数
来源：http://bl.huixiangedu.cn

Py:   math.gcd(a, b)
来源：http://pl.huixiangedu.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://dh.gzmigu.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yv.bookmarksfly.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qk.nicolike.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zz.gzmigu.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ql.jianghongdianzi.cn

Ruby: a.gcd(b)
来源：http://lc.9csxet.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://di.hnjuh.cn

[N06] 判断回文字符串
来源：http://pn.shxzskj.cn

Py:   s == s[::-1]
来源：http://tt.colortex.cn

PHP:  $s === strrev($s);
来源：http://wg.shtwfgs.cn

JS:   s === [...s].reverse().join("")
来源：http://aq.jianghongdianzi.cn

TS:   s === [...s].reverse().join("")
来源：http://rp.asd995.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xa.colortex.cn

Go:   // 双指针从两端比较
来源：http://nj.hnjuh.cn

Ruby: s == s.reverse
来源：http://zy.shxzukj.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://uq.wgjwhj.cn

[N07] 两数之和（返回下标）
来源：http://xy.lnxyls.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://me.shtwfgs.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://xy.hahajie.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://vs.bjjhwx.cn

TS:   // 手写 Map<string, number>
来源：http://ut.colortex.cn

Java: // 手写 HashMap
来源：http://ly.shtwfgs.cn

Go:   // 手写 map[int]int
来源：http://cv.yuexingan06.cn

Ruby: // 手写 Hash
来源：http://ie.yuexingan06.cn

C#:   // 手写 Dictionary<int, int>
来源：http://kk.haigaiapp.cn

[N08] 生成全排列
来源：http://zl.bjjhwx.cn

Py:   itertools.permutations(arr)
来源：http://pv.bookmarksfly.cn

PHP:  // 手写递归交换
来源：http://us.wgjwhj.cn

JS:   // 手写回溯递归
来源：http://js.jctech888.com.cn

TS:   // 手写回溯递归
来源：http://wj.szxytkj.cn

Java: // 手写回溯递归
来源：http://tw.szxytkj.cn

Go:   // 手写回溯递归
来源：http://ja.jianghongdianzi.cn

Ruby: arr.permutation.to_a
来源：http://ab.yuntaijiaju.cn

C#:   // 手写回溯递归
来源：http://oq.muxihuayi.cn

[N09] 栈与队列
来源：http://bg.szxytkj.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://fm.bookmarksfly.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://pe.panjiajie.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hl.hahajie.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ia.jctech888.com.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://kf.yuexingan06.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://jd.szsharing.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://bg.shxzskj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ty.bjjhwx.cn

[N10] 链表节点定义
来源：http://zp.huanxung.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ue.huanxung.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://qn.9csxet.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ku.jctech888.com.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://fr.szsharing.cn

Java: class Node { int v; Node next; }
来源：http://pn.521024.cn

Go:   type Node struct { V int; Next *Node }
来源：http://qs.chemitech.net.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ka.haigaiapp.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://gh.wgjwhj.cn

[N11] 二叉树中序遍历
来源：http://ai.hahajie.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wi.9csxet.cn

PHP:  // 手写递归函数
来源：http://ps.huanxung.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://oo.huixinmuqiang.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sn.hnjuh.cn

Java: // 手写递归
来源：http://br.bjjhwx.cn

Go:   // 手写递归
来源：http://ut.asd995.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mp.bjjhwx.cn

C#:   // 手写递归
来源：http://jz.shxzskj.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://rg.gzmigu.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://sg.lnxyls.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mk.chemitech.net.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://uo.huixiangedu.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lk.bookmarksfly.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://lt.szsharing.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://po.wgjwhj.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://bk.muxihuayi.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://oo.lnxyls.cn

================================================================================
来源：http://xy.jctech888.com.cn

O. 并发与异步
来源：http://hb.bookmarksfly.cn

================================================================================
来源：http://gg.szsharing.cn

[O01] 启动一个线程
来源：http://iw.bjjhwx.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://vd.jianghongdianzi.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://pa.hahajie.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://vr.chemitech.net.cn

TS:   // 同 JS
来源：http://rc.hnjuh.cn

Java: new Thread(() -> f()).start()
来源：http://gm.gzmigu.cn

Go:   go f()
来源：http://pw.huanxung.cn

Ruby: Thread.new { f }
来源：http://no.muxihuayi.cn

C#:   Task.Run(() => F());
来源：http://kd.hahajie.cn

[O02] 使用线程池
来源：http://dg.9csxet.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ix.szxytkj.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://bl.yuntaijiaju.cn

JS:   // worker_threads 线程池
来源：http://yq.szxytkj.cn

TS:   // worker_threads 线程池
来源：http://or.hahajie.cn

Java: Executors.newFixedThreadPool(4)
来源：http://eq.newstarts.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://bq.yuexingan06.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://gg.haigaiapp.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hl.bjjhwx.cn

[O03] 加锁保护共享数据
来源：http://uc.huixiangedu.cn

Py:   with lock: shared += 1
来源：http://cp.newstarts.cn

PHP:  // 用 flock() 做文件锁
来源：http://tg.yuntaijiaju.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://pb.szxytkj.cn

TS:   // 同 JS
来源：http://la.bjjhwx.cn

Java: synchronized (this) { shared++; }
来源：http://vj.chemitech.net.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://aj.9csxet.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://tk.jctech888.com.cn

C#:   lock (gate) { shared++; }
来源：http://qb.nicolike.cn

[O04] 定义异步函数并等待
来源：http://vu.hahajie.cn

Py:   async def f():⏎    await g()
来源：http://of.haigaiapp.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://zy.asd995.cn

JS:   async function f() { await g(); }
来源：http://wy.bookmarksfly.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://lt.yuexingan06.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://gw.huixinmuqiang.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://pe.nszjky.cn

Ruby: # 用 Fiber 或 async gem
来源：http://bz.nicolike.cn

C#:   async Task F() { await G(); }
来源：http://er.jctech888.com.cn

[O05] 并发执行并等待全部完成
来源：http://ea.jianghongdianzi.cn

Py:   asyncio.gather(*tasks)
来源：http://yu.jianghongdianzi.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ui.szsharing.cn

JS:   await Promise.all(tasks)
来源：http://az.haigaiapp.cn

TS:   await Promise.all(tasks)
来源：http://ct.chemitech.net.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ic.chemitech.net.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ui.wgjwhj.cn

Ruby: threads.map(&:join)
来源：http://lu.gzmigu.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://eq.colortex.cn

[O06] 使用进程池
来源：http://qq.bjjhwx.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://df.panjiajie.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://rr.nszjky.cn

JS:   // child_process / cluster 模块
来源：http://sv.bjjhwx.cn


<!-- 参考信息 -->