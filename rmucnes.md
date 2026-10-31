代发 wailian999

Java: Duration.between(start, end).toSeconds()
来源：http://pj.asd995.cn

Go:   end.Sub(start).Hours()
来源：http://oj.yuntaijiaju.cn

Ruby: end - start                 # 返回秒数
来源：http://vh.muxihuayi.cn

C#:   (end - start).TotalSeconds
来源：http://vw.521024.cn

[J07] 比较两个日期
来源：http://ze.yuntaijiaju.cn

Py:   d1 < d2;  d1 == d2
来源：http://kv.lnxyls.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wx.panjiajie.cn

JS:   d1.getTime() < d2.getTime()
来源：http://hn.huanxung.cn

TS:   d1.getTime() < d2.getTime()
来源：http://xq.asd995.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://jn.9csxet.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ti.jctech888.com.cn

Ruby: d1 < d2;  d1 == d2
来源：http://kf.huixiangedu.cn

C#:   d1 < d2;  d1 == d2
来源：http://yg.jianghongdianzi.cn

[J08] 提取年月日与星期
来源：http://hx.nszjky.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://fj.newstarts.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://fv.yuntaijiaju.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://fz.shtwfgs.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ti.yuntaijiaju.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mm.nszjky.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://sx.huixinmuqiang.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://pq.bookmarksfly.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mw.jianghongdianzi.cn

[J09] 时区处理
来源：http://xk.wgjwhj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://rg.huixiangedu.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://of.newstarts.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mh.bookmarksfly.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mt.hahajie.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hl.yuexingan06.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ag.panjiajie.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ko.nszjky.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://da.9csxet.cn

[J10] 取今天 / 本月第一天
来源：http://nc.muxihuayi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ys.wgjwhj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://nq.huixinmuqiang.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://zc.nicolike.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://je.521024.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hr.asd995.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://cu.521024.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vv.muxihuayi.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://br.szsharing.cn

================================================================================
来源：http://ca.hnjuh.cn

K. JSON 与序列化
来源：http://yn.chemitech.net.cn

================================================================================
来源：http://jx.lnxyls.cn

[K01] 对象转 JSON 字符串
来源：http://li.shxzukj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://gb.nicolike.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://yr.gzmigu.cn

JS:   JSON.stringify(obj)
来源：http://al.nszjky.cn

TS:   JSON.stringify(obj)
来源：http://hz.huixinmuqiang.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://gu.jctech888.com.cn

Go:   json.Marshal(obj)
来源：http://sn.huanxung.cn

Ruby: obj.to_json                                     // require "json"
来源：http://vr.gzmigu.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://rh.colortex.cn

[K02] JSON 字符串转对象
来源：http://sv.huixinmuqiang.cn

Py:   json.loads(s)
来源：http://nc.huanxung.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wv.jianghongdianzi.cn

JS:   JSON.parse(s)
来源：http://hr.haigaiapp.cn

TS:   JSON.parse(s)
来源：http://ky.gzmigu.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qw.bookmarksfly.cn

Go:   json.Unmarshal(data, &v)
来源：http://rk.hahajie.cn

Ruby: JSON.parse(s)
来源：http://cr.shtwfgs.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://fx.asd995.cn

[K03] JSON 美化输出（带缩进）
来源：http://pr.chemitech.net.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://pm.lnxyls.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mb.szxytkj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://xj.shxzskj.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://zh.huixiangedu.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://gp.haigaiapp.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ex.shxzukj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://wq.bjjhwx.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://bo.chemitech.net.cn

[K04] 读取 JSON 文件
来源：http://xk.szxytkj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://gv.shxzukj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://rj.hahajie.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://om.chemitech.net.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gz.shxzukj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://fb.wgjwhj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://tq.szsharing.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://gw.bjjhwx.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://cd.nicolike.cn

[K05] 深拷贝对象
来源：http://cv.panjiajie.cn

Py:   copy.deepcopy(obj)
来源：http://mi.bjjhwx.cn

PHP:  unserialize(serialize($obj));
来源：http://ef.wgjwhj.cn

JS:   structuredClone(obj)
来源：http://jj.gzmigu.cn

TS:   structuredClone(obj)
来源：http://fn.yuntaijiaju.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://no.huixiangedu.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://xn.szxytkj.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://qg.nicolike.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ys.yuntaijiaju.cn

[K06] 解析 URL 查询串
来源：http://ce.jctech888.com.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://kw.chemitech.net.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mx.hnjuh.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mn.hnjuh.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cc.haigaiapp.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://nm.huixiangedu.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://zc.yuntaijiaju.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vk.shxzskj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://si.yuexingan06.cn

[K07] 进制转换
来源：http://ts.hnjuh.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://qk.huixinmuqiang.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hd.hahajie.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wi.521024.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://dg.chemitech.net.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://jg.nszjky.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://pw.nszjky.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://xe.nszjky.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://av.bookmarksfly.cn

[K08] 二进制序列化（非 JSON）
来源：http://xw.huixiangedu.cn

Py:   pickle.dumps(obj)
来源：http://yz.newstarts.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://jf.gzmigu.cn

JS:   v8.serialize(obj)        // Node
来源：http://be.bookmarksfly.cn

TS:   v8.serialize(obj)        // Node
来源：http://zv.asd995.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://yo.wgjwhj.cn

Go:   encoding/gob
来源：http://ut.shxzukj.cn

Ruby: Marshal.dump(obj)
来源：http://ks.muxihuayi.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://gi.jctech888.com.cn

================================================================================
来源：http://ls.gzmigu.cn

L. 网络请求
来源：http://ko.bookmarksfly.cn

================================================================================
来源：http://xt.yuexingan06.cn

[L01] 发送 GET 请求
来源：http://bg.bjjhwx.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jp.hnjuh.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://gh.shxzskj.cn

JS:   await fetch(url)
来源：http://bq.521024.cn

TS:   await fetch(url)
来源：http://ug.panjiajie.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://kz.lnxyls.cn

Go:   resp, err := http.Get(url)
来源：http://zh.szsharing.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://lc.bookmarksfly.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wd.shxzskj.cn

[L02] 发送 POST JSON
来源：http://mj.huixinmuqiang.cn

Py:   requests.post(url, json={"a": 1})
来源：http://kr.panjiajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://vr.huixinmuqiang.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ay.huixiangedu.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hv.muxihuayi.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vx.lnxyls.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://uo.panjiajie.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hb.yuexingan06.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://zh.huixiangedu.cn

[L03] 设置自定义请求头
来源：http://bv.shxzskj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://fl.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hd.yuntaijiaju.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://iy.hnjuh.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://td.newstarts.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://gl.9csxet.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ms.nszjky.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://tq.lnxyls.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://qy.panjiajie.cn

[L04] 设置超时
来源：http://ba.newstarts.cn

Py:   requests.get(url, timeout=5)
来源：http://dk.szsharing.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://yr.panjiajie.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cg.muxihuayi.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://eb.huixinmuqiang.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://oe.9csxet.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ks.haigaiapp.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://fl.jianghongdianzi.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ld.chemitech.net.cn

[L05] 上传文件（multipart）
来源：http://ah.chemitech.net.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://er.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ga.huixiangedu.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://lz.jctech888.com.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://dx.szxytkj.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ry.panjiajie.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://zr.9csxet.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://sv.lnxyls.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://gg.szsharing.cn

[L06] 解析响应为 JSON
来源：http://sa.huanxung.cn

Py:   resp.json()
来源：http://vc.yuexingan06.cn

PHP:  json_decode($body, true);
来源：http://ie.521024.cn

JS:   await resp.json()
来源：http://wb.chemitech.net.cn

TS:   await resp.json()
来源：http://pj.jctech888.com.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://bp.szsharing.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hj.colortex.cn

Ruby: JSON.parse(resp.body)
来源：http://yl.bookmarksfly.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ia.nicolike.cn

[L07] 处理 HTTP 状态码
来源：http://ep.gzmigu.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ej.huanxung.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ij.haigaiapp.cn

JS:   resp.ok;  resp.status
来源：http://cq.gzmigu.cn

TS:   resp.ok;  resp.status
来源：http://xm.szsharing.cn

Java: resp.statusCode()
来源：http://th.huixinmuqiang.cn

Go:   resp.StatusCode
来源：http://mk.jianghongdianzi.cn

Ruby: resp.code.to_i
来源：http://tq.newstarts.cn

C#:   (int)resp.StatusCode
来源：http://bi.521024.cn

[L08] 并发请求多个地址
来源：http://et.nszjky.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wd.lnxyls.cn

PHP:  curl_multi_init() 系列
来源：http://yh.jctech888.com.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://se.nszjky.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lt.szxytkj.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://tf.colortex.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://sl.haigaiapp.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://cj.panjiajie.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xs.szsharing.cn

================================================================================
来源：http://ew.shxzukj.cn

M. 命令行 / 进程 / 环境
来源：http://jk.shxzskj.cn

================================================================================
来源：http://sw.bookmarksfly.cn

[M01] 读取命令行参数
来源：http://bq.9csxet.cn

Py:   sys.argv[1:]
来源：http://qu.muxihuayi.cn

PHP:  $argv;  $argc;
来源：http://bq.colortex.cn

JS:   process.argv.slice(2)
来源：http://ih.nicolike.cn

TS:   process.argv.slice(2)
来源：http://lw.yuexingan06.cn

Java: args 数组（main 方法参数）
来源：http://ec.bjjhwx.cn

Go:   os.Args[1:]
来源：http://vw.huanxung.cn

Ruby: ARGV
来源：http://dw.shxzskj.cn

C#:   args 数组（Main 方法参数）
来源：http://nk.panjiajie.cn

[M02] 读取环境变量
来源：http://nf.yuexingan06.cn

Py:   os.environ.get("HOME")
来源：http://pb.wgjwhj.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wr.jianghongdianzi.cn

JS:   process.env.HOME
来源：http://nf.colortex.cn

TS:   process.env.HOME
来源：http://ty.chemitech.net.cn

Java: System.getenv("HOME")
来源：http://fg.bookmarksfly.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://za.huixinmuqiang.cn

Ruby: ENV["HOME"]
来源：http://cf.jianghongdianzi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://re.szxytkj.cn

[M03] 执行外部命令
来源：http://az.jianghongdianzi.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://dj.colortex.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://pu.shxzskj.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://jb.jianghongdianzi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://je.newstarts.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://an.huanxung.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://kc.hnjuh.cn

Ruby: system("ls -l");  `ls -l`
来源：http://xp.shxzskj.cn

C#:   Process.Start("ls", "-l");
来源：http://ni.huixinmuqiang.cn

[M04] 获取当前工作目录
来源：http://fv.hnjuh.cn

Py:   os.getcwd()
来源：http://su.haigaiapp.cn

PHP:  getcwd();
来源：http://ru.huixiangedu.cn

JS:   process.cwd()
来源：http://pz.muxihuayi.cn

TS:   process.cwd()
来源：http://vh.huixinmuqiang.cn

Java: Path.of("").toAbsolutePath()
来源：http://dr.nicolike.cn

Go:   os.Getwd()
来源：http://om.huixinmuqiang.cn

Ruby: Dir.pwd
来源：http://ll.hahajie.cn

C#:   Directory.GetCurrentDirectory()
来源：http://bd.521024.cn

[M05] 设置退出码
来源：http://wb.wgjwhj.cn

Py:   sys.exit(1)
来源：http://vk.9csxet.cn

PHP:  exit(1);
来源：http://nz.wgjwhj.cn

JS:   process.exit(1)
来源：http://yo.newstarts.cn

TS:   process.exit(1)
来源：http://pq.yuntaijiaju.cn

Java: System.exit(1)
来源：http://vc.9csxet.cn

Go:   os.Exit(1)
来源：http://wa.chemitech.net.cn

Ruby: exit 1
来源：http://nt.chemitech.net.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://yj.huixinmuqiang.cn

[M06] 向标准错误输出
来源：http://zq.panjiajie.cn

Py:   print("err", file=sys.stderr)
来源：http://lr.yuexingan06.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://uc.bookmarksfly.cn

JS:   console.error("err")
来源：http://lf.asd995.cn

TS:   console.error("err")
来源：http://qi.huixinmuqiang.cn

Java: System.err.println("err")
来源：http://pk.panjiajie.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://cb.jianghongdianzi.cn

Ruby: warn "err"
来源：http://jo.shxzukj.cn

C#:   Console.Error.WriteLine("err")
来源：http://vm.521024.cn

[M07] 判断是否为主入口
来源：http://rr.gzmigu.cn

Py:   if __name__ == "__main__":
来源：http://ya.shxzskj.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://rk.yuntaijiaju.cn

JS:   require.main === module
来源：http://qn.521024.cn

TS:   require.main === module
来源：http://le.szxytkj.cn

Java: public static void main(String[] args)
来源：http://ka.muxihuayi.cn

Go:   func main()
来源：http://tz.panjiajie.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://lh.jctech888.com.cn

C#:   static void Main(string[] args)
来源：http://xh.asd995.cn

[M08] 获取系统与运行时信息
来源：http://cr.wgjwhj.cn

Py:   platform.system();  platform.python_version()
来源：http://oi.nicolike.cn

PHP:  PHP_OS;  phpversion();
来源：http://sp.szxytkj.cn

JS:   process.platform;  process.version
来源：http://tz.lnxyls.cn

TS:   process.platform;  process.version
来源：http://uc.chemitech.net.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://vq.bjjhwx.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ni.huixiangedu.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://dp.yuntaijiaju.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://mc.jctech888.com.cn

================================================================================
来源：http://xj.lnxyls.cn

N. 数据结构与算法
来源：http://pz.yuntaijiaju.cn

================================================================================
来源：http://ay.hnjuh.cn

[N01] 二分查找（有序数组）
来源：http://th.panjiajie.cn

Py:   bisect.bisect_left(arr, x)
来源：http://my.colortex.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://jb.haigaiapp.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ls.newstarts.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ir.panjiajie.cn

Java: Arrays.binarySearch(arr, x)
来源：http://zj.huanxung.cn

Go:   sort.SearchInts(arr, x)
来源：http://fx.szsharing.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://kn.yuexingan06.cn

C#:   Array.BinarySearch(arr, x)
来源：http://wa.szxytkj.cn

[N02] 排序（工程实践用内置实现）
来源：http://wj.szsharing.cn

Py:   sorted(arr);  arr.sort()
来源：http://db.colortex.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://vs.huixinmuqiang.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://nd.colortex.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://no.asd995.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://uq.9csxet.cn

Go:   slices.Sort(arr)
来源：http://da.yuntaijiaju.cn

Ruby: arr.sort
来源：http://vq.bookmarksfly.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://oq.jianghongdianzi.cn

[N03] 快速排序（分治示例）
来源：http://ls.shxzukj.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://yn.jianghongdianzi.cn

PHP:  // 递归实现，或用 usort
来源：http://jf.gzmigu.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wp.nszjky.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jo.wgjwhj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://kg.bjjhwx.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://fk.shtwfgs.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://dh.muxihuayi.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ms.jctech888.com.cn

[N04] 斐波那契数列
来源：http://zs.szsharing.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qw.9csxet.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://fd.asd995.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ys.asd995.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fn.bookmarksfly.cn


<!-- 参考信息 -->