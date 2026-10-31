代发 wailian999

Go:   time.Now().AddDate(0, 0, 7)
来源：http://yx.huixinmuqiang.cn

Ruby: Time.now + 7 * 86400
来源：http://ka.hahajie.cn

C#:   DateTime.Now.AddDays(7)
来源：http://qd.haigaiapp.cn

[J06] 计算两时间之差
来源：http://fw.huixinmuqiang.cn

Py:   (end - start).total_seconds()
来源：http://zz.szxytkj.cn

PHP:  $end->diff($start)->days;
来源：http://sp.chemitech.net.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://md.yuntaijiaju.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://fz.asd995.cn

Java: Duration.between(start, end).toSeconds()
来源：http://np.szxytkj.cn

Go:   end.Sub(start).Hours()
来源：http://ew.bjjhwx.cn

Ruby: end - start                 # 返回秒数
来源：http://ha.huixiangedu.cn

C#:   (end - start).TotalSeconds
来源：http://az.hnjuh.cn

[J07] 比较两个日期
来源：http://qp.bookmarksfly.cn

Py:   d1 < d2;  d1 == d2
来源：http://nf.muxihuayi.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://lg.bookmarksfly.cn

JS:   d1.getTime() < d2.getTime()
来源：http://zq.muxihuayi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://rv.panjiajie.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ou.chemitech.net.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://nz.szxytkj.cn

Ruby: d1 < d2;  d1 == d2
来源：http://pi.hnjuh.cn

C#:   d1 < d2;  d1 == d2
来源：http://mn.shxzskj.cn

[J08] 提取年月日与星期
来源：http://oy.nszjky.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://pr.newstarts.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://dc.asd995.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ll.huixinmuqiang.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hd.chemitech.net.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://oq.yuexingan06.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://rx.panjiajie.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://bi.nicolike.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://tv.9csxet.cn

[J09] 时区处理
来源：http://pu.9csxet.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://kg.haigaiapp.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://tr.shtwfgs.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ro.9csxet.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bi.haigaiapp.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mz.shtwfgs.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://cb.jianghongdianzi.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://uz.9csxet.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://eq.wgjwhj.cn

[J10] 取今天 / 本月第一天
来源：http://dr.huanxung.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://io.haigaiapp.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://bc.gzmigu.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://uw.lnxyls.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://gq.szsharing.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qj.szsharing.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ib.nicolike.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://jj.nicolike.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://cb.jianghongdianzi.cn

================================================================================
来源：http://cz.huixinmuqiang.cn

K. JSON 与序列化
来源：http://oq.jctech888.com.cn

================================================================================
来源：http://wz.newstarts.cn

[K01] 对象转 JSON 字符串
来源：http://te.bjjhwx.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://xc.haigaiapp.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://qi.gzmigu.cn

JS:   JSON.stringify(obj)
来源：http://bk.jctech888.com.cn

TS:   JSON.stringify(obj)
来源：http://od.shtwfgs.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://bm.shxzskj.cn

Go:   json.Marshal(obj)
来源：http://up.nicolike.cn

Ruby: obj.to_json                                     // require "json"
来源：http://bj.huixiangedu.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://xo.asd995.cn

[K02] JSON 字符串转对象
来源：http://yi.bjjhwx.cn

Py:   json.loads(s)
来源：http://wq.hnjuh.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://lk.9csxet.cn

JS:   JSON.parse(s)
来源：http://gt.szsharing.cn

TS:   JSON.parse(s)
来源：http://sb.colortex.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://he.haigaiapp.cn

Go:   json.Unmarshal(data, &v)
来源：http://bd.chemitech.net.cn

Ruby: JSON.parse(s)
来源：http://ww.shtwfgs.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://tg.muxihuayi.cn

[K03] JSON 美化输出（带缩进）
来源：http://dz.muxihuayi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://sn.huanxung.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mq.chemitech.net.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://kk.panjiajie.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://mx.colortex.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ar.huixinmuqiang.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xe.shxzskj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://tr.bookmarksfly.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://fv.huanxung.cn

[K04] 读取 JSON 文件
来源：http://tw.panjiajie.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ed.lnxyls.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://gm.nicolike.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cu.wgjwhj.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ze.colortex.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://so.nicolike.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://xe.panjiajie.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://dd.colortex.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://uh.asd995.cn

[K05] 深拷贝对象
来源：http://uk.huanxung.cn

Py:   copy.deepcopy(obj)
来源：http://ui.shxzukj.cn

PHP:  unserialize(serialize($obj));
来源：http://so.nicolike.cn

JS:   structuredClone(obj)
来源：http://qg.szsharing.cn

TS:   structuredClone(obj)
来源：http://jo.jianghongdianzi.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://em.yuexingan06.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ey.muxihuayi.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://lj.panjiajie.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://tv.haigaiapp.cn

[K06] 解析 URL 查询串
来源：http://vu.jctech888.com.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://iw.nszjky.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mi.huixinmuqiang.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wf.huixinmuqiang.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bo.szsharing.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ew.chemitech.net.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://pr.yuntaijiaju.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://nm.haigaiapp.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://xd.bookmarksfly.cn

[K07] 进制转换
来源：http://nk.521024.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://jp.jctech888.com.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ec.shtwfgs.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xn.bookmarksfly.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wm.shxzskj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://te.shtwfgs.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://yn.panjiajie.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://vy.hnjuh.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://fp.muxihuayi.cn

[K08] 二进制序列化（非 JSON）
来源：http://om.panjiajie.cn

Py:   pickle.dumps(obj)
来源：http://co.chemitech.net.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://su.colortex.cn

JS:   v8.serialize(obj)        // Node
来源：http://tm.hnjuh.cn

TS:   v8.serialize(obj)        // Node
来源：http://rg.nszjky.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://kh.bookmarksfly.cn

Go:   encoding/gob
来源：http://el.hnjuh.cn

Ruby: Marshal.dump(obj)
来源：http://hm.yuexingan06.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://pi.huixinmuqiang.cn

================================================================================
来源：http://ru.hahajie.cn

L. 网络请求
来源：http://ez.gzmigu.cn

================================================================================
来源：http://qb.shtwfgs.cn

[L01] 发送 GET 请求
来源：http://bj.yuexingan06.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ez.nszjky.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://je.nszjky.cn

JS:   await fetch(url)
来源：http://sr.bjjhwx.cn

TS:   await fetch(url)
来源：http://pa.yuexingan06.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://gn.yuexingan06.cn

Go:   resp, err := http.Get(url)
来源：http://vb.shxzukj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://as.huixiangedu.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ql.asd995.cn

[L02] 发送 POST JSON
来源：http://gq.hnjuh.cn

Py:   requests.post(url, json={"a": 1})
来源：http://af.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://cs.huanxung.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cn.huixinmuqiang.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://iv.wgjwhj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://sb.panjiajie.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mh.szsharing.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://go.yuexingan06.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://eb.nszjky.cn

[L03] 设置自定义请求头
来源：http://lg.szsharing.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://nx.haigaiapp.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://sr.hnjuh.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ur.wgjwhj.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://oe.jianghongdianzi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://kn.9csxet.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://cy.shxzukj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mw.huanxung.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://bu.jianghongdianzi.cn

[L04] 设置超时
来源：http://mu.chemitech.net.cn

Py:   requests.get(url, timeout=5)
来源：http://ko.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://lg.521024.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://me.szxytkj.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zp.shxzskj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://dl.yuntaijiaju.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://zm.huanxung.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ws.jianghongdianzi.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://le.wgjwhj.cn

[L05] 上传文件（multipart）
来源：http://gi.asd995.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://xv.521024.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ul.bjjhwx.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://on.wgjwhj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://tp.521024.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://cf.nszjky.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://tq.hnjuh.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://cs.panjiajie.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://bu.521024.cn

[L06] 解析响应为 JSON
来源：http://ck.szsharing.cn

Py:   resp.json()
来源：http://zq.newstarts.cn

PHP:  json_decode($body, true);
来源：http://ko.wgjwhj.cn

JS:   await resp.json()
来源：http://ng.shxzukj.cn

TS:   await resp.json()
来源：http://jf.chemitech.net.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wf.newstarts.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://he.colortex.cn

Ruby: JSON.parse(resp.body)
来源：http://cq.jctech888.com.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://zg.wgjwhj.cn

[L07] 处理 HTTP 状态码
来源：http://gk.chemitech.net.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://sy.jianghongdianzi.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://sb.shxzukj.cn

JS:   resp.ok;  resp.status
来源：http://sn.lnxyls.cn

TS:   resp.ok;  resp.status
来源：http://hw.jctech888.com.cn

Java: resp.statusCode()
来源：http://vb.9csxet.cn

Go:   resp.StatusCode
来源：http://ah.yuntaijiaju.cn

Ruby: resp.code.to_i
来源：http://xd.szsharing.cn

C#:   (int)resp.StatusCode
来源：http://di.shtwfgs.cn

[L08] 并发请求多个地址
来源：http://go.bjjhwx.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://lp.chemitech.net.cn

PHP:  curl_multi_init() 系列
来源：http://gj.yuntaijiaju.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fd.nicolike.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gd.newstarts.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ze.asd995.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ry.szsharing.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ai.asd995.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ru.gzmigu.cn

================================================================================
来源：http://op.jctech888.com.cn

M. 命令行 / 进程 / 环境
来源：http://ey.szxytkj.cn

================================================================================
来源：http://lc.chemitech.net.cn

[M01] 读取命令行参数
来源：http://qb.hnjuh.cn

Py:   sys.argv[1:]
来源：http://ls.yuexingan06.cn

PHP:  $argv;  $argc;
来源：http://oi.shxzukj.cn

JS:   process.argv.slice(2)
来源：http://gp.bookmarksfly.cn

TS:   process.argv.slice(2)
来源：http://nf.lnxyls.cn

Java: args 数组（main 方法参数）
来源：http://is.szsharing.cn

Go:   os.Args[1:]
来源：http://aw.bjjhwx.cn

Ruby: ARGV
来源：http://ot.nicolike.cn

C#:   args 数组（Main 方法参数）
来源：http://da.huixiangedu.cn

[M02] 读取环境变量
来源：http://qm.huixiangedu.cn

Py:   os.environ.get("HOME")
来源：http://mq.lnxyls.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hw.yuexingan06.cn

JS:   process.env.HOME
来源：http://xe.lnxyls.cn

TS:   process.env.HOME
来源：http://gv.shtwfgs.cn

Java: System.getenv("HOME")
来源：http://nl.9csxet.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://xq.newstarts.cn

Ruby: ENV["HOME"]
来源：http://ni.nicolike.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ae.bookmarksfly.cn

[M03] 执行外部命令
来源：http://uj.lnxyls.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://yo.yuntaijiaju.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hy.yuexingan06.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://pc.nicolike.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ju.szsharing.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://cu.gzmigu.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://kr.521024.cn

Ruby: system("ls -l");  `ls -l`
来源：http://pn.bjjhwx.cn

C#:   Process.Start("ls", "-l");
来源：http://mg.panjiajie.cn

[M04] 获取当前工作目录
来源：http://oj.szsharing.cn

Py:   os.getcwd()
来源：http://sn.huixiangedu.cn

PHP:  getcwd();
来源：http://el.wgjwhj.cn

JS:   process.cwd()
来源：http://fc.huixinmuqiang.cn

TS:   process.cwd()
来源：http://rv.bjjhwx.cn

Java: Path.of("").toAbsolutePath()
来源：http://bh.colortex.cn

Go:   os.Getwd()
来源：http://jv.nicolike.cn

Ruby: Dir.pwd
来源：http://rp.huanxung.cn

C#:   Directory.GetCurrentDirectory()
来源：http://jg.nicolike.cn

[M05] 设置退出码
来源：http://fc.9csxet.cn

Py:   sys.exit(1)
来源：http://az.wgjwhj.cn

PHP:  exit(1);
来源：http://ja.asd995.cn

JS:   process.exit(1)
来源：http://em.yuntaijiaju.cn

TS:   process.exit(1)
来源：http://fq.newstarts.cn

Java: System.exit(1)
来源：http://xi.huanxung.cn

Go:   os.Exit(1)
来源：http://hn.colortex.cn

Ruby: exit 1
来源：http://ok.yuntaijiaju.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://zm.muxihuayi.cn

[M06] 向标准错误输出
来源：http://vr.panjiajie.cn

Py:   print("err", file=sys.stderr)
来源：http://di.colortex.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://uz.haigaiapp.cn

JS:   console.error("err")
来源：http://ni.lnxyls.cn

TS:   console.error("err")
来源：http://mq.lnxyls.cn

Java: System.err.println("err")
来源：http://vb.hnjuh.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://jp.haigaiapp.cn

Ruby: warn "err"
来源：http://gu.nicolike.cn

C#:   Console.Error.WriteLine("err")
来源：http://je.nicolike.cn

[M07] 判断是否为主入口
来源：http://ka.newstarts.cn

Py:   if __name__ == "__main__":
来源：http://gz.yuexingan06.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://io.gzmigu.cn

JS:   require.main === module
来源：http://bb.huixinmuqiang.cn

TS:   require.main === module
来源：http://lz.shxzukj.cn

Java: public static void main(String[] args)
来源：http://xw.bookmarksfly.cn

Go:   func main()
来源：http://gr.yuexingan06.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mx.yuntaijiaju.cn

C#:   static void Main(string[] args)
来源：http://mi.lnxyls.cn

[M08] 获取系统与运行时信息
来源：http://lj.wgjwhj.cn

Py:   platform.system();  platform.python_version()
来源：http://vw.jctech888.com.cn

PHP:  PHP_OS;  phpversion();
来源：http://nv.nszjky.cn

JS:   process.platform;  process.version
来源：http://zu.shxzskj.cn

TS:   process.platform;  process.version
来源：http://fy.szsharing.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ou.shxzskj.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://wt.shtwfgs.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://vw.panjiajie.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://je.521024.cn

================================================================================
来源：http://ql.9csxet.cn

N. 数据结构与算法
来源：http://wr.521024.cn

================================================================================
来源：http://jm.szxytkj.cn

[N01] 二分查找（有序数组）
来源：http://us.shxzukj.cn

Py:   bisect.bisect_left(arr, x)
来源：http://qm.hnjuh.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ns.huixiangedu.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wm.gzmigu.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rw.yuexingan06.cn

Java: Arrays.binarySearch(arr, x)
来源：http://bl.nszjky.cn

Go:   sort.SearchInts(arr, x)
来源：http://kl.huixinmuqiang.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://lp.521024.cn

C#:   Array.BinarySearch(arr, x)
来源：http://mk.yuntaijiaju.cn

[N02] 排序（工程实践用内置实现）
来源：http://fc.nicolike.cn

Py:   sorted(arr);  arr.sort()
来源：http://dj.asd995.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://vc.huixiangedu.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://rg.yuexingan06.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://hd.panjiajie.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://qc.asd995.cn

Go:   slices.Sort(arr)
来源：http://jq.haigaiapp.cn

Ruby: arr.sort
来源：http://cv.nicolike.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://xp.shtwfgs.cn

[N03] 快速排序（分治示例）
来源：http://rv.panjiajie.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://gk.nszjky.cn

PHP:  // 递归实现，或用 usort
来源：http://dq.bjjhwx.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gz.bjjhwx.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ah.nszjky.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://se.asd995.cn


<!-- 参考信息 -->