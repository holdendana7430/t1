代发 wailian999

PHP:  (new DateTime())->modify("+7 days");
来源：http://is.521024.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://uc.lnxyls.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ib.huanxung.cn

Java: LocalDate.now().plusDays(7)
来源：http://mh.szsharing.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://if.9csxet.cn

Ruby: Time.now + 7 * 86400
来源：http://iz.haigaiapp.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ci.shxzukj.cn

[J06] 计算两时间之差
来源：http://lj.shtwfgs.cn

Py:   (end - start).total_seconds()
来源：http://sn.gzmigu.cn

PHP:  $end->diff($start)->days;
来源：http://pi.yuexingan06.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hh.nszjky.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xm.yuexingan06.cn

Java: Duration.between(start, end).toSeconds()
来源：http://fs.nicolike.cn

Go:   end.Sub(start).Hours()
来源：http://js.panjiajie.cn

Ruby: end - start                 # 返回秒数
来源：http://wv.shxzukj.cn

C#:   (end - start).TotalSeconds
来源：http://uj.yuexingan06.cn

[J07] 比较两个日期
来源：http://uz.yuntaijiaju.cn

Py:   d1 < d2;  d1 == d2
来源：http://tw.jianghongdianzi.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ke.colortex.cn

JS:   d1.getTime() < d2.getTime()
来源：http://fo.panjiajie.cn

TS:   d1.getTime() < d2.getTime()
来源：http://aa.yuntaijiaju.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ed.lnxyls.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ae.hnjuh.cn

Ruby: d1 < d2;  d1 == d2
来源：http://am.shxzskj.cn

C#:   d1 < d2;  d1 == d2
来源：http://fx.panjiajie.cn

[J08] 提取年月日与星期
来源：http://zf.jctech888.com.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hp.hnjuh.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://oq.shtwfgs.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://au.gzmigu.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xs.panjiajie.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ro.nicolike.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://cc.gzmigu.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://og.gzmigu.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ig.huixinmuqiang.cn

[J09] 时区处理
来源：http://rn.huixinmuqiang.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ks.nszjky.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://lt.colortex.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pt.jianghongdianzi.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rg.haigaiapp.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://uo.shtwfgs.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://vl.521024.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://tu.panjiajie.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://at.nszjky.cn

[J10] 取今天 / 本月第一天
来源：http://ue.newstarts.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://mx.jctech888.com.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://kb.nicolike.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://zn.muxihuayi.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ds.shxzukj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qg.huixiangedu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ii.asd995.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ir.9csxet.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hl.lnxyls.cn

================================================================================
来源：http://ss.shxzukj.cn

K. JSON 与序列化
来源：http://os.haigaiapp.cn

================================================================================
来源：http://nf.muxihuayi.cn

[K01] 对象转 JSON 字符串
来源：http://ny.chemitech.net.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://fk.shxzskj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wb.shxzukj.cn

JS:   JSON.stringify(obj)
来源：http://gx.hahajie.cn

TS:   JSON.stringify(obj)
来源：http://je.shxzskj.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ve.huixiangedu.cn

Go:   json.Marshal(obj)
来源：http://pi.panjiajie.cn

Ruby: obj.to_json                                     // require "json"
来源：http://dy.chemitech.net.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://uq.lnxyls.cn

[K02] JSON 字符串转对象
来源：http://op.hnjuh.cn

Py:   json.loads(s)
来源：http://pi.lnxyls.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://om.panjiajie.cn

JS:   JSON.parse(s)
来源：http://ak.hnjuh.cn

TS:   JSON.parse(s)
来源：http://ex.asd995.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://zb.nicolike.cn

Go:   json.Unmarshal(data, &v)
来源：http://gy.nszjky.cn

Ruby: JSON.parse(s)
来源：http://ia.521024.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://yb.szsharing.cn

[K03] JSON 美化输出（带缩进）
来源：http://jl.yuntaijiaju.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://qe.newstarts.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://yh.huixinmuqiang.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://sa.asd995.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://qb.huanxung.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://xj.wgjwhj.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://dt.shxzukj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ts.gzmigu.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://pl.huixiangedu.cn

[K04] 读取 JSON 文件
来源：http://ab.9csxet.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://fe.szxytkj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://yv.newstarts.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dt.newstarts.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lj.muxihuayi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://bz.shtwfgs.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mf.shxzskj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://fj.hahajie.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://cg.chemitech.net.cn

[K05] 深拷贝对象
来源：http://zc.gzmigu.cn

Py:   copy.deepcopy(obj)
来源：http://wq.szsharing.cn

PHP:  unserialize(serialize($obj));
来源：http://uj.521024.cn

JS:   structuredClone(obj)
来源：http://za.szsharing.cn

TS:   structuredClone(obj)
来源：http://io.shxzskj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://qn.huixinmuqiang.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ij.panjiajie.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://la.chemitech.net.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://wi.shxzukj.cn

[K06] 解析 URL 查询串
来源：http://kx.lnxyls.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://fl.521024.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mt.shxzukj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ji.muxihuayi.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://it.asd995.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ae.huixiangedu.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://oy.muxihuayi.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://sq.szxytkj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zi.nszjky.cn

[K07] 进制转换
来源：http://ow.wgjwhj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ph.jianghongdianzi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://qj.jianghongdianzi.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://vz.colortex.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://gc.haigaiapp.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://st.huanxung.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://lq.szsharing.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://nb.jctech888.com.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://jb.521024.cn

[K08] 二进制序列化（非 JSON）
来源：http://wc.hnjuh.cn

Py:   pickle.dumps(obj)
来源：http://ao.yuexingan06.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://bb.szxytkj.cn

JS:   v8.serialize(obj)        // Node
来源：http://dx.9csxet.cn

TS:   v8.serialize(obj)        // Node
来源：http://er.yuntaijiaju.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://vy.wgjwhj.cn

Go:   encoding/gob
来源：http://my.szxytkj.cn

Ruby: Marshal.dump(obj)
来源：http://no.huixiangedu.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ro.yuntaijiaju.cn

================================================================================
来源：http://jg.nszjky.cn

L. 网络请求
来源：http://er.haigaiapp.cn

================================================================================
来源：http://sa.nszjky.cn

[L01] 发送 GET 请求
来源：http://sf.jianghongdianzi.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jq.chemitech.net.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://aw.gzmigu.cn

JS:   await fetch(url)
来源：http://tk.nszjky.cn

TS:   await fetch(url)
来源：http://wp.bjjhwx.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wi.szxytkj.cn

Go:   resp, err := http.Get(url)
来源：http://mx.panjiajie.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://nc.bookmarksfly.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://oe.shtwfgs.cn

[L02] 发送 POST JSON
来源：http://hz.yuntaijiaju.cn

Py:   requests.post(url, json={"a": 1})
来源：http://lx.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mw.huixinmuqiang.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fa.lnxyls.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xl.panjiajie.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://tg.haigaiapp.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ca.szsharing.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://nw.huanxung.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://gr.lnxyls.cn

[L03] 设置自定义请求头
来源：http://mh.jctech888.com.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ju.szsharing.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://pn.huanxung.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cm.9csxet.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bd.gzmigu.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://dm.haigaiapp.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://rq.yuntaijiaju.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://xd.haigaiapp.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://rc.shxzukj.cn

[L04] 设置超时
来源：http://ru.newstarts.cn

Py:   requests.get(url, timeout=5)
来源：http://pu.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://jv.jctech888.com.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tn.shxzskj.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dl.bjjhwx.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://jn.huanxung.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://bu.huixinmuqiang.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ae.muxihuayi.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ba.bookmarksfly.cn

[L05] 上传文件（multipart）
来源：http://ut.asd995.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ym.huixiangedu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mj.muxihuayi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://jx.shxzskj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://en.gzmigu.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://az.huixinmuqiang.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://gq.bjjhwx.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ur.colortex.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://iz.nszjky.cn

[L06] 解析响应为 JSON
来源：http://mm.szxytkj.cn

Py:   resp.json()
来源：http://dv.hahajie.cn

PHP:  json_decode($body, true);
来源：http://xy.hnjuh.cn

JS:   await resp.json()
来源：http://xq.colortex.cn

TS:   await resp.json()
来源：http://tf.gzmigu.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://aa.nicolike.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://dc.jianghongdianzi.cn

Ruby: JSON.parse(resp.body)
来源：http://tw.szsharing.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://gl.shxzskj.cn

[L07] 处理 HTTP 状态码
来源：http://eo.wgjwhj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ns.nicolike.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://sr.wgjwhj.cn

JS:   resp.ok;  resp.status
来源：http://pl.chemitech.net.cn

TS:   resp.ok;  resp.status
来源：http://wi.9csxet.cn

Java: resp.statusCode()
来源：http://gx.newstarts.cn

Go:   resp.StatusCode
来源：http://aj.gzmigu.cn

Ruby: resp.code.to_i
来源：http://pu.huanxung.cn

C#:   (int)resp.StatusCode
来源：http://cx.shxzukj.cn

[L08] 并发请求多个地址
来源：http://pt.nszjky.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://yj.521024.cn

PHP:  curl_multi_init() 系列
来源：http://eu.chemitech.net.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cb.haigaiapp.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rd.yuexingan06.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ju.huixinmuqiang.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qu.gzmigu.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ny.yuntaijiaju.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ok.huixiangedu.cn

================================================================================
来源：http://jf.hahajie.cn

M. 命令行 / 进程 / 环境
来源：http://hq.shxzukj.cn

================================================================================
来源：http://jh.szsharing.cn

[M01] 读取命令行参数
来源：http://px.9csxet.cn

Py:   sys.argv[1:]
来源：http://ho.panjiajie.cn

PHP:  $argv;  $argc;
来源：http://qd.szxytkj.cn

JS:   process.argv.slice(2)
来源：http://qd.huixiangedu.cn

TS:   process.argv.slice(2)
来源：http://eq.gzmigu.cn

Java: args 数组（main 方法参数）
来源：http://xs.panjiajie.cn

Go:   os.Args[1:]
来源：http://mm.9csxet.cn

Ruby: ARGV
来源：http://qy.bjjhwx.cn

C#:   args 数组（Main 方法参数）
来源：http://wg.newstarts.cn

[M02] 读取环境变量
来源：http://ec.chemitech.net.cn

Py:   os.environ.get("HOME")
来源：http://mw.colortex.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://dn.jianghongdianzi.cn

JS:   process.env.HOME
来源：http://uf.szxytkj.cn

TS:   process.env.HOME
来源：http://ma.yuntaijiaju.cn

Java: System.getenv("HOME")
来源：http://te.huixiangedu.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://xn.huixinmuqiang.cn

Ruby: ENV["HOME"]
来源：http://ld.shxzukj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://oi.colortex.cn

[M03] 执行外部命令
来源：http://bf.muxihuayi.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ti.chemitech.net.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://vx.yuexingan06.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://cr.newstarts.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://sd.newstarts.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ox.asd995.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://px.chemitech.net.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ju.shxzukj.cn

C#:   Process.Start("ls", "-l");
来源：http://yd.hnjuh.cn

[M04] 获取当前工作目录
来源：http://mw.newstarts.cn

Py:   os.getcwd()
来源：http://tg.szsharing.cn

PHP:  getcwd();
来源：http://mv.wgjwhj.cn

JS:   process.cwd()
来源：http://cj.gzmigu.cn

TS:   process.cwd()
来源：http://aw.szxytkj.cn

Java: Path.of("").toAbsolutePath()
来源：http://bc.nicolike.cn

Go:   os.Getwd()
来源：http://qq.521024.cn

Ruby: Dir.pwd
来源：http://sg.nszjky.cn

C#:   Directory.GetCurrentDirectory()
来源：http://qo.huixinmuqiang.cn

[M05] 设置退出码
来源：http://ww.huixinmuqiang.cn

Py:   sys.exit(1)
来源：http://qh.huanxung.cn

PHP:  exit(1);
来源：http://py.chemitech.net.cn

JS:   process.exit(1)
来源：http://ly.bjjhwx.cn

TS:   process.exit(1)
来源：http://op.asd995.cn

Java: System.exit(1)
来源：http://ze.hahajie.cn

Go:   os.Exit(1)
来源：http://bd.haigaiapp.cn

Ruby: exit 1
来源：http://fr.lnxyls.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ib.bookmarksfly.cn

[M06] 向标准错误输出
来源：http://ul.szxytkj.cn

Py:   print("err", file=sys.stderr)
来源：http://to.shxzukj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://nz.lnxyls.cn

JS:   console.error("err")
来源：http://dx.szsharing.cn

TS:   console.error("err")
来源：http://cn.szsharing.cn

Java: System.err.println("err")
来源：http://az.szsharing.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://az.asd995.cn

Ruby: warn "err"
来源：http://fq.hnjuh.cn

C#:   Console.Error.WriteLine("err")
来源：http://rw.bookmarksfly.cn

[M07] 判断是否为主入口
来源：http://ax.asd995.cn

Py:   if __name__ == "__main__":
来源：http://te.haigaiapp.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://jw.bjjhwx.cn

JS:   require.main === module
来源：http://ap.panjiajie.cn

TS:   require.main === module
来源：http://tk.yuntaijiaju.cn

Java: public static void main(String[] args)
来源：http://lh.gzmigu.cn

Go:   func main()
来源：http://wc.szxytkj.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hp.panjiajie.cn

C#:   static void Main(string[] args)
来源：http://fn.bjjhwx.cn

[M08] 获取系统与运行时信息
来源：http://re.panjiajie.cn

Py:   platform.system();  platform.python_version()
来源：http://xb.wgjwhj.cn

PHP:  PHP_OS;  phpversion();
来源：http://nj.nszjky.cn

JS:   process.platform;  process.version
来源：http://cm.colortex.cn

TS:   process.platform;  process.version
来源：http://it.hahajie.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://pn.521024.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://tc.9csxet.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://gl.jianghongdianzi.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://zi.lnxyls.cn

================================================================================
来源：http://ax.nicolike.cn

N. 数据结构与算法
来源：http://fe.wgjwhj.cn

================================================================================
来源：http://uc.hnjuh.cn

[N01] 二分查找（有序数组）
来源：http://cg.newstarts.cn

Py:   bisect.bisect_left(arr, x)
来源：http://xn.huixiangedu.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wc.wgjwhj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tm.panjiajie.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ef.9csxet.cn

Java: Arrays.binarySearch(arr, x)
来源：http://wj.yuexingan06.cn

Go:   sort.SearchInts(arr, x)
来源：http://xh.bookmarksfly.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://oy.521024.cn

C#:   Array.BinarySearch(arr, x)
来源：http://uv.lnxyls.cn

[N02] 排序（工程实践用内置实现）
来源：http://og.521024.cn

Py:   sorted(arr);  arr.sort()
来源：http://pc.521024.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mt.lnxyls.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://je.huixiangedu.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://yl.newstarts.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ay.shtwfgs.cn

Go:   slices.Sort(arr)
来源：http://tu.wgjwhj.cn

Ruby: arr.sort
来源：http://ct.asd995.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ex.szsharing.cn

[N03] 快速排序（分治示例）
来源：http://iy.chemitech.net.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://sx.szsharing.cn


<!-- 参考信息 -->