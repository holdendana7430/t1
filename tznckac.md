代发 wailian999

PHP:  (new DateTime())->modify("+7 days");
来源：http://di.szsharing.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://jc.gzmigu.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://zn.hnjuh.cn

Java: LocalDate.now().plusDays(7)
来源：http://ap.asd995.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zi.huixiangedu.cn

Ruby: Time.now + 7 * 86400
来源：http://dn.bookmarksfly.cn

C#:   DateTime.Now.AddDays(7)
来源：http://yf.nszjky.cn

[J06] 计算两时间之差
来源：http://bs.jctech888.com.cn

Py:   (end - start).total_seconds()
来源：http://xl.newstarts.cn

PHP:  $end->diff($start)->days;
来源：http://zw.nicolike.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mo.lnxyls.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mw.wgjwhj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://kj.huixinmuqiang.cn

Go:   end.Sub(start).Hours()
来源：http://zn.hahajie.cn

Ruby: end - start                 # 返回秒数
来源：http://zs.jianghongdianzi.cn

C#:   (end - start).TotalSeconds
来源：http://fd.hnjuh.cn

[J07] 比较两个日期
来源：http://cz.nicolike.cn

Py:   d1 < d2;  d1 == d2
来源：http://os.muxihuayi.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://yi.nszjky.cn

JS:   d1.getTime() < d2.getTime()
来源：http://rt.haigaiapp.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ql.yuntaijiaju.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://cn.shxzukj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://nn.chemitech.net.cn

Ruby: d1 < d2;  d1 == d2
来源：http://bs.shxzskj.cn

C#:   d1 < d2;  d1 == d2
来源：http://le.jctech888.com.cn

[J08] 提取年月日与星期
来源：http://bk.huixiangedu.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://nd.haigaiapp.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ed.bookmarksfly.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://pi.521024.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mm.shxzskj.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://aa.muxihuayi.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://gs.nszjky.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ac.szxytkj.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://cu.asd995.cn

[J09] 时区处理
来源：http://hr.nicolike.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hy.hnjuh.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://vw.yuntaijiaju.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lv.szxytkj.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mo.shtwfgs.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://gf.jianghongdianzi.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://az.szxytkj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://dk.lnxyls.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ok.hnjuh.cn

[J10] 取今天 / 本月第一天
来源：http://bc.szxytkj.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://fl.muxihuayi.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mu.muxihuayi.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://gx.szsharing.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ah.huanxung.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://py.nicolike.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://sa.szsharing.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://yt.521024.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://tm.shxzskj.cn

================================================================================
来源：http://hg.bookmarksfly.cn

K. JSON 与序列化
来源：http://cb.wgjwhj.cn

================================================================================
来源：http://cp.hahajie.cn

[K01] 对象转 JSON 字符串
来源：http://zj.shxzukj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wi.asd995.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://zo.shxzskj.cn

JS:   JSON.stringify(obj)
来源：http://ha.yuntaijiaju.cn

TS:   JSON.stringify(obj)
来源：http://vb.yuntaijiaju.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ws.wgjwhj.cn

Go:   json.Marshal(obj)
来源：http://ig.bookmarksfly.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ob.yuexingan06.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://mi.521024.cn

[K02] JSON 字符串转对象
来源：http://eg.haigaiapp.cn

Py:   json.loads(s)
来源：http://jm.huixinmuqiang.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://sg.gzmigu.cn

JS:   JSON.parse(s)
来源：http://nv.gzmigu.cn

TS:   JSON.parse(s)
来源：http://ly.shxzskj.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ez.szsharing.cn

Go:   json.Unmarshal(data, &v)
来源：http://ch.szsharing.cn

Ruby: JSON.parse(s)
来源：http://tf.wgjwhj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ry.szxytkj.cn

[K03] JSON 美化输出（带缩进）
来源：http://dp.haigaiapp.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://kc.huanxung.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ze.haigaiapp.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://il.gzmigu.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ij.jctech888.com.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://rb.gzmigu.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://lb.szsharing.cn

Ruby: JSON.pretty_generate(obj)
来源：http://wc.gzmigu.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://gj.shxzukj.cn

[K04] 读取 JSON 文件
来源：http://ik.huixiangedu.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://zq.yuexingan06.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fr.bookmarksfly.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cu.bjjhwx.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yz.jctech888.com.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://xq.9csxet.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://yh.szsharing.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://bz.colortex.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hw.nszjky.cn

[K05] 深拷贝对象
来源：http://pf.yuexingan06.cn

Py:   copy.deepcopy(obj)
来源：http://hz.bjjhwx.cn

PHP:  unserialize(serialize($obj));
来源：http://aa.chemitech.net.cn

JS:   structuredClone(obj)
来源：http://zq.yuexingan06.cn

TS:   structuredClone(obj)
来源：http://ws.huanxung.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://fd.521024.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://dm.huixinmuqiang.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://dz.szxytkj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://pe.gzmigu.cn

[K06] 解析 URL 查询串
来源：http://me.wgjwhj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://sr.huixinmuqiang.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://vl.hahajie.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://by.nszjky.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qv.nicolike.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://qd.shtwfgs.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://xn.chemitech.net.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://sf.shxzskj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wi.hahajie.cn

[K07] 进制转换
来源：http://tn.newstarts.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://vd.9csxet.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://dz.shxzukj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://zw.lnxyls.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://cf.bjjhwx.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://sv.panjiajie.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://fc.yuntaijiaju.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://fy.muxihuayi.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hk.huanxung.cn

[K08] 二进制序列化（非 JSON）
来源：http://ix.9csxet.cn

Py:   pickle.dumps(obj)
来源：http://vn.huanxung.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ne.bjjhwx.cn

JS:   v8.serialize(obj)        // Node
来源：http://cl.colortex.cn

TS:   v8.serialize(obj)        // Node
来源：http://pb.nicolike.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://er.huanxung.cn

Go:   encoding/gob
来源：http://tp.colortex.cn

Ruby: Marshal.dump(obj)
来源：http://qh.huixiangedu.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mt.bookmarksfly.cn

================================================================================
来源：http://jq.yuntaijiaju.cn

L. 网络请求
来源：http://dj.shtwfgs.cn

================================================================================
来源：http://dn.nszjky.cn

[L01] 发送 GET 请求
来源：http://hb.jianghongdianzi.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://bo.bookmarksfly.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://fa.jctech888.com.cn

JS:   await fetch(url)
来源：http://sp.nicolike.cn

TS:   await fetch(url)
来源：http://lp.9csxet.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qe.9csxet.cn

Go:   resp, err := http.Get(url)
来源：http://os.yuntaijiaju.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://uq.panjiajie.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ol.shtwfgs.cn

[L02] 发送 POST JSON
来源：http://pu.shxzskj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://vn.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://vh.hnjuh.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ni.yuntaijiaju.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://at.szxytkj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://jr.huixinmuqiang.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://eo.9csxet.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hm.nicolike.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wr.nszjky.cn

[L03] 设置自定义请求头
来源：http://wc.asd995.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://st.wgjwhj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://yn.wgjwhj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ey.szsharing.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vu.shxzukj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wk.bjjhwx.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://sa.chemitech.net.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://sp.huixiangedu.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jr.hnjuh.cn

[L04] 设置超时
来源：http://ho.lnxyls.cn

Py:   requests.get(url, timeout=5)
来源：http://ny.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://yl.shxzukj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wv.wgjwhj.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vy.shxzskj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://yj.hnjuh.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://rt.asd995.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hk.jctech888.com.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wz.521024.cn

[L05] 上传文件（multipart）
来源：http://ya.nicolike.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ri.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://iv.szxytkj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gw.muxihuayi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://pf.panjiajie.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ib.lnxyls.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mi.jctech888.com.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vj.hnjuh.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://tw.bookmarksfly.cn

[L06] 解析响应为 JSON
来源：http://nd.jianghongdianzi.cn

Py:   resp.json()
来源：http://vp.521024.cn

PHP:  json_decode($body, true);
来源：http://wk.9csxet.cn

JS:   await resp.json()
来源：http://jr.asd995.cn

TS:   await resp.json()
来源：http://cs.huixinmuqiang.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://yj.newstarts.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://oq.chemitech.net.cn

Ruby: JSON.parse(resp.body)
来源：http://wm.shxzukj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://gs.jianghongdianzi.cn

[L07] 处理 HTTP 状态码
来源：http://iv.hnjuh.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://lb.yuntaijiaju.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://bb.szxytkj.cn

JS:   resp.ok;  resp.status
来源：http://cr.haigaiapp.cn

TS:   resp.ok;  resp.status
来源：http://um.jctech888.com.cn

Java: resp.statusCode()
来源：http://gw.hnjuh.cn

Go:   resp.StatusCode
来源：http://kg.jctech888.com.cn

Ruby: resp.code.to_i
来源：http://qv.lnxyls.cn

C#:   (int)resp.StatusCode
来源：http://vm.asd995.cn

[L08] 并发请求多个地址
来源：http://lp.521024.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hp.gzmigu.cn

PHP:  curl_multi_init() 系列
来源：http://ym.shxzukj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dz.shxzskj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ir.jianghongdianzi.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://fz.jianghongdianzi.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://zo.newstarts.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://bd.szsharing.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://tw.nicolike.cn

================================================================================
来源：http://cl.9csxet.cn

M. 命令行 / 进程 / 环境
来源：http://mm.jctech888.com.cn

================================================================================
来源：http://fb.nicolike.cn

[M01] 读取命令行参数
来源：http://ih.newstarts.cn

Py:   sys.argv[1:]
来源：http://wg.jianghongdianzi.cn

PHP:  $argv;  $argc;
来源：http://ez.huanxung.cn

JS:   process.argv.slice(2)
来源：http://kc.wgjwhj.cn

TS:   process.argv.slice(2)
来源：http://tc.szxytkj.cn

Java: args 数组（main 方法参数）
来源：http://tp.lnxyls.cn

Go:   os.Args[1:]
来源：http://bb.yuntaijiaju.cn

Ruby: ARGV
来源：http://va.bookmarksfly.cn

C#:   args 数组（Main 方法参数）
来源：http://by.521024.cn

[M02] 读取环境变量
来源：http://fw.muxihuayi.cn

Py:   os.environ.get("HOME")
来源：http://ow.521024.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://br.newstarts.cn

JS:   process.env.HOME
来源：http://dv.shxzukj.cn

TS:   process.env.HOME
来源：http://sn.yuntaijiaju.cn

Java: System.getenv("HOME")
来源：http://ck.huixinmuqiang.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://nk.szsharing.cn

Ruby: ENV["HOME"]
来源：http://wp.muxihuayi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hu.chemitech.net.cn

[M03] 执行外部命令
来源：http://ek.gzmigu.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ci.gzmigu.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://kl.shxzukj.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ha.lnxyls.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ik.asd995.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mj.huixinmuqiang.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://cu.nicolike.cn

Ruby: system("ls -l");  `ls -l`
来源：http://xd.szxytkj.cn

C#:   Process.Start("ls", "-l");
来源：http://wc.yuntaijiaju.cn

[M04] 获取当前工作目录
来源：http://wi.shtwfgs.cn

Py:   os.getcwd()
来源：http://hk.jianghongdianzi.cn

PHP:  getcwd();
来源：http://qq.huixinmuqiang.cn

JS:   process.cwd()
来源：http://ka.nicolike.cn

TS:   process.cwd()
来源：http://ux.yuexingan06.cn

Java: Path.of("").toAbsolutePath()
来源：http://dw.szsharing.cn

Go:   os.Getwd()
来源：http://wx.muxihuayi.cn

Ruby: Dir.pwd
来源：http://up.panjiajie.cn

C#:   Directory.GetCurrentDirectory()
来源：http://qk.nicolike.cn

[M05] 设置退出码
来源：http://sx.wgjwhj.cn

Py:   sys.exit(1)
来源：http://kq.huanxung.cn

PHP:  exit(1);
来源：http://ug.huixinmuqiang.cn

JS:   process.exit(1)
来源：http://gs.gzmigu.cn

TS:   process.exit(1)
来源：http://qr.nicolike.cn

Java: System.exit(1)
来源：http://oo.hahajie.cn

Go:   os.Exit(1)
来源：http://aq.bookmarksfly.cn

Ruby: exit 1
来源：http://hx.hnjuh.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://bg.wgjwhj.cn

[M06] 向标准错误输出
来源：http://ky.asd995.cn

Py:   print("err", file=sys.stderr)
来源：http://vj.gzmigu.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://vi.shtwfgs.cn

JS:   console.error("err")
来源：http://pb.wgjwhj.cn

TS:   console.error("err")
来源：http://xo.bookmarksfly.cn

Java: System.err.println("err")
来源：http://ck.bookmarksfly.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://eg.yuntaijiaju.cn

Ruby: warn "err"
来源：http://bz.huanxung.cn

C#:   Console.Error.WriteLine("err")
来源：http://pz.nicolike.cn

[M07] 判断是否为主入口
来源：http://bi.panjiajie.cn

Py:   if __name__ == "__main__":
来源：http://hu.bookmarksfly.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://od.nszjky.cn

JS:   require.main === module
来源：http://vo.bookmarksfly.cn

TS:   require.main === module
来源：http://oi.panjiajie.cn

Java: public static void main(String[] args)
来源：http://cn.panjiajie.cn

Go:   func main()
来源：http://jy.yuexingan06.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://qx.shxzskj.cn

C#:   static void Main(string[] args)
来源：http://ji.nicolike.cn

[M08] 获取系统与运行时信息
来源：http://tv.szsharing.cn

Py:   platform.system();  platform.python_version()
来源：http://pq.shtwfgs.cn

PHP:  PHP_OS;  phpversion();
来源：http://dy.jctech888.com.cn

JS:   process.platform;  process.version
来源：http://ha.hahajie.cn

TS:   process.platform;  process.version
来源：http://ta.newstarts.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://sn.newstarts.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ls.szsharing.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://uw.huanxung.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://cd.shxzukj.cn

================================================================================
来源：http://br.lnxyls.cn

N. 数据结构与算法
来源：http://fn.chemitech.net.cn

================================================================================
来源：http://xz.hnjuh.cn

[N01] 二分查找（有序数组）
来源：http://bp.bookmarksfly.cn

Py:   bisect.bisect_left(arr, x)
来源：http://qj.huixinmuqiang.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hh.wgjwhj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hb.szxytkj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yk.hnjuh.cn

Java: Arrays.binarySearch(arr, x)
来源：http://xt.muxihuayi.cn

Go:   sort.SearchInts(arr, x)
来源：http://xv.bjjhwx.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://qk.huixiangedu.cn

C#:   Array.BinarySearch(arr, x)
来源：http://hy.huixiangedu.cn

[N02] 排序（工程实践用内置实现）
来源：http://hg.muxihuayi.cn

Py:   sorted(arr);  arr.sort()
来源：http://tg.szsharing.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://lr.lnxyls.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://qk.521024.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://sn.gzmigu.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://jd.muxihuayi.cn

Go:   slices.Sort(arr)
来源：http://nr.huixiangedu.cn

Ruby: arr.sort
来源：http://jk.newstarts.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://cy.muxihuayi.cn

[N03] 快速排序（分治示例）
来源：http://rf.nszjky.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://zr.huixiangedu.cn


<!-- 参考信息 -->