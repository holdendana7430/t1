代发 wailian999

Java: Duration.between(start, end).toSeconds()
来源：http://ay.chemitech.net.cn

Go:   end.Sub(start).Hours()
来源：http://mi.jctech888.com.cn

Ruby: end - start                 # 返回秒数
来源：http://hx.huixiangedu.cn

C#:   (end - start).TotalSeconds
来源：http://ml.shtwfgs.cn

[J07] 比较两个日期
来源：http://il.colortex.cn

Py:   d1 < d2;  d1 == d2
来源：http://bt.shxzukj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://rm.huixiangedu.cn

JS:   d1.getTime() < d2.getTime()
来源：http://yi.hahajie.cn

TS:   d1.getTime() < d2.getTime()
来源：http://uz.wgjwhj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://em.bookmarksfly.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://jt.muxihuayi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://bo.bookmarksfly.cn

C#:   d1 < d2;  d1 == d2
来源：http://xp.huanxung.cn

[J08] 提取年月日与星期
来源：http://ne.newstarts.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mk.shtwfgs.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://an.huanxung.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ov.nicolike.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://kj.hnjuh.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://et.9csxet.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://pg.yuntaijiaju.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ow.szxytkj.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://iq.lnxyls.cn

[J09] 时区处理
来源：http://kh.colortex.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ka.yuntaijiaju.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://bu.chemitech.net.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://oo.huixiangedu.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fs.colortex.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://le.shtwfgs.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://em.9csxet.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://or.jianghongdianzi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://bx.huixiangedu.cn

[J10] 取今天 / 本月第一天
来源：http://nu.521024.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://gn.huanxung.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://vk.wgjwhj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hu.hahajie.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://df.nszjky.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://fs.521024.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://sa.hnjuh.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ez.panjiajie.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ba.9csxet.cn

================================================================================
来源：http://ns.hnjuh.cn

K. JSON 与序列化
来源：http://tr.shxzukj.cn

================================================================================
来源：http://wt.gzmigu.cn

[K01] 对象转 JSON 字符串
来源：http://ge.hahajie.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ti.shtwfgs.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ei.szxytkj.cn

JS:   JSON.stringify(obj)
来源：http://ji.bookmarksfly.cn

TS:   JSON.stringify(obj)
来源：http://uu.jianghongdianzi.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://pt.shxzukj.cn

Go:   json.Marshal(obj)
来源：http://wk.wgjwhj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ca.wgjwhj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://se.shxzskj.cn

[K02] JSON 字符串转对象
来源：http://jk.shxzskj.cn

Py:   json.loads(s)
来源：http://qa.shxzskj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://kz.jctech888.com.cn

JS:   JSON.parse(s)
来源：http://aq.gzmigu.cn

TS:   JSON.parse(s)
来源：http://yq.yuntaijiaju.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://nb.chemitech.net.cn

Go:   json.Unmarshal(data, &v)
来源：http://tw.shxzskj.cn

Ruby: JSON.parse(s)
来源：http://xm.jianghongdianzi.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://vm.lnxyls.cn

[K03] JSON 美化输出（带缩进）
来源：http://vh.jianghongdianzi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://cw.hahajie.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://fd.szxytkj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://sj.huixiangedu.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://te.asd995.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ki.shxzukj.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://qu.jianghongdianzi.cn

Ruby: JSON.pretty_generate(obj)
来源：http://sn.huixinmuqiang.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://zt.huanxung.cn

[K04] 读取 JSON 文件
来源：http://zt.nszjky.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://sc.huanxung.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://iz.hnjuh.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ct.bjjhwx.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wu.asd995.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://dh.chemitech.net.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://oa.shtwfgs.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ta.nszjky.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ky.szsharing.cn

[K05] 深拷贝对象
来源：http://wv.gzmigu.cn

Py:   copy.deepcopy(obj)
来源：http://wf.shxzskj.cn

PHP:  unserialize(serialize($obj));
来源：http://fw.huixinmuqiang.cn

JS:   structuredClone(obj)
来源：http://hk.haigaiapp.cn

TS:   structuredClone(obj)
来源：http://dv.szxytkj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://uv.521024.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://us.gzmigu.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://kj.bookmarksfly.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://jj.nicolike.cn

[K06] 解析 URL 查询串
来源：http://gr.hnjuh.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://we.521024.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://tw.hnjuh.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rz.jctech888.com.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://iq.shxzukj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://rs.panjiajie.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://za.panjiajie.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hg.shtwfgs.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://on.newstarts.cn

[K07] 进制转换
来源：http://qu.yuexingan06.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://lh.jianghongdianzi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://fe.panjiajie.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xk.huanxung.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://bj.huanxung.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://fn.bookmarksfly.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://to.bookmarksfly.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ld.szxytkj.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ns.jianghongdianzi.cn

[K08] 二进制序列化（非 JSON）
来源：http://nr.shxzukj.cn

Py:   pickle.dumps(obj)
来源：http://bl.chemitech.net.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://tz.lnxyls.cn

JS:   v8.serialize(obj)        // Node
来源：http://ti.nicolike.cn

TS:   v8.serialize(obj)        // Node
来源：http://ev.chemitech.net.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://bs.muxihuayi.cn

Go:   encoding/gob
来源：http://uq.chemitech.net.cn

Ruby: Marshal.dump(obj)
来源：http://fo.muxihuayi.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://pn.shxzskj.cn

================================================================================
来源：http://sy.shxzukj.cn

L. 网络请求
来源：http://rm.gzmigu.cn

================================================================================
来源：http://il.asd995.cn

[L01] 发送 GET 请求
来源：http://ib.szxytkj.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://nh.shxzukj.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://br.nicolike.cn

JS:   await fetch(url)
来源：http://ie.muxihuayi.cn

TS:   await fetch(url)
来源：http://bm.panjiajie.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ji.chemitech.net.cn

Go:   resp, err := http.Get(url)
来源：http://ss.9csxet.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://si.szsharing.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ef.asd995.cn

[L02] 发送 POST JSON
来源：http://cw.jctech888.com.cn

Py:   requests.post(url, json={"a": 1})
来源：http://gn.hnjuh.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ly.shxzskj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wy.huixinmuqiang.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lk.wgjwhj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://tr.haigaiapp.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wt.asd995.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://sr.nicolike.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hj.shtwfgs.cn

[L03] 设置自定义请求头
来源：http://rm.shxzskj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://dj.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://gs.huixiangedu.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ve.szsharing.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jg.haigaiapp.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ey.nszjky.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://rk.szxytkj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://kw.nicolike.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ji.muxihuayi.cn

[L04] 设置超时
来源：http://rz.nszjky.cn

Py:   requests.get(url, timeout=5)
来源：http://bq.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://tx.asd995.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zs.shxzskj.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cd.nszjky.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://se.newstarts.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ra.jianghongdianzi.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://tp.panjiajie.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://vz.newstarts.cn

[L05] 上传文件（multipart）
来源：http://du.lnxyls.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://bu.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://li.huixinmuqiang.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://bn.hnjuh.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://fi.panjiajie.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://sc.panjiajie.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://dv.yuntaijiaju.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ry.colortex.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://dq.huixinmuqiang.cn

[L06] 解析响应为 JSON
来源：http://qr.gzmigu.cn

Py:   resp.json()
来源：http://wr.nszjky.cn

PHP:  json_decode($body, true);
来源：http://uh.lnxyls.cn

JS:   await resp.json()
来源：http://yt.muxihuayi.cn

TS:   await resp.json()
来源：http://xg.szsharing.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ei.yuntaijiaju.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://fn.shxzukj.cn

Ruby: JSON.parse(resp.body)
来源：http://ac.jctech888.com.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://dl.hnjuh.cn

[L07] 处理 HTTP 状态码
来源：http://do.9csxet.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://kt.yuntaijiaju.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://jk.panjiajie.cn

JS:   resp.ok;  resp.status
来源：http://xw.nicolike.cn

TS:   resp.ok;  resp.status
来源：http://zd.wgjwhj.cn

Java: resp.statusCode()
来源：http://nr.szxytkj.cn

Go:   resp.StatusCode
来源：http://di.shxzskj.cn

Ruby: resp.code.to_i
来源：http://wg.yuexingan06.cn

C#:   (int)resp.StatusCode
来源：http://wm.shtwfgs.cn

[L08] 并发请求多个地址
来源：http://tj.chemitech.net.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://kp.nszjky.cn

PHP:  curl_multi_init() 系列
来源：http://df.panjiajie.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ff.nicolike.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ce.jianghongdianzi.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ld.yuexingan06.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mf.szsharing.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://cq.newstarts.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://zl.asd995.cn

================================================================================
来源：http://zq.szxytkj.cn

M. 命令行 / 进程 / 环境
来源：http://tm.nszjky.cn

================================================================================
来源：http://bv.muxihuayi.cn

[M01] 读取命令行参数
来源：http://ei.newstarts.cn

Py:   sys.argv[1:]
来源：http://ie.newstarts.cn

PHP:  $argv;  $argc;
来源：http://of.shtwfgs.cn

JS:   process.argv.slice(2)
来源：http://ml.muxihuayi.cn

TS:   process.argv.slice(2)
来源：http://ft.huixinmuqiang.cn

Java: args 数组（main 方法参数）
来源：http://vl.jctech888.com.cn

Go:   os.Args[1:]
来源：http://av.huixiangedu.cn

Ruby: ARGV
来源：http://yf.nszjky.cn

C#:   args 数组（Main 方法参数）
来源：http://zx.9csxet.cn

[M02] 读取环境变量
来源：http://za.nszjky.cn

Py:   os.environ.get("HOME")
来源：http://kf.lnxyls.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://qk.shxzukj.cn

JS:   process.env.HOME
来源：http://im.nszjky.cn

TS:   process.env.HOME
来源：http://qg.hahajie.cn

Java: System.getenv("HOME")
来源：http://hq.hahajie.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mp.bookmarksfly.cn

Ruby: ENV["HOME"]
来源：http://hf.colortex.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wd.szsharing.cn

[M03] 执行外部命令
来源：http://ke.asd995.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ew.huanxung.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://cs.lnxyls.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://xd.shxzukj.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://yr.shtwfgs.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://cd.muxihuayi.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://sf.shxzukj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://qd.9csxet.cn

C#:   Process.Start("ls", "-l");
来源：http://qq.hahajie.cn

[M04] 获取当前工作目录
来源：http://gl.shtwfgs.cn

Py:   os.getcwd()
来源：http://kq.hahajie.cn

PHP:  getcwd();
来源：http://xy.hnjuh.cn

JS:   process.cwd()
来源：http://qc.huixinmuqiang.cn

TS:   process.cwd()
来源：http://sx.panjiajie.cn

Java: Path.of("").toAbsolutePath()
来源：http://jt.9csxet.cn

Go:   os.Getwd()
来源：http://uo.huixiangedu.cn

Ruby: Dir.pwd
来源：http://wd.huixinmuqiang.cn

C#:   Directory.GetCurrentDirectory()
来源：http://mx.muxihuayi.cn

[M05] 设置退出码
来源：http://na.shxzukj.cn

Py:   sys.exit(1)
来源：http://jb.asd995.cn

PHP:  exit(1);
来源：http://iw.shtwfgs.cn

JS:   process.exit(1)
来源：http://jc.yuexingan06.cn

TS:   process.exit(1)
来源：http://il.chemitech.net.cn

Java: System.exit(1)
来源：http://ie.chemitech.net.cn

Go:   os.Exit(1)
来源：http://wr.9csxet.cn

Ruby: exit 1
来源：http://np.newstarts.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ci.9csxet.cn

[M06] 向标准错误输出
来源：http://up.yuntaijiaju.cn

Py:   print("err", file=sys.stderr)
来源：http://vs.yuntaijiaju.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://zz.bjjhwx.cn

JS:   console.error("err")
来源：http://uu.jianghongdianzi.cn

TS:   console.error("err")
来源：http://in.shxzskj.cn

Java: System.err.println("err")
来源：http://ur.panjiajie.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://vn.huanxung.cn

Ruby: warn "err"
来源：http://bj.szsharing.cn

C#:   Console.Error.WriteLine("err")
来源：http://dg.yuntaijiaju.cn

[M07] 判断是否为主入口
来源：http://sr.colortex.cn

Py:   if __name__ == "__main__":
来源：http://mu.shxzskj.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://uc.huanxung.cn

JS:   require.main === module
来源：http://az.jianghongdianzi.cn

TS:   require.main === module
来源：http://kr.jctech888.com.cn

Java: public static void main(String[] args)
来源：http://gf.shtwfgs.cn

Go:   func main()
来源：http://je.gzmigu.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wo.newstarts.cn

C#:   static void Main(string[] args)
来源：http://cy.muxihuayi.cn

[M08] 获取系统与运行时信息
来源：http://bl.shtwfgs.cn

Py:   platform.system();  platform.python_version()
来源：http://ws.chemitech.net.cn

PHP:  PHP_OS;  phpversion();
来源：http://lt.gzmigu.cn

JS:   process.platform;  process.version
来源：http://so.chemitech.net.cn

TS:   process.platform;  process.version
来源：http://uu.huanxung.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://vc.jianghongdianzi.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ss.shxzukj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://tx.hahajie.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://lr.gzmigu.cn

================================================================================
来源：http://zf.9csxet.cn

N. 数据结构与算法
来源：http://pa.haigaiapp.cn

================================================================================
来源：http://hr.asd995.cn

[N01] 二分查找（有序数组）
来源：http://ck.521024.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ge.gzmigu.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://uc.hnjuh.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qk.huixiangedu.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://al.yuexingan06.cn

Java: Arrays.binarySearch(arr, x)
来源：http://jq.shxzskj.cn

Go:   sort.SearchInts(arr, x)
来源：http://pm.szxytkj.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://qn.jianghongdianzi.cn

C#:   Array.BinarySearch(arr, x)
来源：http://vb.yuexingan06.cn

[N02] 排序（工程实践用内置实现）
来源：http://mx.newstarts.cn

Py:   sorted(arr);  arr.sort()
来源：http://mu.newstarts.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ml.hnjuh.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ik.gzmigu.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://pq.nszjky.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://cq.shxzukj.cn

Go:   slices.Sort(arr)
来源：http://vl.yuexingan06.cn

Ruby: arr.sort
来源：http://ne.newstarts.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://vm.wgjwhj.cn

[N03] 快速排序（分治示例）
来源：http://tl.nicolike.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ma.haigaiapp.cn

PHP:  // 递归实现，或用 usort
来源：http://xc.panjiajie.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://el.shxzukj.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vm.bjjhwx.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://bk.szxytkj.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://xg.szsharing.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://sd.panjiajie.cn

C#:   // 手写递归，或 Array.Sort
来源：http://rw.nicolike.cn

[N04] 斐波那契数列
来源：http://vo.szsharing.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://di.yuexingan06.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://la.szsharing.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dp.huixiangedu.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ck.panjiajie.cn


<!-- 参考信息 -->