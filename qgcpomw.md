代发 wailian999

Go:   time.Now().AddDate(0, 0, 7)
来源：http://oe.yuntaijiaju.cn

Ruby: Time.now + 7 * 86400
来源：http://mf.panjiajie.cn

C#:   DateTime.Now.AddDays(7)
来源：http://uw.521024.cn

[J06] 计算两时间之差
来源：http://wk.huanxung.cn

Py:   (end - start).total_seconds()
来源：http://rj.yuexingan06.cn

PHP:  $end->diff($start)->days;
来源：http://ku.9csxet.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hk.jctech888.com.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ll.panjiajie.cn

Java: Duration.between(start, end).toSeconds()
来源：http://gc.hahajie.cn

Go:   end.Sub(start).Hours()
来源：http://yt.hahajie.cn

Ruby: end - start                 # 返回秒数
来源：http://xl.newstarts.cn

C#:   (end - start).TotalSeconds
来源：http://aa.haigaiapp.cn

[J07] 比较两个日期
来源：http://ha.huixiangedu.cn

Py:   d1 < d2;  d1 == d2
来源：http://vy.szsharing.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://co.yuexingan06.cn

JS:   d1.getTime() < d2.getTime()
来源：http://kp.hnjuh.cn

TS:   d1.getTime() < d2.getTime()
来源：http://bi.panjiajie.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://no.nszjky.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://rh.asd995.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ty.chemitech.net.cn

C#:   d1 < d2;  d1 == d2
来源：http://hq.yuexingan06.cn

[J08] 提取年月日与星期
来源：http://qz.shtwfgs.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://gj.521024.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://cg.wgjwhj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://fq.yuexingan06.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://vk.hnjuh.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ch.hnjuh.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wv.shtwfgs.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://xp.jctech888.com.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://dj.wgjwhj.cn

[J09] 时区处理
来源：http://eo.hahajie.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://jd.asd995.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ra.panjiajie.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hq.chemitech.net.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vk.jianghongdianzi.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ha.9csxet.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wx.newstarts.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://dv.jianghongdianzi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://zk.nszjky.cn

[J10] 取今天 / 本月第一天
来源：http://iq.521024.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://vl.9csxet.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ui.hnjuh.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://es.nszjky.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://bj.hnjuh.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://om.chemitech.net.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://bz.521024.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://pv.jctech888.com.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://rj.newstarts.cn

================================================================================
来源：http://yc.huixinmuqiang.cn

K. JSON 与序列化
来源：http://ye.hahajie.cn

================================================================================
来源：http://mv.colortex.cn

[K01] 对象转 JSON 字符串
来源：http://mu.jianghongdianzi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://lr.chemitech.net.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://og.muxihuayi.cn

JS:   JSON.stringify(obj)
来源：http://it.bjjhwx.cn

TS:   JSON.stringify(obj)
来源：http://tc.nicolike.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://gm.haigaiapp.cn

Go:   json.Marshal(obj)
来源：http://dm.colortex.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ww.hahajie.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://fj.bookmarksfly.cn

[K02] JSON 字符串转对象
来源：http://mw.hahajie.cn

Py:   json.loads(s)
来源：http://ge.nicolike.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://bm.huixinmuqiang.cn

JS:   JSON.parse(s)
来源：http://cj.panjiajie.cn

TS:   JSON.parse(s)
来源：http://gc.hahajie.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ek.shtwfgs.cn

Go:   json.Unmarshal(data, &v)
来源：http://yl.lnxyls.cn

Ruby: JSON.parse(s)
来源：http://ec.colortex.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://nu.521024.cn

[K03] JSON 美化输出（带缩进）
来源：http://gt.chemitech.net.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hn.bjjhwx.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://nz.yuexingan06.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://js.nszjky.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://py.szsharing.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://fs.jianghongdianzi.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://nx.gzmigu.cn

Ruby: JSON.pretty_generate(obj)
来源：http://zb.szsharing.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://sh.hahajie.cn

[K04] 读取 JSON 文件
来源：http://ft.shxzskj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wn.huixiangedu.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://cs.panjiajie.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ug.newstarts.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wv.gzmigu.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://cv.shtwfgs.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://br.huanxung.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://sd.huixiangedu.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mt.bookmarksfly.cn

[K05] 深拷贝对象
来源：http://ub.chemitech.net.cn

Py:   copy.deepcopy(obj)
来源：http://oy.yuntaijiaju.cn

PHP:  unserialize(serialize($obj));
来源：http://wv.huanxung.cn

JS:   structuredClone(obj)
来源：http://kh.panjiajie.cn

TS:   structuredClone(obj)
来源：http://la.hahajie.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ur.jctech888.com.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://dm.521024.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://va.shxzukj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://xh.huixiangedu.cn

[K06] 解析 URL 查询串
来源：http://cm.bjjhwx.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://vc.gzmigu.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://vy.yuntaijiaju.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sx.asd995.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ez.muxihuayi.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://uq.bjjhwx.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://qd.shxzukj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://xf.huanxung.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://kl.9csxet.cn

[K07] 进制转换
来源：http://rq.hahajie.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://nh.9csxet.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://px.szsharing.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ny.bjjhwx.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qp.521024.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://yo.bookmarksfly.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://sb.szxytkj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://jj.nicolike.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://dl.bookmarksfly.cn

[K08] 二进制序列化（非 JSON）
来源：http://fk.asd995.cn

Py:   pickle.dumps(obj)
来源：http://fj.nicolike.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://xb.shxzskj.cn

JS:   v8.serialize(obj)        // Node
来源：http://dn.hahajie.cn

TS:   v8.serialize(obj)        // Node
来源：http://ss.yuntaijiaju.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://as.nszjky.cn

Go:   encoding/gob
来源：http://jk.shxzukj.cn

Ruby: Marshal.dump(obj)
来源：http://id.wgjwhj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://lu.szsharing.cn

================================================================================
来源：http://mw.wgjwhj.cn

L. 网络请求
来源：http://db.hahajie.cn

================================================================================
来源：http://yk.shxzukj.cn

[L01] 发送 GET 请求
来源：http://uq.shxzskj.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://fk.nszjky.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://rs.9csxet.cn

JS:   await fetch(url)
来源：http://da.panjiajie.cn

TS:   await fetch(url)
来源：http://qp.colortex.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://fl.nszjky.cn

Go:   resp, err := http.Get(url)
来源：http://bc.shxzukj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://vo.shxzskj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wx.panjiajie.cn

[L02] 发送 POST JSON
来源：http://pe.lnxyls.cn

Py:   requests.post(url, json={"a": 1})
来源：http://de.shtwfgs.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://dn.shxzskj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dl.shxzukj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ta.szxytkj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://zv.521024.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://vq.muxihuayi.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ek.yuntaijiaju.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://cj.shxzukj.cn

[L03] 设置自定义请求头
来源：http://lg.521024.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://qq.hnjuh.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ys.hahajie.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jb.521024.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://me.colortex.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ge.shtwfgs.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://zc.newstarts.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://zu.chemitech.net.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jv.bookmarksfly.cn

[L04] 设置超时
来源：http://up.shxzukj.cn

Py:   requests.get(url, timeout=5)
来源：http://tw.wgjwhj.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xe.nszjky.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://df.muxihuayi.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dd.lnxyls.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wr.hnjuh.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://lq.bookmarksfly.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://kt.wgjwhj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://nm.panjiajie.cn

[L05] 上传文件（multipart）
来源：http://ue.wgjwhj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ou.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://rh.shtwfgs.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://pq.nicolike.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ng.nszjky.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vv.haigaiapp.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://fz.lnxyls.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ql.nszjky.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://na.jctech888.com.cn

[L06] 解析响应为 JSON
来源：http://ls.hahajie.cn

Py:   resp.json()
来源：http://vq.gzmigu.cn

PHP:  json_decode($body, true);
来源：http://vv.huanxung.cn

JS:   await resp.json()
来源：http://vr.panjiajie.cn

TS:   await resp.json()
来源：http://cu.muxihuayi.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ht.nicolike.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://pv.hahajie.cn

Ruby: JSON.parse(resp.body)
来源：http://er.huixiangedu.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://sj.muxihuayi.cn

[L07] 处理 HTTP 状态码
来源：http://ab.muxihuayi.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://pg.haigaiapp.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://sz.huixiangedu.cn

JS:   resp.ok;  resp.status
来源：http://mq.lnxyls.cn

TS:   resp.ok;  resp.status
来源：http://wz.wgjwhj.cn

Java: resp.statusCode()
来源：http://sv.shxzskj.cn

Go:   resp.StatusCode
来源：http://fm.asd995.cn

Ruby: resp.code.to_i
来源：http://gr.bookmarksfly.cn

C#:   (int)resp.StatusCode
来源：http://bm.chemitech.net.cn

[L08] 并发请求多个地址
来源：http://lu.jctech888.com.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://bh.hahajie.cn

PHP:  curl_multi_init() 系列
来源：http://pj.szsharing.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ll.hahajie.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mx.asd995.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://zo.lnxyls.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://bi.colortex.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://rh.jctech888.com.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://fv.asd995.cn

================================================================================
来源：http://ta.bookmarksfly.cn

M. 命令行 / 进程 / 环境
来源：http://fd.bookmarksfly.cn

================================================================================
来源：http://hd.shxzskj.cn

[M01] 读取命令行参数
来源：http://lp.9csxet.cn

Py:   sys.argv[1:]
来源：http://bm.shxzskj.cn

PHP:  $argv;  $argc;
来源：http://ec.521024.cn

JS:   process.argv.slice(2)
来源：http://sr.yuntaijiaju.cn

TS:   process.argv.slice(2)
来源：http://yr.bjjhwx.cn

Java: args 数组（main 方法参数）
来源：http://tt.huixiangedu.cn

Go:   os.Args[1:]
来源：http://kj.szxytkj.cn

Ruby: ARGV
来源：http://ca.hnjuh.cn

C#:   args 数组（Main 方法参数）
来源：http://tg.nszjky.cn

[M02] 读取环境变量
来源：http://uf.yuntaijiaju.cn

Py:   os.environ.get("HOME")
来源：http://tr.jianghongdianzi.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://kr.lnxyls.cn

JS:   process.env.HOME
来源：http://lx.bjjhwx.cn

TS:   process.env.HOME
来源：http://qh.huixiangedu.cn

Java: System.getenv("HOME")
来源：http://ia.jianghongdianzi.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vt.hahajie.cn

Ruby: ENV["HOME"]
来源：http://kt.wgjwhj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://rj.huixinmuqiang.cn

[M03] 执行外部命令
来源：http://vw.muxihuayi.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://yt.gzmigu.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://qv.huixinmuqiang.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://wl.shxzukj.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ly.yuexingan06.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://lz.shxzukj.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://th.haigaiapp.cn

Ruby: system("ls -l");  `ls -l`
来源：http://pj.muxihuayi.cn

C#:   Process.Start("ls", "-l");
来源：http://fj.szsharing.cn

[M04] 获取当前工作目录
来源：http://dy.newstarts.cn

Py:   os.getcwd()
来源：http://lj.shxzskj.cn

PHP:  getcwd();
来源：http://ec.huanxung.cn

JS:   process.cwd()
来源：http://kv.szsharing.cn

TS:   process.cwd()
来源：http://sh.huixinmuqiang.cn

Java: Path.of("").toAbsolutePath()
来源：http://be.szsharing.cn

Go:   os.Getwd()
来源：http://gy.asd995.cn

Ruby: Dir.pwd
来源：http://ku.szxytkj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://hk.huixiangedu.cn

[M05] 设置退出码
来源：http://zb.huanxung.cn

Py:   sys.exit(1)
来源：http://uk.shxzskj.cn

PHP:  exit(1);
来源：http://xx.huixinmuqiang.cn

JS:   process.exit(1)
来源：http://vp.szsharing.cn

TS:   process.exit(1)
来源：http://xm.nicolike.cn

Java: System.exit(1)
来源：http://gv.jianghongdianzi.cn

Go:   os.Exit(1)
来源：http://ax.bookmarksfly.cn

Ruby: exit 1
来源：http://yk.szxytkj.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://rs.bookmarksfly.cn

[M06] 向标准错误输出
来源：http://oa.jctech888.com.cn

Py:   print("err", file=sys.stderr)
来源：http://ur.asd995.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://uh.hnjuh.cn

JS:   console.error("err")
来源：http://di.hnjuh.cn

TS:   console.error("err")
来源：http://qk.szsharing.cn

Java: System.err.println("err")
来源：http://ri.shxzukj.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://tk.wgjwhj.cn

Ruby: warn "err"
来源：http://wz.panjiajie.cn

C#:   Console.Error.WriteLine("err")
来源：http://ft.panjiajie.cn

[M07] 判断是否为主入口
来源：http://gz.shtwfgs.cn

Py:   if __name__ == "__main__":
来源：http://ys.gzmigu.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://lv.colortex.cn

JS:   require.main === module
来源：http://nx.shtwfgs.cn

TS:   require.main === module
来源：http://be.chemitech.net.cn

Java: public static void main(String[] args)
来源：http://kp.yuexingan06.cn

Go:   func main()
来源：http://yz.colortex.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ru.shtwfgs.cn

C#:   static void Main(string[] args)
来源：http://sl.shxzskj.cn

[M08] 获取系统与运行时信息
来源：http://hh.chemitech.net.cn

Py:   platform.system();  platform.python_version()
来源：http://wm.muxihuayi.cn

PHP:  PHP_OS;  phpversion();
来源：http://qa.newstarts.cn

JS:   process.platform;  process.version
来源：http://tu.bookmarksfly.cn

TS:   process.platform;  process.version
来源：http://sw.asd995.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://gt.huixinmuqiang.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ut.haigaiapp.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ps.haigaiapp.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://yk.hahajie.cn

================================================================================
来源：http://je.jianghongdianzi.cn

N. 数据结构与算法
来源：http://fh.haigaiapp.cn

================================================================================
来源：http://qh.hahajie.cn

[N01] 二分查找（有序数组）
来源：http://hv.huixiangedu.cn

Py:   bisect.bisect_left(arr, x)
来源：http://xd.hnjuh.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://dv.jctech888.com.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zg.huixinmuqiang.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zg.muxihuayi.cn

Java: Arrays.binarySearch(arr, x)
来源：http://jv.huixinmuqiang.cn

Go:   sort.SearchInts(arr, x)
来源：http://uv.chemitech.net.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://mp.jctech888.com.cn

C#:   Array.BinarySearch(arr, x)
来源：http://pa.panjiajie.cn

[N02] 排序（工程实践用内置实现）
来源：http://sf.9csxet.cn

Py:   sorted(arr);  arr.sort()
来源：http://dt.colortex.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://rz.9csxet.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://rq.shxzskj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://yq.hahajie.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://cn.lnxyls.cn

Go:   slices.Sort(arr)
来源：http://yl.colortex.cn

Ruby: arr.sort
来源：http://mo.bjjhwx.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://kg.521024.cn

[N03] 快速排序（分治示例）
来源：http://pr.shxzukj.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://tt.gzmigu.cn

PHP:  // 递归实现，或用 usort
来源：http://on.wgjwhj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ns.huixinmuqiang.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ml.szxytkj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://um.yuntaijiaju.cn


<!-- 参考信息 -->