代发 wailian999

Py:   requests.post(url, json={"a": 1})
来源：http://zm.yuntaijiaju.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://bk.521024.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zb.szsharing.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fv.yuexingan06.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://cz.huixiangedu.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://dk.bookmarksfly.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xk.yuntaijiaju.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://rz.chemitech.net.cn

[L03] 设置自定义请求头
来源：http://el.yuexingan06.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://kv.szxytkj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://vd.hnjuh.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://by.asd995.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kf.wgjwhj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://zd.jctech888.com.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ti.chemitech.net.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wn.szsharing.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://fv.shxzukj.cn

[L04] 设置超时
来源：http://xf.yuexingan06.cn

Py:   requests.get(url, timeout=5)
来源：http://hb.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://st.shtwfgs.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nu.huanxung.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cu.521024.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://rp.jctech888.com.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://dq.wgjwhj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://kr.szxytkj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://vs.chemitech.net.cn

[L05] 上传文件（multipart）
来源：http://hc.gzmigu.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ag.nicolike.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://gs.nicolike.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://vl.panjiajie.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://kr.jianghongdianzi.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://oo.yuexingan06.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://pz.shtwfgs.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://cz.newstarts.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://sb.panjiajie.cn

[L06] 解析响应为 JSON
来源：http://vv.yuntaijiaju.cn

Py:   resp.json()
来源：http://ld.chemitech.net.cn

PHP:  json_decode($body, true);
来源：http://yj.lnxyls.cn

JS:   await resp.json()
来源：http://wz.jianghongdianzi.cn

TS:   await resp.json()
来源：http://ac.lnxyls.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ec.shxzskj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ts.colortex.cn

Ruby: JSON.parse(resp.body)
来源：http://ys.yuntaijiaju.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ea.nszjky.cn

[L07] 处理 HTTP 状态码
来源：http://jy.nszjky.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ff.hahajie.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://nx.shxzskj.cn

JS:   resp.ok;  resp.status
来源：http://fh.muxihuayi.cn

TS:   resp.ok;  resp.status
来源：http://qw.colortex.cn

Java: resp.statusCode()
来源：http://io.bookmarksfly.cn

Go:   resp.StatusCode
来源：http://sz.szsharing.cn

Ruby: resp.code.to_i
来源：http://qb.huanxung.cn

C#:   (int)resp.StatusCode
来源：http://oh.nszjky.cn

[L08] 并发请求多个地址
来源：http://or.hahajie.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://oa.haigaiapp.cn

PHP:  curl_multi_init() 系列
来源：http://ki.chemitech.net.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ln.gzmigu.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sp.wgjwhj.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ny.521024.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://jx.yuexingan06.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zn.colortex.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://uv.huixinmuqiang.cn

================================================================================
来源：http://ly.huixinmuqiang.cn

M. 命令行 / 进程 / 环境
来源：http://hv.muxihuayi.cn

================================================================================
来源：http://lm.muxihuayi.cn

[M01] 读取命令行参数
来源：http://fr.panjiajie.cn

Py:   sys.argv[1:]
来源：http://dh.szsharing.cn

PHP:  $argv;  $argc;
来源：http://yu.wgjwhj.cn

JS:   process.argv.slice(2)
来源：http://qz.nszjky.cn

TS:   process.argv.slice(2)
来源：http://bs.jctech888.com.cn

Java: args 数组（main 方法参数）
来源：http://qr.huanxung.cn

Go:   os.Args[1:]
来源：http://rw.521024.cn

Ruby: ARGV
来源：http://qz.huixiangedu.cn

C#:   args 数组（Main 方法参数）
来源：http://ct.haigaiapp.cn

[M02] 读取环境变量
来源：http://nh.huanxung.cn

Py:   os.environ.get("HOME")
来源：http://jf.muxihuayi.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ae.yuntaijiaju.cn

JS:   process.env.HOME
来源：http://wb.jianghongdianzi.cn

TS:   process.env.HOME
来源：http://dt.hahajie.cn

Java: System.getenv("HOME")
来源：http://iy.chemitech.net.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wt.huanxung.cn

Ruby: ENV["HOME"]
来源：http://fw.yuntaijiaju.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://uk.jctech888.com.cn

[M03] 执行外部命令
来源：http://ng.wgjwhj.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://tt.szxytkj.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ev.shxzskj.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://qc.huanxung.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://gw.huixiangedu.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://lw.szxytkj.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://xu.521024.cn

Ruby: system("ls -l");  `ls -l`
来源：http://de.wgjwhj.cn

C#:   Process.Start("ls", "-l");
来源：http://dg.panjiajie.cn

[M04] 获取当前工作目录
来源：http://gt.chemitech.net.cn

Py:   os.getcwd()
来源：http://fg.asd995.cn

PHP:  getcwd();
来源：http://wp.jctech888.com.cn

JS:   process.cwd()
来源：http://le.shxzskj.cn

TS:   process.cwd()
来源：http://kz.gzmigu.cn

Java: Path.of("").toAbsolutePath()
来源：http://yl.haigaiapp.cn

Go:   os.Getwd()
来源：http://nh.chemitech.net.cn

Ruby: Dir.pwd
来源：http://mg.521024.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ex.haigaiapp.cn

[M05] 设置退出码
来源：http://gj.nszjky.cn

Py:   sys.exit(1)
来源：http://yj.wgjwhj.cn

PHP:  exit(1);
来源：http://po.wgjwhj.cn

JS:   process.exit(1)
来源：http://pr.haigaiapp.cn

TS:   process.exit(1)
来源：http://lx.huixiangedu.cn

Java: System.exit(1)
来源：http://ys.nicolike.cn

Go:   os.Exit(1)
来源：http://ge.yuntaijiaju.cn

Ruby: exit 1
来源：http://yd.yuntaijiaju.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://zo.huixiangedu.cn

[M06] 向标准错误输出
来源：http://ks.colortex.cn

Py:   print("err", file=sys.stderr)
来源：http://ii.nszjky.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://cs.yuntaijiaju.cn

JS:   console.error("err")
来源：http://lq.yuntaijiaju.cn

TS:   console.error("err")
来源：http://ar.chemitech.net.cn

Java: System.err.println("err")
来源：http://im.bjjhwx.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ex.asd995.cn

Ruby: warn "err"
来源：http://ku.wgjwhj.cn

C#:   Console.Error.WriteLine("err")
来源：http://em.gzmigu.cn

[M07] 判断是否为主入口
来源：http://nw.bjjhwx.cn

Py:   if __name__ == "__main__":
来源：http://uf.bjjhwx.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://qs.shxzukj.cn

JS:   require.main === module
来源：http://qb.haigaiapp.cn

TS:   require.main === module
来源：http://du.muxihuayi.cn

Java: public static void main(String[] args)
来源：http://hp.huixiangedu.cn

Go:   func main()
来源：http://uo.shxzskj.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://cd.szsharing.cn

C#:   static void Main(string[] args)
来源：http://bo.muxihuayi.cn

[M08] 获取系统与运行时信息
来源：http://wb.bjjhwx.cn

Py:   platform.system();  platform.python_version()
来源：http://gj.panjiajie.cn

PHP:  PHP_OS;  phpversion();
来源：http://wf.szsharing.cn

JS:   process.platform;  process.version
来源：http://qe.nszjky.cn

TS:   process.platform;  process.version
来源：http://qj.haigaiapp.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://nu.huixinmuqiang.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://bd.wgjwhj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://oa.shtwfgs.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://nc.yuntaijiaju.cn

================================================================================
来源：http://yt.jianghongdianzi.cn

N. 数据结构与算法
来源：http://nv.haigaiapp.cn

================================================================================
来源：http://eq.nszjky.cn

[N01] 二分查找（有序数组）
来源：http://yu.bjjhwx.cn

Py:   bisect.bisect_left(arr, x)
来源：http://va.521024.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://js.9csxet.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cx.yuexingan06.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cr.huixinmuqiang.cn

Java: Arrays.binarySearch(arr, x)
来源：http://sj.wgjwhj.cn

Go:   sort.SearchInts(arr, x)
来源：http://kf.hnjuh.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ho.jctech888.com.cn

C#:   Array.BinarySearch(arr, x)
来源：http://sm.521024.cn

[N02] 排序（工程实践用内置实现）
来源：http://ub.newstarts.cn

Py:   sorted(arr);  arr.sort()
来源：http://fw.colortex.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://xw.nszjky.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://kg.hahajie.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://cm.haigaiapp.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://yq.szsharing.cn

Go:   slices.Sort(arr)
来源：http://tw.shtwfgs.cn

Ruby: arr.sort
来源：http://aa.bookmarksfly.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://qq.hahajie.cn

[N03] 快速排序（分治示例）
来源：http://ns.shtwfgs.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://lh.jctech888.com.cn

PHP:  // 递归实现，或用 usort
来源：http://ch.huixinmuqiang.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ag.shxzskj.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fg.nszjky.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://je.9csxet.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://bi.huixiangedu.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://gy.nicolike.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ux.gzmigu.cn

[N04] 斐波那契数列
来源：http://xv.muxihuayi.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ig.szsharing.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://by.nicolike.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ma.shxzukj.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bk.shxzukj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://aa.panjiajie.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://zj.huanxung.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://kc.yuexingan06.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ei.huixinmuqiang.cn

[N05] 最大公约数
来源：http://hm.wgjwhj.cn

Py:   math.gcd(a, b)
来源：http://rh.lnxyls.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://es.gzmigu.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vj.nszjky.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ul.gzmigu.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://pp.asd995.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ve.nicolike.cn

Ruby: a.gcd(b)
来源：http://ry.panjiajie.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://jt.yuexingan06.cn

[N06] 判断回文字符串
来源：http://gf.lnxyls.cn

Py:   s == s[::-1]
来源：http://pg.szsharing.cn

PHP:  $s === strrev($s);
来源：http://et.nszjky.cn

JS:   s === [...s].reverse().join("")
来源：http://uj.521024.cn

TS:   s === [...s].reverse().join("")
来源：http://fo.bookmarksfly.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://yy.jctech888.com.cn

Go:   // 双指针从两端比较
来源：http://kh.shxzukj.cn

Ruby: s == s.reverse
来源：http://oe.szxytkj.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ol.yuntaijiaju.cn

[N07] 两数之和（返回下标）
来源：http://nc.shtwfgs.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://tw.yuntaijiaju.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jw.hahajie.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ea.jctech888.com.cn

TS:   // 手写 Map<string, number>
来源：http://lp.yuntaijiaju.cn

Java: // 手写 HashMap
来源：http://vf.szxytkj.cn

Go:   // 手写 map[int]int
来源：http://th.9csxet.cn

Ruby: // 手写 Hash
来源：http://mz.huanxung.cn

C#:   // 手写 Dictionary<int, int>
来源：http://sr.lnxyls.cn

[N08] 生成全排列
来源：http://lm.huanxung.cn

Py:   itertools.permutations(arr)
来源：http://jg.shtwfgs.cn

PHP:  // 手写递归交换
来源：http://hk.chemitech.net.cn

JS:   // 手写回溯递归
来源：http://wr.szsharing.cn

TS:   // 手写回溯递归
来源：http://ly.huanxung.cn

Java: // 手写回溯递归
来源：http://gr.yuexingan06.cn

Go:   // 手写回溯递归
来源：http://ye.nicolike.cn

Ruby: arr.permutation.to_a
来源：http://ys.bookmarksfly.cn

C#:   // 手写回溯递归
来源：http://lq.shxzskj.cn

[N09] 栈与队列
来源：http://jq.gzmigu.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://la.huixiangedu.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ps.jianghongdianzi.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://by.szsharing.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://at.asd995.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ym.newstarts.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://vo.9csxet.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ol.huixiangedu.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://pd.muxihuayi.cn

[N10] 链表节点定义
来源：http://ef.gzmigu.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://od.lnxyls.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://cd.huixinmuqiang.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://vl.szsharing.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wq.huixiangedu.cn

Java: class Node { int v; Node next; }
来源：http://xs.bjjhwx.cn

Go:   type Node struct { V int; Next *Node }
来源：http://eo.panjiajie.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://xm.shxzskj.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://wk.chemitech.net.cn

[N11] 二叉树中序遍历
来源：http://lm.colortex.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://sv.521024.cn

PHP:  // 手写递归函数
来源：http://qb.9csxet.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zn.colortex.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://oi.huixiangedu.cn

Java: // 手写递归
来源：http://zb.szsharing.cn

Go:   // 手写递归
来源：http://uc.hahajie.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://rc.wgjwhj.cn

C#:   // 手写递归
来源：http://xb.yuntaijiaju.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://vv.yuntaijiaju.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://yl.lnxyls.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://od.bookmarksfly.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yx.asd995.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qd.nszjky.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://le.huixinmuqiang.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://rg.9csxet.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ww.huixinmuqiang.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://me.haigaiapp.cn

================================================================================
来源：http://jp.lnxyls.cn

O. 并发与异步
来源：http://yt.newstarts.cn

================================================================================
来源：http://sx.yuntaijiaju.cn

[O01] 启动一个线程
来源：http://gq.lnxyls.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://oo.hahajie.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://zt.shxzukj.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://qh.haigaiapp.cn

TS:   // 同 JS
来源：http://pd.szxytkj.cn

Java: new Thread(() -> f()).start()
来源：http://gc.panjiajie.cn

Go:   go f()
来源：http://qq.gzmigu.cn

Ruby: Thread.new { f }
来源：http://ou.panjiajie.cn

C#:   Task.Run(() => F());
来源：http://by.lnxyls.cn

[O02] 使用线程池
来源：http://px.bookmarksfly.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://iz.hnjuh.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://cd.szxytkj.cn

JS:   // worker_threads 线程池
来源：http://eq.huixiangedu.cn

TS:   // worker_threads 线程池
来源：http://cm.jctech888.com.cn

Java: Executors.newFixedThreadPool(4)
来源：http://db.huixiangedu.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://so.szxytkj.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://sv.yuntaijiaju.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mg.szxytkj.cn

[O03] 加锁保护共享数据
来源：http://io.hnjuh.cn

Py:   with lock: shared += 1
来源：http://hq.hahajie.cn

PHP:  // 用 flock() 做文件锁
来源：http://gu.nicolike.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ff.bookmarksfly.cn

TS:   // 同 JS
来源：http://aw.colortex.cn

Java: synchronized (this) { shared++; }
来源：http://xu.szxytkj.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://az.wgjwhj.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://zo.nicolike.cn

C#:   lock (gate) { shared++; }
来源：http://rj.gzmigu.cn

[O04] 定义异步函数并等待
来源：http://hk.hnjuh.cn

Py:   async def f():⏎    await g()
来源：http://sy.newstarts.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://vb.bookmarksfly.cn

JS:   async function f() { await g(); }
来源：http://mh.nicolike.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://lo.521024.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://zm.jianghongdianzi.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://qo.9csxet.cn

Ruby: # 用 Fiber 或 async gem
来源：http://am.nicolike.cn

C#:   async Task F() { await G(); }
来源：http://aj.huanxung.cn

[O05] 并发执行并等待全部完成
来源：http://hb.9csxet.cn

Py:   asyncio.gather(*tasks)
来源：http://hd.newstarts.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://za.jctech888.com.cn

JS:   await Promise.all(tasks)
来源：http://cv.hahajie.cn

TS:   await Promise.all(tasks)
来源：http://fw.wgjwhj.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hy.nszjky.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://kr.haigaiapp.cn

Ruby: threads.map(&:join)
来源：http://us.haigaiapp.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://uj.shxzskj.cn

[O06] 使用进程池
来源：http://cc.haigaiapp.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://iy.huixiangedu.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://go.bookmarksfly.cn

JS:   // child_process / cluster 模块
来源：http://ko.gzmigu.cn


<!-- 参考信息 -->