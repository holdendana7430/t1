代发 wailian999

PHP:  (new DateTime())->modify("+7 days");
来源：http://cs.gzmigu.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ov.wgjwhj.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://gj.9csxet.cn

Java: LocalDate.now().plusDays(7)
来源：http://bu.lnxyls.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://oi.huixiangedu.cn

Ruby: Time.now + 7 * 86400
来源：http://ib.lnxyls.cn

C#:   DateTime.Now.AddDays(7)
来源：http://jy.muxihuayi.cn

[J06] 计算两时间之差
来源：http://oz.huixiangedu.cn

Py:   (end - start).total_seconds()
来源：http://wo.gzmigu.cn

PHP:  $end->diff($start)->days;
来源：http://vr.wgjwhj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://pc.bookmarksfly.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://nm.muxihuayi.cn

Java: Duration.between(start, end).toSeconds()
来源：http://px.huixinmuqiang.cn

Go:   end.Sub(start).Hours()
来源：http://ha.szxytkj.cn

Ruby: end - start                 # 返回秒数
来源：http://xz.asd995.cn

C#:   (end - start).TotalSeconds
来源：http://dz.newstarts.cn

[J07] 比较两个日期
来源：http://lj.jianghongdianzi.cn

Py:   d1 < d2;  d1 == d2
来源：http://cj.gzmigu.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://nf.wgjwhj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://az.shxzskj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://lz.bookmarksfly.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://uf.lnxyls.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wa.jctech888.com.cn

Ruby: d1 < d2;  d1 == d2
来源：http://us.shxzskj.cn

C#:   d1 < d2;  d1 == d2
来源：http://po.shxzskj.cn

[J08] 提取年月日与星期
来源：http://dc.9csxet.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://xm.huixinmuqiang.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://uv.yuntaijiaju.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hl.nszjky.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://pq.yuntaijiaju.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ar.jctech888.com.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://sv.jianghongdianzi.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://qj.nicolike.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://xi.muxihuayi.cn

[J09] 时区处理
来源：http://wi.haigaiapp.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ba.huanxung.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://lg.asd995.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kb.lnxyls.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mk.jianghongdianzi.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://fs.huanxung.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://vu.gzmigu.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ix.bjjhwx.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://fw.yuexingan06.cn

[J10] 取今天 / 本月第一天
来源：http://bh.jianghongdianzi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://bw.hnjuh.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://iq.szsharing.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://tx.panjiajie.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://xz.huanxung.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://yr.hahajie.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://kz.newstarts.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ky.szsharing.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://pe.newstarts.cn

================================================================================
来源：http://jz.hnjuh.cn

K. JSON 与序列化
来源：http://xv.yuexingan06.cn

================================================================================
来源：http://oc.szsharing.cn

[K01] 对象转 JSON 字符串
来源：http://kn.nicolike.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://jo.panjiajie.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://qr.jctech888.com.cn

JS:   JSON.stringify(obj)
来源：http://ev.shtwfgs.cn

TS:   JSON.stringify(obj)
来源：http://up.shxzukj.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://pc.gzmigu.cn

Go:   json.Marshal(obj)
来源：http://dr.wgjwhj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://gm.shxzukj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://vr.szxytkj.cn

[K02] JSON 字符串转对象
来源：http://yp.huixinmuqiang.cn

Py:   json.loads(s)
来源：http://yk.jianghongdianzi.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://od.jianghongdianzi.cn

JS:   JSON.parse(s)
来源：http://ma.chemitech.net.cn

TS:   JSON.parse(s)
来源：http://ta.colortex.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://du.lnxyls.cn

Go:   json.Unmarshal(data, &v)
来源：http://lq.panjiajie.cn

Ruby: JSON.parse(s)
来源：http://pt.yuntaijiaju.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://gi.shxzskj.cn

[K03] JSON 美化输出（带缩进）
来源：http://lu.panjiajie.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://as.gzmigu.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://yj.jianghongdianzi.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://fa.lnxyls.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://fq.lnxyls.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ny.nicolike.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ca.haigaiapp.cn

Ruby: JSON.pretty_generate(obj)
来源：http://pw.szxytkj.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://rk.szxytkj.cn

[K04] 读取 JSON 文件
来源：http://ii.yuexingan06.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://pd.panjiajie.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://aq.521024.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hi.hahajie.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jk.szsharing.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://uy.jianghongdianzi.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://vb.hahajie.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://lx.9csxet.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://bv.bookmarksfly.cn

[K05] 深拷贝对象
来源：http://op.huixiangedu.cn

Py:   copy.deepcopy(obj)
来源：http://uy.huanxung.cn

PHP:  unserialize(serialize($obj));
来源：http://ma.shxzukj.cn

JS:   structuredClone(obj)
来源：http://xa.huixiangedu.cn

TS:   structuredClone(obj)
来源：http://ei.yuntaijiaju.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ba.muxihuayi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ie.gzmigu.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://az.huanxung.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://la.jianghongdianzi.cn

[K06] 解析 URL 查询串
来源：http://bz.hahajie.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://tw.nszjky.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wk.9csxet.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://io.panjiajie.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kr.9csxet.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://te.wgjwhj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://qu.haigaiapp.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://kl.chemitech.net.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ez.yuexingan06.cn

[K07] 进制转换
来源：http://du.jianghongdianzi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wj.nszjky.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://go.newstarts.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://lz.gzmigu.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://xw.gzmigu.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://cb.newstarts.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://rs.nszjky.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://sx.szsharing.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wt.hahajie.cn

[K08] 二进制序列化（非 JSON）
来源：http://ag.jctech888.com.cn

Py:   pickle.dumps(obj)
来源：http://wc.bookmarksfly.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://pb.9csxet.cn

JS:   v8.serialize(obj)        // Node
来源：http://uj.gzmigu.cn

TS:   v8.serialize(obj)        // Node
来源：http://pc.muxihuayi.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://vb.haigaiapp.cn

Go:   encoding/gob
来源：http://rz.nicolike.cn

Ruby: Marshal.dump(obj)
来源：http://zb.shxzskj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mt.bjjhwx.cn

================================================================================
来源：http://wv.shxzskj.cn

L. 网络请求
来源：http://fw.lnxyls.cn

================================================================================
来源：http://zw.shtwfgs.cn

[L01] 发送 GET 请求
来源：http://sr.jianghongdianzi.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://yx.shxzskj.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://rw.huixinmuqiang.cn

JS:   await fetch(url)
来源：http://iu.yuexingan06.cn

TS:   await fetch(url)
来源：http://zc.bookmarksfly.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://pd.huixinmuqiang.cn

Go:   resp, err := http.Get(url)
来源：http://bl.haigaiapp.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://nj.shxzskj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://vu.haigaiapp.cn

[L02] 发送 POST JSON
来源：http://gm.wgjwhj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://xw.panjiajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ok.bjjhwx.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://oy.huanxung.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fs.nicolike.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://bt.szsharing.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qs.muxihuayi.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ps.colortex.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://cs.nszjky.cn

[L03] 设置自定义请求头
来源：http://lm.shxzukj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://um.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://lc.shxzskj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cd.hahajie.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bt.huixinmuqiang.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://vq.wgjwhj.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ya.asd995.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://dm.shxzukj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://dk.hnjuh.cn

[L04] 设置超时
来源：http://fs.jctech888.com.cn

Py:   requests.get(url, timeout=5)
来源：http://bh.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mi.asd995.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xv.bookmarksfly.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://af.nicolike.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://pz.bookmarksfly.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://bd.hnjuh.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://zn.huixiangedu.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://xw.521024.cn

[L05] 上传文件（multipart）
来源：http://hc.huanxung.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://jk.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ue.haigaiapp.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://dt.9csxet.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xm.nicolike.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://lf.9csxet.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://br.hnjuh.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://dv.szxytkj.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://sf.bookmarksfly.cn

[L06] 解析响应为 JSON
来源：http://dg.521024.cn

Py:   resp.json()
来源：http://qe.hahajie.cn

PHP:  json_decode($body, true);
来源：http://xi.chemitech.net.cn

JS:   await resp.json()
来源：http://ju.bjjhwx.cn

TS:   await resp.json()
来源：http://ck.huixiangedu.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://rf.shtwfgs.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://da.wgjwhj.cn

Ruby: JSON.parse(resp.body)
来源：http://js.szsharing.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hj.yuntaijiaju.cn

[L07] 处理 HTTP 状态码
来源：http://wq.szxytkj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://pb.muxihuayi.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://pk.gzmigu.cn

JS:   resp.ok;  resp.status
来源：http://yn.yuntaijiaju.cn

TS:   resp.ok;  resp.status
来源：http://ho.asd995.cn

Java: resp.statusCode()
来源：http://xy.wgjwhj.cn

Go:   resp.StatusCode
来源：http://xd.jianghongdianzi.cn

Ruby: resp.code.to_i
来源：http://yy.bookmarksfly.cn

C#:   (int)resp.StatusCode
来源：http://gf.asd995.cn

[L08] 并发请求多个地址
来源：http://qy.colortex.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://fd.muxihuayi.cn

PHP:  curl_multi_init() 系列
来源：http://cl.nicolike.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dp.huixiangedu.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nw.panjiajie.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wu.huixiangedu.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://yo.szxytkj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://gq.gzmigu.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ev.colortex.cn

================================================================================
来源：http://od.bjjhwx.cn

M. 命令行 / 进程 / 环境
来源：http://zu.nicolike.cn

================================================================================
来源：http://xj.yuntaijiaju.cn

[M01] 读取命令行参数
来源：http://is.shxzskj.cn

Py:   sys.argv[1:]
来源：http://fi.chemitech.net.cn

PHP:  $argv;  $argc;
来源：http://ll.shtwfgs.cn

JS:   process.argv.slice(2)
来源：http://dt.panjiajie.cn

TS:   process.argv.slice(2)
来源：http://hi.haigaiapp.cn

Java: args 数组（main 方法参数）
来源：http://ky.newstarts.cn

Go:   os.Args[1:]
来源：http://mf.huixinmuqiang.cn

Ruby: ARGV
来源：http://dg.shtwfgs.cn

C#:   args 数组（Main 方法参数）
来源：http://si.shtwfgs.cn

[M02] 读取环境变量
来源：http://gy.gzmigu.cn

Py:   os.environ.get("HOME")
来源：http://wn.colortex.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zk.shxzskj.cn

JS:   process.env.HOME
来源：http://kj.szxytkj.cn

TS:   process.env.HOME
来源：http://rt.wgjwhj.cn

Java: System.getenv("HOME")
来源：http://nt.newstarts.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ye.shxzskj.cn

Ruby: ENV["HOME"]
来源：http://os.asd995.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ts.hnjuh.cn

[M03] 执行外部命令
来源：http://uf.hnjuh.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://je.nicolike.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://yf.nicolike.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://zn.haigaiapp.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://hm.gzmigu.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ld.jianghongdianzi.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://wz.bookmarksfly.cn

Ruby: system("ls -l");  `ls -l`
来源：http://xb.jianghongdianzi.cn

C#:   Process.Start("ls", "-l");
来源：http://dk.shxzukj.cn

[M04] 获取当前工作目录
来源：http://xu.szsharing.cn

Py:   os.getcwd()
来源：http://pt.shtwfgs.cn

PHP:  getcwd();
来源：http://fn.lnxyls.cn

JS:   process.cwd()
来源：http://hb.asd995.cn

TS:   process.cwd()
来源：http://yx.hnjuh.cn

Java: Path.of("").toAbsolutePath()
来源：http://hn.bjjhwx.cn

Go:   os.Getwd()
来源：http://lj.gzmigu.cn

Ruby: Dir.pwd
来源：http://gw.huixiangedu.cn

C#:   Directory.GetCurrentDirectory()
来源：http://rp.jianghongdianzi.cn

[M05] 设置退出码
来源：http://ln.bookmarksfly.cn

Py:   sys.exit(1)
来源：http://or.jctech888.com.cn

PHP:  exit(1);
来源：http://da.shxzukj.cn

JS:   process.exit(1)
来源：http://ey.asd995.cn

TS:   process.exit(1)
来源：http://vj.panjiajie.cn

Java: System.exit(1)
来源：http://mu.nicolike.cn

Go:   os.Exit(1)
来源：http://sk.hahajie.cn

Ruby: exit 1
来源：http://ap.colortex.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://vu.gzmigu.cn

[M06] 向标准错误输出
来源：http://vf.shtwfgs.cn

Py:   print("err", file=sys.stderr)
来源：http://ly.jianghongdianzi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://rh.panjiajie.cn

JS:   console.error("err")
来源：http://me.jctech888.com.cn

TS:   console.error("err")
来源：http://ck.haigaiapp.cn

Java: System.err.println("err")
来源：http://dj.huixiangedu.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://id.jctech888.com.cn

Ruby: warn "err"
来源：http://ul.bookmarksfly.cn

C#:   Console.Error.WriteLine("err")
来源：http://cl.bjjhwx.cn

[M07] 判断是否为主入口
来源：http://bk.shtwfgs.cn

Py:   if __name__ == "__main__":
来源：http://us.huixiangedu.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://pv.muxihuayi.cn

JS:   require.main === module
来源：http://qn.hahajie.cn

TS:   require.main === module
来源：http://yh.shtwfgs.cn

Java: public static void main(String[] args)
来源：http://zn.bookmarksfly.cn

Go:   func main()
来源：http://uw.jctech888.com.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://yv.huanxung.cn

C#:   static void Main(string[] args)
来源：http://tl.hahajie.cn

[M08] 获取系统与运行时信息
来源：http://kp.huanxung.cn

Py:   platform.system();  platform.python_version()
来源：http://rv.huixiangedu.cn

PHP:  PHP_OS;  phpversion();
来源：http://qb.szxytkj.cn

JS:   process.platform;  process.version
来源：http://sk.shtwfgs.cn

TS:   process.platform;  process.version
来源：http://xs.chemitech.net.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ww.bjjhwx.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://we.colortex.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ua.chemitech.net.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://fk.nicolike.cn

================================================================================
来源：http://mb.yuexingan06.cn

N. 数据结构与算法
来源：http://zn.bjjhwx.cn

================================================================================
来源：http://by.asd995.cn

[N01] 二分查找（有序数组）
来源：http://rm.hahajie.cn

Py:   bisect.bisect_left(arr, x)
来源：http://vg.colortex.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ni.jianghongdianzi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wd.haigaiapp.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qt.hnjuh.cn

Java: Arrays.binarySearch(arr, x)
来源：http://zn.bookmarksfly.cn

Go:   sort.SearchInts(arr, x)
来源：http://ro.nicolike.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ky.chemitech.net.cn

C#:   Array.BinarySearch(arr, x)
来源：http://fn.colortex.cn

[N02] 排序（工程实践用内置实现）
来源：http://yw.colortex.cn

Py:   sorted(arr);  arr.sort()
来源：http://ba.szxytkj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://if.muxihuayi.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://xs.wgjwhj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://hr.asd995.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://yd.gzmigu.cn

Go:   slices.Sort(arr)
来源：http://qn.521024.cn

Ruby: arr.sort
来源：http://pd.gzmigu.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ub.wgjwhj.cn

[N03] 快速排序（分治示例）
来源：http://uv.panjiajie.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ah.newstarts.cn


<!-- 参考信息 -->