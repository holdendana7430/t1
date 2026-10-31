代发 wailian999

Py:   (end - start).total_seconds()
来源：http://wb.hahajie.cn

PHP:  $end->diff($start)->days;
来源：http://kt.panjiajie.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://pm.hahajie.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ju.bjjhwx.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ug.yuexingan06.cn

Go:   end.Sub(start).Hours()
来源：http://fh.9csxet.cn

Ruby: end - start                 # 返回秒数
来源：http://kr.newstarts.cn

C#:   (end - start).TotalSeconds
来源：http://lz.hnjuh.cn

[J07] 比较两个日期
来源：http://hk.jctech888.com.cn

Py:   d1 < d2;  d1 == d2
来源：http://iy.huanxung.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://yu.lnxyls.cn

JS:   d1.getTime() < d2.getTime()
来源：http://gr.bookmarksfly.cn

TS:   d1.getTime() < d2.getTime()
来源：http://xj.shtwfgs.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hs.jctech888.com.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://qi.wgjwhj.cn

Ruby: d1 < d2;  d1 == d2
来源：http://wt.asd995.cn

C#:   d1 < d2;  d1 == d2
来源：http://jl.muxihuayi.cn

[J08] 提取年月日与星期
来源：http://ub.colortex.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://at.yuexingan06.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://bo.jianghongdianzi.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mj.yuntaijiaju.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://dn.nicolike.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://pf.bjjhwx.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://yn.colortex.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ln.szxytkj.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ca.szxytkj.cn

[J09] 时区处理
来源：http://nm.jianghongdianzi.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://vk.hahajie.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://sc.huanxung.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lf.bjjhwx.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ww.asd995.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://yr.jianghongdianzi.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://jh.521024.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://za.yuexingan06.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mi.bookmarksfly.cn

[J10] 取今天 / 本月第一天
来源：http://bp.hahajie.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://hd.szsharing.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wm.szsharing.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hd.panjiajie.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ch.shxzskj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://gc.bookmarksfly.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://zt.wgjwhj.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://nb.hahajie.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://qr.haigaiapp.cn

================================================================================
来源：http://it.9csxet.cn

K. JSON 与序列化
来源：http://hy.szxytkj.cn

================================================================================
来源：http://rt.haigaiapp.cn

[K01] 对象转 JSON 字符串
来源：http://ob.jctech888.com.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hd.nszjky.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ut.jctech888.com.cn

JS:   JSON.stringify(obj)
来源：http://lu.chemitech.net.cn

TS:   JSON.stringify(obj)
来源：http://rp.nicolike.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://zz.shxzskj.cn

Go:   json.Marshal(obj)
来源：http://qn.shtwfgs.cn

Ruby: obj.to_json                                     // require "json"
来源：http://vd.shxzskj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ff.haigaiapp.cn

[K02] JSON 字符串转对象
来源：http://jp.jianghongdianzi.cn

Py:   json.loads(s)
来源：http://ci.bjjhwx.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wn.szsharing.cn

JS:   JSON.parse(s)
来源：http://mp.newstarts.cn

TS:   JSON.parse(s)
来源：http://zv.wgjwhj.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mf.haigaiapp.cn

Go:   json.Unmarshal(data, &v)
来源：http://zo.haigaiapp.cn

Ruby: JSON.parse(s)
来源：http://nz.chemitech.net.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wk.hnjuh.cn

[K03] JSON 美化输出（带缩进）
来源：http://kv.hahajie.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://bq.yuntaijiaju.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://sd.wgjwhj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ys.yuexingan06.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ru.huixiangedu.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qt.szxytkj.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xp.huixinmuqiang.cn

Ruby: JSON.pretty_generate(obj)
来源：http://cc.hnjuh.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hg.szxytkj.cn

[K04] 读取 JSON 文件
来源：http://eq.huixinmuqiang.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jw.hahajie.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://bs.hahajie.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sa.bookmarksfly.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ar.hahajie.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ol.hnjuh.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://fr.panjiajie.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://it.bookmarksfly.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://db.asd995.cn

[K05] 深拷贝对象
来源：http://cq.bookmarksfly.cn

Py:   copy.deepcopy(obj)
来源：http://gc.nicolike.cn

PHP:  unserialize(serialize($obj));
来源：http://se.shxzskj.cn

JS:   structuredClone(obj)
来源：http://mb.newstarts.cn

TS:   structuredClone(obj)
来源：http://bj.shtwfgs.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://sz.bjjhwx.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://fm.nszjky.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://sg.asd995.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://av.chemitech.net.cn

[K06] 解析 URL 查询串
来源：http://gb.bookmarksfly.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://fb.haigaiapp.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://jm.yuntaijiaju.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pe.shtwfgs.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lf.szxytkj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://pc.nszjky.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://qv.szsharing.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vj.jctech888.com.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://cz.yuntaijiaju.cn

[K07] 进制转换
来源：http://ns.521024.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://xx.shxzskj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mc.jctech888.com.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://qm.muxihuayi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://oa.hnjuh.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ra.jctech888.com.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://pu.huixiangedu.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ka.hnjuh.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://bb.yuexingan06.cn

[K08] 二进制序列化（非 JSON）
来源：http://gj.lnxyls.cn

Py:   pickle.dumps(obj)
来源：http://pa.shxzskj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://xc.hnjuh.cn

JS:   v8.serialize(obj)        // Node
来源：http://zw.521024.cn

TS:   v8.serialize(obj)        // Node
来源：http://cc.gzmigu.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://md.lnxyls.cn

Go:   encoding/gob
来源：http://ew.yuntaijiaju.cn

Ruby: Marshal.dump(obj)
来源：http://zo.huixiangedu.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://uc.gzmigu.cn

================================================================================
来源：http://qg.9csxet.cn

L. 网络请求
来源：http://wc.shtwfgs.cn

================================================================================
来源：http://by.szxytkj.cn

[L01] 发送 GET 请求
来源：http://re.asd995.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://vg.newstarts.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://fq.huanxung.cn

JS:   await fetch(url)
来源：http://dm.szxytkj.cn

TS:   await fetch(url)
来源：http://tc.nszjky.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://bm.hnjuh.cn

Go:   resp, err := http.Get(url)
来源：http://eb.newstarts.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ot.yuntaijiaju.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://oy.shxzskj.cn

[L02] 发送 POST JSON
来源：http://ct.521024.cn

Py:   requests.post(url, json={"a": 1})
来源：http://kh.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://pv.asd995.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jd.newstarts.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ih.jianghongdianzi.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://po.lnxyls.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://oj.huanxung.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://am.yuexingan06.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ac.gzmigu.cn

[L03] 设置自定义请求头
来源：http://hk.haigaiapp.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://fd.yuntaijiaju.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://yi.huixinmuqiang.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rz.panjiajie.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xb.huixinmuqiang.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://cj.chemitech.net.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ed.chemitech.net.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://lc.szsharing.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://fc.hnjuh.cn

[L04] 设置超时
来源：http://lk.haigaiapp.cn

Py:   requests.get(url, timeout=5)
来源：http://jo.nicolike.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mk.lnxyls.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hg.nszjky.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fb.hahajie.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://gw.colortex.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://gd.jctech888.com.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://xx.jctech888.com.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hb.haigaiapp.cn

[L05] 上传文件（multipart）
来源：http://ht.jianghongdianzi.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://cr.wgjwhj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ne.szsharing.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ni.jianghongdianzi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://pa.yuntaijiaju.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://kg.panjiajie.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://yl.szsharing.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hu.shxzukj.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://gk.gzmigu.cn

[L06] 解析响应为 JSON
来源：http://wp.shxzukj.cn

Py:   resp.json()
来源：http://pn.shtwfgs.cn

PHP:  json_decode($body, true);
来源：http://rk.9csxet.cn

JS:   await resp.json()
来源：http://ll.wgjwhj.cn

TS:   await resp.json()
来源：http://vo.huixiangedu.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://lr.huixiangedu.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ni.newstarts.cn

Ruby: JSON.parse(resp.body)
来源：http://jj.9csxet.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hp.jctech888.com.cn

[L07] 处理 HTTP 状态码
来源：http://bn.chemitech.net.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://cm.chemitech.net.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://yc.gzmigu.cn

JS:   resp.ok;  resp.status
来源：http://hs.nszjky.cn

TS:   resp.ok;  resp.status
来源：http://la.huanxung.cn

Java: resp.statusCode()
来源：http://qr.bookmarksfly.cn

Go:   resp.StatusCode
来源：http://mv.gzmigu.cn

Ruby: resp.code.to_i
来源：http://km.bookmarksfly.cn

C#:   (int)resp.StatusCode
来源：http://yl.asd995.cn

[L08] 并发请求多个地址
来源：http://fw.shxzskj.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://yu.newstarts.cn

PHP:  curl_multi_init() 系列
来源：http://am.jianghongdianzi.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tb.hahajie.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://oo.wgjwhj.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://gn.nszjky.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://uk.nicolike.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://td.bookmarksfly.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://gv.nicolike.cn

================================================================================
来源：http://oo.colortex.cn

M. 命令行 / 进程 / 环境
来源：http://mv.hnjuh.cn

================================================================================
来源：http://kp.lnxyls.cn

[M01] 读取命令行参数
来源：http://ux.bookmarksfly.cn

Py:   sys.argv[1:]
来源：http://se.chemitech.net.cn

PHP:  $argv;  $argc;
来源：http://qz.bjjhwx.cn

JS:   process.argv.slice(2)
来源：http://my.bookmarksfly.cn

TS:   process.argv.slice(2)
来源：http://wk.panjiajie.cn

Java: args 数组（main 方法参数）
来源：http://oe.asd995.cn

Go:   os.Args[1:]
来源：http://ab.yuntaijiaju.cn

Ruby: ARGV
来源：http://ii.jianghongdianzi.cn

C#:   args 数组（Main 方法参数）
来源：http://jb.shxzukj.cn

[M02] 读取环境变量
来源：http://bu.huixinmuqiang.cn

Py:   os.environ.get("HOME")
来源：http://iu.yuexingan06.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://gq.shxzskj.cn

JS:   process.env.HOME
来源：http://op.huanxung.cn

TS:   process.env.HOME
来源：http://ev.szxytkj.cn

Java: System.getenv("HOME")
来源：http://oi.huixinmuqiang.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://tm.nicolike.cn

Ruby: ENV["HOME"]
来源：http://ay.yuexingan06.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://gt.yuexingan06.cn

[M03] 执行外部命令
来源：http://yy.bjjhwx.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hm.panjiajie.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://yl.hnjuh.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ce.lnxyls.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://me.huanxung.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://jl.huanxung.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://hv.lnxyls.cn

Ruby: system("ls -l");  `ls -l`
来源：http://tm.yuexingan06.cn

C#:   Process.Start("ls", "-l");
来源：http://hc.yuexingan06.cn

[M04] 获取当前工作目录
来源：http://hl.huixinmuqiang.cn

Py:   os.getcwd()
来源：http://ur.newstarts.cn

PHP:  getcwd();
来源：http://sc.haigaiapp.cn

JS:   process.cwd()
来源：http://eg.shxzukj.cn

TS:   process.cwd()
来源：http://dt.yuexingan06.cn

Java: Path.of("").toAbsolutePath()
来源：http://or.bjjhwx.cn

Go:   os.Getwd()
来源：http://id.521024.cn

Ruby: Dir.pwd
来源：http://sv.muxihuayi.cn

C#:   Directory.GetCurrentDirectory()
来源：http://fm.panjiajie.cn

[M05] 设置退出码
来源：http://nn.szsharing.cn

Py:   sys.exit(1)
来源：http://tn.hnjuh.cn

PHP:  exit(1);
来源：http://yi.521024.cn

JS:   process.exit(1)
来源：http://lq.huixiangedu.cn

TS:   process.exit(1)
来源：http://hr.hahajie.cn

Java: System.exit(1)
来源：http://jy.hahajie.cn

Go:   os.Exit(1)
来源：http://gz.szxytkj.cn

Ruby: exit 1
来源：http://gd.newstarts.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://uf.huixiangedu.cn

[M06] 向标准错误输出
来源：http://ek.nicolike.cn

Py:   print("err", file=sys.stderr)
来源：http://bj.shtwfgs.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://rc.nszjky.cn

JS:   console.error("err")
来源：http://ov.haigaiapp.cn

TS:   console.error("err")
来源：http://jg.yuntaijiaju.cn

Java: System.err.println("err")
来源：http://tz.colortex.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://jp.yuntaijiaju.cn

Ruby: warn "err"
来源：http://ok.asd995.cn

C#:   Console.Error.WriteLine("err")
来源：http://kq.szxytkj.cn

[M07] 判断是否为主入口
来源：http://zp.bjjhwx.cn

Py:   if __name__ == "__main__":
来源：http://sk.lnxyls.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wd.muxihuayi.cn

JS:   require.main === module
来源：http://zo.9csxet.cn

TS:   require.main === module
来源：http://ka.shtwfgs.cn

Java: public static void main(String[] args)
来源：http://ux.yuexingan06.cn

Go:   func main()
来源：http://kg.9csxet.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://cp.szsharing.cn

C#:   static void Main(string[] args)
来源：http://sx.panjiajie.cn

[M08] 获取系统与运行时信息
来源：http://pq.muxihuayi.cn

Py:   platform.system();  platform.python_version()
来源：http://ax.lnxyls.cn

PHP:  PHP_OS;  phpversion();
来源：http://jr.haigaiapp.cn

JS:   process.platform;  process.version
来源：http://cg.huixiangedu.cn

TS:   process.platform;  process.version
来源：http://kh.huixinmuqiang.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://pk.newstarts.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://mz.shxzskj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wh.gzmigu.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://cy.bjjhwx.cn

================================================================================
来源：http://pv.chemitech.net.cn

N. 数据结构与算法
来源：http://ip.szsharing.cn

================================================================================
来源：http://rv.muxihuayi.cn

[N01] 二分查找（有序数组）
来源：http://ka.9csxet.cn

Py:   bisect.bisect_left(arr, x)
来源：http://mt.wgjwhj.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://vt.shxzukj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ho.hahajie.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://te.shxzskj.cn

Java: Arrays.binarySearch(arr, x)
来源：http://qm.shxzukj.cn

Go:   sort.SearchInts(arr, x)
来源：http://jk.shxzukj.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://dj.huixinmuqiang.cn

C#:   Array.BinarySearch(arr, x)
来源：http://iy.bjjhwx.cn

[N02] 排序（工程实践用内置实现）
来源：http://wu.shxzskj.cn

Py:   sorted(arr);  arr.sort()
来源：http://qq.hahajie.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://dt.huixinmuqiang.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ne.szxytkj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://yl.jctech888.com.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://co.shtwfgs.cn

Go:   slices.Sort(arr)
来源：http://tq.huixiangedu.cn

Ruby: arr.sort
来源：http://qk.shxzukj.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://fq.newstarts.cn

[N03] 快速排序（分治示例）
来源：http://xe.wgjwhj.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://jm.bookmarksfly.cn

PHP:  // 递归实现，或用 usort
来源：http://sa.nicolike.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://no.newstarts.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kn.muxihuayi.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://tv.jctech888.com.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://rv.521024.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://fj.chemitech.net.cn

C#:   // 手写递归，或 Array.Sort
来源：http://gv.nszjky.cn

[N04] 斐波那契数列
来源：http://ue.jianghongdianzi.cn


<!-- 参考信息 -->