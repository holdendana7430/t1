代发 wailian999

[J07] 比较两个日期
来源：http://jt.hahajie.cn

Py:   d1 < d2;  d1 == d2
来源：http://gf.panjiajie.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://yy.521024.cn

JS:   d1.getTime() < d2.getTime()
来源：http://we.yuexingan06.cn

TS:   d1.getTime() < d2.getTime()
来源：http://lp.huixinmuqiang.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mj.colortex.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ou.wgjwhj.cn

Ruby: d1 < d2;  d1 == d2
来源：http://oe.lnxyls.cn

C#:   d1 < d2;  d1 == d2
来源：http://ue.newstarts.cn

[J08] 提取年月日与星期
来源：http://pf.gzmigu.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hw.wgjwhj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://gz.panjiajie.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://kr.shxzskj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://en.chemitech.net.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hl.shtwfgs.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://su.9csxet.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ao.chemitech.net.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ds.huixinmuqiang.cn

[J09] 时区处理
来源：http://gp.huixiangedu.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ql.wgjwhj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ld.wgjwhj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mi.szxytkj.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bk.jianghongdianzi.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://et.yuexingan06.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wr.wgjwhj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ph.muxihuayi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ov.szxytkj.cn

[J10] 取今天 / 本月第一天
来源：http://cy.nicolike.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ol.gzmigu.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://vu.szxytkj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://xo.jianghongdianzi.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qv.hnjuh.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wl.szsharing.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://zu.szxytkj.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://xk.521024.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://iy.huixinmuqiang.cn

================================================================================
来源：http://hz.bookmarksfly.cn

K. JSON 与序列化
来源：http://az.huixiangedu.cn

================================================================================
来源：http://kz.haigaiapp.cn

[K01] 对象转 JSON 字符串
来源：http://vw.9csxet.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://vn.panjiajie.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://kk.lnxyls.cn

JS:   JSON.stringify(obj)
来源：http://ig.huanxung.cn

TS:   JSON.stringify(obj)
来源：http://zs.panjiajie.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ar.colortex.cn

Go:   json.Marshal(obj)
来源：http://dx.bjjhwx.cn

Ruby: obj.to_json                                     // require "json"
来源：http://bm.nicolike.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://wy.huanxung.cn

[K02] JSON 字符串转对象
来源：http://ju.chemitech.net.cn

Py:   json.loads(s)
来源：http://oe.shxzskj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://tf.nicolike.cn

JS:   JSON.parse(s)
来源：http://sx.colortex.cn

TS:   JSON.parse(s)
来源：http://mj.bookmarksfly.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ld.lnxyls.cn

Go:   json.Unmarshal(data, &v)
来源：http://ho.521024.cn

Ruby: JSON.parse(s)
来源：http://tz.bookmarksfly.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://se.szsharing.cn

[K03] JSON 美化输出（带缩进）
来源：http://qa.nszjky.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wl.hnjuh.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ed.huixiangedu.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://gr.haigaiapp.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://mw.bookmarksfly.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ba.bookmarksfly.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ph.szsharing.cn

Ruby: JSON.pretty_generate(obj)
来源：http://mg.9csxet.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hf.szxytkj.cn

[K04] 读取 JSON 文件
来源：http://gy.nicolike.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://gl.jctech888.com.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wz.bookmarksfly.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kf.9csxet.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vt.hnjuh.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://nt.hnjuh.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://dl.bookmarksfly.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://dk.jctech888.com.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://cl.shtwfgs.cn

[K05] 深拷贝对象
来源：http://qf.asd995.cn

Py:   copy.deepcopy(obj)
来源：http://ps.shxzukj.cn

PHP:  unserialize(serialize($obj));
来源：http://fl.asd995.cn

JS:   structuredClone(obj)
来源：http://rb.nicolike.cn

TS:   structuredClone(obj)
来源：http://cw.yuexingan06.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://jn.shxzukj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://vg.colortex.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://cr.nszjky.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://fq.lnxyls.cn

[K06] 解析 URL 查询串
来源：http://bd.huanxung.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://bs.wgjwhj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://cj.wgjwhj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uf.shxzskj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qt.bookmarksfly.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://fl.huanxung.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://fc.jctech888.com.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://xb.yuntaijiaju.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://kc.shxzskj.cn

[K07] 进制转换
来源：http://md.colortex.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ov.huixiangedu.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://bt.lnxyls.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://zn.hahajie.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://dr.shxzukj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://cv.nszjky.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ht.panjiajie.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://jv.shtwfgs.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://qt.shtwfgs.cn

[K08] 二进制序列化（非 JSON）
来源：http://kc.yuexingan06.cn

Py:   pickle.dumps(obj)
来源：http://mh.huixinmuqiang.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://nr.shtwfgs.cn

JS:   v8.serialize(obj)        // Node
来源：http://ft.gzmigu.cn

TS:   v8.serialize(obj)        // Node
来源：http://if.yuexingan06.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://yo.szxytkj.cn

Go:   encoding/gob
来源：http://dh.jctech888.com.cn

Ruby: Marshal.dump(obj)
来源：http://dz.asd995.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ra.huanxung.cn

================================================================================
来源：http://am.huixinmuqiang.cn

L. 网络请求
来源：http://kw.nszjky.cn

================================================================================
来源：http://sf.asd995.cn

[L01] 发送 GET 请求
来源：http://fz.9csxet.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://gu.521024.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vk.huixiangedu.cn

JS:   await fetch(url)
来源：http://vg.bjjhwx.cn

TS:   await fetch(url)
来源：http://um.huixinmuqiang.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://th.szsharing.cn

Go:   resp, err := http.Get(url)
来源：http://cb.yuexingan06.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://mw.yuexingan06.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://fn.asd995.cn

[L02] 发送 POST JSON
来源：http://cx.huixinmuqiang.cn

Py:   requests.post(url, json={"a": 1})
来源：http://gf.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://gf.newstarts.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hr.gzmigu.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mk.szxytkj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ke.yuntaijiaju.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://cg.lnxyls.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://gp.nicolike.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wv.colortex.cn

[L03] 设置自定义请求头
来源：http://fa.lnxyls.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mk.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://pd.huixiangedu.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jm.nicolike.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fa.yuntaijiaju.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://bp.yuexingan06.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://zo.panjiajie.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://xl.nszjky.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://rs.hahajie.cn

[L04] 设置超时
来源：http://ut.yuexingan06.cn

Py:   requests.get(url, timeout=5)
来源：http://qp.szxytkj.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://bq.newstarts.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hu.huixinmuqiang.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ep.nicolike.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://bx.9csxet.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mt.huixiangedu.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://od.szxytkj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hi.shtwfgs.cn

[L05] 上传文件（multipart）
来源：http://ms.jianghongdianzi.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://yf.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wh.jianghongdianzi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://iy.panjiajie.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://sc.chemitech.net.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://qt.bjjhwx.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://li.chemitech.net.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ik.shtwfgs.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://yz.shtwfgs.cn

[L06] 解析响应为 JSON
来源：http://fz.panjiajie.cn

Py:   resp.json()
来源：http://ny.521024.cn

PHP:  json_decode($body, true);
来源：http://ce.szxytkj.cn

JS:   await resp.json()
来源：http://id.bjjhwx.cn

TS:   await resp.json()
来源：http://by.yuntaijiaju.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://tu.shtwfgs.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hg.yuntaijiaju.cn

Ruby: JSON.parse(resp.body)
来源：http://ph.muxihuayi.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://pe.yuntaijiaju.cn

[L07] 处理 HTTP 状态码
来源：http://ab.yuexingan06.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ge.bjjhwx.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://vt.nszjky.cn

JS:   resp.ok;  resp.status
来源：http://lq.bookmarksfly.cn

TS:   resp.ok;  resp.status
来源：http://sp.jianghongdianzi.cn

Java: resp.statusCode()
来源：http://bc.shxzskj.cn

Go:   resp.StatusCode
来源：http://kb.lnxyls.cn

Ruby: resp.code.to_i
来源：http://pu.hahajie.cn

C#:   (int)resp.StatusCode
来源：http://nz.panjiajie.cn

[L08] 并发请求多个地址
来源：http://tm.muxihuayi.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hm.muxihuayi.cn

PHP:  curl_multi_init() 系列
来源：http://by.newstarts.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qk.nszjky.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ex.huanxung.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ql.hahajie.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://yg.haigaiapp.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ht.newstarts.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://qu.hahajie.cn

================================================================================
来源：http://kt.asd995.cn

M. 命令行 / 进程 / 环境
来源：http://ir.yuntaijiaju.cn

================================================================================
来源：http://xz.haigaiapp.cn

[M01] 读取命令行参数
来源：http://pc.huanxung.cn

Py:   sys.argv[1:]
来源：http://rb.nicolike.cn

PHP:  $argv;  $argc;
来源：http://fq.newstarts.cn

JS:   process.argv.slice(2)
来源：http://ox.shxzskj.cn

TS:   process.argv.slice(2)
来源：http://eq.nszjky.cn

Java: args 数组（main 方法参数）
来源：http://ez.shxzukj.cn

Go:   os.Args[1:]
来源：http://nb.haigaiapp.cn

Ruby: ARGV
来源：http://zc.hahajie.cn

C#:   args 数组（Main 方法参数）
来源：http://jr.nicolike.cn

[M02] 读取环境变量
来源：http://ti.9csxet.cn

Py:   os.environ.get("HOME")
来源：http://ez.521024.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ti.shxzukj.cn

JS:   process.env.HOME
来源：http://vd.szxytkj.cn

TS:   process.env.HOME
来源：http://dd.panjiajie.cn

Java: System.getenv("HOME")
来源：http://dx.jianghongdianzi.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://dn.chemitech.net.cn

Ruby: ENV["HOME"]
来源：http://ab.szxytkj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://aw.yuntaijiaju.cn

[M03] 执行外部命令
来源：http://ih.colortex.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://do.hnjuh.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://co.szxytkj.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://xv.huanxung.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://kg.hahajie.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://sf.szsharing.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://qq.panjiajie.cn

Ruby: system("ls -l");  `ls -l`
来源：http://pf.bjjhwx.cn

C#:   Process.Start("ls", "-l");
来源：http://id.521024.cn

[M04] 获取当前工作目录
来源：http://vj.jianghongdianzi.cn

Py:   os.getcwd()
来源：http://th.bjjhwx.cn

PHP:  getcwd();
来源：http://ez.hahajie.cn

JS:   process.cwd()
来源：http://px.colortex.cn

TS:   process.cwd()
来源：http://rw.lnxyls.cn

Java: Path.of("").toAbsolutePath()
来源：http://yw.hahajie.cn

Go:   os.Getwd()
来源：http://bd.shxzskj.cn

Ruby: Dir.pwd
来源：http://oi.bjjhwx.cn

C#:   Directory.GetCurrentDirectory()
来源：http://uf.jctech888.com.cn

[M05] 设置退出码
来源：http://ww.nszjky.cn

Py:   sys.exit(1)
来源：http://cp.szsharing.cn

PHP:  exit(1);
来源：http://ke.szxytkj.cn

JS:   process.exit(1)
来源：http://og.521024.cn

TS:   process.exit(1)
来源：http://hd.newstarts.cn

Java: System.exit(1)
来源：http://vn.yuexingan06.cn

Go:   os.Exit(1)
来源：http://lg.shxzskj.cn

Ruby: exit 1
来源：http://lx.yuexingan06.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ms.lnxyls.cn

[M06] 向标准错误输出
来源：http://cn.muxihuayi.cn

Py:   print("err", file=sys.stderr)
来源：http://kq.szxytkj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ni.colortex.cn

JS:   console.error("err")
来源：http://lf.panjiajie.cn

TS:   console.error("err")
来源：http://wj.bookmarksfly.cn

Java: System.err.println("err")
来源：http://tk.nicolike.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ke.huanxung.cn

Ruby: warn "err"
来源：http://bf.bookmarksfly.cn

C#:   Console.Error.WriteLine("err")
来源：http://dr.9csxet.cn

[M07] 判断是否为主入口
来源：http://dk.jianghongdianzi.cn

Py:   if __name__ == "__main__":
来源：http://re.jctech888.com.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://oe.shxzukj.cn

JS:   require.main === module
来源：http://uk.shxzskj.cn

TS:   require.main === module
来源：http://us.gzmigu.cn

Java: public static void main(String[] args)
来源：http://ba.jianghongdianzi.cn

Go:   func main()
来源：http://jc.bookmarksfly.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mf.szxytkj.cn

C#:   static void Main(string[] args)
来源：http://ph.shtwfgs.cn

[M08] 获取系统与运行时信息
来源：http://ew.lnxyls.cn

Py:   platform.system();  platform.python_version()
来源：http://xe.wgjwhj.cn

PHP:  PHP_OS;  phpversion();
来源：http://ey.bookmarksfly.cn

JS:   process.platform;  process.version
来源：http://ck.gzmigu.cn

TS:   process.platform;  process.version
来源：http://dv.bookmarksfly.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://cn.yuexingan06.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://of.nicolike.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://xc.huixinmuqiang.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://mb.gzmigu.cn

================================================================================
来源：http://sf.9csxet.cn

N. 数据结构与算法
来源：http://sj.9csxet.cn

================================================================================
来源：http://md.huixinmuqiang.cn

[N01] 二分查找（有序数组）
来源：http://wb.colortex.cn

Py:   bisect.bisect_left(arr, x)
来源：http://gf.szsharing.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://xa.panjiajie.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yb.asd995.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ng.hahajie.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ai.asd995.cn

Go:   sort.SearchInts(arr, x)
来源：http://qg.yuntaijiaju.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://fd.shxzukj.cn

C#:   Array.BinarySearch(arr, x)
来源：http://hr.jianghongdianzi.cn

[N02] 排序（工程实践用内置实现）
来源：http://wr.jianghongdianzi.cn

Py:   sorted(arr);  arr.sort()
来源：http://bi.lnxyls.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://sy.yuntaijiaju.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://gm.hnjuh.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ey.shxzukj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ef.huanxung.cn

Go:   slices.Sort(arr)
来源：http://js.huanxung.cn

Ruby: arr.sort
来源：http://pv.jianghongdianzi.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://nq.chemitech.net.cn

[N03] 快速排序（分治示例）
来源：http://dq.yuntaijiaju.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hf.hnjuh.cn

PHP:  // 递归实现，或用 usort
来源：http://lf.yuexingan06.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://en.newstarts.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sk.lnxyls.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ql.newstarts.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://zq.huanxung.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://lb.jctech888.com.cn

C#:   // 手写递归，或 Array.Sort
来源：http://un.muxihuayi.cn

[N04] 斐波那契数列
来源：http://nk.9csxet.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qi.hnjuh.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wu.panjiajie.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vb.shxzukj.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qh.huixiangedu.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://dz.bookmarksfly.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://aj.jctech888.com.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://cq.shxzukj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://sg.lnxyls.cn


<!-- 参考信息 -->