代发 wailian999

Py:   (end - start).total_seconds()
来源：http://bj.asd995.cn

PHP:  $end->diff($start)->days;
来源：http://yl.yuntaijiaju.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://dk.wgjwhj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://tk.newstarts.cn

Java: Duration.between(start, end).toSeconds()
来源：http://wd.shxzskj.cn

Go:   end.Sub(start).Hours()
来源：http://vb.wgjwhj.cn

Ruby: end - start                 # 返回秒数
来源：http://hd.hnjuh.cn

C#:   (end - start).TotalSeconds
来源：http://sf.shxzukj.cn

[J07] 比较两个日期
来源：http://lg.shxzukj.cn

Py:   d1 < d2;  d1 == d2
来源：http://zm.shxzskj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://nv.jianghongdianzi.cn

JS:   d1.getTime() < d2.getTime()
来源：http://yl.szxytkj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://gp.huixinmuqiang.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://dn.shxzskj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://sx.huixinmuqiang.cn

Ruby: d1 < d2;  d1 == d2
来源：http://qq.gzmigu.cn

C#:   d1 < d2;  d1 == d2
来源：http://le.haigaiapp.cn

[J08] 提取年月日与星期
来源：http://nf.szsharing.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://bw.9csxet.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ap.shtwfgs.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://kz.hahajie.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://sq.hnjuh.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://bk.shtwfgs.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://py.lnxyls.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://nq.yuexingan06.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://no.shtwfgs.cn

[J09] 时区处理
来源：http://tv.gzmigu.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://xh.shxzukj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://kw.shxzskj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vl.yuntaijiaju.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zk.muxihuayi.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://dq.jianghongdianzi.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xv.bjjhwx.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://if.wgjwhj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://tp.muxihuayi.cn

[J10] 取今天 / 本月第一天
来源：http://qb.wgjwhj.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://cj.szxytkj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://lo.hnjuh.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://lh.hnjuh.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wr.yuntaijiaju.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://jc.asd995.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://tm.bjjhwx.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://qf.yuntaijiaju.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://of.yuntaijiaju.cn

================================================================================
来源：http://ae.gzmigu.cn

K. JSON 与序列化
来源：http://td.asd995.cn

================================================================================
来源：http://qn.chemitech.net.cn

[K01] 对象转 JSON 字符串
来源：http://eu.jctech888.com.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ht.yuexingan06.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://bw.szxytkj.cn

JS:   JSON.stringify(obj)
来源：http://jl.haigaiapp.cn

TS:   JSON.stringify(obj)
来源：http://ct.yuexingan06.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://pr.chemitech.net.cn

Go:   json.Marshal(obj)
来源：http://iy.9csxet.cn

Ruby: obj.to_json                                     // require "json"
来源：http://gh.huixinmuqiang.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ol.yuexingan06.cn

[K02] JSON 字符串转对象
来源：http://sk.jianghongdianzi.cn

Py:   json.loads(s)
来源：http://fc.nszjky.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://iz.shtwfgs.cn

JS:   JSON.parse(s)
来源：http://ma.shxzskj.cn

TS:   JSON.parse(s)
来源：http://kk.newstarts.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jf.nicolike.cn

Go:   json.Unmarshal(data, &v)
来源：http://hu.jctech888.com.cn

Ruby: JSON.parse(s)
来源：http://wq.newstarts.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://rg.yuntaijiaju.cn

[K03] JSON 美化输出（带缩进）
来源：http://tz.muxihuayi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ma.bookmarksfly.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://jw.lnxyls.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://of.nszjky.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://gh.huixiangedu.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://su.521024.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mq.bjjhwx.cn

Ruby: JSON.pretty_generate(obj)
来源：http://dh.muxihuayi.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://lm.panjiajie.cn

[K04] 读取 JSON 文件
来源：http://il.haigaiapp.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://cf.shxzukj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://dg.yuexingan06.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sa.haigaiapp.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hg.huanxung.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://tu.huanxung.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://jb.huanxung.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ky.bookmarksfly.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ji.9csxet.cn

[K05] 深拷贝对象
来源：http://fi.nszjky.cn

Py:   copy.deepcopy(obj)
来源：http://iu.newstarts.cn

PHP:  unserialize(serialize($obj));
来源：http://yo.yuexingan06.cn

JS:   structuredClone(obj)
来源：http://pm.yuexingan06.cn

TS:   structuredClone(obj)
来源：http://oj.shtwfgs.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://dr.huanxung.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://vv.nicolike.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ox.newstarts.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ns.jianghongdianzi.cn

[K06] 解析 URL 查询串
来源：http://hv.wgjwhj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://pr.bookmarksfly.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://kt.bookmarksfly.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rr.huanxung.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://op.jianghongdianzi.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://nh.huixiangedu.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://is.yuexingan06.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://yr.szsharing.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://vm.bjjhwx.cn

[K07] 进制转换
来源：http://jj.huixinmuqiang.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://kf.shxzskj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://rp.shxzskj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://nt.521024.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://gd.jianghongdianzi.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://gz.nszjky.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://vr.haigaiapp.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://lz.szxytkj.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://uq.huixiangedu.cn

[K08] 二进制序列化（非 JSON）
来源：http://qt.szxytkj.cn

Py:   pickle.dumps(obj)
来源：http://my.colortex.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.asd995.cn

JS:   v8.serialize(obj)        // Node
来源：http://ui.shxzukj.cn

TS:   v8.serialize(obj)        // Node
来源：http://ax.gzmigu.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mw.nszjky.cn

Go:   encoding/gob
来源：http://bo.hnjuh.cn

Ruby: Marshal.dump(obj)
来源：http://qd.nszjky.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ei.shxzukj.cn

================================================================================
来源：http://of.hahajie.cn

L. 网络请求
来源：http://ap.szxytkj.cn

================================================================================
来源：http://bb.bookmarksfly.cn

[L01] 发送 GET 请求
来源：http://by.muxihuayi.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://gr.bjjhwx.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://dz.wgjwhj.cn

JS:   await fetch(url)
来源：http://he.521024.cn

TS:   await fetch(url)
来源：http://lo.hahajie.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ia.huanxung.cn

Go:   resp, err := http.Get(url)
来源：http://in.wgjwhj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ut.szsharing.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://fi.nicolike.cn

[L02] 发送 POST JSON
来源：http://jg.lnxyls.cn

Py:   requests.post(url, json={"a": 1})
来源：http://jm.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://pi.9csxet.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jf.yuntaijiaju.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wv.chemitech.net.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ix.hnjuh.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://xh.haigaiapp.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://np.jctech888.com.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://uo.wgjwhj.cn

[L03] 设置自定义请求头
来源：http://oe.lnxyls.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://nz.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://on.shxzskj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ny.szxytkj.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hj.nicolike.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://xv.szsharing.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://bj.huixiangedu.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://cb.shxzukj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://eo.yuexingan06.cn

[L04] 设置超时
来源：http://eu.newstarts.cn

Py:   requests.get(url, timeout=5)
来源：http://gg.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://tm.lnxyls.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kt.yuntaijiaju.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vw.muxihuayi.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://rd.haigaiapp.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://bb.shtwfgs.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://gg.jianghongdianzi.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://bw.bjjhwx.cn

[L05] 上传文件（multipart）
来源：http://hf.hahajie.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://qk.hnjuh.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://iv.colortex.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://cv.jianghongdianzi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mk.chemitech.net.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://rh.jianghongdianzi.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://bc.9csxet.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://cc.shtwfgs.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ta.bjjhwx.cn

[L06] 解析响应为 JSON
来源：http://hm.huixinmuqiang.cn

Py:   resp.json()
来源：http://qg.lnxyls.cn

PHP:  json_decode($body, true);
来源：http://sf.panjiajie.cn

JS:   await resp.json()
来源：http://ad.muxihuayi.cn

TS:   await resp.json()
来源：http://ar.shtwfgs.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://rz.szsharing.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://fl.shtwfgs.cn

Ruby: JSON.parse(resp.body)
来源：http://dl.chemitech.net.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://fv.yuexingan06.cn

[L07] 处理 HTTP 状态码
来源：http://tq.wgjwhj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wd.huixiangedu.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://py.jctech888.com.cn

JS:   resp.ok;  resp.status
来源：http://gc.muxihuayi.cn

TS:   resp.ok;  resp.status
来源：http://bb.szxytkj.cn

Java: resp.statusCode()
来源：http://rn.jctech888.com.cn

Go:   resp.StatusCode
来源：http://wj.newstarts.cn

Ruby: resp.code.to_i
来源：http://ud.muxihuayi.cn

C#:   (int)resp.StatusCode
来源：http://nh.huixiangedu.cn

[L08] 并发请求多个地址
来源：http://jp.huixiangedu.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://yw.bjjhwx.cn

PHP:  curl_multi_init() 系列
来源：http://sh.gzmigu.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lp.asd995.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jy.shtwfgs.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://sa.nicolike.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://kk.hnjuh.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://pt.huixinmuqiang.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ps.panjiajie.cn

================================================================================
来源：http://qb.yuexingan06.cn

M. 命令行 / 进程 / 环境
来源：http://vg.colortex.cn

================================================================================
来源：http://fx.huixiangedu.cn

[M01] 读取命令行参数
来源：http://eu.yuexingan06.cn

Py:   sys.argv[1:]
来源：http://zj.gzmigu.cn

PHP:  $argv;  $argc;
来源：http://si.shxzskj.cn

JS:   process.argv.slice(2)
来源：http://sj.shxzskj.cn

TS:   process.argv.slice(2)
来源：http://uc.panjiajie.cn

Java: args 数组（main 方法参数）
来源：http://rh.jctech888.com.cn

Go:   os.Args[1:]
来源：http://ne.gzmigu.cn

Ruby: ARGV
来源：http://jz.huixinmuqiang.cn

C#:   args 数组（Main 方法参数）
来源：http://ki.huixiangedu.cn

[M02] 读取环境变量
来源：http://me.nicolike.cn

Py:   os.environ.get("HOME")
来源：http://ps.nszjky.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mi.shxzskj.cn

JS:   process.env.HOME
来源：http://ch.lnxyls.cn

TS:   process.env.HOME
来源：http://ug.bjjhwx.cn

Java: System.getenv("HOME")
来源：http://es.haigaiapp.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ib.asd995.cn

Ruby: ENV["HOME"]
来源：http://zj.shxzukj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ax.521024.cn

[M03] 执行外部命令
来源：http://si.9csxet.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://yp.colortex.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wl.shtwfgs.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://zt.jctech888.com.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://id.nszjky.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://dn.huixiangedu.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://nu.hahajie.cn

Ruby: system("ls -l");  `ls -l`
来源：http://uw.wgjwhj.cn

C#:   Process.Start("ls", "-l");
来源：http://qc.yuntaijiaju.cn

[M04] 获取当前工作目录
来源：http://if.9csxet.cn

Py:   os.getcwd()
来源：http://pj.bookmarksfly.cn

PHP:  getcwd();
来源：http://uh.chemitech.net.cn

JS:   process.cwd()
来源：http://mz.newstarts.cn

TS:   process.cwd()
来源：http://zd.shxzukj.cn

Java: Path.of("").toAbsolutePath()
来源：http://ma.wgjwhj.cn

Go:   os.Getwd()
来源：http://hk.shxzukj.cn

Ruby: Dir.pwd
来源：http://zu.muxihuayi.cn

C#:   Directory.GetCurrentDirectory()
来源：http://vw.huixiangedu.cn

[M05] 设置退出码
来源：http://ym.huanxung.cn

Py:   sys.exit(1)
来源：http://ad.szxytkj.cn

PHP:  exit(1);
来源：http://tl.szsharing.cn

JS:   process.exit(1)
来源：http://zr.huanxung.cn

TS:   process.exit(1)
来源：http://jy.shtwfgs.cn

Java: System.exit(1)
来源：http://hc.lnxyls.cn

Go:   os.Exit(1)
来源：http://zn.panjiajie.cn

Ruby: exit 1
来源：http://tt.yuntaijiaju.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://kk.lnxyls.cn

[M06] 向标准错误输出
来源：http://xm.szxytkj.cn

Py:   print("err", file=sys.stderr)
来源：http://ri.huixinmuqiang.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://pp.huixinmuqiang.cn

JS:   console.error("err")
来源：http://yo.9csxet.cn

TS:   console.error("err")
来源：http://ko.jianghongdianzi.cn

Java: System.err.println("err")
来源：http://mq.jctech888.com.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://vv.shxzskj.cn

Ruby: warn "err"
来源：http://ip.yuexingan06.cn

C#:   Console.Error.WriteLine("err")
来源：http://jp.szsharing.cn

[M07] 判断是否为主入口
来源：http://qs.asd995.cn

Py:   if __name__ == "__main__":
来源：http://im.jctech888.com.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ap.gzmigu.cn

JS:   require.main === module
来源：http://mi.lnxyls.cn

TS:   require.main === module
来源：http://be.hnjuh.cn

Java: public static void main(String[] args)
来源：http://pg.szxytkj.cn

Go:   func main()
来源：http://lf.yuntaijiaju.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mq.nszjky.cn

C#:   static void Main(string[] args)
来源：http://qg.bjjhwx.cn

[M08] 获取系统与运行时信息
来源：http://xs.yuntaijiaju.cn

Py:   platform.system();  platform.python_version()
来源：http://jx.hnjuh.cn

PHP:  PHP_OS;  phpversion();
来源：http://iq.bjjhwx.cn

JS:   process.platform;  process.version
来源：http://vd.521024.cn

TS:   process.platform;  process.version
来源：http://jy.lnxyls.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ag.newstarts.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://hb.wgjwhj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://rd.nicolike.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://xi.hahajie.cn

================================================================================
来源：http://yd.szsharing.cn

N. 数据结构与算法
来源：http://ng.haigaiapp.cn

================================================================================
来源：http://wk.shxzukj.cn

[N01] 二分查找（有序数组）
来源：http://ls.bjjhwx.cn

Py:   bisect.bisect_left(arr, x)
来源：http://bq.hnjuh.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://dv.jianghongdianzi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gg.hnjuh.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zo.jianghongdianzi.cn

Java: Arrays.binarySearch(arr, x)
来源：http://wd.bjjhwx.cn

Go:   sort.SearchInts(arr, x)
来源：http://gh.jctech888.com.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://aa.colortex.cn

C#:   Array.BinarySearch(arr, x)
来源：http://id.9csxet.cn

[N02] 排序（工程实践用内置实现）
来源：http://dl.9csxet.cn

Py:   sorted(arr);  arr.sort()
来源：http://ym.jianghongdianzi.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wd.bookmarksfly.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://nf.yuexingan06.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://da.jianghongdianzi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ry.szxytkj.cn

Go:   slices.Sort(arr)
来源：http://oo.hnjuh.cn

Ruby: arr.sort
来源：http://in.huanxung.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://uy.nszjky.cn

[N03] 快速排序（分治示例）
来源：http://yw.huixiangedu.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://vv.colortex.cn

PHP:  // 递归实现，或用 usort
来源：http://ge.jianghongdianzi.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wa.lnxyls.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pz.shxzskj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://sq.shxzukj.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://rs.shtwfgs.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://gv.wgjwhj.cn

C#:   // 手写递归，或 Array.Sort
来源：http://nu.shxzskj.cn

[N04] 斐波那契数列
来源：http://zy.gzmigu.cn


<!-- 参考信息 -->