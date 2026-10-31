代发 wailian999

Go:   time.Now().AddDate(0, 0, 7)
来源：http://cq.jctech888.com.cn

Ruby: Time.now + 7 * 86400
来源：http://io.bookmarksfly.cn

C#:   DateTime.Now.AddDays(7)
来源：http://zh.bookmarksfly.cn

[J06] 计算两时间之差
来源：http://cd.nszjky.cn

Py:   (end - start).total_seconds()
来源：http://pa.hahajie.cn

PHP:  $end->diff($start)->days;
来源：http://qr.shtwfgs.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://pf.shxzukj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://yc.asd995.cn

Java: Duration.between(start, end).toSeconds()
来源：http://iz.nszjky.cn

Go:   end.Sub(start).Hours()
来源：http://ac.shxzskj.cn

Ruby: end - start                 # 返回秒数
来源：http://nm.hahajie.cn

C#:   (end - start).TotalSeconds
来源：http://ls.chemitech.net.cn

[J07] 比较两个日期
来源：http://vo.haigaiapp.cn

Py:   d1 < d2;  d1 == d2
来源：http://gg.shxzukj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://md.lnxyls.cn

JS:   d1.getTime() < d2.getTime()
来源：http://qb.haigaiapp.cn

TS:   d1.getTime() < d2.getTime()
来源：http://sg.9csxet.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mj.jianghongdianzi.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://tr.hahajie.cn

Ruby: d1 < d2;  d1 == d2
来源：http://dc.huixinmuqiang.cn

C#:   d1 < d2;  d1 == d2
来源：http://zr.huixiangedu.cn

[J08] 提取年月日与星期
来源：http://hr.huixinmuqiang.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://he.yuexingan06.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://eq.asd995.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xy.muxihuayi.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://yt.colortex.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hc.asd995.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://kl.muxihuayi.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ui.huixinmuqiang.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wg.bookmarksfly.cn

[J09] 时区处理
来源：http://qv.szxytkj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://au.bjjhwx.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://re.huanxung.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dn.huixiangedu.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vj.yuntaijiaju.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wa.hnjuh.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zb.bjjhwx.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://fw.panjiajie.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mc.muxihuayi.cn

[J10] 取今天 / 本月第一天
来源：http://zn.huanxung.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://bj.muxihuayi.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://yc.wgjwhj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://zl.gzmigu.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://tk.huanxung.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://co.shxzskj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://kd.panjiajie.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://su.chemitech.net.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://cz.wgjwhj.cn

================================================================================
来源：http://hn.shtwfgs.cn

K. JSON 与序列化
来源：http://ib.gzmigu.cn

================================================================================
来源：http://ba.muxihuayi.cn

[K01] 对象转 JSON 字符串
来源：http://ik.521024.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://pi.muxihuayi.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://jp.nicolike.cn

JS:   JSON.stringify(obj)
来源：http://ug.colortex.cn

TS:   JSON.stringify(obj)
来源：http://qf.9csxet.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://uw.colortex.cn

Go:   json.Marshal(obj)
来源：http://tl.muxihuayi.cn

Ruby: obj.to_json                                     // require "json"
来源：http://my.colortex.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://pt.gzmigu.cn

[K02] JSON 字符串转对象
来源：http://ac.szsharing.cn

Py:   json.loads(s)
来源：http://lp.newstarts.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://cq.huixinmuqiang.cn

JS:   JSON.parse(s)
来源：http://lk.9csxet.cn

TS:   JSON.parse(s)
来源：http://dq.yuntaijiaju.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://yo.huanxung.cn

Go:   json.Unmarshal(data, &v)
来源：http://tg.shxzukj.cn

Ruby: JSON.parse(s)
来源：http://cd.hahajie.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://vn.huanxung.cn

[K03] JSON 美化输出（带缩进）
来源：http://ac.bjjhwx.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ek.chemitech.net.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mh.muxihuayi.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ft.wgjwhj.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ih.shtwfgs.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hs.szsharing.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://to.9csxet.cn

Ruby: JSON.pretty_generate(obj)
来源：http://qv.panjiajie.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://bf.yuexingan06.cn

[K04] 读取 JSON 文件
来源：http://mf.nszjky.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://tg.jctech888.com.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://cs.hahajie.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://iy.9csxet.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zk.jianghongdianzi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://lx.haigaiapp.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://zk.bjjhwx.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://av.haigaiapp.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ma.chemitech.net.cn

[K05] 深拷贝对象
来源：http://gb.muxihuayi.cn

Py:   copy.deepcopy(obj)
来源：http://mq.asd995.cn

PHP:  unserialize(serialize($obj));
来源：http://xq.chemitech.net.cn

JS:   structuredClone(obj)
来源：http://nv.asd995.cn

TS:   structuredClone(obj)
来源：http://li.asd995.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://cg.521024.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ks.bjjhwx.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wf.521024.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://xc.yuexingan06.cn

[K06] 解析 URL 查询串
来源：http://wh.muxihuayi.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hr.huanxung.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://yk.szxytkj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sd.huixinmuqiang.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ui.nicolike.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://gr.asd995.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ql.hahajie.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vw.asd995.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wm.nszjky.cn

[K07] 进制转换
来源：http://ft.lnxyls.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://zw.jctech888.com.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://bk.lnxyls.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mo.muxihuayi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://lw.yuntaijiaju.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://er.jianghongdianzi.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ps.asd995.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://fk.bjjhwx.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://pn.huixiangedu.cn

[K08] 二进制序列化（非 JSON）
来源：http://vn.hnjuh.cn

Py:   pickle.dumps(obj)
来源：http://ml.521024.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://dh.shxzskj.cn

JS:   v8.serialize(obj)        // Node
来源：http://od.jianghongdianzi.cn

TS:   v8.serialize(obj)        // Node
来源：http://ve.nicolike.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://sq.szsharing.cn

Go:   encoding/gob
来源：http://ht.hahajie.cn

Ruby: Marshal.dump(obj)
来源：http://bv.521024.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://jg.huanxung.cn

================================================================================
来源：http://ky.panjiajie.cn

L. 网络请求
来源：http://ou.jianghongdianzi.cn

================================================================================
来源：http://kw.shxzukj.cn

[L01] 发送 GET 请求
来源：http://ui.bookmarksfly.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://yc.huixinmuqiang.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://jd.gzmigu.cn

JS:   await fetch(url)
来源：http://zn.yuexingan06.cn

TS:   await fetch(url)
来源：http://ud.yuntaijiaju.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://lf.huixinmuqiang.cn

Go:   resp, err := http.Get(url)
来源：http://hl.szxytkj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ne.muxihuayi.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://rp.huixinmuqiang.cn

[L02] 发送 POST JSON
来源：http://sx.szsharing.cn

Py:   requests.post(url, json={"a": 1})
来源：http://tm.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://pw.jctech888.com.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pu.shxzskj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hv.muxihuayi.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://xn.huixinmuqiang.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ug.yuexingan06.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://lc.chemitech.net.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ci.hnjuh.cn

[L03] 设置自定义请求头
来源：http://rc.haigaiapp.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hb.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://xl.bjjhwx.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://iv.shxzskj.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wu.huanxung.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://aw.yuntaijiaju.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://cs.9csxet.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://kk.yuntaijiaju.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://gz.bookmarksfly.cn

[L04] 设置超时
来源：http://bc.yuntaijiaju.cn

Py:   requests.get(url, timeout=5)
来源：http://us.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://tf.9csxet.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lg.gzmigu.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lu.yuntaijiaju.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://pj.shxzskj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hj.shtwfgs.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://uo.jctech888.com.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://lh.jianghongdianzi.cn

[L05] 上传文件（multipart）
来源：http://ly.nszjky.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://jf.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ia.bjjhwx.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ex.jctech888.com.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ey.colortex.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://jq.hnjuh.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ab.9csxet.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://se.newstarts.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ni.shxzukj.cn

[L06] 解析响应为 JSON
来源：http://pj.shxzukj.cn

Py:   resp.json()
来源：http://rj.szxytkj.cn

PHP:  json_decode($body, true);
来源：http://jw.huanxung.cn

JS:   await resp.json()
来源：http://mg.gzmigu.cn

TS:   await resp.json()
来源：http://nk.gzmigu.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://cc.bookmarksfly.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://uh.9csxet.cn

Ruby: JSON.parse(resp.body)
来源：http://rh.asd995.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ug.bjjhwx.cn

[L07] 处理 HTTP 状态码
来源：http://eu.panjiajie.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://my.szxytkj.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://da.nszjky.cn

JS:   resp.ok;  resp.status
来源：http://eu.wgjwhj.cn

TS:   resp.ok;  resp.status
来源：http://wu.bjjhwx.cn

Java: resp.statusCode()
来源：http://xa.yuexingan06.cn

Go:   resp.StatusCode
来源：http://hy.yuntaijiaju.cn

Ruby: resp.code.to_i
来源：http://ra.nszjky.cn

C#:   (int)resp.StatusCode
来源：http://fr.huixinmuqiang.cn

[L08] 并发请求多个地址
来源：http://ya.shxzskj.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://tm.huanxung.cn

PHP:  curl_multi_init() 系列
来源：http://da.shxzukj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mz.hnjuh.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://eb.521024.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hv.muxihuayi.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ua.jctech888.com.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ku.yuntaijiaju.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://li.bjjhwx.cn

================================================================================
来源：http://cq.hnjuh.cn

M. 命令行 / 进程 / 环境
来源：http://zk.shtwfgs.cn

================================================================================
来源：http://js.shtwfgs.cn

[M01] 读取命令行参数
来源：http://ix.wgjwhj.cn

Py:   sys.argv[1:]
来源：http://af.nszjky.cn

PHP:  $argv;  $argc;
来源：http://hk.9csxet.cn

JS:   process.argv.slice(2)
来源：http://hd.jianghongdianzi.cn

TS:   process.argv.slice(2)
来源：http://cg.huanxung.cn

Java: args 数组（main 方法参数）
来源：http://bd.panjiajie.cn

Go:   os.Args[1:]
来源：http://rj.haigaiapp.cn

Ruby: ARGV
来源：http://sx.521024.cn

C#:   args 数组（Main 方法参数）
来源：http://iz.nszjky.cn

[M02] 读取环境变量
来源：http://fa.521024.cn

Py:   os.environ.get("HOME")
来源：http://nd.hahajie.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://cq.huixinmuqiang.cn

JS:   process.env.HOME
来源：http://ai.shxzukj.cn

TS:   process.env.HOME
来源：http://jx.yuntaijiaju.cn

Java: System.getenv("HOME")
来源：http://rb.wgjwhj.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wv.yuntaijiaju.cn

Ruby: ENV["HOME"]
来源：http://xj.lnxyls.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://iq.huixiangedu.cn

[M03] 执行外部命令
来源：http://xu.huanxung.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://dh.bjjhwx.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://kr.shxzukj.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ir.nicolike.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://mb.muxihuayi.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://si.hahajie.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://qt.haigaiapp.cn

Ruby: system("ls -l");  `ls -l`
来源：http://yu.yuexingan06.cn

C#:   Process.Start("ls", "-l");
来源：http://wc.chemitech.net.cn

[M04] 获取当前工作目录
来源：http://uo.colortex.cn

Py:   os.getcwd()
来源：http://ui.colortex.cn

PHP:  getcwd();
来源：http://tw.nicolike.cn

JS:   process.cwd()
来源：http://bo.yuexingan06.cn

TS:   process.cwd()
来源：http://ov.hnjuh.cn

Java: Path.of("").toAbsolutePath()
来源：http://vc.huixiangedu.cn

Go:   os.Getwd()
来源：http://bg.shxzskj.cn

Ruby: Dir.pwd
来源：http://gy.wgjwhj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://xe.muxihuayi.cn

[M05] 设置退出码
来源：http://gm.haigaiapp.cn

Py:   sys.exit(1)
来源：http://il.colortex.cn

PHP:  exit(1);
来源：http://cm.chemitech.net.cn

JS:   process.exit(1)
来源：http://kj.hnjuh.cn

TS:   process.exit(1)
来源：http://xy.jianghongdianzi.cn

Java: System.exit(1)
来源：http://ou.bookmarksfly.cn

Go:   os.Exit(1)
来源：http://pp.wgjwhj.cn

Ruby: exit 1
来源：http://cx.haigaiapp.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://xc.yuexingan06.cn

[M06] 向标准错误输出
来源：http://sb.nicolike.cn

Py:   print("err", file=sys.stderr)
来源：http://wg.gzmigu.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://mp.yuntaijiaju.cn

JS:   console.error("err")
来源：http://rz.muxihuayi.cn

TS:   console.error("err")
来源：http://aw.jianghongdianzi.cn

Java: System.err.println("err")
来源：http://lj.shxzukj.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://oh.hnjuh.cn

Ruby: warn "err"
来源：http://yh.szsharing.cn

C#:   Console.Error.WriteLine("err")
来源：http://ca.nicolike.cn

[M07] 判断是否为主入口
来源：http://jn.huixiangedu.cn

Py:   if __name__ == "__main__":
来源：http://qc.yuexingan06.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ex.bookmarksfly.cn

JS:   require.main === module
来源：http://cp.nszjky.cn

TS:   require.main === module
来源：http://nv.hahajie.cn

Java: public static void main(String[] args)
来源：http://mc.hahajie.cn

Go:   func main()
来源：http://dh.lnxyls.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://nv.hahajie.cn

C#:   static void Main(string[] args)
来源：http://nc.nicolike.cn

[M08] 获取系统与运行时信息
来源：http://nu.bookmarksfly.cn

Py:   platform.system();  platform.python_version()
来源：http://xp.yuexingan06.cn

PHP:  PHP_OS;  phpversion();
来源：http://tt.colortex.cn

JS:   process.platform;  process.version
来源：http://sn.9csxet.cn

TS:   process.platform;  process.version
来源：http://oc.newstarts.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xr.huanxung.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://bs.huanxung.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://xn.colortex.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ed.huanxung.cn

================================================================================
来源：http://nu.wgjwhj.cn

N. 数据结构与算法
来源：http://hy.colortex.cn

================================================================================
来源：http://bn.panjiajie.cn

[N01] 二分查找（有序数组）
来源：http://jv.wgjwhj.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ux.bjjhwx.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://fj.nszjky.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://px.huixinmuqiang.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zi.wgjwhj.cn

Java: Arrays.binarySearch(arr, x)
来源：http://jo.jctech888.com.cn

Go:   sort.SearchInts(arr, x)
来源：http://ob.newstarts.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://kr.nicolike.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ui.chemitech.net.cn

[N02] 排序（工程实践用内置实现）
来源：http://wa.yuntaijiaju.cn

Py:   sorted(arr);  arr.sort()
来源：http://ms.shtwfgs.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://td.bjjhwx.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://wg.asd995.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://tt.huixinmuqiang.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://gl.yuntaijiaju.cn

Go:   slices.Sort(arr)
来源：http://gh.huanxung.cn

Ruby: arr.sort
来源：http://lx.lnxyls.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://en.huixiangedu.cn

[N03] 快速排序（分治示例）
来源：http://yv.wgjwhj.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://yx.muxihuayi.cn

PHP:  // 递归实现，或用 usort
来源：http://he.lnxyls.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mg.hnjuh.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vm.huanxung.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wt.chemitech.net.cn


<!-- 参考信息 -->