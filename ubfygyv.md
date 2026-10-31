代发 wailian999

Py:   (end - start).total_seconds()
来源：http://lm.nszjky.cn

PHP:  $end->diff($start)->days;
来源：http://rc.521024.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://cq.huixiangedu.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://jf.colortex.cn

Java: Duration.between(start, end).toSeconds()
来源：http://vm.panjiajie.cn

Go:   end.Sub(start).Hours()
来源：http://mp.nicolike.cn

Ruby: end - start                 # 返回秒数
来源：http://ev.szsharing.cn

C#:   (end - start).TotalSeconds
来源：http://jt.nszjky.cn

[J07] 比较两个日期
来源：http://io.szsharing.cn

Py:   d1 < d2;  d1 == d2
来源：http://ga.bjjhwx.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://zh.panjiajie.cn

JS:   d1.getTime() < d2.getTime()
来源：http://jq.gzmigu.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ru.szxytkj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://nk.shtwfgs.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://xp.huanxung.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ys.asd995.cn

C#:   d1 < d2;  d1 == d2
来源：http://yw.lnxyls.cn

[J08] 提取年月日与星期
来源：http://ln.nszjky.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ku.nicolike.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://rp.nicolike.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xb.yuexingan06.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ca.newstarts.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://xm.yuexingan06.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://gb.shxzskj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ff.muxihuayi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://sp.huanxung.cn

[J09] 时区处理
来源：http://nb.huanxung.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://dp.haigaiapp.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://si.bookmarksfly.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yw.jctech888.com.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://az.jianghongdianzi.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://cg.muxihuayi.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://vg.nszjky.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://wf.yuexingan06.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://st.muxihuayi.cn

[J10] 取今天 / 本月第一天
来源：http://ze.asd995.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://dj.szxytkj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://jp.nszjky.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://oh.szsharing.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qu.asd995.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://nb.huanxung.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://bf.shtwfgs.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://oz.gzmigu.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://fq.panjiajie.cn

================================================================================
来源：http://eo.shxzukj.cn

K. JSON 与序列化
来源：http://ti.panjiajie.cn

================================================================================
来源：http://ch.9csxet.cn

[K01] 对象转 JSON 字符串
来源：http://fw.jianghongdianzi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://py.szxytkj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://kt.asd995.cn

JS:   JSON.stringify(obj)
来源：http://pz.nszjky.cn

TS:   JSON.stringify(obj)
来源：http://nd.huanxung.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://dr.szsharing.cn

Go:   json.Marshal(obj)
来源：http://bm.hahajie.cn

Ruby: obj.to_json                                     // require "json"
来源：http://iq.shtwfgs.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://tv.yuntaijiaju.cn

[K02] JSON 字符串转对象
来源：http://my.hahajie.cn

Py:   json.loads(s)
来源：http://cz.szsharing.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://pc.yuntaijiaju.cn

JS:   JSON.parse(s)
来源：http://gk.nszjky.cn

TS:   JSON.parse(s)
来源：http://xk.huanxung.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jv.szsharing.cn

Go:   json.Unmarshal(data, &v)
来源：http://yr.yuexingan06.cn

Ruby: JSON.parse(s)
来源：http://ee.panjiajie.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://vo.nszjky.cn

[K03] JSON 美化输出（带缩进）
来源：http://lg.shxzukj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://jj.lnxyls.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qw.bookmarksfly.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://wr.huixiangedu.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://gq.gzmigu.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://jf.szsharing.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://jw.nszjky.cn

Ruby: JSON.pretty_generate(obj)
来源：http://rl.gzmigu.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://fm.shxzskj.cn

[K04] 读取 JSON 文件
来源：http://wg.jctech888.com.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://np.muxihuayi.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://by.bjjhwx.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fk.hahajie.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lv.yuexingan06.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://th.shtwfgs.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ik.colortex.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://af.hahajie.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mv.wgjwhj.cn

[K05] 深拷贝对象
来源：http://qc.nszjky.cn

Py:   copy.deepcopy(obj)
来源：http://hi.hahajie.cn

PHP:  unserialize(serialize($obj));
来源：http://or.bookmarksfly.cn

JS:   structuredClone(obj)
来源：http://tw.gzmigu.cn

TS:   structuredClone(obj)
来源：http://ju.panjiajie.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://es.szsharing.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://cd.bookmarksfly.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://tt.yuexingan06.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://kc.hahajie.cn

[K06] 解析 URL 查询串
来源：http://et.nicolike.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://zw.jianghongdianzi.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://lr.yuexingan06.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nx.bookmarksfly.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uz.hahajie.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mk.huanxung.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://if.nszjky.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://je.szsharing.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://nd.colortex.cn

[K07] 进制转换
来源：http://gh.huixiangedu.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://vn.jctech888.com.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://cq.haigaiapp.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hr.yuntaijiaju.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ys.shxzskj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ne.hnjuh.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hk.huixiangedu.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ys.hnjuh.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ra.chemitech.net.cn

[K08] 二进制序列化（非 JSON）
来源：http://lx.huanxung.cn

Py:   pickle.dumps(obj)
来源：http://po.jianghongdianzi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://hb.haigaiapp.cn

JS:   v8.serialize(obj)        // Node
来源：http://ti.nicolike.cn

TS:   v8.serialize(obj)        // Node
来源：http://ff.hahajie.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://jh.szxytkj.cn

Go:   encoding/gob
来源：http://mr.bjjhwx.cn

Ruby: Marshal.dump(obj)
来源：http://ul.521024.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://au.hnjuh.cn

================================================================================
来源：http://zh.nicolike.cn

L. 网络请求
来源：http://le.wgjwhj.cn

================================================================================
来源：http://aa.nicolike.cn

[L01] 发送 GET 请求
来源：http://es.lnxyls.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ww.panjiajie.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://jc.muxihuayi.cn

JS:   await fetch(url)
来源：http://ry.shxzukj.cn

TS:   await fetch(url)
来源：http://yj.shxzskj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qj.jctech888.com.cn

Go:   resp, err := http.Get(url)
来源：http://kn.jianghongdianzi.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://tv.hnjuh.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://an.chemitech.net.cn

[L02] 发送 POST JSON
来源：http://pw.huixiangedu.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ml.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://np.huixinmuqiang.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mu.nszjky.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zb.shxzskj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://zt.hnjuh.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mg.szxytkj.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ur.asd995.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ab.szxytkj.cn

[L03] 设置自定义请求头
来源：http://pg.huixinmuqiang.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://fv.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://jl.shxzukj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mj.yuntaijiaju.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ri.huixinmuqiang.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://fe.jctech888.com.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://eq.lnxyls.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://gq.jianghongdianzi.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://xm.colortex.cn

[L04] 设置超时
来源：http://tj.chemitech.net.cn

Py:   requests.get(url, timeout=5)
来源：http://tw.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://bn.huanxung.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nl.huixinmuqiang.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uq.huixiangedu.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wd.szxytkj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://sx.shtwfgs.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://xh.gzmigu.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://th.szxytkj.cn

[L05] 上传文件（multipart）
来源：http://am.colortex.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://eh.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://fm.nicolike.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://bq.wgjwhj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://kf.wgjwhj.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://yn.chemitech.net.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ru.colortex.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://bi.hahajie.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://vf.chemitech.net.cn

[L06] 解析响应为 JSON
来源：http://pq.521024.cn

Py:   resp.json()
来源：http://jt.haigaiapp.cn

PHP:  json_decode($body, true);
来源：http://mz.asd995.cn

JS:   await resp.json()
来源：http://ou.colortex.cn

TS:   await resp.json()
来源：http://vx.lnxyls.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://zp.nicolike.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://lg.szsharing.cn

Ruby: JSON.parse(resp.body)
来源：http://li.yuexingan06.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://vm.szxytkj.cn

[L07] 处理 HTTP 状态码
来源：http://ii.nicolike.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://so.bjjhwx.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://vm.huixinmuqiang.cn

JS:   resp.ok;  resp.status
来源：http://rm.huixinmuqiang.cn

TS:   resp.ok;  resp.status
来源：http://ja.yuntaijiaju.cn

Java: resp.statusCode()
来源：http://xu.huanxung.cn

Go:   resp.StatusCode
来源：http://ym.huixinmuqiang.cn

Ruby: resp.code.to_i
来源：http://dj.jctech888.com.cn

C#:   (int)resp.StatusCode
来源：http://xv.hnjuh.cn

[L08] 并发请求多个地址
来源：http://ox.521024.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://sf.hahajie.cn

PHP:  curl_multi_init() 系列
来源：http://fr.nszjky.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://up.colortex.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zf.wgjwhj.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://bl.yuexingan06.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qk.huanxung.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://dm.chemitech.net.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wk.huixinmuqiang.cn

================================================================================
来源：http://pk.521024.cn

M. 命令行 / 进程 / 环境
来源：http://gy.lnxyls.cn

================================================================================
来源：http://rt.nicolike.cn

[M01] 读取命令行参数
来源：http://re.shtwfgs.cn

Py:   sys.argv[1:]
来源：http://vr.yuntaijiaju.cn

PHP:  $argv;  $argc;
来源：http://zj.jianghongdianzi.cn

JS:   process.argv.slice(2)
来源：http://jr.lnxyls.cn

TS:   process.argv.slice(2)
来源：http://ti.shxzskj.cn

Java: args 数组（main 方法参数）
来源：http://hh.lnxyls.cn

Go:   os.Args[1:]
来源：http://sz.szxytkj.cn

Ruby: ARGV
来源：http://ed.bookmarksfly.cn

C#:   args 数组（Main 方法参数）
来源：http://ij.bookmarksfly.cn

[M02] 读取环境变量
来源：http://xy.panjiajie.cn

Py:   os.environ.get("HOME")
来源：http://se.huixiangedu.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://dj.newstarts.cn

JS:   process.env.HOME
来源：http://ml.lnxyls.cn

TS:   process.env.HOME
来源：http://mb.szsharing.cn

Java: System.getenv("HOME")
来源：http://go.nicolike.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ts.wgjwhj.cn

Ruby: ENV["HOME"]
来源：http://ef.chemitech.net.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://lf.panjiajie.cn

[M03] 执行外部命令
来源：http://cs.jctech888.com.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://nv.colortex.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://eo.hahajie.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ob.panjiajie.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ci.yuntaijiaju.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://yf.hahajie.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://dy.nszjky.cn

Ruby: system("ls -l");  `ls -l`
来源：http://kl.nicolike.cn

C#:   Process.Start("ls", "-l");
来源：http://ao.hnjuh.cn

[M04] 获取当前工作目录
来源：http://xo.hahajie.cn

Py:   os.getcwd()
来源：http://vu.shxzukj.cn

PHP:  getcwd();
来源：http://qu.huixinmuqiang.cn

JS:   process.cwd()
来源：http://sl.jianghongdianzi.cn

TS:   process.cwd()
来源：http://jf.colortex.cn

Java: Path.of("").toAbsolutePath()
来源：http://wr.newstarts.cn

Go:   os.Getwd()
来源：http://tw.szsharing.cn

Ruby: Dir.pwd
来源：http://nr.szxytkj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://dj.colortex.cn

[M05] 设置退出码
来源：http://ky.hahajie.cn

Py:   sys.exit(1)
来源：http://tx.hahajie.cn

PHP:  exit(1);
来源：http://ut.521024.cn

JS:   process.exit(1)
来源：http://pb.yuexingan06.cn

TS:   process.exit(1)
来源：http://xy.bookmarksfly.cn

Java: System.exit(1)
来源：http://ez.yuntaijiaju.cn

Go:   os.Exit(1)
来源：http://ly.yuexingan06.cn

Ruby: exit 1
来源：http://up.shtwfgs.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mj.wgjwhj.cn

[M06] 向标准错误输出
来源：http://hy.shxzskj.cn

Py:   print("err", file=sys.stderr)
来源：http://jh.huixiangedu.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://wn.hahajie.cn

JS:   console.error("err")
来源：http://ms.nszjky.cn

TS:   console.error("err")
来源：http://dq.haigaiapp.cn

Java: System.err.println("err")
来源：http://hi.hahajie.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://va.newstarts.cn

Ruby: warn "err"
来源：http://zn.bookmarksfly.cn

C#:   Console.Error.WriteLine("err")
来源：http://yh.bookmarksfly.cn

[M07] 判断是否为主入口
来源：http://op.newstarts.cn

Py:   if __name__ == "__main__":
来源：http://cq.szsharing.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://it.yuexingan06.cn

JS:   require.main === module
来源：http://xr.huanxung.cn

TS:   require.main === module
来源：http://yv.huanxung.cn

Java: public static void main(String[] args)
来源：http://eu.newstarts.cn

Go:   func main()
来源：http://gk.hnjuh.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://eg.wgjwhj.cn

C#:   static void Main(string[] args)
来源：http://mw.newstarts.cn

[M08] 获取系统与运行时信息
来源：http://uh.muxihuayi.cn

Py:   platform.system();  platform.python_version()
来源：http://je.nszjky.cn

PHP:  PHP_OS;  phpversion();
来源：http://lj.jianghongdianzi.cn

JS:   process.platform;  process.version
来源：http://ui.colortex.cn

TS:   process.platform;  process.version
来源：http://ph.haigaiapp.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://yc.jctech888.com.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ni.hnjuh.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://oh.9csxet.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://zi.yuntaijiaju.cn

================================================================================
来源：http://ej.bookmarksfly.cn

N. 数据结构与算法
来源：http://vb.gzmigu.cn

================================================================================
来源：http://ke.colortex.cn

[N01] 二分查找（有序数组）
来源：http://dh.panjiajie.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ln.yuntaijiaju.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://au.jctech888.com.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gg.chemitech.net.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nj.muxihuayi.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ce.huanxung.cn

Go:   sort.SearchInts(arr, x)
来源：http://uj.jctech888.com.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://sv.jctech888.com.cn

C#:   Array.BinarySearch(arr, x)
来源：http://gn.shtwfgs.cn

[N02] 排序（工程实践用内置实现）
来源：http://ek.lnxyls.cn

Py:   sorted(arr);  arr.sort()
来源：http://ir.wgjwhj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://eg.chemitech.net.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://hj.yuexingan06.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ti.asd995.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://or.huanxung.cn

Go:   slices.Sort(arr)
来源：http://vv.nszjky.cn

Ruby: arr.sort
来源：http://qc.9csxet.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ry.lnxyls.cn

[N03] 快速排序（分治示例）
来源：http://cb.gzmigu.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://pq.hahajie.cn

PHP:  // 递归实现，或用 usort
来源：http://re.newstarts.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://se.9csxet.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sv.lnxyls.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://cv.yuntaijiaju.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://qg.hahajie.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://nb.newstarts.cn

C#:   // 手写递归，或 Array.Sort
来源：http://fz.shxzskj.cn

[N04] 斐波那契数列
来源：http://vf.hnjuh.cn


<!-- 参考信息 -->