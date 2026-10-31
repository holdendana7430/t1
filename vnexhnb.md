代发 wailian999

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ui.yuexingan06.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://cz.jianghongdianzi.cn

[J09] 时区处理
来源：http://ci.yuexingan06.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qo.yuexingan06.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ca.yuntaijiaju.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vy.szsharing.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yi.asd995.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://sl.huanxung.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mv.asd995.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://wp.shxzskj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wb.panjiajie.cn

[J10] 取今天 / 本月第一天
来源：http://sb.panjiajie.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://pd.bjjhwx.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://yq.9csxet.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://gl.colortex.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ol.newstarts.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://jy.huanxung.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://de.nszjky.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://qv.panjiajie.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://qk.chemitech.net.cn

================================================================================
来源：http://sk.shtwfgs.cn

K. JSON 与序列化
来源：http://lc.jianghongdianzi.cn

================================================================================
来源：http://rl.hahajie.cn

[K01] 对象转 JSON 字符串
来源：http://zk.shtwfgs.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://sq.szxytkj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://js.jianghongdianzi.cn

JS:   JSON.stringify(obj)
来源：http://ou.lnxyls.cn

TS:   JSON.stringify(obj)
来源：http://pp.shtwfgs.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ae.colortex.cn

Go:   json.Marshal(obj)
来源：http://wr.shtwfgs.cn

Ruby: obj.to_json                                     // require "json"
来源：http://am.bjjhwx.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://hb.shxzukj.cn

[K02] JSON 字符串转对象
来源：http://tn.haigaiapp.cn

Py:   json.loads(s)
来源：http://hw.chemitech.net.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://oa.gzmigu.cn

JS:   JSON.parse(s)
来源：http://qk.panjiajie.cn

TS:   JSON.parse(s)
来源：http://ml.nszjky.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://sd.chemitech.net.cn

Go:   json.Unmarshal(data, &v)
来源：http://ti.muxihuayi.cn

Ruby: JSON.parse(s)
来源：http://zj.huixiangedu.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ic.huanxung.cn

[K03] JSON 美化输出（带缩进）
来源：http://uy.newstarts.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://aj.szsharing.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hy.521024.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://kt.hnjuh.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ep.hahajie.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wk.521024.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ef.colortex.cn

Ruby: JSON.pretty_generate(obj)
来源：http://qs.chemitech.net.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ja.huixiangedu.cn

[K04] 读取 JSON 文件
来源：http://of.newstarts.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://eq.nszjky.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://dc.chemitech.net.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tu.shxzskj.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pm.9csxet.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://xh.yuexingan06.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ts.bjjhwx.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://bk.huanxung.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://yj.521024.cn

[K05] 深拷贝对象
来源：http://qq.panjiajie.cn

Py:   copy.deepcopy(obj)
来源：http://dy.haigaiapp.cn

PHP:  unserialize(serialize($obj));
来源：http://yo.hahajie.cn

JS:   structuredClone(obj)
来源：http://qr.nszjky.cn

TS:   structuredClone(obj)
来源：http://kk.panjiajie.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://gb.nicolike.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://fd.521024.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ez.hnjuh.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://oa.wgjwhj.cn

[K06] 解析 URL 查询串
来源：http://io.huanxung.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://cm.szsharing.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wk.newstarts.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ic.huixiangedu.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gg.bjjhwx.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ry.shxzukj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ez.szsharing.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ef.lnxyls.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ks.shtwfgs.cn

[K07] 进制转换
来源：http://xe.szxytkj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://oy.9csxet.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://gn.jctech888.com.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://it.newstarts.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://pt.hahajie.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://gx.lnxyls.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ed.bjjhwx.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qh.szsharing.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://xg.shxzukj.cn

[K08] 二进制序列化（非 JSON）
来源：http://tz.bookmarksfly.cn

Py:   pickle.dumps(obj)
来源：http://fn.chemitech.net.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ha.9csxet.cn

JS:   v8.serialize(obj)        // Node
来源：http://ny.newstarts.cn

TS:   v8.serialize(obj)        // Node
来源：http://fo.colortex.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://jx.nicolike.cn

Go:   encoding/gob
来源：http://io.shtwfgs.cn

Ruby: Marshal.dump(obj)
来源：http://kx.shxzukj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://zh.shxzukj.cn

================================================================================
来源：http://ex.bookmarksfly.cn

L. 网络请求
来源：http://uy.hahajie.cn

================================================================================
来源：http://pu.bookmarksfly.cn

[L01] 发送 GET 请求
来源：http://ke.chemitech.net.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hp.lnxyls.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://uo.asd995.cn

JS:   await fetch(url)
来源：http://za.jianghongdianzi.cn

TS:   await fetch(url)
来源：http://iu.colortex.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://sn.521024.cn

Go:   resp, err := http.Get(url)
来源：http://ll.hahajie.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ar.panjiajie.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://qi.shtwfgs.cn

[L02] 发送 POST JSON
来源：http://ih.shxzukj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ne.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://dc.huixiangedu.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://po.colortex.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ad.hahajie.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ea.yuexingan06.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://zk.haigaiapp.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ya.jianghongdianzi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://dy.nicolike.cn

[L03] 设置自定义请求头
来源：http://mv.shxzukj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://il.nicolike.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://sb.bjjhwx.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tp.shtwfgs.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nl.panjiajie.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ud.jctech888.com.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://bh.shxzukj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://dm.lnxyls.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://sm.szsharing.cn

[L04] 设置超时
来源：http://cb.9csxet.cn

Py:   requests.get(url, timeout=5)
来源：http://pe.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ee.asd995.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ux.gzmigu.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cb.yuexingan06.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ts.newstarts.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://zy.wgjwhj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://kf.huanxung.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://be.9csxet.cn

[L05] 上传文件（multipart）
来源：http://mz.wgjwhj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://lt.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://xg.shtwfgs.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ge.muxihuayi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://vw.bjjhwx.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mr.9csxet.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://gn.shxzukj.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hn.huixiangedu.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://aj.521024.cn

[L06] 解析响应为 JSON
来源：http://hj.haigaiapp.cn

Py:   resp.json()
来源：http://zw.nszjky.cn

PHP:  json_decode($body, true);
来源：http://ko.huixiangedu.cn

JS:   await resp.json()
来源：http://xd.muxihuayi.cn

TS:   await resp.json()
来源：http://zo.nicolike.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://al.haigaiapp.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hh.szsharing.cn

Ruby: JSON.parse(resp.body)
来源：http://sg.yuexingan06.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://sz.asd995.cn

[L07] 处理 HTTP 状态码
来源：http://hi.jianghongdianzi.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://of.panjiajie.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://at.521024.cn

JS:   resp.ok;  resp.status
来源：http://qi.yuexingan06.cn

TS:   resp.ok;  resp.status
来源：http://wi.lnxyls.cn

Java: resp.statusCode()
来源：http://hr.szxytkj.cn

Go:   resp.StatusCode
来源：http://wr.huixiangedu.cn

Ruby: resp.code.to_i
来源：http://td.muxihuayi.cn

C#:   (int)resp.StatusCode
来源：http://vf.shtwfgs.cn

[L08] 并发请求多个地址
来源：http://df.szsharing.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hs.hahajie.cn

PHP:  curl_multi_init() 系列
来源：http://lp.panjiajie.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://an.521024.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hc.jianghongdianzi.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://vg.haigaiapp.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://sk.shxzskj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mp.szxytkj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://an.521024.cn

================================================================================
来源：http://ke.chemitech.net.cn

M. 命令行 / 进程 / 环境
来源：http://co.haigaiapp.cn

================================================================================
来源：http://xr.jianghongdianzi.cn

[M01] 读取命令行参数
来源：http://tt.shtwfgs.cn

Py:   sys.argv[1:]
来源：http://bp.hahajie.cn

PHP:  $argv;  $argc;
来源：http://ph.shxzukj.cn

JS:   process.argv.slice(2)
来源：http://eu.nszjky.cn

TS:   process.argv.slice(2)
来源：http://nv.szxytkj.cn

Java: args 数组（main 方法参数）
来源：http://ml.haigaiapp.cn

Go:   os.Args[1:]
来源：http://nu.nszjky.cn

Ruby: ARGV
来源：http://ly.bjjhwx.cn

C#:   args 数组（Main 方法参数）
来源：http://nh.bjjhwx.cn

[M02] 读取环境变量
来源：http://dq.panjiajie.cn

Py:   os.environ.get("HOME")
来源：http://tl.haigaiapp.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ty.bookmarksfly.cn

JS:   process.env.HOME
来源：http://zg.huanxung.cn

TS:   process.env.HOME
来源：http://gd.muxihuayi.cn

Java: System.getenv("HOME")
来源：http://yt.newstarts.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://di.shxzukj.cn

Ruby: ENV["HOME"]
来源：http://zf.shtwfgs.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://em.wgjwhj.cn

[M03] 执行外部命令
来源：http://gu.hahajie.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://st.panjiajie.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://sm.huixiangedu.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://qp.szsharing.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://es.asd995.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hd.9csxet.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://uq.shtwfgs.cn

Ruby: system("ls -l");  `ls -l`
来源：http://od.huanxung.cn

C#:   Process.Start("ls", "-l");
来源：http://pl.huixinmuqiang.cn

[M04] 获取当前工作目录
来源：http://an.newstarts.cn

Py:   os.getcwd()
来源：http://sq.hnjuh.cn

PHP:  getcwd();
来源：http://ab.szsharing.cn

JS:   process.cwd()
来源：http://xo.lnxyls.cn

TS:   process.cwd()
来源：http://am.bjjhwx.cn

Java: Path.of("").toAbsolutePath()
来源：http://fc.bjjhwx.cn

Go:   os.Getwd()
来源：http://sd.bookmarksfly.cn

Ruby: Dir.pwd
来源：http://vk.chemitech.net.cn

C#:   Directory.GetCurrentDirectory()
来源：http://uc.shxzskj.cn

[M05] 设置退出码
来源：http://xx.huanxung.cn

Py:   sys.exit(1)
来源：http://bd.szsharing.cn

PHP:  exit(1);
来源：http://cb.shxzskj.cn

JS:   process.exit(1)
来源：http://ll.huixiangedu.cn

TS:   process.exit(1)
来源：http://df.asd995.cn

Java: System.exit(1)
来源：http://mn.hahajie.cn

Go:   os.Exit(1)
来源：http://gj.asd995.cn

Ruby: exit 1
来源：http://gc.bjjhwx.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hg.szsharing.cn

[M06] 向标准错误输出
来源：http://zw.yuexingan06.cn

Py:   print("err", file=sys.stderr)
来源：http://yo.gzmigu.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://us.wgjwhj.cn

JS:   console.error("err")
来源：http://ky.shtwfgs.cn

TS:   console.error("err")
来源：http://ai.shtwfgs.cn

Java: System.err.println("err")
来源：http://lh.521024.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://bc.nicolike.cn

Ruby: warn "err"
来源：http://dp.bookmarksfly.cn

C#:   Console.Error.WriteLine("err")
来源：http://lb.gzmigu.cn

[M07] 判断是否为主入口
来源：http://tq.huixinmuqiang.cn

Py:   if __name__ == "__main__":
来源：http://el.muxihuayi.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hg.huanxung.cn

JS:   require.main === module
来源：http://pu.huixinmuqiang.cn

TS:   require.main === module
来源：http://jv.asd995.cn

Java: public static void main(String[] args)
来源：http://qw.bookmarksfly.cn

Go:   func main()
来源：http://li.bjjhwx.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://zp.szsharing.cn

C#:   static void Main(string[] args)
来源：http://yz.jctech888.com.cn

[M08] 获取系统与运行时信息
来源：http://gz.bookmarksfly.cn

Py:   platform.system();  platform.python_version()
来源：http://or.huanxung.cn

PHP:  PHP_OS;  phpversion();
来源：http://rx.nicolike.cn

JS:   process.platform;  process.version
来源：http://mx.bjjhwx.cn

TS:   process.platform;  process.version
来源：http://zf.yuntaijiaju.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://en.chemitech.net.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://vf.nicolike.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://sj.huanxung.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://qd.muxihuayi.cn

================================================================================
来源：http://uc.9csxet.cn

N. 数据结构与算法
来源：http://al.yuexingan06.cn

================================================================================
来源：http://bt.szxytkj.cn

[N01] 二分查找（有序数组）
来源：http://kf.haigaiapp.cn

Py:   bisect.bisect_left(arr, x)
来源：http://mo.asd995.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ax.jianghongdianzi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sn.bookmarksfly.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nw.hahajie.cn

Java: Arrays.binarySearch(arr, x)
来源：http://uc.gzmigu.cn

Go:   sort.SearchInts(arr, x)
来源：http://hy.shtwfgs.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ax.shxzskj.cn

C#:   Array.BinarySearch(arr, x)
来源：http://vv.gzmigu.cn

[N02] 排序（工程实践用内置实现）
来源：http://px.jianghongdianzi.cn

Py:   sorted(arr);  arr.sort()
来源：http://pe.wgjwhj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://at.bookmarksfly.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://dn.hnjuh.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://np.szsharing.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://sj.chemitech.net.cn

Go:   slices.Sort(arr)
来源：http://ci.yuexingan06.cn

Ruby: arr.sort
来源：http://gx.nicolike.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://bp.huixiangedu.cn

[N03] 快速排序（分治示例）
来源：http://xf.wgjwhj.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://qx.jianghongdianzi.cn

PHP:  // 递归实现，或用 usort
来源：http://ux.lnxyls.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ep.wgjwhj.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jd.huixiangedu.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://oq.huixinmuqiang.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wo.jianghongdianzi.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ux.bjjhwx.cn

C#:   // 手写递归，或 Array.Sort
来源：http://cq.huanxung.cn

[N04] 斐波那契数列
来源：http://fw.szxytkj.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://az.wgjwhj.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hn.lnxyls.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zh.yuexingan06.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://je.szsharing.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://at.shtwfgs.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hi.bjjhwx.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ut.asd995.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://sa.haigaiapp.cn

[N05] 最大公约数
来源：http://nk.yuexingan06.cn

Py:   math.gcd(a, b)
来源：http://bn.yuntaijiaju.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://vw.hnjuh.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zd.szsharing.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nh.wgjwhj.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hf.colortex.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://rg.huixiangedu.cn

Ruby: a.gcd(b)
来源：http://lp.jctech888.com.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ng.9csxet.cn

[N06] 判断回文字符串
来源：http://bg.521024.cn

Py:   s == s[::-1]
来源：http://em.9csxet.cn

PHP:  $s === strrev($s);
来源：http://yr.jctech888.com.cn

JS:   s === [...s].reverse().join("")
来源：http://vx.gzmigu.cn

TS:   s === [...s].reverse().join("")
来源：http://xh.nicolike.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ep.newstarts.cn

Go:   // 双指针从两端比较
来源：http://sd.newstarts.cn


<!-- 参考信息 -->