代发 wailian999

Java: Duration.between(start, end).toSeconds()
来源：http://kl.huixinmuqiang.cn

Go:   end.Sub(start).Hours()
来源：http://ws.jianghongdianzi.cn

Ruby: end - start                 # 返回秒数
来源：http://th.szsharing.cn

C#:   (end - start).TotalSeconds
来源：http://lm.wgjwhj.cn

[J07] 比较两个日期
来源：http://rx.jianghongdianzi.cn

Py:   d1 < d2;  d1 == d2
来源：http://pq.bookmarksfly.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://va.colortex.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ut.nicolike.cn

TS:   d1.getTime() < d2.getTime()
来源：http://im.nszjky.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://cw.panjiajie.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://fk.shxzukj.cn

Ruby: d1 < d2;  d1 == d2
来源：http://il.huixiangedu.cn

C#:   d1 < d2;  d1 == d2
来源：http://va.huanxung.cn

[J08] 提取年月日与星期
来源：http://qt.szsharing.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://yi.chemitech.net.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ne.hahajie.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://vx.haigaiapp.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://tm.wgjwhj.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://fk.shxzskj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mx.jianghongdianzi.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ty.gzmigu.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ur.bjjhwx.cn

[J09] 时区处理
来源：http://uq.bookmarksfly.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ay.newstarts.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ds.huixinmuqiang.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cj.yuexingan06.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://iv.bookmarksfly.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://jj.muxihuayi.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://yw.9csxet.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://rw.nszjky.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://gg.521024.cn

[J10] 取今天 / 本月第一天
来源：http://wk.nszjky.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://vd.nicolike.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://od.newstarts.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://lv.9csxet.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://xx.nszjky.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://vx.lnxyls.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://kp.szsharing.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://pf.9csxet.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ds.521024.cn

================================================================================
来源：http://qf.shxzukj.cn

K. JSON 与序列化
来源：http://md.colortex.cn

================================================================================
来源：http://gd.wgjwhj.cn

[K01] 对象转 JSON 字符串
来源：http://pp.huanxung.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ym.asd995.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ww.yuexingan06.cn

JS:   JSON.stringify(obj)
来源：http://nc.bookmarksfly.cn

TS:   JSON.stringify(obj)
来源：http://yb.lnxyls.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://is.newstarts.cn

Go:   json.Marshal(obj)
来源：http://et.jctech888.com.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ei.nicolike.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://mo.shxzukj.cn

[K02] JSON 字符串转对象
来源：http://xg.yuexingan06.cn

Py:   json.loads(s)
来源：http://au.panjiajie.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://az.bjjhwx.cn

JS:   JSON.parse(s)
来源：http://xz.szxytkj.cn

TS:   JSON.parse(s)
来源：http://of.yuexingan06.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vt.huixinmuqiang.cn

Go:   json.Unmarshal(data, &v)
来源：http://ci.asd995.cn

Ruby: JSON.parse(s)
来源：http://mp.wgjwhj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://gw.huanxung.cn

[K03] JSON 美化输出（带缩进）
来源：http://qb.jctech888.com.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ra.huixinmuqiang.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://oh.newstarts.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ss.nszjky.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://re.newstarts.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://vy.9csxet.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://sa.haigaiapp.cn

Ruby: JSON.pretty_generate(obj)
来源：http://rs.huixinmuqiang.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://fv.shxzukj.cn

[K04] 读取 JSON 文件
来源：http://gm.521024.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://rn.hahajie.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ib.9csxet.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kn.nszjky.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vz.yuntaijiaju.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://fm.521024.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://tl.bjjhwx.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://uu.szsharing.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://yp.panjiajie.cn

[K05] 深拷贝对象
来源：http://oe.lnxyls.cn

Py:   copy.deepcopy(obj)
来源：http://md.shxzskj.cn

PHP:  unserialize(serialize($obj));
来源：http://ao.lnxyls.cn

JS:   structuredClone(obj)
来源：http://cb.huixiangedu.cn

TS:   structuredClone(obj)
来源：http://vw.szxytkj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://bj.szxytkj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hq.hnjuh.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://in.szsharing.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://xq.colortex.cn

[K06] 解析 URL 查询串
来源：http://nh.newstarts.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rd.hahajie.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://oe.nicolike.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ux.521024.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wv.haigaiapp.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://km.521024.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ve.lnxyls.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mm.panjiajie.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://iz.nicolike.cn

[K07] 进制转换
来源：http://nf.9csxet.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://sf.huanxung.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://dp.muxihuayi.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://kx.huixinmuqiang.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://cz.muxihuayi.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://pi.chemitech.net.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ok.lnxyls.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://fo.shxzskj.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://gr.nszjky.cn

[K08] 二进制序列化（非 JSON）
来源：http://cg.haigaiapp.cn

Py:   pickle.dumps(obj)
来源：http://db.nszjky.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://fe.colortex.cn

JS:   v8.serialize(obj)        // Node
来源：http://je.szsharing.cn

TS:   v8.serialize(obj)        // Node
来源：http://gx.yuntaijiaju.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://vq.asd995.cn

Go:   encoding/gob
来源：http://rz.huanxung.cn

Ruby: Marshal.dump(obj)
来源：http://dn.yuntaijiaju.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://eg.wgjwhj.cn

================================================================================
来源：http://dn.shtwfgs.cn

L. 网络请求
来源：http://ft.shxzskj.cn

================================================================================
来源：http://td.chemitech.net.cn

[L01] 发送 GET 请求
来源：http://js.panjiajie.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://kc.hnjuh.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://rt.yuexingan06.cn

JS:   await fetch(url)
来源：http://kj.newstarts.cn

TS:   await fetch(url)
来源：http://rz.gzmigu.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://lj.gzmigu.cn

Go:   resp, err := http.Get(url)
来源：http://pt.szsharing.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://zu.bjjhwx.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://vo.newstarts.cn

[L02] 发送 POST JSON
来源：http://ro.newstarts.cn

Py:   requests.post(url, json={"a": 1})
来源：http://mv.wgjwhj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ms.szxytkj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://no.nszjky.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nf.shxzukj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://il.shtwfgs.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://vh.asd995.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://vg.hnjuh.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ly.szxytkj.cn

[L03] 设置自定义请求头
来源：http://mz.521024.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hj.shtwfgs.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://nh.panjiajie.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://we.panjiajie.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://aq.huixiangedu.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://sn.shxzskj.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://qa.shxzukj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ki.nicolike.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mg.yuntaijiaju.cn

[L04] 设置超时
来源：http://vh.gzmigu.cn

Py:   requests.get(url, timeout=5)
来源：http://yt.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xh.bookmarksfly.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yd.huixinmuqiang.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ql.haigaiapp.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://tp.nicolike.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://qg.szxytkj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://in.lnxyls.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://vp.huanxung.cn

[L05] 上传文件（multipart）
来源：http://oc.huanxung.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ry.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://tx.521024.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://cp.nszjky.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://kf.szsharing.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://tx.muxihuayi.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://in.9csxet.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://cc.chemitech.net.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://tn.szxytkj.cn

[L06] 解析响应为 JSON
来源：http://jt.huixiangedu.cn

Py:   resp.json()
来源：http://qe.huixiangedu.cn

PHP:  json_decode($body, true);
来源：http://zy.huixiangedu.cn

JS:   await resp.json()
来源：http://nc.lnxyls.cn

TS:   await resp.json()
来源：http://wd.bjjhwx.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://jf.shtwfgs.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://gc.yuexingan06.cn

Ruby: JSON.parse(resp.body)
来源：http://fm.bookmarksfly.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ew.asd995.cn

[L07] 处理 HTTP 状态码
来源：http://fz.shxzskj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wp.huixiangedu.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://di.gzmigu.cn

JS:   resp.ok;  resp.status
来源：http://cp.nszjky.cn

TS:   resp.ok;  resp.status
来源：http://be.wgjwhj.cn

Java: resp.statusCode()
来源：http://ap.szsharing.cn

Go:   resp.StatusCode
来源：http://zw.jianghongdianzi.cn

Ruby: resp.code.to_i
来源：http://fo.asd995.cn

C#:   (int)resp.StatusCode
来源：http://ci.nszjky.cn

[L08] 并发请求多个地址
来源：http://lx.asd995.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://at.colortex.cn

PHP:  curl_multi_init() 系列
来源：http://qb.shxzukj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mc.asd995.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mg.panjiajie.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://me.wgjwhj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://xn.jctech888.com.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://fh.haigaiapp.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://nu.huixinmuqiang.cn

================================================================================
来源：http://rg.chemitech.net.cn

M. 命令行 / 进程 / 环境
来源：http://ok.newstarts.cn

================================================================================
来源：http://kq.huixiangedu.cn

[M01] 读取命令行参数
来源：http://jl.newstarts.cn

Py:   sys.argv[1:]
来源：http://jp.yuntaijiaju.cn

PHP:  $argv;  $argc;
来源：http://lx.9csxet.cn

JS:   process.argv.slice(2)
来源：http://qg.bookmarksfly.cn

TS:   process.argv.slice(2)
来源：http://fd.521024.cn

Java: args 数组（main 方法参数）
来源：http://bx.wgjwhj.cn

Go:   os.Args[1:]
来源：http://hf.chemitech.net.cn

Ruby: ARGV
来源：http://en.9csxet.cn

C#:   args 数组（Main 方法参数）
来源：http://jw.haigaiapp.cn

[M02] 读取环境变量
来源：http://lr.huixinmuqiang.cn

Py:   os.environ.get("HOME")
来源：http://bl.9csxet.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ku.newstarts.cn

JS:   process.env.HOME
来源：http://fq.yuntaijiaju.cn

TS:   process.env.HOME
来源：http://oc.huanxung.cn

Java: System.getenv("HOME")
来源：http://dg.shtwfgs.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://th.nszjky.cn

Ruby: ENV["HOME"]
来源：http://zv.shtwfgs.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://sp.chemitech.net.cn

[M03] 执行外部命令
来源：http://jr.yuexingan06.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://pb.wgjwhj.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ir.chemitech.net.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://al.szxytkj.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://wr.newstarts.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://li.hnjuh.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ez.gzmigu.cn

Ruby: system("ls -l");  `ls -l`
来源：http://wg.colortex.cn

C#:   Process.Start("ls", "-l");
来源：http://xz.chemitech.net.cn

[M04] 获取当前工作目录
来源：http://gj.shxzukj.cn

Py:   os.getcwd()
来源：http://ba.haigaiapp.cn

PHP:  getcwd();
来源：http://py.hnjuh.cn

JS:   process.cwd()
来源：http://kb.panjiajie.cn

TS:   process.cwd()
来源：http://rj.szxytkj.cn

Java: Path.of("").toAbsolutePath()
来源：http://kx.newstarts.cn

Go:   os.Getwd()
来源：http://ps.chemitech.net.cn

Ruby: Dir.pwd
来源：http://xv.yuntaijiaju.cn

C#:   Directory.GetCurrentDirectory()
来源：http://jn.shtwfgs.cn

[M05] 设置退出码
来源：http://mk.shtwfgs.cn

Py:   sys.exit(1)
来源：http://ss.huixinmuqiang.cn

PHP:  exit(1);
来源：http://dm.yuexingan06.cn

JS:   process.exit(1)
来源：http://lb.9csxet.cn

TS:   process.exit(1)
来源：http://nc.lnxyls.cn

Java: System.exit(1)
来源：http://cu.hahajie.cn

Go:   os.Exit(1)
来源：http://gu.jianghongdianzi.cn

Ruby: exit 1
来源：http://ae.bjjhwx.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://jk.shxzskj.cn

[M06] 向标准错误输出
来源：http://lk.9csxet.cn

Py:   print("err", file=sys.stderr)
来源：http://ke.szxytkj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://pa.yuexingan06.cn

JS:   console.error("err")
来源：http://je.szsharing.cn

TS:   console.error("err")
来源：http://jn.newstarts.cn

Java: System.err.println("err")
来源：http://hr.asd995.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://tt.yuexingan06.cn

Ruby: warn "err"
来源：http://ju.chemitech.net.cn

C#:   Console.Error.WriteLine("err")
来源：http://mn.szsharing.cn

[M07] 判断是否为主入口
来源：http://aa.jctech888.com.cn

Py:   if __name__ == "__main__":
来源：http://su.newstarts.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ie.shtwfgs.cn

JS:   require.main === module
来源：http://dk.bjjhwx.cn

TS:   require.main === module
来源：http://wq.gzmigu.cn

Java: public static void main(String[] args)
来源：http://ae.newstarts.cn

Go:   func main()
来源：http://eb.nicolike.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://uu.gzmigu.cn

C#:   static void Main(string[] args)
来源：http://kw.shxzukj.cn

[M08] 获取系统与运行时信息
来源：http://jq.huixiangedu.cn

Py:   platform.system();  platform.python_version()
来源：http://of.hahajie.cn

PHP:  PHP_OS;  phpversion();
来源：http://ev.bookmarksfly.cn

JS:   process.platform;  process.version
来源：http://wz.newstarts.cn

TS:   process.platform;  process.version
来源：http://xu.nicolike.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://pi.521024.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://jf.yuntaijiaju.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://yh.huanxung.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://og.lnxyls.cn

================================================================================
来源：http://ye.shxzskj.cn

N. 数据结构与算法
来源：http://zm.hahajie.cn

================================================================================
来源：http://bq.szsharing.cn

[N01] 二分查找（有序数组）
来源：http://uo.gzmigu.cn

Py:   bisect.bisect_left(arr, x)
来源：http://we.huixinmuqiang.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://nj.jianghongdianzi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fs.szsharing.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://il.huanxung.cn

Java: Arrays.binarySearch(arr, x)
来源：http://vq.nszjky.cn

Go:   sort.SearchInts(arr, x)
来源：http://bd.szsharing.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://kj.muxihuayi.cn

C#:   Array.BinarySearch(arr, x)
来源：http://rb.9csxet.cn

[N02] 排序（工程实践用内置实现）
来源：http://xm.chemitech.net.cn

Py:   sorted(arr);  arr.sort()
来源：http://fb.wgjwhj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://yd.lnxyls.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://du.jctech888.com.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ib.colortex.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://bb.haigaiapp.cn

Go:   slices.Sort(arr)
来源：http://qy.muxihuayi.cn

Ruby: arr.sort
来源：http://op.newstarts.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://xt.huanxung.cn

[N03] 快速排序（分治示例）
来源：http://xq.nszjky.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hg.hahajie.cn

PHP:  // 递归实现，或用 usort
来源：http://so.nszjky.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ww.huixiangedu.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hx.panjiajie.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://bo.nszjky.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ur.nszjky.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://si.hnjuh.cn

C#:   // 手写递归，或 Array.Sort
来源：http://qv.newstarts.cn

[N04] 斐波那契数列
来源：http://fn.hahajie.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://fw.hahajie.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://nn.shxzskj.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://um.hahajie.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fz.huixinmuqiang.cn


<!-- 参考信息 -->