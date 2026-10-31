代发 wailian999

Go:   time.Now().AddDate(0, 0, 7)
来源：http://lq.huixiangedu.cn

Ruby: Time.now + 7 * 86400
来源：http://wi.hnjuh.cn

C#:   DateTime.Now.AddDays(7)
来源：http://th.9csxet.cn

[J06] 计算两时间之差
来源：http://tg.wgjwhj.cn

Py:   (end - start).total_seconds()
来源：http://su.jctech888.com.cn

PHP:  $end->diff($start)->days;
来源：http://qr.jctech888.com.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://zt.jctech888.com.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://qf.huixinmuqiang.cn

Java: Duration.between(start, end).toSeconds()
来源：http://zt.bookmarksfly.cn

Go:   end.Sub(start).Hours()
来源：http://yo.shtwfgs.cn

Ruby: end - start                 # 返回秒数
来源：http://wx.newstarts.cn

C#:   (end - start).TotalSeconds
来源：http://yw.haigaiapp.cn

[J07] 比较两个日期
来源：http://st.bjjhwx.cn

Py:   d1 < d2;  d1 == d2
来源：http://if.huixinmuqiang.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://sv.huixinmuqiang.cn

JS:   d1.getTime() < d2.getTime()
来源：http://bz.jianghongdianzi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://jj.hnjuh.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ac.yuntaijiaju.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://pq.huixinmuqiang.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ge.huixiangedu.cn

C#:   d1 < d2;  d1 == d2
来源：http://za.chemitech.net.cn

[J08] 提取年月日与星期
来源：http://kh.yuexingan06.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://kq.asd995.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xo.szxytkj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://gm.jianghongdianzi.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hv.yuexingan06.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://rp.chemitech.net.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ia.shxzukj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://tp.shtwfgs.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mj.huixiangedu.cn

[J09] 时区处理
来源：http://iw.haigaiapp.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ly.nicolike.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://kj.panjiajie.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gj.szxytkj.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rf.nicolike.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://jt.jianghongdianzi.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ia.shtwfgs.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://vk.newstarts.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://uu.gzmigu.cn

[J10] 取今天 / 本月第一天
来源：http://lp.jctech888.com.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ac.bookmarksfly.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://gv.jctech888.com.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://cp.lnxyls.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://kq.asd995.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://yk.gzmigu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hs.muxihuayi.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://fh.colortex.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://gv.jianghongdianzi.cn

================================================================================
来源：http://cv.chemitech.net.cn

K. JSON 与序列化
来源：http://wj.huixinmuqiang.cn

================================================================================
来源：http://xb.asd995.cn

[K01] 对象转 JSON 字符串
来源：http://lt.yuexingan06.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ay.521024.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://pl.chemitech.net.cn

JS:   JSON.stringify(obj)
来源：http://xw.9csxet.cn

TS:   JSON.stringify(obj)
来源：http://pg.shxzskj.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://uw.huanxung.cn

Go:   json.Marshal(obj)
来源：http://rh.bjjhwx.cn

Ruby: obj.to_json                                     // require "json"
来源：http://cl.huanxung.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://si.szxytkj.cn

[K02] JSON 字符串转对象
来源：http://zz.jianghongdianzi.cn

Py:   json.loads(s)
来源：http://sj.huanxung.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://rk.colortex.cn

JS:   JSON.parse(s)
来源：http://ii.jctech888.com.cn

TS:   JSON.parse(s)
来源：http://ur.huixiangedu.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://yu.haigaiapp.cn

Go:   json.Unmarshal(data, &v)
来源：http://wu.panjiajie.cn

Ruby: JSON.parse(s)
来源：http://rf.huixinmuqiang.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hy.shxzukj.cn

[K03] JSON 美化输出（带缩进）
来源：http://aa.jctech888.com.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ou.asd995.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mk.yuexingan06.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://zx.gzmigu.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://cz.jctech888.com.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ta.szsharing.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://uo.yuexingan06.cn

Ruby: JSON.pretty_generate(obj)
来源：http://gm.nszjky.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://bl.muxihuayi.cn

[K04] 读取 JSON 文件
来源：http://bq.wgjwhj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://xq.nszjky.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://xs.521024.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rt.shxzukj.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qv.521024.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ab.haigaiapp.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://yr.szxytkj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://iz.bjjhwx.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://bm.gzmigu.cn

[K05] 深拷贝对象
来源：http://gs.newstarts.cn

Py:   copy.deepcopy(obj)
来源：http://uo.shxzukj.cn

PHP:  unserialize(serialize($obj));
来源：http://mn.chemitech.net.cn

JS:   structuredClone(obj)
来源：http://nx.hnjuh.cn

TS:   structuredClone(obj)
来源：http://ok.yuntaijiaju.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://zt.szsharing.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ok.huixinmuqiang.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mn.9csxet.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://rv.shxzskj.cn

[K06] 解析 URL 查询串
来源：http://kx.colortex.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wt.jianghongdianzi.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://yq.nicolike.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://um.bjjhwx.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wh.nszjky.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ob.hnjuh.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ph.shtwfgs.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ys.colortex.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://xw.colortex.cn

[K07] 进制转换
来源：http://ni.shtwfgs.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://cx.bjjhwx.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://si.muxihuayi.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://fc.bjjhwx.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://xq.newstarts.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://yt.hahajie.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://gi.colortex.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://sw.muxihuayi.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ks.newstarts.cn

[K08] 二进制序列化（非 JSON）
来源：http://gn.panjiajie.cn

Py:   pickle.dumps(obj)
来源：http://oj.asd995.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://at.szxytkj.cn

JS:   v8.serialize(obj)        // Node
来源：http://le.yuntaijiaju.cn

TS:   v8.serialize(obj)        // Node
来源：http://rf.lnxyls.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://bl.yuntaijiaju.cn

Go:   encoding/gob
来源：http://hd.wgjwhj.cn

Ruby: Marshal.dump(obj)
来源：http://sa.bookmarksfly.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://kv.wgjwhj.cn

================================================================================
来源：http://vv.shtwfgs.cn

L. 网络请求
来源：http://xk.newstarts.cn

================================================================================
来源：http://ba.yuexingan06.cn

[L01] 发送 GET 请求
来源：http://hq.gzmigu.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://sd.shxzukj.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wa.huanxung.cn

JS:   await fetch(url)
来源：http://rb.yuntaijiaju.cn

TS:   await fetch(url)
来源：http://xq.yuexingan06.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ge.shtwfgs.cn

Go:   resp, err := http.Get(url)
来源：http://ht.szsharing.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://nq.jianghongdianzi.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://bu.hahajie.cn

[L02] 发送 POST JSON
来源：http://ko.szxytkj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://cy.nicolike.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://gl.huixiangedu.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bh.bjjhwx.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ml.newstarts.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wn.huixinmuqiang.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://yc.huixiangedu.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://iu.szsharing.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hu.szxytkj.cn

[L03] 设置自定义请求头
来源：http://bz.hnjuh.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://oy.nszjky.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://di.9csxet.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fe.nicolike.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sh.jianghongdianzi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://su.bjjhwx.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://em.huanxung.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://sm.shxzskj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://dj.chemitech.net.cn

[L04] 设置超时
来源：http://id.hnjuh.cn

Py:   requests.get(url, timeout=5)
来源：http://zl.huixiangedu.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://fz.newstarts.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cp.gzmigu.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cz.jctech888.com.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mc.jctech888.com.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://qg.haigaiapp.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ty.colortex.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://rp.hahajie.cn

[L05] 上传文件（multipart）
来源：http://nd.hnjuh.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://nv.yuntaijiaju.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://qr.bookmarksfly.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mj.521024.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://yf.bookmarksfly.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hs.hnjuh.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ab.yuntaijiaju.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://kj.gzmigu.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ya.nicolike.cn

[L06] 解析响应为 JSON
来源：http://bg.panjiajie.cn

Py:   resp.json()
来源：http://vt.yuexingan06.cn

PHP:  json_decode($body, true);
来源：http://gz.asd995.cn

JS:   await resp.json()
来源：http://nw.colortex.cn

TS:   await resp.json()
来源：http://wr.yuexingan06.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://br.chemitech.net.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://dt.shxzukj.cn

Ruby: JSON.parse(resp.body)
来源：http://cb.521024.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://rq.haigaiapp.cn

[L07] 处理 HTTP 状态码
来源：http://cw.nicolike.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://zg.shtwfgs.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://lu.9csxet.cn

JS:   resp.ok;  resp.status
来源：http://du.haigaiapp.cn

TS:   resp.ok;  resp.status
来源：http://tn.muxihuayi.cn

Java: resp.statusCode()
来源：http://uf.szxytkj.cn

Go:   resp.StatusCode
来源：http://xy.nszjky.cn

Ruby: resp.code.to_i
来源：http://ch.521024.cn

C#:   (int)resp.StatusCode
来源：http://rg.bookmarksfly.cn

[L08] 并发请求多个地址
来源：http://ab.szxytkj.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://xe.muxihuayi.cn

PHP:  curl_multi_init() 系列
来源：http://nv.nszjky.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xg.hahajie.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qv.panjiajie.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://dk.haigaiapp.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://vv.huanxung.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://if.shxzukj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://te.hnjuh.cn

================================================================================
来源：http://tb.haigaiapp.cn

M. 命令行 / 进程 / 环境
来源：http://bm.nszjky.cn

================================================================================
来源：http://og.nszjky.cn

[M01] 读取命令行参数
来源：http://hl.521024.cn

Py:   sys.argv[1:]
来源：http://gp.lnxyls.cn

PHP:  $argv;  $argc;
来源：http://hp.nicolike.cn

JS:   process.argv.slice(2)
来源：http://ft.bookmarksfly.cn

TS:   process.argv.slice(2)
来源：http://pg.huixinmuqiang.cn

Java: args 数组（main 方法参数）
来源：http://jc.szsharing.cn

Go:   os.Args[1:]
来源：http://qo.newstarts.cn

Ruby: ARGV
来源：http://ij.yuntaijiaju.cn

C#:   args 数组（Main 方法参数）
来源：http://lv.jianghongdianzi.cn

[M02] 读取环境变量
来源：http://dm.muxihuayi.cn

Py:   os.environ.get("HOME")
来源：http://fd.huanxung.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://vl.nszjky.cn

JS:   process.env.HOME
来源：http://vc.hahajie.cn

TS:   process.env.HOME
来源：http://au.jctech888.com.cn

Java: System.getenv("HOME")
来源：http://yr.huanxung.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wc.yuntaijiaju.cn

Ruby: ENV["HOME"]
来源：http://oe.huixiangedu.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ii.haigaiapp.cn

[M03] 执行外部命令
来源：http://sk.asd995.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://er.asd995.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hv.huixiangedu.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://yv.colortex.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://xv.yuexingan06.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://io.wgjwhj.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://mj.wgjwhj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://zi.haigaiapp.cn

C#:   Process.Start("ls", "-l");
来源：http://bt.yuntaijiaju.cn

[M04] 获取当前工作目录
来源：http://li.lnxyls.cn

Py:   os.getcwd()
来源：http://fk.lnxyls.cn

PHP:  getcwd();
来源：http://yk.521024.cn

JS:   process.cwd()
来源：http://pg.panjiajie.cn

TS:   process.cwd()
来源：http://kx.nicolike.cn

Java: Path.of("").toAbsolutePath()
来源：http://lp.szsharing.cn

Go:   os.Getwd()
来源：http://ii.bjjhwx.cn

Ruby: Dir.pwd
来源：http://nd.shxzskj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://em.nszjky.cn

[M05] 设置退出码
来源：http://xq.huixinmuqiang.cn

Py:   sys.exit(1)
来源：http://tb.hnjuh.cn

PHP:  exit(1);
来源：http://gj.chemitech.net.cn

JS:   process.exit(1)
来源：http://sx.yuexingan06.cn

TS:   process.exit(1)
来源：http://ac.lnxyls.cn

Java: System.exit(1)
来源：http://oo.lnxyls.cn

Go:   os.Exit(1)
来源：http://nr.nszjky.cn

Ruby: exit 1
来源：http://rf.huixiangedu.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ep.asd995.cn

[M06] 向标准错误输出
来源：http://kz.szxytkj.cn

Py:   print("err", file=sys.stderr)
来源：http://rf.huixiangedu.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://yc.jianghongdianzi.cn

JS:   console.error("err")
来源：http://ni.jctech888.com.cn

TS:   console.error("err")
来源：http://vf.hnjuh.cn

Java: System.err.println("err")
来源：http://wp.jianghongdianzi.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://aj.shxzskj.cn

Ruby: warn "err"
来源：http://vu.asd995.cn

C#:   Console.Error.WriteLine("err")
来源：http://id.szsharing.cn

[M07] 判断是否为主入口
来源：http://wv.yuntaijiaju.cn

Py:   if __name__ == "__main__":
来源：http://hk.nicolike.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://qt.jianghongdianzi.cn

JS:   require.main === module
来源：http://wg.lnxyls.cn

TS:   require.main === module
来源：http://uk.wgjwhj.cn

Java: public static void main(String[] args)
来源：http://np.szxytkj.cn

Go:   func main()
来源：http://nt.yuexingan06.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://lz.szsharing.cn

C#:   static void Main(string[] args)
来源：http://dq.nszjky.cn

[M08] 获取系统与运行时信息
来源：http://qe.bookmarksfly.cn

Py:   platform.system();  platform.python_version()
来源：http://hd.jianghongdianzi.cn

PHP:  PHP_OS;  phpversion();
来源：http://hr.9csxet.cn

JS:   process.platform;  process.version
来源：http://ks.jctech888.com.cn

TS:   process.platform;  process.version
来源：http://qm.hahajie.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://gd.colortex.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://rp.huanxung.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ap.jianghongdianzi.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ct.bjjhwx.cn

================================================================================
来源：http://dp.muxihuayi.cn

N. 数据结构与算法
来源：http://zb.shxzukj.cn

================================================================================
来源：http://jg.shxzukj.cn

[N01] 二分查找（有序数组）
来源：http://ug.521024.cn

Py:   bisect.bisect_left(arr, x)
来源：http://fi.panjiajie.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://dc.newstarts.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yf.wgjwhj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nv.chemitech.net.cn

Java: Arrays.binarySearch(arr, x)
来源：http://gm.haigaiapp.cn

Go:   sort.SearchInts(arr, x)
来源：http://qa.yuexingan06.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://dr.chemitech.net.cn

C#:   Array.BinarySearch(arr, x)
来源：http://dn.haigaiapp.cn

[N02] 排序（工程实践用内置实现）
来源：http://mm.hnjuh.cn

Py:   sorted(arr);  arr.sort()
来源：http://km.newstarts.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://jk.huixiangedu.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://dw.szxytkj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://es.yuexingan06.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mu.jctech888.com.cn

Go:   slices.Sort(arr)
来源：http://jz.nicolike.cn

Ruby: arr.sort
来源：http://vm.huixiangedu.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://wg.nicolike.cn

[N03] 快速排序（分治示例）
来源：http://ds.jctech888.com.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ov.panjiajie.cn

PHP:  // 递归实现，或用 usort
来源：http://fc.yuntaijiaju.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mz.9csxet.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jr.haigaiapp.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://dm.hnjuh.cn


<!-- 参考信息 -->