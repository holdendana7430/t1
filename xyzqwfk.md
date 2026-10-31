代发 wailian999

[K06] 解析 URL 查询串
来源：http://tv.szxytkj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://sn.szsharing.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fy.colortex.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zd.asd995.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fs.lnxyls.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://kn.jctech888.com.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://qh.hahajie.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://eq.shtwfgs.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://qg.gzmigu.cn

[K07] 进制转换
来源：http://zj.asd995.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://pp.hnjuh.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://rb.yuexingan06.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ox.jianghongdianzi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://bo.bookmarksfly.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://si.yuexingan06.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://xs.nicolike.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hx.szxytkj.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://lj.hnjuh.cn

[K08] 二进制序列化（非 JSON）
来源：http://cl.shxzukj.cn

Py:   pickle.dumps(obj)
来源：http://rc.shtwfgs.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://lx.hahajie.cn

JS:   v8.serialize(obj)        // Node
来源：http://jy.nszjky.cn

TS:   v8.serialize(obj)        // Node
来源：http://ag.bjjhwx.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ye.wgjwhj.cn

Go:   encoding/gob
来源：http://fb.shxzukj.cn

Ruby: Marshal.dump(obj)
来源：http://vw.wgjwhj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://sg.bjjhwx.cn

================================================================================
来源：http://hw.yuexingan06.cn

L. 网络请求
来源：http://xx.yuexingan06.cn

================================================================================
来源：http://yg.bookmarksfly.cn

[L01] 发送 GET 请求
来源：http://yh.yuntaijiaju.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://zu.bjjhwx.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ce.shxzskj.cn

JS:   await fetch(url)
来源：http://np.chemitech.net.cn

TS:   await fetch(url)
来源：http://pc.gzmigu.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://xr.szxytkj.cn

Go:   resp, err := http.Get(url)
来源：http://dw.newstarts.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ec.jctech888.com.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://vg.shtwfgs.cn

[L02] 发送 POST JSON
来源：http://mx.nicolike.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ta.gzmigu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ep.gzmigu.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lq.521024.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://im.huixinmuqiang.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://pe.huixinmuqiang.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://zd.lnxyls.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://en.nicolike.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wz.nicolike.cn

[L03] 设置自定义请求头
来源：http://wr.huixinmuqiang.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://nx.521024.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://xf.yuntaijiaju.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kn.521024.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ih.szxytkj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ah.jctech888.com.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ts.shxzskj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://zm.huixinmuqiang.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://br.huixiangedu.cn

[L04] 设置超时
来源：http://rt.lnxyls.cn

Py:   requests.get(url, timeout=5)
来源：http://ae.521024.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://jr.shxzukj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ts.haigaiapp.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dv.jianghongdianzi.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ae.gzmigu.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ly.huixiangedu.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://oh.yuexingan06.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://cb.bjjhwx.cn

[L05] 上传文件（multipart）
来源：http://tg.muxihuayi.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://gw.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://li.jianghongdianzi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://fx.szxytkj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://js.colortex.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://iq.panjiajie.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://no.asd995.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://rp.nszjky.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://um.gzmigu.cn

[L06] 解析响应为 JSON
来源：http://aq.shxzukj.cn

Py:   resp.json()
来源：http://tx.asd995.cn

PHP:  json_decode($body, true);
来源：http://mt.jianghongdianzi.cn

JS:   await resp.json()
来源：http://pe.jianghongdianzi.cn

TS:   await resp.json()
来源：http://nu.521024.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://uo.szsharing.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://un.newstarts.cn

Ruby: JSON.parse(resp.body)
来源：http://vm.nicolike.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://dm.huixinmuqiang.cn

[L07] 处理 HTTP 状态码
来源：http://ex.huixinmuqiang.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://fy.gzmigu.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://rz.nszjky.cn

JS:   resp.ok;  resp.status
来源：http://bw.yuntaijiaju.cn

TS:   resp.ok;  resp.status
来源：http://nf.jianghongdianzi.cn

Java: resp.statusCode()
来源：http://zv.521024.cn

Go:   resp.StatusCode
来源：http://ia.newstarts.cn

Ruby: resp.code.to_i
来源：http://zu.shtwfgs.cn

C#:   (int)resp.StatusCode
来源：http://nk.gzmigu.cn

[L08] 并发请求多个地址
来源：http://nu.shxzskj.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://pj.bjjhwx.cn

PHP:  curl_multi_init() 系列
来源：http://nx.shxzskj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jz.hahajie.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vd.gzmigu.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://xm.haigaiapp.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://he.shtwfgs.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://jm.nszjky.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wj.bjjhwx.cn

================================================================================
来源：http://mg.gzmigu.cn

M. 命令行 / 进程 / 环境
来源：http://rw.muxihuayi.cn

================================================================================
来源：http://aj.hnjuh.cn

[M01] 读取命令行参数
来源：http://lw.szxytkj.cn

Py:   sys.argv[1:]
来源：http://bt.hnjuh.cn

PHP:  $argv;  $argc;
来源：http://xj.521024.cn

JS:   process.argv.slice(2)
来源：http://td.haigaiapp.cn

TS:   process.argv.slice(2)
来源：http://cu.9csxet.cn

Java: args 数组（main 方法参数）
来源：http://pg.huanxung.cn

Go:   os.Args[1:]
来源：http://ca.gzmigu.cn

Ruby: ARGV
来源：http://ua.szsharing.cn

C#:   args 数组（Main 方法参数）
来源：http://ej.9csxet.cn

[M02] 读取环境变量
来源：http://cu.huanxung.cn

Py:   os.environ.get("HOME")
来源：http://yp.panjiajie.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://gp.huixiangedu.cn

JS:   process.env.HOME
来源：http://bp.huixiangedu.cn

TS:   process.env.HOME
来源：http://gs.yuntaijiaju.cn

Java: System.getenv("HOME")
来源：http://zv.9csxet.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ur.yuexingan06.cn

Ruby: ENV["HOME"]
来源：http://xd.9csxet.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://uw.nicolike.cn

[M03] 执行外部命令
来源：http://br.szsharing.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://cj.colortex.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://na.9csxet.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://zl.gzmigu.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://xv.shxzskj.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://lr.shxzukj.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://dq.shxzukj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://si.nszjky.cn

C#:   Process.Start("ls", "-l");
来源：http://ci.521024.cn

[M04] 获取当前工作目录
来源：http://zc.521024.cn

Py:   os.getcwd()
来源：http://wt.colortex.cn

PHP:  getcwd();
来源：http://hj.jianghongdianzi.cn

JS:   process.cwd()
来源：http://nm.nszjky.cn

TS:   process.cwd()
来源：http://ql.nszjky.cn

Java: Path.of("").toAbsolutePath()
来源：http://xy.jianghongdianzi.cn

Go:   os.Getwd()
来源：http://zz.shxzukj.cn

Ruby: Dir.pwd
来源：http://bk.haigaiapp.cn

C#:   Directory.GetCurrentDirectory()
来源：http://rb.bookmarksfly.cn

[M05] 设置退出码
来源：http://vy.shxzukj.cn

Py:   sys.exit(1)
来源：http://vp.newstarts.cn

PHP:  exit(1);
来源：http://zb.jianghongdianzi.cn

JS:   process.exit(1)
来源：http://ml.muxihuayi.cn

TS:   process.exit(1)
来源：http://ii.521024.cn

Java: System.exit(1)
来源：http://mn.nszjky.cn

Go:   os.Exit(1)
来源：http://qy.colortex.cn

Ruby: exit 1
来源：http://oq.chemitech.net.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://lb.shxzskj.cn

[M06] 向标准错误输出
来源：http://dq.wgjwhj.cn

Py:   print("err", file=sys.stderr)
来源：http://vc.colortex.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://jm.szxytkj.cn

JS:   console.error("err")
来源：http://cm.panjiajie.cn

TS:   console.error("err")
来源：http://rl.panjiajie.cn

Java: System.err.println("err")
来源：http://ud.yuexingan06.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ca.shxzskj.cn

Ruby: warn "err"
来源：http://ni.asd995.cn

C#:   Console.Error.WriteLine("err")
来源：http://ky.nszjky.cn

[M07] 判断是否为主入口
来源：http://mj.muxihuayi.cn

Py:   if __name__ == "__main__":
来源：http://oa.hahajie.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://vn.wgjwhj.cn

JS:   require.main === module
来源：http://vw.newstarts.cn

TS:   require.main === module
来源：http://ev.haigaiapp.cn

Java: public static void main(String[] args)
来源：http://zb.yuntaijiaju.cn

Go:   func main()
来源：http://lp.szsharing.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://bd.shxzskj.cn

C#:   static void Main(string[] args)
来源：http://yx.bookmarksfly.cn

[M08] 获取系统与运行时信息
来源：http://ja.shxzukj.cn

Py:   platform.system();  platform.python_version()
来源：http://gv.wgjwhj.cn

PHP:  PHP_OS;  phpversion();
来源：http://vy.lnxyls.cn

JS:   process.platform;  process.version
来源：http://yl.huanxung.cn

TS:   process.platform;  process.version
来源：http://pu.nszjky.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://yx.szsharing.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://pt.shxzukj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://in.muxihuayi.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://wl.hahajie.cn

================================================================================
来源：http://lp.gzmigu.cn

N. 数据结构与算法
来源：http://qc.bjjhwx.cn

================================================================================
来源：http://my.chemitech.net.cn

[N01] 二分查找（有序数组）
来源：http://jw.gzmigu.cn

Py:   bisect.bisect_left(arr, x)
来源：http://oc.colortex.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hd.chemitech.net.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://af.jctech888.com.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gq.huixinmuqiang.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ba.shxzukj.cn

Go:   sort.SearchInts(arr, x)
来源：http://sw.jctech888.com.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://sn.yuexingan06.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ob.newstarts.cn

[N02] 排序（工程实践用内置实现）
来源：http://ln.bookmarksfly.cn

Py:   sorted(arr);  arr.sort()
来源：http://zc.muxihuayi.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://tj.muxihuayi.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://lt.szxytkj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://xr.shtwfgs.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ek.hahajie.cn

Go:   slices.Sort(arr)
来源：http://uz.haigaiapp.cn

Ruby: arr.sort
来源：http://nt.colortex.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://bz.521024.cn

[N03] 快速排序（分治示例）
来源：http://cy.hnjuh.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://yt.gzmigu.cn

PHP:  // 递归实现，或用 usort
来源：http://ek.bookmarksfly.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bj.haigaiapp.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vj.huixinmuqiang.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ti.colortex.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ah.gzmigu.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://jj.panjiajie.cn

C#:   // 手写递归，或 Array.Sort
来源：http://wd.asd995.cn

[N04] 斐波那契数列
来源：http://su.shtwfgs.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://so.huanxung.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ol.bookmarksfly.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hl.asd995.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://in.huixinmuqiang.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://de.gzmigu.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mm.bjjhwx.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://yp.szsharing.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://il.muxihuayi.cn

[N05] 最大公约数
来源：http://mo.panjiajie.cn

Py:   math.gcd(a, b)
来源：http://bg.huanxung.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://tg.muxihuayi.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ym.muxihuayi.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nn.gzmigu.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://nv.huanxung.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://at.yuexingan06.cn

Ruby: a.gcd(b)
来源：http://di.huanxung.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wb.nszjky.cn

[N06] 判断回文字符串
来源：http://vp.hahajie.cn

Py:   s == s[::-1]
来源：http://ri.chemitech.net.cn

PHP:  $s === strrev($s);
来源：http://nk.szsharing.cn

JS:   s === [...s].reverse().join("")
来源：http://wq.bookmarksfly.cn

TS:   s === [...s].reverse().join("")
来源：http://hr.wgjwhj.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ke.haigaiapp.cn

Go:   // 双指针从两端比较
来源：http://si.lnxyls.cn

Ruby: s == s.reverse
来源：http://ng.huanxung.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ym.gzmigu.cn

[N07] 两数之和（返回下标）
来源：http://di.colortex.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://il.hahajie.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ao.muxihuayi.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://yf.yuexingan06.cn

TS:   // 手写 Map<string, number>
来源：http://gd.hahajie.cn

Java: // 手写 HashMap
来源：http://rf.szxytkj.cn

Go:   // 手写 map[int]int
来源：http://bq.shxzukj.cn

Ruby: // 手写 Hash
来源：http://ch.huixiangedu.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ga.newstarts.cn

[N08] 生成全排列
来源：http://fq.jctech888.com.cn

Py:   itertools.permutations(arr)
来源：http://vp.gzmigu.cn

PHP:  // 手写递归交换
来源：http://lb.gzmigu.cn

JS:   // 手写回溯递归
来源：http://qd.shxzskj.cn

TS:   // 手写回溯递归
来源：http://nm.colortex.cn

Java: // 手写回溯递归
来源：http://ci.huixinmuqiang.cn

Go:   // 手写回溯递归
来源：http://pq.nicolike.cn

Ruby: arr.permutation.to_a
来源：http://wk.huanxung.cn

C#:   // 手写回溯递归
来源：http://re.shxzukj.cn

[N09] 栈与队列
来源：http://bq.bjjhwx.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://kr.shxzukj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wj.szxytkj.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://is.hnjuh.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://jn.wgjwhj.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://fn.hnjuh.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://my.huixiangedu.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://rj.9csxet.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://uh.jianghongdianzi.cn

[N10] 链表节点定义
来源：http://pp.newstarts.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://lc.lnxyls.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://pq.521024.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://th.wgjwhj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://pk.gzmigu.cn

Java: class Node { int v; Node next; }
来源：http://tl.muxihuayi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://wz.521024.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://hf.521024.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://oq.shxzukj.cn

[N11] 二叉树中序遍历
来源：http://gm.szxytkj.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wa.szxytkj.cn

PHP:  // 手写递归函数
来源：http://vu.asd995.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tq.huixinmuqiang.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bg.yuntaijiaju.cn

Java: // 手写递归
来源：http://ee.nicolike.cn

Go:   // 手写递归
来源：http://tz.bookmarksfly.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://cf.panjiajie.cn

C#:   // 手写递归
来源：http://jj.huixiangedu.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://oh.bjjhwx.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ns.lnxyls.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ow.colortex.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sg.hnjuh.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bf.szsharing.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ts.shxzukj.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://yz.szsharing.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://cw.huixinmuqiang.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://gv.haigaiapp.cn

================================================================================
来源：http://wp.chemitech.net.cn

O. 并发与异步
来源：http://nu.wgjwhj.cn

================================================================================
来源：http://bv.bookmarksfly.cn

[O01] 启动一个线程
来源：http://hw.jctech888.com.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ih.lnxyls.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://tv.asd995.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://yt.shxzukj.cn

TS:   // 同 JS
来源：http://ic.chemitech.net.cn

Java: new Thread(() -> f()).start()
来源：http://ek.huixiangedu.cn

Go:   go f()
来源：http://ks.jianghongdianzi.cn

Ruby: Thread.new { f }
来源：http://li.bookmarksfly.cn

C#:   Task.Run(() => F());
来源：http://dn.szsharing.cn


<!-- 参考信息 -->