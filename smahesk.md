代发 wailian999

Py:   (end - start).total_seconds()
来源：http://cw.chemitech.net.cn

PHP:  $end->diff($start)->days;
来源：http://ql.shxzukj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://fj.muxihuayi.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ci.huixinmuqiang.cn

Java: Duration.between(start, end).toSeconds()
来源：http://fk.chemitech.net.cn

Go:   end.Sub(start).Hours()
来源：http://hb.shtwfgs.cn

Ruby: end - start                 # 返回秒数
来源：http://fd.521024.cn

C#:   (end - start).TotalSeconds
来源：http://ol.szxytkj.cn

[J07] 比较两个日期
来源：http://hw.haigaiapp.cn

Py:   d1 < d2;  d1 == d2
来源：http://ud.lnxyls.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://re.huixiangedu.cn

JS:   d1.getTime() < d2.getTime()
来源：http://kc.huixiangedu.cn

TS:   d1.getTime() < d2.getTime()
来源：http://vq.nicolike.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://pi.szsharing.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://eb.nicolike.cn

Ruby: d1 < d2;  d1 == d2
来源：http://vv.newstarts.cn

C#:   d1 < d2;  d1 == d2
来源：http://wb.hahajie.cn

[J08] 提取年月日与星期
来源：http://wi.gzmigu.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://xm.nicolike.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://no.panjiajie.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ki.huixiangedu.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://zf.szxytkj.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://oo.wgjwhj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ft.gzmigu.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zq.huanxung.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://gl.colortex.cn

[J09] 时区处理
来源：http://ez.huixinmuqiang.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://uz.jctech888.com.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://qp.haigaiapp.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://is.muxihuayi.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ds.nszjky.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://kc.huanxung.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://nz.shxzskj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://xu.yuntaijiaju.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://vs.lnxyls.cn

[J10] 取今天 / 本月第一天
来源：http://ts.wgjwhj.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://lz.gzmigu.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://nw.wgjwhj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ai.huixinmuqiang.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://pb.haigaiapp.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://do.yuexingan06.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://df.hnjuh.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://bt.huanxung.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://nb.lnxyls.cn

================================================================================
来源：http://oz.521024.cn

K. JSON 与序列化
来源：http://ro.szxytkj.cn

================================================================================
来源：http://qj.chemitech.net.cn

[K01] 对象转 JSON 字符串
来源：http://qi.szsharing.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ww.colortex.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://vw.huixinmuqiang.cn

JS:   JSON.stringify(obj)
来源：http://kc.bjjhwx.cn

TS:   JSON.stringify(obj)
来源：http://rd.bookmarksfly.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ca.hnjuh.cn

Go:   json.Marshal(obj)
来源：http://ik.jianghongdianzi.cn

Ruby: obj.to_json                                     // require "json"
来源：http://sc.hahajie.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://vg.jctech888.com.cn

[K02] JSON 字符串转对象
来源：http://fr.9csxet.cn

Py:   json.loads(s)
来源：http://fs.yuntaijiaju.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://au.bookmarksfly.cn

JS:   JSON.parse(s)
来源：http://ho.jianghongdianzi.cn

TS:   JSON.parse(s)
来源：http://rd.hahajie.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://yl.bjjhwx.cn

Go:   json.Unmarshal(data, &v)
来源：http://ot.521024.cn

Ruby: JSON.parse(s)
来源：http://if.nicolike.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://rk.bookmarksfly.cn

[K03] JSON 美化输出（带缩进）
来源：http://tj.jianghongdianzi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://nv.shtwfgs.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://im.asd995.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://gy.huixinmuqiang.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://kr.wgjwhj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://sa.huanxung.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wc.shxzskj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://zo.huixinmuqiang.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://tv.yuexingan06.cn

[K04] 读取 JSON 文件
来源：http://ss.colortex.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://gq.shxzukj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://kv.lnxyls.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://aa.chemitech.net.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rd.shxzskj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vq.panjiajie.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://xb.hahajie.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://te.nszjky.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://db.asd995.cn

[K05] 深拷贝对象
来源：http://sd.jianghongdianzi.cn

Py:   copy.deepcopy(obj)
来源：http://pn.jianghongdianzi.cn

PHP:  unserialize(serialize($obj));
来源：http://eu.bookmarksfly.cn

JS:   structuredClone(obj)
来源：http://ke.hnjuh.cn

TS:   structuredClone(obj)
来源：http://pg.nicolike.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://lu.yuexingan06.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zu.521024.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://bs.szsharing.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://xl.yuexingan06.cn

[K06] 解析 URL 查询串
来源：http://ht.yuntaijiaju.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mq.gzmigu.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hb.shxzukj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vj.panjiajie.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jw.9csxet.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://od.asd995.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://hj.hahajie.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hl.huixinmuqiang.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://up.asd995.cn

[K07] 进制转换
来源：http://xe.haigaiapp.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://jw.shxzukj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://rr.panjiajie.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://nd.9csxet.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://id.yuntaijiaju.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wa.nszjky.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://bo.jianghongdianzi.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://gh.shtwfgs.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hr.shtwfgs.cn

[K08] 二进制序列化（非 JSON）
来源：http://jz.chemitech.net.cn

Py:   pickle.dumps(obj)
来源：http://li.bookmarksfly.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ya.newstarts.cn

JS:   v8.serialize(obj)        // Node
来源：http://fo.muxihuayi.cn

TS:   v8.serialize(obj)        // Node
来源：http://ui.szxytkj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://cd.bjjhwx.cn

Go:   encoding/gob
来源：http://hx.lnxyls.cn

Ruby: Marshal.dump(obj)
来源：http://fr.haigaiapp.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://pb.bookmarksfly.cn

================================================================================
来源：http://jq.panjiajie.cn

L. 网络请求
来源：http://wb.9csxet.cn

================================================================================
来源：http://hq.bookmarksfly.cn

[L01] 发送 GET 请求
来源：http://qf.huanxung.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://nm.asd995.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://sl.shtwfgs.cn

JS:   await fetch(url)
来源：http://tq.newstarts.cn

TS:   await fetch(url)
来源：http://ty.9csxet.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ar.shxzukj.cn

Go:   resp, err := http.Get(url)
来源：http://nc.chemitech.net.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://fy.asd995.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://og.lnxyls.cn

[L02] 发送 POST JSON
来源：http://pp.9csxet.cn

Py:   requests.post(url, json={"a": 1})
来源：http://up.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://gt.haigaiapp.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ll.gzmigu.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ya.colortex.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ad.bookmarksfly.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://bo.haigaiapp.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://er.szxytkj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://tv.chemitech.net.cn

[L03] 设置自定义请求头
来源：http://vh.chemitech.net.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://zd.wgjwhj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://tf.yuntaijiaju.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xc.haigaiapp.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sa.bookmarksfly.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://yd.jctech888.com.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://be.yuntaijiaju.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://dd.hahajie.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://fa.hnjuh.cn

[L04] 设置超时
来源：http://sa.bookmarksfly.cn

Py:   requests.get(url, timeout=5)
来源：http://jw.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://rx.panjiajie.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tz.bjjhwx.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://op.shtwfgs.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://kw.jianghongdianzi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://op.yuexingan06.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://zy.bookmarksfly.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://dp.huixiangedu.cn

[L05] 上传文件（multipart）
来源：http://eq.wgjwhj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ff.huixiangedu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://gj.haigaiapp.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ds.hahajie.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://fe.haigaiapp.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ll.shxzukj.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ar.shxzukj.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://jr.yuexingan06.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://un.shxzskj.cn

[L06] 解析响应为 JSON
来源：http://xf.shtwfgs.cn

Py:   resp.json()
来源：http://od.newstarts.cn

PHP:  json_decode($body, true);
来源：http://tb.huixinmuqiang.cn

JS:   await resp.json()
来源：http://qi.shtwfgs.cn

TS:   await resp.json()
来源：http://jg.bookmarksfly.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mc.hnjuh.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://je.shxzukj.cn

Ruby: JSON.parse(resp.body)
来源：http://wh.bookmarksfly.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://at.huanxung.cn

[L07] 处理 HTTP 状态码
来源：http://ai.hahajie.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://iz.asd995.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://nw.9csxet.cn

JS:   resp.ok;  resp.status
来源：http://yh.haigaiapp.cn

TS:   resp.ok;  resp.status
来源：http://es.9csxet.cn

Java: resp.statusCode()
来源：http://ag.yuexingan06.cn

Go:   resp.StatusCode
来源：http://ka.szsharing.cn

Ruby: resp.code.to_i
来源：http://hq.wgjwhj.cn

C#:   (int)resp.StatusCode
来源：http://bt.newstarts.cn

[L08] 并发请求多个地址
来源：http://hj.chemitech.net.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ft.chemitech.net.cn

PHP:  curl_multi_init() 系列
来源：http://dy.hnjuh.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://il.bjjhwx.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://eh.bjjhwx.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://en.9csxet.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ln.chemitech.net.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://yg.colortex.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://lu.colortex.cn

================================================================================
来源：http://hg.szxytkj.cn

M. 命令行 / 进程 / 环境
来源：http://hp.colortex.cn

================================================================================
来源：http://pu.nicolike.cn

[M01] 读取命令行参数
来源：http://tk.huixiangedu.cn

Py:   sys.argv[1:]
来源：http://rw.nicolike.cn

PHP:  $argv;  $argc;
来源：http://og.huixiangedu.cn

JS:   process.argv.slice(2)
来源：http://qr.wgjwhj.cn

TS:   process.argv.slice(2)
来源：http://ul.huixinmuqiang.cn

Java: args 数组（main 方法参数）
来源：http://mj.jctech888.com.cn

Go:   os.Args[1:]
来源：http://de.9csxet.cn

Ruby: ARGV
来源：http://lv.huanxung.cn

C#:   args 数组（Main 方法参数）
来源：http://sw.gzmigu.cn

[M02] 读取环境变量
来源：http://ay.szxytkj.cn

Py:   os.environ.get("HOME")
来源：http://qx.521024.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://sy.yuexingan06.cn

JS:   process.env.HOME
来源：http://iv.nszjky.cn

TS:   process.env.HOME
来源：http://uf.hahajie.cn

Java: System.getenv("HOME")
来源：http://uo.panjiajie.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://yb.colortex.cn

Ruby: ENV["HOME"]
来源：http://eh.lnxyls.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wr.521024.cn

[M03] 执行外部命令
来源：http://jq.haigaiapp.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://jk.huixinmuqiang.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://he.huixinmuqiang.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://dy.haigaiapp.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://se.hahajie.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ln.shxzskj.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://xq.nicolike.cn

Ruby: system("ls -l");  `ls -l`
来源：http://xb.gzmigu.cn

C#:   Process.Start("ls", "-l");
来源：http://wn.shxzukj.cn

[M04] 获取当前工作目录
来源：http://re.newstarts.cn

Py:   os.getcwd()
来源：http://bz.muxihuayi.cn

PHP:  getcwd();
来源：http://ki.shxzskj.cn

JS:   process.cwd()
来源：http://ld.huixinmuqiang.cn

TS:   process.cwd()
来源：http://ce.shxzskj.cn

Java: Path.of("").toAbsolutePath()
来源：http://pv.hahajie.cn

Go:   os.Getwd()
来源：http://cn.newstarts.cn

Ruby: Dir.pwd
来源：http://aj.9csxet.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ig.huixinmuqiang.cn

[M05] 设置退出码
来源：http://qu.panjiajie.cn

Py:   sys.exit(1)
来源：http://ch.lnxyls.cn

PHP:  exit(1);
来源：http://fi.haigaiapp.cn

JS:   process.exit(1)
来源：http://us.jctech888.com.cn

TS:   process.exit(1)
来源：http://gg.colortex.cn

Java: System.exit(1)
来源：http://tl.panjiajie.cn

Go:   os.Exit(1)
来源：http://ig.chemitech.net.cn

Ruby: exit 1
来源：http://kb.huanxung.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ob.huixiangedu.cn

[M06] 向标准错误输出
来源：http://hi.jianghongdianzi.cn

Py:   print("err", file=sys.stderr)
来源：http://nx.jctech888.com.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://cn.colortex.cn

JS:   console.error("err")
来源：http://oy.huanxung.cn

TS:   console.error("err")
来源：http://ly.chemitech.net.cn

Java: System.err.println("err")
来源：http://em.huixiangedu.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://nd.shxzukj.cn

Ruby: warn "err"
来源：http://im.yuntaijiaju.cn

C#:   Console.Error.WriteLine("err")
来源：http://uh.szxytkj.cn

[M07] 判断是否为主入口
来源：http://ly.gzmigu.cn

Py:   if __name__ == "__main__":
来源：http://lh.yuexingan06.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://cg.bookmarksfly.cn

JS:   require.main === module
来源：http://tf.lnxyls.cn

TS:   require.main === module
来源：http://zt.huixinmuqiang.cn

Java: public static void main(String[] args)
来源：http://az.jianghongdianzi.cn

Go:   func main()
来源：http://gb.colortex.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://lj.chemitech.net.cn

C#:   static void Main(string[] args)
来源：http://iw.szxytkj.cn

[M08] 获取系统与运行时信息
来源：http://fe.yuntaijiaju.cn

Py:   platform.system();  platform.python_version()
来源：http://rj.shxzskj.cn

PHP:  PHP_OS;  phpversion();
来源：http://hq.shtwfgs.cn

JS:   process.platform;  process.version
来源：http://hf.hahajie.cn

TS:   process.platform;  process.version
来源：http://ot.szsharing.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://kr.jianghongdianzi.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://pg.lnxyls.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ap.gzmigu.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ws.jctech888.com.cn

================================================================================
来源：http://nm.hnjuh.cn

N. 数据结构与算法
来源：http://lk.lnxyls.cn

================================================================================
来源：http://hx.yuexingan06.cn

[N01] 二分查找（有序数组）
来源：http://be.shxzskj.cn

Py:   bisect.bisect_left(arr, x)
来源：http://kg.shtwfgs.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ps.shxzskj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yx.szxytkj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://os.hahajie.cn

Java: Arrays.binarySearch(arr, x)
来源：http://xa.huanxung.cn

Go:   sort.SearchInts(arr, x)
来源：http://ow.wgjwhj.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://tg.panjiajie.cn

C#:   Array.BinarySearch(arr, x)
来源：http://iy.huixinmuqiang.cn

[N02] 排序（工程实践用内置实现）
来源：http://ru.wgjwhj.cn

Py:   sorted(arr);  arr.sort()
来源：http://fw.shxzskj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://kj.gzmigu.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://oo.szxytkj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://lk.muxihuayi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://cd.hahajie.cn

Go:   slices.Sort(arr)
来源：http://tp.bookmarksfly.cn

Ruby: arr.sort
来源：http://gx.huixinmuqiang.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ed.jctech888.com.cn

[N03] 快速排序（分治示例）
来源：http://qn.muxihuayi.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://tp.huanxung.cn

PHP:  // 递归实现，或用 usort
来源：http://hj.newstarts.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bc.haigaiapp.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://de.gzmigu.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://jf.panjiajie.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wp.shxzukj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://zv.shtwfgs.cn

C#:   // 手写递归，或 Array.Sort
来源：http://eh.chemitech.net.cn

[N04] 斐波那契数列
来源：http://zw.yuexingan06.cn


<!-- 参考信息 -->