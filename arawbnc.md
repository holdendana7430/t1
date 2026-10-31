代发 wailian999

Go:   time.Now().AddDate(0, 0, 7)
来源：http://us.9csxet.cn

Ruby: Time.now + 7 * 86400
来源：http://xv.asd995.cn

C#:   DateTime.Now.AddDays(7)
来源：http://xw.newstarts.cn

[J06] 计算两时间之差
来源：http://di.yuexingan06.cn

Py:   (end - start).total_seconds()
来源：http://fc.bookmarksfly.cn

PHP:  $end->diff($start)->days;
来源：http://jt.newstarts.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://en.9csxet.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ha.wgjwhj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://qc.yuexingan06.cn

Go:   end.Sub(start).Hours()
来源：http://lz.colortex.cn

Ruby: end - start                 # 返回秒数
来源：http://bi.newstarts.cn

C#:   (end - start).TotalSeconds
来源：http://yf.panjiajie.cn

[J07] 比较两个日期
来源：http://xb.jctech888.com.cn

Py:   d1 < d2;  d1 == d2
来源：http://qm.lnxyls.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://uo.panjiajie.cn

JS:   d1.getTime() < d2.getTime()
来源：http://uj.shxzukj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://fk.asd995.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wn.chemitech.net.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://jo.hahajie.cn

Ruby: d1 < d2;  d1 == d2
来源：http://os.bookmarksfly.cn

C#:   d1 < d2;  d1 == d2
来源：http://mq.lnxyls.cn

[J08] 提取年月日与星期
来源：http://gf.shxzskj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://gs.nicolike.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://gz.huixinmuqiang.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://cl.shxzskj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://eg.lnxyls.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ov.yuexingan06.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://np.jctech888.com.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://jo.haigaiapp.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://aj.521024.cn

[J09] 时区处理
来源：http://yx.hahajie.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://pk.yuntaijiaju.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://vc.huixinmuqiang.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ll.wgjwhj.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mo.hnjuh.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://rt.bookmarksfly.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hi.asd995.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ue.shtwfgs.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://nd.bookmarksfly.cn

[J10] 取今天 / 本月第一天
来源：http://cw.asd995.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ph.asd995.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://cd.nszjky.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ii.szxytkj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://fr.jctech888.com.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mx.bjjhwx.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://zu.muxihuayi.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://pi.newstarts.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ye.colortex.cn

================================================================================
来源：http://kh.newstarts.cn

K. JSON 与序列化
来源：http://lo.szsharing.cn

================================================================================
来源：http://jc.bjjhwx.cn

[K01] 对象转 JSON 字符串
来源：http://bz.szxytkj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://kg.lnxyls.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xl.bjjhwx.cn

JS:   JSON.stringify(obj)
来源：http://lx.nszjky.cn

TS:   JSON.stringify(obj)
来源：http://eo.shxzukj.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://sp.panjiajie.cn

Go:   json.Marshal(obj)
来源：http://pa.nszjky.cn

Ruby: obj.to_json                                     // require "json"
来源：http://zc.chemitech.net.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://fn.gzmigu.cn

[K02] JSON 字符串转对象
来源：http://vc.shxzukj.cn

Py:   json.loads(s)
来源：http://uw.szxytkj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://cm.jctech888.com.cn

JS:   JSON.parse(s)
来源：http://hn.asd995.cn

TS:   JSON.parse(s)
来源：http://ly.nicolike.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ew.521024.cn

Go:   json.Unmarshal(data, &v)
来源：http://st.szxytkj.cn

Ruby: JSON.parse(s)
来源：http://ku.hnjuh.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ws.newstarts.cn

[K03] JSON 美化输出（带缩进）
来源：http://om.jctech888.com.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://yc.nszjky.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://gd.szxytkj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://kx.bjjhwx.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://nb.yuexingan06.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://at.shtwfgs.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://rm.wgjwhj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://jx.chemitech.net.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://he.shxzskj.cn

[K04] 读取 JSON 文件
来源：http://do.yuexingan06.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ts.521024.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ru.521024.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://py.huixiangedu.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://os.huixiangedu.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vm.huixinmuqiang.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://tk.yuexingan06.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ue.shxzukj.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://fw.szxytkj.cn

[K05] 深拷贝对象
来源：http://yx.szsharing.cn

Py:   copy.deepcopy(obj)
来源：http://eq.shxzukj.cn

PHP:  unserialize(serialize($obj));
来源：http://qs.yuexingan06.cn

JS:   structuredClone(obj)
来源：http://jf.chemitech.net.cn

TS:   structuredClone(obj)
来源：http://ii.yuntaijiaju.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://oi.shxzskj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://vk.yuntaijiaju.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ql.huanxung.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ut.shtwfgs.cn

[K06] 解析 URL 查询串
来源：http://fu.chemitech.net.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://jr.huixiangedu.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://au.muxihuayi.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ss.newstarts.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pr.muxihuayi.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://nl.hnjuh.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://yp.jctech888.com.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://sj.szsharing.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://vz.newstarts.cn

[K07] 进制转换
来源：http://zw.newstarts.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://py.shxzukj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ve.jctech888.com.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://av.shtwfgs.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wm.jianghongdianzi.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://qm.szxytkj.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://qw.lnxyls.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://db.nszjky.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://nj.shxzskj.cn

[K08] 二进制序列化（非 JSON）
来源：http://yn.panjiajie.cn

Py:   pickle.dumps(obj)
来源：http://nf.shxzukj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://qq.newstarts.cn

JS:   v8.serialize(obj)        // Node
来源：http://gt.nicolike.cn

TS:   v8.serialize(obj)        // Node
来源：http://bs.colortex.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://fs.hahajie.cn

Go:   encoding/gob
来源：http://nb.nicolike.cn

Ruby: Marshal.dump(obj)
来源：http://no.shxzskj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://lb.hahajie.cn

================================================================================
来源：http://zn.bjjhwx.cn

L. 网络请求
来源：http://uf.yuexingan06.cn

================================================================================
来源：http://ma.bookmarksfly.cn

[L01] 发送 GET 请求
来源：http://yl.chemitech.net.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://nc.huixiangedu.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://iw.lnxyls.cn

JS:   await fetch(url)
来源：http://yq.jctech888.com.cn

TS:   await fetch(url)
来源：http://ht.bjjhwx.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://bo.bookmarksfly.cn

Go:   resp, err := http.Get(url)
来源：http://cw.bookmarksfly.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://yp.9csxet.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://fp.jctech888.com.cn

[L02] 发送 POST JSON
来源：http://vm.muxihuayi.cn

Py:   requests.post(url, json={"a": 1})
来源：http://lo.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://fn.521024.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dl.521024.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://py.521024.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ct.shxzukj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://tr.gzmigu.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://bt.huixiangedu.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mi.jctech888.com.cn

[L03] 设置自定义请求头
来源：http://wh.jctech888.com.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://fd.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ct.wgjwhj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ee.szsharing.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://et.hahajie.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ax.9csxet.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://or.jianghongdianzi.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://bp.szxytkj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://gl.newstarts.cn

[L04] 设置超时
来源：http://gj.yuexingan06.cn

Py:   requests.get(url, timeout=5)
来源：http://dy.nicolike.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wv.nszjky.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cw.panjiajie.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kz.colortex.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://cj.jianghongdianzi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://je.szxytkj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://kz.hahajie.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://zp.panjiajie.cn

[L05] 上传文件（multipart）
来源：http://eg.hnjuh.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://sp.asd995.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://gq.gzmigu.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://zg.yuntaijiaju.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://up.newstarts.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://la.huanxung.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://fx.shxzskj.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://jx.huixinmuqiang.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ja.muxihuayi.cn

[L06] 解析响应为 JSON
来源：http://nv.szsharing.cn

Py:   resp.json()
来源：http://np.huixinmuqiang.cn

PHP:  json_decode($body, true);
来源：http://yr.shtwfgs.cn

JS:   await resp.json()
来源：http://rg.huixiangedu.cn

TS:   await resp.json()
来源：http://kf.muxihuayi.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://fk.nicolike.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://lp.hnjuh.cn

Ruby: JSON.parse(resp.body)
来源：http://tk.nicolike.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wt.asd995.cn

[L07] 处理 HTTP 状态码
来源：http://sd.huanxung.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://kh.lnxyls.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://bk.newstarts.cn

JS:   resp.ok;  resp.status
来源：http://ty.hnjuh.cn

TS:   resp.ok;  resp.status
来源：http://tq.nicolike.cn

Java: resp.statusCode()
来源：http://rt.colortex.cn

Go:   resp.StatusCode
来源：http://rq.gzmigu.cn

Ruby: resp.code.to_i
来源：http://rz.bookmarksfly.cn

C#:   (int)resp.StatusCode
来源：http://ad.haigaiapp.cn

[L08] 并发请求多个地址
来源：http://qd.newstarts.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://bt.colortex.cn

PHP:  curl_multi_init() 系列
来源：http://yc.yuexingan06.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://eo.wgjwhj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wk.newstarts.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://da.asd995.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://au.asd995.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://lp.huixiangedu.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ng.huixinmuqiang.cn

================================================================================
来源：http://wn.shxzskj.cn

M. 命令行 / 进程 / 环境
来源：http://dv.shxzskj.cn

================================================================================
来源：http://gy.szsharing.cn

[M01] 读取命令行参数
来源：http://wg.nicolike.cn

Py:   sys.argv[1:]
来源：http://lp.nicolike.cn

PHP:  $argv;  $argc;
来源：http://el.newstarts.cn

JS:   process.argv.slice(2)
来源：http://xx.wgjwhj.cn

TS:   process.argv.slice(2)
来源：http://sf.yuntaijiaju.cn

Java: args 数组（main 方法参数）
来源：http://ag.shtwfgs.cn

Go:   os.Args[1:]
来源：http://en.colortex.cn

Ruby: ARGV
来源：http://rg.shxzukj.cn

C#:   args 数组（Main 方法参数）
来源：http://tn.colortex.cn

[M02] 读取环境变量
来源：http://ej.hnjuh.cn

Py:   os.environ.get("HOME")
来源：http://mu.bjjhwx.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://af.colortex.cn

JS:   process.env.HOME
来源：http://em.muxihuayi.cn

TS:   process.env.HOME
来源：http://vz.asd995.cn

Java: System.getenv("HOME")
来源：http://gj.9csxet.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ro.shxzskj.cn

Ruby: ENV["HOME"]
来源：http://on.panjiajie.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://pw.shtwfgs.cn

[M03] 执行外部命令
来源：http://kc.bookmarksfly.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wz.panjiajie.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ws.haigaiapp.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://wh.yuntaijiaju.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://iw.szsharing.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://cv.panjiajie.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://eo.muxihuayi.cn

Ruby: system("ls -l");  `ls -l`
来源：http://bu.9csxet.cn

C#:   Process.Start("ls", "-l");
来源：http://xo.bookmarksfly.cn

[M04] 获取当前工作目录
来源：http://jz.9csxet.cn

Py:   os.getcwd()
来源：http://ox.9csxet.cn

PHP:  getcwd();
来源：http://zd.bookmarksfly.cn

JS:   process.cwd()
来源：http://nn.haigaiapp.cn

TS:   process.cwd()
来源：http://vw.9csxet.cn

Java: Path.of("").toAbsolutePath()
来源：http://ff.asd995.cn

Go:   os.Getwd()
来源：http://rz.nszjky.cn

Ruby: Dir.pwd
来源：http://xp.huixiangedu.cn

C#:   Directory.GetCurrentDirectory()
来源：http://pq.bookmarksfly.cn

[M05] 设置退出码
来源：http://cb.haigaiapp.cn

Py:   sys.exit(1)
来源：http://yy.szsharing.cn

PHP:  exit(1);
来源：http://wc.huanxung.cn

JS:   process.exit(1)
来源：http://qs.yuexingan06.cn

TS:   process.exit(1)
来源：http://kn.nicolike.cn

Java: System.exit(1)
来源：http://zb.huixinmuqiang.cn

Go:   os.Exit(1)
来源：http://es.huixinmuqiang.cn

Ruby: exit 1
来源：http://nw.haigaiapp.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://px.colortex.cn

[M06] 向标准错误输出
来源：http://gn.shxzskj.cn

Py:   print("err", file=sys.stderr)
来源：http://nv.hnjuh.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://cf.9csxet.cn

JS:   console.error("err")
来源：http://ij.bjjhwx.cn

TS:   console.error("err")
来源：http://hz.bookmarksfly.cn

Java: System.err.println("err")
来源：http://cx.wgjwhj.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mo.huixiangedu.cn

Ruby: warn "err"
来源：http://vd.9csxet.cn

C#:   Console.Error.WriteLine("err")
来源：http://eb.shtwfgs.cn

[M07] 判断是否为主入口
来源：http://zu.jianghongdianzi.cn

Py:   if __name__ == "__main__":
来源：http://pa.haigaiapp.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ig.bjjhwx.cn

JS:   require.main === module
来源：http://cb.asd995.cn

TS:   require.main === module
来源：http://zg.gzmigu.cn

Java: public static void main(String[] args)
来源：http://yt.huixiangedu.cn

Go:   func main()
来源：http://dz.huixiangedu.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://du.chemitech.net.cn

C#:   static void Main(string[] args)
来源：http://vh.bookmarksfly.cn

[M08] 获取系统与运行时信息
来源：http://vn.huixiangedu.cn

Py:   platform.system();  platform.python_version()
来源：http://fa.9csxet.cn

PHP:  PHP_OS;  phpversion();
来源：http://eh.newstarts.cn

JS:   process.platform;  process.version
来源：http://la.haigaiapp.cn

TS:   process.platform;  process.version
来源：http://yn.shtwfgs.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://uo.521024.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://nq.szsharing.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://jw.wgjwhj.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://gt.panjiajie.cn

================================================================================
来源：http://mh.huanxung.cn

N. 数据结构与算法
来源：http://kq.lnxyls.cn

================================================================================
来源：http://ci.haigaiapp.cn

[N01] 二分查找（有序数组）
来源：http://hb.huixinmuqiang.cn

Py:   bisect.bisect_left(arr, x)
来源：http://bf.hnjuh.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://iq.yuexingan06.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zg.hahajie.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kx.shxzukj.cn

Java: Arrays.binarySearch(arr, x)
来源：http://tf.nszjky.cn

Go:   sort.SearchInts(arr, x)
来源：http://fx.jianghongdianzi.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://xp.wgjwhj.cn

C#:   Array.BinarySearch(arr, x)
来源：http://zb.521024.cn

[N02] 排序（工程实践用内置实现）
来源：http://zh.haigaiapp.cn

Py:   sorted(arr);  arr.sort()
来源：http://ba.gzmigu.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ch.asd995.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://cx.hnjuh.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://fi.haigaiapp.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ps.gzmigu.cn

Go:   slices.Sort(arr)
来源：http://uh.521024.cn

Ruby: arr.sort
来源：http://gv.szxytkj.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ar.521024.cn

[N03] 快速排序（分治示例）
来源：http://kc.jianghongdianzi.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ry.newstarts.cn

PHP:  // 递归实现，或用 usort
来源：http://uq.chemitech.net.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://by.szxytkj.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qh.nicolike.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://eo.newstarts.cn


<!-- 参考信息 -->