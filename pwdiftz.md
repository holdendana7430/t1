代发 wailian999

TS:   d1.getTime() < d2.getTime()
来源：http://ur.asd995.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xo.wgjwhj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://rg.shxzukj.cn

Ruby: d1 < d2;  d1 == d2
来源：http://wo.shxzskj.cn

C#:   d1 < d2;  d1 == d2
来源：http://nm.521024.cn

[J08] 提取年月日与星期
来源：http://ir.bjjhwx.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ya.yuntaijiaju.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://dp.chemitech.net.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ul.nicolike.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ww.huanxung.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://dn.nszjky.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://vk.nszjky.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ik.9csxet.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://sf.huixiangedu.cn

[J09] 时区处理
来源：http://ti.asd995.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://bf.wgjwhj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://lu.shxzukj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cm.nszjky.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rz.yuexingan06.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hk.huixinmuqiang.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://fk.9csxet.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://tm.bjjhwx.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://yy.wgjwhj.cn

[J10] 取今天 / 本月第一天
来源：http://qs.haigaiapp.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://js.shxzukj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://aw.hnjuh.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://xw.newstarts.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://au.haigaiapp.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://jn.szsharing.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ga.hahajie.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://lx.yuntaijiaju.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://iq.shtwfgs.cn

================================================================================
来源：http://tb.shxzukj.cn

K. JSON 与序列化
来源：http://si.shtwfgs.cn

================================================================================
来源：http://cu.shtwfgs.cn

[K01] 对象转 JSON 字符串
来源：http://cx.wgjwhj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://rb.huixinmuqiang.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://zr.nicolike.cn

JS:   JSON.stringify(obj)
来源：http://fj.shxzskj.cn

TS:   JSON.stringify(obj)
来源：http://ht.jctech888.com.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://qe.lnxyls.cn

Go:   json.Marshal(obj)
来源：http://qd.bookmarksfly.cn

Ruby: obj.to_json                                     // require "json"
来源：http://im.newstarts.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://yi.lnxyls.cn

[K02] JSON 字符串转对象
来源：http://ig.huanxung.cn

Py:   json.loads(s)
来源：http://hi.shxzskj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://bd.panjiajie.cn

JS:   JSON.parse(s)
来源：http://wc.shtwfgs.cn

TS:   JSON.parse(s)
来源：http://km.shxzskj.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://kk.colortex.cn

Go:   json.Unmarshal(data, &v)
来源：http://zc.huixiangedu.cn

Ruby: JSON.parse(s)
来源：http://oa.lnxyls.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://xu.shxzukj.cn

[K03] JSON 美化输出（带缩进）
来源：http://td.huanxung.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ui.bjjhwx.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://zb.yuexingan06.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://sk.muxihuayi.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://gy.colortex.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://oc.shtwfgs.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hq.jctech888.com.cn

Ruby: JSON.pretty_generate(obj)
来源：http://xw.newstarts.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://pp.haigaiapp.cn

[K04] 读取 JSON 文件
来源：http://lu.9csxet.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://xf.nicolike.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://jp.yuntaijiaju.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sw.yuntaijiaju.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://te.huixiangedu.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://rz.9csxet.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://kv.shxzskj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ep.nszjky.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ym.nszjky.cn

[K05] 深拷贝对象
来源：http://tg.yuntaijiaju.cn

Py:   copy.deepcopy(obj)
来源：http://vc.bjjhwx.cn

PHP:  unserialize(serialize($obj));
来源：http://qs.shxzukj.cn

JS:   structuredClone(obj)
来源：http://zy.9csxet.cn

TS:   structuredClone(obj)
来源：http://gu.gzmigu.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://jc.hahajie.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://rd.nszjky.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wo.bookmarksfly.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://vj.shtwfgs.cn

[K06] 解析 URL 查询串
来源：http://yp.yuntaijiaju.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ih.bjjhwx.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://qm.shxzskj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ll.szxytkj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cf.szxytkj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://pd.yuntaijiaju.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://zg.muxihuayi.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://tb.lnxyls.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://vs.wgjwhj.cn

[K07] 进制转换
来源：http://xg.yuntaijiaju.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ma.szsharing.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://lc.jianghongdianzi.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://qk.szxytkj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://tr.hnjuh.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wm.asd995.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mf.shtwfgs.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://xh.jctech888.com.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ax.nicolike.cn

[K08] 二进制序列化（非 JSON）
来源：http://ut.gzmigu.cn

Py:   pickle.dumps(obj)
来源：http://yh.nicolike.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://nv.huixinmuqiang.cn

JS:   v8.serialize(obj)        // Node
来源：http://in.panjiajie.cn

TS:   v8.serialize(obj)        // Node
来源：http://oi.hahajie.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://vf.wgjwhj.cn

Go:   encoding/gob
来源：http://kg.muxihuayi.cn

Ruby: Marshal.dump(obj)
来源：http://tp.newstarts.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://iq.521024.cn

================================================================================
来源：http://ts.huixinmuqiang.cn

L. 网络请求
来源：http://cx.szxytkj.cn

================================================================================
来源：http://cn.bjjhwx.cn

[L01] 发送 GET 请求
来源：http://ys.jctech888.com.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://pw.huixinmuqiang.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://kp.jctech888.com.cn

JS:   await fetch(url)
来源：http://fq.asd995.cn

TS:   await fetch(url)
来源：http://fx.muxihuayi.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qy.shxzskj.cn

Go:   resp, err := http.Get(url)
来源：http://hu.521024.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://zr.panjiajie.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.newstarts.cn

[L02] 发送 POST JSON
来源：http://cz.9csxet.cn

Py:   requests.post(url, json={"a": 1})
来源：http://pp.gzmigu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://tf.shxzukj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dv.shxzskj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zm.9csxet.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ko.asd995.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jz.bookmarksfly.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://qz.gzmigu.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://iq.muxihuayi.cn

[L03] 设置自定义请求头
来源：http://aq.szxytkj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://qc.wgjwhj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://nt.panjiajie.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ua.jianghongdianzi.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zu.9csxet.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://au.chemitech.net.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://qj.huixiangedu.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://vx.colortex.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ai.szxytkj.cn

[L04] 设置超时
来源：http://kj.colortex.cn

Py:   requests.get(url, timeout=5)
来源：http://is.nszjky.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://vk.newstarts.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zr.huixiangedu.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jw.bjjhwx.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://dp.shxzskj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ea.bookmarksfly.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://bo.gzmigu.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://rp.colortex.cn

[L05] 上传文件（multipart）
来源：http://gf.huixinmuqiang.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://lg.521024.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://kl.yuntaijiaju.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://kt.szxytkj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://zu.chemitech.net.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vw.szsharing.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://sm.jianghongdianzi.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://nb.szsharing.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://to.shtwfgs.cn

[L06] 解析响应为 JSON
来源：http://vb.yuntaijiaju.cn

Py:   resp.json()
来源：http://ry.bjjhwx.cn

PHP:  json_decode($body, true);
来源：http://zm.9csxet.cn

JS:   await resp.json()
来源：http://kk.huanxung.cn

TS:   await resp.json()
来源：http://nn.521024.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://se.chemitech.net.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wf.jctech888.com.cn

Ruby: JSON.parse(resp.body)
来源：http://ed.shtwfgs.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://up.newstarts.cn

[L07] 处理 HTTP 状态码
来源：http://nb.yuexingan06.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://jn.nszjky.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://kf.huixiangedu.cn

JS:   resp.ok;  resp.status
来源：http://ni.9csxet.cn

TS:   resp.ok;  resp.status
来源：http://mo.huixinmuqiang.cn

Java: resp.statusCode()
来源：http://xs.bjjhwx.cn

Go:   resp.StatusCode
来源：http://pa.chemitech.net.cn

Ruby: resp.code.to_i
来源：http://bx.szsharing.cn

C#:   (int)resp.StatusCode
来源：http://mo.huixiangedu.cn

[L08] 并发请求多个地址
来源：http://gz.szsharing.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ux.jianghongdianzi.cn

PHP:  curl_multi_init() 系列
来源：http://nc.haigaiapp.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mc.521024.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ky.muxihuayi.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://fs.lnxyls.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qy.jianghongdianzi.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ko.haigaiapp.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wz.9csxet.cn

================================================================================
来源：http://yw.hahajie.cn

M. 命令行 / 进程 / 环境
来源：http://he.9csxet.cn

================================================================================
来源：http://ds.huixinmuqiang.cn

[M01] 读取命令行参数
来源：http://gu.yuntaijiaju.cn

Py:   sys.argv[1:]
来源：http://pz.newstarts.cn

PHP:  $argv;  $argc;
来源：http://pe.shxzskj.cn

JS:   process.argv.slice(2)
来源：http://ym.jctech888.com.cn

TS:   process.argv.slice(2)
来源：http://ek.9csxet.cn

Java: args 数组（main 方法参数）
来源：http://xg.9csxet.cn

Go:   os.Args[1:]
来源：http://zk.521024.cn

Ruby: ARGV
来源：http://xx.hnjuh.cn

C#:   args 数组（Main 方法参数）
来源：http://zg.huanxung.cn

[M02] 读取环境变量
来源：http://iu.nicolike.cn

Py:   os.environ.get("HOME")
来源：http://vv.szxytkj.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://lg.9csxet.cn

JS:   process.env.HOME
来源：http://mn.gzmigu.cn

TS:   process.env.HOME
来源：http://fs.colortex.cn

Java: System.getenv("HOME")
来源：http://ss.gzmigu.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://yz.yuexingan06.cn

Ruby: ENV["HOME"]
来源：http://mz.bookmarksfly.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ib.wgjwhj.cn

[M03] 执行外部命令
来源：http://sp.lnxyls.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ui.jctech888.com.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://vh.jianghongdianzi.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://rm.hnjuh.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ma.yuntaijiaju.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ty.bookmarksfly.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://xw.haigaiapp.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ig.bookmarksfly.cn

C#:   Process.Start("ls", "-l");
来源：http://tu.asd995.cn

[M04] 获取当前工作目录
来源：http://lw.jianghongdianzi.cn

Py:   os.getcwd()
来源：http://qw.szxytkj.cn

PHP:  getcwd();
来源：http://yn.panjiajie.cn

JS:   process.cwd()
来源：http://rs.bookmarksfly.cn

TS:   process.cwd()
来源：http://su.newstarts.cn

Java: Path.of("").toAbsolutePath()
来源：http://oi.shxzukj.cn

Go:   os.Getwd()
来源：http://xp.wgjwhj.cn

Ruby: Dir.pwd
来源：http://xk.shxzukj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://cf.asd995.cn

[M05] 设置退出码
来源：http://ck.yuexingan06.cn

Py:   sys.exit(1)
来源：http://lv.hahajie.cn

PHP:  exit(1);
来源：http://lm.wgjwhj.cn

JS:   process.exit(1)
来源：http://en.nicolike.cn

TS:   process.exit(1)
来源：http://dd.szsharing.cn

Java: System.exit(1)
来源：http://ld.shtwfgs.cn

Go:   os.Exit(1)
来源：http://xp.szxytkj.cn

Ruby: exit 1
来源：http://pg.newstarts.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://fx.wgjwhj.cn

[M06] 向标准错误输出
来源：http://bo.shxzukj.cn

Py:   print("err", file=sys.stderr)
来源：http://ek.haigaiapp.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://zf.huixinmuqiang.cn

JS:   console.error("err")
来源：http://bu.muxihuayi.cn

TS:   console.error("err")
来源：http://sj.bjjhwx.cn

Java: System.err.println("err")
来源：http://ss.shtwfgs.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://xl.shxzskj.cn

Ruby: warn "err"
来源：http://an.9csxet.cn

C#:   Console.Error.WriteLine("err")
来源：http://sk.shtwfgs.cn

[M07] 判断是否为主入口
来源：http://jw.shxzukj.cn

Py:   if __name__ == "__main__":
来源：http://ik.szxytkj.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hd.yuntaijiaju.cn

JS:   require.main === module
来源：http://xo.chemitech.net.cn

TS:   require.main === module
来源：http://mp.yuexingan06.cn

Java: public static void main(String[] args)
来源：http://pa.szxytkj.cn

Go:   func main()
来源：http://le.asd995.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ie.bookmarksfly.cn

C#:   static void Main(string[] args)
来源：http://ft.hnjuh.cn

[M08] 获取系统与运行时信息
来源：http://cp.szxytkj.cn

Py:   platform.system();  platform.python_version()
来源：http://yh.wgjwhj.cn

PHP:  PHP_OS;  phpversion();
来源：http://ui.gzmigu.cn

JS:   process.platform;  process.version
来源：http://vd.newstarts.cn

TS:   process.platform;  process.version
来源：http://ca.asd995.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://zs.jianghongdianzi.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://tw.521024.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ny.hnjuh.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://wr.newstarts.cn

================================================================================
来源：http://sl.shxzskj.cn

N. 数据结构与算法
来源：http://ah.gzmigu.cn

================================================================================
来源：http://vs.newstarts.cn

[N01] 二分查找（有序数组）
来源：http://af.wgjwhj.cn

Py:   bisect.bisect_left(arr, x)
来源：http://hb.asd995.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://jv.hnjuh.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sd.shtwfgs.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gp.nicolike.cn

Java: Arrays.binarySearch(arr, x)
来源：http://tu.szsharing.cn

Go:   sort.SearchInts(arr, x)
来源：http://tu.panjiajie.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://jp.yuntaijiaju.cn

C#:   Array.BinarySearch(arr, x)
来源：http://vh.wgjwhj.cn

[N02] 排序（工程实践用内置实现）
来源：http://ah.szxytkj.cn

Py:   sorted(arr);  arr.sort()
来源：http://ah.bjjhwx.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ay.huanxung.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://re.9csxet.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://yr.asd995.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://za.huixiangedu.cn

Go:   slices.Sort(arr)
来源：http://vo.hahajie.cn

Ruby: arr.sort
来源：http://xu.shxzskj.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ew.szsharing.cn

[N03] 快速排序（分治示例）
来源：http://uy.shtwfgs.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://yd.panjiajie.cn

PHP:  // 递归实现，或用 usort
来源：http://an.nszjky.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wd.9csxet.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vr.shxzukj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://zg.muxihuayi.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://cd.panjiajie.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://tn.bjjhwx.cn

C#:   // 手写递归，或 Array.Sort
来源：http://wb.nicolike.cn

[N04] 斐波那契数列
来源：http://vq.lnxyls.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://vj.shtwfgs.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://te.asd995.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jn.9csxet.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fs.shxzskj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://nx.wgjwhj.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://un.hnjuh.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://am.nicolike.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://af.shtwfgs.cn

[N05] 最大公约数
来源：http://qg.521024.cn

Py:   math.gcd(a, b)
来源：http://nn.jianghongdianzi.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://lj.shxzskj.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rs.panjiajie.cn


<!-- 参考信息 -->