代发 wailian999

Java: Duration.between(start, end).toSeconds()
来源：http://eh.huixiangedu.cn

Go:   end.Sub(start).Hours()
来源：http://sf.hahajie.cn

Ruby: end - start                 # 返回秒数
来源：http://yi.szsharing.cn

C#:   (end - start).TotalSeconds
来源：http://jn.shtwfgs.cn

[J07] 比较两个日期
来源：http://im.panjiajie.cn

Py:   d1 < d2;  d1 == d2
来源：http://vg.gzmigu.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ma.hahajie.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ee.chemitech.net.cn

TS:   d1.getTime() < d2.getTime()
来源：http://pp.hahajie.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://qp.bjjhwx.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://pn.huixinmuqiang.cn

Ruby: d1 < d2;  d1 == d2
来源：http://sr.nszjky.cn

C#:   d1 < d2;  d1 == d2
来源：http://pj.shxzukj.cn

[J08] 提取年月日与星期
来源：http://re.yuntaijiaju.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://df.shxzskj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mw.521024.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://zi.nszjky.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://nd.nicolike.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wl.shxzukj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://eg.lnxyls.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ah.9csxet.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://os.521024.cn

[J09] 时区处理
来源：http://yh.wgjwhj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ww.szxytkj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wg.bjjhwx.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://af.yuexingan06.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ss.bjjhwx.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://pe.asd995.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://bv.bookmarksfly.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ww.lnxyls.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://db.haigaiapp.cn

[J10] 取今天 / 本月第一天
来源：http://kg.nszjky.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://so.shtwfgs.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://yo.wgjwhj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://rs.huixiangedu.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hx.newstarts.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://lh.hahajie.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://tb.haigaiapp.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://iw.hnjuh.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://np.jctech888.com.cn

================================================================================
来源：http://uv.shxzukj.cn

K. JSON 与序列化
来源：http://bq.huanxung.cn

================================================================================
来源：http://yu.jctech888.com.cn

[K01] 对象转 JSON 字符串
来源：http://mc.bookmarksfly.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://xf.lnxyls.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://eq.gzmigu.cn

JS:   JSON.stringify(obj)
来源：http://nq.yuntaijiaju.cn

TS:   JSON.stringify(obj)
来源：http://ds.yuntaijiaju.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ye.yuntaijiaju.cn

Go:   json.Marshal(obj)
来源：http://xo.shtwfgs.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ku.lnxyls.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://rb.yuexingan06.cn

[K02] JSON 字符串转对象
来源：http://dy.521024.cn

Py:   json.loads(s)
来源：http://tn.shxzukj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ti.yuntaijiaju.cn

JS:   JSON.parse(s)
来源：http://ju.hnjuh.cn

TS:   JSON.parse(s)
来源：http://rf.hahajie.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://or.chemitech.net.cn

Go:   json.Unmarshal(data, &v)
来源：http://dr.jianghongdianzi.cn

Ruby: JSON.parse(s)
来源：http://gr.muxihuayi.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://oj.jianghongdianzi.cn

[K03] JSON 美化输出（带缩进）
来源：http://mf.shxzskj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://nv.nicolike.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://th.9csxet.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://fl.szsharing.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://js.shtwfgs.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qj.newstarts.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://na.yuntaijiaju.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ec.9csxet.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://zc.asd995.cn

[K04] 读取 JSON 文件
来源：http://fr.asd995.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://sp.jctech888.com.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://xr.jctech888.com.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mn.nicolike.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vm.lnxyls.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://cn.szsharing.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ys.nszjky.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://kx.haigaiapp.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://pb.9csxet.cn

[K05] 深拷贝对象
来源：http://wf.huanxung.cn

Py:   copy.deepcopy(obj)
来源：http://vp.gzmigu.cn

PHP:  unserialize(serialize($obj));
来源：http://zn.haigaiapp.cn

JS:   structuredClone(obj)
来源：http://oo.shxzskj.cn

TS:   structuredClone(obj)
来源：http://np.lnxyls.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://kf.newstarts.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qn.jianghongdianzi.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://bx.nszjky.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://zo.huixiangedu.cn

[K06] 解析 URL 查询串
来源：http://jr.bookmarksfly.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ch.muxihuayi.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://dy.nicolike.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ov.bjjhwx.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kv.muxihuayi.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://kz.jctech888.com.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://bi.nicolike.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://pz.shxzukj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://gu.shxzskj.cn

[K07] 进制转换
来源：http://ny.hnjuh.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://qi.bjjhwx.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://em.9csxet.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://co.asd995.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://fr.asd995.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://lm.colortex.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://uh.521024.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ku.9csxet.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://xo.bjjhwx.cn

[K08] 二进制序列化（非 JSON）
来源：http://ax.huanxung.cn

Py:   pickle.dumps(obj)
来源：http://ia.bjjhwx.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://rx.hahajie.cn

JS:   v8.serialize(obj)        // Node
来源：http://zh.szxytkj.cn

TS:   v8.serialize(obj)        // Node
来源：http://zp.nicolike.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://kx.hnjuh.cn

Go:   encoding/gob
来源：http://wd.hahajie.cn

Ruby: Marshal.dump(obj)
来源：http://xw.jianghongdianzi.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qr.shxzukj.cn

================================================================================
来源：http://dj.yuexingan06.cn

L. 网络请求
来源：http://us.huixinmuqiang.cn

================================================================================
来源：http://wj.521024.cn

[L01] 发送 GET 请求
来源：http://xr.shtwfgs.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://di.nicolike.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://zp.shxzukj.cn

JS:   await fetch(url)
来源：http://mh.nszjky.cn

TS:   await fetch(url)
来源：http://ga.shxzukj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://fg.wgjwhj.cn

Go:   resp, err := http.Get(url)
来源：http://ad.nszjky.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://wg.newstarts.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://vj.nicolike.cn

[L02] 发送 POST JSON
来源：http://ug.yuexingan06.cn

Py:   requests.post(url, json={"a": 1})
来源：http://rq.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ie.panjiajie.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://iw.yuexingan06.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rv.nicolike.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://zt.newstarts.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://it.huanxung.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ew.asd995.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mh.nicolike.cn

[L03] 设置自定义请求头
来源：http://vi.shtwfgs.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ki.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://lu.lnxyls.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pk.nszjky.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kr.huixiangedu.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ef.yuntaijiaju.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://aj.huixinmuqiang.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://nm.gzmigu.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://xq.shxzukj.cn

[L04] 设置超时
来源：http://rb.yuntaijiaju.cn

Py:   requests.get(url, timeout=5)
来源：http://ck.hnjuh.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://sn.yuntaijiaju.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nj.bjjhwx.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://aw.huixinmuqiang.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hb.gzmigu.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ah.wgjwhj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://dx.521024.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://rg.huixiangedu.cn

[L05] 上传文件（multipart）
来源：http://xt.huanxung.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://fd.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mb.shxzskj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://xa.szsharing.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://dr.asd995.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ij.bjjhwx.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://fa.lnxyls.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ri.lnxyls.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://id.shxzukj.cn

[L06] 解析响应为 JSON
来源：http://ia.bookmarksfly.cn

Py:   resp.json()
来源：http://ru.lnxyls.cn

PHP:  json_decode($body, true);
来源：http://qr.huanxung.cn

JS:   await resp.json()
来源：http://hh.9csxet.cn

TS:   await resp.json()
来源：http://sj.wgjwhj.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://xn.nicolike.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://kj.jctech888.com.cn

Ruby: JSON.parse(resp.body)
来源：http://az.jianghongdianzi.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://qw.haigaiapp.cn

[L07] 处理 HTTP 状态码
来源：http://tp.9csxet.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://li.shtwfgs.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://kw.wgjwhj.cn

JS:   resp.ok;  resp.status
来源：http://dc.hnjuh.cn

TS:   resp.ok;  resp.status
来源：http://xy.szxytkj.cn

Java: resp.statusCode()
来源：http://ih.huixiangedu.cn

Go:   resp.StatusCode
来源：http://ge.shxzskj.cn

Ruby: resp.code.to_i
来源：http://dw.bjjhwx.cn

C#:   (int)resp.StatusCode
来源：http://jo.nszjky.cn

[L08] 并发请求多个地址
来源：http://rp.huanxung.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://gz.shxzskj.cn

PHP:  curl_multi_init() 系列
来源：http://iy.asd995.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ly.szsharing.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hq.asd995.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://lr.huanxung.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://bp.lnxyls.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ho.hnjuh.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://qg.huixinmuqiang.cn

================================================================================
来源：http://zh.newstarts.cn

M. 命令行 / 进程 / 环境
来源：http://vp.521024.cn

================================================================================
来源：http://yj.wgjwhj.cn

[M01] 读取命令行参数
来源：http://vc.hnjuh.cn

Py:   sys.argv[1:]
来源：http://im.muxihuayi.cn

PHP:  $argv;  $argc;
来源：http://pf.hnjuh.cn

JS:   process.argv.slice(2)
来源：http://wd.gzmigu.cn

TS:   process.argv.slice(2)
来源：http://go.gzmigu.cn

Java: args 数组（main 方法参数）
来源：http://ci.haigaiapp.cn

Go:   os.Args[1:]
来源：http://oz.wgjwhj.cn

Ruby: ARGV
来源：http://hf.szxytkj.cn

C#:   args 数组（Main 方法参数）
来源：http://zv.shxzskj.cn

[M02] 读取环境变量
来源：http://oo.shxzukj.cn

Py:   os.environ.get("HOME")
来源：http://ha.chemitech.net.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ua.huixinmuqiang.cn

JS:   process.env.HOME
来源：http://aq.jianghongdianzi.cn

TS:   process.env.HOME
来源：http://sn.shtwfgs.cn

Java: System.getenv("HOME")
来源：http://zl.jctech888.com.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://xq.szsharing.cn

Ruby: ENV["HOME"]
来源：http://re.shxzukj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://gr.yuntaijiaju.cn

[M03] 执行外部命令
来源：http://an.nszjky.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hf.jianghongdianzi.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://tm.huixinmuqiang.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://iy.muxihuayi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ii.nszjky.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://uk.521024.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://or.hahajie.cn

Ruby: system("ls -l");  `ls -l`
来源：http://hk.nszjky.cn

C#:   Process.Start("ls", "-l");
来源：http://qe.panjiajie.cn

[M04] 获取当前工作目录
来源：http://cl.colortex.cn

Py:   os.getcwd()
来源：http://hs.shtwfgs.cn

PHP:  getcwd();
来源：http://dw.lnxyls.cn

JS:   process.cwd()
来源：http://am.gzmigu.cn

TS:   process.cwd()
来源：http://ke.gzmigu.cn

Java: Path.of("").toAbsolutePath()
来源：http://wr.hnjuh.cn

Go:   os.Getwd()
来源：http://gv.yuntaijiaju.cn

Ruby: Dir.pwd
来源：http://id.bjjhwx.cn

C#:   Directory.GetCurrentDirectory()
来源：http://iy.newstarts.cn

[M05] 设置退出码
来源：http://yt.jianghongdianzi.cn

Py:   sys.exit(1)
来源：http://ae.panjiajie.cn

PHP:  exit(1);
来源：http://bk.shxzukj.cn

JS:   process.exit(1)
来源：http://cb.nszjky.cn

TS:   process.exit(1)
来源：http://us.shtwfgs.cn

Java: System.exit(1)
来源：http://oe.chemitech.net.cn

Go:   os.Exit(1)
来源：http://aj.jianghongdianzi.cn

Ruby: exit 1
来源：http://ed.jctech888.com.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ne.huanxung.cn

[M06] 向标准错误输出
来源：http://ru.huixiangedu.cn

Py:   print("err", file=sys.stderr)
来源：http://lm.chemitech.net.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://xr.521024.cn

JS:   console.error("err")
来源：http://wv.bjjhwx.cn

TS:   console.error("err")
来源：http://oo.bookmarksfly.cn

Java: System.err.println("err")
来源：http://wu.bjjhwx.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://pl.lnxyls.cn

Ruby: warn "err"
来源：http://qa.jianghongdianzi.cn

C#:   Console.Error.WriteLine("err")
来源：http://kn.chemitech.net.cn

[M07] 判断是否为主入口
来源：http://vy.shtwfgs.cn

Py:   if __name__ == "__main__":
来源：http://zf.nszjky.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://yb.haigaiapp.cn

JS:   require.main === module
来源：http://ec.muxihuayi.cn

TS:   require.main === module
来源：http://nw.lnxyls.cn

Java: public static void main(String[] args)
来源：http://nv.lnxyls.cn

Go:   func main()
来源：http://zi.shxzukj.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://at.shxzskj.cn

C#:   static void Main(string[] args)
来源：http://xl.haigaiapp.cn

[M08] 获取系统与运行时信息
来源：http://zk.wgjwhj.cn

Py:   platform.system();  platform.python_version()
来源：http://gc.huixiangedu.cn

PHP:  PHP_OS;  phpversion();
来源：http://hw.9csxet.cn

JS:   process.platform;  process.version
来源：http://kx.huixinmuqiang.cn

TS:   process.platform;  process.version
来源：http://dr.newstarts.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://uz.panjiajie.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://qn.nicolike.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://zk.colortex.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://st.newstarts.cn

================================================================================
来源：http://bo.bjjhwx.cn

N. 数据结构与算法
来源：http://ds.521024.cn

================================================================================
来源：http://bi.huixinmuqiang.cn

[N01] 二分查找（有序数组）
来源：http://mg.yuexingan06.cn

Py:   bisect.bisect_left(arr, x)
来源：http://wy.hahajie.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://vk.shxzskj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://az.hahajie.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gh.shtwfgs.cn

Java: Arrays.binarySearch(arr, x)
来源：http://sb.9csxet.cn

Go:   sort.SearchInts(arr, x)
来源：http://rh.521024.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://db.asd995.cn

C#:   Array.BinarySearch(arr, x)
来源：http://uj.asd995.cn

[N02] 排序（工程实践用内置实现）
来源：http://ho.huixinmuqiang.cn

Py:   sorted(arr);  arr.sort()
来源：http://mr.huixinmuqiang.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://pa.yuntaijiaju.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ik.lnxyls.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://mc.9csxet.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://lz.chemitech.net.cn

Go:   slices.Sort(arr)
来源：http://wz.521024.cn

Ruby: arr.sort
来源：http://dj.nicolike.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://fm.nicolike.cn

[N03] 快速排序（分治示例）
来源：http://tm.9csxet.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://kv.jianghongdianzi.cn

PHP:  // 递归实现，或用 usort
来源：http://ic.shtwfgs.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://oo.shtwfgs.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zm.bookmarksfly.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ua.521024.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://xk.hahajie.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://gt.panjiajie.cn

C#:   // 手写递归，或 Array.Sort
来源：http://vj.huixiangedu.cn

[N04] 斐波那契数列
来源：http://wx.huixiangedu.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://da.asd995.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://iy.huixiangedu.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ai.chemitech.net.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://uk.asd995.cn


<!-- 参考信息 -->