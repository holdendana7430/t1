代发 wailian999

Java: Duration.between(start, end).toSeconds()
来源：http://dq.huanxung.cn

Go:   end.Sub(start).Hours()
来源：http://la.huixinmuqiang.cn

Ruby: end - start                 # 返回秒数
来源：http://lo.asd995.cn

C#:   (end - start).TotalSeconds
来源：http://ph.bookmarksfly.cn

[J07] 比较两个日期
来源：http://mb.huanxung.cn

Py:   d1 < d2;  d1 == d2
来源：http://lj.panjiajie.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://yb.yuexingan06.cn

JS:   d1.getTime() < d2.getTime()
来源：http://tf.bjjhwx.cn

TS:   d1.getTime() < d2.getTime()
来源：http://lf.hnjuh.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://vq.jctech888.com.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://nv.colortex.cn

Ruby: d1 < d2;  d1 == d2
来源：http://an.521024.cn

C#:   d1 < d2;  d1 == d2
来源：http://nv.shxzskj.cn

[J08] 提取年月日与星期
来源：http://hf.yuntaijiaju.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://qu.chemitech.net.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hk.wgjwhj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://gs.nszjky.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ev.hnjuh.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://os.gzmigu.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://sx.muxihuayi.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://bv.szxytkj.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ai.szsharing.cn

[J09] 时区处理
来源：http://hi.huixinmuqiang.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ub.bjjhwx.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hk.nicolike.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vn.huixinmuqiang.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gh.haigaiapp.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ud.szsharing.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mo.haigaiapp.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://rn.muxihuayi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jp.panjiajie.cn

[J10] 取今天 / 本月第一天
来源：http://hn.huixiangedu.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://zv.nicolike.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wa.gzmigu.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ku.9csxet.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://cq.shxzukj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://jv.newstarts.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://gw.huixinmuqiang.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mn.yuexingan06.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://kq.haigaiapp.cn

================================================================================
来源：http://em.shtwfgs.cn

K. JSON 与序列化
来源：http://ax.bjjhwx.cn

================================================================================
来源：http://zo.asd995.cn

[K01] 对象转 JSON 字符串
来源：http://lr.haigaiapp.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://yl.nicolike.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://le.hahajie.cn

JS:   JSON.stringify(obj)
来源：http://no.gzmigu.cn

TS:   JSON.stringify(obj)
来源：http://cb.haigaiapp.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ui.9csxet.cn

Go:   json.Marshal(obj)
来源：http://rv.bjjhwx.cn

Ruby: obj.to_json                                     // require "json"
来源：http://bk.nszjky.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://he.hahajie.cn

[K02] JSON 字符串转对象
来源：http://mn.9csxet.cn

Py:   json.loads(s)
来源：http://dh.lnxyls.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ed.huanxung.cn

JS:   JSON.parse(s)
来源：http://fj.panjiajie.cn

TS:   JSON.parse(s)
来源：http://rh.hnjuh.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ca.colortex.cn

Go:   json.Unmarshal(data, &v)
来源：http://nj.9csxet.cn

Ruby: JSON.parse(s)
来源：http://nl.jctech888.com.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wd.521024.cn

[K03] JSON 美化输出（带缩进）
来源：http://dw.jctech888.com.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://gv.shxzukj.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://kd.huixiangedu.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://pb.nszjky.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://uv.yuexingan06.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://da.muxihuayi.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://zl.jianghongdianzi.cn

Ruby: JSON.pretty_generate(obj)
来源：http://xd.9csxet.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://yz.muxihuayi.cn

[K04] 读取 JSON 文件
来源：http://lt.huixiangedu.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wl.hahajie.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://js.colortex.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xa.asd995.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hb.wgjwhj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://nu.bjjhwx.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://es.nicolike.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ct.jctech888.com.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://vi.nszjky.cn

[K05] 深拷贝对象
来源：http://za.yuntaijiaju.cn

Py:   copy.deepcopy(obj)
来源：http://nm.wgjwhj.cn

PHP:  unserialize(serialize($obj));
来源：http://jh.bjjhwx.cn

JS:   structuredClone(obj)
来源：http://js.9csxet.cn

TS:   structuredClone(obj)
来源：http://cz.jianghongdianzi.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://pv.nicolike.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://rq.asd995.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://fz.bjjhwx.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://oc.nicolike.cn

[K06] 解析 URL 查询串
来源：http://sz.jctech888.com.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://gq.hnjuh.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://em.nszjky.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://st.gzmigu.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uo.huixinmuqiang.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://sw.bjjhwx.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://fm.chemitech.net.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://gj.521024.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wv.yuntaijiaju.cn

[K07] 进制转换
来源：http://yc.panjiajie.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://uv.jianghongdianzi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mz.muxihuayi.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mc.jianghongdianzi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://cr.521024.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://rl.chemitech.net.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://cn.haigaiapp.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://zc.yuexingan06.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://yg.gzmigu.cn

[K08] 二进制序列化（非 JSON）
来源：http://ef.bookmarksfly.cn

Py:   pickle.dumps(obj)
来源：http://sk.jctech888.com.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://gz.521024.cn

JS:   v8.serialize(obj)        // Node
来源：http://av.chemitech.net.cn

TS:   v8.serialize(obj)        // Node
来源：http://ta.hnjuh.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://az.9csxet.cn

Go:   encoding/gob
来源：http://mm.newstarts.cn

Ruby: Marshal.dump(obj)
来源：http://bb.szxytkj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://nh.asd995.cn

================================================================================
来源：http://oy.bookmarksfly.cn

L. 网络请求
来源：http://re.huanxung.cn

================================================================================
来源：http://by.shtwfgs.cn

[L01] 发送 GET 请求
来源：http://wk.bookmarksfly.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://vb.colortex.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ro.newstarts.cn

JS:   await fetch(url)
来源：http://tp.chemitech.net.cn

TS:   await fetch(url)
来源：http://hc.shtwfgs.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wk.asd995.cn

Go:   resp, err := http.Get(url)
来源：http://ho.521024.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://hb.shxzukj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ap.nicolike.cn

[L02] 发送 POST JSON
来源：http://rd.wgjwhj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://tm.gzmigu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wt.521024.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fz.hnjuh.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xs.bookmarksfly.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://bd.szsharing.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://la.jctech888.com.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ku.9csxet.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://rh.shxzskj.cn

[L03] 设置自定义请求头
来源：http://by.yuexingan06.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://fu.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ag.hnjuh.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fr.521024.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ox.colortex.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://vi.bjjhwx.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jp.colortex.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ud.bjjhwx.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://tx.nszjky.cn

[L04] 设置超时
来源：http://si.huixiangedu.cn

Py:   requests.get(url, timeout=5)
来源：http://pw.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://qa.newstarts.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lt.panjiajie.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://iq.szsharing.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ci.hahajie.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://eb.gzmigu.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hp.szxytkj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ik.nszjky.cn

[L05] 上传文件（multipart）
来源：http://zn.bookmarksfly.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ai.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://xf.huixiangedu.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://vd.huixinmuqiang.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://fh.hahajie.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mq.hnjuh.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://yy.hahajie.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ju.shtwfgs.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ti.chemitech.net.cn

[L06] 解析响应为 JSON
来源：http://po.wgjwhj.cn

Py:   resp.json()
来源：http://vi.521024.cn

PHP:  json_decode($body, true);
来源：http://ch.colortex.cn

JS:   await resp.json()
来源：http://mv.gzmigu.cn

TS:   await resp.json()
来源：http://ve.yuexingan06.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ce.9csxet.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://rl.9csxet.cn

Ruby: JSON.parse(resp.body)
来源：http://cp.shtwfgs.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ng.newstarts.cn

[L07] 处理 HTTP 状态码
来源：http://cz.bookmarksfly.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://tm.bjjhwx.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://kt.huanxung.cn

JS:   resp.ok;  resp.status
来源：http://yi.521024.cn

TS:   resp.ok;  resp.status
来源：http://hu.hahajie.cn

Java: resp.statusCode()
来源：http://yx.bjjhwx.cn

Go:   resp.StatusCode
来源：http://gm.jianghongdianzi.cn

Ruby: resp.code.to_i
来源：http://qp.bjjhwx.cn

C#:   (int)resp.StatusCode
来源：http://zf.szsharing.cn

[L08] 并发请求多个地址
来源：http://yl.hnjuh.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hd.521024.cn

PHP:  curl_multi_init() 系列
来源：http://un.nszjky.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ik.szsharing.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ul.9csxet.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://xc.shxzskj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://xy.huixiangedu.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://cs.shxzskj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ep.yuexingan06.cn

================================================================================
来源：http://kq.szxytkj.cn

M. 命令行 / 进程 / 环境
来源：http://em.gzmigu.cn

================================================================================
来源：http://zh.bookmarksfly.cn

[M01] 读取命令行参数
来源：http://ar.colortex.cn

Py:   sys.argv[1:]
来源：http://ps.colortex.cn

PHP:  $argv;  $argc;
来源：http://zd.huixinmuqiang.cn

JS:   process.argv.slice(2)
来源：http://fb.hnjuh.cn

TS:   process.argv.slice(2)
来源：http://iu.chemitech.net.cn

Java: args 数组（main 方法参数）
来源：http://na.yuntaijiaju.cn

Go:   os.Args[1:]
来源：http://vu.nicolike.cn

Ruby: ARGV
来源：http://oi.jianghongdianzi.cn

C#:   args 数组（Main 方法参数）
来源：http://kr.bjjhwx.cn

[M02] 读取环境变量
来源：http://fh.szsharing.cn

Py:   os.environ.get("HOME")
来源：http://ti.bookmarksfly.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://oa.colortex.cn

JS:   process.env.HOME
来源：http://zz.lnxyls.cn

TS:   process.env.HOME
来源：http://aj.hnjuh.cn

Java: System.getenv("HOME")
来源：http://ky.nicolike.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://fy.yuexingan06.cn

Ruby: ENV["HOME"]
来源：http://yi.newstarts.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://bw.asd995.cn

[M03] 执行外部命令
来源：http://ej.hahajie.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://tr.hahajie.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://bl.asd995.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://gq.colortex.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ll.521024.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://fu.huixinmuqiang.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://fg.shtwfgs.cn

Ruby: system("ls -l");  `ls -l`
来源：http://wi.colortex.cn

C#:   Process.Start("ls", "-l");
来源：http://eg.huanxung.cn

[M04] 获取当前工作目录
来源：http://wa.muxihuayi.cn

Py:   os.getcwd()
来源：http://tl.521024.cn

PHP:  getcwd();
来源：http://zh.bjjhwx.cn

JS:   process.cwd()
来源：http://ej.hahajie.cn

TS:   process.cwd()
来源：http://wh.nicolike.cn

Java: Path.of("").toAbsolutePath()
来源：http://ow.jctech888.com.cn

Go:   os.Getwd()
来源：http://br.9csxet.cn

Ruby: Dir.pwd
来源：http://fu.colortex.cn

C#:   Directory.GetCurrentDirectory()
来源：http://gg.jctech888.com.cn

[M05] 设置退出码
来源：http://qq.wgjwhj.cn

Py:   sys.exit(1)
来源：http://vz.nszjky.cn

PHP:  exit(1);
来源：http://mf.szxytkj.cn

JS:   process.exit(1)
来源：http://na.yuexingan06.cn

TS:   process.exit(1)
来源：http://ik.szsharing.cn

Java: System.exit(1)
来源：http://uk.shxzukj.cn

Go:   os.Exit(1)
来源：http://ta.hahajie.cn

Ruby: exit 1
来源：http://pm.shxzskj.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ch.bjjhwx.cn

[M06] 向标准错误输出
来源：http://jr.huixinmuqiang.cn

Py:   print("err", file=sys.stderr)
来源：http://sj.shxzukj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://tu.muxihuayi.cn

JS:   console.error("err")
来源：http://rp.newstarts.cn

TS:   console.error("err")
来源：http://ee.bjjhwx.cn

Java: System.err.println("err")
来源：http://lt.muxihuayi.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hg.bookmarksfly.cn

Ruby: warn "err"
来源：http://dl.shtwfgs.cn

C#:   Console.Error.WriteLine("err")
来源：http://ld.panjiajie.cn

[M07] 判断是否为主入口
来源：http://nj.lnxyls.cn

Py:   if __name__ == "__main__":
来源：http://wg.shxzukj.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://yd.muxihuayi.cn

JS:   require.main === module
来源：http://ih.colortex.cn

TS:   require.main === module
来源：http://uh.yuexingan06.cn

Java: public static void main(String[] args)
来源：http://dg.szsharing.cn

Go:   func main()
来源：http://km.muxihuayi.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://yy.jianghongdianzi.cn

C#:   static void Main(string[] args)
来源：http://yj.huixiangedu.cn

[M08] 获取系统与运行时信息
来源：http://di.bjjhwx.cn

Py:   platform.system();  platform.python_version()
来源：http://wr.szsharing.cn

PHP:  PHP_OS;  phpversion();
来源：http://ia.jctech888.com.cn

JS:   process.platform;  process.version
来源：http://qt.yuntaijiaju.cn

TS:   process.platform;  process.version
来源：http://je.shtwfgs.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://aq.yuntaijiaju.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://tz.shxzskj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://tv.bjjhwx.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://xo.yuntaijiaju.cn

================================================================================
来源：http://ac.shxzskj.cn

N. 数据结构与算法
来源：http://ga.shxzskj.cn

================================================================================
来源：http://jr.wgjwhj.cn

[N01] 二分查找（有序数组）
来源：http://uy.huixinmuqiang.cn

Py:   bisect.bisect_left(arr, x)
来源：http://qf.9csxet.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ag.colortex.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://om.hnjuh.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kv.9csxet.cn

Java: Arrays.binarySearch(arr, x)
来源：http://mu.nszjky.cn

Go:   sort.SearchInts(arr, x)
来源：http://qr.yuntaijiaju.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://qz.newstarts.cn

C#:   Array.BinarySearch(arr, x)
来源：http://dr.muxihuayi.cn

[N02] 排序（工程实践用内置实现）
来源：http://oo.shxzskj.cn

Py:   sorted(arr);  arr.sort()
来源：http://jy.shxzukj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://fp.wgjwhj.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://gb.szxytkj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://zj.asd995.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://uo.lnxyls.cn

Go:   slices.Sort(arr)
来源：http://io.521024.cn

Ruby: arr.sort
来源：http://sf.521024.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://gi.yuexingan06.cn

[N03] 快速排序（分治示例）
来源：http://dd.huixiangedu.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://um.wgjwhj.cn

PHP:  // 递归实现，或用 usort
来源：http://zr.nszjky.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mx.newstarts.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nn.yuntaijiaju.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://rc.panjiajie.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://cz.haigaiapp.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://tg.lnxyls.cn

C#:   // 手写递归，或 Array.Sort
来源：http://lr.bjjhwx.cn

[N04] 斐波那契数列
来源：http://do.nszjky.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://im.huanxung.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ld.asd995.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sh.wgjwhj.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ac.gzmigu.cn


<!-- 参考信息 -->