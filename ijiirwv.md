代发 wailian999

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://jd.asd995.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pa.muxihuayi.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ws.panjiajie.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://un.asd995.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://uc.szxytkj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://pe.jianghongdianzi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ks.muxihuayi.cn

[J10] 取今天 / 本月第一天
来源：http://mk.9csxet.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://mw.huanxung.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ls.muxihuayi.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wd.nicolike.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://np.gzmigu.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://sj.bjjhwx.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xi.9csxet.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://gp.yuntaijiaju.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://sc.521024.cn

================================================================================
来源：http://or.hnjuh.cn

K. JSON 与序列化
来源：http://rc.9csxet.cn

================================================================================
来源：http://ac.hnjuh.cn

[K01] 对象转 JSON 字符串
来源：http://zq.bjjhwx.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://nh.huanxung.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://uw.bookmarksfly.cn

JS:   JSON.stringify(obj)
来源：http://wi.nicolike.cn

TS:   JSON.stringify(obj)
来源：http://pc.shxzukj.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://qm.shxzukj.cn

Go:   json.Marshal(obj)
来源：http://kp.colortex.cn

Ruby: obj.to_json                                     // require "json"
来源：http://dz.bookmarksfly.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://io.szxytkj.cn

[K02] JSON 字符串转对象
来源：http://dq.jianghongdianzi.cn

Py:   json.loads(s)
来源：http://ny.hnjuh.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://vf.szxytkj.cn

JS:   JSON.parse(s)
来源：http://fl.hahajie.cn

TS:   JSON.parse(s)
来源：http://fd.jctech888.com.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://or.huanxung.cn

Go:   json.Unmarshal(data, &v)
来源：http://gl.shxzukj.cn

Ruby: JSON.parse(s)
来源：http://ue.muxihuayi.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zv.lnxyls.cn

[K03] JSON 美化输出（带缩进）
来源：http://rr.asd995.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ia.shxzukj.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ry.nszjky.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://hv.hahajie.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://nq.shtwfgs.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hi.huixinmuqiang.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ki.nicolike.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ej.newstarts.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://jq.wgjwhj.cn

[K04] 读取 JSON 文件
来源：http://rg.chemitech.net.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ar.yuexingan06.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://qt.asd995.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yc.newstarts.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mf.shtwfgs.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ib.hahajie.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://eb.muxihuayi.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://dl.gzmigu.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ad.huixiangedu.cn

[K05] 深拷贝对象
来源：http://ml.huixiangedu.cn

Py:   copy.deepcopy(obj)
来源：http://fo.asd995.cn

PHP:  unserialize(serialize($obj));
来源：http://xx.jianghongdianzi.cn

JS:   structuredClone(obj)
来源：http://kw.huixinmuqiang.cn

TS:   structuredClone(obj)
来源：http://vp.shtwfgs.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://bm.wgjwhj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://kv.shtwfgs.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ri.jctech888.com.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://or.panjiajie.cn

[K06] 解析 URL 查询串
来源：http://kx.yuexingan06.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rl.shxzskj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://gf.521024.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ln.hahajie.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gc.shxzskj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wj.huanxung.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://bu.huixiangedu.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://gf.gzmigu.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://vg.bookmarksfly.cn

[K07] 进制转换
来源：http://nc.bookmarksfly.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ch.gzmigu.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vp.jianghongdianzi.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://as.wgjwhj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://eo.bookmarksfly.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ye.huixinmuqiang.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://xr.9csxet.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://sr.szsharing.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://rs.nicolike.cn

[K08] 二进制序列化（非 JSON）
来源：http://wz.shtwfgs.cn

Py:   pickle.dumps(obj)
来源：http://pd.colortex.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://dk.yuexingan06.cn

JS:   v8.serialize(obj)        // Node
来源：http://aa.9csxet.cn

TS:   v8.serialize(obj)        // Node
来源：http://op.szxytkj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://nd.bjjhwx.cn

Go:   encoding/gob
来源：http://te.bjjhwx.cn

Ruby: Marshal.dump(obj)
来源：http://ah.yuexingan06.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://zd.huixiangedu.cn

================================================================================
来源：http://up.hnjuh.cn

L. 网络请求
来源：http://fm.panjiajie.cn

================================================================================
来源：http://hj.yuntaijiaju.cn

[L01] 发送 GET 请求
来源：http://rw.jianghongdianzi.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://kd.haigaiapp.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ul.521024.cn

JS:   await fetch(url)
来源：http://ra.szsharing.cn

TS:   await fetch(url)
来源：http://cd.521024.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ks.nszjky.cn

Go:   resp, err := http.Get(url)
来源：http://ix.colortex.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://xo.gzmigu.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ij.gzmigu.cn

[L02] 发送 POST JSON
来源：http://uh.nicolike.cn

Py:   requests.post(url, json={"a": 1})
来源：http://nw.521024.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://og.bookmarksfly.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ob.newstarts.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gj.shtwfgs.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://nm.gzmigu.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hh.bookmarksfly.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://oa.jianghongdianzi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://cy.panjiajie.cn

[L03] 设置自定义请求头
来源：http://zt.yuntaijiaju.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://va.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://fx.521024.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://we.huixinmuqiang.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jm.haigaiapp.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ex.yuexingan06.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://cw.shxzukj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://zf.hnjuh.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://dg.521024.cn

[L04] 设置超时
来源：http://om.szsharing.cn

Py:   requests.get(url, timeout=5)
来源：http://ix.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://jg.chemitech.net.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hm.521024.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://aa.9csxet.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://tp.yuntaijiaju.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xk.nszjky.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://tu.haigaiapp.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://fe.jianghongdianzi.cn

[L05] 上传文件（multipart）
来源：http://ng.wgjwhj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://na.yuntaijiaju.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://fv.nicolike.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ms.jctech888.com.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wr.nicolike.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ro.lnxyls.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ed.nszjky.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://aq.521024.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://pz.jctech888.com.cn

[L06] 解析响应为 JSON
来源：http://zo.szsharing.cn

Py:   resp.json()
来源：http://iu.shxzskj.cn

PHP:  json_decode($body, true);
来源：http://oh.bjjhwx.cn

JS:   await resp.json()
来源：http://ca.shtwfgs.cn

TS:   await resp.json()
来源：http://hr.hahajie.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://tw.bookmarksfly.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://qa.521024.cn

Ruby: JSON.parse(resp.body)
来源：http://cx.huixiangedu.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ik.jctech888.com.cn

[L07] 处理 HTTP 状态码
来源：http://bs.nicolike.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://dm.bookmarksfly.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://kl.asd995.cn

JS:   resp.ok;  resp.status
来源：http://zs.nicolike.cn

TS:   resp.ok;  resp.status
来源：http://ot.521024.cn

Java: resp.statusCode()
来源：http://fw.gzmigu.cn

Go:   resp.StatusCode
来源：http://tg.colortex.cn

Ruby: resp.code.to_i
来源：http://mz.nicolike.cn

C#:   (int)resp.StatusCode
来源：http://qv.szsharing.cn

[L08] 并发请求多个地址
来源：http://zt.muxihuayi.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://xo.szsharing.cn

PHP:  curl_multi_init() 系列
来源：http://ky.nicolike.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zq.wgjwhj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ie.hnjuh.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://zl.nicolike.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ff.chemitech.net.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ba.hahajie.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://io.chemitech.net.cn

================================================================================
来源：http://pp.haigaiapp.cn

M. 命令行 / 进程 / 环境
来源：http://to.haigaiapp.cn

================================================================================
来源：http://rw.haigaiapp.cn

[M01] 读取命令行参数
来源：http://yg.shtwfgs.cn

Py:   sys.argv[1:]
来源：http://nx.asd995.cn

PHP:  $argv;  $argc;
来源：http://ys.shxzukj.cn

JS:   process.argv.slice(2)
来源：http://uq.nszjky.cn

TS:   process.argv.slice(2)
来源：http://rt.lnxyls.cn

Java: args 数组（main 方法参数）
来源：http://wa.asd995.cn

Go:   os.Args[1:]
来源：http://nw.asd995.cn

Ruby: ARGV
来源：http://bl.nicolike.cn

C#:   args 数组（Main 方法参数）
来源：http://ia.lnxyls.cn

[M02] 读取环境变量
来源：http://yu.colortex.cn

Py:   os.environ.get("HOME")
来源：http://tl.lnxyls.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hn.shtwfgs.cn

JS:   process.env.HOME
来源：http://bo.jctech888.com.cn

TS:   process.env.HOME
来源：http://iv.nszjky.cn

Java: System.getenv("HOME")
来源：http://iw.asd995.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://dt.jianghongdianzi.cn

Ruby: ENV["HOME"]
来源：http://ko.jianghongdianzi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://dr.jianghongdianzi.cn

[M03] 执行外部命令
来源：http://iq.jctech888.com.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mf.panjiajie.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://iu.gzmigu.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://so.yuntaijiaju.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://rt.newstarts.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://yp.huanxung.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://bo.jianghongdianzi.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ya.9csxet.cn

C#:   Process.Start("ls", "-l");
来源：http://um.chemitech.net.cn

[M04] 获取当前工作目录
来源：http://tw.shxzskj.cn

Py:   os.getcwd()
来源：http://tv.9csxet.cn

PHP:  getcwd();
来源：http://we.hnjuh.cn

JS:   process.cwd()
来源：http://qs.lnxyls.cn

TS:   process.cwd()
来源：http://pa.asd995.cn

Java: Path.of("").toAbsolutePath()
来源：http://qn.9csxet.cn

Go:   os.Getwd()
来源：http://wt.haigaiapp.cn

Ruby: Dir.pwd
来源：http://oz.nszjky.cn

C#:   Directory.GetCurrentDirectory()
来源：http://no.bookmarksfly.cn

[M05] 设置退出码
来源：http://fx.hahajie.cn

Py:   sys.exit(1)
来源：http://vf.shxzskj.cn

PHP:  exit(1);
来源：http://uh.szsharing.cn

JS:   process.exit(1)
来源：http://lm.panjiajie.cn

TS:   process.exit(1)
来源：http://rz.muxihuayi.cn

Java: System.exit(1)
来源：http://hj.nicolike.cn

Go:   os.Exit(1)
来源：http://wj.wgjwhj.cn

Ruby: exit 1
来源：http://la.9csxet.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ab.shxzskj.cn

[M06] 向标准错误输出
来源：http://ij.lnxyls.cn

Py:   print("err", file=sys.stderr)
来源：http://td.asd995.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://js.newstarts.cn

JS:   console.error("err")
来源：http://kh.gzmigu.cn

TS:   console.error("err")
来源：http://yx.shxzukj.cn

Java: System.err.println("err")
来源：http://sz.haigaiapp.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://dr.huanxung.cn

Ruby: warn "err"
来源：http://gj.9csxet.cn

C#:   Console.Error.WriteLine("err")
来源：http://vr.chemitech.net.cn

[M07] 判断是否为主入口
来源：http://lo.huixinmuqiang.cn

Py:   if __name__ == "__main__":
来源：http://th.huixiangedu.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://th.asd995.cn

JS:   require.main === module
来源：http://gv.newstarts.cn

TS:   require.main === module
来源：http://si.bjjhwx.cn

Java: public static void main(String[] args)
来源：http://ei.colortex.cn

Go:   func main()
来源：http://ez.huixiangedu.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://rd.hnjuh.cn

C#:   static void Main(string[] args)
来源：http://zg.szsharing.cn

[M08] 获取系统与运行时信息
来源：http://gs.asd995.cn

Py:   platform.system();  platform.python_version()
来源：http://gf.muxihuayi.cn

PHP:  PHP_OS;  phpversion();
来源：http://qm.gzmigu.cn

JS:   process.platform;  process.version
来源：http://dz.bjjhwx.cn

TS:   process.platform;  process.version
来源：http://lt.haigaiapp.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://vm.bookmarksfly.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://bk.bjjhwx.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ej.jianghongdianzi.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://gq.9csxet.cn

================================================================================
来源：http://bd.huixinmuqiang.cn

N. 数据结构与算法
来源：http://sj.haigaiapp.cn

================================================================================
来源：http://gs.bookmarksfly.cn

[N01] 二分查找（有序数组）
来源：http://iq.panjiajie.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ct.yuexingan06.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://qw.9csxet.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://am.muxihuayi.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ie.521024.cn

Java: Arrays.binarySearch(arr, x)
来源：http://wp.9csxet.cn

Go:   sort.SearchInts(arr, x)
来源：http://hw.haigaiapp.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ba.nicolike.cn

C#:   Array.BinarySearch(arr, x)
来源：http://en.521024.cn

[N02] 排序（工程实践用内置实现）
来源：http://gn.muxihuayi.cn

Py:   sorted(arr);  arr.sort()
来源：http://xv.panjiajie.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wi.haigaiapp.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ye.nszjky.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://hp.colortex.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://gd.huixiangedu.cn

Go:   slices.Sort(arr)
来源：http://cm.hnjuh.cn

Ruby: arr.sort
来源：http://kg.shxzskj.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://lr.jctech888.com.cn

[N03] 快速排序（分治示例）
来源：http://lz.szxytkj.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://zi.hnjuh.cn

PHP:  // 递归实现，或用 usort
来源：http://rh.bookmarksfly.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jo.bjjhwx.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dr.lnxyls.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ml.chemitech.net.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://nj.lnxyls.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ix.shtwfgs.cn

C#:   // 手写递归，或 Array.Sort
来源：http://gz.hahajie.cn

[N04] 斐波那契数列
来源：http://jq.muxihuayi.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://gg.gzmigu.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wv.chemitech.net.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ju.shtwfgs.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lr.asd995.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wj.wgjwhj.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://sr.szsharing.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ce.bookmarksfly.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hv.gzmigu.cn

[N05] 最大公约数
来源：http://kg.shxzskj.cn

Py:   math.gcd(a, b)
来源：http://df.huixiangedu.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wc.9csxet.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ei.panjiajie.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xp.9csxet.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ba.shxzskj.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ay.9csxet.cn

Ruby: a.gcd(b)
来源：http://mb.haigaiapp.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://fu.panjiajie.cn

[N06] 判断回文字符串
来源：http://xw.yuntaijiaju.cn

Py:   s == s[::-1]
来源：http://sh.yuntaijiaju.cn

PHP:  $s === strrev($s);
来源：http://mb.nszjky.cn

JS:   s === [...s].reverse().join("")
来源：http://xq.colortex.cn

TS:   s === [...s].reverse().join("")
来源：http://gc.lnxyls.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://js.9csxet.cn

Go:   // 双指针从两端比较
来源：http://uz.colortex.cn

Ruby: s == s.reverse
来源：http://rb.bookmarksfly.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://kc.nicolike.cn

[N07] 两数之和（返回下标）
来源：http://jr.huixiangedu.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://xa.muxihuayi.cn


<!-- 参考信息 -->