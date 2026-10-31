代发 wailian999

Py:   (end - start).total_seconds()
来源：http://cr.huanxung.cn

PHP:  $end->diff($start)->days;
来源：http://js.hnjuh.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ea.lnxyls.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://tg.huixinmuqiang.cn

Java: Duration.between(start, end).toSeconds()
来源：http://dy.newstarts.cn

Go:   end.Sub(start).Hours()
来源：http://vh.shtwfgs.cn

Ruby: end - start                 # 返回秒数
来源：http://zc.jianghongdianzi.cn

C#:   (end - start).TotalSeconds
来源：http://vx.9csxet.cn

[J07] 比较两个日期
来源：http://bd.newstarts.cn

Py:   d1 < d2;  d1 == d2
来源：http://tx.yuexingan06.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://eg.nszjky.cn

JS:   d1.getTime() < d2.getTime()
来源：http://lr.9csxet.cn

TS:   d1.getTime() < d2.getTime()
来源：http://fp.jctech888.com.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mv.panjiajie.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://fv.yuntaijiaju.cn

Ruby: d1 < d2;  d1 == d2
来源：http://qw.hnjuh.cn

C#:   d1 < d2;  d1 == d2
来源：http://jk.jctech888.com.cn

[J08] 提取年月日与星期
来源：http://po.asd995.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://pt.shxzskj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ah.nicolike.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://tg.huixiangedu.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://uq.newstarts.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://br.bjjhwx.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://cz.yuexingan06.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ar.bookmarksfly.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://iz.521024.cn

[J09] 时区处理
来源：http://st.wgjwhj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://tc.wgjwhj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://fi.521024.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pv.huanxung.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ms.521024.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://xu.jianghongdianzi.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://jk.shtwfgs.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://pf.shxzskj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://zb.szxytkj.cn

[J10] 取今天 / 本月第一天
来源：http://bf.9csxet.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ho.asd995.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://qx.521024.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://tl.yuexingan06.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://cw.wgjwhj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://pe.asd995.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://rp.shxzskj.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ny.nicolike.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://cq.shxzskj.cn

================================================================================
来源：http://eh.hnjuh.cn

K. JSON 与序列化
来源：http://fv.colortex.cn

================================================================================
来源：http://gy.szxytkj.cn

[K01] 对象转 JSON 字符串
来源：http://hi.hnjuh.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://za.szxytkj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://us.yuexingan06.cn

JS:   JSON.stringify(obj)
来源：http://dw.yuntaijiaju.cn

TS:   JSON.stringify(obj)
来源：http://in.bjjhwx.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://jd.shxzskj.cn

Go:   json.Marshal(obj)
来源：http://zk.jianghongdianzi.cn

Ruby: obj.to_json                                     // require "json"
来源：http://gj.shxzskj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://rq.jianghongdianzi.cn

[K02] JSON 字符串转对象
来源：http://ni.muxihuayi.cn

Py:   json.loads(s)
来源：http://tn.wgjwhj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://qo.shxzskj.cn

JS:   JSON.parse(s)
来源：http://xm.nszjky.cn

TS:   JSON.parse(s)
来源：http://wa.muxihuayi.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ne.newstarts.cn

Go:   json.Unmarshal(data, &v)
来源：http://oy.hahajie.cn

Ruby: JSON.parse(s)
来源：http://xv.wgjwhj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://xl.huanxung.cn

[K03] JSON 美化输出（带缩进）
来源：http://va.bookmarksfly.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://yk.asd995.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mc.yuexingan06.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://zc.szsharing.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://uq.521024.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://pv.chemitech.net.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://uo.huixinmuqiang.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ij.colortex.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ol.yuntaijiaju.cn

[K04] 读取 JSON 文件
来源：http://kx.huixinmuqiang.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://uj.shtwfgs.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://nu.haigaiapp.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://km.gzmigu.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pn.9csxet.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://oa.hnjuh.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://fb.hahajie.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://pv.panjiajie.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://vs.hahajie.cn

[K05] 深拷贝对象
来源：http://ij.jctech888.com.cn

Py:   copy.deepcopy(obj)
来源：http://fk.szsharing.cn

PHP:  unserialize(serialize($obj));
来源：http://xl.shxzskj.cn

JS:   structuredClone(obj)
来源：http://uw.szxytkj.cn

TS:   structuredClone(obj)
来源：http://if.huixinmuqiang.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://kx.newstarts.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://iz.shxzskj.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://jd.yuexingan06.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://hm.chemitech.net.cn

[K06] 解析 URL 查询串
来源：http://sa.gzmigu.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://jk.panjiajie.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://pd.panjiajie.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bw.hahajie.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ye.nszjky.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wd.szsharing.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://xs.szxytkj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vz.huixinmuqiang.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://iz.jctech888.com.cn

[K07] 进制转换
来源：http://ot.huanxung.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://vo.shtwfgs.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://tz.asd995.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://yl.nicolike.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://rn.521024.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://yf.huixinmuqiang.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ov.bjjhwx.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hv.9csxet.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://kq.jianghongdianzi.cn

[K08] 二进制序列化（非 JSON）
来源：http://qa.colortex.cn

Py:   pickle.dumps(obj)
来源：http://cv.chemitech.net.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://nb.hnjuh.cn

JS:   v8.serialize(obj)        // Node
来源：http://bw.szxytkj.cn

TS:   v8.serialize(obj)        // Node
来源：http://zk.hahajie.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://se.panjiajie.cn

Go:   encoding/gob
来源：http://vv.yuntaijiaju.cn

Ruby: Marshal.dump(obj)
来源：http://se.lnxyls.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://rz.muxihuayi.cn

================================================================================
来源：http://hm.asd995.cn

L. 网络请求
来源：http://iy.colortex.cn

================================================================================
来源：http://me.gzmigu.cn

[L01] 发送 GET 请求
来源：http://fq.szxytkj.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xl.lnxyls.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ec.wgjwhj.cn

JS:   await fetch(url)
来源：http://io.huixiangedu.cn

TS:   await fetch(url)
来源：http://pv.muxihuayi.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ch.bookmarksfly.cn

Go:   resp, err := http.Get(url)
来源：http://cf.hahajie.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://jx.yuexingan06.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ot.colortex.cn

[L02] 发送 POST JSON
来源：http://jv.szxytkj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://jb.panjiajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hm.nicolike.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pf.nicolike.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qj.yuexingan06.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://bh.haigaiapp.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://be.jctech888.com.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://aq.bookmarksfly.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://yr.huixinmuqiang.cn

[L03] 设置自定义请求头
来源：http://ia.shtwfgs.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://zy.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://zq.gzmigu.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vu.szxytkj.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fz.chemitech.net.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://aq.huanxung.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://cd.huixinmuqiang.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://bn.nicolike.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://av.asd995.cn

[L04] 设置超时
来源：http://hu.nicolike.cn

Py:   requests.get(url, timeout=5)
来源：http://ks.szxytkj.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://pc.521024.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wk.panjiajie.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ya.huixiangedu.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://dg.jianghongdianzi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hj.newstarts.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ul.asd995.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://zw.huanxung.cn

[L05] 上传文件（multipart）
来源：http://ym.lnxyls.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hi.haigaiapp.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://aw.nicolike.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ut.huanxung.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://jp.yuntaijiaju.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://pr.jianghongdianzi.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://zm.panjiajie.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ln.lnxyls.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hj.nszjky.cn

[L06] 解析响应为 JSON
来源：http://du.bjjhwx.cn

Py:   resp.json()
来源：http://qq.hnjuh.cn

PHP:  json_decode($body, true);
来源：http://fo.hahajie.cn

JS:   await resp.json()
来源：http://pq.hahajie.cn

TS:   await resp.json()
来源：http://vk.colortex.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://gv.hahajie.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ot.panjiajie.cn

Ruby: JSON.parse(resp.body)
来源：http://rc.haigaiapp.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://jh.nicolike.cn

[L07] 处理 HTTP 状态码
来源：http://kv.huanxung.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://qp.gzmigu.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ok.shxzukj.cn

JS:   resp.ok;  resp.status
来源：http://wo.9csxet.cn

TS:   resp.ok;  resp.status
来源：http://bv.hahajie.cn

Java: resp.statusCode()
来源：http://yv.szxytkj.cn

Go:   resp.StatusCode
来源：http://mc.huanxung.cn

Ruby: resp.code.to_i
来源：http://km.shxzskj.cn

C#:   (int)resp.StatusCode
来源：http://su.shxzskj.cn

[L08] 并发请求多个地址
来源：http://yi.shxzukj.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://vc.shxzukj.cn

PHP:  curl_multi_init() 系列
来源：http://fk.gzmigu.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jl.huanxung.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rr.nicolike.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ky.asd995.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://fj.521024.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://gf.jctech888.com.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://fq.lnxyls.cn

================================================================================
来源：http://tg.jianghongdianzi.cn

M. 命令行 / 进程 / 环境
来源：http://it.shtwfgs.cn

================================================================================
来源：http://xd.bookmarksfly.cn

[M01] 读取命令行参数
来源：http://mx.shxzskj.cn

Py:   sys.argv[1:]
来源：http://fc.gzmigu.cn

PHP:  $argv;  $argc;
来源：http://fb.hnjuh.cn

JS:   process.argv.slice(2)
来源：http://xq.jctech888.com.cn

TS:   process.argv.slice(2)
来源：http://ow.newstarts.cn

Java: args 数组（main 方法参数）
来源：http://cu.huanxung.cn

Go:   os.Args[1:]
来源：http://cq.huixinmuqiang.cn

Ruby: ARGV
来源：http://oe.szxytkj.cn

C#:   args 数组（Main 方法参数）
来源：http://om.yuexingan06.cn

[M02] 读取环境变量
来源：http://pm.gzmigu.cn

Py:   os.environ.get("HOME")
来源：http://rx.jianghongdianzi.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://uc.jianghongdianzi.cn

JS:   process.env.HOME
来源：http://yj.bookmarksfly.cn

TS:   process.env.HOME
来源：http://dg.shxzskj.cn

Java: System.getenv("HOME")
来源：http://fp.lnxyls.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wg.gzmigu.cn

Ruby: ENV["HOME"]
来源：http://fp.yuexingan06.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://yy.huixinmuqiang.cn

[M03] 执行外部命令
来源：http://eo.huixinmuqiang.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://au.hahajie.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://aw.yuntaijiaju.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://us.muxihuayi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ql.hnjuh.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://uq.nszjky.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ms.szxytkj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ss.yuexingan06.cn

C#:   Process.Start("ls", "-l");
来源：http://sz.hnjuh.cn

[M04] 获取当前工作目录
来源：http://lm.shxzskj.cn

Py:   os.getcwd()
来源：http://wi.panjiajie.cn

PHP:  getcwd();
来源：http://py.jctech888.com.cn

JS:   process.cwd()
来源：http://hm.panjiajie.cn

TS:   process.cwd()
来源：http://te.colortex.cn

Java: Path.of("").toAbsolutePath()
来源：http://na.muxihuayi.cn

Go:   os.Getwd()
来源：http://ay.szxytkj.cn

Ruby: Dir.pwd
来源：http://ra.yuexingan06.cn

C#:   Directory.GetCurrentDirectory()
来源：http://di.521024.cn

[M05] 设置退出码
来源：http://xf.hnjuh.cn

Py:   sys.exit(1)
来源：http://nj.newstarts.cn

PHP:  exit(1);
来源：http://zo.asd995.cn

JS:   process.exit(1)
来源：http://rj.shtwfgs.cn

TS:   process.exit(1)
来源：http://hw.szxytkj.cn

Java: System.exit(1)
来源：http://cr.shxzukj.cn

Go:   os.Exit(1)
来源：http://vn.nicolike.cn

Ruby: exit 1
来源：http://jw.yuexingan06.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://nk.wgjwhj.cn

[M06] 向标准错误输出
来源：http://vv.jctech888.com.cn

Py:   print("err", file=sys.stderr)
来源：http://xa.newstarts.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://tn.hnjuh.cn

JS:   console.error("err")
来源：http://xw.jctech888.com.cn

TS:   console.error("err")
来源：http://dw.szsharing.cn

Java: System.err.println("err")
来源：http://dl.hahajie.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://dk.shtwfgs.cn

Ruby: warn "err"
来源：http://hg.chemitech.net.cn

C#:   Console.Error.WriteLine("err")
来源：http://gz.bjjhwx.cn

[M07] 判断是否为主入口
来源：http://zt.shtwfgs.cn

Py:   if __name__ == "__main__":
来源：http://nu.lnxyls.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://cc.haigaiapp.cn

JS:   require.main === module
来源：http://ab.yuntaijiaju.cn

TS:   require.main === module
来源：http://ie.yuexingan06.cn

Java: public static void main(String[] args)
来源：http://kw.lnxyls.cn

Go:   func main()
来源：http://lq.nszjky.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://pn.nicolike.cn

C#:   static void Main(string[] args)
来源：http://yg.szxytkj.cn

[M08] 获取系统与运行时信息
来源：http://uk.yuntaijiaju.cn

Py:   platform.system();  platform.python_version()
来源：http://lu.yuexingan06.cn

PHP:  PHP_OS;  phpversion();
来源：http://wo.gzmigu.cn

JS:   process.platform;  process.version
来源：http://ox.szsharing.cn

TS:   process.platform;  process.version
来源：http://ys.huixinmuqiang.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hn.szsharing.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://gn.yuntaijiaju.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://fp.bjjhwx.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://rg.lnxyls.cn

================================================================================
来源：http://tj.shxzukj.cn

N. 数据结构与算法
来源：http://ju.hnjuh.cn

================================================================================
来源：http://eh.hnjuh.cn

[N01] 二分查找（有序数组）
来源：http://rk.huanxung.cn

Py:   bisect.bisect_left(arr, x)
来源：http://zm.yuexingan06.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://gl.haigaiapp.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://np.muxihuayi.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nd.bookmarksfly.cn

Java: Arrays.binarySearch(arr, x)
来源：http://gz.szxytkj.cn

Go:   sort.SearchInts(arr, x)
来源：http://nc.asd995.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://hc.shtwfgs.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ju.jctech888.com.cn

[N02] 排序（工程实践用内置实现）
来源：http://vt.yuntaijiaju.cn

Py:   sorted(arr);  arr.sort()
来源：http://va.newstarts.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://bg.jianghongdianzi.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://fe.jctech888.com.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://oh.szsharing.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wy.nszjky.cn

Go:   slices.Sort(arr)
来源：http://me.nszjky.cn

Ruby: arr.sort
来源：http://dm.szxytkj.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ug.lnxyls.cn

[N03] 快速排序（分治示例）
来源：http://im.yuexingan06.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://qj.huixinmuqiang.cn

PHP:  // 递归实现，或用 usort
来源：http://gv.muxihuayi.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://th.yuexingan06.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ol.jianghongdianzi.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ls.9csxet.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://xb.shxzukj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wc.hahajie.cn

C#:   // 手写递归，或 Array.Sort
来源：http://eb.szsharing.cn

[N04] 斐波那契数列
来源：http://rm.hnjuh.cn


<!-- 参考信息 -->