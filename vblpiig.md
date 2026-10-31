代发 wailian999

JS:   JSON.stringify(obj, null, 2)
来源：http://th.hnjuh.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://qg.jctech888.com.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://vu.shxzskj.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ur.panjiajie.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ha.gzmigu.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://bm.lnxyls.cn

[K04] 读取 JSON 文件
来源：http://rx.jianghongdianzi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ui.bookmarksfly.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://im.gzmigu.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zr.yuntaijiaju.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wd.gzmigu.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://uf.shxzukj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://sq.521024.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://kw.521024.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ii.jianghongdianzi.cn

[K05] 深拷贝对象
来源：http://le.chemitech.net.cn

Py:   copy.deepcopy(obj)
来源：http://zg.hahajie.cn

PHP:  unserialize(serialize($obj));
来源：http://gp.yuntaijiaju.cn

JS:   structuredClone(obj)
来源：http://mu.bookmarksfly.cn

TS:   structuredClone(obj)
来源：http://qy.nszjky.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://hq.nszjky.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://fd.chemitech.net.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://bm.huanxung.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://dd.colortex.cn

[K06] 解析 URL 查询串
来源：http://je.szxytkj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://dt.hahajie.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://sf.chemitech.net.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ta.muxihuayi.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tv.colortex.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://xx.colortex.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://yh.asd995.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://do.gzmigu.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://eg.haigaiapp.cn

[K07] 进制转换
来源：http://so.szxytkj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://fn.haigaiapp.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://kc.shxzskj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://up.huixinmuqiang.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://nc.huixinmuqiang.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://rz.jianghongdianzi.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ta.colortex.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ua.huixinmuqiang.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://pr.haigaiapp.cn

[K08] 二进制序列化（非 JSON）
来源：http://ah.hnjuh.cn

Py:   pickle.dumps(obj)
来源：http://gg.521024.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://xb.yuexingan06.cn

JS:   v8.serialize(obj)        // Node
来源：http://wq.huanxung.cn

TS:   v8.serialize(obj)        // Node
来源：http://ov.9csxet.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ye.yuntaijiaju.cn

Go:   encoding/gob
来源：http://rj.newstarts.cn

Ruby: Marshal.dump(obj)
来源：http://eu.shtwfgs.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ym.gzmigu.cn

================================================================================
来源：http://nv.shxzskj.cn

L. 网络请求
来源：http://pl.9csxet.cn

================================================================================
来源：http://hi.nicolike.cn

[L01] 发送 GET 请求
来源：http://vc.colortex.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://nr.wgjwhj.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://id.521024.cn

JS:   await fetch(url)
来源：http://ug.gzmigu.cn

TS:   await fetch(url)
来源：http://ig.colortex.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://kt.nszjky.cn

Go:   resp, err := http.Get(url)
来源：http://sm.haigaiapp.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://kb.newstarts.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ah.bookmarksfly.cn

[L02] 发送 POST JSON
来源：http://bw.muxihuayi.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ae.gzmigu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://zq.panjiajie.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nm.shtwfgs.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hh.newstarts.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://pr.panjiajie.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://xd.lnxyls.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://zu.shtwfgs.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xd.chemitech.net.cn

[L03] 设置自定义请求头
来源：http://pq.shxzukj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://je.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://dp.huanxung.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://uq.521024.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fw.colortex.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://tb.hahajie.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ll.shtwfgs.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://pg.wgjwhj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wx.jianghongdianzi.cn

[L04] 设置超时
来源：http://ge.shtwfgs.cn

Py:   requests.get(url, timeout=5)
来源：http://yd.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://jd.chemitech.net.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://av.521024.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://md.yuexingan06.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://aj.wgjwhj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ho.bjjhwx.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://sh.521024.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://nb.nszjky.cn

[L05] 上传文件（multipart）
来源：http://ey.asd995.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ae.521024.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://nj.hnjuh.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hw.hahajie.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ui.colortex.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ei.gzmigu.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://cn.asd995.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://pq.shtwfgs.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://tu.colortex.cn

[L06] 解析响应为 JSON
来源：http://sd.9csxet.cn

Py:   resp.json()
来源：http://fn.bjjhwx.cn

PHP:  json_decode($body, true);
来源：http://ay.jctech888.com.cn

JS:   await resp.json()
来源：http://oq.huixiangedu.cn

TS:   await resp.json()
来源：http://cm.haigaiapp.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://uv.szsharing.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ib.hnjuh.cn

Ruby: JSON.parse(resp.body)
来源：http://kr.bjjhwx.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ha.chemitech.net.cn

[L07] 处理 HTTP 状态码
来源：http://dq.asd995.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://pe.szsharing.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mx.chemitech.net.cn

JS:   resp.ok;  resp.status
来源：http://zh.chemitech.net.cn

TS:   resp.ok;  resp.status
来源：http://eb.huixinmuqiang.cn

Java: resp.statusCode()
来源：http://zg.nszjky.cn

Go:   resp.StatusCode
来源：http://rq.bookmarksfly.cn

Ruby: resp.code.to_i
来源：http://cs.szsharing.cn

C#:   (int)resp.StatusCode
来源：http://fg.jctech888.com.cn

[L08] 并发请求多个地址
来源：http://ft.haigaiapp.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://fj.hnjuh.cn

PHP:  curl_multi_init() 系列
来源：http://xx.huanxung.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sg.szsharing.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cn.szsharing.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ki.panjiajie.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://lp.muxihuayi.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://xu.chemitech.net.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ir.asd995.cn

================================================================================
来源：http://rc.panjiajie.cn

M. 命令行 / 进程 / 环境
来源：http://zb.wgjwhj.cn

================================================================================
来源：http://si.shxzskj.cn

[M01] 读取命令行参数
来源：http://ic.shtwfgs.cn

Py:   sys.argv[1:]
来源：http://ry.huixinmuqiang.cn

PHP:  $argv;  $argc;
来源：http://kz.colortex.cn

JS:   process.argv.slice(2)
来源：http://mg.shtwfgs.cn

TS:   process.argv.slice(2)
来源：http://bi.bookmarksfly.cn

Java: args 数组（main 方法参数）
来源：http://fq.wgjwhj.cn

Go:   os.Args[1:]
来源：http://rq.hnjuh.cn

Ruby: ARGV
来源：http://if.asd995.cn

C#:   args 数组（Main 方法参数）
来源：http://oe.szxytkj.cn

[M02] 读取环境变量
来源：http://xa.shxzskj.cn

Py:   os.environ.get("HOME")
来源：http://wt.nszjky.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rg.muxihuayi.cn

JS:   process.env.HOME
来源：http://io.gzmigu.cn

TS:   process.env.HOME
来源：http://tm.hnjuh.cn

Java: System.getenv("HOME")
来源：http://yo.jctech888.com.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://rm.chemitech.net.cn

Ruby: ENV["HOME"]
来源：http://np.huixinmuqiang.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://us.colortex.cn

[M03] 执行外部命令
来源：http://ws.szsharing.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://eu.szsharing.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mj.shxzukj.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://it.chemitech.net.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://or.newstarts.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.jctech888.com.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://gb.asd995.cn

Ruby: system("ls -l");  `ls -l`
来源：http://bl.colortex.cn

C#:   Process.Start("ls", "-l");
来源：http://ux.shtwfgs.cn

[M04] 获取当前工作目录
来源：http://jy.nicolike.cn

Py:   os.getcwd()
来源：http://mt.muxihuayi.cn

PHP:  getcwd();
来源：http://fj.wgjwhj.cn

JS:   process.cwd()
来源：http://kn.bookmarksfly.cn

TS:   process.cwd()
来源：http://sj.szxytkj.cn

Java: Path.of("").toAbsolutePath()
来源：http://xy.panjiajie.cn

Go:   os.Getwd()
来源：http://ge.521024.cn

Ruby: Dir.pwd
来源：http://rh.nicolike.cn

C#:   Directory.GetCurrentDirectory()
来源：http://jj.huanxung.cn

[M05] 设置退出码
来源：http://js.gzmigu.cn

Py:   sys.exit(1)
来源：http://ff.shtwfgs.cn

PHP:  exit(1);
来源：http://cy.gzmigu.cn

JS:   process.exit(1)
来源：http://xk.lnxyls.cn

TS:   process.exit(1)
来源：http://kl.gzmigu.cn

Java: System.exit(1)
来源：http://yx.shxzskj.cn

Go:   os.Exit(1)
来源：http://tj.newstarts.cn

Ruby: exit 1
来源：http://mi.bjjhwx.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://up.huanxung.cn

[M06] 向标准错误输出
来源：http://th.newstarts.cn

Py:   print("err", file=sys.stderr)
来源：http://bf.jctech888.com.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://me.gzmigu.cn

JS:   console.error("err")
来源：http://ys.wgjwhj.cn

TS:   console.error("err")
来源：http://po.521024.cn

Java: System.err.println("err")
来源：http://jv.521024.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://um.bookmarksfly.cn

Ruby: warn "err"
来源：http://ib.jctech888.com.cn

C#:   Console.Error.WriteLine("err")
来源：http://xt.wgjwhj.cn

[M07] 判断是否为主入口
来源：http://ie.yuntaijiaju.cn

Py:   if __name__ == "__main__":
来源：http://tr.wgjwhj.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ir.asd995.cn

JS:   require.main === module
来源：http://ut.bookmarksfly.cn

TS:   require.main === module
来源：http://ii.bookmarksfly.cn

Java: public static void main(String[] args)
来源：http://ac.shtwfgs.cn

Go:   func main()
来源：http://lf.nicolike.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ip.nszjky.cn

C#:   static void Main(string[] args)
来源：http://rv.521024.cn

[M08] 获取系统与运行时信息
来源：http://cv.shxzukj.cn

Py:   platform.system();  platform.python_version()
来源：http://in.wgjwhj.cn

PHP:  PHP_OS;  phpversion();
来源：http://tc.jctech888.com.cn

JS:   process.platform;  process.version
来源：http://by.huixinmuqiang.cn

TS:   process.platform;  process.version
来源：http://re.szxytkj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://fa.521024.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ui.yuntaijiaju.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://kt.gzmigu.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://uq.bjjhwx.cn

================================================================================
来源：http://ld.szsharing.cn

N. 数据结构与算法
来源：http://bp.nszjky.cn

================================================================================
来源：http://uz.muxihuayi.cn

[N01] 二分查找（有序数组）
来源：http://cl.bookmarksfly.cn

Py:   bisect.bisect_left(arr, x)
来源：http://mf.szsharing.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://yk.521024.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jq.chemitech.net.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://oz.gzmigu.cn

Java: Arrays.binarySearch(arr, x)
来源：http://us.panjiajie.cn

Go:   sort.SearchInts(arr, x)
来源：http://yg.haigaiapp.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://kx.nicolike.cn

C#:   Array.BinarySearch(arr, x)
来源：http://qa.jctech888.com.cn

[N02] 排序（工程实践用内置实现）
来源：http://en.521024.cn

Py:   sorted(arr);  arr.sort()
来源：http://kw.nicolike.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hb.wgjwhj.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://pg.szsharing.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://dz.jianghongdianzi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://fg.jianghongdianzi.cn

Go:   slices.Sort(arr)
来源：http://sl.521024.cn

Ruby: arr.sort
来源：http://ft.asd995.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://od.bjjhwx.cn

[N03] 快速排序（分治示例）
来源：http://dl.newstarts.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://lq.szsharing.cn

PHP:  // 递归实现，或用 usort
来源：http://sw.nszjky.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tn.asd995.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bp.chemitech.net.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://kd.shxzukj.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://pl.chemitech.net.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://du.chemitech.net.cn

C#:   // 手写递归，或 Array.Sort
来源：http://xy.shtwfgs.cn

[N04] 斐波那契数列
来源：http://ny.wgjwhj.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://xz.huixiangedu.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://vv.huixiangedu.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zr.bookmarksfly.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://oj.huanxung.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://gm.chemitech.net.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ep.yuexingan06.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://zp.muxihuayi.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://kd.nszjky.cn

[N05] 最大公约数
来源：http://lo.asd995.cn

Py:   math.gcd(a, b)
来源：http://xz.521024.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://vc.hnjuh.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://eq.szxytkj.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ku.huixiangedu.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://nt.shxzukj.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://jb.szxytkj.cn

Ruby: a.gcd(b)
来源：http://xe.shxzukj.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://pt.9csxet.cn

[N06] 判断回文字符串
来源：http://hl.shxzukj.cn

Py:   s == s[::-1]
来源：http://zg.shxzskj.cn

PHP:  $s === strrev($s);
来源：http://xr.shtwfgs.cn

JS:   s === [...s].reverse().join("")
来源：http://gn.szsharing.cn

TS:   s === [...s].reverse().join("")
来源：http://qx.hnjuh.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://vx.huanxung.cn

Go:   // 双指针从两端比较
来源：http://ed.newstarts.cn

Ruby: s == s.reverse
来源：http://tw.hahajie.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ih.szsharing.cn

[N07] 两数之和（返回下标）
来源：http://oz.szxytkj.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://po.yuexingan06.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://gk.bookmarksfly.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://nm.shxzskj.cn

TS:   // 手写 Map<string, number>
来源：http://sk.wgjwhj.cn

Java: // 手写 HashMap
来源：http://hs.szsharing.cn

Go:   // 手写 map[int]int
来源：http://dn.huanxung.cn

Ruby: // 手写 Hash
来源：http://oc.newstarts.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ep.yuexingan06.cn

[N08] 生成全排列
来源：http://jc.lnxyls.cn

Py:   itertools.permutations(arr)
来源：http://at.bookmarksfly.cn

PHP:  // 手写递归交换
来源：http://re.shxzukj.cn

JS:   // 手写回溯递归
来源：http://kv.bookmarksfly.cn

TS:   // 手写回溯递归
来源：http://cy.lnxyls.cn

Java: // 手写回溯递归
来源：http://dm.jctech888.com.cn

Go:   // 手写回溯递归
来源：http://mr.gzmigu.cn

Ruby: arr.permutation.to_a
来源：http://yu.asd995.cn

C#:   // 手写回溯递归
来源：http://dk.gzmigu.cn

[N09] 栈与队列
来源：http://mw.jctech888.com.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://fj.shxzskj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://xp.huanxung.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ki.szsharing.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ne.yuntaijiaju.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://tg.lnxyls.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hv.nicolike.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://lg.haigaiapp.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ti.bookmarksfly.cn

[N10] 链表节点定义
来源：http://yw.yuntaijiaju.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://tg.haigaiapp.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://wc.lnxyls.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://sr.521024.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ze.colortex.cn

Java: class Node { int v; Node next; }
来源：http://nb.bjjhwx.cn

Go:   type Node struct { V int; Next *Node }
来源：http://nh.bjjhwx.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ym.9csxet.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ih.asd995.cn

[N11] 二叉树中序遍历
来源：http://cb.bookmarksfly.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://nv.lnxyls.cn

PHP:  // 手写递归函数
来源：http://fb.haigaiapp.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ts.asd995.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qv.shxzskj.cn

Java: // 手写递归
来源：http://uu.521024.cn


<!-- 参考信息 -->