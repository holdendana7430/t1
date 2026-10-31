代发 wailian999

[J07] 比较两个日期
来源：http://lp.panjiajie.cn

Py:   d1 < d2;  d1 == d2
来源：http://qv.yuntaijiaju.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://cc.yuntaijiaju.cn

JS:   d1.getTime() < d2.getTime()
来源：http://an.bookmarksfly.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ny.521024.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://fs.huanxung.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://zp.bookmarksfly.cn

Ruby: d1 < d2;  d1 == d2
来源：http://af.colortex.cn

C#:   d1 < d2;  d1 == d2
来源：http://wr.wgjwhj.cn

[J08] 提取年月日与星期
来源：http://ek.shxzskj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wl.jianghongdianzi.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://kl.shtwfgs.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://cf.huixiangedu.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://la.lnxyls.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://nn.nszjky.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://pt.521024.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://vg.hahajie.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ua.shxzskj.cn

[J09] 时区处理
来源：http://tu.bookmarksfly.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hn.chemitech.net.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://yy.9csxet.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://er.hahajie.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qi.haigaiapp.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://gu.colortex.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://lz.yuexingan06.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://wi.yuntaijiaju.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://pd.shtwfgs.cn

[J10] 取今天 / 本月第一天
来源：http://qk.shxzskj.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ca.shxzukj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://qd.gzmigu.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ou.asd995.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qc.asd995.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://kw.nszjky.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://iz.bookmarksfly.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ei.asd995.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ut.huixinmuqiang.cn

================================================================================
来源：http://fz.panjiajie.cn

K. JSON 与序列化
来源：http://dd.szxytkj.cn

================================================================================
来源：http://bv.shtwfgs.cn

[K01] 对象转 JSON 字符串
来源：http://qt.szsharing.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://pp.hnjuh.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://rk.yuntaijiaju.cn

JS:   JSON.stringify(obj)
来源：http://ea.huixinmuqiang.cn

TS:   JSON.stringify(obj)
来源：http://xr.asd995.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mo.colortex.cn

Go:   json.Marshal(obj)
来源：http://mc.gzmigu.cn

Ruby: obj.to_json                                     // require "json"
来源：http://qt.nicolike.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://fk.newstarts.cn

[K02] JSON 字符串转对象
来源：http://qj.wgjwhj.cn

Py:   json.loads(s)
来源：http://bh.yuntaijiaju.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://kg.hahajie.cn

JS:   JSON.parse(s)
来源：http://bu.huanxung.cn

TS:   JSON.parse(s)
来源：http://zs.wgjwhj.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://sc.newstarts.cn

Go:   json.Unmarshal(data, &v)
来源：http://bd.wgjwhj.cn

Ruby: JSON.parse(s)
来源：http://mz.yuexingan06.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://lf.szxytkj.cn

[K03] JSON 美化输出（带缩进）
来源：http://bv.asd995.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://gh.newstarts.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ax.huixiangedu.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://gs.szxytkj.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://hm.colortex.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://lz.521024.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ze.asd995.cn

Ruby: JSON.pretty_generate(obj)
来源：http://bz.asd995.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://lv.hahajie.cn

[K04] 读取 JSON 文件
来源：http://jh.huixinmuqiang.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://xq.haigaiapp.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://kn.asd995.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://py.jctech888.com.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ae.9csxet.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://gw.shtwfgs.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wu.nszjky.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://yl.newstarts.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://sh.shxzskj.cn

[K05] 深拷贝对象
来源：http://gn.chemitech.net.cn

Py:   copy.deepcopy(obj)
来源：http://rr.asd995.cn

PHP:  unserialize(serialize($obj));
来源：http://dp.bookmarksfly.cn

JS:   structuredClone(obj)
来源：http://mx.9csxet.cn

TS:   structuredClone(obj)
来源：http://vs.bjjhwx.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://py.shtwfgs.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ad.huanxung.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://yd.yuntaijiaju.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://xc.nicolike.cn

[K06] 解析 URL 查询串
来源：http://lw.lnxyls.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://iu.nszjky.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://qm.panjiajie.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yq.yuexingan06.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ss.shtwfgs.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://kw.yuexingan06.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://tc.chemitech.net.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ho.shtwfgs.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://bw.lnxyls.cn

[K07] 进制转换
来源：http://vj.521024.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://lh.asd995.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://gj.hahajie.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://gk.gzmigu.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://fy.newstarts.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://yo.chemitech.net.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://fc.szxytkj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qi.chemitech.net.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wj.yuntaijiaju.cn

[K08] 二进制序列化（非 JSON）
来源：http://hw.hnjuh.cn

Py:   pickle.dumps(obj)
来源：http://ul.nicolike.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://mj.szxytkj.cn

JS:   v8.serialize(obj)        // Node
来源：http://xg.asd995.cn

TS:   v8.serialize(obj)        // Node
来源：http://jn.huixiangedu.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://sg.lnxyls.cn

Go:   encoding/gob
来源：http://mx.panjiajie.cn

Ruby: Marshal.dump(obj)
来源：http://yq.shtwfgs.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://zj.yuexingan06.cn

================================================================================
来源：http://rn.bookmarksfly.cn

L. 网络请求
来源：http://or.haigaiapp.cn

================================================================================
来源：http://xg.521024.cn

[L01] 发送 GET 请求
来源：http://sq.shxzukj.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xx.gzmigu.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xh.hnjuh.cn

JS:   await fetch(url)
来源：http://bc.muxihuayi.cn

TS:   await fetch(url)
来源：http://cj.newstarts.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://jh.haigaiapp.cn

Go:   resp, err := http.Get(url)
来源：http://fd.yuexingan06.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://gj.hahajie.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://lx.bjjhwx.cn

[L02] 发送 POST JSON
来源：http://kg.lnxyls.cn

Py:   requests.post(url, json={"a": 1})
来源：http://gt.521024.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://kf.szsharing.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fz.asd995.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cn.haigaiapp.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://so.gzmigu.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://yi.bookmarksfly.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://zn.bookmarksfly.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://jz.nszjky.cn

[L03] 设置自定义请求头
来源：http://wu.panjiajie.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://rh.shtwfgs.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://fb.shxzskj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ow.shxzskj.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ku.jctech888.com.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://aj.nszjky.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wr.jianghongdianzi.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://yg.shxzukj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://va.yuntaijiaju.cn

[L04] 设置超时
来源：http://dj.asd995.cn

Py:   requests.get(url, timeout=5)
来源：http://fh.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wn.9csxet.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://eb.szxytkj.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cn.asd995.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://nn.nszjky.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://yz.huanxung.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://te.jctech888.com.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ix.gzmigu.cn

[L05] 上传文件（multipart）
来源：http://vh.bookmarksfly.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://pp.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://yb.521024.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://db.jctech888.com.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ej.chemitech.net.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ii.nszjky.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://sg.wgjwhj.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://gm.haigaiapp.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://jl.muxihuayi.cn

[L06] 解析响应为 JSON
来源：http://bm.colortex.cn

Py:   resp.json()
来源：http://eo.nicolike.cn

PHP:  json_decode($body, true);
来源：http://yd.szsharing.cn

JS:   await resp.json()
来源：http://wz.hahajie.cn

TS:   await resp.json()
来源：http://wu.newstarts.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://he.jianghongdianzi.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://qi.newstarts.cn

Ruby: JSON.parse(resp.body)
来源：http://rf.nicolike.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://py.bjjhwx.cn

[L07] 处理 HTTP 状态码
来源：http://yf.asd995.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ke.jianghongdianzi.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mr.asd995.cn

JS:   resp.ok;  resp.status
来源：http://ta.asd995.cn

TS:   resp.ok;  resp.status
来源：http://xd.wgjwhj.cn

Java: resp.statusCode()
来源：http://ja.nszjky.cn

Go:   resp.StatusCode
来源：http://lg.chemitech.net.cn

Ruby: resp.code.to_i
来源：http://te.nszjky.cn

C#:   (int)resp.StatusCode
来源：http://ls.hnjuh.cn

[L08] 并发请求多个地址
来源：http://ge.haigaiapp.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://un.yuntaijiaju.cn

PHP:  curl_multi_init() 系列
来源：http://nk.muxihuayi.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xk.huanxung.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zi.szsharing.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://sp.haigaiapp.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://re.colortex.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://bb.panjiajie.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xr.jianghongdianzi.cn

================================================================================
来源：http://oj.newstarts.cn

M. 命令行 / 进程 / 环境
来源：http://xo.huanxung.cn

================================================================================
来源：http://gu.huixinmuqiang.cn

[M01] 读取命令行参数
来源：http://ag.lnxyls.cn

Py:   sys.argv[1:]
来源：http://bx.nicolike.cn

PHP:  $argv;  $argc;
来源：http://po.huixiangedu.cn

JS:   process.argv.slice(2)
来源：http://lh.shtwfgs.cn

TS:   process.argv.slice(2)
来源：http://ip.wgjwhj.cn

Java: args 数组（main 方法参数）
来源：http://by.hahajie.cn

Go:   os.Args[1:]
来源：http://oj.asd995.cn

Ruby: ARGV
来源：http://qe.jianghongdianzi.cn

C#:   args 数组（Main 方法参数）
来源：http://kn.nicolike.cn

[M02] 读取环境变量
来源：http://fw.panjiajie.cn

Py:   os.environ.get("HOME")
来源：http://kx.panjiajie.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://aq.chemitech.net.cn

JS:   process.env.HOME
来源：http://pl.muxihuayi.cn

TS:   process.env.HOME
来源：http://lc.bookmarksfly.cn

Java: System.getenv("HOME")
来源：http://kr.lnxyls.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://xi.bookmarksfly.cn

Ruby: ENV["HOME"]
来源：http://mm.bookmarksfly.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wj.panjiajie.cn

[M03] 执行外部命令
来源：http://nf.huixiangedu.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ef.huanxung.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://cv.wgjwhj.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://dl.lnxyls.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://kh.huanxung.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://bv.wgjwhj.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://wp.yuexingan06.cn

Ruby: system("ls -l");  `ls -l`
来源：http://kv.hnjuh.cn

C#:   Process.Start("ls", "-l");
来源：http://vj.lnxyls.cn

[M04] 获取当前工作目录
来源：http://dz.huixinmuqiang.cn

Py:   os.getcwd()
来源：http://sz.asd995.cn

PHP:  getcwd();
来源：http://ky.yuexingan06.cn

JS:   process.cwd()
来源：http://fw.gzmigu.cn

TS:   process.cwd()
来源：http://dj.gzmigu.cn

Java: Path.of("").toAbsolutePath()
来源：http://ow.chemitech.net.cn

Go:   os.Getwd()
来源：http://cn.jianghongdianzi.cn

Ruby: Dir.pwd
来源：http://ev.nszjky.cn

C#:   Directory.GetCurrentDirectory()
来源：http://au.huanxung.cn

[M05] 设置退出码
来源：http://zv.jianghongdianzi.cn

Py:   sys.exit(1)
来源：http://ie.szxytkj.cn

PHP:  exit(1);
来源：http://ok.jctech888.com.cn

JS:   process.exit(1)
来源：http://hh.szxytkj.cn

TS:   process.exit(1)
来源：http://bs.szsharing.cn

Java: System.exit(1)
来源：http://wu.chemitech.net.cn

Go:   os.Exit(1)
来源：http://gt.nicolike.cn

Ruby: exit 1
来源：http://bq.chemitech.net.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://nj.shxzskj.cn

[M06] 向标准错误输出
来源：http://cb.szsharing.cn

Py:   print("err", file=sys.stderr)
来源：http://fo.bookmarksfly.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://lf.muxihuayi.cn

JS:   console.error("err")
来源：http://si.huixiangedu.cn

TS:   console.error("err")
来源：http://zs.asd995.cn

Java: System.err.println("err")
来源：http://nb.shtwfgs.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mx.huanxung.cn

Ruby: warn "err"
来源：http://xd.nszjky.cn

C#:   Console.Error.WriteLine("err")
来源：http://by.szxytkj.cn

[M07] 判断是否为主入口
来源：http://kg.yuntaijiaju.cn

Py:   if __name__ == "__main__":
来源：http://dd.nicolike.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://qi.yuexingan06.cn

JS:   require.main === module
来源：http://xx.muxihuayi.cn

TS:   require.main === module
来源：http://vi.colortex.cn

Java: public static void main(String[] args)
来源：http://hv.wgjwhj.cn

Go:   func main()
来源：http://jq.bookmarksfly.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://nj.nicolike.cn

C#:   static void Main(string[] args)
来源：http://gn.nicolike.cn

[M08] 获取系统与运行时信息
来源：http://id.huixiangedu.cn

Py:   platform.system();  platform.python_version()
来源：http://jk.shxzukj.cn

PHP:  PHP_OS;  phpversion();
来源：http://fj.hahajie.cn

JS:   process.platform;  process.version
来源：http://sj.panjiajie.cn

TS:   process.platform;  process.version
来源：http://kw.nicolike.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://yb.haigaiapp.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://rr.asd995.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://vk.shtwfgs.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://qi.9csxet.cn

================================================================================
来源：http://ud.9csxet.cn

N. 数据结构与算法
来源：http://qf.asd995.cn

================================================================================
来源：http://en.shtwfgs.cn

[N01] 二分查找（有序数组）
来源：http://hp.chemitech.net.cn

Py:   bisect.bisect_left(arr, x)
来源：http://bw.wgjwhj.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://zv.szsharing.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mc.szxytkj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dy.shxzukj.cn

Java: Arrays.binarySearch(arr, x)
来源：http://jq.szxytkj.cn

Go:   sort.SearchInts(arr, x)
来源：http://bl.yuntaijiaju.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://uw.yuexingan06.cn

C#:   Array.BinarySearch(arr, x)
来源：http://vs.colortex.cn

[N02] 排序（工程实践用内置实现）
来源：http://tl.haigaiapp.cn

Py:   sorted(arr);  arr.sort()
来源：http://cw.szsharing.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://xo.hahajie.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://nk.shxzskj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ix.colortex.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://qr.chemitech.net.cn

Go:   slices.Sort(arr)
来源：http://bq.huixiangedu.cn

Ruby: arr.sort
来源：http://rl.huixinmuqiang.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ol.newstarts.cn

[N03] 快速排序（分治示例）
来源：http://bs.yuntaijiaju.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://fy.yuntaijiaju.cn

PHP:  // 递归实现，或用 usort
来源：http://gg.haigaiapp.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vg.yuexingan06.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fw.huixiangedu.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hu.yuntaijiaju.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wg.huixiangedu.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://be.jctech888.com.cn

C#:   // 手写递归，或 Array.Sort
来源：http://vk.panjiajie.cn

[N04] 斐波那契数列
来源：http://yv.hnjuh.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ga.9csxet.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://qk.shxzskj.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wy.wgjwhj.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xd.nszjky.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ij.shxzukj.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://aj.colortex.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://gh.chemitech.net.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://jq.colortex.cn


<!-- 参考信息 -->