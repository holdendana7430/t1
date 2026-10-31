代发 wailian999

Go:   time.Now().AddDate(0, 0, 7)
来源：http://kr.shtwfgs.cn

Ruby: Time.now + 7 * 86400
来源：http://vb.yuntaijiaju.cn

C#:   DateTime.Now.AddDays(7)
来源：http://mx.shxzukj.cn

[J06] 计算两时间之差
来源：http://cu.yuntaijiaju.cn

Py:   (end - start).total_seconds()
来源：http://yz.521024.cn

PHP:  $end->diff($start)->days;
来源：http://uc.panjiajie.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://jx.yuexingan06.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://sl.gzmigu.cn

Java: Duration.between(start, end).toSeconds()
来源：http://pu.shxzukj.cn

Go:   end.Sub(start).Hours()
来源：http://hf.chemitech.net.cn

Ruby: end - start                 # 返回秒数
来源：http://ee.nszjky.cn

C#:   (end - start).TotalSeconds
来源：http://dz.lnxyls.cn

[J07] 比较两个日期
来源：http://ev.newstarts.cn

Py:   d1 < d2;  d1 == d2
来源：http://qw.szxytkj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://cl.newstarts.cn

JS:   d1.getTime() < d2.getTime()
来源：http://cw.panjiajie.cn

TS:   d1.getTime() < d2.getTime()
来源：http://mb.bookmarksfly.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://nk.hnjuh.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ik.lnxyls.cn

Ruby: d1 < d2;  d1 == d2
来源：http://yt.szxytkj.cn

C#:   d1 < d2;  d1 == d2
来源：http://gg.jctech888.com.cn

[J08] 提取年月日与星期
来源：http://yr.muxihuayi.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://tp.hnjuh.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://qk.shxzukj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mf.yuexingan06.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ds.shxzskj.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://xp.huixinmuqiang.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://pd.jctech888.com.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://qq.bookmarksfly.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://aq.huanxung.cn

[J09] 时区处理
来源：http://wd.9csxet.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://nn.9csxet.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://vf.huixiangedu.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wq.huixiangedu.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://la.panjiajie.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ji.hahajie.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://le.hnjuh.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://im.haigaiapp.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://il.muxihuayi.cn

[J10] 取今天 / 本月第一天
来源：http://lh.huixinmuqiang.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://zy.hahajie.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://qo.szsharing.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://oc.szxytkj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://il.shxzskj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zu.colortex.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ny.szxytkj.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://st.asd995.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mx.hnjuh.cn

================================================================================
来源：http://oj.jianghongdianzi.cn

K. JSON 与序列化
来源：http://wi.yuntaijiaju.cn

================================================================================
来源：http://uj.panjiajie.cn

[K01] 对象转 JSON 字符串
来源：http://jq.jianghongdianzi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://yg.bookmarksfly.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://db.shxzskj.cn

JS:   JSON.stringify(obj)
来源：http://xv.wgjwhj.cn

TS:   JSON.stringify(obj)
来源：http://qs.haigaiapp.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://vw.hahajie.cn

Go:   json.Marshal(obj)
来源：http://ue.shxzskj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://vq.newstarts.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://oj.9csxet.cn

[K02] JSON 字符串转对象
来源：http://pq.bookmarksfly.cn

Py:   json.loads(s)
来源：http://ho.huanxung.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ah.shtwfgs.cn

JS:   JSON.parse(s)
来源：http://pj.colortex.cn

TS:   JSON.parse(s)
来源：http://bd.gzmigu.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qo.shxzukj.cn

Go:   json.Unmarshal(data, &v)
来源：http://un.shxzskj.cn

Ruby: JSON.parse(s)
来源：http://vw.shxzskj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zq.nszjky.cn

[K03] JSON 美化输出（带缩进）
来源：http://wa.shxzskj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://lz.hahajie.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://sv.asd995.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://nz.szxytkj.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://wg.yuntaijiaju.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ld.bookmarksfly.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://gr.jianghongdianzi.cn

Ruby: JSON.pretty_generate(obj)
来源：http://qo.bjjhwx.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://eo.newstarts.cn

[K04] 读取 JSON 文件
来源：http://py.wgjwhj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://te.szsharing.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://th.asd995.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cu.colortex.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://am.bookmarksfly.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://yo.bjjhwx.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://fq.newstarts.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://pa.521024.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://zq.hnjuh.cn

[K05] 深拷贝对象
来源：http://fh.colortex.cn

Py:   copy.deepcopy(obj)
来源：http://mz.huixiangedu.cn

PHP:  unserialize(serialize($obj));
来源：http://jy.shxzskj.cn

JS:   structuredClone(obj)
来源：http://th.hnjuh.cn

TS:   structuredClone(obj)
来源：http://fj.huanxung.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ar.hahajie.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://sp.newstarts.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://uk.asd995.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://kq.yuntaijiaju.cn

[K06] 解析 URL 查询串
来源：http://qr.yuexingan06.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://kx.jctech888.com.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://gr.szxytkj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rb.shxzskj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uc.jctech888.com.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://jp.bookmarksfly.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ur.lnxyls.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mw.yuexingan06.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://sp.9csxet.cn

[K07] 进制转换
来源：http://yh.chemitech.net.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://bk.shtwfgs.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://zp.jctech888.com.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://dy.shxzukj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ei.huanxung.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://dp.szxytkj.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mo.panjiajie.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://eu.lnxyls.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ha.hahajie.cn

[K08] 二进制序列化（非 JSON）
来源：http://cu.bjjhwx.cn

Py:   pickle.dumps(obj)
来源：http://rv.bookmarksfly.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ig.hahajie.cn

JS:   v8.serialize(obj)        // Node
来源：http://aj.huixiangedu.cn

TS:   v8.serialize(obj)        // Node
来源：http://yb.bookmarksfly.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://yc.bookmarksfly.cn

Go:   encoding/gob
来源：http://wi.521024.cn

Ruby: Marshal.dump(obj)
来源：http://ji.shtwfgs.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://sk.szxytkj.cn

================================================================================
来源：http://xy.shxzskj.cn

L. 网络请求
来源：http://pn.wgjwhj.cn

================================================================================
来源：http://sx.muxihuayi.cn

[L01] 发送 GET 请求
来源：http://hb.gzmigu.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ty.yuntaijiaju.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ch.nszjky.cn

JS:   await fetch(url)
来源：http://oq.chemitech.net.cn

TS:   await fetch(url)
来源：http://ik.yuntaijiaju.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://fy.newstarts.cn

Go:   resp, err := http.Get(url)
来源：http://tt.bjjhwx.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://bu.szsharing.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mu.huixinmuqiang.cn

[L02] 发送 POST JSON
来源：http://uy.shtwfgs.cn

Py:   requests.post(url, json={"a": 1})
来源：http://gj.nicolike.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://va.muxihuayi.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fa.9csxet.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gf.szsharing.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://oy.jctech888.com.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://gr.muxihuayi.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://oz.bookmarksfly.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ey.jctech888.com.cn

[L03] 设置自定义请求头
来源：http://nl.bjjhwx.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://gs.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://vj.shtwfgs.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dc.huixinmuqiang.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wi.nszjky.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://es.shtwfgs.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wl.panjiajie.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ws.hahajie.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://cc.huanxung.cn

[L04] 设置超时
来源：http://hp.yuntaijiaju.cn

Py:   requests.get(url, timeout=5)
来源：http://xi.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://vt.521024.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bp.huanxung.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://aw.nszjky.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://gq.yuntaijiaju.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://on.colortex.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://fy.asd995.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://fe.colortex.cn

[L05] 上传文件（multipart）
来源：http://cf.chemitech.net.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hq.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ql.newstarts.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://bb.lnxyls.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://uw.nszjky.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://sn.asd995.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://zh.hahajie.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://rg.szxytkj.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hs.shxzskj.cn

[L06] 解析响应为 JSON
来源：http://mf.shxzskj.cn

Py:   resp.json()
来源：http://ly.nicolike.cn

PHP:  json_decode($body, true);
来源：http://lh.bookmarksfly.cn

JS:   await resp.json()
来源：http://qk.shxzukj.cn

TS:   await resp.json()
来源：http://tn.nicolike.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wb.hnjuh.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://zl.gzmigu.cn

Ruby: JSON.parse(resp.body)
来源：http://gr.nszjky.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://lb.shxzskj.cn

[L07] 处理 HTTP 状态码
来源：http://ky.haigaiapp.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ky.chemitech.net.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hx.muxihuayi.cn

JS:   resp.ok;  resp.status
来源：http://gv.9csxet.cn

TS:   resp.ok;  resp.status
来源：http://ig.huanxung.cn

Java: resp.statusCode()
来源：http://lz.nszjky.cn

Go:   resp.StatusCode
来源：http://xc.panjiajie.cn

Ruby: resp.code.to_i
来源：http://ic.shxzskj.cn

C#:   (int)resp.StatusCode
来源：http://gy.yuntaijiaju.cn

[L08] 并发请求多个地址
来源：http://in.nszjky.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://fg.szxytkj.cn

PHP:  curl_multi_init() 系列
来源：http://pv.haigaiapp.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ln.chemitech.net.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bt.jianghongdianzi.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ay.gzmigu.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://pr.shxzskj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hc.muxihuayi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://bv.asd995.cn

================================================================================
来源：http://fa.huanxung.cn

M. 命令行 / 进程 / 环境
来源：http://jk.521024.cn

================================================================================
来源：http://pg.shxzukj.cn

[M01] 读取命令行参数
来源：http://gf.hnjuh.cn

Py:   sys.argv[1:]
来源：http://kw.nicolike.cn

PHP:  $argv;  $argc;
来源：http://qx.yuntaijiaju.cn

JS:   process.argv.slice(2)
来源：http://gm.szxytkj.cn

TS:   process.argv.slice(2)
来源：http://mv.hahajie.cn

Java: args 数组（main 方法参数）
来源：http://vy.shtwfgs.cn

Go:   os.Args[1:]
来源：http://yj.wgjwhj.cn

Ruby: ARGV
来源：http://lq.shtwfgs.cn

C#:   args 数组（Main 方法参数）
来源：http://bu.szxytkj.cn

[M02] 读取环境变量
来源：http://zt.hahajie.cn

Py:   os.environ.get("HOME")
来源：http://ox.jctech888.com.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://sd.shxzukj.cn

JS:   process.env.HOME
来源：http://ov.9csxet.cn

TS:   process.env.HOME
来源：http://lc.huixiangedu.cn

Java: System.getenv("HOME")
来源：http://xc.shxzskj.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ze.nszjky.cn

Ruby: ENV["HOME"]
来源：http://qa.nicolike.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://qw.huixinmuqiang.cn

[M03] 执行外部命令
来源：http://yo.9csxet.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ow.huixinmuqiang.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ln.shxzskj.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ss.bjjhwx.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ba.nicolike.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://id.shtwfgs.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://su.hahajie.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ma.hahajie.cn

C#:   Process.Start("ls", "-l");
来源：http://nc.wgjwhj.cn

[M04] 获取当前工作目录
来源：http://pc.lnxyls.cn

Py:   os.getcwd()
来源：http://mo.huixinmuqiang.cn

PHP:  getcwd();
来源：http://fg.shtwfgs.cn

JS:   process.cwd()
来源：http://dc.bookmarksfly.cn

TS:   process.cwd()
来源：http://rz.hnjuh.cn

Java: Path.of("").toAbsolutePath()
来源：http://lw.muxihuayi.cn

Go:   os.Getwd()
来源：http://pr.jianghongdianzi.cn

Ruby: Dir.pwd
来源：http://vb.muxihuayi.cn

C#:   Directory.GetCurrentDirectory()
来源：http://gh.szxytkj.cn

[M05] 设置退出码
来源：http://dp.hnjuh.cn

Py:   sys.exit(1)
来源：http://pj.huixiangedu.cn

PHP:  exit(1);
来源：http://ub.huixinmuqiang.cn

JS:   process.exit(1)
来源：http://jp.newstarts.cn

TS:   process.exit(1)
来源：http://uc.szsharing.cn

Java: System.exit(1)
来源：http://wo.nicolike.cn

Go:   os.Exit(1)
来源：http://jn.lnxyls.cn

Ruby: exit 1
来源：http://ni.chemitech.net.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://bc.haigaiapp.cn

[M06] 向标准错误输出
来源：http://sw.jianghongdianzi.cn

Py:   print("err", file=sys.stderr)
来源：http://kh.lnxyls.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://rf.yuexingan06.cn

JS:   console.error("err")
来源：http://pb.panjiajie.cn

TS:   console.error("err")
来源：http://gf.bookmarksfly.cn

Java: System.err.println("err")
来源：http://qf.wgjwhj.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ev.panjiajie.cn

Ruby: warn "err"
来源：http://cu.chemitech.net.cn

C#:   Console.Error.WriteLine("err")
来源：http://kr.chemitech.net.cn

[M07] 判断是否为主入口
来源：http://lb.wgjwhj.cn

Py:   if __name__ == "__main__":
来源：http://hu.huixinmuqiang.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ya.lnxyls.cn

JS:   require.main === module
来源：http://pc.yuntaijiaju.cn

TS:   require.main === module
来源：http://vf.haigaiapp.cn

Java: public static void main(String[] args)
来源：http://jc.gzmigu.cn

Go:   func main()
来源：http://aa.huanxung.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://le.szxytkj.cn

C#:   static void Main(string[] args)
来源：http://rj.newstarts.cn

[M08] 获取系统与运行时信息
来源：http://uz.huanxung.cn

Py:   platform.system();  platform.python_version()
来源：http://fc.huixiangedu.cn

PHP:  PHP_OS;  phpversion();
来源：http://as.shtwfgs.cn

JS:   process.platform;  process.version
来源：http://fl.panjiajie.cn

TS:   process.platform;  process.version
来源：http://vv.shtwfgs.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://za.huixinmuqiang.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://vx.jianghongdianzi.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://my.yuntaijiaju.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ag.bookmarksfly.cn

================================================================================
来源：http://qi.gzmigu.cn

N. 数据结构与算法
来源：http://xf.jctech888.com.cn

================================================================================
来源：http://go.newstarts.cn

[N01] 二分查找（有序数组）
来源：http://iv.hnjuh.cn

Py:   bisect.bisect_left(arr, x)
来源：http://rd.hahajie.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://uy.szsharing.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fv.nicolike.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://so.haigaiapp.cn

Java: Arrays.binarySearch(arr, x)
来源：http://tv.huanxung.cn

Go:   sort.SearchInts(arr, x)
来源：http://ws.9csxet.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://fc.yuntaijiaju.cn

C#:   Array.BinarySearch(arr, x)
来源：http://fm.yuntaijiaju.cn

[N02] 排序（工程实践用内置实现）
来源：http://rl.nszjky.cn

Py:   sorted(arr);  arr.sort()
来源：http://iv.wgjwhj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hc.hnjuh.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://gj.jctech888.com.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ti.jctech888.com.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wg.jctech888.com.cn

Go:   slices.Sort(arr)
来源：http://re.521024.cn

Ruby: arr.sort
来源：http://ij.chemitech.net.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://wz.newstarts.cn

[N03] 快速排序（分治示例）
来源：http://fp.nicolike.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://gx.gzmigu.cn

PHP:  // 递归实现，或用 usort
来源：http://kd.yuntaijiaju.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ci.shtwfgs.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cr.panjiajie.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ko.bjjhwx.cn


<!-- 参考信息 -->