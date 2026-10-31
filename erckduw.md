代发 wailian999

Py:   (end - start).total_seconds()
来源：http://pc.shxzukj.cn

PHP:  $end->diff($start)->days;
来源：http://pt.newstarts.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wu.szsharing.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://de.huixinmuqiang.cn

Java: Duration.between(start, end).toSeconds()
来源：http://sp.lnxyls.cn

Go:   end.Sub(start).Hours()
来源：http://yl.lnxyls.cn

Ruby: end - start                 # 返回秒数
来源：http://dl.jctech888.com.cn

C#:   (end - start).TotalSeconds
来源：http://fw.521024.cn

[J07] 比较两个日期
来源：http://os.wgjwhj.cn

Py:   d1 < d2;  d1 == d2
来源：http://ei.bookmarksfly.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://vu.yuntaijiaju.cn

JS:   d1.getTime() < d2.getTime()
来源：http://sq.shxzskj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://zo.yuexingan06.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wg.nicolike.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://fz.nszjky.cn

Ruby: d1 < d2;  d1 == d2
来源：http://pv.huanxung.cn

C#:   d1 < d2;  d1 == d2
来源：http://ff.yuexingan06.cn

[J08] 提取年月日与星期
来源：http://wa.huixiangedu.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mq.nicolike.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://uu.shxzskj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hq.lnxyls.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ya.szxytkj.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ml.muxihuayi.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://cw.shtwfgs.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://yx.huixiangedu.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://bd.lnxyls.cn

[J09] 时区处理
来源：http://ve.hahajie.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://lf.asd995.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://dk.panjiajie.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://px.9csxet.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mn.hahajie.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://oh.wgjwhj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://fv.yuntaijiaju.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://jz.jctech888.com.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://uu.wgjwhj.cn

[J10] 取今天 / 本月第一天
来源：http://rb.szsharing.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://hj.jianghongdianzi.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://zz.bookmarksfly.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vs.jctech888.com.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qa.hnjuh.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zu.bjjhwx.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ig.wgjwhj.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://jo.521024.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://bf.yuntaijiaju.cn

================================================================================
来源：http://mg.hnjuh.cn

K. JSON 与序列化
来源：http://rn.huixinmuqiang.cn

================================================================================
来源：http://ov.bookmarksfly.cn

[K01] 对象转 JSON 字符串
来源：http://gw.bookmarksfly.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ra.bookmarksfly.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://yx.yuexingan06.cn

JS:   JSON.stringify(obj)
来源：http://hp.jctech888.com.cn

TS:   JSON.stringify(obj)
来源：http://yd.chemitech.net.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ld.huixinmuqiang.cn

Go:   json.Marshal(obj)
来源：http://mq.bjjhwx.cn

Ruby: obj.to_json                                     // require "json"
来源：http://tc.9csxet.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://gg.hahajie.cn

[K02] JSON 字符串转对象
来源：http://zf.nszjky.cn

Py:   json.loads(s)
来源：http://pt.haigaiapp.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://oy.huixinmuqiang.cn

JS:   JSON.parse(s)
来源：http://eq.yuexingan06.cn

TS:   JSON.parse(s)
来源：http://tt.gzmigu.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://it.szxytkj.cn

Go:   json.Unmarshal(data, &v)
来源：http://dv.gzmigu.cn

Ruby: JSON.parse(s)
来源：http://ia.jctech888.com.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qr.colortex.cn

[K03] JSON 美化输出（带缩进）
来源：http://dh.yuntaijiaju.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://im.yuntaijiaju.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://tv.szxytkj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://vt.huanxung.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://fu.panjiajie.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ie.hahajie.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://el.haigaiapp.cn

Ruby: JSON.pretty_generate(obj)
来源：http://qu.nicolike.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ht.asd995.cn

[K04] 读取 JSON 文件
来源：http://zq.newstarts.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ia.hnjuh.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ll.lnxyls.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sv.yuntaijiaju.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wu.gzmigu.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ck.huanxung.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ba.bookmarksfly.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://pm.chemitech.net.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ix.newstarts.cn

[K05] 深拷贝对象
来源：http://vy.shtwfgs.cn

Py:   copy.deepcopy(obj)
来源：http://oh.jctech888.com.cn

PHP:  unserialize(serialize($obj));
来源：http://rz.shxzskj.cn

JS:   structuredClone(obj)
来源：http://dg.jctech888.com.cn

TS:   structuredClone(obj)
来源：http://vt.colortex.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ua.szxytkj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://gj.szsharing.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ls.shtwfgs.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ex.huixiangedu.cn

[K06] 解析 URL 查询串
来源：http://ly.9csxet.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://tq.nszjky.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fn.bookmarksfly.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vw.nszjky.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sb.huanxung.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ia.shxzukj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://yk.huixinmuqiang.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://nb.chemitech.net.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ed.huixiangedu.cn

[K07] 进制转换
来源：http://ls.521024.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ig.haigaiapp.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vo.jctech888.com.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://qu.hahajie.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://bp.hnjuh.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xh.huanxung.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://va.panjiajie.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://je.wgjwhj.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wf.yuntaijiaju.cn

[K08] 二进制序列化（非 JSON）
来源：http://en.chemitech.net.cn

Py:   pickle.dumps(obj)
来源：http://ck.haigaiapp.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://eu.yuntaijiaju.cn

JS:   v8.serialize(obj)        // Node
来源：http://mo.nicolike.cn

TS:   v8.serialize(obj)        // Node
来源：http://kc.yuexingan06.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://am.newstarts.cn

Go:   encoding/gob
来源：http://os.huixiangedu.cn

Ruby: Marshal.dump(obj)
来源：http://co.nszjky.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://we.jianghongdianzi.cn

================================================================================
来源：http://rp.szsharing.cn

L. 网络请求
来源：http://we.colortex.cn

================================================================================
来源：http://av.muxihuayi.cn

[L01] 发送 GET 请求
来源：http://ef.521024.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ai.jctech888.com.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://gj.newstarts.cn

JS:   await fetch(url)
来源：http://xe.lnxyls.cn

TS:   await fetch(url)
来源：http://mo.huixinmuqiang.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wm.bjjhwx.cn

Go:   resp, err := http.Get(url)
来源：http://qo.huixiangedu.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://em.chemitech.net.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://vm.asd995.cn

[L02] 发送 POST JSON
来源：http://jr.shxzskj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://po.szsharing.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://uu.newstarts.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zp.szsharing.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kr.jctech888.com.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ah.gzmigu.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://iz.huixinmuqiang.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://vo.shxzskj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ls.shxzukj.cn

[L03] 设置自定义请求头
来源：http://jr.szxytkj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://la.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://bn.chemitech.net.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ds.nszjky.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xj.jianghongdianzi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://eb.szxytkj.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ga.huixiangedu.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.yuntaijiaju.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ox.newstarts.cn

[L04] 设置超时
来源：http://if.chemitech.net.cn

Py:   requests.get(url, timeout=5)
来源：http://zi.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://us.9csxet.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rx.bjjhwx.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qv.bookmarksfly.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://tc.bookmarksfly.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://uk.haigaiapp.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ql.asd995.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://da.nszjky.cn

[L05] 上传文件（multipart）
来源：http://fk.jctech888.com.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://db.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://dg.hahajie.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mo.muxihuayi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hy.chemitech.net.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://xj.yuntaijiaju.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://rj.chemitech.net.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ig.huixinmuqiang.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://tx.hnjuh.cn

[L06] 解析响应为 JSON
来源：http://tc.newstarts.cn

Py:   resp.json()
来源：http://ue.gzmigu.cn

PHP:  json_decode($body, true);
来源：http://ao.huanxung.cn

JS:   await resp.json()
来源：http://zi.shxzukj.cn

TS:   await resp.json()
来源：http://zq.szsharing.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://nl.colortex.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://jf.haigaiapp.cn

Ruby: JSON.parse(resp.body)
来源：http://ut.panjiajie.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ho.haigaiapp.cn

[L07] 处理 HTTP 状态码
来源：http://gi.panjiajie.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://tj.shtwfgs.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ek.nicolike.cn

JS:   resp.ok;  resp.status
来源：http://hy.jctech888.com.cn

TS:   resp.ok;  resp.status
来源：http://dn.chemitech.net.cn

Java: resp.statusCode()
来源：http://gp.yuexingan06.cn

Go:   resp.StatusCode
来源：http://wi.nszjky.cn

Ruby: resp.code.to_i
来源：http://tv.yuexingan06.cn

C#:   (int)resp.StatusCode
来源：http://br.9csxet.cn

[L08] 并发请求多个地址
来源：http://vt.shtwfgs.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://re.bjjhwx.cn

PHP:  curl_multi_init() 系列
来源：http://jd.bookmarksfly.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kz.hnjuh.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nb.yuntaijiaju.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://xw.huanxung.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://bk.huixinmuqiang.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ef.huanxung.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://jp.huixiangedu.cn

================================================================================
来源：http://jo.wgjwhj.cn

M. 命令行 / 进程 / 环境
来源：http://cy.jctech888.com.cn

================================================================================
来源：http://yj.haigaiapp.cn

[M01] 读取命令行参数
来源：http://bj.yuntaijiaju.cn

Py:   sys.argv[1:]
来源：http://go.yuntaijiaju.cn

PHP:  $argv;  $argc;
来源：http://vh.shtwfgs.cn

JS:   process.argv.slice(2)
来源：http://hz.chemitech.net.cn

TS:   process.argv.slice(2)
来源：http://ge.hahajie.cn

Java: args 数组（main 方法参数）
来源：http://wq.szxytkj.cn

Go:   os.Args[1:]
来源：http://wl.shtwfgs.cn

Ruby: ARGV
来源：http://mu.huanxung.cn

C#:   args 数组（Main 方法参数）
来源：http://lb.shtwfgs.cn

[M02] 读取环境变量
来源：http://iw.panjiajie.cn

Py:   os.environ.get("HOME")
来源：http://di.hahajie.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ru.shxzukj.cn

JS:   process.env.HOME
来源：http://tu.haigaiapp.cn

TS:   process.env.HOME
来源：http://kf.gzmigu.cn

Java: System.getenv("HOME")
来源：http://ul.bjjhwx.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://su.jianghongdianzi.cn

Ruby: ENV["HOME"]
来源：http://rc.newstarts.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ro.szsharing.cn

[M03] 执行外部命令
来源：http://dm.szsharing.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ca.nszjky.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://yl.muxihuayi.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://fl.bookmarksfly.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://nk.nszjky.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://nx.colortex.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://uh.huixiangedu.cn

Ruby: system("ls -l");  `ls -l`
来源：http://et.hnjuh.cn

C#:   Process.Start("ls", "-l");
来源：http://ea.colortex.cn

[M04] 获取当前工作目录
来源：http://hx.huanxung.cn

Py:   os.getcwd()
来源：http://pw.bookmarksfly.cn

PHP:  getcwd();
来源：http://or.hahajie.cn

JS:   process.cwd()
来源：http://ut.bookmarksfly.cn

TS:   process.cwd()
来源：http://uc.asd995.cn

Java: Path.of("").toAbsolutePath()
来源：http://oy.yuexingan06.cn

Go:   os.Getwd()
来源：http://em.huixinmuqiang.cn

Ruby: Dir.pwd
来源：http://am.jctech888.com.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ce.yuntaijiaju.cn

[M05] 设置退出码
来源：http://jc.shxzukj.cn

Py:   sys.exit(1)
来源：http://to.gzmigu.cn

PHP:  exit(1);
来源：http://qj.muxihuayi.cn

JS:   process.exit(1)
来源：http://lo.muxihuayi.cn

TS:   process.exit(1)
来源：http://ko.newstarts.cn

Java: System.exit(1)
来源：http://kr.yuntaijiaju.cn

Go:   os.Exit(1)
来源：http://ds.hahajie.cn

Ruby: exit 1
来源：http://jz.hahajie.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wq.muxihuayi.cn

[M06] 向标准错误输出
来源：http://jy.haigaiapp.cn

Py:   print("err", file=sys.stderr)
来源：http://xa.hnjuh.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://lw.yuntaijiaju.cn

JS:   console.error("err")
来源：http://sw.bookmarksfly.cn

TS:   console.error("err")
来源：http://us.huanxung.cn

Java: System.err.println("err")
来源：http://lo.huixinmuqiang.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://fx.jianghongdianzi.cn

Ruby: warn "err"
来源：http://gr.shxzukj.cn

C#:   Console.Error.WriteLine("err")
来源：http://ta.gzmigu.cn

[M07] 判断是否为主入口
来源：http://ue.szsharing.cn

Py:   if __name__ == "__main__":
来源：http://pm.jianghongdianzi.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mo.newstarts.cn

JS:   require.main === module
来源：http://jt.panjiajie.cn

TS:   require.main === module
来源：http://ji.bookmarksfly.cn

Java: public static void main(String[] args)
来源：http://yj.shtwfgs.cn

Go:   func main()
来源：http://ri.shtwfgs.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://jj.haigaiapp.cn

C#:   static void Main(string[] args)
来源：http://xd.yuexingan06.cn

[M08] 获取系统与运行时信息
来源：http://au.nicolike.cn

Py:   platform.system();  platform.python_version()
来源：http://bu.huanxung.cn

PHP:  PHP_OS;  phpversion();
来源：http://tm.szsharing.cn

JS:   process.platform;  process.version
来源：http://nz.shxzskj.cn

TS:   process.platform;  process.version
来源：http://pu.hnjuh.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://fi.shtwfgs.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://yj.muxihuayi.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ob.yuexingan06.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://dm.lnxyls.cn

================================================================================
来源：http://po.jctech888.com.cn

N. 数据结构与算法
来源：http://mt.nszjky.cn

================================================================================
来源：http://mp.gzmigu.cn

[N01] 二分查找（有序数组）
来源：http://wl.chemitech.net.cn

Py:   bisect.bisect_left(arr, x)
来源：http://vp.bjjhwx.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://lx.asd995.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hf.panjiajie.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xx.bjjhwx.cn

Java: Arrays.binarySearch(arr, x)
来源：http://oc.muxihuayi.cn

Go:   sort.SearchInts(arr, x)
来源：http://qg.panjiajie.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://bk.hnjuh.cn

C#:   Array.BinarySearch(arr, x)
来源：http://mu.lnxyls.cn

[N02] 排序（工程实践用内置实现）
来源：http://ys.shxzskj.cn

Py:   sorted(arr);  arr.sort()
来源：http://cl.9csxet.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mh.yuexingan06.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://kt.lnxyls.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://bq.jianghongdianzi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://er.muxihuayi.cn

Go:   slices.Sort(arr)
来源：http://fu.huixinmuqiang.cn

Ruby: arr.sort
来源：http://ue.hnjuh.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://mb.yuexingan06.cn

[N03] 快速排序（分治示例）
来源：http://qc.9csxet.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://az.lnxyls.cn

PHP:  // 递归实现，或用 usort
来源：http://iq.haigaiapp.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://co.huanxung.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://as.nicolike.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hc.jctech888.com.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://sl.hnjuh.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://bo.huixinmuqiang.cn

C#:   // 手写递归，或 Array.Sort
来源：http://bw.jctech888.com.cn

[N04] 斐波那契数列
来源：http://tx.shtwfgs.cn


<!-- 参考信息 -->