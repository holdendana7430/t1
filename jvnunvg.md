代发 wailian999

PHP:  serialize($obj);  unserialize($s);
来源：http://vd.jianghongdianzi.cn

JS:   v8.serialize(obj)        // Node
来源：http://td.huanxung.cn

TS:   v8.serialize(obj)        // Node
来源：http://eq.shtwfgs.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://pe.nszjky.cn

Go:   encoding/gob
来源：http://nm.colortex.cn

Ruby: Marshal.dump(obj)
来源：http://ev.shtwfgs.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://yj.muxihuayi.cn

================================================================================
来源：http://ka.panjiajie.cn

L. 网络请求
来源：http://zx.chemitech.net.cn

================================================================================
来源：http://km.chemitech.net.cn

[L01] 发送 GET 请求
来源：http://cx.jianghongdianzi.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://cg.panjiajie.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://pr.hahajie.cn

JS:   await fetch(url)
来源：http://ch.colortex.cn

TS:   await fetch(url)
来源：http://ww.szsharing.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ou.shxzskj.cn

Go:   resp, err := http.Get(url)
来源：http://oh.gzmigu.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://gq.muxihuayi.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ic.bookmarksfly.cn

[L02] 发送 POST JSON
来源：http://uk.yuexingan06.cn

Py:   requests.post(url, json={"a": 1})
来源：http://aw.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://km.muxihuayi.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cz.newstarts.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cn.asd995.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://fe.shxzukj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://he.lnxyls.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://sx.huixiangedu.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://jh.hnjuh.cn

[L03] 设置自定义请求头
来源：http://ug.yuntaijiaju.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://gn.521024.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mf.shxzskj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cc.bookmarksfly.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://io.shxzskj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wk.bookmarksfly.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hq.wgjwhj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://dq.huanxung.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://xg.yuexingan06.cn

[L04] 设置超时
来源：http://be.yuntaijiaju.cn

Py:   requests.get(url, timeout=5)
来源：http://tp.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wt.hnjuh.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pq.yuntaijiaju.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nz.wgjwhj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ia.bookmarksfly.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xl.gzmigu.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://dj.szxytkj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://kj.shxzukj.cn

[L05] 上传文件（multipart）
来源：http://zo.huixiangedu.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zk.haigaiapp.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://px.hahajie.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ye.szsharing.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hf.shxzskj.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vo.szsharing.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://kv.hahajie.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://rf.hnjuh.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://se.shxzskj.cn

[L06] 解析响应为 JSON
来源：http://pg.huixiangedu.cn

Py:   resp.json()
来源：http://ck.lnxyls.cn

PHP:  json_decode($body, true);
来源：http://ru.bjjhwx.cn

JS:   await resp.json()
来源：http://be.bookmarksfly.cn

TS:   await resp.json()
来源：http://ry.szsharing.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://qn.hahajie.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://tz.yuntaijiaju.cn

Ruby: JSON.parse(resp.body)
来源：http://jf.huanxung.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://iz.szxytkj.cn

[L07] 处理 HTTP 状态码
来源：http://bs.huixinmuqiang.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://cy.newstarts.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hk.yuntaijiaju.cn

JS:   resp.ok;  resp.status
来源：http://xw.shtwfgs.cn

TS:   resp.ok;  resp.status
来源：http://yw.wgjwhj.cn

Java: resp.statusCode()
来源：http://xt.newstarts.cn

Go:   resp.StatusCode
来源：http://rr.asd995.cn

Ruby: resp.code.to_i
来源：http://wp.bookmarksfly.cn

C#:   (int)resp.StatusCode
来源：http://gq.bjjhwx.cn

[L08] 并发请求多个地址
来源：http://tp.lnxyls.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ql.hnjuh.cn

PHP:  curl_multi_init() 系列
来源：http://nz.panjiajie.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nj.shxzukj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vy.newstarts.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://rg.bookmarksfly.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://eh.bjjhwx.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zj.gzmigu.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://jl.asd995.cn

================================================================================
来源：http://wh.colortex.cn

M. 命令行 / 进程 / 环境
来源：http://ej.hahajie.cn

================================================================================
来源：http://ss.hnjuh.cn

[M01] 读取命令行参数
来源：http://pj.bookmarksfly.cn

Py:   sys.argv[1:]
来源：http://yk.521024.cn

PHP:  $argv;  $argc;
来源：http://eu.jctech888.com.cn

JS:   process.argv.slice(2)
来源：http://tg.gzmigu.cn

TS:   process.argv.slice(2)
来源：http://tx.bjjhwx.cn

Java: args 数组（main 方法参数）
来源：http://ak.shxzskj.cn

Go:   os.Args[1:]
来源：http://jb.huixinmuqiang.cn

Ruby: ARGV
来源：http://rw.newstarts.cn

C#:   args 数组（Main 方法参数）
来源：http://pb.asd995.cn

[M02] 读取环境变量
来源：http://pi.jianghongdianzi.cn

Py:   os.environ.get("HOME")
来源：http://sk.asd995.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://dp.521024.cn

JS:   process.env.HOME
来源：http://zr.521024.cn

TS:   process.env.HOME
来源：http://fk.9csxet.cn

Java: System.getenv("HOME")
来源：http://lx.nszjky.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://np.panjiajie.cn

Ruby: ENV["HOME"]
来源：http://kc.bookmarksfly.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://az.9csxet.cn

[M03] 执行外部命令
来源：http://fn.yuntaijiaju.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://jv.jianghongdianzi.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ip.nicolike.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ld.muxihuayi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://oj.newstarts.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hr.huixiangedu.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://bo.bookmarksfly.cn

Ruby: system("ls -l");  `ls -l`
来源：http://od.nszjky.cn

C#:   Process.Start("ls", "-l");
来源：http://kg.huixiangedu.cn

[M04] 获取当前工作目录
来源：http://by.asd995.cn

Py:   os.getcwd()
来源：http://yj.huixiangedu.cn

PHP:  getcwd();
来源：http://ed.wgjwhj.cn

JS:   process.cwd()
来源：http://bk.yuntaijiaju.cn

TS:   process.cwd()
来源：http://ng.hnjuh.cn

Java: Path.of("").toAbsolutePath()
来源：http://tp.shtwfgs.cn

Go:   os.Getwd()
来源：http://wj.gzmigu.cn

Ruby: Dir.pwd
来源：http://mv.yuntaijiaju.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ex.szsharing.cn

[M05] 设置退出码
来源：http://cn.521024.cn

Py:   sys.exit(1)
来源：http://cl.colortex.cn

PHP:  exit(1);
来源：http://po.huanxung.cn

JS:   process.exit(1)
来源：http://fi.jianghongdianzi.cn

TS:   process.exit(1)
来源：http://ja.shxzukj.cn

Java: System.exit(1)
来源：http://dv.colortex.cn

Go:   os.Exit(1)
来源：http://pf.shtwfgs.cn

Ruby: exit 1
来源：http://ww.hahajie.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://vc.yuntaijiaju.cn

[M06] 向标准错误输出
来源：http://xy.szxytkj.cn

Py:   print("err", file=sys.stderr)
来源：http://vr.szxytkj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://av.shxzukj.cn

JS:   console.error("err")
来源：http://gd.huanxung.cn

TS:   console.error("err")
来源：http://tx.yuexingan06.cn

Java: System.err.println("err")
来源：http://mg.bookmarksfly.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ym.wgjwhj.cn

Ruby: warn "err"
来源：http://vr.colortex.cn

C#:   Console.Error.WriteLine("err")
来源：http://wa.newstarts.cn

[M07] 判断是否为主入口
来源：http://bb.hahajie.cn

Py:   if __name__ == "__main__":
来源：http://lh.hahajie.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://bn.yuntaijiaju.cn

JS:   require.main === module
来源：http://mc.jianghongdianzi.cn

TS:   require.main === module
来源：http://ao.newstarts.cn

Java: public static void main(String[] args)
来源：http://ot.haigaiapp.cn

Go:   func main()
来源：http://rs.haigaiapp.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://in.jianghongdianzi.cn

C#:   static void Main(string[] args)
来源：http://ts.huanxung.cn

[M08] 获取系统与运行时信息
来源：http://hw.colortex.cn

Py:   platform.system();  platform.python_version()
来源：http://iz.jctech888.com.cn

PHP:  PHP_OS;  phpversion();
来源：http://gn.muxihuayi.cn

JS:   process.platform;  process.version
来源：http://tx.jianghongdianzi.cn

TS:   process.platform;  process.version
来源：http://kl.wgjwhj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://cu.bookmarksfly.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://oh.hnjuh.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://it.huanxung.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://np.yuexingan06.cn

================================================================================
来源：http://qt.chemitech.net.cn

N. 数据结构与算法
来源：http://di.szxytkj.cn

================================================================================
来源：http://ej.yuexingan06.cn

[N01] 二分查找（有序数组）
来源：http://ee.colortex.cn

Py:   bisect.bisect_left(arr, x)
来源：http://df.hahajie.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://oz.muxihuayi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fe.szsharing.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pr.hnjuh.cn

Java: Arrays.binarySearch(arr, x)
来源：http://gj.asd995.cn

Go:   sort.SearchInts(arr, x)
来源：http://ui.jianghongdianzi.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://bl.jianghongdianzi.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ar.huixinmuqiang.cn

[N02] 排序（工程实践用内置实现）
来源：http://di.yuexingan06.cn

Py:   sorted(arr);  arr.sort()
来源：http://te.asd995.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://kk.nszjky.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://qi.bjjhwx.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://nk.lnxyls.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://jm.shxzukj.cn

Go:   slices.Sort(arr)
来源：http://fo.shxzskj.cn

Ruby: arr.sort
来源：http://cf.gzmigu.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://qz.jctech888.com.cn

[N03] 快速排序（分治示例）
来源：http://cd.huixiangedu.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wj.shxzukj.cn

PHP:  // 递归实现，或用 usort
来源：http://ia.jianghongdianzi.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://px.huixinmuqiang.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xz.nicolike.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://bp.gzmigu.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://xv.9csxet.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://pm.gzmigu.cn

C#:   // 手写递归，或 Array.Sort
来源：http://nk.yuntaijiaju.cn

[N04] 斐波那契数列
来源：http://dn.gzmigu.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://dz.yuexingan06.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://bp.colortex.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cd.yuexingan06.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ba.jctech888.com.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://vp.hahajie.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://vz.bjjhwx.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://xk.wgjwhj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://bo.jianghongdianzi.cn

[N05] 最大公约数
来源：http://bo.jianghongdianzi.cn

Py:   math.gcd(a, b)
来源：http://vy.nszjky.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://bh.newstarts.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wp.yuexingan06.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ol.shxzukj.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://op.huanxung.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://jm.colortex.cn

Ruby: a.gcd(b)
来源：http://gf.szxytkj.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ss.huixiangedu.cn

[N06] 判断回文字符串
来源：http://wp.bjjhwx.cn

Py:   s == s[::-1]
来源：http://ec.9csxet.cn

PHP:  $s === strrev($s);
来源：http://kf.jctech888.com.cn

JS:   s === [...s].reverse().join("")
来源：http://uz.huixiangedu.cn

TS:   s === [...s].reverse().join("")
来源：http://gj.yuntaijiaju.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ho.wgjwhj.cn

Go:   // 双指针从两端比较
来源：http://rn.9csxet.cn

Ruby: s == s.reverse
来源：http://qp.nicolike.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://el.muxihuayi.cn

[N07] 两数之和（返回下标）
来源：http://wt.colortex.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://iv.shxzskj.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ac.yuexingan06.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://cb.panjiajie.cn

TS:   // 手写 Map<string, number>
来源：http://sp.wgjwhj.cn

Java: // 手写 HashMap
来源：http://oc.haigaiapp.cn

Go:   // 手写 map[int]int
来源：http://il.szsharing.cn

Ruby: // 手写 Hash
来源：http://wc.521024.cn

C#:   // 手写 Dictionary<int, int>
来源：http://tt.nicolike.cn

[N08] 生成全排列
来源：http://np.huixinmuqiang.cn

Py:   itertools.permutations(arr)
来源：http://du.nszjky.cn

PHP:  // 手写递归交换
来源：http://tk.wgjwhj.cn

JS:   // 手写回溯递归
来源：http://wf.hahajie.cn

TS:   // 手写回溯递归
来源：http://ti.yuntaijiaju.cn

Java: // 手写回溯递归
来源：http://tv.wgjwhj.cn

Go:   // 手写回溯递归
来源：http://bp.huixinmuqiang.cn

Ruby: arr.permutation.to_a
来源：http://ih.szsharing.cn

C#:   // 手写回溯递归
来源：http://yb.szxytkj.cn

[N09] 栈与队列
来源：http://mn.yuexingan06.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ml.haigaiapp.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://pz.huixinmuqiang.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://vk.jctech888.com.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ir.yuexingan06.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://je.colortex.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ej.haigaiapp.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://au.hnjuh.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://vt.jctech888.com.cn

[N10] 链表节点定义
来源：http://um.haigaiapp.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hm.yuexingan06.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://jg.shxzukj.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://dp.szsharing.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://gj.asd995.cn

Java: class Node { int v; Node next; }
来源：http://cz.lnxyls.cn

Go:   type Node struct { V int; Next *Node }
来源：http://jk.jctech888.com.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://in.haigaiapp.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://fj.muxihuayi.cn

[N11] 二叉树中序遍历
来源：http://zv.9csxet.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://xx.muxihuayi.cn

PHP:  // 手写递归函数
来源：http://qo.gzmigu.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://in.newstarts.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nm.hahajie.cn

Java: // 手写递归
来源：http://vp.nszjky.cn

Go:   // 手写递归
来源：http://br.yuexingan06.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ry.bookmarksfly.cn

C#:   // 手写递归
来源：http://ma.huixinmuqiang.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ab.wgjwhj.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://es.huixinmuqiang.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://yc.shxzukj.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ge.muxihuayi.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vg.szxytkj.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://gu.chemitech.net.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://iy.szsharing.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://xi.nszjky.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://jc.lnxyls.cn

================================================================================
来源：http://fk.haigaiapp.cn

O. 并发与异步
来源：http://ma.yuntaijiaju.cn

================================================================================
来源：http://oy.huixinmuqiang.cn

[O01] 启动一个线程
来源：http://uo.521024.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://cr.jianghongdianzi.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://zc.muxihuayi.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ud.lnxyls.cn

TS:   // 同 JS
来源：http://jh.521024.cn

Java: new Thread(() -> f()).start()
来源：http://zq.huixinmuqiang.cn

Go:   go f()
来源：http://fd.asd995.cn

Ruby: Thread.new { f }
来源：http://vh.nicolike.cn

C#:   Task.Run(() => F());
来源：http://hp.panjiajie.cn

[O02] 使用线程池
来源：http://mt.yuexingan06.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://nb.hahajie.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wg.jianghongdianzi.cn

JS:   // worker_threads 线程池
来源：http://lg.huixiangedu.cn

TS:   // worker_threads 线程池
来源：http://fo.nicolike.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ln.shtwfgs.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://it.huixinmuqiang.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://pj.colortex.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://qm.nszjky.cn

[O03] 加锁保护共享数据
来源：http://vn.shxzskj.cn

Py:   with lock: shared += 1
来源：http://ql.panjiajie.cn

PHP:  // 用 flock() 做文件锁
来源：http://yy.wgjwhj.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://nj.szxytkj.cn

TS:   // 同 JS
来源：http://da.bjjhwx.cn

Java: synchronized (this) { shared++; }
来源：http://ao.lnxyls.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://um.bjjhwx.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://lm.lnxyls.cn

C#:   lock (gate) { shared++; }
来源：http://sg.szsharing.cn

[O04] 定义异步函数并等待
来源：http://xy.jctech888.com.cn

Py:   async def f():⏎    await g()
来源：http://fq.gzmigu.cn


<!-- 参考信息 -->