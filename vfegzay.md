代发 wailian999

Java: Duration.between(start, end).toSeconds()
来源：http://rm.lnxyls.cn

Go:   end.Sub(start).Hours()
来源：http://qs.panjiajie.cn

Ruby: end - start                 # 返回秒数
来源：http://vj.gzmigu.cn

C#:   (end - start).TotalSeconds
来源：http://po.huixinmuqiang.cn

[J07] 比较两个日期
来源：http://se.huixinmuqiang.cn

Py:   d1 < d2;  d1 == d2
来源：http://br.chemitech.net.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://lw.haigaiapp.cn

JS:   d1.getTime() < d2.getTime()
来源：http://hb.shxzukj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://qz.panjiajie.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mo.wgjwhj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://gi.wgjwhj.cn

Ruby: d1 < d2;  d1 == d2
来源：http://gz.szxytkj.cn

C#:   d1 < d2;  d1 == d2
来源：http://or.szxytkj.cn

[J08] 提取年月日与星期
来源：http://cj.szsharing.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://rc.hahajie.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://vm.nicolike.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://sn.yuntaijiaju.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://lo.gzmigu.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://nm.bjjhwx.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://tj.huixinmuqiang.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://dy.szsharing.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ih.lnxyls.cn

[J09] 时区处理
来源：http://st.shxzukj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://jv.shxzukj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://du.szxytkj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vc.huixinmuqiang.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yz.haigaiapp.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://qk.lnxyls.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://no.yuexingan06.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://fm.yuntaijiaju.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://lv.chemitech.net.cn

[J10] 取今天 / 本月第一天
来源：http://kq.huixiangedu.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://vc.9csxet.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ql.shxzskj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://fa.panjiajie.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://sb.asd995.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ec.lnxyls.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://pi.haigaiapp.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://gi.chemitech.net.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://nf.huanxung.cn

================================================================================
来源：http://ii.asd995.cn

K. JSON 与序列化
来源：http://xk.bjjhwx.cn

================================================================================
来源：http://ts.9csxet.cn

[K01] 对象转 JSON 字符串
来源：http://rg.huanxung.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://uf.gzmigu.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://id.huixinmuqiang.cn

JS:   JSON.stringify(obj)
来源：http://yp.jianghongdianzi.cn

TS:   JSON.stringify(obj)
来源：http://pv.shtwfgs.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://yj.shxzukj.cn

Go:   json.Marshal(obj)
来源：http://bn.gzmigu.cn

Ruby: obj.to_json                                     // require "json"
来源：http://jy.9csxet.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://nw.bookmarksfly.cn

[K02] JSON 字符串转对象
来源：http://kt.9csxet.cn

Py:   json.loads(s)
来源：http://md.bjjhwx.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ww.shxzskj.cn

JS:   JSON.parse(s)
来源：http://kg.colortex.cn

TS:   JSON.parse(s)
来源：http://wy.yuexingan06.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jb.521024.cn

Go:   json.Unmarshal(data, &v)
来源：http://hw.panjiajie.cn

Ruby: JSON.parse(s)
来源：http://sl.nicolike.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://oi.szxytkj.cn

[K03] JSON 美化输出（带缩进）
来源：http://ii.huixinmuqiang.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://yw.panjiajie.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://lt.lnxyls.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://cw.nicolike.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://hf.gzmigu.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://it.shxzskj.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://kn.bjjhwx.cn

Ruby: JSON.pretty_generate(obj)
来源：http://yx.yuntaijiaju.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mn.bookmarksfly.cn

[K04] 读取 JSON 文件
来源：http://xh.shtwfgs.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://bk.521024.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://rv.huixinmuqiang.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://td.huixiangedu.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wi.521024.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://jm.9csxet.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ch.wgjwhj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://bf.jctech888.com.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://xq.huanxung.cn

[K05] 深拷贝对象
来源：http://tj.huanxung.cn

Py:   copy.deepcopy(obj)
来源：http://or.huixiangedu.cn

PHP:  unserialize(serialize($obj));
来源：http://op.wgjwhj.cn

JS:   structuredClone(obj)
来源：http://sn.gzmigu.cn

TS:   structuredClone(obj)
来源：http://ea.chemitech.net.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://sf.jianghongdianzi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://dt.nszjky.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://qh.huixiangedu.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://lz.jctech888.com.cn

[K06] 解析 URL 查询串
来源：http://my.wgjwhj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://bi.shxzukj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ng.szxytkj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://km.lnxyls.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yz.chemitech.net.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://qp.yuexingan06.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://if.haigaiapp.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://zd.shxzukj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ku.nszjky.cn

[K07] 进制转换
来源：http://bs.szxytkj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://qw.szxytkj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://py.shxzskj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wk.lnxyls.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://bs.hahajie.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://dk.muxihuayi.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://lz.gzmigu.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://op.haigaiapp.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ff.nicolike.cn

[K08] 二进制序列化（非 JSON）
来源：http://gs.panjiajie.cn

Py:   pickle.dumps(obj)
来源：http://kd.hnjuh.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://by.haigaiapp.cn

JS:   v8.serialize(obj)        // Node
来源：http://ow.shtwfgs.cn

TS:   v8.serialize(obj)        // Node
来源：http://vl.asd995.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://vc.huanxung.cn

Go:   encoding/gob
来源：http://in.szsharing.cn

Ruby: Marshal.dump(obj)
来源：http://wj.szsharing.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wm.gzmigu.cn

================================================================================
来源：http://kq.521024.cn

L. 网络请求
来源：http://qk.asd995.cn

================================================================================
来源：http://bi.szxytkj.cn

[L01] 发送 GET 请求
来源：http://nr.wgjwhj.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://uj.nicolike.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://gx.muxihuayi.cn

JS:   await fetch(url)
来源：http://gd.muxihuayi.cn

TS:   await fetch(url)
来源：http://cs.asd995.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://yu.hahajie.cn

Go:   resp, err := http.Get(url)
来源：http://ju.szxytkj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://tz.asd995.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://iz.bjjhwx.cn

[L02] 发送 POST JSON
来源：http://dj.chemitech.net.cn

Py:   requests.post(url, json={"a": 1})
来源：http://zr.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ge.muxihuayi.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lr.lnxyls.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tw.colortex.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://he.bjjhwx.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://br.gzmigu.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://kt.shxzukj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://zn.shxzskj.cn

[L03] 设置自定义请求头
来源：http://zy.shtwfgs.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://xa.521024.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mf.colortex.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://da.hahajie.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sz.gzmigu.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://dy.panjiajie.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://vi.haigaiapp.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qx.huixinmuqiang.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ns.9csxet.cn

[L04] 设置超时
来源：http://uz.muxihuayi.cn

Py:   requests.get(url, timeout=5)
来源：http://oq.haigaiapp.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wj.huixiangedu.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://od.huixiangedu.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ej.nicolike.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ol.bjjhwx.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://vq.huanxung.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hd.huixiangedu.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ax.hahajie.cn

[L05] 上传文件（multipart）
来源：http://vx.asd995.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://pe.521024.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ic.bjjhwx.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://dk.9csxet.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://on.wgjwhj.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://nl.szsharing.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://kb.newstarts.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://zp.huixinmuqiang.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://fw.haigaiapp.cn

[L06] 解析响应为 JSON
来源：http://rs.hnjuh.cn

Py:   resp.json()
来源：http://tt.chemitech.net.cn

PHP:  json_decode($body, true);
来源：http://ds.haigaiapp.cn

JS:   await resp.json()
来源：http://rd.521024.cn

TS:   await resp.json()
来源：http://if.521024.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://tr.panjiajie.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://xf.yuntaijiaju.cn

Ruby: JSON.parse(resp.body)
来源：http://wr.chemitech.net.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ih.huixinmuqiang.cn

[L07] 处理 HTTP 状态码
来源：http://xv.muxihuayi.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://uc.huixinmuqiang.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://kd.shxzskj.cn

JS:   resp.ok;  resp.status
来源：http://me.wgjwhj.cn

TS:   resp.ok;  resp.status
来源：http://qt.huixiangedu.cn

Java: resp.statusCode()
来源：http://si.shxzukj.cn

Go:   resp.StatusCode
来源：http://ct.bjjhwx.cn

Ruby: resp.code.to_i
来源：http://fq.szsharing.cn

C#:   (int)resp.StatusCode
来源：http://ci.shtwfgs.cn

[L08] 并发请求多个地址
来源：http://nx.gzmigu.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://af.yuexingan06.cn

PHP:  curl_multi_init() 系列
来源：http://pt.newstarts.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yf.yuexingan06.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fu.jctech888.com.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://rr.panjiajie.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ad.lnxyls.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ab.muxihuayi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ov.gzmigu.cn

================================================================================
来源：http://ze.huixiangedu.cn

M. 命令行 / 进程 / 环境
来源：http://js.newstarts.cn

================================================================================
来源：http://ug.muxihuayi.cn

[M01] 读取命令行参数
来源：http://in.nszjky.cn

Py:   sys.argv[1:]
来源：http://tm.huixiangedu.cn

PHP:  $argv;  $argc;
来源：http://hd.yuntaijiaju.cn

JS:   process.argv.slice(2)
来源：http://ca.szxytkj.cn

TS:   process.argv.slice(2)
来源：http://jj.huixinmuqiang.cn

Java: args 数组（main 方法参数）
来源：http://fh.asd995.cn

Go:   os.Args[1:]
来源：http://ha.shtwfgs.cn

Ruby: ARGV
来源：http://sy.chemitech.net.cn

C#:   args 数组（Main 方法参数）
来源：http://qy.chemitech.net.cn

[M02] 读取环境变量
来源：http://rt.colortex.cn

Py:   os.environ.get("HOME")
来源：http://pm.nicolike.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ur.shtwfgs.cn

JS:   process.env.HOME
来源：http://zv.hnjuh.cn

TS:   process.env.HOME
来源：http://gv.bookmarksfly.cn

Java: System.getenv("HOME")
来源：http://wy.521024.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://rf.huanxung.cn

Ruby: ENV["HOME"]
来源：http://kn.hahajie.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://qi.huanxung.cn

[M03] 执行外部命令
来源：http://pj.huixinmuqiang.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://qt.521024.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://vi.wgjwhj.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ra.yuexingan06.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://py.muxihuayi.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://vv.huixinmuqiang.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://jv.yuexingan06.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ca.panjiajie.cn

C#:   Process.Start("ls", "-l");
来源：http://mc.gzmigu.cn

[M04] 获取当前工作目录
来源：http://xu.huixinmuqiang.cn

Py:   os.getcwd()
来源：http://lo.521024.cn

PHP:  getcwd();
来源：http://wq.newstarts.cn

JS:   process.cwd()
来源：http://pf.yuntaijiaju.cn

TS:   process.cwd()
来源：http://nv.9csxet.cn

Java: Path.of("").toAbsolutePath()
来源：http://ex.jianghongdianzi.cn

Go:   os.Getwd()
来源：http://pn.chemitech.net.cn

Ruby: Dir.pwd
来源：http://iw.jctech888.com.cn

C#:   Directory.GetCurrentDirectory()
来源：http://hk.bjjhwx.cn

[M05] 设置退出码
来源：http://et.panjiajie.cn

Py:   sys.exit(1)
来源：http://yf.yuntaijiaju.cn

PHP:  exit(1);
来源：http://ky.lnxyls.cn

JS:   process.exit(1)
来源：http://qu.lnxyls.cn

TS:   process.exit(1)
来源：http://yk.9csxet.cn

Java: System.exit(1)
来源：http://or.huixiangedu.cn

Go:   os.Exit(1)
来源：http://ew.yuntaijiaju.cn

Ruby: exit 1
来源：http://qb.jctech888.com.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://tr.huixinmuqiang.cn

[M06] 向标准错误输出
来源：http://ii.hnjuh.cn

Py:   print("err", file=sys.stderr)
来源：http://oo.shxzskj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://zy.shtwfgs.cn

JS:   console.error("err")
来源：http://dk.jctech888.com.cn

TS:   console.error("err")
来源：http://mw.huixiangedu.cn

Java: System.err.println("err")
来源：http://eq.haigaiapp.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://gv.chemitech.net.cn

Ruby: warn "err"
来源：http://hg.shxzukj.cn

C#:   Console.Error.WriteLine("err")
来源：http://jk.9csxet.cn

[M07] 判断是否为主入口
来源：http://am.nicolike.cn

Py:   if __name__ == "__main__":
来源：http://sf.muxihuayi.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://jy.shtwfgs.cn

JS:   require.main === module
来源：http://ys.521024.cn

TS:   require.main === module
来源：http://ed.shtwfgs.cn

Java: public static void main(String[] args)
来源：http://ny.chemitech.net.cn

Go:   func main()
来源：http://tv.lnxyls.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://qf.szsharing.cn

C#:   static void Main(string[] args)
来源：http://ou.huixinmuqiang.cn

[M08] 获取系统与运行时信息
来源：http://qo.szxytkj.cn

Py:   platform.system();  platform.python_version()
来源：http://to.huixiangedu.cn

PHP:  PHP_OS;  phpversion();
来源：http://aw.yuntaijiaju.cn

JS:   process.platform;  process.version
来源：http://pg.asd995.cn

TS:   process.platform;  process.version
来源：http://lo.yuexingan06.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://eo.bjjhwx.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ja.nszjky.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://jz.gzmigu.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://gp.muxihuayi.cn

================================================================================
来源：http://qq.jianghongdianzi.cn

N. 数据结构与算法
来源：http://qg.chemitech.net.cn

================================================================================
来源：http://oc.chemitech.net.cn

[N01] 二分查找（有序数组）
来源：http://bw.huixiangedu.cn

Py:   bisect.bisect_left(arr, x)
来源：http://pz.lnxyls.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://pg.jianghongdianzi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ci.szxytkj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ad.newstarts.cn

Java: Arrays.binarySearch(arr, x)
来源：http://sx.shxzskj.cn

Go:   sort.SearchInts(arr, x)
来源：http://ax.shxzukj.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://kq.yuntaijiaju.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ib.shxzukj.cn

[N02] 排序（工程实践用内置实现）
来源：http://id.huanxung.cn

Py:   sorted(arr);  arr.sort()
来源：http://rf.szxytkj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://gi.szsharing.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://fb.9csxet.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://xj.bookmarksfly.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://nx.jctech888.com.cn

Go:   slices.Sort(arr)
来源：http://kl.gzmigu.cn

Ruby: arr.sort
来源：http://um.shxzskj.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://id.jianghongdianzi.cn

[N03] 快速排序（分治示例）
来源：http://fe.hahajie.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://nu.huanxung.cn

PHP:  // 递归实现，或用 usort
来源：http://xh.9csxet.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://va.bookmarksfly.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://db.huanxung.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://jf.yuntaijiaju.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://qx.panjiajie.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://jx.wgjwhj.cn

C#:   // 手写递归，或 Array.Sort
来源：http://hb.yuntaijiaju.cn

[N04] 斐波那契数列
来源：http://an.jianghongdianzi.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ns.hahajie.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wj.shxzukj.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ki.huixiangedu.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kr.asd995.cn


<!-- 参考信息 -->