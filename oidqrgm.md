代发 wailian999

PHP:  (new DateTime())->modify("+7 days");
来源：http://zh.szsharing.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://bj.shxzskj.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://jb.lnxyls.cn

Java: LocalDate.now().plusDays(7)
来源：http://py.jianghongdianzi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://lo.lnxyls.cn

Ruby: Time.now + 7 * 86400
来源：http://dh.bookmarksfly.cn

C#:   DateTime.Now.AddDays(7)
来源：http://rw.huanxung.cn

[J06] 计算两时间之差
来源：http://zk.521024.cn

Py:   (end - start).total_seconds()
来源：http://nt.bjjhwx.cn

PHP:  $end->diff($start)->days;
来源：http://si.szxytkj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://bh.huixinmuqiang.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wc.chemitech.net.cn

Java: Duration.between(start, end).toSeconds()
来源：http://eo.jctech888.com.cn

Go:   end.Sub(start).Hours()
来源：http://rt.9csxet.cn

Ruby: end - start                 # 返回秒数
来源：http://em.colortex.cn

C#:   (end - start).TotalSeconds
来源：http://ld.521024.cn

[J07] 比较两个日期
来源：http://ya.shxzukj.cn

Py:   d1 < d2;  d1 == d2
来源：http://hr.muxihuayi.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://dj.colortex.cn

JS:   d1.getTime() < d2.getTime()
来源：http://fz.nicolike.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ub.yuntaijiaju.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://cf.newstarts.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://pe.9csxet.cn

Ruby: d1 < d2;  d1 == d2
来源：http://dm.shxzukj.cn

C#:   d1 < d2;  d1 == d2
来源：http://gm.jianghongdianzi.cn

[J08] 提取年月日与星期
来源：http://zd.newstarts.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mf.gzmigu.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://rs.asd995.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ek.jianghongdianzi.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://tc.shtwfgs.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://js.shxzskj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ef.9csxet.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://rk.asd995.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ij.nicolike.cn

[J09] 时区处理
来源：http://rs.chemitech.net.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hs.asd995.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://oa.bookmarksfly.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://el.hnjuh.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pj.nszjky.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bf.9csxet.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://cw.yuexingan06.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://bh.shxzukj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://pu.hahajie.cn

[J10] 取今天 / 本月第一天
来源：http://ds.nszjky.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://tk.shtwfgs.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://nt.lnxyls.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qx.haigaiapp.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://eh.bookmarksfly.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ax.asd995.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://st.lnxyls.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hf.asd995.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://rx.shxzukj.cn

================================================================================
来源：http://jm.szsharing.cn

K. JSON 与序列化
来源：http://cn.9csxet.cn

================================================================================
来源：http://st.jctech888.com.cn

[K01] 对象转 JSON 字符串
来源：http://hs.nicolike.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ya.panjiajie.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://fg.hahajie.cn

JS:   JSON.stringify(obj)
来源：http://tt.yuexingan06.cn

TS:   JSON.stringify(obj)
来源：http://mr.huanxung.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://dk.jianghongdianzi.cn

Go:   json.Marshal(obj)
来源：http://ch.gzmigu.cn

Ruby: obj.to_json                                     // require "json"
来源：http://xm.szxytkj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://uo.muxihuayi.cn

[K02] JSON 字符串转对象
来源：http://ew.bjjhwx.cn

Py:   json.loads(s)
来源：http://sp.jianghongdianzi.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ix.wgjwhj.cn

JS:   JSON.parse(s)
来源：http://ra.gzmigu.cn

TS:   JSON.parse(s)
来源：http://kt.hahajie.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://nu.shtwfgs.cn

Go:   json.Unmarshal(data, &v)
来源：http://mi.asd995.cn

Ruby: JSON.parse(s)
来源：http://ai.huixinmuqiang.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://jp.9csxet.cn

[K03] JSON 美化输出（带缩进）
来源：http://yb.hnjuh.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://kz.newstarts.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ie.jctech888.com.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ll.shtwfgs.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://qj.lnxyls.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hb.yuntaijiaju.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://rs.nszjky.cn

Ruby: JSON.pretty_generate(obj)
来源：http://rs.chemitech.net.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ly.nszjky.cn

[K04] 读取 JSON 文件
来源：http://bm.lnxyls.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://dd.colortex.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ba.shxzskj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bq.yuntaijiaju.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pq.bjjhwx.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://cq.yuntaijiaju.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ao.shtwfgs.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://wj.huanxung.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wc.jianghongdianzi.cn

[K05] 深拷贝对象
来源：http://ty.haigaiapp.cn

Py:   copy.deepcopy(obj)
来源：http://qg.bookmarksfly.cn

PHP:  unserialize(serialize($obj));
来源：http://dn.bookmarksfly.cn

JS:   structuredClone(obj)
来源：http://dl.shxzskj.cn

TS:   structuredClone(obj)
来源：http://at.chemitech.net.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://eh.yuntaijiaju.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://sw.nicolike.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wg.shxzskj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://vg.hahajie.cn

[K06] 解析 URL 查询串
来源：http://uu.521024.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://dl.chemitech.net.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mi.newstarts.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wj.chemitech.net.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gb.muxihuayi.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://md.hnjuh.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://gt.yuexingan06.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://pl.gzmigu.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ea.yuntaijiaju.cn

[K07] 进制转换
来源：http://jr.haigaiapp.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://kk.szxytkj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://uk.jianghongdianzi.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://db.yuexingan06.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://la.shxzskj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://lz.yuexingan06.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ru.huixiangedu.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://sb.szsharing.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://kr.9csxet.cn

[K08] 二进制序列化（非 JSON）
来源：http://my.shtwfgs.cn

Py:   pickle.dumps(obj)
来源：http://mz.bookmarksfly.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://wl.szsharing.cn

JS:   v8.serialize(obj)        // Node
来源：http://gz.jctech888.com.cn

TS:   v8.serialize(obj)        // Node
来源：http://vr.huixinmuqiang.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hg.szsharing.cn

Go:   encoding/gob
来源：http://lm.gzmigu.cn

Ruby: Marshal.dump(obj)
来源：http://gq.szsharing.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ti.haigaiapp.cn

================================================================================
来源：http://mv.huanxung.cn

L. 网络请求
来源：http://zv.9csxet.cn

================================================================================
来源：http://bm.yuexingan06.cn

[L01] 发送 GET 请求
来源：http://iw.huixinmuqiang.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://es.nszjky.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://kj.shxzskj.cn

JS:   await fetch(url)
来源：http://lu.szxytkj.cn

TS:   await fetch(url)
来源：http://el.panjiajie.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://oc.wgjwhj.cn

Go:   resp, err := http.Get(url)
来源：http://iw.9csxet.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ux.hahajie.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://yt.jianghongdianzi.cn

[L02] 发送 POST JSON
来源：http://mt.szxytkj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://lb.hnjuh.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://jj.huixinmuqiang.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xq.nszjky.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ye.bookmarksfly.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qd.bjjhwx.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://dp.yuexingan06.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ae.newstarts.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://fd.colortex.cn

[L03] 设置自定义请求头
来源：http://gb.bjjhwx.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://iq.yuntaijiaju.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mp.jctech888.com.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wq.9csxet.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yj.bjjhwx.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://bs.colortex.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://vd.wgjwhj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://xs.shxzukj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://eu.shxzskj.cn

[L04] 设置超时
来源：http://tj.huixiangedu.cn

Py:   requests.get(url, timeout=5)
来源：http://ee.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://co.nicolike.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://sj.yuexingan06.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pt.colortex.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://sl.huixiangedu.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://yg.shxzskj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://kz.jianghongdianzi.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://tu.huanxung.cn

[L05] 上传文件（multipart）
来源：http://bp.muxihuayi.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zs.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://rw.9csxet.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://tr.gzmigu.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://bf.chemitech.net.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://le.newstarts.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ah.hnjuh.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://nj.szsharing.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://nr.chemitech.net.cn

[L06] 解析响应为 JSON
来源：http://ej.colortex.cn

Py:   resp.json()
来源：http://si.wgjwhj.cn

PHP:  json_decode($body, true);
来源：http://oi.gzmigu.cn

JS:   await resp.json()
来源：http://qj.panjiajie.cn

TS:   await resp.json()
来源：http://gq.9csxet.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://tr.haigaiapp.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://pk.shxzskj.cn

Ruby: JSON.parse(resp.body)
来源：http://be.huanxung.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://st.jianghongdianzi.cn

[L07] 处理 HTTP 状态码
来源：http://wx.haigaiapp.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://vl.shxzukj.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://cs.gzmigu.cn

JS:   resp.ok;  resp.status
来源：http://vs.yuntaijiaju.cn

TS:   resp.ok;  resp.status
来源：http://nf.wgjwhj.cn

Java: resp.statusCode()
来源：http://zm.huixinmuqiang.cn

Go:   resp.StatusCode
来源：http://vi.asd995.cn

Ruby: resp.code.to_i
来源：http://vl.lnxyls.cn

C#:   (int)resp.StatusCode
来源：http://st.haigaiapp.cn

[L08] 并发请求多个地址
来源：http://cp.haigaiapp.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://bt.lnxyls.cn

PHP:  curl_multi_init() 系列
来源：http://np.bjjhwx.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://og.wgjwhj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fm.asd995.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wn.shtwfgs.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://py.shtwfgs.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ai.yuntaijiaju.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://sk.hnjuh.cn

================================================================================
来源：http://pc.9csxet.cn

M. 命令行 / 进程 / 环境
来源：http://sj.shxzukj.cn

================================================================================
来源：http://uw.nicolike.cn

[M01] 读取命令行参数
来源：http://zb.lnxyls.cn

Py:   sys.argv[1:]
来源：http://yx.chemitech.net.cn

PHP:  $argv;  $argc;
来源：http://di.wgjwhj.cn

JS:   process.argv.slice(2)
来源：http://tf.shtwfgs.cn

TS:   process.argv.slice(2)
来源：http://pi.huanxung.cn

Java: args 数组（main 方法参数）
来源：http://jl.bookmarksfly.cn

Go:   os.Args[1:]
来源：http://gv.haigaiapp.cn

Ruby: ARGV
来源：http://ej.shxzukj.cn

C#:   args 数组（Main 方法参数）
来源：http://pj.nicolike.cn

[M02] 读取环境变量
来源：http://oz.nicolike.cn

Py:   os.environ.get("HOME")
来源：http://pf.jctech888.com.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://vd.jctech888.com.cn

JS:   process.env.HOME
来源：http://am.szxytkj.cn

TS:   process.env.HOME
来源：http://wk.nicolike.cn

Java: System.getenv("HOME")
来源：http://kj.asd995.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://kc.yuexingan06.cn

Ruby: ENV["HOME"]
来源：http://ay.wgjwhj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://yh.yuntaijiaju.cn

[M03] 执行外部命令
来源：http://wd.newstarts.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://rb.nicolike.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://lj.hnjuh.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://an.muxihuayi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://kt.szsharing.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://nh.521024.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://kt.yuexingan06.cn

Ruby: system("ls -l");  `ls -l`
来源：http://pu.jctech888.com.cn

C#:   Process.Start("ls", "-l");
来源：http://ss.hahajie.cn

[M04] 获取当前工作目录
来源：http://fv.hnjuh.cn

Py:   os.getcwd()
来源：http://rx.huixiangedu.cn

PHP:  getcwd();
来源：http://cs.9csxet.cn

JS:   process.cwd()
来源：http://es.hnjuh.cn

TS:   process.cwd()
来源：http://tv.hnjuh.cn

Java: Path.of("").toAbsolutePath()
来源：http://ww.bookmarksfly.cn

Go:   os.Getwd()
来源：http://ci.huanxung.cn

Ruby: Dir.pwd
来源：http://hg.nicolike.cn

C#:   Directory.GetCurrentDirectory()
来源：http://wb.huixinmuqiang.cn

[M05] 设置退出码
来源：http://dg.shxzskj.cn

Py:   sys.exit(1)
来源：http://nr.shxzukj.cn

PHP:  exit(1);
来源：http://ls.huixinmuqiang.cn

JS:   process.exit(1)
来源：http://ci.9csxet.cn

TS:   process.exit(1)
来源：http://ts.yuntaijiaju.cn

Java: System.exit(1)
来源：http://iw.szsharing.cn

Go:   os.Exit(1)
来源：http://kg.jianghongdianzi.cn

Ruby: exit 1
来源：http://my.jianghongdianzi.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ct.chemitech.net.cn

[M06] 向标准错误输出
来源：http://kw.huanxung.cn

Py:   print("err", file=sys.stderr)
来源：http://al.shtwfgs.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://gm.muxihuayi.cn

JS:   console.error("err")
来源：http://qn.9csxet.cn

TS:   console.error("err")
来源：http://ax.shxzskj.cn

Java: System.err.println("err")
来源：http://yn.nicolike.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://oa.haigaiapp.cn

Ruby: warn "err"
来源：http://em.szxytkj.cn

C#:   Console.Error.WriteLine("err")
来源：http://gx.muxihuayi.cn

[M07] 判断是否为主入口
来源：http://cd.9csxet.cn

Py:   if __name__ == "__main__":
来源：http://ao.huixiangedu.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://pa.newstarts.cn

JS:   require.main === module
来源：http://co.haigaiapp.cn

TS:   require.main === module
来源：http://ux.muxihuayi.cn

Java: public static void main(String[] args)
来源：http://aj.shtwfgs.cn

Go:   func main()
来源：http://fn.521024.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ru.wgjwhj.cn

C#:   static void Main(string[] args)
来源：http://fv.yuntaijiaju.cn

[M08] 获取系统与运行时信息
来源：http://uu.hahajie.cn

Py:   platform.system();  platform.python_version()
来源：http://vg.521024.cn

PHP:  PHP_OS;  phpversion();
来源：http://bf.asd995.cn

JS:   process.platform;  process.version
来源：http://ef.nicolike.cn

TS:   process.platform;  process.version
来源：http://lx.huanxung.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://uk.haigaiapp.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://np.panjiajie.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://qt.shxzukj.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://tb.bjjhwx.cn

================================================================================
来源：http://zk.hnjuh.cn

N. 数据结构与算法
来源：http://so.huixinmuqiang.cn

================================================================================
来源：http://hb.yuexingan06.cn

[N01] 二分查找（有序数组）
来源：http://bn.hahajie.cn

Py:   bisect.bisect_left(arr, x)
来源：http://qu.wgjwhj.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://eq.lnxyls.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tz.yuexingan06.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qz.shxzukj.cn

Java: Arrays.binarySearch(arr, x)
来源：http://nq.szsharing.cn

Go:   sort.SearchInts(arr, x)
来源：http://qi.hnjuh.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://pb.haigaiapp.cn

C#:   Array.BinarySearch(arr, x)
来源：http://nn.gzmigu.cn

[N02] 排序（工程实践用内置实现）
来源：http://el.9csxet.cn

Py:   sorted(arr);  arr.sort()
来源：http://ty.lnxyls.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://lp.jctech888.com.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://cf.shxzskj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://mw.wgjwhj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://az.szsharing.cn

Go:   slices.Sort(arr)
来源：http://iw.haigaiapp.cn

Ruby: arr.sort
来源：http://hb.muxihuayi.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://fg.huanxung.cn

[N03] 快速排序（分治示例）
来源：http://dr.huixinmuqiang.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hb.colortex.cn


<!-- 参考信息 -->