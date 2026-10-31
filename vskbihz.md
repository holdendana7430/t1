代发 wailian999

PHP:  (new DateTime())->modify("+7 days");
来源：http://qd.yuexingan06.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://le.wgjwhj.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://jk.shtwfgs.cn

Java: LocalDate.now().plusDays(7)
来源：http://af.szsharing.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://fv.9csxet.cn

Ruby: Time.now + 7 * 86400
来源：http://fm.lnxyls.cn

C#:   DateTime.Now.AddDays(7)
来源：http://mb.gzmigu.cn

[J06] 计算两时间之差
来源：http://qw.lnxyls.cn

Py:   (end - start).total_seconds()
来源：http://ou.colortex.cn

PHP:  $end->diff($start)->days;
来源：http://qs.hahajie.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://oj.shxzukj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://yx.colortex.cn

Java: Duration.between(start, end).toSeconds()
来源：http://jg.nszjky.cn

Go:   end.Sub(start).Hours()
来源：http://xf.jctech888.com.cn

Ruby: end - start                 # 返回秒数
来源：http://ey.panjiajie.cn

C#:   (end - start).TotalSeconds
来源：http://cm.jianghongdianzi.cn

[J07] 比较两个日期
来源：http://hg.shxzskj.cn

Py:   d1 < d2;  d1 == d2
来源：http://hw.szxytkj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ht.szsharing.cn

JS:   d1.getTime() < d2.getTime()
来源：http://cy.521024.cn

TS:   d1.getTime() < d2.getTime()
来源：http://br.huixinmuqiang.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mh.newstarts.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://tg.hahajie.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ey.hahajie.cn

C#:   d1 < d2;  d1 == d2
来源：http://od.muxihuayi.cn

[J08] 提取年月日与星期
来源：http://nw.newstarts.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ov.colortex.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://jw.shtwfgs.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://vb.9csxet.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://lg.haigaiapp.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mb.szsharing.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://tc.huixiangedu.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://cw.bjjhwx.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wr.huixinmuqiang.cn

[J09] 时区处理
来源：http://es.shtwfgs.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ot.jctech888.com.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://lq.bookmarksfly.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ad.gzmigu.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://av.shtwfgs.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ck.colortex.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qm.huixiangedu.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://hs.hahajie.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://yi.muxihuayi.cn

[J10] 取今天 / 本月第一天
来源：http://mo.nicolike.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://bc.shxzskj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://pf.shxzukj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://jv.szxytkj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://id.shxzskj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xs.asd995.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ed.szxytkj.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://fb.shxzukj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://po.shxzskj.cn

================================================================================
来源：http://hh.colortex.cn

K. JSON 与序列化
来源：http://or.asd995.cn

================================================================================
来源：http://be.huixiangedu.cn

[K01] 对象转 JSON 字符串
来源：http://ok.yuntaijiaju.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ib.521024.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://dl.colortex.cn

JS:   JSON.stringify(obj)
来源：http://nx.shxzskj.cn

TS:   JSON.stringify(obj)
来源：http://hs.newstarts.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://bj.9csxet.cn

Go:   json.Marshal(obj)
来源：http://ve.lnxyls.cn

Ruby: obj.to_json                                     // require "json"
来源：http://at.szxytkj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ok.asd995.cn

[K02] JSON 字符串转对象
来源：http://sv.nszjky.cn

Py:   json.loads(s)
来源：http://by.shtwfgs.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://he.chemitech.net.cn

JS:   JSON.parse(s)
来源：http://xm.yuntaijiaju.cn

TS:   JSON.parse(s)
来源：http://av.jianghongdianzi.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://uf.wgjwhj.cn

Go:   json.Unmarshal(data, &v)
来源：http://es.colortex.cn

Ruby: JSON.parse(s)
来源：http://io.bookmarksfly.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://tj.nicolike.cn

[K03] JSON 美化输出（带缩进）
来源：http://ld.nicolike.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://qv.huixinmuqiang.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://nc.asd995.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://il.yuexingan06.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://yz.jctech888.com.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://kk.newstarts.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ky.yuexingan06.cn

Ruby: JSON.pretty_generate(obj)
来源：http://qn.lnxyls.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://pc.shxzukj.cn

[K04] 读取 JSON 文件
来源：http://wd.9csxet.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jq.hnjuh.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://di.lnxyls.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ft.shxzskj.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://te.yuntaijiaju.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://iy.yuntaijiaju.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://rw.huixiangedu.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://xg.nszjky.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://yq.yuexingan06.cn

[K05] 深拷贝对象
来源：http://bp.shxzukj.cn

Py:   copy.deepcopy(obj)
来源：http://eo.9csxet.cn

PHP:  unserialize(serialize($obj));
来源：http://uy.nszjky.cn

JS:   structuredClone(obj)
来源：http://fh.haigaiapp.cn

TS:   structuredClone(obj)
来源：http://cc.chemitech.net.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://yh.muxihuayi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://fo.nicolike.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://bf.wgjwhj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://qt.newstarts.cn

[K06] 解析 URL 查询串
来源：http://gk.shxzukj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mm.chemitech.net.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://eo.shxzukj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yf.huixinmuqiang.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fo.huanxung.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://fg.shtwfgs.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://hf.bookmarksfly.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://im.nszjky.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://fr.chemitech.net.cn

[K07] 进制转换
来源：http://wq.shtwfgs.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://aj.shxzukj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://qg.colortex.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ez.jctech888.com.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://oa.haigaiapp.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wy.bjjhwx.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ub.gzmigu.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://xr.huanxung.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ck.nicolike.cn

[K08] 二进制序列化（非 JSON）
来源：http://xb.huixinmuqiang.cn

Py:   pickle.dumps(obj)
来源：http://jj.nicolike.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://vl.gzmigu.cn

JS:   v8.serialize(obj)        // Node
来源：http://gs.shxzskj.cn

TS:   v8.serialize(obj)        // Node
来源：http://dt.panjiajie.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://um.bookmarksfly.cn

Go:   encoding/gob
来源：http://rm.521024.cn

Ruby: Marshal.dump(obj)
来源：http://of.jctech888.com.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://vz.colortex.cn

================================================================================
来源：http://fk.9csxet.cn

L. 网络请求
来源：http://qw.haigaiapp.cn

================================================================================
来源：http://uu.521024.cn

[L01] 发送 GET 请求
来源：http://vm.nicolike.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://iq.chemitech.net.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://um.asd995.cn

JS:   await fetch(url)
来源：http://mx.shtwfgs.cn

TS:   await fetch(url)
来源：http://rj.huixiangedu.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://nq.wgjwhj.cn

Go:   resp, err := http.Get(url)
来源：http://zz.521024.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://gz.bookmarksfly.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://yx.wgjwhj.cn

[L02] 发送 POST JSON
来源：http://kc.szsharing.cn

Py:   requests.post(url, json={"a": 1})
来源：http://wj.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://sb.jianghongdianzi.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yb.9csxet.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ri.chemitech.net.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://yl.jctech888.com.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jj.szsharing.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://yu.panjiajie.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://gt.shxzukj.cn

[L03] 设置自定义请求头
来源：http://zz.9csxet.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mv.szsharing.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ei.newstarts.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lu.bjjhwx.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mt.chemitech.net.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://si.huixiangedu.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ph.jianghongdianzi.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ul.shtwfgs.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ko.nicolike.cn

[L04] 设置超时
来源：http://cz.hnjuh.cn

Py:   requests.get(url, timeout=5)
来源：http://wn.hnjuh.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://vq.muxihuayi.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hh.huixiangedu.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ea.shtwfgs.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://gm.asd995.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ib.szxytkj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://lz.chemitech.net.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://xr.nszjky.cn

[L05] 上传文件（multipart）
来源：http://qi.jianghongdianzi.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://go.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://fh.yuexingan06.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qg.yuexingan06.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ye.gzmigu.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ec.521024.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://qg.huixiangedu.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mh.nszjky.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://le.shtwfgs.cn

[L06] 解析响应为 JSON
来源：http://xw.jianghongdianzi.cn

Py:   resp.json()
来源：http://sq.haigaiapp.cn

PHP:  json_decode($body, true);
来源：http://yf.panjiajie.cn

JS:   await resp.json()
来源：http://qi.yuntaijiaju.cn

TS:   await resp.json()
来源：http://tz.szxytkj.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://yj.shtwfgs.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wr.huanxung.cn

Ruby: JSON.parse(resp.body)
来源：http://qt.panjiajie.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://gl.yuexingan06.cn

[L07] 处理 HTTP 状态码
来源：http://ns.shxzskj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mk.nszjky.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://dv.nicolike.cn

JS:   resp.ok;  resp.status
来源：http://au.hnjuh.cn

TS:   resp.ok;  resp.status
来源：http://eq.colortex.cn

Java: resp.statusCode()
来源：http://zj.newstarts.cn

Go:   resp.StatusCode
来源：http://tk.colortex.cn

Ruby: resp.code.to_i
来源：http://vk.9csxet.cn

C#:   (int)resp.StatusCode
来源：http://ee.szsharing.cn

[L08] 并发请求多个地址
来源：http://hd.chemitech.net.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://js.asd995.cn

PHP:  curl_multi_init() 系列
来源：http://qi.chemitech.net.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ru.szxytkj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ph.jctech888.com.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mo.shxzukj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://oe.shxzskj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://my.wgjwhj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://tq.bookmarksfly.cn

================================================================================
来源：http://mt.szxytkj.cn

M. 命令行 / 进程 / 环境
来源：http://xs.wgjwhj.cn

================================================================================
来源：http://jh.haigaiapp.cn

[M01] 读取命令行参数
来源：http://ib.yuntaijiaju.cn

Py:   sys.argv[1:]
来源：http://uk.gzmigu.cn

PHP:  $argv;  $argc;
来源：http://xy.hnjuh.cn

JS:   process.argv.slice(2)
来源：http://ka.jctech888.com.cn

TS:   process.argv.slice(2)
来源：http://dy.gzmigu.cn

Java: args 数组（main 方法参数）
来源：http://xx.colortex.cn

Go:   os.Args[1:]
来源：http://al.521024.cn

Ruby: ARGV
来源：http://hn.szsharing.cn

C#:   args 数组（Main 方法参数）
来源：http://vi.bjjhwx.cn

[M02] 读取环境变量
来源：http://uv.hnjuh.cn

Py:   os.environ.get("HOME")
来源：http://aa.chemitech.net.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://oa.chemitech.net.cn

JS:   process.env.HOME
来源：http://hu.huixinmuqiang.cn

TS:   process.env.HOME
来源：http://wd.szxytkj.cn

Java: System.getenv("HOME")
来源：http://ev.huixinmuqiang.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mp.jianghongdianzi.cn

Ruby: ENV["HOME"]
来源：http://ic.chemitech.net.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ko.huanxung.cn

[M03] 执行外部命令
来源：http://vf.asd995.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://fx.shxzukj.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://rc.nszjky.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://oe.shxzskj.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://yr.shxzskj.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ei.shxzskj.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://gz.shxzukj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://dv.chemitech.net.cn

C#:   Process.Start("ls", "-l");
来源：http://rl.colortex.cn

[M04] 获取当前工作目录
来源：http://rw.nszjky.cn

Py:   os.getcwd()
来源：http://kx.lnxyls.cn

PHP:  getcwd();
来源：http://df.huanxung.cn

JS:   process.cwd()
来源：http://mo.szxytkj.cn

TS:   process.cwd()
来源：http://ql.hahajie.cn

Java: Path.of("").toAbsolutePath()
来源：http://lb.panjiajie.cn

Go:   os.Getwd()
来源：http://yh.newstarts.cn

Ruby: Dir.pwd
来源：http://lg.nicolike.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ca.hahajie.cn

[M05] 设置退出码
来源：http://ts.huixiangedu.cn

Py:   sys.exit(1)
来源：http://pu.hnjuh.cn

PHP:  exit(1);
来源：http://ge.yuexingan06.cn

JS:   process.exit(1)
来源：http://sd.nicolike.cn

TS:   process.exit(1)
来源：http://lk.asd995.cn

Java: System.exit(1)
来源：http://mj.nicolike.cn

Go:   os.Exit(1)
来源：http://qm.bookmarksfly.cn

Ruby: exit 1
来源：http://nt.gzmigu.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ji.chemitech.net.cn

[M06] 向标准错误输出
来源：http://mu.9csxet.cn

Py:   print("err", file=sys.stderr)
来源：http://yz.szxytkj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://dr.wgjwhj.cn

JS:   console.error("err")
来源：http://jy.huanxung.cn

TS:   console.error("err")
来源：http://mp.shxzskj.cn

Java: System.err.println("err")
来源：http://lf.shxzukj.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://tc.bjjhwx.cn

Ruby: warn "err"
来源：http://nq.haigaiapp.cn

C#:   Console.Error.WriteLine("err")
来源：http://xx.9csxet.cn

[M07] 判断是否为主入口
来源：http://pd.hnjuh.cn

Py:   if __name__ == "__main__":
来源：http://kx.jctech888.com.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://bx.szxytkj.cn

JS:   require.main === module
来源：http://bm.shxzukj.cn

TS:   require.main === module
来源：http://vw.szsharing.cn

Java: public static void main(String[] args)
来源：http://vj.colortex.cn

Go:   func main()
来源：http://hh.hnjuh.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://yb.521024.cn

C#:   static void Main(string[] args)
来源：http://dd.shxzukj.cn

[M08] 获取系统与运行时信息
来源：http://js.521024.cn

Py:   platform.system();  platform.python_version()
来源：http://sb.hnjuh.cn

PHP:  PHP_OS;  phpversion();
来源：http://xy.colortex.cn

JS:   process.platform;  process.version
来源：http://ip.gzmigu.cn

TS:   process.platform;  process.version
来源：http://yk.shxzskj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://bb.yuexingan06.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://uv.szxytkj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ps.hahajie.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://zi.newstarts.cn

================================================================================
来源：http://tv.chemitech.net.cn

N. 数据结构与算法
来源：http://sv.huanxung.cn

================================================================================
来源：http://cn.asd995.cn

[N01] 二分查找（有序数组）
来源：http://em.jctech888.com.cn

Py:   bisect.bisect_left(arr, x)
来源：http://vn.jctech888.com.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://nz.szxytkj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vy.newstarts.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rj.shxzukj.cn

Java: Arrays.binarySearch(arr, x)
来源：http://xn.bjjhwx.cn

Go:   sort.SearchInts(arr, x)
来源：http://av.szsharing.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://tt.muxihuayi.cn

C#:   Array.BinarySearch(arr, x)
来源：http://cg.huixiangedu.cn

[N02] 排序（工程实践用内置实现）
来源：http://rk.panjiajie.cn

Py:   sorted(arr);  arr.sort()
来源：http://ic.shxzskj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://gf.lnxyls.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://xg.nicolike.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://cy.yuexingan06.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ao.shxzukj.cn

Go:   slices.Sort(arr)
来源：http://gg.bjjhwx.cn

Ruby: arr.sort
来源：http://ah.huixinmuqiang.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://wi.hahajie.cn

[N03] 快速排序（分治示例）
来源：http://pd.haigaiapp.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://jn.muxihuayi.cn


<!-- 参考信息 -->