代发 wailian999

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://xe.shtwfgs.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://aa.shxzskj.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bj.hnjuh.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://zo.chemitech.net.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://bu.shxzskj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://eb.szsharing.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wv.hnjuh.cn

[J10] 取今天 / 本月第一天
来源：http://mx.panjiajie.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://gg.bookmarksfly.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://nd.bookmarksfly.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://se.hnjuh.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ia.bjjhwx.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ut.wgjwhj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hi.nszjky.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://zs.521024.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://di.yuntaijiaju.cn

================================================================================
来源：http://lx.hnjuh.cn

K. JSON 与序列化
来源：http://xx.huixiangedu.cn

================================================================================
来源：http://zp.lnxyls.cn

[K01] 对象转 JSON 字符串
来源：http://ld.shtwfgs.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://gx.wgjwhj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://kf.yuexingan06.cn

JS:   JSON.stringify(obj)
来源：http://ny.yuntaijiaju.cn

TS:   JSON.stringify(obj)
来源：http://hi.wgjwhj.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://cf.jianghongdianzi.cn

Go:   json.Marshal(obj)
来源：http://hr.9csxet.cn

Ruby: obj.to_json                                     // require "json"
来源：http://yp.wgjwhj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ek.lnxyls.cn

[K02] JSON 字符串转对象
来源：http://lf.yuexingan06.cn

Py:   json.loads(s)
来源：http://gr.szxytkj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://gw.gzmigu.cn

JS:   JSON.parse(s)
来源：http://ts.jianghongdianzi.cn

TS:   JSON.parse(s)
来源：http://tu.yuexingan06.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ds.muxihuayi.cn

Go:   json.Unmarshal(data, &v)
来源：http://ws.shxzukj.cn

Ruby: JSON.parse(s)
来源：http://ni.shxzskj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://oa.shxzskj.cn

[K03] JSON 美化输出（带缩进）
来源：http://dd.shtwfgs.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://bb.panjiajie.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ys.huixinmuqiang.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ov.colortex.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://cx.shtwfgs.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://tf.panjiajie.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ck.9csxet.cn

Ruby: JSON.pretty_generate(obj)
来源：http://pg.chemitech.net.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://en.colortex.cn

[K04] 读取 JSON 文件
来源：http://ax.huanxung.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://vw.newstarts.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://so.yuntaijiaju.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hk.521024.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kx.asd995.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://lf.newstarts.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://yc.shxzskj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://og.asd995.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://fe.shxzukj.cn

[K05] 深拷贝对象
来源：http://fg.lnxyls.cn

Py:   copy.deepcopy(obj)
来源：http://yz.bjjhwx.cn

PHP:  unserialize(serialize($obj));
来源：http://lq.hnjuh.cn

JS:   structuredClone(obj)
来源：http://eh.yuexingan06.cn

TS:   structuredClone(obj)
来源：http://il.huanxung.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://uv.shxzskj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://en.wgjwhj.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://tw.521024.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://zd.nicolike.cn

[K06] 解析 URL 查询串
来源：http://pd.panjiajie.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://lp.huixiangedu.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zv.panjiajie.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lk.bookmarksfly.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xi.shxzukj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://rd.yuntaijiaju.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://wz.haigaiapp.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ds.szsharing.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wl.asd995.cn

[K07] 进制转换
来源：http://de.colortex.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://xg.nszjky.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://nr.huixiangedu.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://io.chemitech.net.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://gt.huanxung.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://au.asd995.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://yp.muxihuayi.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hl.huanxung.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ot.shxzukj.cn

[K08] 二进制序列化（非 JSON）
来源：http://yu.9csxet.cn

Py:   pickle.dumps(obj)
来源：http://pf.yuntaijiaju.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://gh.wgjwhj.cn

JS:   v8.serialize(obj)        // Node
来源：http://db.jctech888.com.cn

TS:   v8.serialize(obj)        // Node
来源：http://gw.hnjuh.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://yf.9csxet.cn

Go:   encoding/gob
来源：http://yu.colortex.cn

Ruby: Marshal.dump(obj)
来源：http://mf.hnjuh.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://sr.gzmigu.cn

================================================================================
来源：http://li.521024.cn

L. 网络请求
来源：http://ia.nicolike.cn

================================================================================
来源：http://zj.bookmarksfly.cn

[L01] 发送 GET 请求
来源：http://vc.gzmigu.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://oc.bookmarksfly.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://pq.haigaiapp.cn

JS:   await fetch(url)
来源：http://zu.nicolike.cn

TS:   await fetch(url)
来源：http://sh.szxytkj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ca.nszjky.cn

Go:   resp, err := http.Get(url)
来源：http://vf.9csxet.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://wk.lnxyls.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ya.9csxet.cn

[L02] 发送 POST JSON
来源：http://vr.huixinmuqiang.cn

Py:   requests.post(url, json={"a": 1})
来源：http://zo.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://yd.szxytkj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pi.newstarts.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ue.lnxyls.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://bi.hnjuh.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://dc.shxzukj.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://lo.chemitech.net.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://nf.szsharing.cn

[L03] 设置自定义请求头
来源：http://lu.nicolike.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://um.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://oc.muxihuayi.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fz.jctech888.com.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ut.newstarts.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://it.colortex.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://it.yuntaijiaju.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mq.huixinmuqiang.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://yk.shxzukj.cn

[L04] 设置超时
来源：http://tw.newstarts.cn

Py:   requests.get(url, timeout=5)
来源：http://oe.521024.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ia.hnjuh.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dz.huixiangedu.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ij.521024.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ci.nicolike.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ki.shxzukj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wz.shtwfgs.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://om.nicolike.cn

[L05] 上传文件（multipart）
来源：http://ot.hahajie.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ue.panjiajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://jd.colortex.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://xe.bookmarksfly.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ds.gzmigu.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://cq.haigaiapp.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://qp.shxzukj.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://cy.szxytkj.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://jp.jianghongdianzi.cn

[L06] 解析响应为 JSON
来源：http://gm.shxzskj.cn

Py:   resp.json()
来源：http://ep.colortex.cn

PHP:  json_decode($body, true);
来源：http://if.yuntaijiaju.cn

JS:   await resp.json()
来源：http://or.colortex.cn

TS:   await resp.json()
来源：http://xh.newstarts.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://jr.yuexingan06.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://io.panjiajie.cn

Ruby: JSON.parse(resp.body)
来源：http://tx.shtwfgs.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://nh.521024.cn

[L07] 处理 HTTP 状态码
来源：http://rx.yuexingan06.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://jq.bookmarksfly.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ax.jianghongdianzi.cn

JS:   resp.ok;  resp.status
来源：http://oj.bjjhwx.cn

TS:   resp.ok;  resp.status
来源：http://dg.jctech888.com.cn

Java: resp.statusCode()
来源：http://ep.chemitech.net.cn

Go:   resp.StatusCode
来源：http://vo.wgjwhj.cn

Ruby: resp.code.to_i
来源：http://my.nicolike.cn

C#:   (int)resp.StatusCode
来源：http://ac.shtwfgs.cn

[L08] 并发请求多个地址
来源：http://rk.bookmarksfly.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mi.szsharing.cn

PHP:  curl_multi_init() 系列
来源：http://dv.shxzskj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hi.jianghongdianzi.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gm.hahajie.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://rb.szsharing.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://fz.shtwfgs.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://yi.muxihuayi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ts.hahajie.cn

================================================================================
来源：http://tg.szxytkj.cn

M. 命令行 / 进程 / 环境
来源：http://nq.bjjhwx.cn

================================================================================
来源：http://mg.521024.cn

[M01] 读取命令行参数
来源：http://st.jctech888.com.cn

Py:   sys.argv[1:]
来源：http://ur.521024.cn

PHP:  $argv;  $argc;
来源：http://mr.colortex.cn

JS:   process.argv.slice(2)
来源：http://lb.wgjwhj.cn

TS:   process.argv.slice(2)
来源：http://ws.nicolike.cn

Java: args 数组（main 方法参数）
来源：http://lf.huixiangedu.cn

Go:   os.Args[1:]
来源：http://ym.nszjky.cn

Ruby: ARGV
来源：http://tu.huixinmuqiang.cn

C#:   args 数组（Main 方法参数）
来源：http://gf.colortex.cn

[M02] 读取环境变量
来源：http://on.jctech888.com.cn

Py:   os.environ.get("HOME")
来源：http://nf.jianghongdianzi.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ff.wgjwhj.cn

JS:   process.env.HOME
来源：http://lw.hnjuh.cn

TS:   process.env.HOME
来源：http://lt.nicolike.cn

Java: System.getenv("HOME")
来源：http://px.yuntaijiaju.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://os.shtwfgs.cn

Ruby: ENV["HOME"]
来源：http://fa.wgjwhj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ow.wgjwhj.cn

[M03] 执行外部命令
来源：http://tf.bjjhwx.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://yq.wgjwhj.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://xz.lnxyls.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://of.shxzukj.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://rq.hahajie.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://qk.shtwfgs.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ru.panjiajie.cn

Ruby: system("ls -l");  `ls -l`
来源：http://tn.muxihuayi.cn

C#:   Process.Start("ls", "-l");
来源：http://ey.haigaiapp.cn

[M04] 获取当前工作目录
来源：http://ms.jctech888.com.cn

Py:   os.getcwd()
来源：http://mc.bookmarksfly.cn

PHP:  getcwd();
来源：http://af.panjiajie.cn

JS:   process.cwd()
来源：http://sx.asd995.cn

TS:   process.cwd()
来源：http://em.colortex.cn

Java: Path.of("").toAbsolutePath()
来源：http://te.huanxung.cn

Go:   os.Getwd()
来源：http://uh.shtwfgs.cn

Ruby: Dir.pwd
来源：http://ov.haigaiapp.cn

C#:   Directory.GetCurrentDirectory()
来源：http://vn.521024.cn

[M05] 设置退出码
来源：http://io.shtwfgs.cn

Py:   sys.exit(1)
来源：http://ce.jianghongdianzi.cn

PHP:  exit(1);
来源：http://zm.bookmarksfly.cn

JS:   process.exit(1)
来源：http://gq.gzmigu.cn

TS:   process.exit(1)
来源：http://tr.nicolike.cn

Java: System.exit(1)
来源：http://dm.newstarts.cn

Go:   os.Exit(1)
来源：http://nm.huixiangedu.cn

Ruby: exit 1
来源：http://dv.yuntaijiaju.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wv.521024.cn

[M06] 向标准错误输出
来源：http://at.newstarts.cn

Py:   print("err", file=sys.stderr)
来源：http://po.521024.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://gd.shtwfgs.cn

JS:   console.error("err")
来源：http://gr.colortex.cn

TS:   console.error("err")
来源：http://lb.yuexingan06.cn

Java: System.err.println("err")
来源：http://rd.szsharing.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://zi.shxzskj.cn

Ruby: warn "err"
来源：http://cg.muxihuayi.cn

C#:   Console.Error.WriteLine("err")
来源：http://sr.szxytkj.cn

[M07] 判断是否为主入口
来源：http://do.521024.cn

Py:   if __name__ == "__main__":
来源：http://da.huixinmuqiang.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://dt.jianghongdianzi.cn

JS:   require.main === module
来源：http://vf.jianghongdianzi.cn

TS:   require.main === module
来源：http://wh.521024.cn

Java: public static void main(String[] args)
来源：http://wk.panjiajie.cn

Go:   func main()
来源：http://rc.panjiajie.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://om.9csxet.cn

C#:   static void Main(string[] args)
来源：http://wg.shxzskj.cn

[M08] 获取系统与运行时信息
来源：http://sv.bjjhwx.cn

Py:   platform.system();  platform.python_version()
来源：http://fx.hnjuh.cn

PHP:  PHP_OS;  phpversion();
来源：http://cb.colortex.cn

JS:   process.platform;  process.version
来源：http://cd.muxihuayi.cn

TS:   process.platform;  process.version
来源：http://bx.jianghongdianzi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ej.shtwfgs.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://rw.shxzskj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://eh.jctech888.com.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ne.hahajie.cn

================================================================================
来源：http://zf.yuexingan06.cn

N. 数据结构与算法
来源：http://kt.nicolike.cn

================================================================================
来源：http://xs.huanxung.cn

[N01] 二分查找（有序数组）
来源：http://bn.szsharing.cn

Py:   bisect.bisect_left(arr, x)
来源：http://di.jctech888.com.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://lw.jianghongdianzi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jr.szxytkj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nu.newstarts.cn

Java: Arrays.binarySearch(arr, x)
来源：http://fu.nszjky.cn

Go:   sort.SearchInts(arr, x)
来源：http://gm.huanxung.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://sa.haigaiapp.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ge.hnjuh.cn

[N02] 排序（工程实践用内置实现）
来源：http://qn.9csxet.cn

Py:   sorted(arr);  arr.sort()
来源：http://rw.lnxyls.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hw.panjiajie.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://aa.shxzukj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://vo.jctech888.com.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hw.szsharing.cn

Go:   slices.Sort(arr)
来源：http://it.colortex.cn

Ruby: arr.sort
来源：http://xe.panjiajie.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://oa.newstarts.cn

[N03] 快速排序（分治示例）
来源：http://nh.shtwfgs.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://pe.shxzskj.cn

PHP:  // 递归实现，或用 usort
来源：http://ll.asd995.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ye.chemitech.net.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ul.shxzukj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ej.jctech888.com.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://sp.nszjky.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://zk.521024.cn

C#:   // 手写递归，或 Array.Sort
来源：http://zr.bookmarksfly.cn

[N04] 斐波那契数列
来源：http://ma.panjiajie.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://kq.asd995.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://yn.asd995.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://py.chemitech.net.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hd.shtwfgs.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://du.nicolike.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hp.panjiajie.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ir.shtwfgs.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mt.jianghongdianzi.cn

[N05] 最大公约数
来源：http://lr.bjjhwx.cn

Py:   math.gcd(a, b)
来源：http://hw.wgjwhj.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://qo.bookmarksfly.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ve.521024.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xj.yuexingan06.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://sl.jctech888.com.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ji.huanxung.cn

Ruby: a.gcd(b)
来源：http://kt.haigaiapp.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://dw.asd995.cn

[N06] 判断回文字符串
来源：http://hm.szxytkj.cn

Py:   s == s[::-1]
来源：http://nb.huanxung.cn

PHP:  $s === strrev($s);
来源：http://wk.huixinmuqiang.cn

JS:   s === [...s].reverse().join("")
来源：http://uh.nszjky.cn

TS:   s === [...s].reverse().join("")
来源：http://jv.9csxet.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://uk.colortex.cn

Go:   // 双指针从两端比较
来源：http://sk.colortex.cn

Ruby: s == s.reverse
来源：http://xt.jianghongdianzi.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://vr.huixiangedu.cn

[N07] 两数之和（返回下标）
来源：http://jg.jianghongdianzi.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://tm.hahajie.cn


<!-- 参考信息 -->