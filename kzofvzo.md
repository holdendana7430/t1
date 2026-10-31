代发 wailian999

Py:   requests.post(url, json={"a": 1})
来源：http://jq.yuntaijiaju.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://kx.chemitech.net.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://at.muxihuayi.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pc.jianghongdianzi.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://kk.wgjwhj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://gu.haigaiapp.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wj.haigaiapp.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://tc.newstarts.cn

[L03] 设置自定义请求头
来源：http://ow.wgjwhj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ky.haigaiapp.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://sm.bjjhwx.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://go.panjiajie.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ql.nszjky.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://lo.shxzukj.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://pi.hahajie.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://fj.huanxung.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://sq.nicolike.cn

[L04] 设置超时
来源：http://lt.bookmarksfly.cn

Py:   requests.get(url, timeout=5)
来源：http://lb.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://my.jianghongdianzi.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qw.huanxung.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jf.nszjky.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ji.shtwfgs.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://pc.hnjuh.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://sa.szxytkj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://pt.521024.cn

[L05] 上传文件（multipart）
来源：http://jn.lnxyls.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://tt.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ga.colortex.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://oe.huixiangedu.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ec.szsharing.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ki.szxytkj.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://lr.huanxung.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ao.gzmigu.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://jt.jctech888.com.cn

[L06] 解析响应为 JSON
来源：http://ah.muxihuayi.cn

Py:   resp.json()
来源：http://dq.panjiajie.cn

PHP:  json_decode($body, true);
来源：http://bs.huixiangedu.cn

JS:   await resp.json()
来源：http://un.yuntaijiaju.cn

TS:   await resp.json()
来源：http://zz.szxytkj.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://bq.yuntaijiaju.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://qe.yuntaijiaju.cn

Ruby: JSON.parse(resp.body)
来源：http://yh.haigaiapp.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://db.521024.cn

[L07] 处理 HTTP 状态码
来源：http://uj.shxzukj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://du.lnxyls.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qr.haigaiapp.cn

JS:   resp.ok;  resp.status
来源：http://ou.gzmigu.cn

TS:   resp.ok;  resp.status
来源：http://kh.9csxet.cn

Java: resp.statusCode()
来源：http://rs.huixinmuqiang.cn

Go:   resp.StatusCode
来源：http://cl.jctech888.com.cn

Ruby: resp.code.to_i
来源：http://co.jianghongdianzi.cn

C#:   (int)resp.StatusCode
来源：http://gb.bookmarksfly.cn

[L08] 并发请求多个地址
来源：http://xu.wgjwhj.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ev.yuexingan06.cn

PHP:  curl_multi_init() 系列
来源：http://zx.wgjwhj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://su.521024.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vy.hnjuh.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hy.huanxung.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ge.chemitech.net.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://pb.wgjwhj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://we.muxihuayi.cn

================================================================================
来源：http://up.szxytkj.cn

M. 命令行 / 进程 / 环境
来源：http://pz.lnxyls.cn

================================================================================
来源：http://ez.wgjwhj.cn

[M01] 读取命令行参数
来源：http://ht.szsharing.cn

Py:   sys.argv[1:]
来源：http://eq.asd995.cn

PHP:  $argv;  $argc;
来源：http://al.gzmigu.cn

JS:   process.argv.slice(2)
来源：http://ym.bjjhwx.cn

TS:   process.argv.slice(2)
来源：http://dw.shtwfgs.cn

Java: args 数组（main 方法参数）
来源：http://bc.hnjuh.cn

Go:   os.Args[1:]
来源：http://qu.asd995.cn

Ruby: ARGV
来源：http://tf.bjjhwx.cn

C#:   args 数组（Main 方法参数）
来源：http://tx.521024.cn

[M02] 读取环境变量
来源：http://xj.szxytkj.cn

Py:   os.environ.get("HOME")
来源：http://vd.panjiajie.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://lz.nicolike.cn

JS:   process.env.HOME
来源：http://ay.szsharing.cn

TS:   process.env.HOME
来源：http://kr.shtwfgs.cn

Java: System.getenv("HOME")
来源：http://bw.jctech888.com.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ih.asd995.cn

Ruby: ENV["HOME"]
来源：http://nm.wgjwhj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ea.yuexingan06.cn

[M03] 执行外部命令
来源：http://ns.huanxung.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://in.huanxung.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ch.521024.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://bx.muxihuayi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://nc.lnxyls.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://os.panjiajie.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ze.huixinmuqiang.cn

Ruby: system("ls -l");  `ls -l`
来源：http://oy.hahajie.cn

C#:   Process.Start("ls", "-l");
来源：http://qx.jianghongdianzi.cn

[M04] 获取当前工作目录
来源：http://df.nszjky.cn

Py:   os.getcwd()
来源：http://at.panjiajie.cn

PHP:  getcwd();
来源：http://rs.jianghongdianzi.cn

JS:   process.cwd()
来源：http://pj.shtwfgs.cn

TS:   process.cwd()
来源：http://fx.haigaiapp.cn

Java: Path.of("").toAbsolutePath()
来源：http://yy.asd995.cn

Go:   os.Getwd()
来源：http://lk.bjjhwx.cn

Ruby: Dir.pwd
来源：http://jb.yuntaijiaju.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ga.gzmigu.cn

[M05] 设置退出码
来源：http://ww.huanxung.cn

Py:   sys.exit(1)
来源：http://bb.shtwfgs.cn

PHP:  exit(1);
来源：http://hf.shxzskj.cn

JS:   process.exit(1)
来源：http://qg.szsharing.cn

TS:   process.exit(1)
来源：http://oc.chemitech.net.cn

Java: System.exit(1)
来源：http://cc.huixinmuqiang.cn

Go:   os.Exit(1)
来源：http://xj.huixiangedu.cn

Ruby: exit 1
来源：http://zj.asd995.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mf.jctech888.com.cn

[M06] 向标准错误输出
来源：http://pe.bookmarksfly.cn

Py:   print("err", file=sys.stderr)
来源：http://dk.newstarts.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://vi.jctech888.com.cn

JS:   console.error("err")
来源：http://gg.shxzskj.cn

TS:   console.error("err")
来源：http://cc.nicolike.cn

Java: System.err.println("err")
来源：http://yw.bjjhwx.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://gf.nszjky.cn

Ruby: warn "err"
来源：http://ki.huixiangedu.cn

C#:   Console.Error.WriteLine("err")
来源：http://wa.shtwfgs.cn

[M07] 判断是否为主入口
来源：http://kn.szxytkj.cn

Py:   if __name__ == "__main__":
来源：http://uu.huixinmuqiang.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://lt.szxytkj.cn

JS:   require.main === module
来源：http://ac.jctech888.com.cn

TS:   require.main === module
来源：http://hi.hnjuh.cn

Java: public static void main(String[] args)
来源：http://hu.nszjky.cn

Go:   func main()
来源：http://lw.yuexingan06.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://kt.newstarts.cn

C#:   static void Main(string[] args)
来源：http://zt.szsharing.cn

[M08] 获取系统与运行时信息
来源：http://su.huixiangedu.cn

Py:   platform.system();  platform.python_version()
来源：http://mq.lnxyls.cn

PHP:  PHP_OS;  phpversion();
来源：http://fp.jctech888.com.cn

JS:   process.platform;  process.version
来源：http://wb.huanxung.cn

TS:   process.platform;  process.version
来源：http://hv.521024.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://rc.yuexingan06.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://jm.yuexingan06.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mq.asd995.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://sc.yuexingan06.cn

================================================================================
来源：http://xq.colortex.cn

N. 数据结构与算法
来源：http://up.lnxyls.cn

================================================================================
来源：http://jo.bjjhwx.cn

[N01] 二分查找（有序数组）
来源：http://ft.lnxyls.cn

Py:   bisect.bisect_left(arr, x)
来源：http://aw.huixiangedu.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wt.gzmigu.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lj.shtwfgs.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ua.huanxung.cn

Java: Arrays.binarySearch(arr, x)
来源：http://oe.szxytkj.cn

Go:   sort.SearchInts(arr, x)
来源：http://gc.shxzskj.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://mc.shxzskj.cn

C#:   Array.BinarySearch(arr, x)
来源：http://vd.wgjwhj.cn

[N02] 排序（工程实践用内置实现）
来源：http://zf.szsharing.cn

Py:   sorted(arr);  arr.sort()
来源：http://pe.newstarts.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://gp.shtwfgs.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://no.hnjuh.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://vi.nicolike.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ft.yuntaijiaju.cn

Go:   slices.Sort(arr)
来源：http://hk.521024.cn

Ruby: arr.sort
来源：http://nn.521024.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ol.jctech888.com.cn

[N03] 快速排序（分治示例）
来源：http://lt.521024.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ys.huixiangedu.cn

PHP:  // 递归实现，或用 usort
来源：http://ul.lnxyls.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kv.newstarts.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ew.521024.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://sr.szxytkj.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ka.521024.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://vo.huixiangedu.cn

C#:   // 手写递归，或 Array.Sort
来源：http://we.yuexingan06.cn

[N04] 斐波那契数列
来源：http://jj.9csxet.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://fs.yuexingan06.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://bz.nszjky.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bn.521024.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ne.nicolike.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://cy.bookmarksfly.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hx.jctech888.com.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://vo.jianghongdianzi.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ao.nszjky.cn

[N05] 最大公约数
来源：http://kl.chemitech.net.cn

Py:   math.gcd(a, b)
来源：http://xo.szxytkj.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ej.nicolike.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://be.huanxung.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ih.huanxung.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://pv.wgjwhj.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://oi.muxihuayi.cn

Ruby: a.gcd(b)
来源：http://vn.nicolike.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://yg.gzmigu.cn

[N06] 判断回文字符串
来源：http://ww.bjjhwx.cn

Py:   s == s[::-1]
来源：http://xp.jianghongdianzi.cn

PHP:  $s === strrev($s);
来源：http://gm.szxytkj.cn

JS:   s === [...s].reverse().join("")
来源：http://vh.colortex.cn

TS:   s === [...s].reverse().join("")
来源：http://iy.jianghongdianzi.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://bu.bookmarksfly.cn

Go:   // 双指针从两端比较
来源：http://nz.nszjky.cn

Ruby: s == s.reverse
来源：http://ai.gzmigu.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://qy.gzmigu.cn

[N07] 两数之和（返回下标）
来源：http://oe.jctech888.com.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://sj.yuexingan06.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ic.chemitech.net.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://fh.nszjky.cn

TS:   // 手写 Map<string, number>
来源：http://tm.shxzskj.cn

Java: // 手写 HashMap
来源：http://ke.521024.cn

Go:   // 手写 map[int]int
来源：http://hd.muxihuayi.cn

Ruby: // 手写 Hash
来源：http://vb.haigaiapp.cn

C#:   // 手写 Dictionary<int, int>
来源：http://lj.521024.cn

[N08] 生成全排列
来源：http://gl.muxihuayi.cn

Py:   itertools.permutations(arr)
来源：http://xk.colortex.cn

PHP:  // 手写递归交换
来源：http://yi.nszjky.cn

JS:   // 手写回溯递归
来源：http://lv.szxytkj.cn

TS:   // 手写回溯递归
来源：http://ny.newstarts.cn

Java: // 手写回溯递归
来源：http://ps.yuntaijiaju.cn

Go:   // 手写回溯递归
来源：http://sc.huixiangedu.cn

Ruby: arr.permutation.to_a
来源：http://zq.muxihuayi.cn

C#:   // 手写回溯递归
来源：http://pq.hahajie.cn

[N09] 栈与队列
来源：http://ph.asd995.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://si.chemitech.net.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mc.gzmigu.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://zo.newstarts.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://nz.newstarts.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://es.hahajie.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://md.nszjky.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ma.shxzskj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://by.bookmarksfly.cn

[N10] 链表节点定义
来源：http://en.521024.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://lf.yuntaijiaju.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://mt.hahajie.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://oi.nszjky.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://cc.lnxyls.cn

Java: class Node { int v; Node next; }
来源：http://aa.huixinmuqiang.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ab.szxytkj.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://bf.lnxyls.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://fx.szxytkj.cn

[N11] 二叉树中序遍历
来源：http://kd.newstarts.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wi.bjjhwx.cn

PHP:  // 手写递归函数
来源：http://zz.newstarts.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rx.521024.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jv.shxzukj.cn

Java: // 手写递归
来源：http://yj.hahajie.cn

Go:   // 手写递归
来源：http://dw.jianghongdianzi.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://gq.chemitech.net.cn

C#:   // 手写递归
来源：http://jg.jianghongdianzi.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://cr.521024.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://jj.huixiangedu.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://pr.lnxyls.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yo.shxzukj.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pv.yuntaijiaju.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ct.panjiajie.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://pa.colortex.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://xc.yuexingan06.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://bw.panjiajie.cn

================================================================================
来源：http://no.lnxyls.cn

O. 并发与异步
来源：http://nr.jianghongdianzi.cn

================================================================================
来源：http://nx.haigaiapp.cn

[O01] 启动一个线程
来源：http://vm.colortex.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://nm.jctech888.com.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://zr.haigaiapp.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://en.muxihuayi.cn

TS:   // 同 JS
来源：http://vv.huixinmuqiang.cn

Java: new Thread(() -> f()).start()
来源：http://ay.huixinmuqiang.cn

Go:   go f()
来源：http://es.szxytkj.cn

Ruby: Thread.new { f }
来源：http://zm.jianghongdianzi.cn

C#:   Task.Run(() => F());
来源：http://qa.newstarts.cn

[O02] 使用线程池
来源：http://bz.bjjhwx.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://rj.hahajie.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://rj.gzmigu.cn

JS:   // worker_threads 线程池
来源：http://ao.chemitech.net.cn

TS:   // worker_threads 线程池
来源：http://ww.9csxet.cn

Java: Executors.newFixedThreadPool(4)
来源：http://rd.panjiajie.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ah.szsharing.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mn.chemitech.net.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://gs.haigaiapp.cn

[O03] 加锁保护共享数据
来源：http://vn.lnxyls.cn

Py:   with lock: shared += 1
来源：http://bf.nicolike.cn

PHP:  // 用 flock() 做文件锁
来源：http://gx.hnjuh.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://iz.jianghongdianzi.cn

TS:   // 同 JS
来源：http://wi.hahajie.cn

Java: synchronized (this) { shared++; }
来源：http://fq.wgjwhj.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mk.jianghongdianzi.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://fx.haigaiapp.cn

C#:   lock (gate) { shared++; }
来源：http://ek.panjiajie.cn

[O04] 定义异步函数并等待
来源：http://rh.hahajie.cn

Py:   async def f():⏎    await g()
来源：http://mi.huanxung.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://of.szxytkj.cn

JS:   async function f() { await g(); }
来源：http://ku.bjjhwx.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://fn.panjiajie.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hr.jctech888.com.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ys.szxytkj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ds.szxytkj.cn

C#:   async Task F() { await G(); }
来源：http://wd.bookmarksfly.cn

[O05] 并发执行并等待全部完成
来源：http://ne.bjjhwx.cn

Py:   asyncio.gather(*tasks)
来源：http://wt.yuntaijiaju.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://km.shtwfgs.cn

JS:   await Promise.all(tasks)
来源：http://ho.jctech888.com.cn

TS:   await Promise.all(tasks)
来源：http://kn.panjiajie.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hi.panjiajie.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://zr.huixinmuqiang.cn

Ruby: threads.map(&:join)
来源：http://xs.huanxung.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://vv.9csxet.cn

[O06] 使用进程池
来源：http://rz.colortex.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mz.haigaiapp.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://gt.shtwfgs.cn

JS:   // child_process / cluster 模块
来源：http://rv.hahajie.cn


<!-- 参考信息 -->