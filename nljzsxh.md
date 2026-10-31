代发 wailian999

[J07] 比较两个日期
来源：http://dg.shxzukj.cn

Py:   d1 < d2;  d1 == d2
来源：http://fp.huixinmuqiang.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://si.shxzskj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://xi.yuexingan06.cn

TS:   d1.getTime() < d2.getTime()
来源：http://cm.nszjky.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://rr.wgjwhj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hv.huanxung.cn

Ruby: d1 < d2;  d1 == d2
来源：http://kt.nszjky.cn

C#:   d1 < d2;  d1 == d2
来源：http://qr.muxihuayi.cn

[J08] 提取年月日与星期
来源：http://ok.asd995.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ul.wgjwhj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://dn.jctech888.com.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://kt.yuntaijiaju.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://le.huixinmuqiang.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://as.panjiajie.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ai.huixinmuqiang.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://yy.nicolike.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://pd.yuntaijiaju.cn

[J09] 时区处理
来源：http://nt.szxytkj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hr.wgjwhj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://bg.nicolike.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ye.yuntaijiaju.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dz.hnjuh.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://rr.huixinmuqiang.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qe.nicolike.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://mw.panjiajie.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ew.colortex.cn

[J10] 取今天 / 本月第一天
来源：http://zx.yuntaijiaju.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ks.bjjhwx.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://cj.wgjwhj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://fm.9csxet.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ib.hahajie.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://tl.hnjuh.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ze.muxihuayi.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ix.shxzukj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://dg.9csxet.cn

================================================================================
来源：http://pd.szxytkj.cn

K. JSON 与序列化
来源：http://tz.bjjhwx.cn

================================================================================
来源：http://gp.yuntaijiaju.cn

[K01] 对象转 JSON 字符串
来源：http://md.chemitech.net.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://yv.shxzskj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://bj.colortex.cn

JS:   JSON.stringify(obj)
来源：http://pv.nszjky.cn

TS:   JSON.stringify(obj)
来源：http://xd.jianghongdianzi.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://sr.shtwfgs.cn

Go:   json.Marshal(obj)
来源：http://um.lnxyls.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ow.jianghongdianzi.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://xa.szxytkj.cn

[K02] JSON 字符串转对象
来源：http://tq.lnxyls.cn

Py:   json.loads(s)
来源：http://se.muxihuayi.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ez.hahajie.cn

JS:   JSON.parse(s)
来源：http://cs.shxzukj.cn

TS:   JSON.parse(s)
来源：http://kv.yuexingan06.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ch.lnxyls.cn

Go:   json.Unmarshal(data, &v)
来源：http://gb.9csxet.cn

Ruby: JSON.parse(s)
来源：http://wt.9csxet.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://vs.panjiajie.cn

[K03] JSON 美化输出（带缩进）
来源：http://ye.hahajie.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hm.nszjky.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://xr.newstarts.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ln.huanxung.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://sq.lnxyls.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://sd.lnxyls.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://fv.bookmarksfly.cn

Ruby: JSON.pretty_generate(obj)
来源：http://gu.521024.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://bb.521024.cn

[K04] 读取 JSON 文件
来源：http://qz.muxihuayi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ry.chemitech.net.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://bn.lnxyls.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rx.asd995.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fk.haigaiapp.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://rx.colortex.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hy.yuexingan06.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ya.shxzskj.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://bn.huanxung.cn

[K05] 深拷贝对象
来源：http://oq.huixiangedu.cn

Py:   copy.deepcopy(obj)
来源：http://ca.nszjky.cn

PHP:  unserialize(serialize($obj));
来源：http://gv.huixiangedu.cn

JS:   structuredClone(obj)
来源：http://xv.szsharing.cn

TS:   structuredClone(obj)
来源：http://kz.huanxung.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://nq.szxytkj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://cz.huanxung.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wk.asd995.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://fu.shxzukj.cn

[K06] 解析 URL 查询串
来源：http://zs.521024.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wg.nicolike.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://qx.9csxet.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kh.wgjwhj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://st.wgjwhj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://dp.nicolike.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ku.huixinmuqiang.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ea.chemitech.net.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://qc.hnjuh.cn

[K07] 进制转换
来源：http://ob.shtwfgs.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://gv.muxihuayi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ak.huixinmuqiang.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ku.huanxung.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ab.jianghongdianzi.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://fa.huixinmuqiang.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://fj.521024.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ah.shtwfgs.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://uk.asd995.cn

[K08] 二进制序列化（非 JSON）
来源：http://td.huixinmuqiang.cn

Py:   pickle.dumps(obj)
来源：http://ie.muxihuayi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ca.jctech888.com.cn

JS:   v8.serialize(obj)        // Node
来源：http://dz.huixinmuqiang.cn

TS:   v8.serialize(obj)        // Node
来源：http://qd.hnjuh.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://tm.9csxet.cn

Go:   encoding/gob
来源：http://op.asd995.cn

Ruby: Marshal.dump(obj)
来源：http://tz.jianghongdianzi.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://oe.hnjuh.cn

================================================================================
来源：http://mv.nszjky.cn

L. 网络请求
来源：http://nf.huixinmuqiang.cn

================================================================================
来源：http://cv.jianghongdianzi.cn

[L01] 发送 GET 请求
来源：http://pj.gzmigu.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://bu.9csxet.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vq.shxzskj.cn

JS:   await fetch(url)
来源：http://km.bjjhwx.cn

TS:   await fetch(url)
来源：http://eg.chemitech.net.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://eq.haigaiapp.cn

Go:   resp, err := http.Get(url)
来源：http://yc.bjjhwx.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://mj.shxzskj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://sd.szxytkj.cn

[L02] 发送 POST JSON
来源：http://zb.jctech888.com.cn

Py:   requests.post(url, json={"a": 1})
来源：http://pm.huixiangedu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ea.muxihuayi.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ti.huanxung.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wd.nszjky.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://jx.lnxyls.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://du.9csxet.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://na.nszjky.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://rk.hnjuh.cn

[L03] 设置自定义请求头
来源：http://xv.newstarts.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://xs.huixiangedu.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://bu.shxzskj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ro.hnjuh.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gq.bookmarksfly.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://qf.wgjwhj.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://sn.shxzskj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://gv.huixinmuqiang.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://vf.shxzukj.cn

[L04] 设置超时
来源：http://cd.shxzskj.cn

Py:   requests.get(url, timeout=5)
来源：http://bf.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ll.521024.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gi.yuntaijiaju.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tn.asd995.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://id.lnxyls.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ex.bookmarksfly.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://qj.haigaiapp.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mo.nszjky.cn

[L05] 上传文件（multipart）
来源：http://tr.bjjhwx.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://sm.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://es.nszjky.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://fx.nicolike.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://kj.shxzukj.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://pv.jianghongdianzi.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://zr.szsharing.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://fr.szsharing.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://nj.shxzskj.cn

[L06] 解析响应为 JSON
来源：http://fn.jianghongdianzi.cn

Py:   resp.json()
来源：http://yf.521024.cn

PHP:  json_decode($body, true);
来源：http://pk.szsharing.cn

JS:   await resp.json()
来源：http://bc.jianghongdianzi.cn

TS:   await resp.json()
来源：http://bp.gzmigu.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://nz.bjjhwx.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://nx.newstarts.cn

Ruby: JSON.parse(resp.body)
来源：http://ta.9csxet.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://oy.yuntaijiaju.cn

[L07] 处理 HTTP 状态码
来源：http://gm.wgjwhj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mm.jctech888.com.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ml.yuexingan06.cn

JS:   resp.ok;  resp.status
来源：http://tl.hahajie.cn

TS:   resp.ok;  resp.status
来源：http://jf.newstarts.cn

Java: resp.statusCode()
来源：http://fl.asd995.cn

Go:   resp.StatusCode
来源：http://sk.wgjwhj.cn

Ruby: resp.code.to_i
来源：http://zk.lnxyls.cn

C#:   (int)resp.StatusCode
来源：http://rl.haigaiapp.cn

[L08] 并发请求多个地址
来源：http://mb.jctech888.com.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://dr.yuexingan06.cn

PHP:  curl_multi_init() 系列
来源：http://tx.bjjhwx.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lb.nicolike.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://df.yuntaijiaju.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://sb.nszjky.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://bn.panjiajie.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wy.huixinmuqiang.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xx.huanxung.cn

================================================================================
来源：http://ll.521024.cn

M. 命令行 / 进程 / 环境
来源：http://oe.jianghongdianzi.cn

================================================================================
来源：http://qp.newstarts.cn

[M01] 读取命令行参数
来源：http://ve.huixiangedu.cn

Py:   sys.argv[1:]
来源：http://vd.shtwfgs.cn

PHP:  $argv;  $argc;
来源：http://mq.huixiangedu.cn

JS:   process.argv.slice(2)
来源：http://ye.szxytkj.cn

TS:   process.argv.slice(2)
来源：http://bz.haigaiapp.cn

Java: args 数组（main 方法参数）
来源：http://xc.nicolike.cn

Go:   os.Args[1:]
来源：http://tr.yuntaijiaju.cn

Ruby: ARGV
来源：http://fo.yuntaijiaju.cn

C#:   args 数组（Main 方法参数）
来源：http://xm.szxytkj.cn

[M02] 读取环境变量
来源：http://ne.newstarts.cn

Py:   os.environ.get("HOME")
来源：http://fi.shxzskj.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://sh.jctech888.com.cn

JS:   process.env.HOME
来源：http://ln.huixiangedu.cn

TS:   process.env.HOME
来源：http://hk.hahajie.cn

Java: System.getenv("HOME")
来源：http://wa.wgjwhj.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://fv.huanxung.cn

Ruby: ENV["HOME"]
来源：http://kr.huixinmuqiang.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://co.wgjwhj.cn

[M03] 执行外部命令
来源：http://sk.bookmarksfly.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://gr.panjiajie.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ph.hnjuh.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://me.huixinmuqiang.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://zr.yuexingan06.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://lp.haigaiapp.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://xx.colortex.cn

Ruby: system("ls -l");  `ls -l`
来源：http://nt.shxzukj.cn

C#:   Process.Start("ls", "-l");
来源：http://pk.wgjwhj.cn

[M04] 获取当前工作目录
来源：http://jj.yuntaijiaju.cn

Py:   os.getcwd()
来源：http://uz.chemitech.net.cn

PHP:  getcwd();
来源：http://wl.bjjhwx.cn

JS:   process.cwd()
来源：http://eq.shxzukj.cn

TS:   process.cwd()
来源：http://rf.huixiangedu.cn

Java: Path.of("").toAbsolutePath()
来源：http://qb.521024.cn

Go:   os.Getwd()
来源：http://xa.nicolike.cn

Ruby: Dir.pwd
来源：http://sf.jianghongdianzi.cn

C#:   Directory.GetCurrentDirectory()
来源：http://dt.hnjuh.cn

[M05] 设置退出码
来源：http://gq.hnjuh.cn

Py:   sys.exit(1)
来源：http://fi.nszjky.cn

PHP:  exit(1);
来源：http://et.chemitech.net.cn

JS:   process.exit(1)
来源：http://lw.muxihuayi.cn

TS:   process.exit(1)
来源：http://hm.huixiangedu.cn

Java: System.exit(1)
来源：http://kt.muxihuayi.cn

Go:   os.Exit(1)
来源：http://qx.hahajie.cn

Ruby: exit 1
来源：http://ua.yuexingan06.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ng.shtwfgs.cn

[M06] 向标准错误输出
来源：http://cd.shxzukj.cn

Py:   print("err", file=sys.stderr)
来源：http://rs.chemitech.net.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://hj.shtwfgs.cn

JS:   console.error("err")
来源：http://lw.huanxung.cn

TS:   console.error("err")
来源：http://wj.shxzukj.cn

Java: System.err.println("err")
来源：http://dm.shxzskj.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://of.9csxet.cn

Ruby: warn "err"
来源：http://vw.nicolike.cn

C#:   Console.Error.WriteLine("err")
来源：http://re.szxytkj.cn

[M07] 判断是否为主入口
来源：http://ri.newstarts.cn

Py:   if __name__ == "__main__":
来源：http://hr.panjiajie.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://rs.9csxet.cn

JS:   require.main === module
来源：http://sm.hnjuh.cn

TS:   require.main === module
来源：http://sv.shtwfgs.cn

Java: public static void main(String[] args)
来源：http://ue.hnjuh.cn

Go:   func main()
来源：http://fl.wgjwhj.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://jm.newstarts.cn

C#:   static void Main(string[] args)
来源：http://ub.9csxet.cn

[M08] 获取系统与运行时信息
来源：http://bt.szxytkj.cn

Py:   platform.system();  platform.python_version()
来源：http://un.gzmigu.cn

PHP:  PHP_OS;  phpversion();
来源：http://de.shtwfgs.cn

JS:   process.platform;  process.version
来源：http://ah.colortex.cn

TS:   process.platform;  process.version
来源：http://rc.haigaiapp.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://yj.521024.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://gb.haigaiapp.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://lo.szxytkj.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://zl.hahajie.cn

================================================================================
来源：http://jz.nszjky.cn

N. 数据结构与算法
来源：http://qx.szsharing.cn

================================================================================
来源：http://ke.panjiajie.cn

[N01] 二分查找（有序数组）
来源：http://qp.hnjuh.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ub.haigaiapp.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://sq.9csxet.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lm.haigaiapp.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kr.hahajie.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ob.yuntaijiaju.cn

Go:   sort.SearchInts(arr, x)
来源：http://vn.newstarts.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ip.yuexingan06.cn

C#:   Array.BinarySearch(arr, x)
来源：http://lk.szsharing.cn

[N02] 排序（工程实践用内置实现）
来源：http://bo.yuntaijiaju.cn

Py:   sorted(arr);  arr.sort()
来源：http://nd.huixinmuqiang.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://jw.asd995.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://qo.nszjky.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://tt.szsharing.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://pi.panjiajie.cn

Go:   slices.Sort(arr)
来源：http://wv.shxzskj.cn

Ruby: arr.sort
来源：http://yb.jianghongdianzi.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://cb.gzmigu.cn

[N03] 快速排序（分治示例）
来源：http://xx.jctech888.com.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ut.haigaiapp.cn

PHP:  // 递归实现，或用 usort
来源：http://ok.hahajie.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ck.wgjwhj.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://de.newstarts.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://de.yuntaijiaju.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://jz.muxihuayi.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://em.hahajie.cn

C#:   // 手写递归，或 Array.Sort
来源：http://hl.gzmigu.cn

[N04] 斐波那契数列
来源：http://rk.newstarts.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://co.panjiajie.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://lt.haigaiapp.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rf.huixiangedu.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gz.szsharing.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://qc.jctech888.com.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ic.szsharing.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ru.szxytkj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hi.colortex.cn


<!-- 参考信息 -->