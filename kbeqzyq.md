代发 wailian999

[J07] 比较两个日期
来源：http://kd.asd995.cn

Py:   d1 < d2;  d1 == d2
来源：http://ns.gzmigu.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ry.521024.cn

JS:   d1.getTime() < d2.getTime()
来源：http://jg.muxihuayi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ou.yuntaijiaju.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mj.szsharing.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://rx.chemitech.net.cn

Ruby: d1 < d2;  d1 == d2
来源：http://iy.9csxet.cn

C#:   d1 < d2;  d1 == d2
来源：http://ph.huixiangedu.cn

[J08] 提取年月日与星期
来源：http://mo.jctech888.com.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://fg.muxihuayi.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ah.szxytkj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://tg.muxihuayi.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ta.huixiangedu.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://xa.shtwfgs.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://pl.bookmarksfly.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://tb.muxihuayi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://io.shtwfgs.cn

[J09] 时区处理
来源：http://ky.shxzukj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://nw.jctech888.com.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://kn.haigaiapp.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mh.panjiajie.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ea.panjiajie.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://db.lnxyls.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zq.bjjhwx.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://qs.bjjhwx.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://tp.haigaiapp.cn

[J10] 取今天 / 本月第一天
来源：http://xs.nszjky.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://nq.huixinmuqiang.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://vh.szsharing.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qo.haigaiapp.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://bs.colortex.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://eu.521024.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://cd.panjiajie.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://uc.chemitech.net.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://dz.jctech888.com.cn

================================================================================
来源：http://zd.muxihuayi.cn

K. JSON 与序列化
来源：http://tm.szxytkj.cn

================================================================================
来源：http://jo.9csxet.cn

[K01] 对象转 JSON 字符串
来源：http://mu.lnxyls.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ih.szxytkj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mb.wgjwhj.cn

JS:   JSON.stringify(obj)
来源：http://ab.haigaiapp.cn

TS:   JSON.stringify(obj)
来源：http://td.haigaiapp.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://gg.newstarts.cn

Go:   json.Marshal(obj)
来源：http://ij.521024.cn

Ruby: obj.to_json                                     // require "json"
来源：http://cp.shxzukj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://qo.panjiajie.cn

[K02] JSON 字符串转对象
来源：http://qf.hnjuh.cn

Py:   json.loads(s)
来源：http://ge.yuexingan06.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ku.newstarts.cn

JS:   JSON.parse(s)
来源：http://zz.newstarts.cn

TS:   JSON.parse(s)
来源：http://yr.hahajie.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jt.haigaiapp.cn

Go:   json.Unmarshal(data, &v)
来源：http://hg.wgjwhj.cn

Ruby: JSON.parse(s)
来源：http://yc.shxzskj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://fq.jianghongdianzi.cn

[K03] JSON 美化输出（带缩进）
来源：http://ev.jianghongdianzi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ly.bjjhwx.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hs.szxytkj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://xc.muxihuayi.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://gv.yuexingan06.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://bu.panjiajie.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://un.haigaiapp.cn

Ruby: JSON.pretty_generate(obj)
来源：http://cu.yuntaijiaju.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ul.lnxyls.cn

[K04] 读取 JSON 文件
来源：http://hp.chemitech.net.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://kv.nszjky.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://cv.gzmigu.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ud.hnjuh.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qx.shtwfgs.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://aq.newstarts.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://sr.huanxung.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ro.panjiajie.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://eo.huixinmuqiang.cn

[K05] 深拷贝对象
来源：http://sw.bjjhwx.cn

Py:   copy.deepcopy(obj)
来源：http://gg.hahajie.cn

PHP:  unserialize(serialize($obj));
来源：http://ms.nszjky.cn

JS:   structuredClone(obj)
来源：http://mu.521024.cn

TS:   structuredClone(obj)
来源：http://ar.nszjky.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ls.chemitech.net.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hu.szxytkj.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ij.hahajie.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://bi.chemitech.net.cn

[K06] 解析 URL 查询串
来源：http://rh.yuntaijiaju.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://yt.jianghongdianzi.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://kd.nicolike.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ww.nicolike.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://si.szsharing.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://un.colortex.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://cl.shxzukj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://su.muxihuayi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://xf.9csxet.cn

[K07] 进制转换
来源：http://pg.haigaiapp.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://sr.haigaiapp.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ok.newstarts.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://zr.newstarts.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hq.bookmarksfly.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://cf.yuexingan06.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://vy.shxzskj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://zs.huixiangedu.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://qs.shtwfgs.cn

[K08] 二进制序列化（非 JSON）
来源：http://tb.bjjhwx.cn

Py:   pickle.dumps(obj)
来源：http://dr.muxihuayi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://be.huixinmuqiang.cn

JS:   v8.serialize(obj)        // Node
来源：http://nu.huanxung.cn

TS:   v8.serialize(obj)        // Node
来源：http://zs.hahajie.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://gx.asd995.cn

Go:   encoding/gob
来源：http://ye.szsharing.cn

Ruby: Marshal.dump(obj)
来源：http://vf.gzmigu.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://rn.szxytkj.cn

================================================================================
来源：http://yk.colortex.cn

L. 网络请求
来源：http://uk.shtwfgs.cn

================================================================================
来源：http://ml.asd995.cn

[L01] 发送 GET 请求
来源：http://bt.521024.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://nz.huanxung.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://op.colortex.cn

JS:   await fetch(url)
来源：http://ri.muxihuayi.cn

TS:   await fetch(url)
来源：http://bt.szxytkj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://aa.yuexingan06.cn

Go:   resp, err := http.Get(url)
来源：http://wn.shxzukj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://oc.gzmigu.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://jf.muxihuayi.cn

[L02] 发送 POST JSON
来源：http://ej.shxzukj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://in.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://bl.szsharing.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ih.bjjhwx.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kg.haigaiapp.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ox.521024.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mx.asd995.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ou.newstarts.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://je.lnxyls.cn

[L03] 设置自定义请求头
来源：http://lu.yuexingan06.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ob.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://vg.asd995.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pg.jianghongdianzi.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tv.huixiangedu.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://go.lnxyls.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jj.panjiajie.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://cj.asd995.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://gp.colortex.cn

[L04] 设置超时
来源：http://wc.bookmarksfly.cn

Py:   requests.get(url, timeout=5)
来源：http://ff.shtwfgs.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://qf.muxihuayi.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kb.huixiangedu.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gb.colortex.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mr.521024.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fn.shxzskj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://et.jctech888.com.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ds.colortex.cn

[L05] 上传文件（multipart）
来源：http://fe.szxytkj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ee.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://tw.jianghongdianzi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://sx.haigaiapp.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://sf.huixiangedu.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vg.huixiangedu.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mm.521024.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://lb.muxihuayi.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://of.shtwfgs.cn

[L06] 解析响应为 JSON
来源：http://dx.nicolike.cn

Py:   resp.json()
来源：http://bf.muxihuayi.cn

PHP:  json_decode($body, true);
来源：http://gf.lnxyls.cn

JS:   await resp.json()
来源：http://kh.yuexingan06.cn

TS:   await resp.json()
来源：http://jm.yuexingan06.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ro.panjiajie.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://et.szsharing.cn

Ruby: JSON.parse(resp.body)
来源：http://tg.szsharing.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://fp.hnjuh.cn

[L07] 处理 HTTP 状态码
来源：http://dq.bookmarksfly.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://nk.hahajie.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://we.haigaiapp.cn

JS:   resp.ok;  resp.status
来源：http://ce.newstarts.cn

TS:   resp.ok;  resp.status
来源：http://kk.9csxet.cn

Java: resp.statusCode()
来源：http://lp.chemitech.net.cn

Go:   resp.StatusCode
来源：http://gn.asd995.cn

Ruby: resp.code.to_i
来源：http://ng.jianghongdianzi.cn

C#:   (int)resp.StatusCode
来源：http://zw.9csxet.cn

[L08] 并发请求多个地址
来源：http://ab.hahajie.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://qx.bjjhwx.cn

PHP:  curl_multi_init() 系列
来源：http://vm.bookmarksfly.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zx.chemitech.net.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://es.shtwfgs.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://fy.lnxyls.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ic.nszjky.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://qz.huixinmuqiang.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xs.shxzskj.cn

================================================================================
来源：http://wc.jianghongdianzi.cn

M. 命令行 / 进程 / 环境
来源：http://iy.shxzskj.cn

================================================================================
来源：http://bi.wgjwhj.cn

[M01] 读取命令行参数
来源：http://cz.asd995.cn

Py:   sys.argv[1:]
来源：http://ne.jctech888.com.cn

PHP:  $argv;  $argc;
来源：http://np.newstarts.cn

JS:   process.argv.slice(2)
来源：http://zb.gzmigu.cn

TS:   process.argv.slice(2)
来源：http://hf.asd995.cn

Java: args 数组（main 方法参数）
来源：http://on.panjiajie.cn

Go:   os.Args[1:]
来源：http://ni.yuntaijiaju.cn

Ruby: ARGV
来源：http://an.huixiangedu.cn

C#:   args 数组（Main 方法参数）
来源：http://ug.panjiajie.cn

[M02] 读取环境变量
来源：http://jq.szxytkj.cn

Py:   os.environ.get("HOME")
来源：http://mc.521024.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ty.jctech888.com.cn

JS:   process.env.HOME
来源：http://jp.huixinmuqiang.cn

TS:   process.env.HOME
来源：http://og.muxihuayi.cn

Java: System.getenv("HOME")
来源：http://tq.shxzukj.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://qd.shxzukj.cn

Ruby: ENV["HOME"]
来源：http://wj.chemitech.net.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://bl.szxytkj.cn

[M03] 执行外部命令
来源：http://jg.panjiajie.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://yy.panjiajie.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://sv.lnxyls.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://bg.bookmarksfly.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://pe.hahajie.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mm.chemitech.net.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://cu.yuntaijiaju.cn

Ruby: system("ls -l");  `ls -l`
来源：http://uu.huanxung.cn

C#:   Process.Start("ls", "-l");
来源：http://cc.haigaiapp.cn

[M04] 获取当前工作目录
来源：http://nu.shxzukj.cn

Py:   os.getcwd()
来源：http://qe.huixiangedu.cn

PHP:  getcwd();
来源：http://tu.hnjuh.cn

JS:   process.cwd()
来源：http://yv.colortex.cn

TS:   process.cwd()
来源：http://wu.gzmigu.cn

Java: Path.of("").toAbsolutePath()
来源：http://dy.wgjwhj.cn

Go:   os.Getwd()
来源：http://it.nszjky.cn

Ruby: Dir.pwd
来源：http://op.521024.cn

C#:   Directory.GetCurrentDirectory()
来源：http://xb.asd995.cn

[M05] 设置退出码
来源：http://nw.shxzukj.cn

Py:   sys.exit(1)
来源：http://mz.bookmarksfly.cn

PHP:  exit(1);
来源：http://hf.huanxung.cn

JS:   process.exit(1)
来源：http://rj.bjjhwx.cn

TS:   process.exit(1)
来源：http://pa.bookmarksfly.cn

Java: System.exit(1)
来源：http://wr.lnxyls.cn

Go:   os.Exit(1)
来源：http://uf.newstarts.cn

Ruby: exit 1
来源：http://tx.521024.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://lc.hahajie.cn

[M06] 向标准错误输出
来源：http://ch.bjjhwx.cn

Py:   print("err", file=sys.stderr)
来源：http://bu.wgjwhj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://va.huanxung.cn

JS:   console.error("err")
来源：http://st.huixiangedu.cn

TS:   console.error("err")
来源：http://vf.9csxet.cn

Java: System.err.println("err")
来源：http://bd.lnxyls.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://cc.9csxet.cn

Ruby: warn "err"
来源：http://jp.jianghongdianzi.cn

C#:   Console.Error.WriteLine("err")
来源：http://kx.newstarts.cn

[M07] 判断是否为主入口
来源：http://xd.shxzukj.cn

Py:   if __name__ == "__main__":
来源：http://tq.lnxyls.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://tf.wgjwhj.cn

JS:   require.main === module
来源：http://kl.lnxyls.cn

TS:   require.main === module
来源：http://gr.yuexingan06.cn

Java: public static void main(String[] args)
来源：http://zf.521024.cn

Go:   func main()
来源：http://kq.gzmigu.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://rc.huixinmuqiang.cn

C#:   static void Main(string[] args)
来源：http://kk.wgjwhj.cn

[M08] 获取系统与运行时信息
来源：http://cb.521024.cn

Py:   platform.system();  platform.python_version()
来源：http://ol.bookmarksfly.cn

PHP:  PHP_OS;  phpversion();
来源：http://ln.colortex.cn

JS:   process.platform;  process.version
来源：http://dv.huixinmuqiang.cn

TS:   process.platform;  process.version
来源：http://fq.newstarts.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://kc.nszjky.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://vp.521024.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ep.bookmarksfly.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://lh.huixiangedu.cn

================================================================================
来源：http://gm.hahajie.cn

N. 数据结构与算法
来源：http://ak.yuexingan06.cn

================================================================================
来源：http://ih.asd995.cn

[N01] 二分查找（有序数组）
来源：http://gm.nicolike.cn

Py:   bisect.bisect_left(arr, x)
来源：http://fh.521024.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ys.panjiajie.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ei.szsharing.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dn.jctech888.com.cn

Java: Arrays.binarySearch(arr, x)
来源：http://im.chemitech.net.cn

Go:   sort.SearchInts(arr, x)
来源：http://mm.nicolike.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ev.asd995.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ct.asd995.cn

[N02] 排序（工程实践用内置实现）
来源：http://ph.gzmigu.cn

Py:   sorted(arr);  arr.sort()
来源：http://dn.szxytkj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://gb.nszjky.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://de.nicolike.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://qr.asd995.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://pl.huixinmuqiang.cn

Go:   slices.Sort(arr)
来源：http://ne.yuexingan06.cn

Ruby: arr.sort
来源：http://bs.huixinmuqiang.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://es.huixiangedu.cn

[N03] 快速排序（分治示例）
来源：http://su.asd995.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://vn.yuntaijiaju.cn

PHP:  // 递归实现，或用 usort
来源：http://yy.chemitech.net.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lz.wgjwhj.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nu.lnxyls.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://fj.colortex.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ba.huixiangedu.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://bu.huanxung.cn

C#:   // 手写递归，或 Array.Sort
来源：http://zq.bjjhwx.cn

[N04] 斐波那契数列
来源：http://xr.haigaiapp.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://gr.nicolike.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://cn.bjjhwx.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jf.wgjwhj.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ep.newstarts.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ef.szsharing.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://nr.jianghongdianzi.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://iz.chemitech.net.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://do.szxytkj.cn


<!-- 参考信息 -->