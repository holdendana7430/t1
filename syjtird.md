代发 wailian999

[J07] 比较两个日期
来源：http://ct.yuexingan06.cn

Py:   d1 < d2;  d1 == d2
来源：http://oq.hnjuh.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wo.huixinmuqiang.cn

JS:   d1.getTime() < d2.getTime()
来源：http://bj.shtwfgs.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ij.huanxung.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://yf.jianghongdianzi.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://tv.nicolike.cn

Ruby: d1 < d2;  d1 == d2
来源：http://na.haigaiapp.cn

C#:   d1 < d2;  d1 == d2
来源：http://hp.gzmigu.cn

[J08] 提取年月日与星期
来源：http://ux.shxzskj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hx.lnxyls.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://qr.asd995.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://rg.haigaiapp.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wz.bookmarksfly.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://bz.hnjuh.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://yw.jctech888.com.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://pg.huixiangedu.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hl.bookmarksfly.cn

[J09] 时区处理
来源：http://fw.shxzukj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ya.haigaiapp.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://fp.521024.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cm.hnjuh.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uu.521024.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://nw.huanxung.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://js.huixiangedu.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://mn.shtwfgs.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wu.panjiajie.cn

[J10] 取今天 / 本月第一天
来源：http://vv.hnjuh.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://vh.yuexingan06.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://cz.gzmigu.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ho.szxytkj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wo.muxihuayi.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://dz.haigaiapp.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://nj.shxzskj.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ma.jianghongdianzi.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ev.9csxet.cn

================================================================================
来源：http://oo.bjjhwx.cn

K. JSON 与序列化
来源：http://fw.chemitech.net.cn

================================================================================
来源：http://yp.jianghongdianzi.cn

[K01] 对象转 JSON 字符串
来源：http://sk.lnxyls.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ci.yuexingan06.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ww.szxytkj.cn

JS:   JSON.stringify(obj)
来源：http://qk.shxzskj.cn

TS:   JSON.stringify(obj)
来源：http://ob.haigaiapp.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wi.bjjhwx.cn

Go:   json.Marshal(obj)
来源：http://yl.jctech888.com.cn

Ruby: obj.to_json                                     // require "json"
来源：http://gl.yuexingan06.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://lh.panjiajie.cn

[K02] JSON 字符串转对象
来源：http://pj.bjjhwx.cn

Py:   json.loads(s)
来源：http://hs.nszjky.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://am.asd995.cn

JS:   JSON.parse(s)
来源：http://in.haigaiapp.cn

TS:   JSON.parse(s)
来源：http://gp.chemitech.net.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jp.bookmarksfly.cn

Go:   json.Unmarshal(data, &v)
来源：http://gk.asd995.cn

Ruby: JSON.parse(s)
来源：http://gw.yuntaijiaju.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://oo.jianghongdianzi.cn

[K03] JSON 美化输出（带缩进）
来源：http://lr.colortex.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://cb.colortex.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://zd.szsharing.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://il.lnxyls.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://zy.shxzskj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qu.hnjuh.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ja.szsharing.cn

Ruby: JSON.pretty_generate(obj)
来源：http://yb.bjjhwx.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mp.muxihuayi.cn

[K04] 读取 JSON 文件
来源：http://wv.colortex.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mo.yuexingan06.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hf.yuexingan06.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ve.nicolike.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rs.huixiangedu.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://my.haigaiapp.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ws.muxihuayi.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ck.jctech888.com.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://dt.yuntaijiaju.cn

[K05] 深拷贝对象
来源：http://at.bookmarksfly.cn

Py:   copy.deepcopy(obj)
来源：http://uj.jianghongdianzi.cn

PHP:  unserialize(serialize($obj));
来源：http://dy.shxzskj.cn

JS:   structuredClone(obj)
来源：http://gx.newstarts.cn

TS:   structuredClone(obj)
来源：http://ox.shxzskj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://in.szxytkj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://cp.haigaiapp.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mp.nszjky.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://qy.gzmigu.cn

[K06] 解析 URL 查询串
来源：http://wj.huixiangedu.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://jf.muxihuayi.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://rb.chemitech.net.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://za.huanxung.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ye.jctech888.com.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://jw.huixinmuqiang.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ma.haigaiapp.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ly.521024.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wh.gzmigu.cn

[K07] 进制转换
来源：http://jl.huixinmuqiang.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://cx.yuexingan06.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vo.shxzskj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://in.bookmarksfly.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://kz.szxytkj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://pk.shxzukj.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://nq.szsharing.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://sj.haigaiapp.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ql.yuntaijiaju.cn

[K08] 二进制序列化（非 JSON）
来源：http://bp.panjiajie.cn

Py:   pickle.dumps(obj)
来源：http://io.colortex.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ba.nszjky.cn

JS:   v8.serialize(obj)        // Node
来源：http://of.huixinmuqiang.cn

TS:   v8.serialize(obj)        // Node
来源：http://vu.9csxet.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mt.nszjky.cn

Go:   encoding/gob
来源：http://mu.yuexingan06.cn

Ruby: Marshal.dump(obj)
来源：http://yd.nszjky.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://dq.shxzukj.cn

================================================================================
来源：http://tu.chemitech.net.cn

L. 网络请求
来源：http://ai.shxzskj.cn

================================================================================
来源：http://lh.521024.cn

[L01] 发送 GET 请求
来源：http://jx.muxihuayi.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xr.wgjwhj.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://iu.shxzukj.cn

JS:   await fetch(url)
来源：http://iu.yuexingan06.cn

TS:   await fetch(url)
来源：http://dg.colortex.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://kr.shtwfgs.cn

Go:   resp, err := http.Get(url)
来源：http://av.nicolike.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://dl.gzmigu.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://nq.hnjuh.cn

[L02] 发送 POST JSON
来源：http://qc.chemitech.net.cn

Py:   requests.post(url, json={"a": 1})
来源：http://lj.asd995.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://zj.panjiajie.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yv.asd995.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://se.szsharing.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://sj.huanxung.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ug.szsharing.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://po.gzmigu.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://il.szxytkj.cn

[L03] 设置自定义请求头
来源：http://rh.huanxung.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mn.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://fr.huanxung.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rs.haigaiapp.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rh.chemitech.net.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://jn.shxzukj.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ic.nszjky.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://fm.shxzskj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://gl.gzmigu.cn

[L04] 设置超时
来源：http://yu.colortex.cn

Py:   requests.get(url, timeout=5)
来源：http://jc.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://aa.jctech888.com.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ro.lnxyls.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zv.newstarts.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://og.nszjky.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://kx.muxihuayi.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://yo.szsharing.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://od.chemitech.net.cn

[L05] 上传文件（multipart）
来源：http://nu.lnxyls.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://lh.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ri.nicolike.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://oz.huanxung.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mw.nicolike.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://uu.yuexingan06.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ml.szsharing.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://gp.huanxung.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://py.gzmigu.cn

[L06] 解析响应为 JSON
来源：http://uc.hahajie.cn

Py:   resp.json()
来源：http://uf.huanxung.cn

PHP:  json_decode($body, true);
来源：http://ik.shxzskj.cn

JS:   await resp.json()
来源：http://my.yuexingan06.cn

TS:   await resp.json()
来源：http://ov.nszjky.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://gi.hnjuh.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mn.haigaiapp.cn

Ruby: JSON.parse(resp.body)
来源：http://db.chemitech.net.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://eg.hnjuh.cn

[L07] 处理 HTTP 状态码
来源：http://no.nicolike.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ze.newstarts.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://oh.shtwfgs.cn

JS:   resp.ok;  resp.status
来源：http://rh.yuexingan06.cn

TS:   resp.ok;  resp.status
来源：http://fd.panjiajie.cn

Java: resp.statusCode()
来源：http://jw.nicolike.cn

Go:   resp.StatusCode
来源：http://dw.gzmigu.cn

Ruby: resp.code.to_i
来源：http://ol.huixiangedu.cn

C#:   (int)resp.StatusCode
来源：http://cz.chemitech.net.cn

[L08] 并发请求多个地址
来源：http://gs.chemitech.net.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ry.colortex.cn

PHP:  curl_multi_init() 系列
来源：http://kn.nszjky.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://et.hahajie.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bw.shxzukj.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ic.szxytkj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://nn.hahajie.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://tm.shtwfgs.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://oc.jianghongdianzi.cn

================================================================================
来源：http://ad.lnxyls.cn

M. 命令行 / 进程 / 环境
来源：http://pr.huanxung.cn

================================================================================
来源：http://gi.bjjhwx.cn

[M01] 读取命令行参数
来源：http://ia.yuexingan06.cn

Py:   sys.argv[1:]
来源：http://ly.wgjwhj.cn

PHP:  $argv;  $argc;
来源：http://tf.lnxyls.cn

JS:   process.argv.slice(2)
来源：http://dw.muxihuayi.cn

TS:   process.argv.slice(2)
来源：http://xd.nicolike.cn

Java: args 数组（main 方法参数）
来源：http://ou.bookmarksfly.cn

Go:   os.Args[1:]
来源：http://or.wgjwhj.cn

Ruby: ARGV
来源：http://uw.newstarts.cn

C#:   args 数组（Main 方法参数）
来源：http://bw.wgjwhj.cn

[M02] 读取环境变量
来源：http://ev.colortex.cn

Py:   os.environ.get("HOME")
来源：http://bp.chemitech.net.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ej.yuntaijiaju.cn

JS:   process.env.HOME
来源：http://ja.shxzskj.cn

TS:   process.env.HOME
来源：http://mf.shtwfgs.cn

Java: System.getenv("HOME")
来源：http://zc.colortex.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://gi.colortex.cn

Ruby: ENV["HOME"]
来源：http://vu.gzmigu.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ge.jianghongdianzi.cn

[M03] 执行外部命令
来源：http://ps.bookmarksfly.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://fk.hnjuh.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://sf.huixinmuqiang.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://dt.shtwfgs.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://tu.colortex.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://gt.shxzukj.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ss.muxihuayi.cn

Ruby: system("ls -l");  `ls -l`
来源：http://re.shxzukj.cn

C#:   Process.Start("ls", "-l");
来源：http://qv.bjjhwx.cn

[M04] 获取当前工作目录
来源：http://bw.nszjky.cn

Py:   os.getcwd()
来源：http://cg.521024.cn

PHP:  getcwd();
来源：http://mc.szsharing.cn

JS:   process.cwd()
来源：http://oj.521024.cn

TS:   process.cwd()
来源：http://uw.newstarts.cn

Java: Path.of("").toAbsolutePath()
来源：http://fx.haigaiapp.cn

Go:   os.Getwd()
来源：http://uj.bjjhwx.cn

Ruby: Dir.pwd
来源：http://hs.huixinmuqiang.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ad.nszjky.cn

[M05] 设置退出码
来源：http://yx.chemitech.net.cn

Py:   sys.exit(1)
来源：http://ko.shtwfgs.cn

PHP:  exit(1);
来源：http://pq.newstarts.cn

JS:   process.exit(1)
来源：http://dj.chemitech.net.cn

TS:   process.exit(1)
来源：http://wu.521024.cn

Java: System.exit(1)
来源：http://ub.asd995.cn

Go:   os.Exit(1)
来源：http://eh.shxzskj.cn

Ruby: exit 1
来源：http://xt.muxihuayi.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ny.jctech888.com.cn

[M06] 向标准错误输出
来源：http://zp.jianghongdianzi.cn

Py:   print("err", file=sys.stderr)
来源：http://zf.yuexingan06.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://vu.521024.cn

JS:   console.error("err")
来源：http://du.yuntaijiaju.cn

TS:   console.error("err")
来源：http://yt.nicolike.cn

Java: System.err.println("err")
来源：http://mj.haigaiapp.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://vd.haigaiapp.cn

Ruby: warn "err"
来源：http://ls.huanxung.cn

C#:   Console.Error.WriteLine("err")
来源：http://is.colortex.cn

[M07] 判断是否为主入口
来源：http://ng.wgjwhj.cn

Py:   if __name__ == "__main__":
来源：http://ai.wgjwhj.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://lv.wgjwhj.cn

JS:   require.main === module
来源：http://fj.nszjky.cn

TS:   require.main === module
来源：http://xz.shxzukj.cn

Java: public static void main(String[] args)
来源：http://gt.asd995.cn

Go:   func main()
来源：http://qx.haigaiapp.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://np.colortex.cn

C#:   static void Main(string[] args)
来源：http://bm.panjiajie.cn

[M08] 获取系统与运行时信息
来源：http://cv.9csxet.cn

Py:   platform.system();  platform.python_version()
来源：http://ba.szsharing.cn

PHP:  PHP_OS;  phpversion();
来源：http://bj.nszjky.cn

JS:   process.platform;  process.version
来源：http://be.haigaiapp.cn

TS:   process.platform;  process.version
来源：http://od.bjjhwx.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://yj.yuntaijiaju.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://nf.shxzukj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ob.shxzukj.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://wb.muxihuayi.cn

================================================================================
来源：http://ud.shxzskj.cn

N. 数据结构与算法
来源：http://zm.panjiajie.cn

================================================================================
来源：http://ng.shxzskj.cn

[N01] 二分查找（有序数组）
来源：http://ca.yuexingan06.cn

Py:   bisect.bisect_left(arr, x)
来源：http://qs.huixinmuqiang.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://sg.szxytkj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dj.yuntaijiaju.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jq.huixiangedu.cn

Java: Arrays.binarySearch(arr, x)
来源：http://jk.asd995.cn

Go:   sort.SearchInts(arr, x)
来源：http://ge.asd995.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://xj.newstarts.cn

C#:   Array.BinarySearch(arr, x)
来源：http://gb.wgjwhj.cn

[N02] 排序（工程实践用内置实现）
来源：http://lv.panjiajie.cn

Py:   sorted(arr);  arr.sort()
来源：http://ow.huixiangedu.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://zp.shtwfgs.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://kw.nicolike.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://zo.shxzskj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://zy.shxzukj.cn

Go:   slices.Sort(arr)
来源：http://oh.nszjky.cn

Ruby: arr.sort
来源：http://ob.muxihuayi.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ap.wgjwhj.cn

[N03] 快速排序（分治示例）
来源：http://uf.huanxung.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://vg.9csxet.cn

PHP:  // 递归实现，或用 usort
来源：http://qr.szxytkj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lo.newstarts.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ai.panjiajie.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ug.jctech888.com.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://oz.jianghongdianzi.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://os.bookmarksfly.cn

C#:   // 手写递归，或 Array.Sort
来源：http://gq.hnjuh.cn

[N04] 斐波那契数列
来源：http://jn.huixiangedu.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://dl.huanxung.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ks.muxihuayi.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sm.huixiangedu.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ww.shtwfgs.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://jv.lnxyls.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://bg.szxytkj.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://rv.haigaiapp.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ws.yuexingan06.cn


<!-- 参考信息 -->