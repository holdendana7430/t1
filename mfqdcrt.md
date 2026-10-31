代发 wailian999

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://kk.szsharing.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://si.haigaiapp.cn

[J05] 时间加减（加 7 天）
来源：http://pa.newstarts.cn

Py:   now + timedelta(days=7)
来源：http://iw.bjjhwx.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://fv.bookmarksfly.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://fo.bjjhwx.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://zj.asd995.cn

Java: LocalDate.now().plusDays(7)
来源：http://zq.gzmigu.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ab.haigaiapp.cn

Ruby: Time.now + 7 * 86400
来源：http://rx.jianghongdianzi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://zl.hnjuh.cn

[J06] 计算两时间之差
来源：http://lg.gzmigu.cn

Py:   (end - start).total_seconds()
来源：http://ei.bookmarksfly.cn

PHP:  $end->diff($start)->days;
来源：http://fq.bookmarksfly.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://vm.gzmigu.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://kh.huixiangedu.cn

Java: Duration.between(start, end).toSeconds()
来源：http://bl.haigaiapp.cn

Go:   end.Sub(start).Hours()
来源：http://md.szxytkj.cn

Ruby: end - start                 # 返回秒数
来源：http://ji.hnjuh.cn

C#:   (end - start).TotalSeconds
来源：http://pl.bookmarksfly.cn

[J07] 比较两个日期
来源：http://xa.nszjky.cn

Py:   d1 < d2;  d1 == d2
来源：http://jf.chemitech.net.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://qh.muxihuayi.cn

JS:   d1.getTime() < d2.getTime()
来源：http://so.huixinmuqiang.cn

TS:   d1.getTime() < d2.getTime()
来源：http://fw.newstarts.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://jg.panjiajie.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://am.muxihuayi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://nu.colortex.cn

C#:   d1 < d2;  d1 == d2
来源：http://gw.nszjky.cn

[J08] 提取年月日与星期
来源：http://qp.colortex.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://zw.huixinmuqiang.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://vl.521024.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://qu.colortex.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ke.521024.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://uj.nicolike.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ub.huixiangedu.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://br.yuexingan06.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ej.szxytkj.cn

[J09] 时区处理
来源：http://ml.szsharing.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://dy.lnxyls.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://rq.asd995.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jr.bookmarksfly.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xh.wgjwhj.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://fp.haigaiapp.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://gi.shxzskj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://sy.panjiajie.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qg.asd995.cn

[J10] 取今天 / 本月第一天
来源：http://rn.hnjuh.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://zs.muxihuayi.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://uw.nszjky.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://gb.gzmigu.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://iy.szsharing.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mk.hnjuh.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://rf.jctech888.com.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://de.bookmarksfly.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://oa.hahajie.cn

================================================================================
来源：http://cw.shxzskj.cn

K. JSON 与序列化
来源：http://jw.hnjuh.cn

================================================================================
来源：http://ob.huanxung.cn

[K01] 对象转 JSON 字符串
来源：http://py.szxytkj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ue.szsharing.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hj.huixinmuqiang.cn

JS:   JSON.stringify(obj)
来源：http://xd.shxzskj.cn

TS:   JSON.stringify(obj)
来源：http://bl.huixinmuqiang.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ot.9csxet.cn

Go:   json.Marshal(obj)
来源：http://gp.szsharing.cn

Ruby: obj.to_json                                     // require "json"
来源：http://tt.yuexingan06.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ui.yuntaijiaju.cn

[K02] JSON 字符串转对象
来源：http://cd.9csxet.cn

Py:   json.loads(s)
来源：http://xf.huanxung.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ka.muxihuayi.cn

JS:   JSON.parse(s)
来源：http://xu.lnxyls.cn

TS:   JSON.parse(s)
来源：http://io.huanxung.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ql.huixinmuqiang.cn

Go:   json.Unmarshal(data, &v)
来源：http://la.jctech888.com.cn

Ruby: JSON.parse(s)
来源：http://zm.szxytkj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://cx.panjiajie.cn

[K03] JSON 美化输出（带缩进）
来源：http://zp.chemitech.net.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://lz.huixiangedu.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qk.yuexingan06.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://qo.jctech888.com.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://kc.bjjhwx.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://bc.newstarts.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://cm.nicolike.cn

Ruby: JSON.pretty_generate(obj)
来源：http://qi.huixinmuqiang.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://cn.yuntaijiaju.cn

[K04] 读取 JSON 文件
来源：http://pu.shtwfgs.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ij.nszjky.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://df.huanxung.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tt.nicolike.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bw.9csxet.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://fa.huixiangedu.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://fn.muxihuayi.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://wp.szxytkj.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://aq.shxzskj.cn

[K05] 深拷贝对象
来源：http://lt.521024.cn

Py:   copy.deepcopy(obj)
来源：http://tn.bookmarksfly.cn

PHP:  unserialize(serialize($obj));
来源：http://nc.hnjuh.cn

JS:   structuredClone(obj)
来源：http://hp.chemitech.net.cn

TS:   structuredClone(obj)
来源：http://ea.szsharing.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://kr.haigaiapp.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://em.jianghongdianzi.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hi.lnxyls.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://xn.bookmarksfly.cn

[K06] 解析 URL 查询串
来源：http://wq.hnjuh.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ck.colortex.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://xd.bookmarksfly.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yu.szsharing.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gh.yuexingan06.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://my.huixiangedu.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://pm.szxytkj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ih.hnjuh.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ii.asd995.cn

[K07] 进制转换
来源：http://nz.haigaiapp.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://gl.panjiajie.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ob.nicolike.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://zr.gzmigu.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://uw.huanxung.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xv.hahajie.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://du.521024.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://tg.nszjky.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mn.panjiajie.cn

[K08] 二进制序列化（非 JSON）
来源：http://bt.hahajie.cn

Py:   pickle.dumps(obj)
来源：http://jb.shxzskj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://bh.huixinmuqiang.cn

JS:   v8.serialize(obj)        // Node
来源：http://wi.huixinmuqiang.cn

TS:   v8.serialize(obj)        // Node
来源：http://qx.colortex.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://jj.muxihuayi.cn

Go:   encoding/gob
来源：http://je.bookmarksfly.cn

Ruby: Marshal.dump(obj)
来源：http://ht.jctech888.com.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://je.nicolike.cn

================================================================================
来源：http://vu.szxytkj.cn

L. 网络请求
来源：http://oz.yuexingan06.cn

================================================================================
来源：http://gb.szsharing.cn

[L01] 发送 GET 请求
来源：http://ap.yuexingan06.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.bookmarksfly.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://dh.jianghongdianzi.cn

JS:   await fetch(url)
来源：http://wc.521024.cn

TS:   await fetch(url)
来源：http://oc.szxytkj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://og.wgjwhj.cn

Go:   resp, err := http.Get(url)
来源：http://tr.shxzukj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://zm.lnxyls.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ji.bookmarksfly.cn

[L02] 发送 POST JSON
来源：http://pt.huanxung.cn

Py:   requests.post(url, json={"a": 1})
来源：http://eo.asd995.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://cy.shxzukj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ko.yuntaijiaju.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zj.bjjhwx.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ih.haigaiapp.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://av.yuexingan06.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ph.9csxet.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://rj.bookmarksfly.cn

[L03] 设置自定义请求头
来源：http://pq.panjiajie.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ww.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://yo.haigaiapp.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ck.newstarts.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://aj.wgjwhj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://yh.huixiangedu.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ho.gzmigu.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://tc.yuntaijiaju.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://le.szxytkj.cn

[L04] 设置超时
来源：http://qp.bjjhwx.cn

Py:   requests.get(url, timeout=5)
来源：http://rt.nicolike.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://nw.haigaiapp.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ov.chemitech.net.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dx.yuntaijiaju.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://pm.shtwfgs.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mg.huixiangedu.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://rr.szsharing.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://gp.panjiajie.cn

[L05] 上传文件（multipart）
来源：http://fw.panjiajie.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ym.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://la.9csxet.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://bl.bookmarksfly.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ns.hahajie.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://bf.huanxung.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://th.nicolike.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://rs.nicolike.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://sj.huixiangedu.cn

[L06] 解析响应为 JSON
来源：http://fc.hahajie.cn

Py:   resp.json()
来源：http://iy.jianghongdianzi.cn

PHP:  json_decode($body, true);
来源：http://ie.nicolike.cn

JS:   await resp.json()
来源：http://ik.huixiangedu.cn

TS:   await resp.json()
来源：http://ei.szsharing.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://bf.lnxyls.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mq.shtwfgs.cn

Ruby: JSON.parse(resp.body)
来源：http://zp.yuntaijiaju.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://av.yuntaijiaju.cn

[L07] 处理 HTTP 状态码
来源：http://or.chemitech.net.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://en.haigaiapp.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://la.nicolike.cn

JS:   resp.ok;  resp.status
来源：http://cd.newstarts.cn

TS:   resp.ok;  resp.status
来源：http://yy.huixinmuqiang.cn

Java: resp.statusCode()
来源：http://cx.shtwfgs.cn

Go:   resp.StatusCode
来源：http://sc.bjjhwx.cn

Ruby: resp.code.to_i
来源：http://hs.shxzukj.cn

C#:   (int)resp.StatusCode
来源：http://ai.chemitech.net.cn

[L08] 并发请求多个地址
来源：http://ya.shtwfgs.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://rb.521024.cn

PHP:  curl_multi_init() 系列
来源：http://zx.huixiangedu.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pz.wgjwhj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pb.newstarts.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hp.szsharing.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://eu.huanxung.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ev.shxzukj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://vw.wgjwhj.cn

================================================================================
来源：http://ts.asd995.cn

M. 命令行 / 进程 / 环境
来源：http://ov.huixiangedu.cn

================================================================================
来源：http://qa.huixinmuqiang.cn

[M01] 读取命令行参数
来源：http://bm.lnxyls.cn

Py:   sys.argv[1:]
来源：http://ae.jianghongdianzi.cn

PHP:  $argv;  $argc;
来源：http://th.jctech888.com.cn

JS:   process.argv.slice(2)
来源：http://ov.hahajie.cn

TS:   process.argv.slice(2)
来源：http://yl.shxzskj.cn

Java: args 数组（main 方法参数）
来源：http://km.nicolike.cn

Go:   os.Args[1:]
来源：http://ht.chemitech.net.cn

Ruby: ARGV
来源：http://zm.jctech888.com.cn

C#:   args 数组（Main 方法参数）
来源：http://yh.hnjuh.cn

[M02] 读取环境变量
来源：http://gu.panjiajie.cn

Py:   os.environ.get("HOME")
来源：http://ip.521024.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rq.jianghongdianzi.cn

JS:   process.env.HOME
来源：http://ui.521024.cn

TS:   process.env.HOME
来源：http://yh.bookmarksfly.cn

Java: System.getenv("HOME")
来源：http://ql.hnjuh.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hk.chemitech.net.cn

Ruby: ENV["HOME"]
来源：http://wb.shtwfgs.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://iy.yuntaijiaju.cn

[M03] 执行外部命令
来源：http://pp.muxihuayi.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://tr.jianghongdianzi.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://oo.huixiangedu.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://gm.bookmarksfly.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://st.chemitech.net.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://qf.shxzukj.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://dh.nszjky.cn

Ruby: system("ls -l");  `ls -l`
来源：http://xx.hnjuh.cn

C#:   Process.Start("ls", "-l");
来源：http://kn.jianghongdianzi.cn

[M04] 获取当前工作目录
来源：http://ug.nicolike.cn

Py:   os.getcwd()
来源：http://cw.jianghongdianzi.cn

PHP:  getcwd();
来源：http://wi.521024.cn

JS:   process.cwd()
来源：http://bd.huixiangedu.cn

TS:   process.cwd()
来源：http://jd.hahajie.cn

Java: Path.of("").toAbsolutePath()
来源：http://pc.yuexingan06.cn

Go:   os.Getwd()
来源：http://qw.yuexingan06.cn

Ruby: Dir.pwd
来源：http://pr.panjiajie.cn

C#:   Directory.GetCurrentDirectory()
来源：http://el.szxytkj.cn

[M05] 设置退出码
来源：http://oe.lnxyls.cn

Py:   sys.exit(1)
来源：http://id.shtwfgs.cn

PHP:  exit(1);
来源：http://oq.bjjhwx.cn

JS:   process.exit(1)
来源：http://ff.newstarts.cn

TS:   process.exit(1)
来源：http://wl.yuexingan06.cn

Java: System.exit(1)
来源：http://vn.shxzskj.cn

Go:   os.Exit(1)
来源：http://mn.lnxyls.cn

Ruby: exit 1
来源：http://nv.szsharing.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://fd.wgjwhj.cn

[M06] 向标准错误输出
来源：http://af.nszjky.cn

Py:   print("err", file=sys.stderr)
来源：http://kj.colortex.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ta.shxzskj.cn

JS:   console.error("err")
来源：http://oa.lnxyls.cn

TS:   console.error("err")
来源：http://wt.nszjky.cn

Java: System.err.println("err")
来源：http://mq.newstarts.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://rv.gzmigu.cn

Ruby: warn "err"
来源：http://jx.panjiajie.cn

C#:   Console.Error.WriteLine("err")
来源：http://ss.521024.cn

[M07] 判断是否为主入口
来源：http://at.hnjuh.cn

Py:   if __name__ == "__main__":
来源：http://pm.haigaiapp.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://xh.nicolike.cn

JS:   require.main === module
来源：http://vp.yuntaijiaju.cn

TS:   require.main === module
来源：http://hq.huixiangedu.cn

Java: public static void main(String[] args)
来源：http://ru.jianghongdianzi.cn

Go:   func main()
来源：http://np.nicolike.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://su.gzmigu.cn

C#:   static void Main(string[] args)
来源：http://jh.jianghongdianzi.cn

[M08] 获取系统与运行时信息
来源：http://ba.shxzskj.cn

Py:   platform.system();  platform.python_version()
来源：http://bo.shxzukj.cn

PHP:  PHP_OS;  phpversion();
来源：http://xj.bjjhwx.cn

JS:   process.platform;  process.version
来源：http://av.hahajie.cn

TS:   process.platform;  process.version
来源：http://tp.haigaiapp.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://qp.lnxyls.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://sl.asd995.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://yo.huanxung.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://xy.huixinmuqiang.cn

================================================================================
来源：http://dq.9csxet.cn

N. 数据结构与算法
来源：http://yv.hahajie.cn

================================================================================
来源：http://cp.yuntaijiaju.cn

[N01] 二分查找（有序数组）
来源：http://qx.jctech888.com.cn

Py:   bisect.bisect_left(arr, x)
来源：http://zq.yuntaijiaju.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://op.wgjwhj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://od.shxzskj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dq.jianghongdianzi.cn

Java: Arrays.binarySearch(arr, x)
来源：http://vt.bookmarksfly.cn

Go:   sort.SearchInts(arr, x)
来源：http://ag.newstarts.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://my.haigaiapp.cn

C#:   Array.BinarySearch(arr, x)
来源：http://rd.huixinmuqiang.cn

[N02] 排序（工程实践用内置实现）
来源：http://zn.hnjuh.cn

Py:   sorted(arr);  arr.sort()
来源：http://qr.huanxung.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://es.9csxet.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://dz.huanxung.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://jm.nszjky.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://fi.yuexingan06.cn

Go:   slices.Sort(arr)
来源：http://fd.panjiajie.cn


<!-- 参考信息 -->