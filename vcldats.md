代发 wailian999

Go:   time.Now().AddDate(0, 0, 7)
来源：http://tl.panjiajie.cn

Ruby: Time.now + 7 * 86400
来源：http://ab.nicolike.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ve.colortex.cn

[J06] 计算两时间之差
来源：http://bk.gzmigu.cn

Py:   (end - start).total_seconds()
来源：http://hh.shtwfgs.cn

PHP:  $end->diff($start)->days;
来源：http://ol.9csxet.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://sb.szxytkj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://vx.yuexingan06.cn

Java: Duration.between(start, end).toSeconds()
来源：http://gp.jianghongdianzi.cn

Go:   end.Sub(start).Hours()
来源：http://ed.lnxyls.cn

Ruby: end - start                 # 返回秒数
来源：http://vw.bjjhwx.cn

C#:   (end - start).TotalSeconds
来源：http://zz.hahajie.cn

[J07] 比较两个日期
来源：http://qd.colortex.cn

Py:   d1 < d2;  d1 == d2
来源：http://oj.lnxyls.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ti.yuntaijiaju.cn

JS:   d1.getTime() < d2.getTime()
来源：http://we.szsharing.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ln.huixiangedu.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://nn.huixiangedu.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://do.nszjky.cn

Ruby: d1 < d2;  d1 == d2
来源：http://na.9csxet.cn

C#:   d1 < d2;  d1 == d2
来源：http://ld.chemitech.net.cn

[J08] 提取年月日与星期
来源：http://bk.chemitech.net.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://up.muxihuayi.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xl.asd995.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://zg.huixinmuqiang.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ji.jianghongdianzi.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://rh.shxzukj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://nx.jianghongdianzi.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wh.nszjky.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vf.huixiangedu.cn

[J09] 时区处理
来源：http://zi.9csxet.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wf.9csxet.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://gb.newstarts.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ne.chemitech.net.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jm.bookmarksfly.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://zv.asd995.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zu.shtwfgs.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://dg.huixiangedu.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://pd.nszjky.cn

[J10] 取今天 / 本月第一天
来源：http://pv.shxzskj.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://cu.hahajie.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://kb.huanxung.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://if.chemitech.net.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://xo.wgjwhj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://gh.shtwfgs.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xq.asd995.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vi.hnjuh.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://dy.hahajie.cn

================================================================================
来源：http://qh.jianghongdianzi.cn

K. JSON 与序列化
来源：http://pc.asd995.cn

================================================================================
来源：http://dn.szsharing.cn

[K01] 对象转 JSON 字符串
来源：http://oa.huanxung.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://lk.shxzukj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://fv.hahajie.cn

JS:   JSON.stringify(obj)
来源：http://jl.jctech888.com.cn

TS:   JSON.stringify(obj)
来源：http://qy.panjiajie.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://yh.szxytkj.cn

Go:   json.Marshal(obj)
来源：http://ux.bookmarksfly.cn

Ruby: obj.to_json                                     // require "json"
来源：http://qd.521024.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ex.gzmigu.cn

[K02] JSON 字符串转对象
来源：http://si.muxihuayi.cn

Py:   json.loads(s)
来源：http://uy.shxzukj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://xt.huanxung.cn

JS:   JSON.parse(s)
来源：http://vs.huixinmuqiang.cn

TS:   JSON.parse(s)
来源：http://ko.huanxung.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://lh.bookmarksfly.cn

Go:   json.Unmarshal(data, &v)
来源：http://sw.huixiangedu.cn

Ruby: JSON.parse(s)
来源：http://zk.521024.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://oa.huanxung.cn

[K03] JSON 美化输出（带缩进）
来源：http://pk.huixinmuqiang.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://rc.gzmigu.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://jq.shxzskj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://yc.shtwfgs.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://iy.nicolike.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ec.shtwfgs.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xf.jctech888.com.cn

Ruby: JSON.pretty_generate(obj)
来源：http://yf.yuntaijiaju.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://fq.hnjuh.cn

[K04] 读取 JSON 文件
来源：http://ko.shxzskj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://kh.shxzskj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://rr.huixinmuqiang.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hs.jianghongdianzi.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tb.panjiajie.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://gm.newstarts.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ye.panjiajie.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://lj.lnxyls.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ow.nicolike.cn

[K05] 深拷贝对象
来源：http://vo.shxzukj.cn

Py:   copy.deepcopy(obj)
来源：http://rn.szsharing.cn

PHP:  unserialize(serialize($obj));
来源：http://lh.chemitech.net.cn

JS:   structuredClone(obj)
来源：http://cw.chemitech.net.cn

TS:   structuredClone(obj)
来源：http://re.panjiajie.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://qd.521024.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://by.nszjky.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://pd.shxzskj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://mr.wgjwhj.cn

[K06] 解析 URL 查询串
来源：http://ie.9csxet.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://lq.9csxet.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://et.jctech888.com.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qb.hnjuh.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wd.newstarts.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://xg.shxzskj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://dz.wgjwhj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://uk.panjiajie.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://lg.nszjky.cn

[K07] 进制转换
来源：http://mz.nicolike.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://zg.shxzskj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ko.huixiangedu.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://rc.bookmarksfly.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://fq.szsharing.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ue.jctech888.com.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://yw.huanxung.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://cc.jctech888.com.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ab.bjjhwx.cn

[K08] 二进制序列化（非 JSON）
来源：http://sr.wgjwhj.cn

Py:   pickle.dumps(obj)
来源：http://ex.szsharing.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ut.hahajie.cn

JS:   v8.serialize(obj)        // Node
来源：http://du.huixiangedu.cn

TS:   v8.serialize(obj)        // Node
来源：http://cm.shxzskj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://pm.hahajie.cn

Go:   encoding/gob
来源：http://sq.hahajie.cn

Ruby: Marshal.dump(obj)
来源：http://df.bjjhwx.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://pw.shxzukj.cn

================================================================================
来源：http://ok.521024.cn

L. 网络请求
来源：http://bd.haigaiapp.cn

================================================================================
来源：http://lf.yuexingan06.cn

[L01] 发送 GET 请求
来源：http://hz.nszjky.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://zv.nszjky.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mm.hahajie.cn

JS:   await fetch(url)
来源：http://ya.9csxet.cn

TS:   await fetch(url)
来源：http://kp.yuntaijiaju.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wj.wgjwhj.cn

Go:   resp, err := http.Get(url)
来源：http://wu.bjjhwx.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://jf.wgjwhj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://vj.nszjky.cn

[L02] 发送 POST JSON
来源：http://lb.panjiajie.cn

Py:   requests.post(url, json={"a": 1})
来源：http://hp.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://vx.yuexingan06.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vt.jctech888.com.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tx.521024.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://zj.bjjhwx.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://eh.jctech888.com.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://af.muxihuayi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ta.gzmigu.cn

[L03] 设置自定义请求头
来源：http://iz.521024.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ev.szsharing.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://jc.lnxyls.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ac.haigaiapp.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gc.521024.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://cw.wgjwhj.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://eb.gzmigu.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://xm.nicolike.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://vx.hnjuh.cn

[L04] 设置超时
来源：http://ov.huanxung.cn

Py:   requests.get(url, timeout=5)
来源：http://yw.521024.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ue.huixiangedu.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://to.nicolike.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vk.bookmarksfly.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qi.gzmigu.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://np.muxihuayi.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://vn.yuntaijiaju.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://jq.shtwfgs.cn

[L05] 上传文件（multipart）
来源：http://gd.shxzskj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://fp.asd995.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ry.wgjwhj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://vr.bjjhwx.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://dx.szxytkj.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ib.hahajie.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://cn.nicolike.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://tu.huixiangedu.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://db.asd995.cn

[L06] 解析响应为 JSON
来源：http://yc.szsharing.cn

Py:   resp.json()
来源：http://hl.panjiajie.cn

PHP:  json_decode($body, true);
来源：http://xp.yuexingan06.cn

JS:   await resp.json()
来源：http://vr.haigaiapp.cn

TS:   await resp.json()
来源：http://bx.szxytkj.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://nd.colortex.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://iw.shtwfgs.cn

Ruby: JSON.parse(resp.body)
来源：http://xk.huixinmuqiang.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://pt.nicolike.cn

[L07] 处理 HTTP 状态码
来源：http://lp.bookmarksfly.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://fs.newstarts.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wj.lnxyls.cn

JS:   resp.ok;  resp.status
来源：http://vk.newstarts.cn

TS:   resp.ok;  resp.status
来源：http://dk.bjjhwx.cn

Java: resp.statusCode()
来源：http://wg.jctech888.com.cn

Go:   resp.StatusCode
来源：http://xu.jctech888.com.cn

Ruby: resp.code.to_i
来源：http://xz.bjjhwx.cn

C#:   (int)resp.StatusCode
来源：http://pr.hnjuh.cn

[L08] 并发请求多个地址
来源：http://dx.szxytkj.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://rf.yuexingan06.cn

PHP:  curl_multi_init() 系列
来源：http://zx.gzmigu.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ji.lnxyls.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ru.huixiangedu.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://zu.yuexingan06.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qu.gzmigu.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zx.huixiangedu.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://jp.haigaiapp.cn

================================================================================
来源：http://zn.bjjhwx.cn

M. 命令行 / 进程 / 环境
来源：http://bh.jctech888.com.cn

================================================================================
来源：http://pv.hahajie.cn

[M01] 读取命令行参数
来源：http://ql.szsharing.cn

Py:   sys.argv[1:]
来源：http://po.newstarts.cn

PHP:  $argv;  $argc;
来源：http://cj.huixinmuqiang.cn

JS:   process.argv.slice(2)
来源：http://ko.bookmarksfly.cn

TS:   process.argv.slice(2)
来源：http://ld.huanxung.cn

Java: args 数组（main 方法参数）
来源：http://te.chemitech.net.cn

Go:   os.Args[1:]
来源：http://tt.9csxet.cn

Ruby: ARGV
来源：http://jr.asd995.cn

C#:   args 数组（Main 方法参数）
来源：http://pm.yuntaijiaju.cn

[M02] 读取环境变量
来源：http://uj.jianghongdianzi.cn

Py:   os.environ.get("HOME")
来源：http://rp.jianghongdianzi.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://qb.asd995.cn

JS:   process.env.HOME
来源：http://zf.bjjhwx.cn

TS:   process.env.HOME
来源：http://vg.shtwfgs.cn

Java: System.getenv("HOME")
来源：http://wb.haigaiapp.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://zk.wgjwhj.cn

Ruby: ENV["HOME"]
来源：http://xf.hahajie.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://uv.huixinmuqiang.cn

[M03] 执行外部命令
来源：http://tj.chemitech.net.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ct.hahajie.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ro.szxytkj.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://xn.gzmigu.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://hk.szsharing.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://xq.szsharing.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://wp.bookmarksfly.cn

Ruby: system("ls -l");  `ls -l`
来源：http://io.gzmigu.cn

C#:   Process.Start("ls", "-l");
来源：http://rw.asd995.cn

[M04] 获取当前工作目录
来源：http://xb.jianghongdianzi.cn

Py:   os.getcwd()
来源：http://du.9csxet.cn

PHP:  getcwd();
来源：http://vi.nszjky.cn

JS:   process.cwd()
来源：http://pa.colortex.cn

TS:   process.cwd()
来源：http://bg.shtwfgs.cn

Java: Path.of("").toAbsolutePath()
来源：http://in.huixinmuqiang.cn

Go:   os.Getwd()
来源：http://zu.panjiajie.cn

Ruby: Dir.pwd
来源：http://tx.jianghongdianzi.cn

C#:   Directory.GetCurrentDirectory()
来源：http://tm.hnjuh.cn

[M05] 设置退出码
来源：http://zh.huixinmuqiang.cn

Py:   sys.exit(1)
来源：http://ks.9csxet.cn

PHP:  exit(1);
来源：http://qo.newstarts.cn

JS:   process.exit(1)
来源：http://tu.muxihuayi.cn

TS:   process.exit(1)
来源：http://uf.shtwfgs.cn

Java: System.exit(1)
来源：http://wj.bjjhwx.cn

Go:   os.Exit(1)
来源：http://mo.521024.cn

Ruby: exit 1
来源：http://vl.bookmarksfly.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://yl.yuntaijiaju.cn

[M06] 向标准错误输出
来源：http://mh.shtwfgs.cn

Py:   print("err", file=sys.stderr)
来源：http://yw.huanxung.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://hd.huixinmuqiang.cn

JS:   console.error("err")
来源：http://wf.newstarts.cn

TS:   console.error("err")
来源：http://xe.panjiajie.cn

Java: System.err.println("err")
来源：http://zx.9csxet.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://lb.hnjuh.cn

Ruby: warn "err"
来源：http://gh.szsharing.cn

C#:   Console.Error.WriteLine("err")
来源：http://dk.shtwfgs.cn

[M07] 判断是否为主入口
来源：http://mx.jctech888.com.cn

Py:   if __name__ == "__main__":
来源：http://lh.chemitech.net.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://pu.shxzukj.cn

JS:   require.main === module
来源：http://zu.haigaiapp.cn

TS:   require.main === module
来源：http://la.shxzskj.cn

Java: public static void main(String[] args)
来源：http://er.nszjky.cn

Go:   func main()
来源：http://zc.szsharing.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://yj.yuntaijiaju.cn

C#:   static void Main(string[] args)
来源：http://sg.huanxung.cn

[M08] 获取系统与运行时信息
来源：http://ip.nicolike.cn

Py:   platform.system();  platform.python_version()
来源：http://eg.shxzukj.cn

PHP:  PHP_OS;  phpversion();
来源：http://qs.gzmigu.cn

JS:   process.platform;  process.version
来源：http://nz.szxytkj.cn

TS:   process.platform;  process.version
来源：http://bz.hnjuh.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://fo.huixiangedu.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://mp.huanxung.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wa.bjjhwx.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://gm.wgjwhj.cn

================================================================================
来源：http://ox.colortex.cn

N. 数据结构与算法
来源：http://oy.gzmigu.cn

================================================================================
来源：http://xv.bjjhwx.cn

[N01] 二分查找（有序数组）
来源：http://nc.huixiangedu.cn

Py:   bisect.bisect_left(arr, x)
来源：http://yh.bjjhwx.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ls.bookmarksfly.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jc.wgjwhj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dx.yuntaijiaju.cn

Java: Arrays.binarySearch(arr, x)
来源：http://pc.szsharing.cn

Go:   sort.SearchInts(arr, x)
来源：http://tb.shxzukj.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://vk.wgjwhj.cn

C#:   Array.BinarySearch(arr, x)
来源：http://du.muxihuayi.cn

[N02] 排序（工程实践用内置实现）
来源：http://eh.haigaiapp.cn

Py:   sorted(arr);  arr.sort()
来源：http://vd.nicolike.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hi.huixinmuqiang.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://jj.jctech888.com.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://lb.shxzukj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://xd.wgjwhj.cn

Go:   slices.Sort(arr)
来源：http://je.shxzskj.cn

Ruby: arr.sort
来源：http://kd.nszjky.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://my.hahajie.cn

[N03] 快速排序（分治示例）
来源：http://xx.newstarts.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://vq.bookmarksfly.cn

PHP:  // 递归实现，或用 usort
来源：http://ik.yuexingan06.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://og.nszjky.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tl.bjjhwx.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://zl.wgjwhj.cn


<!-- 参考信息 -->