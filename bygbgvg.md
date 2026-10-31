代发 wailian999

Java: Duration.between(start, end).toSeconds()
来源：http://iy.huanxung.cn

Go:   end.Sub(start).Hours()
来源：http://jz.bookmarksfly.cn

Ruby: end - start                 # 返回秒数
来源：http://pg.wgjwhj.cn

C#:   (end - start).TotalSeconds
来源：http://ub.shxzskj.cn

[J07] 比较两个日期
来源：http://rq.jctech888.com.cn

Py:   d1 < d2;  d1 == d2
来源：http://lq.bjjhwx.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ne.521024.cn

JS:   d1.getTime() < d2.getTime()
来源：http://an.jctech888.com.cn

TS:   d1.getTime() < d2.getTime()
来源：http://tb.nicolike.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://je.szxytkj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://sp.jctech888.com.cn

Ruby: d1 < d2;  d1 == d2
来源：http://bt.jianghongdianzi.cn

C#:   d1 < d2;  d1 == d2
来源：http://bn.muxihuayi.cn

[J08] 提取年月日与星期
来源：http://bw.chemitech.net.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wk.bjjhwx.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xq.panjiajie.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://nq.nszjky.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://zn.muxihuayi.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ra.colortex.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://uh.huixinmuqiang.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zl.9csxet.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://js.jctech888.com.cn

[J09] 时区处理
来源：http://ib.shtwfgs.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ib.asd995.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wv.yuntaijiaju.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vp.521024.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cr.huixiangedu.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ab.hnjuh.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xj.nicolike.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://rj.gzmigu.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ov.shxzskj.cn

[J10] 取今天 / 本月第一天
来源：http://py.lnxyls.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://xb.wgjwhj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://cc.yuntaijiaju.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ep.szxytkj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://sz.haigaiapp.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ek.9csxet.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ku.bjjhwx.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://sk.9csxet.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://in.hnjuh.cn

================================================================================
来源：http://og.bookmarksfly.cn

K. JSON 与序列化
来源：http://ca.newstarts.cn

================================================================================
来源：http://yy.szxytkj.cn

[K01] 对象转 JSON 字符串
来源：http://ae.huixinmuqiang.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://xa.9csxet.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://kx.szsharing.cn

JS:   JSON.stringify(obj)
来源：http://ls.lnxyls.cn

TS:   JSON.stringify(obj)
来源：http://li.huixiangedu.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ck.szxytkj.cn

Go:   json.Marshal(obj)
来源：http://qm.shxzukj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://mm.bookmarksfly.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://yt.lnxyls.cn

[K02] JSON 字符串转对象
来源：http://bo.huanxung.cn

Py:   json.loads(s)
来源：http://hi.huanxung.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://vu.nszjky.cn

JS:   JSON.parse(s)
来源：http://xm.bjjhwx.cn

TS:   JSON.parse(s)
来源：http://pm.shxzskj.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://sx.nicolike.cn

Go:   json.Unmarshal(data, &v)
来源：http://qg.bjjhwx.cn

Ruby: JSON.parse(s)
来源：http://jn.jctech888.com.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://yo.huanxung.cn

[K03] JSON 美化输出（带缩进）
来源：http://hw.huixinmuqiang.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://as.panjiajie.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qw.huixiangedu.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://co.huixinmuqiang.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://en.hahajie.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://jm.asd995.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://zl.chemitech.net.cn

Ruby: JSON.pretty_generate(obj)
来源：http://pv.szxytkj.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://bw.bjjhwx.cn

[K04] 读取 JSON 文件
来源：http://dh.jianghongdianzi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ye.521024.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://pe.colortex.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vy.newstarts.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cp.nszjky.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://cm.szsharing.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://sr.hnjuh.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://wo.panjiajie.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://en.szsharing.cn

[K05] 深拷贝对象
来源：http://ai.bookmarksfly.cn

Py:   copy.deepcopy(obj)
来源：http://hs.shtwfgs.cn

PHP:  unserialize(serialize($obj));
来源：http://lz.lnxyls.cn

JS:   structuredClone(obj)
来源：http://am.shxzskj.cn

TS:   structuredClone(obj)
来源：http://al.szxytkj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://cp.huanxung.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://rf.huixinmuqiang.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wf.shtwfgs.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ik.bookmarksfly.cn

[K06] 解析 URL 查询串
来源：http://dj.yuntaijiaju.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://lx.nszjky.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://by.panjiajie.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nx.bjjhwx.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wf.shxzukj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://qw.bookmarksfly.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://eh.huanxung.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wz.jianghongdianzi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://tq.bookmarksfly.cn

[K07] 进制转换
来源：http://qh.chemitech.net.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ru.jianghongdianzi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wy.jianghongdianzi.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://qt.shxzukj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ej.yuexingan06.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://iu.shxzukj.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://fn.bookmarksfly.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ag.panjiajie.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hl.521024.cn

[K08] 二进制序列化（非 JSON）
来源：http://at.521024.cn

Py:   pickle.dumps(obj)
来源：http://ff.szxytkj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://gu.bjjhwx.cn

JS:   v8.serialize(obj)        // Node
来源：http://on.colortex.cn

TS:   v8.serialize(obj)        // Node
来源：http://po.bjjhwx.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://bo.wgjwhj.cn

Go:   encoding/gob
来源：http://il.bjjhwx.cn

Ruby: Marshal.dump(obj)
来源：http://ex.colortex.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://jc.chemitech.net.cn

================================================================================
来源：http://ee.panjiajie.cn

L. 网络请求
来源：http://nw.chemitech.net.cn

================================================================================
来源：http://ng.hnjuh.cn

[L01] 发送 GET 请求
来源：http://ud.hnjuh.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://iq.szsharing.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vt.huixinmuqiang.cn

JS:   await fetch(url)
来源：http://yk.panjiajie.cn

TS:   await fetch(url)
来源：http://ic.haigaiapp.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ae.jianghongdianzi.cn

Go:   resp, err := http.Get(url)
来源：http://ag.jianghongdianzi.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://cc.jctech888.com.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://lc.wgjwhj.cn

[L02] 发送 POST JSON
来源：http://lk.huanxung.cn

Py:   requests.post(url, json={"a": 1})
来源：http://re.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qc.shxzukj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pg.szsharing.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ki.nszjky.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wc.hahajie.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ky.jianghongdianzi.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://no.yuntaijiaju.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://sj.yuntaijiaju.cn

[L03] 设置自定义请求头
来源：http://bn.jianghongdianzi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://zr.haigaiapp.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://yt.bookmarksfly.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pa.chemitech.net.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kd.521024.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://oc.newstarts.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://eu.yuexingan06.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://zo.shxzskj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://cw.szsharing.cn

[L04] 设置超时
来源：http://qw.521024.cn

Py:   requests.get(url, timeout=5)
来源：http://kw.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://kj.yuexingan06.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zk.jctech888.com.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wv.szxytkj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wq.nicolike.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://om.shxzukj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://fn.huixiangedu.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://gm.nszjky.cn

[L05] 上传文件（multipart）
来源：http://cl.wgjwhj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://nu.nicolike.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://zd.9csxet.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://rc.huixinmuqiang.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://pn.jctech888.com.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://dl.yuexingan06.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://pb.newstarts.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://nd.nicolike.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://gp.shxzskj.cn

[L06] 解析响应为 JSON
来源：http://bw.lnxyls.cn

Py:   resp.json()
来源：http://tl.szxytkj.cn

PHP:  json_decode($body, true);
来源：http://lc.colortex.cn

JS:   await resp.json()
来源：http://ip.haigaiapp.cn

TS:   await resp.json()
来源：http://ma.newstarts.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ip.yuntaijiaju.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://qw.9csxet.cn

Ruby: JSON.parse(resp.body)
来源：http://ye.szxytkj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://zo.nicolike.cn

[L07] 处理 HTTP 状态码
来源：http://qr.huixiangedu.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ee.jctech888.com.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hd.huixiangedu.cn

JS:   resp.ok;  resp.status
来源：http://nt.hahajie.cn

TS:   resp.ok;  resp.status
来源：http://mh.muxihuayi.cn

Java: resp.statusCode()
来源：http://vo.haigaiapp.cn

Go:   resp.StatusCode
来源：http://zo.521024.cn

Ruby: resp.code.to_i
来源：http://oq.hnjuh.cn

C#:   (int)resp.StatusCode
来源：http://ts.chemitech.net.cn

[L08] 并发请求多个地址
来源：http://mh.hahajie.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://bv.huanxung.cn

PHP:  curl_multi_init() 系列
来源：http://hu.hahajie.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wf.huanxung.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://co.jianghongdianzi.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ou.yuntaijiaju.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://kl.jianghongdianzi.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://jg.asd995.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://de.asd995.cn

================================================================================
来源：http://ns.szsharing.cn

M. 命令行 / 进程 / 环境
来源：http://mb.nszjky.cn

================================================================================
来源：http://iw.asd995.cn

[M01] 读取命令行参数
来源：http://xt.jianghongdianzi.cn

Py:   sys.argv[1:]
来源：http://jn.chemitech.net.cn

PHP:  $argv;  $argc;
来源：http://bn.shxzskj.cn

JS:   process.argv.slice(2)
来源：http://mw.shxzskj.cn

TS:   process.argv.slice(2)
来源：http://vl.bookmarksfly.cn

Java: args 数组（main 方法参数）
来源：http://nd.nszjky.cn

Go:   os.Args[1:]
来源：http://eq.huixiangedu.cn

Ruby: ARGV
来源：http://oa.hnjuh.cn

C#:   args 数组（Main 方法参数）
来源：http://de.shxzukj.cn

[M02] 读取环境变量
来源：http://nv.yuntaijiaju.cn

Py:   os.environ.get("HOME")
来源：http://rb.gzmigu.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ct.szsharing.cn

JS:   process.env.HOME
来源：http://xy.shxzukj.cn

TS:   process.env.HOME
来源：http://gj.bjjhwx.cn

Java: System.getenv("HOME")
来源：http://zp.bjjhwx.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wg.huixiangedu.cn

Ruby: ENV["HOME"]
来源：http://mq.huanxung.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://nf.521024.cn

[M03] 执行外部命令
来源：http://nz.hnjuh.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://oi.huixiangedu.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://xz.shtwfgs.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://rk.jctech888.com.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://lk.muxihuayi.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://gj.huixinmuqiang.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://jv.hnjuh.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ho.gzmigu.cn

C#:   Process.Start("ls", "-l");
来源：http://lo.haigaiapp.cn

[M04] 获取当前工作目录
来源：http://bl.szxytkj.cn

Py:   os.getcwd()
来源：http://ei.bookmarksfly.cn

PHP:  getcwd();
来源：http://sh.lnxyls.cn

JS:   process.cwd()
来源：http://ym.szsharing.cn

TS:   process.cwd()
来源：http://od.521024.cn

Java: Path.of("").toAbsolutePath()
来源：http://hw.nicolike.cn

Go:   os.Getwd()
来源：http://vx.hahajie.cn

Ruby: Dir.pwd
来源：http://bl.nszjky.cn

C#:   Directory.GetCurrentDirectory()
来源：http://lj.huanxung.cn

[M05] 设置退出码
来源：http://ay.szsharing.cn

Py:   sys.exit(1)
来源：http://kr.szxytkj.cn

PHP:  exit(1);
来源：http://pt.521024.cn

JS:   process.exit(1)
来源：http://kw.panjiajie.cn

TS:   process.exit(1)
来源：http://pb.nicolike.cn

Java: System.exit(1)
来源：http://ro.bjjhwx.cn

Go:   os.Exit(1)
来源：http://gz.szsharing.cn

Ruby: exit 1
来源：http://rz.hnjuh.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://de.panjiajie.cn

[M06] 向标准错误输出
来源：http://ri.521024.cn

Py:   print("err", file=sys.stderr)
来源：http://az.9csxet.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://bt.szsharing.cn

JS:   console.error("err")
来源：http://em.lnxyls.cn

TS:   console.error("err")
来源：http://gm.jianghongdianzi.cn

Java: System.err.println("err")
来源：http://sa.huixinmuqiang.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://cs.muxihuayi.cn

Ruby: warn "err"
来源：http://kx.muxihuayi.cn

C#:   Console.Error.WriteLine("err")
来源：http://tc.colortex.cn

[M07] 判断是否为主入口
来源：http://jf.shtwfgs.cn

Py:   if __name__ == "__main__":
来源：http://ni.wgjwhj.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://aw.chemitech.net.cn

JS:   require.main === module
来源：http://wy.yuexingan06.cn

TS:   require.main === module
来源：http://cd.bjjhwx.cn

Java: public static void main(String[] args)
来源：http://kt.bookmarksfly.cn

Go:   func main()
来源：http://ut.newstarts.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://pw.hnjuh.cn

C#:   static void Main(string[] args)
来源：http://be.shxzukj.cn

[M08] 获取系统与运行时信息
来源：http://ve.lnxyls.cn

Py:   platform.system();  platform.python_version()
来源：http://qw.nszjky.cn

PHP:  PHP_OS;  phpversion();
来源：http://wi.nszjky.cn

JS:   process.platform;  process.version
来源：http://by.yuntaijiaju.cn

TS:   process.platform;  process.version
来源：http://fu.shxzskj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://fs.gzmigu.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://gm.shxzukj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://fd.yuexingan06.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://gy.9csxet.cn

================================================================================
来源：http://kj.bookmarksfly.cn

N. 数据结构与算法
来源：http://fh.hahajie.cn

================================================================================
来源：http://di.szsharing.cn

[N01] 二分查找（有序数组）
来源：http://pf.huixiangedu.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ch.newstarts.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ry.521024.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://po.newstarts.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dd.panjiajie.cn

Java: Arrays.binarySearch(arr, x)
来源：http://xu.chemitech.net.cn

Go:   sort.SearchInts(arr, x)
来源：http://lz.muxihuayi.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://nv.lnxyls.cn

C#:   Array.BinarySearch(arr, x)
来源：http://mv.nszjky.cn

[N02] 排序（工程实践用内置实现）
来源：http://nr.521024.cn

Py:   sorted(arr);  arr.sort()
来源：http://bz.newstarts.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ne.lnxyls.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://zs.9csxet.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://xk.yuntaijiaju.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://xf.wgjwhj.cn

Go:   slices.Sort(arr)
来源：http://oy.wgjwhj.cn

Ruby: arr.sort
来源：http://ku.shxzskj.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ic.nszjky.cn

[N03] 快速排序（分治示例）
来源：http://wd.nicolike.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://pm.wgjwhj.cn

PHP:  // 递归实现，或用 usort
来源：http://pp.nszjky.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://db.hahajie.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ta.haigaiapp.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hs.huixiangedu.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ef.shxzukj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hv.hahajie.cn

C#:   // 手写递归，或 Array.Sort
来源：http://uz.szsharing.cn

[N04] 斐波那契数列
来源：http://um.gzmigu.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://xm.hahajie.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wl.huixiangedu.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://oq.wgjwhj.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mw.szxytkj.cn


<!-- 参考信息 -->