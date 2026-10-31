代发 wailian999

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://uo.shtwfgs.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://yp.newstarts.cn

[J05] 时间加减（加 7 天）
来源：http://pm.asd995.cn

Py:   now + timedelta(days=7)
来源：http://ok.gzmigu.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://sm.yuexingan06.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://pz.colortex.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://yp.colortex.cn

Java: LocalDate.now().plusDays(7)
来源：http://zl.521024.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ga.lnxyls.cn

Ruby: Time.now + 7 * 86400
来源：http://zr.colortex.cn

C#:   DateTime.Now.AddDays(7)
来源：http://yk.huixinmuqiang.cn

[J06] 计算两时间之差
来源：http://vg.asd995.cn

Py:   (end - start).total_seconds()
来源：http://fo.szxytkj.cn

PHP:  $end->diff($start)->days;
来源：http://gf.newstarts.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://xm.newstarts.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ch.newstarts.cn

Java: Duration.between(start, end).toSeconds()
来源：http://qh.chemitech.net.cn

Go:   end.Sub(start).Hours()
来源：http://xp.szxytkj.cn

Ruby: end - start                 # 返回秒数
来源：http://ti.nszjky.cn

C#:   (end - start).TotalSeconds
来源：http://aq.newstarts.cn

[J07] 比较两个日期
来源：http://oa.huixinmuqiang.cn

Py:   d1 < d2;  d1 == d2
来源：http://za.nicolike.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://fx.chemitech.net.cn

JS:   d1.getTime() < d2.getTime()
来源：http://de.yuntaijiaju.cn

TS:   d1.getTime() < d2.getTime()
来源：http://th.huixinmuqiang.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://kk.bjjhwx.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://yk.hahajie.cn

Ruby: d1 < d2;  d1 == d2
来源：http://py.shtwfgs.cn

C#:   d1 < d2;  d1 == d2
来源：http://sc.hahajie.cn

[J08] 提取年月日与星期
来源：http://fq.hnjuh.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ep.haigaiapp.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://gt.yuntaijiaju.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ef.huanxung.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ia.muxihuayi.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://lh.szxytkj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://jf.jctech888.com.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://uh.bjjhwx.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://aa.nszjky.cn

[J09] 时区处理
来源：http://xt.lnxyls.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qq.wgjwhj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://cw.nicolike.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mm.lnxyls.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ny.colortex.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mz.bookmarksfly.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://yi.szxytkj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://bz.gzmigu.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qu.bookmarksfly.cn

[J10] 取今天 / 本月第一天
来源：http://bz.szsharing.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ve.muxihuayi.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://lb.muxihuayi.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ge.szsharing.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://dy.gzmigu.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ax.szsharing.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://qk.huixinmuqiang.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://rt.szsharing.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://up.jctech888.com.cn

================================================================================
来源：http://it.521024.cn

K. JSON 与序列化
来源：http://pj.jianghongdianzi.cn

================================================================================
来源：http://vq.yuexingan06.cn

[K01] 对象转 JSON 字符串
来源：http://cm.huixiangedu.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ty.521024.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://qu.bjjhwx.cn

JS:   JSON.stringify(obj)
来源：http://pe.shtwfgs.cn

TS:   JSON.stringify(obj)
来源：http://tp.szsharing.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hw.bjjhwx.cn

Go:   json.Marshal(obj)
来源：http://vi.huanxung.cn

Ruby: obj.to_json                                     // require "json"
来源：http://gk.wgjwhj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://uo.jctech888.com.cn

[K02] JSON 字符串转对象
来源：http://ga.jctech888.com.cn

Py:   json.loads(s)
来源：http://zm.panjiajie.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ko.colortex.cn

JS:   JSON.parse(s)
来源：http://pr.wgjwhj.cn

TS:   JSON.parse(s)
来源：http://kz.muxihuayi.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://af.newstarts.cn

Go:   json.Unmarshal(data, &v)
来源：http://wo.shtwfgs.cn

Ruby: JSON.parse(s)
来源：http://kw.hahajie.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://gw.hahajie.cn

[K03] JSON 美化输出（带缩进）
来源：http://hv.huanxung.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://aj.asd995.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wz.yuexingan06.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://qf.panjiajie.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://cv.nicolike.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qi.shtwfgs.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://me.bookmarksfly.cn

Ruby: JSON.pretty_generate(obj)
来源：http://fr.bookmarksfly.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://bc.bookmarksfly.cn

[K04] 读取 JSON 文件
来源：http://du.huanxung.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://bo.bjjhwx.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://qe.gzmigu.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nd.521024.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ez.lnxyls.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vr.huixiangedu.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://tg.hnjuh.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://rl.haigaiapp.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://bv.chemitech.net.cn

[K05] 深拷贝对象
来源：http://dz.hahajie.cn

Py:   copy.deepcopy(obj)
来源：http://sa.shxzukj.cn

PHP:  unserialize(serialize($obj));
来源：http://tg.bjjhwx.cn

JS:   structuredClone(obj)
来源：http://ki.bjjhwx.cn

TS:   structuredClone(obj)
来源：http://xb.newstarts.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://uh.szxytkj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zp.hnjuh.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://oy.lnxyls.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://jt.newstarts.cn

[K06] 解析 URL 查询串
来源：http://tg.yuntaijiaju.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mz.nszjky.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://uh.bjjhwx.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xt.huixinmuqiang.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vx.9csxet.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ms.bjjhwx.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://fp.panjiajie.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://om.chemitech.net.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://sw.lnxyls.cn

[K07] 进制转换
来源：http://rp.szsharing.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://zj.nszjky.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://pc.chemitech.net.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hr.shxzskj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://dk.hnjuh.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ws.jianghongdianzi.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://md.colortex.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://bm.chemitech.net.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://rf.jianghongdianzi.cn

[K08] 二进制序列化（非 JSON）
来源：http://fz.hnjuh.cn

Py:   pickle.dumps(obj)
来源：http://ux.shxzukj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://av.yuntaijiaju.cn

JS:   v8.serialize(obj)        // Node
来源：http://kh.szxytkj.cn

TS:   v8.serialize(obj)        // Node
来源：http://gf.shxzukj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wq.nicolike.cn

Go:   encoding/gob
来源：http://jo.colortex.cn

Ruby: Marshal.dump(obj)
来源：http://jh.szsharing.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://rp.panjiajie.cn

================================================================================
来源：http://oj.521024.cn

L. 网络请求
来源：http://ql.lnxyls.cn

================================================================================
来源：http://ud.shtwfgs.cn

[L01] 发送 GET 请求
来源：http://an.colortex.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ng.hahajie.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hx.yuexingan06.cn

JS:   await fetch(url)
来源：http://jk.muxihuayi.cn

TS:   await fetch(url)
来源：http://fp.lnxyls.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wi.colortex.cn

Go:   resp, err := http.Get(url)
来源：http://wt.newstarts.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ud.hnjuh.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://cu.szsharing.cn

[L02] 发送 POST JSON
来源：http://zl.wgjwhj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ek.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://iw.jctech888.com.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sa.9csxet.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rg.huixiangedu.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://kc.shxzskj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://vm.wgjwhj.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://bp.panjiajie.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://cz.9csxet.cn

[L03] 设置自定义请求头
来源：http://hs.szxytkj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wj.huixiangedu.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://yt.shxzskj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gp.huanxung.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zw.shxzukj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://fa.newstarts.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://xl.bookmarksfly.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ub.jianghongdianzi.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ua.shxzukj.cn

[L04] 设置超时
来源：http://ue.shtwfgs.cn

Py:   requests.get(url, timeout=5)
来源：http://uj.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://op.asd995.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zg.hahajie.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lt.gzmigu.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hn.muxihuayi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://an.huixinmuqiang.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ty.shxzskj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wk.bookmarksfly.cn

[L05] 上传文件（multipart）
来源：http://fz.bjjhwx.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hu.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://tm.521024.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qn.szsharing.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://eh.shtwfgs.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wm.521024.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ck.521024.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vh.huixinmuqiang.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mm.huixiangedu.cn

[L06] 解析响应为 JSON
来源：http://pw.panjiajie.cn

Py:   resp.json()
来源：http://sy.bjjhwx.cn

PHP:  json_decode($body, true);
来源：http://oo.521024.cn

JS:   await resp.json()
来源：http://uu.bjjhwx.cn

TS:   await resp.json()
来源：http://ay.hahajie.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ey.nicolike.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://nx.hahajie.cn

Ruby: JSON.parse(resp.body)
来源：http://mm.521024.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://bl.shtwfgs.cn

[L07] 处理 HTTP 状态码
来源：http://gh.panjiajie.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://fc.lnxyls.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://aq.colortex.cn

JS:   resp.ok;  resp.status
来源：http://ke.asd995.cn

TS:   resp.ok;  resp.status
来源：http://df.szxytkj.cn

Java: resp.statusCode()
来源：http://pu.huixiangedu.cn

Go:   resp.StatusCode
来源：http://je.muxihuayi.cn

Ruby: resp.code.to_i
来源：http://ok.bjjhwx.cn

C#:   (int)resp.StatusCode
来源：http://ov.shtwfgs.cn

[L08] 并发请求多个地址
来源：http://gm.huixinmuqiang.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://sn.newstarts.cn

PHP:  curl_multi_init() 系列
来源：http://qf.hahajie.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jt.chemitech.net.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kr.huanxung.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://qe.shxzukj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://tm.lnxyls.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://xw.lnxyls.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://no.newstarts.cn

================================================================================
来源：http://ok.colortex.cn

M. 命令行 / 进程 / 环境
来源：http://wi.hahajie.cn

================================================================================
来源：http://bm.hahajie.cn

[M01] 读取命令行参数
来源：http://jj.yuexingan06.cn

Py:   sys.argv[1:]
来源：http://gy.chemitech.net.cn

PHP:  $argv;  $argc;
来源：http://fb.wgjwhj.cn

JS:   process.argv.slice(2)
来源：http://ao.asd995.cn

TS:   process.argv.slice(2)
来源：http://it.huixiangedu.cn

Java: args 数组（main 方法参数）
来源：http://ix.jianghongdianzi.cn

Go:   os.Args[1:]
来源：http://ns.bookmarksfly.cn

Ruby: ARGV
来源：http://ew.huixinmuqiang.cn

C#:   args 数组（Main 方法参数）
来源：http://jh.huixiangedu.cn

[M02] 读取环境变量
来源：http://by.hahajie.cn

Py:   os.environ.get("HOME")
来源：http://aq.huanxung.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://by.chemitech.net.cn

JS:   process.env.HOME
来源：http://xq.huanxung.cn

TS:   process.env.HOME
来源：http://ld.szsharing.cn

Java: System.getenv("HOME")
来源：http://qc.bjjhwx.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://tm.shtwfgs.cn

Ruby: ENV["HOME"]
来源：http://ou.shxzukj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wm.shxzskj.cn

[M03] 执行外部命令
来源：http://hj.jianghongdianzi.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://rq.nszjky.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ru.bookmarksfly.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://tj.jianghongdianzi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://bx.newstarts.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://bp.asd995.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://jx.9csxet.cn

Ruby: system("ls -l");  `ls -l`
来源：http://hx.gzmigu.cn

C#:   Process.Start("ls", "-l");
来源：http://nh.521024.cn

[M04] 获取当前工作目录
来源：http://pv.huixiangedu.cn

Py:   os.getcwd()
来源：http://cd.nicolike.cn

PHP:  getcwd();
来源：http://li.hnjuh.cn

JS:   process.cwd()
来源：http://ad.wgjwhj.cn

TS:   process.cwd()
来源：http://sn.lnxyls.cn

Java: Path.of("").toAbsolutePath()
来源：http://tm.jctech888.com.cn

Go:   os.Getwd()
来源：http://vx.huixinmuqiang.cn

Ruby: Dir.pwd
来源：http://jm.szsharing.cn

C#:   Directory.GetCurrentDirectory()
来源：http://dm.huixinmuqiang.cn

[M05] 设置退出码
来源：http://lh.nszjky.cn

Py:   sys.exit(1)
来源：http://vz.nicolike.cn

PHP:  exit(1);
来源：http://af.huixinmuqiang.cn

JS:   process.exit(1)
来源：http://mk.hnjuh.cn

TS:   process.exit(1)
来源：http://mj.shxzukj.cn

Java: System.exit(1)
来源：http://ot.szxytkj.cn

Go:   os.Exit(1)
来源：http://hw.shtwfgs.cn

Ruby: exit 1
来源：http://dx.gzmigu.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://qv.jianghongdianzi.cn

[M06] 向标准错误输出
来源：http://co.asd995.cn

Py:   print("err", file=sys.stderr)
来源：http://gt.9csxet.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ey.jianghongdianzi.cn

JS:   console.error("err")
来源：http://bu.521024.cn

TS:   console.error("err")
来源：http://tc.panjiajie.cn

Java: System.err.println("err")
来源：http://ls.lnxyls.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://vv.bookmarksfly.cn

Ruby: warn "err"
来源：http://kr.huixinmuqiang.cn

C#:   Console.Error.WriteLine("err")
来源：http://dt.szsharing.cn

[M07] 判断是否为主入口
来源：http://xh.gzmigu.cn

Py:   if __name__ == "__main__":
来源：http://pg.shtwfgs.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ud.huanxung.cn

JS:   require.main === module
来源：http://he.muxihuayi.cn

TS:   require.main === module
来源：http://bx.haigaiapp.cn

Java: public static void main(String[] args)
来源：http://fc.wgjwhj.cn

Go:   func main()
来源：http://mj.gzmigu.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://cz.shtwfgs.cn

C#:   static void Main(string[] args)
来源：http://wz.newstarts.cn

[M08] 获取系统与运行时信息
来源：http://bh.hnjuh.cn

Py:   platform.system();  platform.python_version()
来源：http://ji.newstarts.cn

PHP:  PHP_OS;  phpversion();
来源：http://lj.jctech888.com.cn

JS:   process.platform;  process.version
来源：http://ag.hnjuh.cn

TS:   process.platform;  process.version
来源：http://hz.9csxet.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://fd.jctech888.com.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://xb.haigaiapp.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://cd.9csxet.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://an.wgjwhj.cn

================================================================================
来源：http://bg.szsharing.cn

N. 数据结构与算法
来源：http://nf.yuntaijiaju.cn

================================================================================
来源：http://yy.panjiajie.cn

[N01] 二分查找（有序数组）
来源：http://rj.huanxung.cn

Py:   bisect.bisect_left(arr, x)
来源：http://rk.wgjwhj.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://sd.muxihuayi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tn.nszjky.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cg.bjjhwx.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ux.shtwfgs.cn

Go:   sort.SearchInts(arr, x)
来源：http://ht.panjiajie.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://mu.newstarts.cn

C#:   Array.BinarySearch(arr, x)
来源：http://rz.jianghongdianzi.cn

[N02] 排序（工程实践用内置实现）
来源：http://ck.haigaiapp.cn

Py:   sorted(arr);  arr.sort()
来源：http://lh.szxytkj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://pt.panjiajie.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://cn.wgjwhj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://hi.newstarts.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ml.panjiajie.cn

Go:   slices.Sort(arr)
来源：http://ke.nszjky.cn


<!-- 参考信息 -->