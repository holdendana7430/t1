代发 wailian999

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wp.bookmarksfly.cn

Ruby: Time.now + 7 * 86400
来源：http://dg.hahajie.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ei.shxzukj.cn

[J06] 计算两时间之差
来源：http://ry.huanxung.cn

Py:   (end - start).total_seconds()
来源：http://et.hnjuh.cn

PHP:  $end->diff($start)->days;
来源：http://hm.shxzukj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://au.chemitech.net.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ur.gzmigu.cn

Java: Duration.between(start, end).toSeconds()
来源：http://rt.521024.cn

Go:   end.Sub(start).Hours()
来源：http://wd.colortex.cn

Ruby: end - start                 # 返回秒数
来源：http://tk.nszjky.cn

C#:   (end - start).TotalSeconds
来源：http://ze.jianghongdianzi.cn

[J07] 比较两个日期
来源：http://kz.panjiajie.cn

Py:   d1 < d2;  d1 == d2
来源：http://wp.hnjuh.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://si.muxihuayi.cn

JS:   d1.getTime() < d2.getTime()
来源：http://zw.huanxung.cn

TS:   d1.getTime() < d2.getTime()
来源：http://pc.haigaiapp.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://er.huixiangedu.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://jq.panjiajie.cn

Ruby: d1 < d2;  d1 == d2
来源：http://kd.9csxet.cn

C#:   d1 < d2;  d1 == d2
来源：http://ru.yuntaijiaju.cn

[J08] 提取年月日与星期
来源：http://az.hahajie.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://kb.huixiangedu.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://gj.jianghongdianzi.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://bs.jctech888.com.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hs.haigaiapp.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://yr.huanxung.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://dh.lnxyls.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ct.bjjhwx.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fe.nszjky.cn

[J09] 时区处理
来源：http://ig.bjjhwx.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://vm.gzmigu.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://nf.bookmarksfly.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ll.bjjhwx.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ek.hahajie.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ea.wgjwhj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://fs.szxytkj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://qj.huanxung.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://xl.hahajie.cn

[J10] 取今天 / 本月第一天
来源：http://qq.yuexingan06.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://pm.shxzukj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://gv.yuexingan06.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://he.bookmarksfly.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://cu.szsharing.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xx.huanxung.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://gb.yuexingan06.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://da.szxytkj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://re.bjjhwx.cn

================================================================================
来源：http://wc.panjiajie.cn

K. JSON 与序列化
来源：http://kt.muxihuayi.cn

================================================================================
来源：http://dq.521024.cn

[K01] 对象转 JSON 字符串
来源：http://av.szxytkj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://pf.muxihuayi.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hh.yuexingan06.cn

JS:   JSON.stringify(obj)
来源：http://go.muxihuayi.cn

TS:   JSON.stringify(obj)
来源：http://im.yuexingan06.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://tx.nszjky.cn

Go:   json.Marshal(obj)
来源：http://eg.9csxet.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ic.bookmarksfly.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ji.haigaiapp.cn

[K02] JSON 字符串转对象
来源：http://rt.huanxung.cn

Py:   json.loads(s)
来源：http://uq.gzmigu.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://pm.nicolike.cn

JS:   JSON.parse(s)
来源：http://xc.hahajie.cn

TS:   JSON.parse(s)
来源：http://mf.yuexingan06.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://sx.jianghongdianzi.cn

Go:   json.Unmarshal(data, &v)
来源：http://sb.haigaiapp.cn

Ruby: JSON.parse(s)
来源：http://io.hahajie.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://al.hnjuh.cn

[K03] JSON 美化输出（带缩进）
来源：http://is.hahajie.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://pl.chemitech.net.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qj.shxzskj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://qg.haigaiapp.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://sb.521024.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qu.hnjuh.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xq.huixiangedu.cn

Ruby: JSON.pretty_generate(obj)
来源：http://jy.wgjwhj.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://qw.shxzskj.cn

[K04] 读取 JSON 文件
来源：http://gb.chemitech.net.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://az.lnxyls.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://uh.wgjwhj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xo.chemitech.net.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rg.haigaiapp.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://td.huixiangedu.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://pn.chemitech.net.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://mr.9csxet.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://tx.yuexingan06.cn

[K05] 深拷贝对象
来源：http://ot.shxzskj.cn

Py:   copy.deepcopy(obj)
来源：http://kh.yuexingan06.cn

PHP:  unserialize(serialize($obj));
来源：http://ay.yuntaijiaju.cn

JS:   structuredClone(obj)
来源：http://sq.szxytkj.cn

TS:   structuredClone(obj)
来源：http://ho.yuexingan06.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://cn.hnjuh.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://pr.nszjky.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ok.panjiajie.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://kf.lnxyls.cn

[K06] 解析 URL 查询串
来源：http://ad.colortex.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://oe.hahajie.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://vz.nicolike.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pe.shtwfgs.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://iv.haigaiapp.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://fv.bjjhwx.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://nl.jctech888.com.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ki.szxytkj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://iy.yuexingan06.cn

[K07] 进制转换
来源：http://fv.huixiangedu.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ok.szxytkj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://fn.szsharing.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xf.szsharing.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qv.yuexingan06.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://oh.jctech888.com.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mq.yuexingan06.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://jj.chemitech.net.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://pp.muxihuayi.cn

[K08] 二进制序列化（非 JSON）
来源：http://ck.nszjky.cn

Py:   pickle.dumps(obj)
来源：http://wr.hnjuh.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ay.lnxyls.cn

JS:   v8.serialize(obj)        // Node
来源：http://tj.nszjky.cn

TS:   v8.serialize(obj)        // Node
来源：http://ia.szxytkj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://re.asd995.cn

Go:   encoding/gob
来源：http://ka.shxzskj.cn

Ruby: Marshal.dump(obj)
来源：http://dy.bookmarksfly.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://jw.nicolike.cn

================================================================================
来源：http://st.jianghongdianzi.cn

L. 网络请求
来源：http://em.yuntaijiaju.cn

================================================================================
来源：http://cl.huixinmuqiang.cn

[L01] 发送 GET 请求
来源：http://rb.shtwfgs.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://bk.shxzukj.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ka.hahajie.cn

JS:   await fetch(url)
来源：http://gv.huanxung.cn

TS:   await fetch(url)
来源：http://kg.9csxet.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ce.newstarts.cn

Go:   resp, err := http.Get(url)
来源：http://wz.nszjky.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ut.asd995.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ed.nicolike.cn

[L02] 发送 POST JSON
来源：http://ad.huixiangedu.cn

Py:   requests.post(url, json={"a": 1})
来源：http://gy.gzmigu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://go.jianghongdianzi.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xl.chemitech.net.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ja.szsharing.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://fz.yuexingan06.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://gk.haigaiapp.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://rj.shtwfgs.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://nn.nszjky.cn

[L03] 设置自定义请求头
来源：http://pk.hnjuh.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://kz.szxytkj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://oq.muxihuayi.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fd.bjjhwx.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dp.jianghongdianzi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://fp.huixinmuqiang.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ov.haigaiapp.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://yz.shtwfgs.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://st.shxzskj.cn

[L04] 设置超时
来源：http://vj.shtwfgs.cn

Py:   requests.get(url, timeout=5)
来源：http://sa.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://td.nicolike.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bp.huixiangedu.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://iv.nicolike.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://cw.asd995.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://vx.9csxet.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://bg.huanxung.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://vf.wgjwhj.cn

[L05] 上传文件（multipart）
来源：http://fr.hnjuh.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://vy.huixiangedu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://kr.shxzskj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://na.panjiajie.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hm.huixiangedu.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://lj.9csxet.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hn.shtwfgs.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ag.haigaiapp.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://if.huixinmuqiang.cn

[L06] 解析响应为 JSON
来源：http://sa.muxihuayi.cn

Py:   resp.json()
来源：http://xq.panjiajie.cn

PHP:  json_decode($body, true);
来源：http://rf.521024.cn

JS:   await resp.json()
来源：http://fp.asd995.cn

TS:   await resp.json()
来源：http://nf.haigaiapp.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://pi.bjjhwx.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://pq.colortex.cn

Ruby: JSON.parse(resp.body)
来源：http://zw.gzmigu.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://xc.9csxet.cn

[L07] 处理 HTTP 状态码
来源：http://cu.nicolike.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://bq.gzmigu.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://pu.huixinmuqiang.cn

JS:   resp.ok;  resp.status
来源：http://ou.yuntaijiaju.cn

TS:   resp.ok;  resp.status
来源：http://ut.jianghongdianzi.cn

Java: resp.statusCode()
来源：http://fv.nszjky.cn

Go:   resp.StatusCode
来源：http://gv.bjjhwx.cn

Ruby: resp.code.to_i
来源：http://gj.shxzskj.cn

C#:   (int)resp.StatusCode
来源：http://sr.gzmigu.cn

[L08] 并发请求多个地址
来源：http://fd.nszjky.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://rk.yuexingan06.cn

PHP:  curl_multi_init() 系列
来源：http://eq.bookmarksfly.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://me.jctech888.com.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qq.hahajie.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://fu.hnjuh.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ah.jianghongdianzi.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://jb.huanxung.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://dy.lnxyls.cn

================================================================================
来源：http://nw.jianghongdianzi.cn

M. 命令行 / 进程 / 环境
来源：http://yg.wgjwhj.cn

================================================================================
来源：http://xf.yuntaijiaju.cn

[M01] 读取命令行参数
来源：http://xd.yuntaijiaju.cn

Py:   sys.argv[1:]
来源：http://lb.nicolike.cn

PHP:  $argv;  $argc;
来源：http://jh.muxihuayi.cn

JS:   process.argv.slice(2)
来源：http://tu.hnjuh.cn

TS:   process.argv.slice(2)
来源：http://ud.huanxung.cn

Java: args 数组（main 方法参数）
来源：http://ca.szxytkj.cn

Go:   os.Args[1:]
来源：http://tq.szsharing.cn

Ruby: ARGV
来源：http://ap.haigaiapp.cn

C#:   args 数组（Main 方法参数）
来源：http://ew.gzmigu.cn

[M02] 读取环境变量
来源：http://vl.shxzskj.cn

Py:   os.environ.get("HOME")
来源：http://mv.shxzskj.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://lr.chemitech.net.cn

JS:   process.env.HOME
来源：http://bo.huixiangedu.cn

TS:   process.env.HOME
来源：http://db.hnjuh.cn

Java: System.getenv("HOME")
来源：http://lv.szsharing.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ur.szxytkj.cn

Ruby: ENV["HOME"]
来源：http://mw.yuntaijiaju.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wl.nicolike.cn

[M03] 执行外部命令
来源：http://tn.yuexingan06.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ld.9csxet.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mu.szxytkj.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://my.jctech888.com.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://pp.jianghongdianzi.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://tc.huixiangedu.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ac.huanxung.cn

Ruby: system("ls -l");  `ls -l`
来源：http://zn.bookmarksfly.cn

C#:   Process.Start("ls", "-l");
来源：http://bl.asd995.cn

[M04] 获取当前工作目录
来源：http://wy.haigaiapp.cn

Py:   os.getcwd()
来源：http://jd.colortex.cn

PHP:  getcwd();
来源：http://ad.lnxyls.cn

JS:   process.cwd()
来源：http://gt.huixinmuqiang.cn

TS:   process.cwd()
来源：http://op.gzmigu.cn

Java: Path.of("").toAbsolutePath()
来源：http://sp.haigaiapp.cn

Go:   os.Getwd()
来源：http://zm.panjiajie.cn

Ruby: Dir.pwd
来源：http://vp.haigaiapp.cn

C#:   Directory.GetCurrentDirectory()
来源：http://dk.lnxyls.cn

[M05] 设置退出码
来源：http://yg.yuntaijiaju.cn

Py:   sys.exit(1)
来源：http://og.bookmarksfly.cn

PHP:  exit(1);
来源：http://sf.gzmigu.cn

JS:   process.exit(1)
来源：http://bs.yuntaijiaju.cn

TS:   process.exit(1)
来源：http://ch.panjiajie.cn

Java: System.exit(1)
来源：http://bl.gzmigu.cn

Go:   os.Exit(1)
来源：http://kt.asd995.cn

Ruby: exit 1
来源：http://ok.hahajie.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ow.gzmigu.cn

[M06] 向标准错误输出
来源：http://if.asd995.cn

Py:   print("err", file=sys.stderr)
来源：http://ae.521024.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://kc.panjiajie.cn

JS:   console.error("err")
来源：http://gz.asd995.cn

TS:   console.error("err")
来源：http://mg.jianghongdianzi.cn

Java: System.err.println("err")
来源：http://tb.bookmarksfly.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://rx.huanxung.cn

Ruby: warn "err"
来源：http://vs.shxzskj.cn

C#:   Console.Error.WriteLine("err")
来源：http://pm.haigaiapp.cn

[M07] 判断是否为主入口
来源：http://je.shxzukj.cn

Py:   if __name__ == "__main__":
来源：http://yi.huixinmuqiang.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mc.jctech888.com.cn

JS:   require.main === module
来源：http://aq.shxzukj.cn

TS:   require.main === module
来源：http://mp.bookmarksfly.cn

Java: public static void main(String[] args)
来源：http://qs.panjiajie.cn

Go:   func main()
来源：http://ob.panjiajie.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://op.asd995.cn

C#:   static void Main(string[] args)
来源：http://tk.huixinmuqiang.cn

[M08] 获取系统与运行时信息
来源：http://pf.haigaiapp.cn

Py:   platform.system();  platform.python_version()
来源：http://bf.haigaiapp.cn

PHP:  PHP_OS;  phpversion();
来源：http://qp.shtwfgs.cn

JS:   process.platform;  process.version
来源：http://bb.bookmarksfly.cn

TS:   process.platform;  process.version
来源：http://mp.chemitech.net.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://cx.huixiangedu.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://xm.haigaiapp.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://qa.huixinmuqiang.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://oa.hahajie.cn

================================================================================
来源：http://ry.huixiangedu.cn

N. 数据结构与算法
来源：http://qa.9csxet.cn

================================================================================
来源：http://nj.wgjwhj.cn

[N01] 二分查找（有序数组）
来源：http://py.muxihuayi.cn

Py:   bisect.bisect_left(arr, x)
来源：http://el.bjjhwx.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mp.bjjhwx.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kw.9csxet.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vc.bjjhwx.cn

Java: Arrays.binarySearch(arr, x)
来源：http://lx.yuntaijiaju.cn

Go:   sort.SearchInts(arr, x)
来源：http://rz.521024.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://dh.hahajie.cn

C#:   Array.BinarySearch(arr, x)
来源：http://sd.lnxyls.cn

[N02] 排序（工程实践用内置实现）
来源：http://uh.colortex.cn

Py:   sorted(arr);  arr.sort()
来源：http://ra.newstarts.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://af.wgjwhj.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://qr.nicolike.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://yc.9csxet.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://re.yuntaijiaju.cn

Go:   slices.Sort(arr)
来源：http://by.shtwfgs.cn

Ruby: arr.sort
来源：http://zx.muxihuayi.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://za.nszjky.cn

[N03] 快速排序（分治示例）
来源：http://zf.gzmigu.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://xf.huixiangedu.cn

PHP:  // 递归实现，或用 usort
来源：http://hi.bookmarksfly.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gz.shxzukj.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xn.colortex.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://gs.haigaiapp.cn


<!-- 参考信息 -->