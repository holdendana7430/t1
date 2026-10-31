代发 wailian999

TS:   JSON.parse(s)
来源：http://za.gzmigu.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://gg.jianghongdianzi.cn

Go:   json.Unmarshal(data, &v)
来源：http://xo.huixinmuqiang.cn

Ruby: JSON.parse(s)
来源：http://ah.gzmigu.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://gx.yuntaijiaju.cn

[K03] JSON 美化输出（带缩进）
来源：http://jp.nszjky.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://sz.haigaiapp.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://pv.shtwfgs.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://cn.huixinmuqiang.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://hu.bjjhwx.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://io.yuntaijiaju.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://lp.gzmigu.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ts.9csxet.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ml.hnjuh.cn

[K04] 读取 JSON 文件
来源：http://hq.lnxyls.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://xm.yuntaijiaju.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://xh.panjiajie.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://oc.bjjhwx.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wx.colortex.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://pn.jianghongdianzi.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://fh.yuntaijiaju.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ga.hahajie.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://bb.muxihuayi.cn

[K05] 深拷贝对象
来源：http://ec.wgjwhj.cn

Py:   copy.deepcopy(obj)
来源：http://sa.szxytkj.cn

PHP:  unserialize(serialize($obj));
来源：http://ay.jianghongdianzi.cn

JS:   structuredClone(obj)
来源：http://gq.9csxet.cn

TS:   structuredClone(obj)
来源：http://bh.asd995.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://it.colortex.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://lf.newstarts.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://iv.shxzukj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://dn.colortex.cn

[K06] 解析 URL 查询串
来源：http://zf.bjjhwx.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://qe.521024.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ml.yuexingan06.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nz.asd995.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sn.asd995.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://zv.colortex.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://kc.chemitech.net.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://da.wgjwhj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://iw.gzmigu.cn

[K07] 进制转换
来源：http://my.panjiajie.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://yj.wgjwhj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ub.jianghongdianzi.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://cy.muxihuayi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ax.hahajie.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://lt.muxihuayi.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://he.nszjky.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://dn.szsharing.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://oz.szxytkj.cn

[K08] 二进制序列化（非 JSON）
来源：http://bw.hahajie.cn

Py:   pickle.dumps(obj)
来源：http://pz.newstarts.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://bt.shxzskj.cn

JS:   v8.serialize(obj)        // Node
来源：http://ez.hahajie.cn

TS:   v8.serialize(obj)        // Node
来源：http://mh.521024.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://qz.haigaiapp.cn

Go:   encoding/gob
来源：http://zx.bookmarksfly.cn

Ruby: Marshal.dump(obj)
来源：http://bv.newstarts.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://me.asd995.cn

================================================================================
来源：http://dr.panjiajie.cn

L. 网络请求
来源：http://zb.haigaiapp.cn

================================================================================
来源：http://ek.colortex.cn

[L01] 发送 GET 请求
来源：http://cn.yuntaijiaju.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://uy.shtwfgs.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ur.muxihuayi.cn

JS:   await fetch(url)
来源：http://bu.huanxung.cn

TS:   await fetch(url)
来源：http://cs.jctech888.com.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://iy.muxihuayi.cn

Go:   resp, err := http.Get(url)
来源：http://hk.huixinmuqiang.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://yy.chemitech.net.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://fq.jctech888.com.cn

[L02] 发送 POST JSON
来源：http://da.yuexingan06.cn

Py:   requests.post(url, json={"a": 1})
来源：http://oi.panjiajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://rw.bookmarksfly.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zz.muxihuayi.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fz.huixinmuqiang.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://nh.shxzskj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://kw.huixinmuqiang.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://at.shtwfgs.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://sy.hnjuh.cn

[L03] 设置自定义请求头
来源：http://op.hnjuh.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://bf.gzmigu.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://fh.shxzskj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lq.haigaiapp.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yv.haigaiapp.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://dh.jctech888.com.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jo.panjiajie.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mp.shxzukj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://dv.panjiajie.cn

[L04] 设置超时
来源：http://vm.bookmarksfly.cn

Py:   requests.get(url, timeout=5)
来源：http://dl.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ef.shtwfgs.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://om.hahajie.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yb.jctech888.com.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qh.colortex.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wc.szsharing.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://xu.shxzukj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://vc.panjiajie.cn

[L05] 上传文件（multipart）
来源：http://bh.shtwfgs.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://nm.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://fd.asd995.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://cq.huixiangedu.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://rk.9csxet.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ee.colortex.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://rq.bookmarksfly.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ve.colortex.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://kw.szxytkj.cn

[L06] 解析响应为 JSON
来源：http://dn.newstarts.cn

Py:   resp.json()
来源：http://th.asd995.cn

PHP:  json_decode($body, true);
来源：http://fw.nicolike.cn

JS:   await resp.json()
来源：http://rt.nszjky.cn

TS:   await resp.json()
来源：http://tf.jctech888.com.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://aw.colortex.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://al.colortex.cn

Ruby: JSON.parse(resp.body)
来源：http://dn.huixinmuqiang.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ay.bjjhwx.cn

[L07] 处理 HTTP 状态码
来源：http://lu.hnjuh.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://vk.521024.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://oj.muxihuayi.cn

JS:   resp.ok;  resp.status
来源：http://xy.shxzskj.cn

TS:   resp.ok;  resp.status
来源：http://mf.shtwfgs.cn

Java: resp.statusCode()
来源：http://ye.bjjhwx.cn

Go:   resp.StatusCode
来源：http://jf.wgjwhj.cn

Ruby: resp.code.to_i
来源：http://mz.yuexingan06.cn

C#:   (int)resp.StatusCode
来源：http://tx.haigaiapp.cn

[L08] 并发请求多个地址
来源：http://gt.asd995.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://pt.wgjwhj.cn

PHP:  curl_multi_init() 系列
来源：http://ue.jctech888.com.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sf.hnjuh.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xe.chemitech.net.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://kp.newstarts.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://fj.521024.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://gp.hahajie.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://vk.asd995.cn

================================================================================
来源：http://yw.bjjhwx.cn

M. 命令行 / 进程 / 环境
来源：http://gv.asd995.cn

================================================================================
来源：http://my.yuexingan06.cn

[M01] 读取命令行参数
来源：http://wn.nicolike.cn

Py:   sys.argv[1:]
来源：http://qn.colortex.cn

PHP:  $argv;  $argc;
来源：http://vu.shxzskj.cn

JS:   process.argv.slice(2)
来源：http://hc.wgjwhj.cn

TS:   process.argv.slice(2)
来源：http://rk.asd995.cn

Java: args 数组（main 方法参数）
来源：http://ye.yuexingan06.cn

Go:   os.Args[1:]
来源：http://is.huanxung.cn

Ruby: ARGV
来源：http://tx.jianghongdianzi.cn

C#:   args 数组（Main 方法参数）
来源：http://du.shtwfgs.cn

[M02] 读取环境变量
来源：http://yc.shtwfgs.cn

Py:   os.environ.get("HOME")
来源：http://ax.lnxyls.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ee.huanxung.cn

JS:   process.env.HOME
来源：http://tf.colortex.cn

TS:   process.env.HOME
来源：http://ic.shxzskj.cn

Java: System.getenv("HOME")
来源：http://tu.shxzskj.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ek.asd995.cn

Ruby: ENV["HOME"]
来源：http://pw.newstarts.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://px.shxzukj.cn

[M03] 执行外部命令
来源：http://ra.shxzukj.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://zy.colortex.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://re.yuexingan06.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://yv.haigaiapp.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ne.nszjky.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://rj.521024.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://pn.panjiajie.cn

Ruby: system("ls -l");  `ls -l`
来源：http://nw.9csxet.cn

C#:   Process.Start("ls", "-l");
来源：http://xs.szxytkj.cn

[M04] 获取当前工作目录
来源：http://ud.szsharing.cn

Py:   os.getcwd()
来源：http://tb.jctech888.com.cn

PHP:  getcwd();
来源：http://zm.asd995.cn

JS:   process.cwd()
来源：http://kh.huanxung.cn

TS:   process.cwd()
来源：http://ey.521024.cn

Java: Path.of("").toAbsolutePath()
来源：http://so.haigaiapp.cn

Go:   os.Getwd()
来源：http://vq.jctech888.com.cn

Ruby: Dir.pwd
来源：http://rg.newstarts.cn

C#:   Directory.GetCurrentDirectory()
来源：http://xz.shxzskj.cn

[M05] 设置退出码
来源：http://bw.nszjky.cn

Py:   sys.exit(1)
来源：http://wl.gzmigu.cn

PHP:  exit(1);
来源：http://eb.huixinmuqiang.cn

JS:   process.exit(1)
来源：http://qb.bookmarksfly.cn

TS:   process.exit(1)
来源：http://os.wgjwhj.cn

Java: System.exit(1)
来源：http://dz.szxytkj.cn

Go:   os.Exit(1)
来源：http://uc.wgjwhj.cn

Ruby: exit 1
来源：http://uj.bjjhwx.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://jl.yuexingan06.cn

[M06] 向标准错误输出
来源：http://rd.9csxet.cn

Py:   print("err", file=sys.stderr)
来源：http://sw.muxihuayi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://oq.huixiangedu.cn

JS:   console.error("err")
来源：http://dd.bjjhwx.cn

TS:   console.error("err")
来源：http://vb.9csxet.cn

Java: System.err.println("err")
来源：http://zr.hnjuh.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://pe.szxytkj.cn

Ruby: warn "err"
来源：http://fa.szsharing.cn

C#:   Console.Error.WriteLine("err")
来源：http://xy.wgjwhj.cn

[M07] 判断是否为主入口
来源：http://nv.lnxyls.cn

Py:   if __name__ == "__main__":
来源：http://yh.colortex.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://up.lnxyls.cn

JS:   require.main === module
来源：http://pp.huixiangedu.cn

TS:   require.main === module
来源：http://kj.huanxung.cn

Java: public static void main(String[] args)
来源：http://lo.szsharing.cn

Go:   func main()
来源：http://zs.shxzukj.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://rf.bookmarksfly.cn

C#:   static void Main(string[] args)
来源：http://no.szxytkj.cn

[M08] 获取系统与运行时信息
来源：http://ad.newstarts.cn

Py:   platform.system();  platform.python_version()
来源：http://vz.shxzukj.cn

PHP:  PHP_OS;  phpversion();
来源：http://eg.lnxyls.cn

JS:   process.platform;  process.version
来源：http://nn.521024.cn

TS:   process.platform;  process.version
来源：http://gf.lnxyls.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://fn.yuexingan06.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://nf.shxzskj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://kw.panjiajie.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://kw.521024.cn

================================================================================
来源：http://nl.shtwfgs.cn

N. 数据结构与算法
来源：http://fw.asd995.cn

================================================================================
来源：http://yb.bjjhwx.cn

[N01] 二分查找（有序数组）
来源：http://zt.bjjhwx.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ui.yuntaijiaju.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://nu.shxzskj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fk.jianghongdianzi.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://oe.yuntaijiaju.cn

Java: Arrays.binarySearch(arr, x)
来源：http://cx.chemitech.net.cn

Go:   sort.SearchInts(arr, x)
来源：http://nq.panjiajie.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://cd.jctech888.com.cn

C#:   Array.BinarySearch(arr, x)
来源：http://qs.bookmarksfly.cn

[N02] 排序（工程实践用内置实现）
来源：http://iy.lnxyls.cn

Py:   sorted(arr);  arr.sort()
来源：http://ux.hnjuh.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://rp.chemitech.net.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ir.newstarts.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://gw.newstarts.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://rz.huixinmuqiang.cn

Go:   slices.Sort(arr)
来源：http://la.521024.cn

Ruby: arr.sort
来源：http://qa.lnxyls.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ca.wgjwhj.cn

[N03] 快速排序（分治示例）
来源：http://xw.nicolike.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://jt.shxzukj.cn

PHP:  // 递归实现，或用 usort
来源：http://ew.jctech888.com.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://es.hahajie.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://iz.nicolike.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ri.huixiangedu.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://lj.colortex.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://vl.yuexingan06.cn

C#:   // 手写递归，或 Array.Sort
来源：http://qv.hahajie.cn

[N04] 斐波那契数列
来源：http://el.haigaiapp.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wv.9csxet.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://av.9csxet.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qe.hnjuh.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://eh.9csxet.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://jx.yuntaijiaju.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ed.panjiajie.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wb.9csxet.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://jq.colortex.cn

[N05] 最大公约数
来源：http://os.szxytkj.cn

Py:   math.gcd(a, b)
来源：http://rf.huixinmuqiang.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ur.huixiangedu.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zu.colortex.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://me.shxzskj.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://kr.huixinmuqiang.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://al.szxytkj.cn

Ruby: a.gcd(b)
来源：http://dj.gzmigu.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://pj.huixiangedu.cn

[N06] 判断回文字符串
来源：http://ae.szxytkj.cn

Py:   s == s[::-1]
来源：http://lb.nszjky.cn

PHP:  $s === strrev($s);
来源：http://ws.huanxung.cn

JS:   s === [...s].reverse().join("")
来源：http://lz.shtwfgs.cn

TS:   s === [...s].reverse().join("")
来源：http://xl.shxzukj.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://lv.shxzskj.cn

Go:   // 双指针从两端比较
来源：http://bs.hnjuh.cn

Ruby: s == s.reverse
来源：http://ox.huixinmuqiang.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ch.bookmarksfly.cn

[N07] 两数之和（返回下标）
来源：http://qs.colortex.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://er.hahajie.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://yu.wgjwhj.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://nc.jctech888.com.cn

TS:   // 手写 Map<string, number>
来源：http://uq.szsharing.cn

Java: // 手写 HashMap
来源：http://ql.nicolike.cn

Go:   // 手写 map[int]int
来源：http://ej.shxzskj.cn

Ruby: // 手写 Hash
来源：http://hd.newstarts.cn

C#:   // 手写 Dictionary<int, int>
来源：http://nu.huixinmuqiang.cn

[N08] 生成全排列
来源：http://yl.huixinmuqiang.cn

Py:   itertools.permutations(arr)
来源：http://uo.huixinmuqiang.cn

PHP:  // 手写递归交换
来源：http://ks.wgjwhj.cn

JS:   // 手写回溯递归
来源：http://nw.nszjky.cn

TS:   // 手写回溯递归
来源：http://eb.jctech888.com.cn

Java: // 手写回溯递归
来源：http://xb.szsharing.cn

Go:   // 手写回溯递归
来源：http://ag.szsharing.cn

Ruby: arr.permutation.to_a
来源：http://qt.521024.cn

C#:   // 手写回溯递归
来源：http://ie.shxzskj.cn

[N09] 栈与队列
来源：http://nb.yuntaijiaju.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://qp.hahajie.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://pq.shxzskj.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://xl.asd995.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://zj.panjiajie.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://iv.lnxyls.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://zj.huixinmuqiang.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://rv.nicolike.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://zz.shxzukj.cn

[N10] 链表节点定义
来源：http://br.huanxung.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ae.colortex.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ku.521024.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://lf.shtwfgs.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://fn.lnxyls.cn

Java: class Node { int v; Node next; }
来源：http://ty.hahajie.cn

Go:   type Node struct { V int; Next *Node }
来源：http://xc.nicolike.cn


<!-- 参考信息 -->