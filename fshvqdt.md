代发 wailian999

Py:   date.today();  date.today().replace(day=1)
来源：http://gl.9csxet.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://by.shxzskj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://sb.huixinmuqiang.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://xb.jctech888.com.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://dr.haigaiapp.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://if.szsharing.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://it.521024.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://uy.521024.cn

================================================================================
来源：http://ey.gzmigu.cn

K. JSON 与序列化
来源：http://kn.huanxung.cn

================================================================================
来源：http://ke.huixiangedu.cn

[K01] 对象转 JSON 字符串
来源：http://iu.nicolike.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ts.bjjhwx.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://he.panjiajie.cn

JS:   JSON.stringify(obj)
来源：http://ao.chemitech.net.cn

TS:   JSON.stringify(obj)
来源：http://uc.bookmarksfly.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://zu.bookmarksfly.cn

Go:   json.Marshal(obj)
来源：http://mp.shtwfgs.cn

Ruby: obj.to_json                                     // require "json"
来源：http://cu.521024.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ft.nicolike.cn

[K02] JSON 字符串转对象
来源：http://jh.huanxung.cn

Py:   json.loads(s)
来源：http://kv.lnxyls.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://xc.muxihuayi.cn

JS:   JSON.parse(s)
来源：http://xq.lnxyls.cn

TS:   JSON.parse(s)
来源：http://pj.jianghongdianzi.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jc.521024.cn

Go:   json.Unmarshal(data, &v)
来源：http://bq.hnjuh.cn

Ruby: JSON.parse(s)
来源：http://yl.jianghongdianzi.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qa.nicolike.cn

[K03] JSON 美化输出（带缩进）
来源：http://zq.asd995.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://jv.lnxyls.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://av.asd995.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ut.shxzukj.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://nc.jctech888.com.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qb.colortex.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wr.nicolike.cn

Ruby: JSON.pretty_generate(obj)
来源：http://zi.gzmigu.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://qh.haigaiapp.cn

[K04] 读取 JSON 文件
来源：http://qw.bookmarksfly.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://zb.gzmigu.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mg.muxihuayi.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mg.shxzukj.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://eo.hnjuh.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ld.haigaiapp.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://pd.nszjky.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://gy.shtwfgs.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://cv.wgjwhj.cn

[K05] 深拷贝对象
来源：http://na.huixiangedu.cn

Py:   copy.deepcopy(obj)
来源：http://sj.chemitech.net.cn

PHP:  unserialize(serialize($obj));
来源：http://jz.bookmarksfly.cn

JS:   structuredClone(obj)
来源：http://qu.9csxet.cn

TS:   structuredClone(obj)
来源：http://mf.yuntaijiaju.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://gn.huanxung.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ix.jctech888.com.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ez.wgjwhj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://tz.huixinmuqiang.cn

[K06] 解析 URL 查询串
来源：http://as.jianghongdianzi.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rz.szsharing.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hs.nszjky.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fi.yuexingan06.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wa.shtwfgs.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mg.shtwfgs.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://dt.colortex.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ee.hahajie.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://rx.newstarts.cn

[K07] 进制转换
来源：http://nj.muxihuayi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ed.521024.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ys.newstarts.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ba.bjjhwx.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://vr.yuntaijiaju.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://dy.bjjhwx.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://eu.asd995.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://gy.9csxet.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://dz.nszjky.cn

[K08] 二进制序列化（非 JSON）
来源：http://co.huanxung.cn

Py:   pickle.dumps(obj)
来源：http://kp.chemitech.net.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://hq.nszjky.cn

JS:   v8.serialize(obj)        // Node
来源：http://nz.newstarts.cn

TS:   v8.serialize(obj)        // Node
来源：http://ym.jianghongdianzi.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://st.shxzukj.cn

Go:   encoding/gob
来源：http://da.shxzukj.cn

Ruby: Marshal.dump(obj)
来源：http://tr.szsharing.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://tk.haigaiapp.cn

================================================================================
来源：http://bz.nicolike.cn

L. 网络请求
来源：http://jr.panjiajie.cn

================================================================================
来源：http://df.shxzukj.cn

[L01] 发送 GET 请求
来源：http://xi.huixinmuqiang.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://gc.panjiajie.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://fw.521024.cn

JS:   await fetch(url)
来源：http://bp.colortex.cn

TS:   await fetch(url)
来源：http://km.lnxyls.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ga.9csxet.cn

Go:   resp, err := http.Get(url)
来源：http://iq.jianghongdianzi.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://hx.bjjhwx.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ax.hahajie.cn

[L02] 发送 POST JSON
来源：http://gd.muxihuayi.cn

Py:   requests.post(url, json={"a": 1})
来源：http://cx.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://sq.yuexingan06.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ty.bookmarksfly.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://st.haigaiapp.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://yk.nszjky.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://tl.chemitech.net.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://nl.wgjwhj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://js.nicolike.cn

[L03] 设置自定义请求头
来源：http://bq.nicolike.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://pn.wgjwhj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://xh.bjjhwx.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://uw.colortex.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vg.szxytkj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://pi.gzmigu.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://nf.yuexingan06.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://dy.panjiajie.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ng.muxihuayi.cn

[L04] 设置超时
来源：http://xo.bookmarksfly.cn

Py:   requests.get(url, timeout=5)
来源：http://zh.nszjky.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hp.nszjky.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://io.huanxung.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ni.hnjuh.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wb.nicolike.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://gi.jctech888.com.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ll.hahajie.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://gm.haigaiapp.cn

[L05] 上传文件（multipart）
来源：http://wl.asd995.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://bq.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://se.nszjky.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ge.yuexingan06.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://rx.huixinmuqiang.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://cd.hnjuh.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://zh.muxihuayi.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://pm.colortex.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://fb.huixinmuqiang.cn

[L06] 解析响应为 JSON
来源：http://ab.panjiajie.cn

Py:   resp.json()
来源：http://cu.shxzskj.cn

PHP:  json_decode($body, true);
来源：http://tf.wgjwhj.cn

JS:   await resp.json()
来源：http://gi.haigaiapp.cn

TS:   await resp.json()
来源：http://vu.huixinmuqiang.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://so.szxytkj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hl.wgjwhj.cn

Ruby: JSON.parse(resp.body)
来源：http://gb.newstarts.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wb.wgjwhj.cn

[L07] 处理 HTTP 状态码
来源：http://yn.chemitech.net.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://il.wgjwhj.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://zv.shxzukj.cn

JS:   resp.ok;  resp.status
来源：http://de.panjiajie.cn

TS:   resp.ok;  resp.status
来源：http://ro.gzmigu.cn

Java: resp.statusCode()
来源：http://yn.yuntaijiaju.cn

Go:   resp.StatusCode
来源：http://uh.nicolike.cn

Ruby: resp.code.to_i
来源：http://vp.lnxyls.cn

C#:   (int)resp.StatusCode
来源：http://hw.newstarts.cn

[L08] 并发请求多个地址
来源：http://bx.bjjhwx.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://be.9csxet.cn

PHP:  curl_multi_init() 系列
来源：http://fd.nicolike.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hs.yuntaijiaju.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ci.shxzskj.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wb.gzmigu.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://uv.huixiangedu.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://yh.panjiajie.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://zo.hahajie.cn

================================================================================
来源：http://ii.yuntaijiaju.cn

M. 命令行 / 进程 / 环境
来源：http://ku.newstarts.cn

================================================================================
来源：http://kl.szxytkj.cn

[M01] 读取命令行参数
来源：http://vr.muxihuayi.cn

Py:   sys.argv[1:]
来源：http://vd.yuntaijiaju.cn

PHP:  $argv;  $argc;
来源：http://oe.nszjky.cn

JS:   process.argv.slice(2)
来源：http://zh.huixinmuqiang.cn

TS:   process.argv.slice(2)
来源：http://ha.muxihuayi.cn

Java: args 数组（main 方法参数）
来源：http://kd.huanxung.cn

Go:   os.Args[1:]
来源：http://kd.asd995.cn

Ruby: ARGV
来源：http://uv.shxzskj.cn

C#:   args 数组（Main 方法参数）
来源：http://me.colortex.cn

[M02] 读取环境变量
来源：http://al.shtwfgs.cn

Py:   os.environ.get("HOME")
来源：http://wu.nszjky.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://gj.szsharing.cn

JS:   process.env.HOME
来源：http://oc.szxytkj.cn

TS:   process.env.HOME
来源：http://vj.nicolike.cn

Java: System.getenv("HOME")
来源：http://xa.wgjwhj.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ny.muxihuayi.cn

Ruby: ENV["HOME"]
来源：http://xa.nszjky.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://bc.yuntaijiaju.cn

[M03] 执行外部命令
来源：http://fy.jianghongdianzi.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ip.9csxet.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://vz.haigaiapp.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://oe.szxytkj.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://zf.colortex.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ba.521024.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ob.asd995.cn

Ruby: system("ls -l");  `ls -l`
来源：http://cl.lnxyls.cn

C#:   Process.Start("ls", "-l");
来源：http://bf.jctech888.com.cn

[M04] 获取当前工作目录
来源：http://ub.jctech888.com.cn

Py:   os.getcwd()
来源：http://wf.yuexingan06.cn

PHP:  getcwd();
来源：http://uc.hahajie.cn

JS:   process.cwd()
来源：http://cj.colortex.cn

TS:   process.cwd()
来源：http://ds.jianghongdianzi.cn

Java: Path.of("").toAbsolutePath()
来源：http://fq.gzmigu.cn

Go:   os.Getwd()
来源：http://zc.szxytkj.cn

Ruby: Dir.pwd
来源：http://xv.hnjuh.cn

C#:   Directory.GetCurrentDirectory()
来源：http://qa.chemitech.net.cn

[M05] 设置退出码
来源：http://rq.muxihuayi.cn

Py:   sys.exit(1)
来源：http://ce.jctech888.com.cn

PHP:  exit(1);
来源：http://kk.hahajie.cn

JS:   process.exit(1)
来源：http://uz.jctech888.com.cn

TS:   process.exit(1)
来源：http://pl.huixiangedu.cn

Java: System.exit(1)
来源：http://qc.muxihuayi.cn

Go:   os.Exit(1)
来源：http://ts.yuntaijiaju.cn

Ruby: exit 1
来源：http://hh.muxihuayi.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ng.jctech888.com.cn

[M06] 向标准错误输出
来源：http://xi.chemitech.net.cn

Py:   print("err", file=sys.stderr)
来源：http://pa.bjjhwx.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://kr.521024.cn

JS:   console.error("err")
来源：http://oy.newstarts.cn

TS:   console.error("err")
来源：http://wa.colortex.cn

Java: System.err.println("err")
来源：http://pr.colortex.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://lw.colortex.cn

Ruby: warn "err"
来源：http://sl.gzmigu.cn

C#:   Console.Error.WriteLine("err")
来源：http://rd.chemitech.net.cn

[M07] 判断是否为主入口
来源：http://cm.yuexingan06.cn

Py:   if __name__ == "__main__":
来源：http://di.bjjhwx.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hk.shxzskj.cn

JS:   require.main === module
来源：http://ja.wgjwhj.cn

TS:   require.main === module
来源：http://jm.szxytkj.cn

Java: public static void main(String[] args)
来源：http://mk.jianghongdianzi.cn

Go:   func main()
来源：http://za.lnxyls.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ca.nszjky.cn

C#:   static void Main(string[] args)
来源：http://xl.colortex.cn

[M08] 获取系统与运行时信息
来源：http://vq.huixinmuqiang.cn

Py:   platform.system();  platform.python_version()
来源：http://cr.szxytkj.cn

PHP:  PHP_OS;  phpversion();
来源：http://pi.huixinmuqiang.cn

JS:   process.platform;  process.version
来源：http://kl.huixinmuqiang.cn

TS:   process.platform;  process.version
来源：http://un.hahajie.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://iw.jianghongdianzi.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://wg.haigaiapp.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ri.wgjwhj.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://dv.nszjky.cn

================================================================================
来源：http://nd.muxihuayi.cn

N. 数据结构与算法
来源：http://dq.colortex.cn

================================================================================
来源：http://zd.shxzskj.cn

[N01] 二分查找（有序数组）
来源：http://bg.gzmigu.cn

Py:   bisect.bisect_left(arr, x)
来源：http://zt.newstarts.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://eo.chemitech.net.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pm.521024.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cs.yuexingan06.cn

Java: Arrays.binarySearch(arr, x)
来源：http://yr.9csxet.cn

Go:   sort.SearchInts(arr, x)
来源：http://wf.colortex.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://st.szsharing.cn

C#:   Array.BinarySearch(arr, x)
来源：http://pp.hnjuh.cn

[N02] 排序（工程实践用内置实现）
来源：http://qm.yuntaijiaju.cn

Py:   sorted(arr);  arr.sort()
来源：http://yj.jctech888.com.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ma.panjiajie.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://uh.jianghongdianzi.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://op.szsharing.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hh.bookmarksfly.cn

Go:   slices.Sort(arr)
来源：http://nj.muxihuayi.cn

Ruby: arr.sort
来源：http://al.bookmarksfly.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://dm.gzmigu.cn

[N03] 快速排序（分治示例）
来源：http://kz.yuntaijiaju.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://in.bjjhwx.cn

PHP:  // 递归实现，或用 usort
来源：http://fc.gzmigu.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ex.newstarts.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qo.gzmigu.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://zx.colortex.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://yh.gzmigu.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://bm.asd995.cn

C#:   // 手写递归，或 Array.Sort
来源：http://kb.newstarts.cn

[N04] 斐波那契数列
来源：http://zd.huixinmuqiang.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://af.yuntaijiaju.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ff.9csxet.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jt.gzmigu.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ia.hahajie.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ka.gzmigu.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://bo.wgjwhj.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://tn.asd995.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://iy.jianghongdianzi.cn

[N05] 最大公约数
来源：http://fj.nicolike.cn

Py:   math.gcd(a, b)
来源：http://wb.asd995.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://dd.bjjhwx.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://na.521024.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wo.huanxung.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ro.shxzukj.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://bn.jctech888.com.cn

Ruby: a.gcd(b)
来源：http://hz.wgjwhj.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://rz.huixiangedu.cn

[N06] 判断回文字符串
来源：http://gg.colortex.cn

Py:   s == s[::-1]
来源：http://jd.yuntaijiaju.cn

PHP:  $s === strrev($s);
来源：http://mf.szxytkj.cn

JS:   s === [...s].reverse().join("")
来源：http://wp.nicolike.cn

TS:   s === [...s].reverse().join("")
来源：http://ol.szxytkj.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://de.yuntaijiaju.cn

Go:   // 双指针从两端比较
来源：http://ec.shxzskj.cn

Ruby: s == s.reverse
来源：http://nf.jctech888.com.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://at.bookmarksfly.cn

[N07] 两数之和（返回下标）
来源：http://kb.hahajie.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ub.gzmigu.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ke.huixiangedu.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://lc.hahajie.cn

TS:   // 手写 Map<string, number>
来源：http://zl.szsharing.cn

Java: // 手写 HashMap
来源：http://yv.lnxyls.cn

Go:   // 手写 map[int]int
来源：http://aq.yuexingan06.cn

Ruby: // 手写 Hash
来源：http://ly.newstarts.cn

C#:   // 手写 Dictionary<int, int>
来源：http://jo.9csxet.cn

[N08] 生成全排列
来源：http://to.shxzukj.cn


<!-- 参考信息 -->