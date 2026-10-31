代发 wailian999

Py:   (end - start).total_seconds()
来源：http://ub.panjiajie.cn

PHP:  $end->diff($start)->days;
来源：http://iv.huixiangedu.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://my.panjiajie.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://nh.wgjwhj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ts.hahajie.cn

Go:   end.Sub(start).Hours()
来源：http://xi.hahajie.cn

Ruby: end - start                 # 返回秒数
来源：http://xd.colortex.cn

C#:   (end - start).TotalSeconds
来源：http://tq.shtwfgs.cn

[J07] 比较两个日期
来源：http://pp.huixiangedu.cn

Py:   d1 < d2;  d1 == d2
来源：http://by.bjjhwx.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hy.colortex.cn

JS:   d1.getTime() < d2.getTime()
来源：http://hq.asd995.cn

TS:   d1.getTime() < d2.getTime()
来源：http://oy.yuexingan06.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://iq.lnxyls.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://sy.521024.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ht.szsharing.cn

C#:   d1 < d2;  d1 == d2
来源：http://ws.yuntaijiaju.cn

[J08] 提取年月日与星期
来源：http://ou.shxzskj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://tu.asd995.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ul.nicolike.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://kh.muxihuayi.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://cy.szxytkj.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://cu.colortex.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wr.chemitech.net.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://eg.wgjwhj.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vr.yuntaijiaju.cn

[J09] 时区处理
来源：http://rz.hnjuh.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ap.nicolike.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ci.newstarts.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rb.haigaiapp.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yt.bookmarksfly.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wn.szxytkj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://yp.shtwfgs.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://pn.jianghongdianzi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://nq.szsharing.cn

[J10] 取今天 / 本月第一天
来源：http://ph.shxzskj.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://jz.newstarts.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xi.huixiangedu.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vd.bjjhwx.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hq.haigaiapp.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://vy.huanxung.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ys.nicolike.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ss.panjiajie.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://gr.shxzskj.cn

================================================================================
来源：http://cm.hnjuh.cn

K. JSON 与序列化
来源：http://fx.shxzukj.cn

================================================================================
来源：http://ym.jctech888.com.cn

[K01] 对象转 JSON 字符串
来源：http://ga.szsharing.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://jo.chemitech.net.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://nq.bjjhwx.cn

JS:   JSON.stringify(obj)
来源：http://sz.wgjwhj.cn

TS:   JSON.stringify(obj)
来源：http://tl.huixiangedu.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://zd.shtwfgs.cn

Go:   json.Marshal(obj)
来源：http://ux.shxzukj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://aj.colortex.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ps.panjiajie.cn

[K02] JSON 字符串转对象
来源：http://ad.9csxet.cn

Py:   json.loads(s)
来源：http://vr.yuntaijiaju.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://yc.panjiajie.cn

JS:   JSON.parse(s)
来源：http://nr.szsharing.cn

TS:   JSON.parse(s)
来源：http://th.521024.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ur.jianghongdianzi.cn

Go:   json.Unmarshal(data, &v)
来源：http://td.yuntaijiaju.cn

Ruby: JSON.parse(s)
来源：http://kh.bjjhwx.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ww.hahajie.cn

[K03] JSON 美化输出（带缩进）
来源：http://ao.szsharing.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://lk.huixinmuqiang.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://il.bookmarksfly.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://cy.9csxet.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ho.jianghongdianzi.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://kg.asd995.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vd.huixiangedu.cn

Ruby: JSON.pretty_generate(obj)
来源：http://fu.jianghongdianzi.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://bq.nicolike.cn

[K04] 读取 JSON 文件
来源：http://fm.jctech888.com.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://zz.huixinmuqiang.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://qi.colortex.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://uo.huixinmuqiang.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yc.nicolike.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://bg.yuexingan06.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://rk.lnxyls.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ag.bookmarksfly.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://vc.lnxyls.cn

[K05] 深拷贝对象
来源：http://vz.wgjwhj.cn

Py:   copy.deepcopy(obj)
来源：http://fp.chemitech.net.cn

PHP:  unserialize(serialize($obj));
来源：http://pb.bjjhwx.cn

JS:   structuredClone(obj)
来源：http://yc.bookmarksfly.cn

TS:   structuredClone(obj)
来源：http://cz.9csxet.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://xw.chemitech.net.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://sx.asd995.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://eh.nicolike.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://bj.haigaiapp.cn

[K06] 解析 URL 查询串
来源：http://gh.521024.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://tn.gzmigu.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mg.nszjky.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fy.gzmigu.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fn.yuexingan06.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hs.hnjuh.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://bb.newstarts.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ns.521024.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://eo.jianghongdianzi.cn

[K07] 进制转换
来源：http://bg.huixiangedu.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://kf.panjiajie.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://uz.gzmigu.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://dg.chemitech.net.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hx.521024.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ok.bookmarksfly.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://yy.9csxet.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://le.nicolike.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://tb.yuntaijiaju.cn

[K08] 二进制序列化（非 JSON）
来源：http://zw.szsharing.cn

Py:   pickle.dumps(obj)
来源：http://jf.shtwfgs.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://kd.shtwfgs.cn

JS:   v8.serialize(obj)        // Node
来源：http://ae.9csxet.cn

TS:   v8.serialize(obj)        // Node
来源：http://qd.lnxyls.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://qw.asd995.cn

Go:   encoding/gob
来源：http://qe.hahajie.cn

Ruby: Marshal.dump(obj)
来源：http://aj.huanxung.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://zd.huixiangedu.cn

================================================================================
来源：http://km.shtwfgs.cn

L. 网络请求
来源：http://wz.haigaiapp.cn

================================================================================
来源：http://vb.gzmigu.cn

[L01] 发送 GET 请求
来源：http://qb.521024.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://je.9csxet.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://yj.chemitech.net.cn

JS:   await fetch(url)
来源：http://hm.bjjhwx.cn

TS:   await fetch(url)
来源：http://dp.yuntaijiaju.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://af.wgjwhj.cn

Go:   resp, err := http.Get(url)
来源：http://vj.hnjuh.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://wz.jianghongdianzi.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://bk.huixiangedu.cn

[L02] 发送 POST JSON
来源：http://oy.szsharing.cn

Py:   requests.post(url, json={"a": 1})
来源：http://wl.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://lq.bjjhwx.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ca.nszjky.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://aj.newstarts.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://je.hnjuh.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ji.bjjhwx.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://cn.bookmarksfly.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://to.szsharing.cn

[L03] 设置自定义请求头
来源：http://ph.hahajie.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ik.nszjky.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ov.hnjuh.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sq.huanxung.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ha.9csxet.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://km.szsharing.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ky.lnxyls.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qm.521024.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ap.asd995.cn

[L04] 设置超时
来源：http://eo.hahajie.cn

Py:   requests.get(url, timeout=5)
来源：http://ji.wgjwhj.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://oo.colortex.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://sv.huixiangedu.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ln.hnjuh.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://pf.jianghongdianzi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://up.haigaiapp.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://fz.521024.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ua.szsharing.cn

[L05] 上传文件（multipart）
来源：http://cl.huixiangedu.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://dr.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://xk.yuexingan06.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://tj.gzmigu.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://fu.newstarts.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://id.shxzukj.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://eg.huixiangedu.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vk.lnxyls.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ts.521024.cn

[L06] 解析响应为 JSON
来源：http://fk.yuntaijiaju.cn

Py:   resp.json()
来源：http://vp.shxzukj.cn

PHP:  json_decode($body, true);
来源：http://lu.asd995.cn

JS:   await resp.json()
来源：http://ac.huixiangedu.cn

TS:   await resp.json()
来源：http://lp.521024.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://dq.szxytkj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hx.szxytkj.cn

Ruby: JSON.parse(resp.body)
来源：http://sn.szsharing.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ir.jianghongdianzi.cn

[L07] 处理 HTTP 状态码
来源：http://op.bjjhwx.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wp.colortex.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ks.nicolike.cn

JS:   resp.ok;  resp.status
来源：http://dl.bookmarksfly.cn

TS:   resp.ok;  resp.status
来源：http://em.colortex.cn

Java: resp.statusCode()
来源：http://pw.jctech888.com.cn

Go:   resp.StatusCode
来源：http://md.nszjky.cn

Ruby: resp.code.to_i
来源：http://xa.lnxyls.cn

C#:   (int)resp.StatusCode
来源：http://to.shxzskj.cn

[L08] 并发请求多个地址
来源：http://pd.panjiajie.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://kl.wgjwhj.cn

PHP:  curl_multi_init() 系列
来源：http://qk.huixiangedu.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mv.huixiangedu.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vk.nszjky.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hf.haigaiapp.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://kk.yuexingan06.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://xy.shtwfgs.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ym.szxytkj.cn

================================================================================
来源：http://im.yuexingan06.cn

M. 命令行 / 进程 / 环境
来源：http://du.gzmigu.cn

================================================================================
来源：http://rf.shxzukj.cn

[M01] 读取命令行参数
来源：http://dr.nicolike.cn

Py:   sys.argv[1:]
来源：http://yj.lnxyls.cn

PHP:  $argv;  $argc;
来源：http://ja.szxytkj.cn

JS:   process.argv.slice(2)
来源：http://lc.bjjhwx.cn

TS:   process.argv.slice(2)
来源：http://bp.shtwfgs.cn

Java: args 数组（main 方法参数）
来源：http://zw.jianghongdianzi.cn

Go:   os.Args[1:]
来源：http://lc.bookmarksfly.cn

Ruby: ARGV
来源：http://kl.jianghongdianzi.cn

C#:   args 数组（Main 方法参数）
来源：http://jz.yuexingan06.cn

[M02] 读取环境变量
来源：http://wy.yuntaijiaju.cn

Py:   os.environ.get("HOME")
来源：http://nk.jianghongdianzi.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://tf.panjiajie.cn

JS:   process.env.HOME
来源：http://dp.huixinmuqiang.cn

TS:   process.env.HOME
来源：http://nq.asd995.cn

Java: System.getenv("HOME")
来源：http://qn.szxytkj.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://li.hnjuh.cn

Ruby: ENV["HOME"]
来源：http://xb.lnxyls.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ma.nicolike.cn

[M03] 执行外部命令
来源：http://hb.szxytkj.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hb.muxihuayi.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://bs.yuntaijiaju.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://cz.lnxyls.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://xz.yuexingan06.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://gp.hahajie.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://oz.shtwfgs.cn

Ruby: system("ls -l");  `ls -l`
来源：http://hc.huanxung.cn

C#:   Process.Start("ls", "-l");
来源：http://yp.hahajie.cn

[M04] 获取当前工作目录
来源：http://ta.chemitech.net.cn

Py:   os.getcwd()
来源：http://hr.nszjky.cn

PHP:  getcwd();
来源：http://ra.nszjky.cn

JS:   process.cwd()
来源：http://ns.bookmarksfly.cn

TS:   process.cwd()
来源：http://bv.nicolike.cn

Java: Path.of("").toAbsolutePath()
来源：http://fr.shxzukj.cn

Go:   os.Getwd()
来源：http://ni.gzmigu.cn

Ruby: Dir.pwd
来源：http://bc.nszjky.cn

C#:   Directory.GetCurrentDirectory()
来源：http://zt.shtwfgs.cn

[M05] 设置退出码
来源：http://dd.nszjky.cn

Py:   sys.exit(1)
来源：http://ou.jianghongdianzi.cn

PHP:  exit(1);
来源：http://xs.jianghongdianzi.cn

JS:   process.exit(1)
来源：http://zg.shxzukj.cn

TS:   process.exit(1)
来源：http://pg.yuntaijiaju.cn

Java: System.exit(1)
来源：http://wg.bookmarksfly.cn

Go:   os.Exit(1)
来源：http://hb.muxihuayi.cn

Ruby: exit 1
来源：http://zm.jctech888.com.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://kq.huixinmuqiang.cn

[M06] 向标准错误输出
来源：http://ho.yuntaijiaju.cn

Py:   print("err", file=sys.stderr)
来源：http://at.panjiajie.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://wj.colortex.cn

JS:   console.error("err")
来源：http://ss.newstarts.cn

TS:   console.error("err")
来源：http://tt.haigaiapp.cn

Java: System.err.println("err")
来源：http://ej.newstarts.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://oa.huixinmuqiang.cn

Ruby: warn "err"
来源：http://oa.jctech888.com.cn

C#:   Console.Error.WriteLine("err")
来源：http://tu.gzmigu.cn

[M07] 判断是否为主入口
来源：http://uz.szsharing.cn

Py:   if __name__ == "__main__":
来源：http://ww.chemitech.net.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://xi.colortex.cn

JS:   require.main === module
来源：http://av.newstarts.cn

TS:   require.main === module
来源：http://bj.haigaiapp.cn

Java: public static void main(String[] args)
来源：http://gv.shxzukj.cn

Go:   func main()
来源：http://fp.nicolike.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://cs.gzmigu.cn

C#:   static void Main(string[] args)
来源：http://si.hnjuh.cn

[M08] 获取系统与运行时信息
来源：http://sj.hahajie.cn

Py:   platform.system();  platform.python_version()
来源：http://vp.newstarts.cn

PHP:  PHP_OS;  phpversion();
来源：http://df.nicolike.cn

JS:   process.platform;  process.version
来源：http://ux.szxytkj.cn

TS:   process.platform;  process.version
来源：http://ir.hahajie.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://zb.521024.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://dz.chemitech.net.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://oi.haigaiapp.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://rp.gzmigu.cn

================================================================================
来源：http://pa.jctech888.com.cn

N. 数据结构与算法
来源：http://hf.nszjky.cn

================================================================================
来源：http://eh.jctech888.com.cn

[N01] 二分查找（有序数组）
来源：http://nc.huanxung.cn

Py:   bisect.bisect_left(arr, x)
来源：http://zk.yuntaijiaju.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://lj.asd995.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xw.lnxyls.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kk.9csxet.cn

Java: Arrays.binarySearch(arr, x)
来源：http://rt.jianghongdianzi.cn

Go:   sort.SearchInts(arr, x)
来源：http://lm.jctech888.com.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://yq.wgjwhj.cn

C#:   Array.BinarySearch(arr, x)
来源：http://qi.chemitech.net.cn

[N02] 排序（工程实践用内置实现）
来源：http://fy.newstarts.cn

Py:   sorted(arr);  arr.sort()
来源：http://yy.bookmarksfly.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://fm.9csxet.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ga.shtwfgs.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://hi.jianghongdianzi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ej.shxzskj.cn

Go:   slices.Sort(arr)
来源：http://ng.szxytkj.cn

Ruby: arr.sort
来源：http://pr.chemitech.net.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ne.jctech888.com.cn

[N03] 快速排序（分治示例）
来源：http://oi.lnxyls.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ez.shxzskj.cn

PHP:  // 递归实现，或用 usort
来源：http://wm.colortex.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ve.colortex.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nd.chemitech.net.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://xk.asd995.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ue.haigaiapp.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://lx.yuexingan06.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ka.huixinmuqiang.cn

[N04] 斐波那契数列
来源：http://oa.shxzskj.cn


<!-- 参考信息 -->