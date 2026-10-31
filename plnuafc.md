代发 wailian999

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://gc.asd995.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://sz.huixiangedu.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://tx.jctech888.com.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://rt.nicolike.cn

[L03] 设置自定义请求头
来源：http://vs.jianghongdianzi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://cd.hnjuh.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ay.asd995.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bq.hnjuh.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rc.huixinmuqiang.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mx.jianghongdianzi.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mz.shxzukj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://tf.yuntaijiaju.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://bm.haigaiapp.cn

[L04] 设置超时
来源：http://go.nicolike.cn

Py:   requests.get(url, timeout=5)
来源：http://yw.521024.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://yy.colortex.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xt.yuexingan06.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://au.huixiangedu.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://fc.bjjhwx.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wu.huanxung.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://gj.nicolike.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ot.shxzskj.cn

[L05] 上传文件（multipart）
来源：http://ko.shxzskj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://rs.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://tz.shtwfgs.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mf.wgjwhj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://rz.chemitech.net.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://gk.shxzskj.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://pq.hnjuh.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://xa.wgjwhj.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://um.yuntaijiaju.cn

[L06] 解析响应为 JSON
来源：http://eg.shxzukj.cn

Py:   resp.json()
来源：http://cd.newstarts.cn

PHP:  json_decode($body, true);
来源：http://kv.nszjky.cn

JS:   await resp.json()
来源：http://ra.colortex.cn

TS:   await resp.json()
来源：http://gi.jianghongdianzi.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://me.huixinmuqiang.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ry.huixiangedu.cn

Ruby: JSON.parse(resp.body)
来源：http://fq.521024.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://bd.colortex.cn

[L07] 处理 HTTP 状态码
来源：http://ys.nicolike.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hn.9csxet.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://sh.wgjwhj.cn

JS:   resp.ok;  resp.status
来源：http://ty.gzmigu.cn

TS:   resp.ok;  resp.status
来源：http://yz.yuexingan06.cn

Java: resp.statusCode()
来源：http://iz.wgjwhj.cn

Go:   resp.StatusCode
来源：http://ne.colortex.cn

Ruby: resp.code.to_i
来源：http://zl.jctech888.com.cn

C#:   (int)resp.StatusCode
来源：http://jo.newstarts.cn

[L08] 并发请求多个地址
来源：http://lt.nszjky.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hc.jianghongdianzi.cn

PHP:  curl_multi_init() 系列
来源：http://uu.haigaiapp.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://aw.shtwfgs.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xn.shxzukj.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://br.chemitech.net.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://cd.asd995.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vv.szxytkj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://sh.haigaiapp.cn

================================================================================
来源：http://rk.bookmarksfly.cn

M. 命令行 / 进程 / 环境
来源：http://my.hnjuh.cn

================================================================================
来源：http://oq.muxihuayi.cn

[M01] 读取命令行参数
来源：http://if.521024.cn

Py:   sys.argv[1:]
来源：http://va.haigaiapp.cn

PHP:  $argv;  $argc;
来源：http://tt.gzmigu.cn

JS:   process.argv.slice(2)
来源：http://lw.muxihuayi.cn

TS:   process.argv.slice(2)
来源：http://to.yuntaijiaju.cn

Java: args 数组（main 方法参数）
来源：http://fn.shtwfgs.cn

Go:   os.Args[1:]
来源：http://eq.szsharing.cn

Ruby: ARGV
来源：http://xb.gzmigu.cn

C#:   args 数组（Main 方法参数）
来源：http://fj.lnxyls.cn

[M02] 读取环境变量
来源：http://ao.huixiangedu.cn

Py:   os.environ.get("HOME")
来源：http://ku.shxzskj.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://di.nicolike.cn

JS:   process.env.HOME
来源：http://qg.haigaiapp.cn

TS:   process.env.HOME
来源：http://sv.yuexingan06.cn

Java: System.getenv("HOME")
来源：http://ca.newstarts.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://og.chemitech.net.cn

Ruby: ENV["HOME"]
来源：http://yh.szsharing.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://xd.shxzukj.cn

[M03] 执行外部命令
来源：http://xx.asd995.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hl.haigaiapp.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://fz.hnjuh.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://fz.muxihuayi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://wy.9csxet.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://tk.yuntaijiaju.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://un.haigaiapp.cn

Ruby: system("ls -l");  `ls -l`
来源：http://iy.shtwfgs.cn

C#:   Process.Start("ls", "-l");
来源：http://ji.muxihuayi.cn

[M04] 获取当前工作目录
来源：http://ax.nicolike.cn

Py:   os.getcwd()
来源：http://gl.huixiangedu.cn

PHP:  getcwd();
来源：http://qb.panjiajie.cn

JS:   process.cwd()
来源：http://nd.9csxet.cn

TS:   process.cwd()
来源：http://hi.bookmarksfly.cn

Java: Path.of("").toAbsolutePath()
来源：http://bw.szsharing.cn

Go:   os.Getwd()
来源：http://aa.huixiangedu.cn

Ruby: Dir.pwd
来源：http://qv.huanxung.cn

C#:   Directory.GetCurrentDirectory()
来源：http://xo.lnxyls.cn

[M05] 设置退出码
来源：http://cq.bookmarksfly.cn

Py:   sys.exit(1)
来源：http://pr.muxihuayi.cn

PHP:  exit(1);
来源：http://sb.shtwfgs.cn

JS:   process.exit(1)
来源：http://rz.asd995.cn

TS:   process.exit(1)
来源：http://rj.wgjwhj.cn

Java: System.exit(1)
来源：http://jq.newstarts.cn

Go:   os.Exit(1)
来源：http://qd.wgjwhj.cn

Ruby: exit 1
来源：http://np.huixiangedu.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://te.asd995.cn

[M06] 向标准错误输出
来源：http://fd.hahajie.cn

Py:   print("err", file=sys.stderr)
来源：http://oe.huixiangedu.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://qa.szxytkj.cn

JS:   console.error("err")
来源：http://dk.szsharing.cn

TS:   console.error("err")
来源：http://rd.jianghongdianzi.cn

Java: System.err.println("err")
来源：http://ce.panjiajie.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://bw.haigaiapp.cn

Ruby: warn "err"
来源：http://xn.huanxung.cn

C#:   Console.Error.WriteLine("err")
来源：http://fq.jctech888.com.cn

[M07] 判断是否为主入口
来源：http://pm.jctech888.com.cn

Py:   if __name__ == "__main__":
来源：http://kv.haigaiapp.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hj.shxzskj.cn

JS:   require.main === module
来源：http://qw.huixinmuqiang.cn

TS:   require.main === module
来源：http://gj.9csxet.cn

Java: public static void main(String[] args)
来源：http://yv.bjjhwx.cn

Go:   func main()
来源：http://em.jianghongdianzi.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://if.shxzskj.cn

C#:   static void Main(string[] args)
来源：http://vd.szsharing.cn

[M08] 获取系统与运行时信息
来源：http://fb.lnxyls.cn

Py:   platform.system();  platform.python_version()
来源：http://aa.9csxet.cn

PHP:  PHP_OS;  phpversion();
来源：http://or.nszjky.cn

JS:   process.platform;  process.version
来源：http://iw.hnjuh.cn

TS:   process.platform;  process.version
来源：http://wo.lnxyls.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://nm.panjiajie.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://fd.szxytkj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://pf.panjiajie.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://bm.nicolike.cn

================================================================================
来源：http://fh.shxzskj.cn

N. 数据结构与算法
来源：http://mv.szxytkj.cn

================================================================================
来源：http://vb.jianghongdianzi.cn

[N01] 二分查找（有序数组）
来源：http://di.jctech888.com.cn

Py:   bisect.bisect_left(arr, x)
来源：http://dq.newstarts.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ns.9csxet.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xv.newstarts.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://si.jctech888.com.cn

Java: Arrays.binarySearch(arr, x)
来源：http://bp.haigaiapp.cn

Go:   sort.SearchInts(arr, x)
来源：http://do.yuntaijiaju.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://sk.asd995.cn

C#:   Array.BinarySearch(arr, x)
来源：http://wa.yuexingan06.cn

[N02] 排序（工程实践用内置实现）
来源：http://mu.yuntaijiaju.cn

Py:   sorted(arr);  arr.sort()
来源：http://wa.szxytkj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://be.jianghongdianzi.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ef.shtwfgs.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://dc.hnjuh.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://pv.muxihuayi.cn

Go:   slices.Sort(arr)
来源：http://ww.shtwfgs.cn

Ruby: arr.sort
来源：http://sq.jianghongdianzi.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://la.yuexingan06.cn

[N03] 快速排序（分治示例）
来源：http://ug.bjjhwx.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://fp.nszjky.cn

PHP:  // 递归实现，或用 usort
来源：http://ts.yuntaijiaju.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lo.bjjhwx.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ht.521024.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://eo.wgjwhj.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://pr.huixinmuqiang.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://nw.haigaiapp.cn

C#:   // 手写递归，或 Array.Sort
来源：http://gx.muxihuayi.cn

[N04] 斐波那契数列
来源：http://cn.haigaiapp.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://yp.shtwfgs.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://iq.yuntaijiaju.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nf.haigaiapp.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pg.nicolike.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://zt.bjjhwx.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://cu.yuexingan06.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ip.hnjuh.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://xc.bjjhwx.cn

[N05] 最大公约数
来源：http://fw.yuntaijiaju.cn

Py:   math.gcd(a, b)
来源：http://rl.huanxung.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ji.9csxet.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ft.bjjhwx.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zc.521024.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://yk.panjiajie.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://qa.nszjky.cn

Ruby: a.gcd(b)
来源：http://oc.hahajie.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://vi.huixiangedu.cn

[N06] 判断回文字符串
来源：http://ja.haigaiapp.cn

Py:   s == s[::-1]
来源：http://gn.lnxyls.cn

PHP:  $s === strrev($s);
来源：http://oo.jianghongdianzi.cn

JS:   s === [...s].reverse().join("")
来源：http://ft.huixinmuqiang.cn

TS:   s === [...s].reverse().join("")
来源：http://nm.nicolike.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://kw.szxytkj.cn

Go:   // 双指针从两端比较
来源：http://em.shxzukj.cn

Ruby: s == s.reverse
来源：http://mb.huixiangedu.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ng.yuexingan06.cn

[N07] 两数之和（返回下标）
来源：http://zi.muxihuayi.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://kw.muxihuayi.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://rl.haigaiapp.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://mu.panjiajie.cn

TS:   // 手写 Map<string, number>
来源：http://wj.colortex.cn

Java: // 手写 HashMap
来源：http://ef.yuexingan06.cn

Go:   // 手写 map[int]int
来源：http://uo.nszjky.cn

Ruby: // 手写 Hash
来源：http://ed.jctech888.com.cn

C#:   // 手写 Dictionary<int, int>
来源：http://si.gzmigu.cn

[N08] 生成全排列
来源：http://fd.bjjhwx.cn

Py:   itertools.permutations(arr)
来源：http://jx.asd995.cn

PHP:  // 手写递归交换
来源：http://hc.yuexingan06.cn

JS:   // 手写回溯递归
来源：http://qr.muxihuayi.cn

TS:   // 手写回溯递归
来源：http://qw.huixinmuqiang.cn

Java: // 手写回溯递归
来源：http://zo.bjjhwx.cn

Go:   // 手写回溯递归
来源：http://mv.hnjuh.cn

Ruby: arr.permutation.to_a
来源：http://rl.jianghongdianzi.cn

C#:   // 手写回溯递归
来源：http://ml.shxzskj.cn

[N09] 栈与队列
来源：http://wy.muxihuayi.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://rw.huixiangedu.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mc.9csxet.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://yq.panjiajie.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://dw.huixiangedu.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://io.chemitech.net.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hy.shtwfgs.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://rf.521024.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://do.panjiajie.cn

[N10] 链表节点定义
来源：http://rh.bjjhwx.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://vj.521024.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ux.huixiangedu.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://uk.wgjwhj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://xj.nszjky.cn

Java: class Node { int v; Node next; }
来源：http://om.yuntaijiaju.cn

Go:   type Node struct { V int; Next *Node }
来源：http://du.jctech888.com.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ww.szxytkj.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://dl.nszjky.cn

[N11] 二叉树中序遍历
来源：http://xt.shxzskj.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://eo.jctech888.com.cn

PHP:  // 手写递归函数
来源：http://km.shxzukj.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xd.haigaiapp.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://eb.szxytkj.cn

Java: // 手写递归
来源：http://mv.chemitech.net.cn

Go:   // 手写递归
来源：http://jq.yuntaijiaju.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://em.shxzukj.cn

C#:   // 手写递归
来源：http://aa.szsharing.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ek.shtwfgs.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://jj.wgjwhj.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://al.newstarts.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cc.huixinmuqiang.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bt.szxytkj.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://pe.haigaiapp.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://bs.huanxung.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://vt.szsharing.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://zq.huanxung.cn

================================================================================
来源：http://ci.huixinmuqiang.cn

O. 并发与异步
来源：http://rj.jctech888.com.cn

================================================================================
来源：http://uw.haigaiapp.cn

[O01] 启动一个线程
来源：http://vl.bookmarksfly.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://zv.muxihuayi.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://eg.colortex.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wp.szxytkj.cn

TS:   // 同 JS
来源：http://tk.haigaiapp.cn

Java: new Thread(() -> f()).start()
来源：http://kr.shxzukj.cn

Go:   go f()
来源：http://vm.nszjky.cn

Ruby: Thread.new { f }
来源：http://hi.colortex.cn

C#:   Task.Run(() => F());
来源：http://we.bookmarksfly.cn

[O02] 使用线程池
来源：http://bc.521024.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://er.shxzukj.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://sm.huixinmuqiang.cn

JS:   // worker_threads 线程池
来源：http://rr.szsharing.cn

TS:   // worker_threads 线程池
来源：http://kz.muxihuayi.cn

Java: Executors.newFixedThreadPool(4)
来源：http://da.9csxet.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://xu.newstarts.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ce.newstarts.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://gu.szxytkj.cn

[O03] 加锁保护共享数据
来源：http://hc.hahajie.cn

Py:   with lock: shared += 1
来源：http://qf.yuntaijiaju.cn

PHP:  // 用 flock() 做文件锁
来源：http://eg.521024.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wz.yuntaijiaju.cn

TS:   // 同 JS
来源：http://xm.panjiajie.cn

Java: synchronized (this) { shared++; }
来源：http://xc.shxzskj.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://rk.521024.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://hx.haigaiapp.cn

C#:   lock (gate) { shared++; }
来源：http://ju.huixinmuqiang.cn

[O04] 定义异步函数并等待
来源：http://ln.szxytkj.cn

Py:   async def f():⏎    await g()
来源：http://tb.huixinmuqiang.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://lr.jctech888.com.cn

JS:   async function f() { await g(); }
来源：http://fw.bookmarksfly.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://bm.yuntaijiaju.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://sf.hnjuh.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://am.muxihuayi.cn

Ruby: # 用 Fiber 或 async gem
来源：http://lv.huanxung.cn

C#:   async Task F() { await G(); }
来源：http://ec.nszjky.cn

[O05] 并发执行并等待全部完成
来源：http://go.yuntaijiaju.cn

Py:   asyncio.gather(*tasks)
来源：http://sp.yuexingan06.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ch.wgjwhj.cn

JS:   await Promise.all(tasks)
来源：http://kh.9csxet.cn

TS:   await Promise.all(tasks)
来源：http://re.jctech888.com.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://tn.nicolike.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ey.panjiajie.cn

Ruby: threads.map(&:join)
来源：http://fe.hnjuh.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://dx.haigaiapp.cn

[O06] 使用进程池
来源：http://vf.haigaiapp.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ki.lnxyls.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://au.huixinmuqiang.cn

JS:   // child_process / cluster 模块
来源：http://uv.521024.cn

TS:   // child_process / cluster 模块
来源：http://dw.chemitech.net.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://oc.asd995.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://qp.newstarts.cn

Ruby: // fork 块
来源：http://vd.asd995.cn


<!-- 参考信息 -->