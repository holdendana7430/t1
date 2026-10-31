代发 wailian999

PHP:  serialize($obj);  unserialize($s);
来源：http://da.jianghongdianzi.cn

JS:   v8.serialize(obj)        // Node
来源：http://ej.shtwfgs.cn

TS:   v8.serialize(obj)        // Node
来源：http://wq.yuntaijiaju.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://gf.szxytkj.cn

Go:   encoding/gob
来源：http://hw.muxihuayi.cn

Ruby: Marshal.dump(obj)
来源：http://ll.hnjuh.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://gb.9csxet.cn

================================================================================
来源：http://vs.muxihuayi.cn

L. 网络请求
来源：http://zz.shtwfgs.cn

================================================================================
来源：http://ff.gzmigu.cn

[L01] 发送 GET 请求
来源：http://pa.huixinmuqiang.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ys.huixinmuqiang.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xd.jctech888.com.cn

JS:   await fetch(url)
来源：http://ph.muxihuayi.cn

TS:   await fetch(url)
来源：http://fc.shxzskj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://fc.huanxung.cn

Go:   resp, err := http.Get(url)
来源：http://xg.chemitech.net.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://jy.huixinmuqiang.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://le.yuntaijiaju.cn

[L02] 发送 POST JSON
来源：http://ba.haigaiapp.cn

Py:   requests.post(url, json={"a": 1})
来源：http://wy.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://oq.hahajie.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://na.jctech888.com.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kq.521024.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://no.huanxung.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://sr.bjjhwx.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xk.jianghongdianzi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ma.lnxyls.cn

[L03] 设置自定义请求头
来源：http://fc.szxytkj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://xs.nszjky.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://tr.hnjuh.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dp.bookmarksfly.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qd.nicolike.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ex.9csxet.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://pv.gzmigu.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://xj.jctech888.com.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://tm.wgjwhj.cn

[L04] 设置超时
来源：http://qk.muxihuayi.cn

Py:   requests.get(url, timeout=5)
来源：http://pu.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://jf.haigaiapp.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nj.hnjuh.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ac.huixinmuqiang.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://bi.shtwfgs.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wf.haigaiapp.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://lt.huixinmuqiang.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ek.nszjky.cn

[L05] 上传文件（multipart）
来源：http://fn.bjjhwx.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://iy.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://uv.lnxyls.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ks.yuntaijiaju.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ew.yuntaijiaju.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://in.hahajie.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://tv.shtwfgs.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://bb.colortex.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ty.szsharing.cn

[L06] 解析响应为 JSON
来源：http://ks.lnxyls.cn

Py:   resp.json()
来源：http://wx.gzmigu.cn

PHP:  json_decode($body, true);
来源：http://wt.colortex.cn

JS:   await resp.json()
来源：http://vo.jctech888.com.cn

TS:   await resp.json()
来源：http://zn.szxytkj.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://pl.hnjuh.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://rr.newstarts.cn

Ruby: JSON.parse(resp.body)
来源：http://vr.wgjwhj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://vs.huanxung.cn

[L07] 处理 HTTP 状态码
来源：http://dk.lnxyls.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://jw.bjjhwx.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://fa.hahajie.cn

JS:   resp.ok;  resp.status
来源：http://oo.nicolike.cn

TS:   resp.ok;  resp.status
来源：http://tn.521024.cn

Java: resp.statusCode()
来源：http://kx.yuexingan06.cn

Go:   resp.StatusCode
来源：http://rw.shtwfgs.cn

Ruby: resp.code.to_i
来源：http://we.hahajie.cn

C#:   (int)resp.StatusCode
来源：http://gn.shxzukj.cn

[L08] 并发请求多个地址
来源：http://vr.haigaiapp.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://zc.szxytkj.cn

PHP:  curl_multi_init() 系列
来源：http://ui.nszjky.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yc.jctech888.com.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ge.bookmarksfly.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ex.gzmigu.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ks.shxzskj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ea.nszjky.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://fq.shtwfgs.cn

================================================================================
来源：http://wn.huixinmuqiang.cn

M. 命令行 / 进程 / 环境
来源：http://mb.bookmarksfly.cn

================================================================================
来源：http://iz.shxzukj.cn

[M01] 读取命令行参数
来源：http://zx.szxytkj.cn

Py:   sys.argv[1:]
来源：http://tr.bookmarksfly.cn

PHP:  $argv;  $argc;
来源：http://lm.hnjuh.cn

JS:   process.argv.slice(2)
来源：http://pq.yuntaijiaju.cn

TS:   process.argv.slice(2)
来源：http://uj.huixinmuqiang.cn

Java: args 数组（main 方法参数）
来源：http://xb.gzmigu.cn

Go:   os.Args[1:]
来源：http://od.asd995.cn

Ruby: ARGV
来源：http://ag.hnjuh.cn

C#:   args 数组（Main 方法参数）
来源：http://fv.jianghongdianzi.cn

[M02] 读取环境变量
来源：http://is.chemitech.net.cn

Py:   os.environ.get("HOME")
来源：http://yd.huixinmuqiang.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rg.asd995.cn

JS:   process.env.HOME
来源：http://xj.colortex.cn

TS:   process.env.HOME
来源：http://sf.colortex.cn

Java: System.getenv("HOME")
来源：http://un.nicolike.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://eb.huixinmuqiang.cn

Ruby: ENV["HOME"]
来源：http://xm.yuexingan06.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mu.huixiangedu.cn

[M03] 执行外部命令
来源：http://db.hahajie.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://et.huixinmuqiang.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ik.shxzskj.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://yj.jctech888.com.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ce.jctech888.com.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://uk.lnxyls.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://fo.szsharing.cn

Ruby: system("ls -l");  `ls -l`
来源：http://dy.shxzukj.cn

C#:   Process.Start("ls", "-l");
来源：http://gv.newstarts.cn

[M04] 获取当前工作目录
来源：http://yt.huixiangedu.cn

Py:   os.getcwd()
来源：http://hd.huanxung.cn

PHP:  getcwd();
来源：http://dc.szxytkj.cn

JS:   process.cwd()
来源：http://qd.yuntaijiaju.cn

TS:   process.cwd()
来源：http://xm.nszjky.cn

Java: Path.of("").toAbsolutePath()
来源：http://hd.szsharing.cn

Go:   os.Getwd()
来源：http://wd.chemitech.net.cn

Ruby: Dir.pwd
来源：http://sx.hnjuh.cn

C#:   Directory.GetCurrentDirectory()
来源：http://rf.bookmarksfly.cn

[M05] 设置退出码
来源：http://tg.nszjky.cn

Py:   sys.exit(1)
来源：http://xi.chemitech.net.cn

PHP:  exit(1);
来源：http://fe.huixinmuqiang.cn

JS:   process.exit(1)
来源：http://ri.bjjhwx.cn

TS:   process.exit(1)
来源：http://xv.huixinmuqiang.cn

Java: System.exit(1)
来源：http://zl.gzmigu.cn

Go:   os.Exit(1)
来源：http://yb.panjiajie.cn

Ruby: exit 1
来源：http://fk.9csxet.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://jt.szxytkj.cn

[M06] 向标准错误输出
来源：http://cp.bookmarksfly.cn

Py:   print("err", file=sys.stderr)
来源：http://mh.9csxet.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://hs.shtwfgs.cn

JS:   console.error("err")
来源：http://xg.panjiajie.cn

TS:   console.error("err")
来源：http://bm.lnxyls.cn

Java: System.err.println("err")
来源：http://ko.szsharing.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://kt.panjiajie.cn

Ruby: warn "err"
来源：http://hy.lnxyls.cn

C#:   Console.Error.WriteLine("err")
来源：http://nt.asd995.cn

[M07] 判断是否为主入口
来源：http://fn.chemitech.net.cn

Py:   if __name__ == "__main__":
来源：http://ft.wgjwhj.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://uv.hnjuh.cn

JS:   require.main === module
来源：http://ac.colortex.cn

TS:   require.main === module
来源：http://vm.huixinmuqiang.cn

Java: public static void main(String[] args)
来源：http://ng.bookmarksfly.cn

Go:   func main()
来源：http://ny.haigaiapp.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://tm.jctech888.com.cn

C#:   static void Main(string[] args)
来源：http://ep.panjiajie.cn

[M08] 获取系统与运行时信息
来源：http://rp.szsharing.cn

Py:   platform.system();  platform.python_version()
来源：http://wh.chemitech.net.cn

PHP:  PHP_OS;  phpversion();
来源：http://fp.nicolike.cn

JS:   process.platform;  process.version
来源：http://cf.nszjky.cn

TS:   process.platform;  process.version
来源：http://sa.shxzukj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://cz.szxytkj.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://lo.hahajie.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://io.yuntaijiaju.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://bs.bookmarksfly.cn

================================================================================
来源：http://yj.panjiajie.cn

N. 数据结构与算法
来源：http://bk.nicolike.cn

================================================================================
来源：http://uu.muxihuayi.cn

[N01] 二分查找（有序数组）
来源：http://fk.huanxung.cn

Py:   bisect.bisect_left(arr, x)
来源：http://gl.huixinmuqiang.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://fc.newstarts.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sv.bookmarksfly.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dx.bjjhwx.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ft.colortex.cn

Go:   sort.SearchInts(arr, x)
来源：http://jn.gzmigu.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://du.nszjky.cn

C#:   Array.BinarySearch(arr, x)
来源：http://wm.panjiajie.cn

[N02] 排序（工程实践用内置实现）
来源：http://pd.szxytkj.cn

Py:   sorted(arr);  arr.sort()
来源：http://df.huixinmuqiang.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://yx.hahajie.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://hh.hahajie.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://cm.nszjky.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ot.hahajie.cn

Go:   slices.Sort(arr)
来源：http://fz.newstarts.cn

Ruby: arr.sort
来源：http://ak.huixiangedu.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://eu.bjjhwx.cn

[N03] 快速排序（分治示例）
来源：http://du.szsharing.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://dk.shxzukj.cn

PHP:  // 递归实现，或用 usort
来源：http://wn.hnjuh.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kq.panjiajie.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sj.9csxet.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://cn.chemitech.net.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://nz.9csxet.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://qe.jianghongdianzi.cn

C#:   // 手写递归，或 Array.Sort
来源：http://pl.yuexingan06.cn

[N04] 斐波那契数列
来源：http://eq.9csxet.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://nj.nicolike.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://jp.nicolike.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xb.huixinmuqiang.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bv.asd995.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ac.szxytkj.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ad.colortex.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://am.hnjuh.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ze.asd995.cn

[N05] 最大公约数
来源：http://ue.newstarts.cn

Py:   math.gcd(a, b)
来源：http://il.lnxyls.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://pv.nszjky.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hr.jctech888.com.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ul.hahajie.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://fz.gzmigu.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://md.huixinmuqiang.cn

Ruby: a.gcd(b)
来源：http://fx.jctech888.com.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://to.shtwfgs.cn

[N06] 判断回文字符串
来源：http://qi.haigaiapp.cn

Py:   s == s[::-1]
来源：http://me.shxzskj.cn

PHP:  $s === strrev($s);
来源：http://br.colortex.cn

JS:   s === [...s].reverse().join("")
来源：http://yc.huixinmuqiang.cn

TS:   s === [...s].reverse().join("")
来源：http://hn.shxzskj.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://va.521024.cn

Go:   // 双指针从两端比较
来源：http://rp.muxihuayi.cn

Ruby: s == s.reverse
来源：http://im.521024.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://wj.shxzukj.cn

[N07] 两数之和（返回下标）
来源：http://pe.nicolike.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://rf.szsharing.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jm.newstarts.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ri.521024.cn

TS:   // 手写 Map<string, number>
来源：http://dt.colortex.cn

Java: // 手写 HashMap
来源：http://up.bjjhwx.cn

Go:   // 手写 map[int]int
来源：http://zu.bookmarksfly.cn

Ruby: // 手写 Hash
来源：http://uz.yuexingan06.cn

C#:   // 手写 Dictionary<int, int>
来源：http://hn.szxytkj.cn

[N08] 生成全排列
来源：http://ga.jianghongdianzi.cn

Py:   itertools.permutations(arr)
来源：http://by.9csxet.cn

PHP:  // 手写递归交换
来源：http://eg.chemitech.net.cn

JS:   // 手写回溯递归
来源：http://tm.shxzskj.cn

TS:   // 手写回溯递归
来源：http://mg.yuntaijiaju.cn

Java: // 手写回溯递归
来源：http://ab.bjjhwx.cn

Go:   // 手写回溯递归
来源：http://op.newstarts.cn

Ruby: arr.permutation.to_a
来源：http://qa.shxzskj.cn

C#:   // 手写回溯递归
来源：http://yy.yuntaijiaju.cn

[N09] 栈与队列
来源：http://rj.shtwfgs.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://qr.yuntaijiaju.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hb.shxzukj.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://va.jctech888.com.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://qq.yuntaijiaju.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://xp.521024.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://gm.szsharing.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://xq.lnxyls.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ef.lnxyls.cn

[N10] 链表节点定义
来源：http://lk.shxzukj.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://os.huixiangedu.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://sf.huixiangedu.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://jq.chemitech.net.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://go.huixinmuqiang.cn

Java: class Node { int v; Node next; }
来源：http://no.jianghongdianzi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://dj.bjjhwx.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://vo.wgjwhj.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://cs.jianghongdianzi.cn

[N11] 二叉树中序遍历
来源：http://ht.521024.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://vk.panjiajie.cn

PHP:  // 手写递归函数
来源：http://ij.bookmarksfly.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wp.huixiangedu.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gz.jctech888.com.cn

Java: // 手写递归
来源：http://oo.jianghongdianzi.cn

Go:   // 手写递归
来源：http://rh.huixiangedu.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wz.jianghongdianzi.cn

C#:   // 手写递归
来源：http://tv.jctech888.com.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://lt.szxytkj.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wx.shtwfgs.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://da.jianghongdianzi.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rb.panjiajie.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gf.szsharing.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://yc.521024.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://dn.shtwfgs.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://zo.muxihuayi.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://oc.panjiajie.cn

================================================================================
来源：http://nr.chemitech.net.cn

O. 并发与异步
来源：http://zi.newstarts.cn

================================================================================
来源：http://pz.9csxet.cn

[O01] 启动一个线程
来源：http://nr.521024.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://tx.szsharing.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://zw.bjjhwx.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://no.jctech888.com.cn

TS:   // 同 JS
来源：http://rl.chemitech.net.cn

Java: new Thread(() -> f()).start()
来源：http://nl.colortex.cn

Go:   go f()
来源：http://jx.chemitech.net.cn

Ruby: Thread.new { f }
来源：http://qc.newstarts.cn

C#:   Task.Run(() => F());
来源：http://px.colortex.cn

[O02] 使用线程池
来源：http://nb.huixiangedu.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://jt.szxytkj.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://et.newstarts.cn

JS:   // worker_threads 线程池
来源：http://bl.jctech888.com.cn

TS:   // worker_threads 线程池
来源：http://tq.hnjuh.cn

Java: Executors.newFixedThreadPool(4)
来源：http://oc.szsharing.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ql.hahajie.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wm.huixinmuqiang.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ks.chemitech.net.cn

[O03] 加锁保护共享数据
来源：http://zs.9csxet.cn

Py:   with lock: shared += 1
来源：http://nj.bookmarksfly.cn

PHP:  // 用 flock() 做文件锁
来源：http://cp.jctech888.com.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://py.szxytkj.cn

TS:   // 同 JS
来源：http://dn.colortex.cn

Java: synchronized (this) { shared++; }
来源：http://ml.yuntaijiaju.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://xr.huixiangedu.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://sy.szsharing.cn

C#:   lock (gate) { shared++; }
来源：http://in.yuexingan06.cn

[O04] 定义异步函数并等待
来源：http://ty.nicolike.cn

Py:   async def f():⏎    await g()
来源：http://zw.shxzskj.cn


<!-- 参考信息 -->