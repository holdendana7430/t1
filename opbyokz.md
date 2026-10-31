代发 wailian999

[K06] 解析 URL 查询串
来源：http://zx.shxzskj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://sc.huanxung.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://vb.jianghongdianzi.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tf.shtwfgs.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nu.chemitech.net.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://uz.szxytkj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://rs.haigaiapp.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ys.gzmigu.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zy.jctech888.com.cn

[K07] 进制转换
来源：http://up.hnjuh.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wq.shxzskj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://rn.panjiajie.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://cx.huixinmuqiang.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://jb.szsharing.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hd.hnjuh.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://dz.wgjwhj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://bo.jianghongdianzi.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://dv.muxihuayi.cn

[K08] 二进制序列化（非 JSON）
来源：http://gk.huanxung.cn

Py:   pickle.dumps(obj)
来源：http://bl.lnxyls.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://rn.shxzukj.cn

JS:   v8.serialize(obj)        // Node
来源：http://gr.gzmigu.cn

TS:   v8.serialize(obj)        // Node
来源：http://wt.nicolike.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ig.colortex.cn

Go:   encoding/gob
来源：http://ik.bjjhwx.cn

Ruby: Marshal.dump(obj)
来源：http://jy.jctech888.com.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.szxytkj.cn

================================================================================
来源：http://nd.nicolike.cn

L. 网络请求
来源：http://fq.lnxyls.cn

================================================================================
来源：http://ri.hnjuh.cn

[L01] 发送 GET 请求
来源：http://vj.panjiajie.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hd.chemitech.net.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://sw.muxihuayi.cn

JS:   await fetch(url)
来源：http://nu.shxzskj.cn

TS:   await fetch(url)
来源：http://og.9csxet.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mm.muxihuayi.cn

Go:   resp, err := http.Get(url)
来源：http://rf.521024.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://oe.yuexingan06.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hg.haigaiapp.cn

[L02] 发送 POST JSON
来源：http://cg.szsharing.cn

Py:   requests.post(url, json={"a": 1})
来源：http://cb.wgjwhj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ps.huixiangedu.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hu.huixinmuqiang.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gq.hnjuh.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://co.huanxung.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ei.jianghongdianzi.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://bd.shxzukj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://kw.szsharing.cn

[L03] 设置自定义请求头
来源：http://rn.muxihuayi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://bn.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://zq.9csxet.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ea.szsharing.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qq.bjjhwx.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://xc.lnxyls.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ut.haigaiapp.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wd.bookmarksfly.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://zc.521024.cn

[L04] 设置超时
来源：http://nq.521024.cn

Py:   requests.get(url, timeout=5)
来源：http://wi.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://fk.bookmarksfly.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rc.hahajie.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nz.521024.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://bm.jctech888.com.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://vp.huanxung.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://cn.yuexingan06.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://tb.huixinmuqiang.cn

[L05] 上传文件（multipart）
来源：http://vv.huixiangedu.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://gf.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://go.521024.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://nm.hahajie.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://vn.huixinmuqiang.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://lx.gzmigu.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://pw.haigaiapp.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ny.muxihuayi.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://lq.521024.cn

[L06] 解析响应为 JSON
来源：http://ck.hnjuh.cn

Py:   resp.json()
来源：http://hj.bjjhwx.cn

PHP:  json_decode($body, true);
来源：http://xo.hnjuh.cn

JS:   await resp.json()
来源：http://eg.jctech888.com.cn

TS:   await resp.json()
来源：http://wz.hnjuh.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://zt.9csxet.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hh.jctech888.com.cn

Ruby: JSON.parse(resp.body)
来源：http://mp.huixinmuqiang.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://cz.jianghongdianzi.cn

[L07] 处理 HTTP 状态码
来源：http://gp.shxzukj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://dm.huixiangedu.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hp.shxzukj.cn

JS:   resp.ok;  resp.status
来源：http://ly.hahajie.cn

TS:   resp.ok;  resp.status
来源：http://tl.huixiangedu.cn

Java: resp.statusCode()
来源：http://fk.521024.cn

Go:   resp.StatusCode
来源：http://ei.muxihuayi.cn

Ruby: resp.code.to_i
来源：http://hd.nicolike.cn

C#:   (int)resp.StatusCode
来源：http://ly.gzmigu.cn

[L08] 并发请求多个地址
来源：http://lv.huixiangedu.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://dy.nicolike.cn

PHP:  curl_multi_init() 系列
来源：http://ya.wgjwhj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zm.chemitech.net.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zf.yuntaijiaju.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://no.shxzskj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qd.shxzskj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ji.nicolike.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://cr.wgjwhj.cn

================================================================================
来源：http://ir.szxytkj.cn

M. 命令行 / 进程 / 环境
来源：http://aj.nszjky.cn

================================================================================
来源：http://jo.shxzskj.cn

[M01] 读取命令行参数
来源：http://iu.jianghongdianzi.cn

Py:   sys.argv[1:]
来源：http://ae.newstarts.cn

PHP:  $argv;  $argc;
来源：http://cr.huixinmuqiang.cn

JS:   process.argv.slice(2)
来源：http://kd.hnjuh.cn

TS:   process.argv.slice(2)
来源：http://px.shxzskj.cn

Java: args 数组（main 方法参数）
来源：http://pf.szsharing.cn

Go:   os.Args[1:]
来源：http://ie.shxzukj.cn

Ruby: ARGV
来源：http://of.9csxet.cn

C#:   args 数组（Main 方法参数）
来源：http://tj.lnxyls.cn

[M02] 读取环境变量
来源：http://xg.shtwfgs.cn

Py:   os.environ.get("HOME")
来源：http://ei.huanxung.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://cd.chemitech.net.cn

JS:   process.env.HOME
来源：http://hz.huixiangedu.cn

TS:   process.env.HOME
来源：http://bn.shtwfgs.cn

Java: System.getenv("HOME")
来源：http://kh.nicolike.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://eh.shxzukj.cn

Ruby: ENV["HOME"]
来源：http://tz.bookmarksfly.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://tz.hnjuh.cn

[M03] 执行外部命令
来源：http://rh.chemitech.net.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://fd.huixinmuqiang.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://qw.panjiajie.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://vx.haigaiapp.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://yb.shxzukj.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://il.521024.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://fk.panjiajie.cn

Ruby: system("ls -l");  `ls -l`
来源：http://sq.nicolike.cn

C#:   Process.Start("ls", "-l");
来源：http://xq.shtwfgs.cn

[M04] 获取当前工作目录
来源：http://je.shtwfgs.cn

Py:   os.getcwd()
来源：http://cf.huixiangedu.cn

PHP:  getcwd();
来源：http://wj.jianghongdianzi.cn

JS:   process.cwd()
来源：http://mp.colortex.cn

TS:   process.cwd()
来源：http://ie.shxzukj.cn

Java: Path.of("").toAbsolutePath()
来源：http://qd.panjiajie.cn

Go:   os.Getwd()
来源：http://yz.colortex.cn

Ruby: Dir.pwd
来源：http://li.nszjky.cn

C#:   Directory.GetCurrentDirectory()
来源：http://fy.bjjhwx.cn

[M05] 设置退出码
来源：http://nh.huixinmuqiang.cn

Py:   sys.exit(1)
来源：http://nk.huixiangedu.cn

PHP:  exit(1);
来源：http://bm.bjjhwx.cn

JS:   process.exit(1)
来源：http://wt.shtwfgs.cn

TS:   process.exit(1)
来源：http://aq.hnjuh.cn

Java: System.exit(1)
来源：http://kx.hahajie.cn

Go:   os.Exit(1)
来源：http://jl.panjiajie.cn

Ruby: exit 1
来源：http://dt.521024.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://sk.hahajie.cn

[M06] 向标准错误输出
来源：http://tm.9csxet.cn

Py:   print("err", file=sys.stderr)
来源：http://rx.colortex.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://gp.9csxet.cn

JS:   console.error("err")
来源：http://lr.bookmarksfly.cn

TS:   console.error("err")
来源：http://vv.colortex.cn

Java: System.err.println("err")
来源：http://hf.shxzukj.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://vy.jctech888.com.cn

Ruby: warn "err"
来源：http://mu.yuntaijiaju.cn

C#:   Console.Error.WriteLine("err")
来源：http://xi.gzmigu.cn

[M07] 判断是否为主入口
来源：http://it.shxzskj.cn

Py:   if __name__ == "__main__":
来源：http://rf.jctech888.com.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ty.521024.cn

JS:   require.main === module
来源：http://qg.szxytkj.cn

TS:   require.main === module
来源：http://xt.hahajie.cn

Java: public static void main(String[] args)
来源：http://ir.newstarts.cn

Go:   func main()
来源：http://hj.szxytkj.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ub.lnxyls.cn

C#:   static void Main(string[] args)
来源：http://tf.chemitech.net.cn

[M08] 获取系统与运行时信息
来源：http://ut.szsharing.cn

Py:   platform.system();  platform.python_version()
来源：http://qz.bookmarksfly.cn

PHP:  PHP_OS;  phpversion();
来源：http://uc.asd995.cn

JS:   process.platform;  process.version
来源：http://mm.wgjwhj.cn

TS:   process.platform;  process.version
来源：http://si.9csxet.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://gc.hnjuh.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ig.9csxet.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://sv.jianghongdianzi.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://nd.yuntaijiaju.cn

================================================================================
来源：http://fk.hnjuh.cn

N. 数据结构与算法
来源：http://rv.gzmigu.cn

================================================================================
来源：http://so.huanxung.cn

[N01] 二分查找（有序数组）
来源：http://pl.huixiangedu.cn

Py:   bisect.bisect_left(arr, x)
来源：http://wv.yuntaijiaju.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://xz.muxihuayi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://da.muxihuayi.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ac.shxzukj.cn

Java: Arrays.binarySearch(arr, x)
来源：http://uo.colortex.cn

Go:   sort.SearchInts(arr, x)
来源：http://qx.asd995.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://dx.hnjuh.cn

C#:   Array.BinarySearch(arr, x)
来源：http://gp.szsharing.cn

[N02] 排序（工程实践用内置实现）
来源：http://ox.bookmarksfly.cn

Py:   sorted(arr);  arr.sort()
来源：http://gg.jctech888.com.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://te.shxzskj.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ye.yuntaijiaju.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://pv.shtwfgs.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://gk.huanxung.cn

Go:   slices.Sort(arr)
来源：http://ed.chemitech.net.cn

Ruby: arr.sort
来源：http://uk.shxzukj.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://kz.haigaiapp.cn

[N03] 快速排序（分治示例）
来源：http://iv.chemitech.net.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://km.newstarts.cn

PHP:  // 递归实现，或用 usort
来源：http://tv.nszjky.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rg.nszjky.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jz.hnjuh.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ek.gzmigu.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mq.szxytkj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mg.shxzukj.cn

C#:   // 手写递归，或 Array.Sort
来源：http://gp.haigaiapp.cn

[N04] 斐波那契数列
来源：http://zh.shxzukj.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://sw.muxihuayi.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://bv.szsharing.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://uc.nicolike.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://uc.huixinmuqiang.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://tm.nszjky.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://gm.yuexingan06.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://pr.lnxyls.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://sc.newstarts.cn

[N05] 最大公约数
来源：http://dj.muxihuayi.cn

Py:   math.gcd(a, b)
来源：http://yl.szxytkj.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://vs.yuntaijiaju.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fb.colortex.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mf.521024.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://pw.shxzskj.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://cj.yuexingan06.cn

Ruby: a.gcd(b)
来源：http://sx.huixiangedu.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://gc.haigaiapp.cn

[N06] 判断回文字符串
来源：http://xq.hnjuh.cn

Py:   s == s[::-1]
来源：http://wk.hahajie.cn

PHP:  $s === strrev($s);
来源：http://ap.muxihuayi.cn

JS:   s === [...s].reverse().join("")
来源：http://lh.shxzukj.cn

TS:   s === [...s].reverse().join("")
来源：http://tu.jctech888.com.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://vw.wgjwhj.cn

Go:   // 双指针从两端比较
来源：http://rc.haigaiapp.cn

Ruby: s == s.reverse
来源：http://fe.chemitech.net.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://uz.muxihuayi.cn

[N07] 两数之和（返回下标）
来源：http://sm.9csxet.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ra.shtwfgs.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://xr.hahajie.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://pu.yuntaijiaju.cn

TS:   // 手写 Map<string, number>
来源：http://wp.hahajie.cn

Java: // 手写 HashMap
来源：http://pt.521024.cn

Go:   // 手写 map[int]int
来源：http://pv.asd995.cn

Ruby: // 手写 Hash
来源：http://ai.wgjwhj.cn

C#:   // 手写 Dictionary<int, int>
来源：http://vk.huixinmuqiang.cn

[N08] 生成全排列
来源：http://gg.521024.cn

Py:   itertools.permutations(arr)
来源：http://zr.huanxung.cn

PHP:  // 手写递归交换
来源：http://mr.hnjuh.cn

JS:   // 手写回溯递归
来源：http://me.bookmarksfly.cn

TS:   // 手写回溯递归
来源：http://al.muxihuayi.cn

Java: // 手写回溯递归
来源：http://mr.szxytkj.cn

Go:   // 手写回溯递归
来源：http://ab.muxihuayi.cn

Ruby: arr.permutation.to_a
来源：http://cc.colortex.cn

C#:   // 手写回溯递归
来源：http://jz.hahajie.cn

[N09] 栈与队列
来源：http://ef.gzmigu.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://dh.521024.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://zp.asd995.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wi.9csxet.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://xs.yuntaijiaju.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://jt.shtwfgs.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hm.nicolike.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://am.nicolike.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://sl.lnxyls.cn

[N10] 链表节点定义
来源：http://sr.bookmarksfly.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qp.yuntaijiaju.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://wg.muxihuayi.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://we.shxzskj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://xc.hahajie.cn

Java: class Node { int v; Node next; }
来源：http://uq.haigaiapp.cn

Go:   type Node struct { V int; Next *Node }
来源：http://rd.haigaiapp.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://rb.haigaiapp.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ks.jianghongdianzi.cn

[N11] 二叉树中序遍历
来源：http://nj.bjjhwx.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mr.muxihuayi.cn

PHP:  // 手写递归函数
来源：http://qq.huixiangedu.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kz.shtwfgs.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qv.szxytkj.cn

Java: // 手写递归
来源：http://yj.muxihuayi.cn

Go:   // 手写递归
来源：http://mt.hnjuh.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mc.huixiangedu.cn

C#:   // 手写递归
来源：http://lu.521024.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://qq.hnjuh.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://fi.gzmigu.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://rl.9csxet.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jy.newstarts.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://iy.gzmigu.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://yj.yuntaijiaju.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://aa.yuexingan06.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://jq.shtwfgs.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://jq.hahajie.cn

================================================================================
来源：http://si.lnxyls.cn

O. 并发与异步
来源：http://jf.muxihuayi.cn

================================================================================
来源：http://vl.wgjwhj.cn

[O01] 启动一个线程
来源：http://oz.shxzukj.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://nl.huanxung.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ha.jianghongdianzi.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ys.jianghongdianzi.cn

TS:   // 同 JS
来源：http://ue.huanxung.cn

Java: new Thread(() -> f()).start()
来源：http://va.shxzskj.cn

Go:   go f()
来源：http://oa.nicolike.cn

Ruby: Thread.new { f }
来源：http://im.bookmarksfly.cn

C#:   Task.Run(() => F());
来源：http://tz.huixinmuqiang.cn


<!-- 参考信息 -->