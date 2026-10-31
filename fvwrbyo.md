代发 wailian999

PHP:  (new DateTime())->modify("+7 days");
来源：http://lq.haigaiapp.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://vp.nszjky.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hp.shxzukj.cn

Java: LocalDate.now().plusDays(7)
来源：http://ap.shtwfgs.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ks.9csxet.cn

Ruby: Time.now + 7 * 86400
来源：http://lc.muxihuayi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://jn.huixiangedu.cn

[J06] 计算两时间之差
来源：http://lc.9csxet.cn

Py:   (end - start).total_seconds()
来源：http://fn.szxytkj.cn

PHP:  $end->diff($start)->days;
来源：http://vi.nszjky.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://vc.szsharing.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ef.shxzukj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://lp.szsharing.cn

Go:   end.Sub(start).Hours()
来源：http://yc.muxihuayi.cn

Ruby: end - start                 # 返回秒数
来源：http://bj.hahajie.cn

C#:   (end - start).TotalSeconds
来源：http://yd.muxihuayi.cn

[J07] 比较两个日期
来源：http://ux.newstarts.cn

Py:   d1 < d2;  d1 == d2
来源：http://ym.yuntaijiaju.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ol.muxihuayi.cn

JS:   d1.getTime() < d2.getTime()
来源：http://xg.lnxyls.cn

TS:   d1.getTime() < d2.getTime()
来源：http://gt.jianghongdianzi.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://id.muxihuayi.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://da.9csxet.cn

Ruby: d1 < d2;  d1 == d2
来源：http://au.bjjhwx.cn

C#:   d1 < d2;  d1 == d2
来源：http://jb.521024.cn

[J08] 提取年月日与星期
来源：http://ry.bjjhwx.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://rs.chemitech.net.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://sq.bookmarksfly.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://rx.jctech888.com.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xb.huixinmuqiang.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ik.gzmigu.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://tv.yuntaijiaju.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zj.yuntaijiaju.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hh.hahajie.cn

[J09] 时区处理
来源：http://pf.szsharing.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ny.szsharing.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://zg.hahajie.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lc.haigaiapp.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ti.gzmigu.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bd.chemitech.net.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://id.muxihuayi.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ld.yuntaijiaju.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://gu.bjjhwx.cn

[J10] 取今天 / 本月第一天
来源：http://wk.hahajie.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ih.huanxung.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://uq.bookmarksfly.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://tu.jianghongdianzi.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://xf.yuexingan06.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xi.panjiajie.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://sm.shxzskj.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://pe.hahajie.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://gn.huixiangedu.cn

================================================================================
来源：http://xr.muxihuayi.cn

K. JSON 与序列化
来源：http://zm.yuexingan06.cn

================================================================================
来源：http://dl.szsharing.cn

[K01] 对象转 JSON 字符串
来源：http://tw.nszjky.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://lw.shtwfgs.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://tu.szxytkj.cn

JS:   JSON.stringify(obj)
来源：http://hr.bjjhwx.cn

TS:   JSON.stringify(obj)
来源：http://wb.bjjhwx.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://xp.yuntaijiaju.cn

Go:   json.Marshal(obj)
来源：http://qn.shxzukj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://hc.huixiangedu.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ox.newstarts.cn

[K02] JSON 字符串转对象
来源：http://qh.haigaiapp.cn

Py:   json.loads(s)
来源：http://pz.nicolike.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://tk.shxzskj.cn

JS:   JSON.parse(s)
来源：http://ll.bookmarksfly.cn

TS:   JSON.parse(s)
来源：http://xy.shxzukj.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://gs.hnjuh.cn

Go:   json.Unmarshal(data, &v)
来源：http://jg.huanxung.cn

Ruby: JSON.parse(s)
来源：http://bn.muxihuayi.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ge.szxytkj.cn

[K03] JSON 美化输出（带缩进）
来源：http://ee.asd995.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ml.hahajie.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://uc.gzmigu.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://nx.newstarts.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://rh.huanxung.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://aa.yuntaijiaju.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ix.shxzukj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ej.haigaiapp.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://pu.jianghongdianzi.cn

[K04] 读取 JSON 文件
来源：http://jz.colortex.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://oh.muxihuayi.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://vq.hahajie.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bn.muxihuayi.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ra.nszjky.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://yr.jctech888.com.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ky.shxzukj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ms.haigaiapp.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jb.szxytkj.cn

[K05] 深拷贝对象
来源：http://ep.jianghongdianzi.cn

Py:   copy.deepcopy(obj)
来源：http://nh.gzmigu.cn

PHP:  unserialize(serialize($obj));
来源：http://ll.gzmigu.cn

JS:   structuredClone(obj)
来源：http://ns.jctech888.com.cn

TS:   structuredClone(obj)
来源：http://ot.bookmarksfly.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ae.gzmigu.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ci.chemitech.net.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://me.bjjhwx.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ay.bookmarksfly.cn

[K06] 解析 URL 查询串
来源：http://lg.yuntaijiaju.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://sx.jctech888.com.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wz.521024.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://he.szxytkj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mp.bookmarksfly.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://sa.panjiajie.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ta.colortex.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://eb.bjjhwx.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://js.bjjhwx.cn

[K07] 进制转换
来源：http://ni.yuntaijiaju.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ag.hahajie.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://io.yuexingan06.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ue.huixiangedu.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ya.shxzskj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://gd.hnjuh.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://kq.gzmigu.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://od.nszjky.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hq.wgjwhj.cn

[K08] 二进制序列化（非 JSON）
来源：http://tf.huixiangedu.cn

Py:   pickle.dumps(obj)
来源：http://uw.521024.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://pb.gzmigu.cn

JS:   v8.serialize(obj)        // Node
来源：http://lv.szxytkj.cn

TS:   v8.serialize(obj)        // Node
来源：http://tn.nicolike.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://eh.shxzskj.cn

Go:   encoding/gob
来源：http://rg.gzmigu.cn

Ruby: Marshal.dump(obj)
来源：http://lq.wgjwhj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://il.gzmigu.cn

================================================================================
来源：http://bw.jianghongdianzi.cn

L. 网络请求
来源：http://vt.nszjky.cn

================================================================================
来源：http://om.yuntaijiaju.cn

[L01] 发送 GET 请求
来源：http://cw.muxihuayi.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://bo.colortex.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://pl.huixiangedu.cn

JS:   await fetch(url)
来源：http://nt.lnxyls.cn

TS:   await fetch(url)
来源：http://nd.521024.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://bv.szsharing.cn

Go:   resp, err := http.Get(url)
来源：http://ko.gzmigu.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://us.521024.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://kr.nicolike.cn

[L02] 发送 POST JSON
来源：http://gg.huixinmuqiang.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ih.wgjwhj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://yy.gzmigu.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gj.asd995.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bj.hnjuh.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://sv.huixinmuqiang.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ok.huixiangedu.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://bv.szsharing.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://lm.panjiajie.cn

[L03] 设置自定义请求头
来源：http://oo.nszjky.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://za.huixiangedu.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://av.wgjwhj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bk.chemitech.net.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hh.521024.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://fd.newstarts.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://sk.wgjwhj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://sk.gzmigu.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://nc.hnjuh.cn

[L04] 设置超时
来源：http://zg.newstarts.cn

Py:   requests.get(url, timeout=5)
来源：http://zk.szsharing.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://op.yuexingan06.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xk.hahajie.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ps.chemitech.net.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hy.bjjhwx.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://qb.huixinmuqiang.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mj.shxzukj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://cg.huanxung.cn

[L05] 上传文件（multipart）
来源：http://eo.shtwfgs.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://eu.521024.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://zr.jctech888.com.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mj.9csxet.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xt.yuntaijiaju.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://gw.yuexingan06.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://gm.wgjwhj.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://jj.9csxet.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://so.huixiangedu.cn

[L06] 解析响应为 JSON
来源：http://qz.521024.cn

Py:   resp.json()
来源：http://pd.yuntaijiaju.cn

PHP:  json_decode($body, true);
来源：http://sp.shxzskj.cn

JS:   await resp.json()
来源：http://di.huanxung.cn

TS:   await resp.json()
来源：http://nw.haigaiapp.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ey.yuntaijiaju.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wq.9csxet.cn

Ruby: JSON.parse(resp.body)
来源：http://br.wgjwhj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wo.muxihuayi.cn

[L07] 处理 HTTP 状态码
来源：http://yw.panjiajie.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ab.asd995.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://md.shxzukj.cn

JS:   resp.ok;  resp.status
来源：http://hw.jctech888.com.cn

TS:   resp.ok;  resp.status
来源：http://vs.huixinmuqiang.cn

Java: resp.statusCode()
来源：http://qq.gzmigu.cn

Go:   resp.StatusCode
来源：http://ce.521024.cn

Ruby: resp.code.to_i
来源：http://yt.szsharing.cn

C#:   (int)resp.StatusCode
来源：http://yq.shxzskj.cn

[L08] 并发请求多个地址
来源：http://ro.521024.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://lh.lnxyls.cn

PHP:  curl_multi_init() 系列
来源：http://kx.shxzskj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ir.huixiangedu.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zp.yuexingan06.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://vq.szsharing.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ju.shtwfgs.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://bz.bjjhwx.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://gk.chemitech.net.cn

================================================================================
来源：http://oq.521024.cn

M. 命令行 / 进程 / 环境
来源：http://yn.huixinmuqiang.cn

================================================================================
来源：http://cm.shtwfgs.cn

[M01] 读取命令行参数
来源：http://yq.newstarts.cn

Py:   sys.argv[1:]
来源：http://qu.521024.cn

PHP:  $argv;  $argc;
来源：http://cp.muxihuayi.cn

JS:   process.argv.slice(2)
来源：http://js.szxytkj.cn

TS:   process.argv.slice(2)
来源：http://ae.szxytkj.cn

Java: args 数组（main 方法参数）
来源：http://ku.nicolike.cn

Go:   os.Args[1:]
来源：http://ud.jctech888.com.cn

Ruby: ARGV
来源：http://rb.lnxyls.cn

C#:   args 数组（Main 方法参数）
来源：http://hv.yuntaijiaju.cn

[M02] 读取环境变量
来源：http://ao.nszjky.cn

Py:   os.environ.get("HOME")
来源：http://nx.shtwfgs.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ti.bjjhwx.cn

JS:   process.env.HOME
来源：http://sx.newstarts.cn

TS:   process.env.HOME
来源：http://ax.nicolike.cn

Java: System.getenv("HOME")
来源：http://wj.shxzukj.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://um.huixiangedu.cn

Ruby: ENV["HOME"]
来源：http://uw.haigaiapp.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://bb.panjiajie.cn

[M03] 执行外部命令
来源：http://dl.wgjwhj.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://rk.wgjwhj.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://rv.lnxyls.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://qh.haigaiapp.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://jj.gzmigu.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://of.hnjuh.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://yt.huanxung.cn

Ruby: system("ls -l");  `ls -l`
来源：http://yw.hahajie.cn

C#:   Process.Start("ls", "-l");
来源：http://tj.huixinmuqiang.cn

[M04] 获取当前工作目录
来源：http://jp.bjjhwx.cn

Py:   os.getcwd()
来源：http://jh.jctech888.com.cn

PHP:  getcwd();
来源：http://nd.wgjwhj.cn

JS:   process.cwd()
来源：http://xb.yuntaijiaju.cn

TS:   process.cwd()
来源：http://qd.jianghongdianzi.cn

Java: Path.of("").toAbsolutePath()
来源：http://dv.nszjky.cn

Go:   os.Getwd()
来源：http://mi.huixinmuqiang.cn

Ruby: Dir.pwd
来源：http://yz.asd995.cn

C#:   Directory.GetCurrentDirectory()
来源：http://kg.shtwfgs.cn

[M05] 设置退出码
来源：http://ka.521024.cn

Py:   sys.exit(1)
来源：http://jo.colortex.cn

PHP:  exit(1);
来源：http://mz.521024.cn

JS:   process.exit(1)
来源：http://ry.huixiangedu.cn

TS:   process.exit(1)
来源：http://sf.bookmarksfly.cn

Java: System.exit(1)
来源：http://zy.szsharing.cn

Go:   os.Exit(1)
来源：http://xt.nicolike.cn

Ruby: exit 1
来源：http://gq.gzmigu.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://vn.chemitech.net.cn

[M06] 向标准错误输出
来源：http://ui.nszjky.cn

Py:   print("err", file=sys.stderr)
来源：http://pe.9csxet.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://hm.szxytkj.cn

JS:   console.error("err")
来源：http://ki.521024.cn

TS:   console.error("err")
来源：http://gn.nicolike.cn

Java: System.err.println("err")
来源：http://va.9csxet.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ra.gzmigu.cn

Ruby: warn "err"
来源：http://jf.asd995.cn

C#:   Console.Error.WriteLine("err")
来源：http://ca.hahajie.cn

[M07] 判断是否为主入口
来源：http://bz.hnjuh.cn

Py:   if __name__ == "__main__":
来源：http://pi.bookmarksfly.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ru.wgjwhj.cn

JS:   require.main === module
来源：http://tg.szsharing.cn

TS:   require.main === module
来源：http://hd.jctech888.com.cn

Java: public static void main(String[] args)
来源：http://fn.shxzukj.cn

Go:   func main()
来源：http://ld.gzmigu.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://xg.jctech888.com.cn

C#:   static void Main(string[] args)
来源：http://fi.nicolike.cn

[M08] 获取系统与运行时信息
来源：http://uu.jianghongdianzi.cn

Py:   platform.system();  platform.python_version()
来源：http://tn.lnxyls.cn

PHP:  PHP_OS;  phpversion();
来源：http://pv.shtwfgs.cn

JS:   process.platform;  process.version
来源：http://hx.huixinmuqiang.cn

TS:   process.platform;  process.version
来源：http://eq.hnjuh.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://dj.shtwfgs.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://qp.lnxyls.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://my.521024.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://df.bjjhwx.cn

================================================================================
来源：http://df.hnjuh.cn

N. 数据结构与算法
来源：http://gc.521024.cn

================================================================================
来源：http://ip.huanxung.cn

[N01] 二分查找（有序数组）
来源：http://wy.nicolike.cn

Py:   bisect.bisect_left(arr, x)
来源：http://bn.shxzskj.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://jh.bookmarksfly.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jp.panjiajie.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yh.haigaiapp.cn

Java: Arrays.binarySearch(arr, x)
来源：http://zz.asd995.cn

Go:   sort.SearchInts(arr, x)
来源：http://xk.9csxet.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://mk.szxytkj.cn

C#:   Array.BinarySearch(arr, x)
来源：http://pf.gzmigu.cn

[N02] 排序（工程实践用内置实现）
来源：http://fr.haigaiapp.cn

Py:   sorted(arr);  arr.sort()
来源：http://xq.yuntaijiaju.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ev.nicolike.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://by.521024.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ol.huixinmuqiang.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://qw.szsharing.cn

Go:   slices.Sort(arr)
来源：http://tx.jianghongdianzi.cn

Ruby: arr.sort
来源：http://km.shtwfgs.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://bj.hahajie.cn

[N03] 快速排序（分治示例）
来源：http://ig.yuexingan06.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://po.yuntaijiaju.cn


<!-- 参考信息 -->