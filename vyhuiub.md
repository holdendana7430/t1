代发 wailian999

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mm.lnxyls.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dl.shtwfgs.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mf.newstarts.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://nx.chemitech.net.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://nm.gzmigu.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://od.9csxet.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ww.hahajie.cn

[K05] 深拷贝对象
来源：http://hp.jctech888.com.cn

Py:   copy.deepcopy(obj)
来源：http://jr.yuntaijiaju.cn

PHP:  unserialize(serialize($obj));
来源：http://sa.9csxet.cn

JS:   structuredClone(obj)
来源：http://mh.gzmigu.cn

TS:   structuredClone(obj)
来源：http://hx.newstarts.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ut.colortex.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://tx.9csxet.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ei.yuntaijiaju.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ci.bookmarksfly.cn

[K06] 解析 URL 查询串
来源：http://yb.jianghongdianzi.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://pl.lnxyls.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://od.jianghongdianzi.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://oj.shtwfgs.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yp.bjjhwx.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://zp.lnxyls.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ff.huixinmuqiang.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://xz.newstarts.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ii.shxzskj.cn

[K07] 进制转换
来源：http://it.yuexingan06.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://in.bjjhwx.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://qq.colortex.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://jc.szsharing.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://pq.shxzukj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://bx.shtwfgs.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://oh.wgjwhj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ur.9csxet.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://qc.asd995.cn

[K08] 二进制序列化（非 JSON）
来源：http://pu.chemitech.net.cn

Py:   pickle.dumps(obj)
来源：http://ks.hahajie.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://np.newstarts.cn

JS:   v8.serialize(obj)        // Node
来源：http://qc.yuexingan06.cn

TS:   v8.serialize(obj)        // Node
来源：http://xf.hnjuh.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://xc.bjjhwx.cn

Go:   encoding/gob
来源：http://af.newstarts.cn

Ruby: Marshal.dump(obj)
来源：http://tu.jctech888.com.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://dq.nszjky.cn

================================================================================
来源：http://wv.muxihuayi.cn

L. 网络请求
来源：http://ga.colortex.cn

================================================================================
来源：http://tm.panjiajie.cn

[L01] 发送 GET 请求
来源：http://xk.szxytkj.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ec.lnxyls.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wi.hahajie.cn

JS:   await fetch(url)
来源：http://qe.panjiajie.cn

TS:   await fetch(url)
来源：http://at.nicolike.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://kj.huixiangedu.cn

Go:   resp, err := http.Get(url)
来源：http://nf.huanxung.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ua.muxihuayi.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://qy.gzmigu.cn

[L02] 发送 POST JSON
来源：http://qi.jianghongdianzi.cn

Py:   requests.post(url, json={"a": 1})
来源：http://pe.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ko.wgjwhj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://el.colortex.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ok.muxihuayi.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://te.hahajie.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://rb.yuntaijiaju.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://at.huixiangedu.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://sy.asd995.cn

[L03] 设置自定义请求头
来源：http://th.9csxet.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://nd.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://yp.shxzskj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yu.yuntaijiaju.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ky.hnjuh.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://fg.shxzskj.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://kg.jctech888.com.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://we.nicolike.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ij.bookmarksfly.cn

[L04] 设置超时
来源：http://qr.szsharing.cn

Py:   requests.get(url, timeout=5)
来源：http://ca.nszjky.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://il.haigaiapp.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://re.nszjky.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gt.jianghongdianzi.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://xj.shxzukj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://dh.yuexingan06.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://xo.gzmigu.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://nv.asd995.cn

[L05] 上传文件（multipart）
来源：http://gc.nszjky.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zp.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://gf.huixinmuqiang.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://sq.hnjuh.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://zu.nicolike.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mz.shxzskj.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://jm.lnxyls.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://fc.szxytkj.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://av.bjjhwx.cn

[L06] 解析响应为 JSON
来源：http://qr.shxzukj.cn

Py:   resp.json()
来源：http://uv.gzmigu.cn

PHP:  json_decode($body, true);
来源：http://mr.lnxyls.cn

JS:   await resp.json()
来源：http://si.wgjwhj.cn

TS:   await resp.json()
来源：http://hz.shxzukj.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://yx.yuexingan06.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ku.huanxung.cn

Ruby: JSON.parse(resp.body)
来源：http://mf.nicolike.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://yi.huixinmuqiang.cn

[L07] 处理 HTTP 状态码
来源：http://fq.asd995.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wx.yuexingan06.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://tv.chemitech.net.cn

JS:   resp.ok;  resp.status
来源：http://os.jianghongdianzi.cn

TS:   resp.ok;  resp.status
来源：http://em.newstarts.cn

Java: resp.statusCode()
来源：http://kh.szsharing.cn

Go:   resp.StatusCode
来源：http://fa.hahajie.cn

Ruby: resp.code.to_i
来源：http://bg.9csxet.cn

C#:   (int)resp.StatusCode
来源：http://ax.nicolike.cn

[L08] 并发请求多个地址
来源：http://tp.newstarts.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://cv.521024.cn

PHP:  curl_multi_init() 系列
来源：http://kx.gzmigu.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xq.9csxet.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ka.bjjhwx.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wd.9csxet.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ok.newstarts.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://xm.lnxyls.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ut.bjjhwx.cn

================================================================================
来源：http://jo.hnjuh.cn

M. 命令行 / 进程 / 环境
来源：http://bg.huixinmuqiang.cn

================================================================================
来源：http://jf.szsharing.cn

[M01] 读取命令行参数
来源：http://wh.yuexingan06.cn

Py:   sys.argv[1:]
来源：http://oo.colortex.cn

PHP:  $argv;  $argc;
来源：http://vc.hahajie.cn

JS:   process.argv.slice(2)
来源：http://ew.yuntaijiaju.cn

TS:   process.argv.slice(2)
来源：http://ix.yuexingan06.cn

Java: args 数组（main 方法参数）
来源：http://sc.nicolike.cn

Go:   os.Args[1:]
来源：http://ag.gzmigu.cn

Ruby: ARGV
来源：http://xi.panjiajie.cn

C#:   args 数组（Main 方法参数）
来源：http://jf.huanxung.cn

[M02] 读取环境变量
来源：http://iv.szsharing.cn

Py:   os.environ.get("HOME")
来源：http://um.9csxet.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://du.hahajie.cn

JS:   process.env.HOME
来源：http://jy.bookmarksfly.cn

TS:   process.env.HOME
来源：http://tv.shxzskj.cn

Java: System.getenv("HOME")
来源：http://qy.wgjwhj.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://cl.bookmarksfly.cn

Ruby: ENV["HOME"]
来源：http://zk.newstarts.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mc.panjiajie.cn

[M03] 执行外部命令
来源：http://wr.bookmarksfly.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://xv.shxzskj.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://dj.nicolike.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://eu.yuntaijiaju.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ke.nicolike.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://el.shtwfgs.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://zg.jctech888.com.cn

Ruby: system("ls -l");  `ls -l`
来源：http://fq.huanxung.cn

C#:   Process.Start("ls", "-l");
来源：http://el.hnjuh.cn

[M04] 获取当前工作目录
来源：http://pf.huanxung.cn

Py:   os.getcwd()
来源：http://kz.bookmarksfly.cn

PHP:  getcwd();
来源：http://dp.nszjky.cn

JS:   process.cwd()
来源：http://px.huanxung.cn

TS:   process.cwd()
来源：http://vj.huixiangedu.cn

Java: Path.of("").toAbsolutePath()
来源：http://om.panjiajie.cn

Go:   os.Getwd()
来源：http://in.wgjwhj.cn

Ruby: Dir.pwd
来源：http://wl.nicolike.cn

C#:   Directory.GetCurrentDirectory()
来源：http://oa.521024.cn

[M05] 设置退出码
来源：http://ja.szxytkj.cn

Py:   sys.exit(1)
来源：http://cj.jctech888.com.cn

PHP:  exit(1);
来源：http://dq.shxzskj.cn

JS:   process.exit(1)
来源：http://wx.panjiajie.cn

TS:   process.exit(1)
来源：http://vf.szsharing.cn

Java: System.exit(1)
来源：http://ad.newstarts.cn

Go:   os.Exit(1)
来源：http://qb.muxihuayi.cn

Ruby: exit 1
来源：http://vh.bookmarksfly.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://lx.gzmigu.cn

[M06] 向标准错误输出
来源：http://jz.huixiangedu.cn

Py:   print("err", file=sys.stderr)
来源：http://hk.521024.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://zm.shxzskj.cn

JS:   console.error("err")
来源：http://pi.hahajie.cn

TS:   console.error("err")
来源：http://as.gzmigu.cn

Java: System.err.println("err")
来源：http://sj.gzmigu.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://do.jianghongdianzi.cn

Ruby: warn "err"
来源：http://rv.muxihuayi.cn

C#:   Console.Error.WriteLine("err")
来源：http://ai.huixiangedu.cn

[M07] 判断是否为主入口
来源：http://wx.jianghongdianzi.cn

Py:   if __name__ == "__main__":
来源：http://su.muxihuayi.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://zv.wgjwhj.cn

JS:   require.main === module
来源：http://mw.521024.cn

TS:   require.main === module
来源：http://ee.lnxyls.cn

Java: public static void main(String[] args)
来源：http://rn.jctech888.com.cn

Go:   func main()
来源：http://hw.nszjky.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://md.shxzskj.cn

C#:   static void Main(string[] args)
来源：http://bu.newstarts.cn

[M08] 获取系统与运行时信息
来源：http://pb.bookmarksfly.cn

Py:   platform.system();  platform.python_version()
来源：http://sc.asd995.cn

PHP:  PHP_OS;  phpversion();
来源：http://du.muxihuayi.cn

JS:   process.platform;  process.version
来源：http://zi.hahajie.cn

TS:   process.platform;  process.version
来源：http://dd.shxzukj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://dx.asd995.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://eq.szxytkj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://qz.hnjuh.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://zi.521024.cn

================================================================================
来源：http://hk.hnjuh.cn

N. 数据结构与算法
来源：http://ws.szsharing.cn

================================================================================
来源：http://vj.9csxet.cn

[N01] 二分查找（有序数组）
来源：http://xb.panjiajie.cn

Py:   bisect.bisect_left(arr, x)
来源：http://kg.huixiangedu.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://tx.colortex.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ol.shxzukj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ra.lnxyls.cn

Java: Arrays.binarySearch(arr, x)
来源：http://xk.nszjky.cn

Go:   sort.SearchInts(arr, x)
来源：http://wz.shxzukj.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://kb.521024.cn

C#:   Array.BinarySearch(arr, x)
来源：http://bp.szxytkj.cn

[N02] 排序（工程实践用内置实现）
来源：http://mx.muxihuayi.cn

Py:   sorted(arr);  arr.sort()
来源：http://wy.hnjuh.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ym.lnxyls.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://fb.9csxet.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://tl.shxzukj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://up.yuntaijiaju.cn

Go:   slices.Sort(arr)
来源：http://ni.lnxyls.cn

Ruby: arr.sort
来源：http://qa.szxytkj.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://eg.haigaiapp.cn

[N03] 快速排序（分治示例）
来源：http://bu.szsharing.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://kn.yuntaijiaju.cn

PHP:  // 递归实现，或用 usort
来源：http://jr.wgjwhj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pd.yuexingan06.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gb.shxzukj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://bt.newstarts.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://lt.shxzukj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ro.muxihuayi.cn

C#:   // 手写递归，或 Array.Sort
来源：http://pd.panjiajie.cn

[N04] 斐波那契数列
来源：http://is.nicolike.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://gl.colortex.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://dm.gzmigu.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jx.bjjhwx.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zy.hahajie.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://xd.hnjuh.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://er.chemitech.net.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://jw.wgjwhj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://yf.colortex.cn

[N05] 最大公约数
来源：http://bm.newstarts.cn

Py:   math.gcd(a, b)
来源：http://yw.yuntaijiaju.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://cf.asd995.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fq.bookmarksfly.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wt.haigaiapp.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hh.newstarts.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://qq.bjjhwx.cn

Ruby: a.gcd(b)
来源：http://je.shxzskj.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://cu.wgjwhj.cn

[N06] 判断回文字符串
来源：http://hy.shtwfgs.cn

Py:   s == s[::-1]
来源：http://fn.bjjhwx.cn

PHP:  $s === strrev($s);
来源：http://kc.shxzskj.cn

JS:   s === [...s].reverse().join("")
来源：http://ko.lnxyls.cn

TS:   s === [...s].reverse().join("")
来源：http://kz.szsharing.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://di.muxihuayi.cn

Go:   // 双指针从两端比较
来源：http://xh.lnxyls.cn

Ruby: s == s.reverse
来源：http://pg.9csxet.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://zd.jctech888.com.cn

[N07] 两数之和（返回下标）
来源：http://ab.bookmarksfly.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://gi.newstarts.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wk.bjjhwx.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://wp.chemitech.net.cn

TS:   // 手写 Map<string, number>
来源：http://uk.hnjuh.cn

Java: // 手写 HashMap
来源：http://qk.muxihuayi.cn

Go:   // 手写 map[int]int
来源：http://lv.bookmarksfly.cn

Ruby: // 手写 Hash
来源：http://lj.asd995.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ta.521024.cn

[N08] 生成全排列
来源：http://sn.nszjky.cn

Py:   itertools.permutations(arr)
来源：http://st.jianghongdianzi.cn

PHP:  // 手写递归交换
来源：http://gh.huixinmuqiang.cn

JS:   // 手写回溯递归
来源：http://pm.9csxet.cn

TS:   // 手写回溯递归
来源：http://ob.asd995.cn

Java: // 手写回溯递归
来源：http://eb.jctech888.com.cn

Go:   // 手写回溯递归
来源：http://gk.yuntaijiaju.cn

Ruby: arr.permutation.to_a
来源：http://bm.huixinmuqiang.cn

C#:   // 手写回溯递归
来源：http://mx.yuexingan06.cn

[N09] 栈与队列
来源：http://ui.lnxyls.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ia.521024.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ek.hahajie.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ib.newstarts.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mb.wgjwhj.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://xy.shxzukj.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://si.bjjhwx.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://sy.nicolike.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://og.chemitech.net.cn

[N10] 链表节点定义
来源：http://fe.szxytkj.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://dl.haigaiapp.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://vp.huixinmuqiang.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://xn.yuexingan06.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://qn.szxytkj.cn

Java: class Node { int v; Node next; }
来源：http://kg.nszjky.cn

Go:   type Node struct { V int; Next *Node }
来源：http://mg.gzmigu.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://nq.9csxet.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://vu.bjjhwx.cn

[N11] 二叉树中序遍历
来源：http://fz.shtwfgs.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://tq.szxytkj.cn

PHP:  // 手写递归函数
来源：http://lk.muxihuayi.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lx.gzmigu.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://un.shxzukj.cn

Java: // 手写递归
来源：http://bz.shtwfgs.cn

Go:   // 手写递归
来源：http://wi.yuexingan06.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://lr.wgjwhj.cn

C#:   // 手写递归
来源：http://uo.gzmigu.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://cm.gzmigu.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ob.bookmarksfly.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mb.bookmarksfly.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qj.yuexingan06.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zw.colortex.cn


<!-- 参考信息 -->