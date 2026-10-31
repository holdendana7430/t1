代发 wailian999

PHP:  (new DateTime())->modify("+7 days");
来源：http://un.wgjwhj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ic.muxihuayi.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://fn.chemitech.net.cn

Java: LocalDate.now().plusDays(7)
来源：http://sy.hnjuh.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zh.muxihuayi.cn

Ruby: Time.now + 7 * 86400
来源：http://tl.asd995.cn

C#:   DateTime.Now.AddDays(7)
来源：http://qc.bjjhwx.cn

[J06] 计算两时间之差
来源：http://it.nicolike.cn

Py:   (end - start).total_seconds()
来源：http://eu.huixiangedu.cn

PHP:  $end->diff($start)->days;
来源：http://zn.hnjuh.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ll.yuexingan06.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://cm.panjiajie.cn

Java: Duration.between(start, end).toSeconds()
来源：http://tu.shtwfgs.cn

Go:   end.Sub(start).Hours()
来源：http://gp.lnxyls.cn

Ruby: end - start                 # 返回秒数
来源：http://vj.hahajie.cn

C#:   (end - start).TotalSeconds
来源：http://fo.521024.cn

[J07] 比较两个日期
来源：http://wy.colortex.cn

Py:   d1 < d2;  d1 == d2
来源：http://ub.bjjhwx.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://un.shtwfgs.cn

JS:   d1.getTime() < d2.getTime()
来源：http://wt.lnxyls.cn

TS:   d1.getTime() < d2.getTime()
来源：http://im.szsharing.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://bf.shtwfgs.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://lq.hnjuh.cn

Ruby: d1 < d2;  d1 == d2
来源：http://st.521024.cn

C#:   d1 < d2;  d1 == d2
来源：http://ud.chemitech.net.cn

[J08] 提取年月日与星期
来源：http://ck.yuntaijiaju.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://xv.huixiangedu.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://kd.colortex.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ef.jianghongdianzi.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://pn.shxzukj.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ij.nszjky.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://oc.colortex.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://lo.yuntaijiaju.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://xa.521024.cn

[J09] 时区处理
来源：http://jp.yuntaijiaju.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://dg.521024.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://yk.hahajie.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tq.shtwfgs.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bd.yuntaijiaju.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ke.bookmarksfly.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://za.jianghongdianzi.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://mt.yuntaijiaju.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://bc.yuexingan06.cn

[J10] 取今天 / 本月第一天
来源：http://ku.bookmarksfly.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://lf.huanxung.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ys.jctech888.com.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://nc.wgjwhj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://zz.yuexingan06.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qu.huixiangedu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://pt.huixiangedu.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wz.nicolike.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://pt.jctech888.com.cn

================================================================================
来源：http://nm.yuntaijiaju.cn

K. JSON 与序列化
来源：http://pm.yuexingan06.cn

================================================================================
来源：http://kt.gzmigu.cn

[K01] 对象转 JSON 字符串
来源：http://pz.szxytkj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://dz.shxzukj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://qq.chemitech.net.cn

JS:   JSON.stringify(obj)
来源：http://qq.nszjky.cn

TS:   JSON.stringify(obj)
来源：http://xx.colortex.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://kr.shxzskj.cn

Go:   json.Marshal(obj)
来源：http://jm.bookmarksfly.cn

Ruby: obj.to_json                                     // require "json"
来源：http://zn.huixiangedu.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://un.bookmarksfly.cn

[K02] JSON 字符串转对象
来源：http://tl.shtwfgs.cn

Py:   json.loads(s)
来源：http://vx.yuntaijiaju.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://nm.asd995.cn

JS:   JSON.parse(s)
来源：http://qf.huanxung.cn

TS:   JSON.parse(s)
来源：http://pv.shtwfgs.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://sh.huixinmuqiang.cn

Go:   json.Unmarshal(data, &v)
来源：http://bc.szxytkj.cn

Ruby: JSON.parse(s)
来源：http://cj.jctech888.com.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mc.huixinmuqiang.cn

[K03] JSON 美化输出（带缩进）
来源：http://wk.yuntaijiaju.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wv.lnxyls.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qv.muxihuayi.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://tc.newstarts.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://fb.lnxyls.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ns.bookmarksfly.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://px.muxihuayi.cn

Ruby: JSON.pretty_generate(obj)
来源：http://gq.bookmarksfly.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://eg.asd995.cn

[K04] 读取 JSON 文件
来源：http://rt.jctech888.com.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://iv.hahajie.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mx.shxzskj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dz.jianghongdianzi.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bd.szsharing.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://gp.jianghongdianzi.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://jh.lnxyls.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://df.panjiajie.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://gy.colortex.cn

[K05] 深拷贝对象
来源：http://tl.9csxet.cn

Py:   copy.deepcopy(obj)
来源：http://nz.gzmigu.cn

PHP:  unserialize(serialize($obj));
来源：http://ee.nszjky.cn

JS:   structuredClone(obj)
来源：http://oe.colortex.cn

TS:   structuredClone(obj)
来源：http://up.colortex.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://jh.521024.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://tg.muxihuayi.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zs.huixiangedu.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://tu.wgjwhj.cn

[K06] 解析 URL 查询串
来源：http://av.muxihuayi.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ut.asd995.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ph.jianghongdianzi.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rd.9csxet.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ah.haigaiapp.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ug.jctech888.com.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ts.hahajie.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wa.szsharing.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ec.nicolike.cn

[K07] 进制转换
来源：http://sj.lnxyls.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://bf.muxihuayi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://br.huanxung.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wn.huixiangedu.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ys.9csxet.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://pw.szsharing.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://nj.chemitech.net.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://fv.521024.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://gz.9csxet.cn

[K08] 二进制序列化（非 JSON）
来源：http://mp.jianghongdianzi.cn

Py:   pickle.dumps(obj)
来源：http://lq.colortex.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://up.shtwfgs.cn

JS:   v8.serialize(obj)        // Node
来源：http://hg.shxzukj.cn

TS:   v8.serialize(obj)        // Node
来源：http://jl.asd995.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://oh.haigaiapp.cn

Go:   encoding/gob
来源：http://mk.szxytkj.cn

Ruby: Marshal.dump(obj)
来源：http://mw.huixiangedu.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://gw.colortex.cn

================================================================================
来源：http://em.szxytkj.cn

L. 网络请求
来源：http://iu.shxzskj.cn

================================================================================
来源：http://jg.9csxet.cn

[L01] 发送 GET 请求
来源：http://ab.521024.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://vr.lnxyls.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://uu.9csxet.cn

JS:   await fetch(url)
来源：http://kt.wgjwhj.cn

TS:   await fetch(url)
来源：http://bj.huanxung.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://xs.nszjky.cn

Go:   resp, err := http.Get(url)
来源：http://cq.wgjwhj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ew.wgjwhj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://gl.colortex.cn

[L02] 发送 POST JSON
来源：http://wt.huanxung.cn

Py:   requests.post(url, json={"a": 1})
来源：http://pc.panjiajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://fy.szsharing.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zr.huixinmuqiang.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zf.shxzukj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://cw.521024.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wd.9csxet.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://tv.shtwfgs.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://br.shtwfgs.cn

[L03] 设置自定义请求头
来源：http://vc.shtwfgs.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://pf.wgjwhj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mq.yuexingan06.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ig.nszjky.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jq.szsharing.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mh.shtwfgs.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://on.huixiangedu.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ei.hahajie.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://tt.huixinmuqiang.cn

[L04] 设置超时
来源：http://pz.huixinmuqiang.cn

Py:   requests.get(url, timeout=5)
来源：http://id.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ht.chemitech.net.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lp.panjiajie.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hc.nicolike.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hh.wgjwhj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ou.huixinmuqiang.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://et.panjiajie.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wx.huanxung.cn

[L05] 上传文件（multipart）
来源：http://hw.huixinmuqiang.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://kw.yuntaijiaju.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://bb.huixinmuqiang.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ax.colortex.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://yh.szsharing.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://fj.gzmigu.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ml.lnxyls.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://df.nszjky.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://iq.jctech888.com.cn

[L06] 解析响应为 JSON
来源：http://oc.nicolike.cn

Py:   resp.json()
来源：http://to.szxytkj.cn

PHP:  json_decode($body, true);
来源：http://bx.lnxyls.cn

JS:   await resp.json()
来源：http://go.haigaiapp.cn

TS:   await resp.json()
来源：http://cv.hahajie.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://pp.jianghongdianzi.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://gc.szxytkj.cn

Ruby: JSON.parse(resp.body)
来源：http://ki.bookmarksfly.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://lv.hnjuh.cn

[L07] 处理 HTTP 状态码
来源：http://sc.nszjky.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://rq.jianghongdianzi.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://om.huixiangedu.cn

JS:   resp.ok;  resp.status
来源：http://ib.bjjhwx.cn

TS:   resp.ok;  resp.status
来源：http://qc.muxihuayi.cn

Java: resp.statusCode()
来源：http://qo.huixinmuqiang.cn

Go:   resp.StatusCode
来源：http://up.shxzskj.cn

Ruby: resp.code.to_i
来源：http://gu.gzmigu.cn

C#:   (int)resp.StatusCode
来源：http://ic.yuntaijiaju.cn

[L08] 并发请求多个地址
来源：http://ri.szsharing.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://fz.shxzukj.cn

PHP:  curl_multi_init() 系列
来源：http://ug.yuexingan06.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kc.wgjwhj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kr.huanxung.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wi.shxzskj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://lq.hahajie.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://qb.jctech888.com.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ua.nicolike.cn

================================================================================
来源：http://ow.huanxung.cn

M. 命令行 / 进程 / 环境
来源：http://vx.gzmigu.cn

================================================================================
来源：http://ok.muxihuayi.cn

[M01] 读取命令行参数
来源：http://ix.bookmarksfly.cn

Py:   sys.argv[1:]
来源：http://wq.szxytkj.cn

PHP:  $argv;  $argc;
来源：http://rl.newstarts.cn

JS:   process.argv.slice(2)
来源：http://kp.bjjhwx.cn

TS:   process.argv.slice(2)
来源：http://ki.huixinmuqiang.cn

Java: args 数组（main 方法参数）
来源：http://xt.asd995.cn

Go:   os.Args[1:]
来源：http://mp.hahajie.cn

Ruby: ARGV
来源：http://rs.hahajie.cn

C#:   args 数组（Main 方法参数）
来源：http://sx.huixiangedu.cn

[M02] 读取环境变量
来源：http://ng.shxzskj.cn

Py:   os.environ.get("HOME")
来源：http://mn.newstarts.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://pv.newstarts.cn

JS:   process.env.HOME
来源：http://bn.panjiajie.cn

TS:   process.env.HOME
来源：http://ie.szsharing.cn

Java: System.getenv("HOME")
来源：http://tm.bookmarksfly.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://fz.bookmarksfly.cn

Ruby: ENV["HOME"]
来源：http://in.chemitech.net.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://pj.huanxung.cn

[M03] 执行外部命令
来源：http://ik.shtwfgs.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ls.huanxung.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ta.szsharing.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ks.bjjhwx.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://yv.nszjky.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://un.szxytkj.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://zv.jianghongdianzi.cn

Ruby: system("ls -l");  `ls -l`
来源：http://bl.9csxet.cn

C#:   Process.Start("ls", "-l");
来源：http://yn.huixinmuqiang.cn

[M04] 获取当前工作目录
来源：http://qz.521024.cn

Py:   os.getcwd()
来源：http://kf.gzmigu.cn

PHP:  getcwd();
来源：http://nv.asd995.cn

JS:   process.cwd()
来源：http://tc.colortex.cn

TS:   process.cwd()
来源：http://er.shtwfgs.cn

Java: Path.of("").toAbsolutePath()
来源：http://do.asd995.cn

Go:   os.Getwd()
来源：http://fo.jianghongdianzi.cn

Ruby: Dir.pwd
来源：http://oh.newstarts.cn

C#:   Directory.GetCurrentDirectory()
来源：http://pr.9csxet.cn

[M05] 设置退出码
来源：http://fg.chemitech.net.cn

Py:   sys.exit(1)
来源：http://xi.nicolike.cn

PHP:  exit(1);
来源：http://bf.muxihuayi.cn

JS:   process.exit(1)
来源：http://ud.jianghongdianzi.cn

TS:   process.exit(1)
来源：http://fz.colortex.cn

Java: System.exit(1)
来源：http://am.muxihuayi.cn

Go:   os.Exit(1)
来源：http://kr.shtwfgs.cn

Ruby: exit 1
来源：http://pz.hahajie.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://fr.bjjhwx.cn

[M06] 向标准错误输出
来源：http://zm.chemitech.net.cn

Py:   print("err", file=sys.stderr)
来源：http://af.chemitech.net.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ic.521024.cn

JS:   console.error("err")
来源：http://fj.hnjuh.cn

TS:   console.error("err")
来源：http://wk.asd995.cn

Java: System.err.println("err")
来源：http://jr.huixiangedu.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://fm.panjiajie.cn

Ruby: warn "err"
来源：http://kh.huixiangedu.cn

C#:   Console.Error.WriteLine("err")
来源：http://ur.yuntaijiaju.cn

[M07] 判断是否为主入口
来源：http://wr.huixiangedu.cn

Py:   if __name__ == "__main__":
来源：http://cj.gzmigu.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://un.szxytkj.cn

JS:   require.main === module
来源：http://ay.jctech888.com.cn

TS:   require.main === module
来源：http://qa.muxihuayi.cn

Java: public static void main(String[] args)
来源：http://gg.9csxet.cn

Go:   func main()
来源：http://gk.bookmarksfly.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://jn.nszjky.cn

C#:   static void Main(string[] args)
来源：http://ia.asd995.cn

[M08] 获取系统与运行时信息
来源：http://zm.shtwfgs.cn

Py:   platform.system();  platform.python_version()
来源：http://lz.nicolike.cn

PHP:  PHP_OS;  phpversion();
来源：http://hl.521024.cn

JS:   process.platform;  process.version
来源：http://ov.shxzukj.cn

TS:   process.platform;  process.version
来源：http://vh.hahajie.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://qj.521024.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://qc.9csxet.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wc.muxihuayi.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://mw.jctech888.com.cn

================================================================================
来源：http://sd.lnxyls.cn

N. 数据结构与算法
来源：http://mn.colortex.cn

================================================================================
来源：http://ai.huixinmuqiang.cn

[N01] 二分查找（有序数组）
来源：http://op.shxzukj.cn

Py:   bisect.bisect_left(arr, x)
来源：http://bm.wgjwhj.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://px.bookmarksfly.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://su.wgjwhj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://on.9csxet.cn

Java: Arrays.binarySearch(arr, x)
来源：http://tz.bookmarksfly.cn

Go:   sort.SearchInts(arr, x)
来源：http://gt.yuexingan06.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://qi.szxytkj.cn

C#:   Array.BinarySearch(arr, x)
来源：http://eq.wgjwhj.cn

[N02] 排序（工程实践用内置实现）
来源：http://uh.huanxung.cn

Py:   sorted(arr);  arr.sort()
来源：http://ec.yuntaijiaju.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://xi.shxzukj.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ru.bjjhwx.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://or.huixiangedu.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://xk.gzmigu.cn

Go:   slices.Sort(arr)
来源：http://dd.asd995.cn

Ruby: arr.sort
来源：http://wt.jctech888.com.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://mn.huixinmuqiang.cn

[N03] 快速排序（分治示例）
来源：http://du.shxzukj.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://fd.colortex.cn


<!-- 参考信息 -->