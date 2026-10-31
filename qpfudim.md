代发 wailian999

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://nc.haigaiapp.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://yq.huanxung.cn

[J09] 时区处理
来源：http://ux.wgjwhj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://tz.huixiangedu.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://so.huixiangedu.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ye.panjiajie.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jc.shxzukj.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://au.yuexingan06.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ep.nszjky.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://rs.huixiangedu.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jn.chemitech.net.cn

[J10] 取今天 / 本月第一天
来源：http://dh.lnxyls.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://vy.gzmigu.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://fg.gzmigu.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://px.lnxyls.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://cg.newstarts.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qx.huixinmuqiang.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://at.nszjky.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://jn.shxzskj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ff.gzmigu.cn

================================================================================
来源：http://ik.nicolike.cn

K. JSON 与序列化
来源：http://qw.hahajie.cn

================================================================================
来源：http://it.newstarts.cn

[K01] 对象转 JSON 字符串
来源：http://no.newstarts.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://fh.jianghongdianzi.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://gk.newstarts.cn

JS:   JSON.stringify(obj)
来源：http://nt.lnxyls.cn

TS:   JSON.stringify(obj)
来源：http://ye.hahajie.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ue.9csxet.cn

Go:   json.Marshal(obj)
来源：http://tx.yuexingan06.cn

Ruby: obj.to_json                                     // require "json"
来源：http://al.shxzukj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://fn.gzmigu.cn

[K02] JSON 字符串转对象
来源：http://kt.szsharing.cn

Py:   json.loads(s)
来源：http://qg.huixinmuqiang.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://bb.shxzukj.cn

JS:   JSON.parse(s)
来源：http://zx.jianghongdianzi.cn

TS:   JSON.parse(s)
来源：http://ia.huixinmuqiang.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vj.shxzukj.cn

Go:   json.Unmarshal(data, &v)
来源：http://ba.jianghongdianzi.cn

Ruby: JSON.parse(s)
来源：http://zr.nicolike.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://og.szxytkj.cn

[K03] JSON 美化输出（带缩进）
来源：http://dj.huixinmuqiang.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mo.haigaiapp.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://lz.newstarts.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://gv.muxihuayi.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://kz.szsharing.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://dt.huixiangedu.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ex.bjjhwx.cn

Ruby: JSON.pretty_generate(obj)
来源：http://jo.colortex.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://tz.wgjwhj.cn

[K04] 读取 JSON 文件
来源：http://at.szxytkj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://sl.shxzskj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://cr.colortex.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jb.asd995.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lj.shxzukj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://td.jianghongdianzi.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://rc.huixiangedu.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://xr.9csxet.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://bh.gzmigu.cn

[K05] 深拷贝对象
来源：http://el.jctech888.com.cn

Py:   copy.deepcopy(obj)
来源：http://pg.shtwfgs.cn

PHP:  unserialize(serialize($obj));
来源：http://vz.colortex.cn

JS:   structuredClone(obj)
来源：http://vf.jctech888.com.cn

TS:   structuredClone(obj)
来源：http://rs.muxihuayi.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ug.shtwfgs.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://jf.huanxung.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zw.haigaiapp.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://hh.shxzukj.cn

[K06] 解析 URL 查询串
来源：http://vc.bookmarksfly.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://il.nicolike.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://pr.wgjwhj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ps.colortex.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yc.panjiajie.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.nicolike.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://fr.nicolike.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://se.jianghongdianzi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://jt.yuexingan06.cn

[K07] 进制转换
来源：http://tm.huanxung.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://do.9csxet.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://xh.huixiangedu.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xd.chemitech.net.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hq.wgjwhj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://np.huanxung.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://pd.huixinmuqiang.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ok.bookmarksfly.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ae.521024.cn

[K08] 二进制序列化（非 JSON）
来源：http://me.wgjwhj.cn

Py:   pickle.dumps(obj)
来源：http://zf.szsharing.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://cn.shtwfgs.cn

JS:   v8.serialize(obj)        // Node
来源：http://cc.shxzukj.cn

TS:   v8.serialize(obj)        // Node
来源：http://pn.hnjuh.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://gc.huixiangedu.cn

Go:   encoding/gob
来源：http://qx.yuntaijiaju.cn

Ruby: Marshal.dump(obj)
来源：http://iv.9csxet.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://dh.wgjwhj.cn

================================================================================
来源：http://ba.chemitech.net.cn

L. 网络请求
来源：http://sb.colortex.cn

================================================================================
来源：http://ju.szxytkj.cn

[L01] 发送 GET 请求
来源：http://uw.shxzukj.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://bg.bookmarksfly.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hm.521024.cn

JS:   await fetch(url)
来源：http://lw.muxihuayi.cn

TS:   await fetch(url)
来源：http://bz.jianghongdianzi.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://oc.lnxyls.cn

Go:   resp, err := http.Get(url)
来源：http://tm.colortex.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ng.panjiajie.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://uz.shxzskj.cn

[L02] 发送 POST JSON
来源：http://cj.hahajie.cn

Py:   requests.post(url, json={"a": 1})
来源：http://al.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ba.shxzukj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qy.yuexingan06.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yg.hnjuh.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://zc.chemitech.net.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://go.lnxyls.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://tz.panjiajie.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://eo.shxzskj.cn

[L03] 设置自定义请求头
来源：http://eh.shxzukj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://gh.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ma.hnjuh.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hp.muxihuayi.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://oi.521024.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://cp.muxihuayi.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://po.yuntaijiaju.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://zj.bookmarksfly.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://vj.bjjhwx.cn

[L04] 设置超时
来源：http://bj.bookmarksfly.cn

Py:   requests.get(url, timeout=5)
来源：http://lp.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://nb.huixiangedu.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jt.wgjwhj.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jw.asd995.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mj.newstarts.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://yi.jctech888.com.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://rx.jianghongdianzi.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://vm.gzmigu.cn

[L05] 上传文件（multipart）
来源：http://nk.shxzukj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://pz.szxytkj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://fi.colortex.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://zc.newstarts.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ex.chemitech.net.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ht.colortex.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://br.gzmigu.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://db.wgjwhj.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ds.colortex.cn

[L06] 解析响应为 JSON
来源：http://ry.nszjky.cn

Py:   resp.json()
来源：http://ya.shxzukj.cn

PHP:  json_decode($body, true);
来源：http://hw.hahajie.cn

JS:   await resp.json()
来源：http://bn.yuexingan06.cn

TS:   await resp.json()
来源：http://qe.huanxung.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://tv.chemitech.net.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ug.hnjuh.cn

Ruby: JSON.parse(resp.body)
来源：http://zk.jctech888.com.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://nb.chemitech.net.cn

[L07] 处理 HTTP 状态码
来源：http://zx.huixiangedu.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://kn.yuntaijiaju.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://dj.yuntaijiaju.cn

JS:   resp.ok;  resp.status
来源：http://tj.haigaiapp.cn

TS:   resp.ok;  resp.status
来源：http://fu.huanxung.cn

Java: resp.statusCode()
来源：http://dp.huanxung.cn

Go:   resp.StatusCode
来源：http://zi.huixiangedu.cn

Ruby: resp.code.to_i
来源：http://je.yuntaijiaju.cn

C#:   (int)resp.StatusCode
来源：http://zl.lnxyls.cn

[L08] 并发请求多个地址
来源：http://kt.521024.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://za.yuntaijiaju.cn

PHP:  curl_multi_init() 系列
来源：http://wl.hahajie.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yo.newstarts.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kn.yuntaijiaju.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://yx.gzmigu.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ee.521024.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hm.bookmarksfly.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://bb.bjjhwx.cn

================================================================================
来源：http://it.panjiajie.cn

M. 命令行 / 进程 / 环境
来源：http://tp.haigaiapp.cn

================================================================================
来源：http://wz.huixinmuqiang.cn

[M01] 读取命令行参数
来源：http://lu.szxytkj.cn

Py:   sys.argv[1:]
来源：http://eu.gzmigu.cn

PHP:  $argv;  $argc;
来源：http://nn.yuntaijiaju.cn

JS:   process.argv.slice(2)
来源：http://ow.lnxyls.cn

TS:   process.argv.slice(2)
来源：http://wn.szxytkj.cn

Java: args 数组（main 方法参数）
来源：http://in.chemitech.net.cn

Go:   os.Args[1:]
来源：http://dn.chemitech.net.cn

Ruby: ARGV
来源：http://nk.521024.cn

C#:   args 数组（Main 方法参数）
来源：http://ny.nicolike.cn

[M02] 读取环境变量
来源：http://zq.521024.cn

Py:   os.environ.get("HOME")
来源：http://vy.asd995.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mx.shxzukj.cn

JS:   process.env.HOME
来源：http://oh.hnjuh.cn

TS:   process.env.HOME
来源：http://bk.huixinmuqiang.cn

Java: System.getenv("HOME")
来源：http://rw.huixiangedu.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://rw.jianghongdianzi.cn

Ruby: ENV["HOME"]
来源：http://rl.panjiajie.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://zt.huanxung.cn

[M03] 执行外部命令
来源：http://ql.hnjuh.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://kx.newstarts.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hl.huixiangedu.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ep.wgjwhj.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://pg.szxytkj.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://nb.521024.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://xm.jctech888.com.cn

Ruby: system("ls -l");  `ls -l`
来源：http://er.bjjhwx.cn

C#:   Process.Start("ls", "-l");
来源：http://es.bjjhwx.cn

[M04] 获取当前工作目录
来源：http://jd.bookmarksfly.cn

Py:   os.getcwd()
来源：http://fx.shtwfgs.cn

PHP:  getcwd();
来源：http://ob.521024.cn

JS:   process.cwd()
来源：http://aw.huanxung.cn

TS:   process.cwd()
来源：http://uj.huanxung.cn

Java: Path.of("").toAbsolutePath()
来源：http://cn.9csxet.cn

Go:   os.Getwd()
来源：http://kw.521024.cn

Ruby: Dir.pwd
来源：http://cf.huanxung.cn

C#:   Directory.GetCurrentDirectory()
来源：http://vh.bjjhwx.cn

[M05] 设置退出码
来源：http://ol.shxzskj.cn

Py:   sys.exit(1)
来源：http://et.huixiangedu.cn

PHP:  exit(1);
来源：http://es.yuntaijiaju.cn

JS:   process.exit(1)
来源：http://zm.shxzukj.cn

TS:   process.exit(1)
来源：http://yx.bookmarksfly.cn

Java: System.exit(1)
来源：http://qk.yuexingan06.cn

Go:   os.Exit(1)
来源：http://kl.szxytkj.cn

Ruby: exit 1
来源：http://qm.szxytkj.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://xm.shxzskj.cn

[M06] 向标准错误输出
来源：http://va.hnjuh.cn

Py:   print("err", file=sys.stderr)
来源：http://wv.gzmigu.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://xf.jianghongdianzi.cn

JS:   console.error("err")
来源：http://jj.huixinmuqiang.cn

TS:   console.error("err")
来源：http://jg.bookmarksfly.cn

Java: System.err.println("err")
来源：http://lo.bjjhwx.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://fa.huanxung.cn

Ruby: warn "err"
来源：http://er.yuexingan06.cn

C#:   Console.Error.WriteLine("err")
来源：http://qm.muxihuayi.cn

[M07] 判断是否为主入口
来源：http://sc.bookmarksfly.cn

Py:   if __name__ == "__main__":
来源：http://hy.lnxyls.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ph.nszjky.cn

JS:   require.main === module
来源：http://do.wgjwhj.cn

TS:   require.main === module
来源：http://ei.wgjwhj.cn

Java: public static void main(String[] args)
来源：http://vf.huixiangedu.cn

Go:   func main()
来源：http://gr.wgjwhj.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://jp.huixinmuqiang.cn

C#:   static void Main(string[] args)
来源：http://ct.newstarts.cn

[M08] 获取系统与运行时信息
来源：http://uw.hnjuh.cn

Py:   platform.system();  platform.python_version()
来源：http://wi.lnxyls.cn

PHP:  PHP_OS;  phpversion();
来源：http://ya.szsharing.cn

JS:   process.platform;  process.version
来源：http://mu.yuexingan06.cn

TS:   process.platform;  process.version
来源：http://ks.asd995.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://tr.huixinmuqiang.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://qr.lnxyls.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ud.shxzskj.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://tt.jianghongdianzi.cn

================================================================================
来源：http://ef.asd995.cn

N. 数据结构与算法
来源：http://bw.huanxung.cn

================================================================================
来源：http://uq.szxytkj.cn

[N01] 二分查找（有序数组）
来源：http://ev.szxytkj.cn

Py:   bisect.bisect_left(arr, x)
来源：http://bz.asd995.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ok.asd995.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vz.jctech888.com.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dj.hahajie.cn

Java: Arrays.binarySearch(arr, x)
来源：http://py.hnjuh.cn

Go:   sort.SearchInts(arr, x)
来源：http://ib.nicolike.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://zq.asd995.cn

C#:   Array.BinarySearch(arr, x)
来源：http://wt.jianghongdianzi.cn

[N02] 排序（工程实践用内置实现）
来源：http://ii.newstarts.cn

Py:   sorted(arr);  arr.sort()
来源：http://ae.yuntaijiaju.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wn.521024.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://iy.szxytkj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://tf.huanxung.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://er.muxihuayi.cn

Go:   slices.Sort(arr)
来源：http://rr.huixinmuqiang.cn

Ruby: arr.sort
来源：http://gb.wgjwhj.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://nn.szsharing.cn

[N03] 快速排序（分治示例）
来源：http://yo.wgjwhj.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://nq.9csxet.cn

PHP:  // 递归实现，或用 usort
来源：http://ir.521024.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://no.bjjhwx.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://th.9csxet.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hq.jianghongdianzi.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://cg.9csxet.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://cv.yuexingan06.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ah.nicolike.cn

[N04] 斐波那契数列
来源：http://tg.shtwfgs.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ni.panjiajie.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ue.szxytkj.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://al.szsharing.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ld.huixiangedu.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://rz.bjjhwx.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://sh.szxytkj.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ll.lnxyls.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://re.gzmigu.cn

[N05] 最大公约数
来源：http://he.shtwfgs.cn

Py:   math.gcd(a, b)
来源：http://je.nicolike.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://vm.lnxyls.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jr.yuntaijiaju.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ej.9csxet.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://el.shxzukj.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://tt.hnjuh.cn

Ruby: a.gcd(b)
来源：http://xf.muxihuayi.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://xv.huixiangedu.cn

[N06] 判断回文字符串
来源：http://dn.huanxung.cn

Py:   s == s[::-1]
来源：http://yj.nszjky.cn

PHP:  $s === strrev($s);
来源：http://bs.bookmarksfly.cn

JS:   s === [...s].reverse().join("")
来源：http://vs.jianghongdianzi.cn

TS:   s === [...s].reverse().join("")
来源：http://md.yuexingan06.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ca.521024.cn

Go:   // 双指针从两端比较
来源：http://mt.521024.cn


<!-- 参考信息 -->