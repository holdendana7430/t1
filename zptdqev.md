代发 wailian999

Java: Duration.between(start, end).toSeconds()
来源：http://lu.hahajie.cn

Go:   end.Sub(start).Hours()
来源：http://bj.gzmigu.cn

Ruby: end - start                 # 返回秒数
来源：http://yh.bjjhwx.cn

C#:   (end - start).TotalSeconds
来源：http://us.nicolike.cn

[J07] 比较两个日期
来源：http://eg.nszjky.cn

Py:   d1 < d2;  d1 == d2
来源：http://ju.lnxyls.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ea.colortex.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ay.asd995.cn

TS:   d1.getTime() < d2.getTime()
来源：http://wo.shxzukj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://jk.panjiajie.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://vo.huixinmuqiang.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ta.haigaiapp.cn

C#:   d1 < d2;  d1 == d2
来源：http://dz.chemitech.net.cn

[J08] 提取年月日与星期
来源：http://mp.muxihuayi.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mb.panjiajie.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://sq.wgjwhj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://px.chemitech.net.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://pc.huanxung.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://te.jctech888.com.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://du.asd995.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://bt.9csxet.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://iy.lnxyls.cn

[J09] 时区处理
来源：http://er.szsharing.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mr.lnxyls.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://zz.gzmigu.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tu.panjiajie.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cg.yuntaijiaju.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://zy.newstarts.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://yl.haigaiapp.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ma.shxzskj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hl.panjiajie.cn

[J10] 取今天 / 本月第一天
来源：http://vq.gzmigu.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://xr.colortex.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://gh.chemitech.net.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://jd.jianghongdianzi.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qa.shxzukj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://gc.shtwfgs.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://yy.yuexingan06.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://sx.yuexingan06.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ib.nicolike.cn

================================================================================
来源：http://yc.newstarts.cn

K. JSON 与序列化
来源：http://cx.bjjhwx.cn

================================================================================
来源：http://kz.nicolike.cn

[K01] 对象转 JSON 字符串
来源：http://ah.wgjwhj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://gz.huixinmuqiang.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://gi.wgjwhj.cn

JS:   JSON.stringify(obj)
来源：http://ps.huixiangedu.cn

TS:   JSON.stringify(obj)
来源：http://ax.shxzukj.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://zg.asd995.cn

Go:   json.Marshal(obj)
来源：http://hj.9csxet.cn

Ruby: obj.to_json                                     // require "json"
来源：http://xa.huixinmuqiang.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://vx.chemitech.net.cn

[K02] JSON 字符串转对象
来源：http://mi.jianghongdianzi.cn

Py:   json.loads(s)
来源：http://zo.shxzukj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://do.shtwfgs.cn

JS:   JSON.parse(s)
来源：http://hb.newstarts.cn

TS:   JSON.parse(s)
来源：http://yf.muxihuayi.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mk.shxzukj.cn

Go:   json.Unmarshal(data, &v)
来源：http://xb.nszjky.cn

Ruby: JSON.parse(s)
来源：http://al.haigaiapp.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://bs.yuexingan06.cn

[K03] JSON 美化输出（带缩进）
来源：http://hk.lnxyls.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://gc.9csxet.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ot.nszjky.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://wm.gzmigu.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://yt.bookmarksfly.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://iu.haigaiapp.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ro.nicolike.cn

Ruby: JSON.pretty_generate(obj)
来源：http://vg.huixiangedu.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://on.asd995.cn

[K04] 读取 JSON 文件
来源：http://ry.huixiangedu.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://zc.lnxyls.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ii.yuntaijiaju.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ab.szsharing.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sd.lnxyls.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ki.panjiajie.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mp.shxzskj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://wa.jctech888.com.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://tb.huanxung.cn

[K05] 深拷贝对象
来源：http://my.jctech888.com.cn

Py:   copy.deepcopy(obj)
来源：http://wo.szxytkj.cn

PHP:  unserialize(serialize($obj));
来源：http://aw.jctech888.com.cn

JS:   structuredClone(obj)
来源：http://nc.haigaiapp.cn

TS:   structuredClone(obj)
来源：http://qe.asd995.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://mg.lnxyls.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ag.szxytkj.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://oo.haigaiapp.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ym.hahajie.cn

[K06] 解析 URL 查询串
来源：http://zz.muxihuayi.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://sr.bookmarksfly.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://gp.gzmigu.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zj.chemitech.net.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://aa.shxzukj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://dy.bookmarksfly.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ze.huixinmuqiang.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://zq.huanxung.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://dl.panjiajie.cn

[K07] 进制转换
来源：http://ib.yuexingan06.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ep.szxytkj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ly.bjjhwx.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xb.haigaiapp.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wk.colortex.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://uk.jctech888.com.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://fa.lnxyls.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wd.newstarts.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://zp.huanxung.cn

[K08] 二进制序列化（非 JSON）
来源：http://yl.gzmigu.cn

Py:   pickle.dumps(obj)
来源：http://cn.newstarts.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ma.hnjuh.cn

JS:   v8.serialize(obj)        // Node
来源：http://bj.huixiangedu.cn

TS:   v8.serialize(obj)        // Node
来源：http://si.bjjhwx.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://yl.shtwfgs.cn

Go:   encoding/gob
来源：http://eb.521024.cn

Ruby: Marshal.dump(obj)
来源：http://qh.szsharing.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://lo.colortex.cn

================================================================================
来源：http://ge.jctech888.com.cn

L. 网络请求
来源：http://rm.bjjhwx.cn

================================================================================
来源：http://hr.asd995.cn

[L01] 发送 GET 请求
来源：http://xz.chemitech.net.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://vq.yuntaijiaju.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://na.bookmarksfly.cn

JS:   await fetch(url)
来源：http://ld.newstarts.cn

TS:   await fetch(url)
来源：http://tm.nszjky.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://kb.hnjuh.cn

Go:   resp, err := http.Get(url)
来源：http://wo.shxzskj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ow.jianghongdianzi.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mp.asd995.cn

[L02] 发送 POST JSON
来源：http://dt.huixinmuqiang.cn

Py:   requests.post(url, json={"a": 1})
来源：http://gk.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://dt.wgjwhj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hm.newstarts.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bi.gzmigu.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ec.bookmarksfly.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://na.panjiajie.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hb.yuexingan06.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://jl.colortex.cn

[L03] 设置自定义请求头
来源：http://lt.huixinmuqiang.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://fw.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hc.huixiangedu.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gd.nszjky.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://je.chemitech.net.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ct.asd995.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wz.haigaiapp.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ov.9csxet.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://bt.jianghongdianzi.cn

[L04] 设置超时
来源：http://ok.huixiangedu.cn

Py:   requests.get(url, timeout=5)
来源：http://rx.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://by.bjjhwx.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pv.panjiajie.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://oe.panjiajie.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hw.nszjky.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://tl.hnjuh.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://xs.szsharing.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://di.muxihuayi.cn

[L05] 上传文件（multipart）
来源：http://nn.bookmarksfly.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hl.gzmigu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://dv.nicolike.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://da.szxytkj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hj.huanxung.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://qy.hnjuh.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://bq.lnxyls.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://we.9csxet.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://kh.bookmarksfly.cn

[L06] 解析响应为 JSON
来源：http://dn.bjjhwx.cn

Py:   resp.json()
来源：http://zs.szsharing.cn

PHP:  json_decode($body, true);
来源：http://is.shxzukj.cn

JS:   await resp.json()
来源：http://mm.9csxet.cn

TS:   await resp.json()
来源：http://ym.521024.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://by.bookmarksfly.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://vu.521024.cn

Ruby: JSON.parse(resp.body)
来源：http://kw.szsharing.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://jx.huanxung.cn

[L07] 处理 HTTP 状态码
来源：http://aw.hahajie.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://rl.haigaiapp.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ci.nicolike.cn

JS:   resp.ok;  resp.status
来源：http://wo.chemitech.net.cn

TS:   resp.ok;  resp.status
来源：http://yn.haigaiapp.cn

Java: resp.statusCode()
来源：http://tc.jctech888.com.cn

Go:   resp.StatusCode
来源：http://he.shxzskj.cn

Ruby: resp.code.to_i
来源：http://ae.shxzskj.cn

C#:   (int)resp.StatusCode
来源：http://jo.wgjwhj.cn

[L08] 并发请求多个地址
来源：http://hu.panjiajie.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hs.huanxung.cn

PHP:  curl_multi_init() 系列
来源：http://do.panjiajie.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jr.colortex.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ra.huixiangedu.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ir.hnjuh.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://zk.huixinmuqiang.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mf.521024.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://us.shxzskj.cn

================================================================================
来源：http://pa.hahajie.cn

M. 命令行 / 进程 / 环境
来源：http://it.nszjky.cn

================================================================================
来源：http://fy.gzmigu.cn

[M01] 读取命令行参数
来源：http://nh.asd995.cn

Py:   sys.argv[1:]
来源：http://eg.jctech888.com.cn

PHP:  $argv;  $argc;
来源：http://av.shxzskj.cn

JS:   process.argv.slice(2)
来源：http://od.521024.cn

TS:   process.argv.slice(2)
来源：http://pq.panjiajie.cn

Java: args 数组（main 方法参数）
来源：http://gs.gzmigu.cn

Go:   os.Args[1:]
来源：http://ug.panjiajie.cn

Ruby: ARGV
来源：http://qv.hnjuh.cn

C#:   args 数组（Main 方法参数）
来源：http://om.jianghongdianzi.cn

[M02] 读取环境变量
来源：http://uq.panjiajie.cn

Py:   os.environ.get("HOME")
来源：http://jm.jianghongdianzi.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://tp.shtwfgs.cn

JS:   process.env.HOME
来源：http://iy.huanxung.cn

TS:   process.env.HOME
来源：http://bh.panjiajie.cn

Java: System.getenv("HOME")
来源：http://wd.shxzskj.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://fr.muxihuayi.cn

Ruby: ENV["HOME"]
来源：http://vn.wgjwhj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://tj.bjjhwx.cn

[M03] 执行外部命令
来源：http://pj.newstarts.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://nk.shxzskj.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://jx.colortex.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ba.shxzskj.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ga.haigaiapp.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://bu.yuntaijiaju.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://kr.hnjuh.cn

Ruby: system("ls -l");  `ls -l`
来源：http://wf.shtwfgs.cn

C#:   Process.Start("ls", "-l");
来源：http://xt.bookmarksfly.cn

[M04] 获取当前工作目录
来源：http://xl.wgjwhj.cn

Py:   os.getcwd()
来源：http://sb.yuexingan06.cn

PHP:  getcwd();
来源：http://rl.newstarts.cn

JS:   process.cwd()
来源：http://dl.jianghongdianzi.cn

TS:   process.cwd()
来源：http://pg.szsharing.cn

Java: Path.of("").toAbsolutePath()
来源：http://qz.chemitech.net.cn

Go:   os.Getwd()
来源：http://tz.muxihuayi.cn

Ruby: Dir.pwd
来源：http://dd.asd995.cn

C#:   Directory.GetCurrentDirectory()
来源：http://zu.szsharing.cn

[M05] 设置退出码
来源：http://kh.newstarts.cn

Py:   sys.exit(1)
来源：http://zh.jctech888.com.cn

PHP:  exit(1);
来源：http://kf.hnjuh.cn

JS:   process.exit(1)
来源：http://zi.jctech888.com.cn

TS:   process.exit(1)
来源：http://pe.bookmarksfly.cn

Java: System.exit(1)
来源：http://ww.wgjwhj.cn

Go:   os.Exit(1)
来源：http://yo.gzmigu.cn

Ruby: exit 1
来源：http://kw.asd995.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ge.hnjuh.cn

[M06] 向标准错误输出
来源：http://xz.jianghongdianzi.cn

Py:   print("err", file=sys.stderr)
来源：http://vi.hahajie.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://fs.szsharing.cn

JS:   console.error("err")
来源：http://aa.huixinmuqiang.cn

TS:   console.error("err")
来源：http://ss.nszjky.cn

Java: System.err.println("err")
来源：http://lx.nicolike.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://zc.nicolike.cn

Ruby: warn "err"
来源：http://ge.asd995.cn

C#:   Console.Error.WriteLine("err")
来源：http://zf.szsharing.cn

[M07] 判断是否为主入口
来源：http://hu.chemitech.net.cn

Py:   if __name__ == "__main__":
来源：http://el.shxzskj.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://bk.muxihuayi.cn

JS:   require.main === module
来源：http://uq.chemitech.net.cn

TS:   require.main === module
来源：http://io.szxytkj.cn

Java: public static void main(String[] args)
来源：http://ki.haigaiapp.cn

Go:   func main()
来源：http://xe.jctech888.com.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://dv.jctech888.com.cn

C#:   static void Main(string[] args)
来源：http://ea.gzmigu.cn

[M08] 获取系统与运行时信息
来源：http://bq.szxytkj.cn

Py:   platform.system();  platform.python_version()
来源：http://kq.hnjuh.cn

PHP:  PHP_OS;  phpversion();
来源：http://gc.asd995.cn

JS:   process.platform;  process.version
来源：http://ic.9csxet.cn

TS:   process.platform;  process.version
来源：http://im.9csxet.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://im.gzmigu.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://in.nszjky.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ig.nicolike.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://qn.bjjhwx.cn

================================================================================
来源：http://mk.shtwfgs.cn

N. 数据结构与算法
来源：http://qi.yuntaijiaju.cn

================================================================================
来源：http://mf.shxzukj.cn

[N01] 二分查找（有序数组）
来源：http://rc.muxihuayi.cn

Py:   bisect.bisect_left(arr, x)
来源：http://je.huixiangedu.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://jr.shxzskj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ac.bookmarksfly.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dq.asd995.cn

Java: Arrays.binarySearch(arr, x)
来源：http://xn.wgjwhj.cn

Go:   sort.SearchInts(arr, x)
来源：http://yh.panjiajie.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://bf.yuexingan06.cn

C#:   Array.BinarySearch(arr, x)
来源：http://od.huanxung.cn

[N02] 排序（工程实践用内置实现）
来源：http://qb.bookmarksfly.cn

Py:   sorted(arr);  arr.sort()
来源：http://is.hahajie.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://jw.asd995.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://fj.muxihuayi.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ep.huixinmuqiang.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://dg.9csxet.cn

Go:   slices.Sort(arr)
来源：http://wn.yuntaijiaju.cn

Ruby: arr.sort
来源：http://ce.521024.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://jd.yuexingan06.cn

[N03] 快速排序（分治示例）
来源：http://sd.9csxet.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hc.gzmigu.cn

PHP:  // 递归实现，或用 usort
来源：http://ph.szxytkj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ba.nicolike.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://iq.shxzskj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wg.haigaiapp.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://uk.shxzukj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://sj.jctech888.com.cn

C#:   // 手写递归，或 Array.Sort
来源：http://sv.yuexingan06.cn

[N04] 斐波那契数列
来源：http://ka.lnxyls.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ac.muxihuayi.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://uy.9csxet.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lx.muxihuayi.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://uk.lnxyls.cn


<!-- 参考信息 -->