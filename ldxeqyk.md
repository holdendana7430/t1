代发 wailian999

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ge.shxzukj.cn

Ruby: Time.now + 7 * 86400
来源：http://nm.shxzukj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://wi.bjjhwx.cn

[J06] 计算两时间之差
来源：http://oz.huixiangedu.cn

Py:   (end - start).total_seconds()
来源：http://cc.colortex.cn

PHP:  $end->diff($start)->days;
来源：http://up.yuexingan06.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://xn.bookmarksfly.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ca.szsharing.cn

Java: Duration.between(start, end).toSeconds()
来源：http://qp.asd995.cn

Go:   end.Sub(start).Hours()
来源：http://ow.panjiajie.cn

Ruby: end - start                 # 返回秒数
来源：http://vq.9csxet.cn

C#:   (end - start).TotalSeconds
来源：http://ua.wgjwhj.cn

[J07] 比较两个日期
来源：http://pe.szxytkj.cn

Py:   d1 < d2;  d1 == d2
来源：http://tf.panjiajie.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://nc.muxihuayi.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ua.9csxet.cn

TS:   d1.getTime() < d2.getTime()
来源：http://la.shtwfgs.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xa.colortex.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://yq.9csxet.cn

Ruby: d1 < d2;  d1 == d2
来源：http://dg.jctech888.com.cn

C#:   d1 < d2;  d1 == d2
来源：http://yv.hahajie.cn

[J08] 提取年月日与星期
来源：http://ks.9csxet.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://sc.shxzskj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://oz.lnxyls.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ig.gzmigu.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xs.521024.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ly.lnxyls.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://fp.newstarts.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://xk.chemitech.net.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://he.nicolike.cn

[J09] 时区处理
来源：http://mx.huixinmuqiang.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://sv.chemitech.net.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://yp.lnxyls.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ar.bookmarksfly.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xj.shxzskj.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://jo.huixiangedu.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://uc.chemitech.net.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://xu.hahajie.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wa.szxytkj.cn

[J10] 取今天 / 本月第一天
来源：http://cs.panjiajie.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ue.panjiajie.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://nw.chemitech.net.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://uy.haigaiapp.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://md.jctech888.com.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://db.bookmarksfly.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://sy.521024.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ak.hnjuh.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hq.gzmigu.cn

================================================================================
来源：http://gv.yuexingan06.cn

K. JSON 与序列化
来源：http://nf.shxzukj.cn

================================================================================
来源：http://jq.szxytkj.cn

[K01] 对象转 JSON 字符串
来源：http://hn.wgjwhj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://dp.asd995.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hx.bjjhwx.cn

JS:   JSON.stringify(obj)
来源：http://fa.nicolike.cn

TS:   JSON.stringify(obj)
来源：http://wf.lnxyls.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://jb.yuexingan06.cn

Go:   json.Marshal(obj)
来源：http://dr.shxzskj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://xp.szxytkj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://eu.panjiajie.cn

[K02] JSON 字符串转对象
来源：http://zu.yuntaijiaju.cn

Py:   json.loads(s)
来源：http://kg.hnjuh.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://gc.huixinmuqiang.cn

JS:   JSON.parse(s)
来源：http://wh.jctech888.com.cn

TS:   JSON.parse(s)
来源：http://jq.huixinmuqiang.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ve.bookmarksfly.cn

Go:   json.Unmarshal(data, &v)
来源：http://dl.chemitech.net.cn

Ruby: JSON.parse(s)
来源：http://kp.nszjky.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ef.nicolike.cn

[K03] JSON 美化输出（带缩进）
来源：http://qi.newstarts.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://tf.hnjuh.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://gr.huanxung.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ol.muxihuayi.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ot.szxytkj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://di.yuexingan06.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://op.asd995.cn

Ruby: JSON.pretty_generate(obj)
来源：http://hh.haigaiapp.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://qg.yuntaijiaju.cn

[K04] 读取 JSON 文件
来源：http://gr.colortex.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://qf.huixiangedu.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://vn.shtwfgs.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zk.colortex.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zj.huixiangedu.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://yp.hnjuh.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://rj.9csxet.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://tx.lnxyls.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://rh.muxihuayi.cn

[K05] 深拷贝对象
来源：http://re.huanxung.cn

Py:   copy.deepcopy(obj)
来源：http://cm.shxzskj.cn

PHP:  unserialize(serialize($obj));
来源：http://ot.huixinmuqiang.cn

JS:   structuredClone(obj)
来源：http://nv.szxytkj.cn

TS:   structuredClone(obj)
来源：http://xs.jctech888.com.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://nz.lnxyls.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qj.nszjky.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://nh.colortex.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://re.bookmarksfly.cn

[K06] 解析 URL 查询串
来源：http://pt.szsharing.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://bu.gzmigu.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://xd.colortex.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://iv.huixinmuqiang.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uh.jctech888.com.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://rb.nicolike.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://sj.huanxung.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ug.muxihuayi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://bd.szxytkj.cn

[K07] 进制转换
来源：http://je.jianghongdianzi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://xd.yuexingan06.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://zx.jianghongdianzi.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://sh.nicolike.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mk.nszjky.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://zg.panjiajie.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://nk.chemitech.net.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qu.chemitech.net.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://re.wgjwhj.cn

[K08] 二进制序列化（非 JSON）
来源：http://po.jianghongdianzi.cn

Py:   pickle.dumps(obj)
来源：http://af.newstarts.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://or.gzmigu.cn

JS:   v8.serialize(obj)        // Node
来源：http://ow.lnxyls.cn

TS:   v8.serialize(obj)        // Node
来源：http://bv.newstarts.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://rf.huixinmuqiang.cn

Go:   encoding/gob
来源：http://hh.chemitech.net.cn

Ruby: Marshal.dump(obj)
来源：http://ps.huixinmuqiang.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hv.yuntaijiaju.cn

================================================================================
来源：http://it.yuexingan06.cn

L. 网络请求
来源：http://hl.hahajie.cn

================================================================================
来源：http://wu.huixiangedu.cn

[L01] 发送 GET 请求
来源：http://gd.huanxung.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://uu.shxzskj.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://zz.lnxyls.cn

JS:   await fetch(url)
来源：http://cv.jianghongdianzi.cn

TS:   await fetch(url)
来源：http://mn.yuexingan06.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://pm.gzmigu.cn

Go:   resp, err := http.Get(url)
来源：http://dt.jctech888.com.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://tj.shxzskj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://uw.huanxung.cn

[L02] 发送 POST JSON
来源：http://yj.huixiangedu.cn

Py:   requests.post(url, json={"a": 1})
来源：http://qf.hnjuh.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://yr.bookmarksfly.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lx.shxzskj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://oh.huixinmuqiang.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://zx.szxytkj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://zo.9csxet.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://sy.shxzukj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mn.gzmigu.cn

[L03] 设置自定义请求头
来源：http://nk.shxzskj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://bm.521024.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://vf.haigaiapp.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sm.asd995.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vu.shtwfgs.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://il.shxzskj.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://qr.huixiangedu.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://xl.huixinmuqiang.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ov.jianghongdianzi.cn

[L04] 设置超时
来源：http://ft.yuexingan06.cn

Py:   requests.get(url, timeout=5)
来源：http://vv.hnjuh.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://en.colortex.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mm.colortex.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hm.gzmigu.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://nv.panjiajie.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://kb.huanxung.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://tn.shxzskj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://pt.newstarts.cn

[L05] 上传文件（multipart）
来源：http://wx.szsharing.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://de.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://fn.wgjwhj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://an.wgjwhj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://vh.huanxung.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://xk.yuntaijiaju.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://bj.haigaiapp.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://xv.hahajie.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ws.nicolike.cn

[L06] 解析响应为 JSON
来源：http://yt.hahajie.cn

Py:   resp.json()
来源：http://hm.jctech888.com.cn

PHP:  json_decode($body, true);
来源：http://pv.szxytkj.cn

JS:   await resp.json()
来源：http://dk.shtwfgs.cn

TS:   await resp.json()
来源：http://od.newstarts.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://tu.bookmarksfly.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://xq.nicolike.cn

Ruby: JSON.parse(resp.body)
来源：http://ov.9csxet.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://xc.asd995.cn

[L07] 处理 HTTP 状态码
来源：http://ke.nszjky.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mi.hahajie.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://au.panjiajie.cn

JS:   resp.ok;  resp.status
来源：http://oy.szsharing.cn

TS:   resp.ok;  resp.status
来源：http://vv.newstarts.cn

Java: resp.statusCode()
来源：http://aw.yuntaijiaju.cn

Go:   resp.StatusCode
来源：http://if.szxytkj.cn

Ruby: resp.code.to_i
来源：http://aw.szxytkj.cn

C#:   (int)resp.StatusCode
来源：http://yq.shtwfgs.cn

[L08] 并发请求多个地址
来源：http://gf.panjiajie.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://uq.huanxung.cn

PHP:  curl_multi_init() 系列
来源：http://bp.wgjwhj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jc.hahajie.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ow.panjiajie.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://io.shxzskj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://pz.muxihuayi.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://fd.huixinmuqiang.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ik.wgjwhj.cn

================================================================================
来源：http://hk.szsharing.cn

M. 命令行 / 进程 / 环境
来源：http://ci.yuexingan06.cn

================================================================================
来源：http://lp.shxzskj.cn

[M01] 读取命令行参数
来源：http://pw.yuexingan06.cn

Py:   sys.argv[1:]
来源：http://em.haigaiapp.cn

PHP:  $argv;  $argc;
来源：http://tk.nicolike.cn

JS:   process.argv.slice(2)
来源：http://hj.asd995.cn

TS:   process.argv.slice(2)
来源：http://us.huixinmuqiang.cn

Java: args 数组（main 方法参数）
来源：http://nh.shxzskj.cn

Go:   os.Args[1:]
来源：http://xa.shtwfgs.cn

Ruby: ARGV
来源：http://ol.bjjhwx.cn

C#:   args 数组（Main 方法参数）
来源：http://rl.hahajie.cn

[M02] 读取环境变量
来源：http://yc.gzmigu.cn

Py:   os.environ.get("HOME")
来源：http://gy.colortex.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://re.szxytkj.cn

JS:   process.env.HOME
来源：http://dj.bjjhwx.cn

TS:   process.env.HOME
来源：http://va.colortex.cn

Java: System.getenv("HOME")
来源：http://or.chemitech.net.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ow.shxzskj.cn

Ruby: ENV["HOME"]
来源：http://in.panjiajie.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://fb.bookmarksfly.cn

[M03] 执行外部命令
来源：http://fq.huixinmuqiang.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vv.chemitech.net.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://fq.huanxung.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://hn.huixiangedu.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://hk.shxzukj.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://fc.huixinmuqiang.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ym.huixinmuqiang.cn

Ruby: system("ls -l");  `ls -l`
来源：http://pu.hahajie.cn

C#:   Process.Start("ls", "-l");
来源：http://mh.haigaiapp.cn

[M04] 获取当前工作目录
来源：http://nd.wgjwhj.cn

Py:   os.getcwd()
来源：http://pp.shxzskj.cn

PHP:  getcwd();
来源：http://ss.bookmarksfly.cn

JS:   process.cwd()
来源：http://tv.chemitech.net.cn

TS:   process.cwd()
来源：http://gb.shtwfgs.cn

Java: Path.of("").toAbsolutePath()
来源：http://yd.shxzukj.cn

Go:   os.Getwd()
来源：http://au.jctech888.com.cn

Ruby: Dir.pwd
来源：http://rl.yuntaijiaju.cn

C#:   Directory.GetCurrentDirectory()
来源：http://sz.shxzskj.cn

[M05] 设置退出码
来源：http://bo.asd995.cn

Py:   sys.exit(1)
来源：http://iu.colortex.cn

PHP:  exit(1);
来源：http://gb.gzmigu.cn

JS:   process.exit(1)
来源：http://cr.hnjuh.cn

TS:   process.exit(1)
来源：http://fd.gzmigu.cn

Java: System.exit(1)
来源：http://pm.huanxung.cn

Go:   os.Exit(1)
来源：http://di.yuexingan06.cn

Ruby: exit 1
来源：http://xb.hahajie.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ru.wgjwhj.cn

[M06] 向标准错误输出
来源：http://hh.lnxyls.cn

Py:   print("err", file=sys.stderr)
来源：http://do.shxzskj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://hi.huanxung.cn

JS:   console.error("err")
来源：http://jn.bookmarksfly.cn

TS:   console.error("err")
来源：http://dl.shxzukj.cn

Java: System.err.println("err")
来源：http://mu.huixiangedu.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ot.bookmarksfly.cn

Ruby: warn "err"
来源：http://vt.521024.cn

C#:   Console.Error.WriteLine("err")
来源：http://sw.nicolike.cn

[M07] 判断是否为主入口
来源：http://sb.yuexingan06.cn

Py:   if __name__ == "__main__":
来源：http://ml.jctech888.com.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hn.asd995.cn

JS:   require.main === module
来源：http://qs.panjiajie.cn

TS:   require.main === module
来源：http://uy.yuexingan06.cn

Java: public static void main(String[] args)
来源：http://ns.jianghongdianzi.cn

Go:   func main()
来源：http://yg.nszjky.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://kq.gzmigu.cn

C#:   static void Main(string[] args)
来源：http://cy.huixiangedu.cn

[M08] 获取系统与运行时信息
来源：http://qu.szsharing.cn

Py:   platform.system();  platform.python_version()
来源：http://ar.shxzukj.cn

PHP:  PHP_OS;  phpversion();
来源：http://xt.muxihuayi.cn

JS:   process.platform;  process.version
来源：http://kb.521024.cn

TS:   process.platform;  process.version
来源：http://ug.bookmarksfly.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://cv.muxihuayi.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ko.panjiajie.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ls.nicolike.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ny.shtwfgs.cn

================================================================================
来源：http://iz.9csxet.cn

N. 数据结构与算法
来源：http://bl.jianghongdianzi.cn

================================================================================
来源：http://sb.jianghongdianzi.cn

[N01] 二分查找（有序数组）
来源：http://qk.huanxung.cn

Py:   bisect.bisect_left(arr, x)
来源：http://sy.szsharing.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://uv.wgjwhj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ee.shtwfgs.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://su.szsharing.cn

Java: Arrays.binarySearch(arr, x)
来源：http://vx.panjiajie.cn

Go:   sort.SearchInts(arr, x)
来源：http://yr.haigaiapp.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://kw.shtwfgs.cn

C#:   Array.BinarySearch(arr, x)
来源：http://wx.muxihuayi.cn

[N02] 排序（工程实践用内置实现）
来源：http://qp.muxihuayi.cn

Py:   sorted(arr);  arr.sort()
来源：http://kx.szxytkj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://oi.shxzskj.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ex.hnjuh.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://rg.yuexingan06.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ef.szxytkj.cn

Go:   slices.Sort(arr)
来源：http://xx.yuexingan06.cn

Ruby: arr.sort
来源：http://ib.521024.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://gu.shxzukj.cn

[N03] 快速排序（分治示例）
来源：http://wd.asd995.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://tj.szsharing.cn

PHP:  // 递归实现，或用 usort
来源：http://lc.szxytkj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://on.lnxyls.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ul.bjjhwx.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://jb.hnjuh.cn


<!-- 参考信息 -->