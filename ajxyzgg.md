代发 wailian999

Ruby: JSON.pretty_generate(obj)
来源：http://tx.nszjky.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ey.szsharing.cn

[K04] 读取 JSON 文件
来源：http://vo.szxytkj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ye.shxzskj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://xn.asd995.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ae.yuntaijiaju.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fs.huixiangedu.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://zt.shxzskj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://xo.szxytkj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://yj.szxytkj.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ec.9csxet.cn

[K05] 深拷贝对象
来源：http://es.nszjky.cn

Py:   copy.deepcopy(obj)
来源：http://el.hnjuh.cn

PHP:  unserialize(serialize($obj));
来源：http://oe.muxihuayi.cn

JS:   structuredClone(obj)
来源：http://bi.wgjwhj.cn

TS:   structuredClone(obj)
来源：http://pt.bjjhwx.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://dz.bookmarksfly.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://jl.521024.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hl.haigaiapp.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://bw.asd995.cn

[K06] 解析 URL 查询串
来源：http://hu.wgjwhj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ww.yuntaijiaju.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ad.nicolike.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ce.bookmarksfly.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ne.lnxyls.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://kc.hnjuh.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://de.hahajie.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://zm.gzmigu.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wk.chemitech.net.cn

[K07] 进制转换
来源：http://lf.shxzukj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://fs.shxzukj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ca.lnxyls.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://we.panjiajie.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://lq.shxzukj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://aq.szxytkj.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://vr.bookmarksfly.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ut.jianghongdianzi.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://lw.lnxyls.cn

[K08] 二进制序列化（非 JSON）
来源：http://vk.wgjwhj.cn

Py:   pickle.dumps(obj)
来源：http://co.szsharing.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://xx.hahajie.cn

JS:   v8.serialize(obj)        // Node
来源：http://gy.haigaiapp.cn

TS:   v8.serialize(obj)        // Node
来源：http://eg.szxytkj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://vy.gzmigu.cn

Go:   encoding/gob
来源：http://xu.bjjhwx.cn

Ruby: Marshal.dump(obj)
来源：http://gv.yuexingan06.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://yc.hahajie.cn

================================================================================
来源：http://yt.shtwfgs.cn

L. 网络请求
来源：http://lo.huixiangedu.cn

================================================================================
来源：http://lb.jianghongdianzi.cn

[L01] 发送 GET 请求
来源：http://uv.jctech888.com.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://sq.colortex.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vc.szxytkj.cn

JS:   await fetch(url)
来源：http://rp.yuexingan06.cn

TS:   await fetch(url)
来源：http://sh.bjjhwx.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://jm.bookmarksfly.cn

Go:   resp, err := http.Get(url)
来源：http://pg.panjiajie.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://hk.jctech888.com.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://cy.bookmarksfly.cn

[L02] 发送 POST JSON
来源：http://lm.gzmigu.cn

Py:   requests.post(url, json={"a": 1})
来源：http://uu.nszjky.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ld.panjiajie.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vg.bjjhwx.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zy.jctech888.com.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://zq.huixiangedu.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wf.huixinmuqiang.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://sb.bookmarksfly.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ws.lnxyls.cn

[L03] 设置自定义请求头
来源：http://po.hnjuh.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://qa.gzmigu.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://qn.shxzskj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://aw.hahajie.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hb.shxzskj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://yl.hahajie.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://kn.521024.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wc.bookmarksfly.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://vx.szsharing.cn

[L04] 设置超时
来源：http://hu.hahajie.cn

Py:   requests.get(url, timeout=5)
来源：http://fo.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xs.hahajie.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dv.hnjuh.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xo.asd995.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hy.bookmarksfly.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hr.newstarts.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://xh.haigaiapp.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hk.wgjwhj.cn

[L05] 上传文件（multipart）
来源：http://vd.colortex.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://fx.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://rj.szxytkj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://tp.jctech888.com.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ol.huanxung.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://gu.nszjky.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://fv.lnxyls.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://nz.panjiajie.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ij.wgjwhj.cn

[L06] 解析响应为 JSON
来源：http://os.panjiajie.cn

Py:   resp.json()
来源：http://ec.panjiajie.cn

PHP:  json_decode($body, true);
来源：http://vw.newstarts.cn

JS:   await resp.json()
来源：http://wx.bjjhwx.cn

TS:   await resp.json()
来源：http://rz.nicolike.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://pb.szxytkj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://zd.asd995.cn

Ruby: JSON.parse(resp.body)
来源：http://zw.szsharing.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ks.gzmigu.cn

[L07] 处理 HTTP 状态码
来源：http://ba.szsharing.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://yw.9csxet.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://gu.hnjuh.cn

JS:   resp.ok;  resp.status
来源：http://ou.bookmarksfly.cn

TS:   resp.ok;  resp.status
来源：http://ds.hahajie.cn

Java: resp.statusCode()
来源：http://nw.lnxyls.cn

Go:   resp.StatusCode
来源：http://od.huanxung.cn

Ruby: resp.code.to_i
来源：http://oc.521024.cn

C#:   (int)resp.StatusCode
来源：http://zj.colortex.cn

[L08] 并发请求多个地址
来源：http://gd.muxihuayi.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://dq.bookmarksfly.cn

PHP:  curl_multi_init() 系列
来源：http://ct.yuntaijiaju.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sn.huixiangedu.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zh.jianghongdianzi.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wl.9csxet.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://fc.jctech888.com.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://tn.jianghongdianzi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://iw.yuntaijiaju.cn

================================================================================
来源：http://lj.bookmarksfly.cn

M. 命令行 / 进程 / 环境
来源：http://wd.wgjwhj.cn

================================================================================
来源：http://cc.wgjwhj.cn

[M01] 读取命令行参数
来源：http://dq.szsharing.cn

Py:   sys.argv[1:]
来源：http://ih.chemitech.net.cn

PHP:  $argv;  $argc;
来源：http://lv.huanxung.cn

JS:   process.argv.slice(2)
来源：http://gj.newstarts.cn

TS:   process.argv.slice(2)
来源：http://ij.shtwfgs.cn

Java: args 数组（main 方法参数）
来源：http://th.wgjwhj.cn

Go:   os.Args[1:]
来源：http://zw.shxzskj.cn

Ruby: ARGV
来源：http://kr.colortex.cn

C#:   args 数组（Main 方法参数）
来源：http://od.jctech888.com.cn

[M02] 读取环境变量
来源：http://bw.9csxet.cn

Py:   os.environ.get("HOME")
来源：http://nr.hnjuh.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://so.nicolike.cn

JS:   process.env.HOME
来源：http://cn.asd995.cn

TS:   process.env.HOME
来源：http://lv.shxzukj.cn

Java: System.getenv("HOME")
来源：http://jo.huanxung.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://se.shtwfgs.cn

Ruby: ENV["HOME"]
来源：http://sc.yuexingan06.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://uw.521024.cn

[M03] 执行外部命令
来源：http://hr.bookmarksfly.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://gv.bookmarksfly.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://sx.huanxung.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://th.lnxyls.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://sf.newstarts.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://xh.panjiajie.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://om.huixiangedu.cn

Ruby: system("ls -l");  `ls -l`
来源：http://cy.huixinmuqiang.cn

C#:   Process.Start("ls", "-l");
来源：http://pz.szsharing.cn

[M04] 获取当前工作目录
来源：http://vg.jianghongdianzi.cn

Py:   os.getcwd()
来源：http://om.bookmarksfly.cn

PHP:  getcwd();
来源：http://pu.huixinmuqiang.cn

JS:   process.cwd()
来源：http://dc.asd995.cn

TS:   process.cwd()
来源：http://wm.jianghongdianzi.cn

Java: Path.of("").toAbsolutePath()
来源：http://zh.hnjuh.cn

Go:   os.Getwd()
来源：http://as.chemitech.net.cn

Ruby: Dir.pwd
来源：http://dm.shxzskj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://os.asd995.cn

[M05] 设置退出码
来源：http://id.521024.cn

Py:   sys.exit(1)
来源：http://qv.shtwfgs.cn

PHP:  exit(1);
来源：http://mj.shxzskj.cn

JS:   process.exit(1)
来源：http://wa.wgjwhj.cn

TS:   process.exit(1)
来源：http://lr.muxihuayi.cn

Java: System.exit(1)
来源：http://vp.9csxet.cn

Go:   os.Exit(1)
来源：http://xe.521024.cn

Ruby: exit 1
来源：http://pw.shxzskj.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://vu.colortex.cn

[M06] 向标准错误输出
来源：http://uh.nszjky.cn

Py:   print("err", file=sys.stderr)
来源：http://dy.wgjwhj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ya.panjiajie.cn

JS:   console.error("err")
来源：http://mo.jctech888.com.cn

TS:   console.error("err")
来源：http://me.panjiajie.cn

Java: System.err.println("err")
来源：http://vy.gzmigu.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://pc.asd995.cn

Ruby: warn "err"
来源：http://ls.szxytkj.cn

C#:   Console.Error.WriteLine("err")
来源：http://bo.bookmarksfly.cn

[M07] 判断是否为主入口
来源：http://gp.yuntaijiaju.cn

Py:   if __name__ == "__main__":
来源：http://et.hahajie.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://cx.huanxung.cn

JS:   require.main === module
来源：http://it.lnxyls.cn

TS:   require.main === module
来源：http://pj.yuexingan06.cn

Java: public static void main(String[] args)
来源：http://rj.hnjuh.cn

Go:   func main()
来源：http://ic.colortex.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://fr.lnxyls.cn

C#:   static void Main(string[] args)
来源：http://ab.521024.cn

[M08] 获取系统与运行时信息
来源：http://ue.huanxung.cn

Py:   platform.system();  platform.python_version()
来源：http://sp.panjiajie.cn

PHP:  PHP_OS;  phpversion();
来源：http://ig.chemitech.net.cn

JS:   process.platform;  process.version
来源：http://va.shxzskj.cn

TS:   process.platform;  process.version
来源：http://ot.szxytkj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mf.nszjky.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://dy.yuntaijiaju.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://qf.szsharing.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://hr.hahajie.cn

================================================================================
来源：http://jf.521024.cn

N. 数据结构与算法
来源：http://tb.bjjhwx.cn

================================================================================
来源：http://dr.bjjhwx.cn

[N01] 二分查找（有序数组）
来源：http://oi.newstarts.cn

Py:   bisect.bisect_left(arr, x)
来源：http://sx.nszjky.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://nk.wgjwhj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://iq.nszjky.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fq.huixiangedu.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ok.yuexingan06.cn

Go:   sort.SearchInts(arr, x)
来源：http://td.jianghongdianzi.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://xp.wgjwhj.cn

C#:   Array.BinarySearch(arr, x)
来源：http://sa.lnxyls.cn

[N02] 排序（工程实践用内置实现）
来源：http://yw.shtwfgs.cn

Py:   sorted(arr);  arr.sort()
来源：http://yi.newstarts.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://il.nicolike.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://nm.panjiajie.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://wl.521024.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://cq.nicolike.cn

Go:   slices.Sort(arr)
来源：http://sz.colortex.cn

Ruby: arr.sort
来源：http://bo.lnxyls.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://up.shtwfgs.cn

[N03] 快速排序（分治示例）
来源：http://ba.asd995.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://sc.yuntaijiaju.cn

PHP:  // 递归实现，或用 usort
来源：http://rk.wgjwhj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rx.szxytkj.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nu.colortex.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://gq.newstarts.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mr.chemitech.net.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://yw.nicolike.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ym.huanxung.cn

[N04] 斐波那契数列
来源：http://za.jianghongdianzi.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://bv.panjiajie.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://oh.gzmigu.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jr.muxihuayi.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://to.shxzukj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://la.lnxyls.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://pe.jianghongdianzi.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://um.szsharing.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://zj.shxzskj.cn

[N05] 最大公约数
来源：http://pu.chemitech.net.cn

Py:   math.gcd(a, b)
来源：http://yi.nicolike.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ql.521024.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wh.yuntaijiaju.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gk.shxzskj.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://yw.szsharing.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ku.bookmarksfly.cn

Ruby: a.gcd(b)
来源：http://fa.hnjuh.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://yg.asd995.cn

[N06] 判断回文字符串
来源：http://jr.wgjwhj.cn

Py:   s == s[::-1]
来源：http://um.huanxung.cn

PHP:  $s === strrev($s);
来源：http://mh.yuexingan06.cn

JS:   s === [...s].reverse().join("")
来源：http://bb.bjjhwx.cn

TS:   s === [...s].reverse().join("")
来源：http://hm.shxzskj.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://lv.yuntaijiaju.cn

Go:   // 双指针从两端比较
来源：http://rl.lnxyls.cn

Ruby: s == s.reverse
来源：http://xa.huanxung.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://mv.gzmigu.cn

[N07] 两数之和（返回下标）
来源：http://sp.bjjhwx.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://kz.shxzskj.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ly.hnjuh.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://la.shxzskj.cn

TS:   // 手写 Map<string, number>
来源：http://jh.lnxyls.cn

Java: // 手写 HashMap
来源：http://nd.muxihuayi.cn

Go:   // 手写 map[int]int
来源：http://zy.wgjwhj.cn

Ruby: // 手写 Hash
来源：http://hu.nszjky.cn

C#:   // 手写 Dictionary<int, int>
来源：http://tm.hahajie.cn

[N08] 生成全排列
来源：http://us.asd995.cn

Py:   itertools.permutations(arr)
来源：http://mm.lnxyls.cn

PHP:  // 手写递归交换
来源：http://sh.muxihuayi.cn

JS:   // 手写回溯递归
来源：http://yu.huixinmuqiang.cn

TS:   // 手写回溯递归
来源：http://aq.wgjwhj.cn

Java: // 手写回溯递归
来源：http://ra.nszjky.cn

Go:   // 手写回溯递归
来源：http://ic.hahajie.cn

Ruby: arr.permutation.to_a
来源：http://so.nicolike.cn

C#:   // 手写回溯递归
来源：http://ty.jianghongdianzi.cn

[N09] 栈与队列
来源：http://cy.yuntaijiaju.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://oc.wgjwhj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://gr.gzmigu.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://jp.jianghongdianzi.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ii.hahajie.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://th.huanxung.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.jctech888.com.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://cp.hnjuh.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://bx.huixinmuqiang.cn

[N10] 链表节点定义
来源：http://mw.yuexingan06.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://jj.shtwfgs.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://vn.haigaiapp.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://xy.muxihuayi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://cp.jianghongdianzi.cn

Java: class Node { int v; Node next; }
来源：http://ul.yuntaijiaju.cn

Go:   type Node struct { V int; Next *Node }
来源：http://cp.asd995.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://sz.szsharing.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://dv.521024.cn

[N11] 二叉树中序遍历
来源：http://xs.newstarts.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://sx.bookmarksfly.cn

PHP:  // 手写递归函数
来源：http://nr.bookmarksfly.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bh.muxihuayi.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yl.jctech888.com.cn

Java: // 手写递归
来源：http://el.haigaiapp.cn

Go:   // 手写递归
来源：http://tn.bjjhwx.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://qc.lnxyls.cn

C#:   // 手写递归
来源：http://fo.asd995.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://fv.shxzskj.cn


<!-- 参考信息 -->