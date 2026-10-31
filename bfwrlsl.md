代发 wailian999

PHP:  (new DateTime())->modify("+7 days");
来源：http://fn.nszjky.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://im.hahajie.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ur.haigaiapp.cn

Java: LocalDate.now().plusDays(7)
来源：http://ki.bjjhwx.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://gb.jctech888.com.cn

Ruby: Time.now + 7 * 86400
来源：http://ug.shxzskj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://iy.asd995.cn

[J06] 计算两时间之差
来源：http://sh.muxihuayi.cn

Py:   (end - start).total_seconds()
来源：http://vw.hnjuh.cn

PHP:  $end->diff($start)->days;
来源：http://ux.huixiangedu.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mm.wgjwhj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://bp.bjjhwx.cn

Java: Duration.between(start, end).toSeconds()
来源：http://mk.9csxet.cn

Go:   end.Sub(start).Hours()
来源：http://wz.shxzukj.cn

Ruby: end - start                 # 返回秒数
来源：http://xe.lnxyls.cn

C#:   (end - start).TotalSeconds
来源：http://xa.nicolike.cn

[J07] 比较两个日期
来源：http://ql.yuexingan06.cn

Py:   d1 < d2;  d1 == d2
来源：http://fs.9csxet.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://yl.shxzukj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://mw.lnxyls.cn

TS:   d1.getTime() < d2.getTime()
来源：http://zi.shtwfgs.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://al.shxzukj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://fk.hahajie.cn

Ruby: d1 < d2;  d1 == d2
来源：http://tp.shtwfgs.cn

C#:   d1 < d2;  d1 == d2
来源：http://lg.shxzukj.cn

[J08] 提取年月日与星期
来源：http://fn.asd995.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://kg.huixiangedu.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://qk.shxzskj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xv.asd995.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://am.huixinmuqiang.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://yw.newstarts.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://zq.9csxet.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ws.gzmigu.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wv.9csxet.cn

[J09] 时区处理
来源：http://bg.yuntaijiaju.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://oa.shtwfgs.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://kc.yuntaijiaju.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fy.asd995.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bo.huixiangedu.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://np.asd995.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ug.wgjwhj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ij.shxzukj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://bf.shxzskj.cn

[J10] 取今天 / 本月第一天
来源：http://vd.yuntaijiaju.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://by.huixiangedu.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://yk.9csxet.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vj.nszjky.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://lu.wgjwhj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://vs.newstarts.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://us.hnjuh.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://uv.shxzskj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ys.wgjwhj.cn

================================================================================
来源：http://nh.muxihuayi.cn

K. JSON 与序列化
来源：http://jv.shxzskj.cn

================================================================================
来源：http://wt.bookmarksfly.cn

[K01] 对象转 JSON 字符串
来源：http://hr.jianghongdianzi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://xl.wgjwhj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://tv.newstarts.cn

JS:   JSON.stringify(obj)
来源：http://te.shxzukj.cn

TS:   JSON.stringify(obj)
来源：http://oj.szsharing.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://aq.shxzskj.cn

Go:   json.Marshal(obj)
来源：http://dr.muxihuayi.cn

Ruby: obj.to_json                                     // require "json"
来源：http://rx.chemitech.net.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://fe.bookmarksfly.cn

[K02] JSON 字符串转对象
来源：http://pk.muxihuayi.cn

Py:   json.loads(s)
来源：http://wd.asd995.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://dr.nszjky.cn

JS:   JSON.parse(s)
来源：http://wu.gzmigu.cn

TS:   JSON.parse(s)
来源：http://ao.hnjuh.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hv.colortex.cn

Go:   json.Unmarshal(data, &v)
来源：http://ri.yuexingan06.cn

Ruby: JSON.parse(s)
来源：http://kj.lnxyls.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qu.bjjhwx.cn

[K03] JSON 美化输出（带缩进）
来源：http://ge.szsharing.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://pt.gzmigu.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://fl.szsharing.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://jk.yuntaijiaju.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://vo.newstarts.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://sc.hahajie.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ot.muxihuayi.cn

Ruby: JSON.pretty_generate(obj)
来源：http://pm.huixiangedu.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ee.bjjhwx.cn

[K04] 读取 JSON 文件
来源：http://jo.chemitech.net.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hk.yuexingan06.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://vw.huixiangedu.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qu.szsharing.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jq.huixinmuqiang.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://gj.shxzskj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://bb.szsharing.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://eq.szxytkj.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://xg.hahajie.cn

[K05] 深拷贝对象
来源：http://ms.hahajie.cn

Py:   copy.deepcopy(obj)
来源：http://xi.colortex.cn

PHP:  unserialize(serialize($obj));
来源：http://dk.wgjwhj.cn

JS:   structuredClone(obj)
来源：http://io.bjjhwx.cn

TS:   structuredClone(obj)
来源：http://dr.jctech888.com.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://rw.huixiangedu.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wc.muxihuayi.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://oz.asd995.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://iy.chemitech.net.cn

[K06] 解析 URL 查询串
来源：http://wf.lnxyls.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ea.hnjuh.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mx.yuexingan06.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dy.hahajie.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://no.newstarts.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ft.shtwfgs.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://td.chemitech.net.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.521024.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://pp.haigaiapp.cn

[K07] 进制转换
来源：http://lg.jianghongdianzi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ek.chemitech.net.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://fs.huixinmuqiang.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ww.chemitech.net.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://oz.huixiangedu.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://vk.bjjhwx.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://jb.huanxung.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://fl.huixiangedu.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://nf.nicolike.cn

[K08] 二进制序列化（非 JSON）
来源：http://dp.shxzskj.cn

Py:   pickle.dumps(obj)
来源：http://eq.asd995.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ym.huanxung.cn

JS:   v8.serialize(obj)        // Node
来源：http://jq.yuexingan06.cn

TS:   v8.serialize(obj)        // Node
来源：http://tq.jctech888.com.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://oj.shxzskj.cn

Go:   encoding/gob
来源：http://yy.yuntaijiaju.cn

Ruby: Marshal.dump(obj)
来源：http://yi.newstarts.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://no.shtwfgs.cn

================================================================================
来源：http://qy.shxzukj.cn

L. 网络请求
来源：http://oa.muxihuayi.cn

================================================================================
来源：http://pr.asd995.cn

[L01] 发送 GET 请求
来源：http://ed.shxzukj.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ic.haigaiapp.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://di.szsharing.cn

JS:   await fetch(url)
来源：http://rl.muxihuayi.cn

TS:   await fetch(url)
来源：http://zp.szsharing.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qs.colortex.cn

Go:   resp, err := http.Get(url)
来源：http://di.newstarts.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://dp.shxzskj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://rn.jctech888.com.cn

[L02] 发送 POST JSON
来源：http://uz.huixiangedu.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ho.asd995.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ee.szsharing.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gi.huixiangedu.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ru.panjiajie.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ve.hnjuh.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://zk.shtwfgs.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xi.huixinmuqiang.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://kx.szxytkj.cn

[L03] 设置自定义请求头
来源：http://ip.nicolike.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://qj.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://lw.jctech888.com.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://oq.huanxung.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sk.panjiajie.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://jv.shtwfgs.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://bd.9csxet.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://xf.shtwfgs.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://zq.9csxet.cn

[L04] 设置超时
来源：http://xy.nicolike.cn

Py:   requests.get(url, timeout=5)
来源：http://qb.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://bg.szsharing.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pg.bookmarksfly.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pf.bjjhwx.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qc.bjjhwx.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://je.yuexingan06.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://dr.nszjky.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ji.lnxyls.cn

[L05] 上传文件（multipart）
来源：http://ae.huixiangedu.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://oq.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://se.gzmigu.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ep.huixiangedu.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://eb.szsharing.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://fq.bookmarksfly.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://lf.nszjky.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vj.huanxung.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ii.szxytkj.cn

[L06] 解析响应为 JSON
来源：http://rv.hahajie.cn

Py:   resp.json()
来源：http://qv.asd995.cn

PHP:  json_decode($body, true);
来源：http://uw.shxzukj.cn

JS:   await resp.json()
来源：http://ul.jctech888.com.cn

TS:   await resp.json()
来源：http://iy.newstarts.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ju.szxytkj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://px.lnxyls.cn

Ruby: JSON.parse(resp.body)
来源：http://am.lnxyls.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ln.huixinmuqiang.cn

[L07] 处理 HTTP 状态码
来源：http://mp.nicolike.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://sb.shxzukj.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qu.yuexingan06.cn

JS:   resp.ok;  resp.status
来源：http://mb.asd995.cn

TS:   resp.ok;  resp.status
来源：http://oy.9csxet.cn

Java: resp.statusCode()
来源：http://av.shxzukj.cn

Go:   resp.StatusCode
来源：http://tq.wgjwhj.cn

Ruby: resp.code.to_i
来源：http://ts.9csxet.cn

C#:   (int)resp.StatusCode
来源：http://aw.hahajie.cn

[L08] 并发请求多个地址
来源：http://fx.9csxet.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://up.huixinmuqiang.cn

PHP:  curl_multi_init() 系列
来源：http://sc.shxzukj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wt.jctech888.com.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qe.panjiajie.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://sc.yuntaijiaju.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ei.shxzskj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://sr.hnjuh.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://aw.nicolike.cn

================================================================================
来源：http://tl.szxytkj.cn

M. 命令行 / 进程 / 环境
来源：http://os.colortex.cn

================================================================================
来源：http://jw.muxihuayi.cn

[M01] 读取命令行参数
来源：http://dj.huixinmuqiang.cn

Py:   sys.argv[1:]
来源：http://nl.colortex.cn

PHP:  $argv;  $argc;
来源：http://eh.bookmarksfly.cn

JS:   process.argv.slice(2)
来源：http://iu.shxzskj.cn

TS:   process.argv.slice(2)
来源：http://zc.muxihuayi.cn

Java: args 数组（main 方法参数）
来源：http://ba.bjjhwx.cn

Go:   os.Args[1:]
来源：http://ir.521024.cn

Ruby: ARGV
来源：http://bj.huanxung.cn

C#:   args 数组（Main 方法参数）
来源：http://kf.huixinmuqiang.cn

[M02] 读取环境变量
来源：http://ay.huixiangedu.cn

Py:   os.environ.get("HOME")
来源：http://lm.nicolike.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rs.bookmarksfly.cn

JS:   process.env.HOME
来源：http://lx.yuexingan06.cn

TS:   process.env.HOME
来源：http://tj.chemitech.net.cn

Java: System.getenv("HOME")
来源：http://hp.huanxung.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://dh.chemitech.net.cn

Ruby: ENV["HOME"]
来源：http://mf.colortex.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ms.lnxyls.cn

[M03] 执行外部命令
来源：http://wf.huanxung.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://zz.yuntaijiaju.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://eb.lnxyls.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://wq.nszjky.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ic.bookmarksfly.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://nh.huixiangedu.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://xc.jctech888.com.cn

Ruby: system("ls -l");  `ls -l`
来源：http://sp.jianghongdianzi.cn

C#:   Process.Start("ls", "-l");
来源：http://ys.shxzukj.cn

[M04] 获取当前工作目录
来源：http://zw.haigaiapp.cn

Py:   os.getcwd()
来源：http://by.gzmigu.cn

PHP:  getcwd();
来源：http://ah.lnxyls.cn

JS:   process.cwd()
来源：http://zd.yuntaijiaju.cn

TS:   process.cwd()
来源：http://ur.huanxung.cn

Java: Path.of("").toAbsolutePath()
来源：http://pr.huanxung.cn

Go:   os.Getwd()
来源：http://xo.huixiangedu.cn

Ruby: Dir.pwd
来源：http://ny.shxzskj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://fg.huanxung.cn

[M05] 设置退出码
来源：http://kx.huixinmuqiang.cn

Py:   sys.exit(1)
来源：http://az.szxytkj.cn

PHP:  exit(1);
来源：http://wp.jctech888.com.cn

JS:   process.exit(1)
来源：http://rz.bookmarksfly.cn

TS:   process.exit(1)
来源：http://da.521024.cn

Java: System.exit(1)
来源：http://in.szsharing.cn

Go:   os.Exit(1)
来源：http://th.asd995.cn

Ruby: exit 1
来源：http://ey.gzmigu.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://sd.nszjky.cn

[M06] 向标准错误输出
来源：http://iq.nszjky.cn

Py:   print("err", file=sys.stderr)
来源：http://dq.9csxet.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://nb.shxzskj.cn

JS:   console.error("err")
来源：http://jz.9csxet.cn

TS:   console.error("err")
来源：http://pn.newstarts.cn

Java: System.err.println("err")
来源：http://ya.lnxyls.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://vf.huanxung.cn

Ruby: warn "err"
来源：http://le.jianghongdianzi.cn

C#:   Console.Error.WriteLine("err")
来源：http://yy.nicolike.cn

[M07] 判断是否为主入口
来源：http://cj.newstarts.cn

Py:   if __name__ == "__main__":
来源：http://gr.jctech888.com.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://gd.gzmigu.cn

JS:   require.main === module
来源：http://gx.huixinmuqiang.cn

TS:   require.main === module
来源：http://aj.9csxet.cn

Java: public static void main(String[] args)
来源：http://ke.huixinmuqiang.cn

Go:   func main()
来源：http://dz.bjjhwx.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hw.lnxyls.cn

C#:   static void Main(string[] args)
来源：http://uh.shtwfgs.cn

[M08] 获取系统与运行时信息
来源：http://rm.szsharing.cn

Py:   platform.system();  platform.python_version()
来源：http://du.panjiajie.cn

PHP:  PHP_OS;  phpversion();
来源：http://dc.newstarts.cn

JS:   process.platform;  process.version
来源：http://ip.colortex.cn

TS:   process.platform;  process.version
来源：http://ok.asd995.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://kh.shxzukj.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://yk.shxzukj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://vh.haigaiapp.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ni.nicolike.cn

================================================================================
来源：http://nq.nicolike.cn

N. 数据结构与算法
来源：http://wp.szsharing.cn

================================================================================
来源：http://vm.hahajie.cn

[N01] 二分查找（有序数组）
来源：http://dt.gzmigu.cn

Py:   bisect.bisect_left(arr, x)
来源：http://an.huanxung.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://lb.huanxung.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://at.gzmigu.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bg.wgjwhj.cn

Java: Arrays.binarySearch(arr, x)
来源：http://lk.jianghongdianzi.cn

Go:   sort.SearchInts(arr, x)
来源：http://xw.shtwfgs.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://er.nszjky.cn

C#:   Array.BinarySearch(arr, x)
来源：http://mi.huanxung.cn

[N02] 排序（工程实践用内置实现）
来源：http://gd.hnjuh.cn

Py:   sorted(arr);  arr.sort()
来源：http://nh.yuntaijiaju.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://xq.gzmigu.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://yu.9csxet.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://qc.jctech888.com.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://vb.colortex.cn

Go:   slices.Sort(arr)
来源：http://zi.szxytkj.cn

Ruby: arr.sort
来源：http://sf.huixiangedu.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://gl.shxzskj.cn

[N03] 快速排序（分治示例）
来源：http://zb.szxytkj.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://fx.bjjhwx.cn


<!-- 参考信息 -->