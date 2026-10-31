代发 wailian999

Java: Duration.between(start, end).toSeconds()
来源：http://ia.jianghongdianzi.cn

Go:   end.Sub(start).Hours()
来源：http://dr.huixiangedu.cn

Ruby: end - start                 # 返回秒数
来源：http://wm.szxytkj.cn

C#:   (end - start).TotalSeconds
来源：http://gb.newstarts.cn

[J07] 比较两个日期
来源：http://rp.bjjhwx.cn

Py:   d1 < d2;  d1 == d2
来源：http://de.hnjuh.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://tb.newstarts.cn

JS:   d1.getTime() < d2.getTime()
来源：http://os.newstarts.cn

TS:   d1.getTime() < d2.getTime()
来源：http://fi.muxihuayi.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://do.hahajie.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://jq.huixinmuqiang.cn

Ruby: d1 < d2;  d1 == d2
来源：http://fu.szxytkj.cn

C#:   d1 < d2;  d1 == d2
来源：http://pu.shxzskj.cn

[J08] 提取年月日与星期
来源：http://zo.haigaiapp.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ua.yuntaijiaju.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://je.jianghongdianzi.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://yg.bjjhwx.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://pl.huixiangedu.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://gg.colortex.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://bf.colortex.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://fx.bjjhwx.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://pc.szsharing.cn

[J09] 时区处理
来源：http://wo.szxytkj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://uu.wgjwhj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://jz.chemitech.net.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vr.yuexingan06.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bf.shtwfgs.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://qk.wgjwhj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wp.521024.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ft.9csxet.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://nw.jctech888.com.cn

[J10] 取今天 / 本月第一天
来源：http://lg.colortex.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://yz.szsharing.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://gp.jctech888.com.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://db.szsharing.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://sw.9csxet.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://dt.nicolike.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://fm.jianghongdianzi.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://di.521024.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://jh.wgjwhj.cn

================================================================================
来源：http://uu.nicolike.cn

K. JSON 与序列化
来源：http://ka.wgjwhj.cn

================================================================================
来源：http://be.newstarts.cn

[K01] 对象转 JSON 字符串
来源：http://gk.lnxyls.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://eq.huanxung.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://yn.panjiajie.cn

JS:   JSON.stringify(obj)
来源：http://ye.szxytkj.cn

TS:   JSON.stringify(obj)
来源：http://gf.szsharing.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ip.huixiangedu.cn

Go:   json.Marshal(obj)
来源：http://xa.jctech888.com.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ht.wgjwhj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://bz.huixinmuqiang.cn

[K02] JSON 字符串转对象
来源：http://uj.bjjhwx.cn

Py:   json.loads(s)
来源：http://tq.9csxet.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://jr.chemitech.net.cn

JS:   JSON.parse(s)
来源：http://do.huixinmuqiang.cn

TS:   JSON.parse(s)
来源：http://kl.nszjky.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ua.huanxung.cn

Go:   json.Unmarshal(data, &v)
来源：http://ov.bjjhwx.cn

Ruby: JSON.parse(s)
来源：http://qi.jianghongdianzi.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ri.nicolike.cn

[K03] JSON 美化输出（带缩进）
来源：http://ym.asd995.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://bf.bookmarksfly.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://gk.panjiajie.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://zh.haigaiapp.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://yc.newstarts.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://yq.jctech888.com.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://rr.nicolike.cn

Ruby: JSON.pretty_generate(obj)
来源：http://jr.wgjwhj.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://nd.newstarts.cn

[K04] 读取 JSON 文件
来源：http://up.jctech888.com.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wg.hnjuh.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://gc.jianghongdianzi.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hp.521024.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fz.chemitech.net.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://bi.panjiajie.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mq.9csxet.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://tl.gzmigu.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://nr.nicolike.cn

[K05] 深拷贝对象
来源：http://xj.szsharing.cn

Py:   copy.deepcopy(obj)
来源：http://bd.shtwfgs.cn

PHP:  unserialize(serialize($obj));
来源：http://mz.nicolike.cn

JS:   structuredClone(obj)
来源：http://oi.9csxet.cn

TS:   structuredClone(obj)
来源：http://mb.wgjwhj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://mu.lnxyls.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hy.lnxyls.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ov.haigaiapp.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://op.huixinmuqiang.cn

[K06] 解析 URL 查询串
来源：http://ky.haigaiapp.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://oq.shtwfgs.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://nj.shxzskj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sa.9csxet.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wq.szsharing.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://lm.hnjuh.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://mc.newstarts.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ou.yuexingan06.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://qy.huanxung.cn

[K07] 进制转换
来源：http://sx.szsharing.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://nt.szsharing.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://pc.jctech888.com.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://vf.jianghongdianzi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qn.haigaiapp.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://bl.panjiajie.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ee.asd995.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://rj.shxzukj.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://be.hnjuh.cn

[K08] 二进制序列化（非 JSON）
来源：http://qb.huixinmuqiang.cn

Py:   pickle.dumps(obj)
来源：http://ip.lnxyls.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://yu.shxzukj.cn

JS:   v8.serialize(obj)        // Node
来源：http://et.jctech888.com.cn

TS:   v8.serialize(obj)        // Node
来源：http://af.bookmarksfly.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hk.huixiangedu.cn

Go:   encoding/gob
来源：http://me.shxzskj.cn

Ruby: Marshal.dump(obj)
来源：http://fy.yuexingan06.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://pk.jianghongdianzi.cn

================================================================================
来源：http://ji.nszjky.cn

L. 网络请求
来源：http://ga.szsharing.cn

================================================================================
来源：http://ow.shtwfgs.cn

[L01] 发送 GET 请求
来源：http://eq.yuntaijiaju.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://bz.chemitech.net.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ku.bjjhwx.cn

JS:   await fetch(url)
来源：http://df.huixinmuqiang.cn

TS:   await fetch(url)
来源：http://yo.huixiangedu.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ti.jianghongdianzi.cn

Go:   resp, err := http.Get(url)
来源：http://mx.newstarts.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://lh.shtwfgs.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://jx.newstarts.cn

[L02] 发送 POST JSON
来源：http://aa.bjjhwx.cn

Py:   requests.post(url, json={"a": 1})
来源：http://hu.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://lz.nicolike.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wr.nszjky.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xp.9csxet.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qy.colortex.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://az.chemitech.net.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://bf.gzmigu.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ck.huanxung.cn

[L03] 设置自定义请求头
来源：http://re.huixiangedu.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://lw.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://vi.huixiangedu.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://um.huixinmuqiang.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rs.shxzukj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://pg.huixiangedu.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://dn.szsharing.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://tg.bookmarksfly.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ed.asd995.cn

[L04] 设置超时
来源：http://mi.nicolike.cn

Py:   requests.get(url, timeout=5)
来源：http://zi.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://un.wgjwhj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://oh.colortex.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jx.bookmarksfly.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ot.chemitech.net.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hw.haigaiapp.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://cd.haigaiapp.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ar.newstarts.cn

[L05] 上传文件（multipart）
来源：http://yk.521024.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wg.yuntaijiaju.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ty.yuexingan06.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ru.bookmarksfly.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://gx.bookmarksfly.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://jb.jctech888.com.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://bw.huixiangedu.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://kd.hahajie.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://lz.muxihuayi.cn

[L06] 解析响应为 JSON
来源：http://oj.asd995.cn

Py:   resp.json()
来源：http://ng.bjjhwx.cn

PHP:  json_decode($body, true);
来源：http://kl.huanxung.cn

JS:   await resp.json()
来源：http://wv.yuexingan06.cn

TS:   await resp.json()
来源：http://as.szxytkj.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://eg.huixinmuqiang.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://vy.521024.cn

Ruby: JSON.parse(resp.body)
来源：http://et.bookmarksfly.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wp.colortex.cn

[L07] 处理 HTTP 状态码
来源：http://ik.hnjuh.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://zf.gzmigu.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://pz.lnxyls.cn

JS:   resp.ok;  resp.status
来源：http://nq.szxytkj.cn

TS:   resp.ok;  resp.status
来源：http://vl.shxzukj.cn

Java: resp.statusCode()
来源：http://eg.huixinmuqiang.cn

Go:   resp.StatusCode
来源：http://ce.muxihuayi.cn

Ruby: resp.code.to_i
来源：http://pw.chemitech.net.cn

C#:   (int)resp.StatusCode
来源：http://vt.jianghongdianzi.cn

[L08] 并发请求多个地址
来源：http://uo.9csxet.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hn.wgjwhj.cn

PHP:  curl_multi_init() 系列
来源：http://kn.huixinmuqiang.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bp.huixiangedu.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ow.szsharing.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://zm.asd995.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://lm.lnxyls.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://xw.hahajie.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://rt.chemitech.net.cn

================================================================================
来源：http://ze.huixiangedu.cn

M. 命令行 / 进程 / 环境
来源：http://dw.newstarts.cn

================================================================================
来源：http://jc.muxihuayi.cn

[M01] 读取命令行参数
来源：http://oz.haigaiapp.cn

Py:   sys.argv[1:]
来源：http://ut.jctech888.com.cn

PHP:  $argv;  $argc;
来源：http://wi.colortex.cn

JS:   process.argv.slice(2)
来源：http://pi.chemitech.net.cn

TS:   process.argv.slice(2)
来源：http://yt.shxzukj.cn

Java: args 数组（main 方法参数）
来源：http://jw.bookmarksfly.cn

Go:   os.Args[1:]
来源：http://pj.9csxet.cn

Ruby: ARGV
来源：http://ji.nszjky.cn

C#:   args 数组（Main 方法参数）
来源：http://qw.szxytkj.cn

[M02] 读取环境变量
来源：http://si.yuexingan06.cn

Py:   os.environ.get("HOME")
来源：http://sl.huanxung.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://xn.nicolike.cn

JS:   process.env.HOME
来源：http://oa.nicolike.cn

TS:   process.env.HOME
来源：http://ws.panjiajie.cn

Java: System.getenv("HOME")
来源：http://xp.panjiajie.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://pu.nszjky.cn

Ruby: ENV["HOME"]
来源：http://gl.jctech888.com.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ji.newstarts.cn

[M03] 执行外部命令
来源：http://fb.colortex.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ti.haigaiapp.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ty.bookmarksfly.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://yo.muxihuayi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://pt.yuexingan06.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://yc.nicolike.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://jt.huixiangedu.cn

Ruby: system("ls -l");  `ls -l`
来源：http://rt.521024.cn

C#:   Process.Start("ls", "-l");
来源：http://hl.huanxung.cn

[M04] 获取当前工作目录
来源：http://pq.shxzukj.cn

Py:   os.getcwd()
来源：http://vn.lnxyls.cn

PHP:  getcwd();
来源：http://mw.521024.cn

JS:   process.cwd()
来源：http://to.yuexingan06.cn

TS:   process.cwd()
来源：http://sx.asd995.cn

Java: Path.of("").toAbsolutePath()
来源：http://ju.jianghongdianzi.cn

Go:   os.Getwd()
来源：http://fs.bookmarksfly.cn

Ruby: Dir.pwd
来源：http://ma.hnjuh.cn

C#:   Directory.GetCurrentDirectory()
来源：http://xm.huanxung.cn

[M05] 设置退出码
来源：http://xn.yuntaijiaju.cn

Py:   sys.exit(1)
来源：http://xi.yuntaijiaju.cn

PHP:  exit(1);
来源：http://xi.nszjky.cn

JS:   process.exit(1)
来源：http://pz.shxzskj.cn

TS:   process.exit(1)
来源：http://pz.9csxet.cn

Java: System.exit(1)
来源：http://ts.shtwfgs.cn

Go:   os.Exit(1)
来源：http://cw.huixiangedu.cn

Ruby: exit 1
来源：http://fe.lnxyls.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://tu.szsharing.cn

[M06] 向标准错误输出
来源：http://ta.muxihuayi.cn

Py:   print("err", file=sys.stderr)
来源：http://il.bookmarksfly.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://lf.yuntaijiaju.cn

JS:   console.error("err")
来源：http://ax.colortex.cn

TS:   console.error("err")
来源：http://fy.yuntaijiaju.cn

Java: System.err.println("err")
来源：http://al.yuexingan06.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ek.nszjky.cn

Ruby: warn "err"
来源：http://gm.huixinmuqiang.cn

C#:   Console.Error.WriteLine("err")
来源：http://sr.shxzskj.cn

[M07] 判断是否为主入口
来源：http://fl.yuntaijiaju.cn

Py:   if __name__ == "__main__":
来源：http://fe.huanxung.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ja.szxytkj.cn

JS:   require.main === module
来源：http://rm.panjiajie.cn

TS:   require.main === module
来源：http://tk.asd995.cn

Java: public static void main(String[] args)
来源：http://eo.lnxyls.cn

Go:   func main()
来源：http://ml.jianghongdianzi.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://re.newstarts.cn

C#:   static void Main(string[] args)
来源：http://xn.huixiangedu.cn

[M08] 获取系统与运行时信息
来源：http://og.jianghongdianzi.cn

Py:   platform.system();  platform.python_version()
来源：http://dq.newstarts.cn

PHP:  PHP_OS;  phpversion();
来源：http://by.muxihuayi.cn

JS:   process.platform;  process.version
来源：http://aa.bjjhwx.cn

TS:   process.platform;  process.version
来源：http://kz.lnxyls.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://sf.nszjky.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ur.yuexingan06.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hy.hnjuh.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://lu.shtwfgs.cn

================================================================================
来源：http://ug.colortex.cn

N. 数据结构与算法
来源：http://lw.newstarts.cn

================================================================================
来源：http://en.shtwfgs.cn

[N01] 二分查找（有序数组）
来源：http://wo.bookmarksfly.cn

Py:   bisect.bisect_left(arr, x)
来源：http://tz.haigaiapp.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://qj.haigaiapp.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gh.huixiangedu.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tw.huixinmuqiang.cn

Java: Arrays.binarySearch(arr, x)
来源：http://so.newstarts.cn

Go:   sort.SearchInts(arr, x)
来源：http://qj.huanxung.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://hg.gzmigu.cn

C#:   Array.BinarySearch(arr, x)
来源：http://zy.bookmarksfly.cn

[N02] 排序（工程实践用内置实现）
来源：http://zl.muxihuayi.cn

Py:   sorted(arr);  arr.sort()
来源：http://ob.wgjwhj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://vl.muxihuayi.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://bp.hahajie.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://en.nszjky.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://xb.newstarts.cn

Go:   slices.Sort(arr)
来源：http://vd.asd995.cn

Ruby: arr.sort
来源：http://qb.wgjwhj.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://qt.bjjhwx.cn

[N03] 快速排序（分治示例）
来源：http://gf.yuntaijiaju.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://cr.szxytkj.cn

PHP:  // 递归实现，或用 usort
来源：http://nu.jianghongdianzi.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gy.huixinmuqiang.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bx.newstarts.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://pg.yuexingan06.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wd.huixinmuqiang.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://gl.wgjwhj.cn

C#:   // 手写递归，或 Array.Sort
来源：http://yx.521024.cn

[N04] 斐波那契数列
来源：http://tg.yuntaijiaju.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zr.wgjwhj.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://qq.asd995.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yv.jctech888.com.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cb.nszjky.cn


<!-- 参考信息 -->