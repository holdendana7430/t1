代发 wailian999

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hq.hnjuh.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rl.521024.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dj.lnxyls.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://fp.hnjuh.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://tz.huanxung.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://mu.jctech888.com.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://dd.hahajie.cn

[J10] 取今天 / 本月第一天
来源：http://th.shxzukj.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://xq.bookmarksfly.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ow.521024.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://lc.szxytkj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wz.9csxet.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://nm.shtwfgs.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://qs.panjiajie.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ig.nicolike.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ou.bjjhwx.cn

================================================================================
来源：http://va.haigaiapp.cn

K. JSON 与序列化
来源：http://vg.szxytkj.cn

================================================================================
来源：http://tq.muxihuayi.cn

[K01] 对象转 JSON 字符串
来源：http://bv.colortex.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://og.huixinmuqiang.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hh.colortex.cn

JS:   JSON.stringify(obj)
来源：http://nm.9csxet.cn

TS:   JSON.stringify(obj)
来源：http://hg.9csxet.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ea.bookmarksfly.cn

Go:   json.Marshal(obj)
来源：http://ic.wgjwhj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://uq.nicolike.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://am.bjjhwx.cn

[K02] JSON 字符串转对象
来源：http://wb.huixinmuqiang.cn

Py:   json.loads(s)
来源：http://ns.haigaiapp.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://xi.nicolike.cn

JS:   JSON.parse(s)
来源：http://cy.wgjwhj.cn

TS:   JSON.parse(s)
来源：http://wv.huixinmuqiang.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://tu.521024.cn

Go:   json.Unmarshal(data, &v)
来源：http://oq.newstarts.cn

Ruby: JSON.parse(s)
来源：http://im.bjjhwx.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://xo.jctech888.com.cn

[K03] JSON 美化输出（带缩进）
来源：http://gd.shtwfgs.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://my.muxihuayi.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://yt.nicolike.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://br.yuntaijiaju.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://bs.nicolike.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://jx.nicolike.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://lr.panjiajie.cn

Ruby: JSON.pretty_generate(obj)
来源：http://zg.lnxyls.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://nn.hahajie.cn

[K04] 读取 JSON 文件
来源：http://dn.muxihuayi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://xb.hahajie.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://vr.hahajie.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sf.huanxung.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://za.yuntaijiaju.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://zd.nszjky.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://cx.wgjwhj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://sn.yuexingan06.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://kl.nicolike.cn

[K05] 深拷贝对象
来源：http://yc.hnjuh.cn

Py:   copy.deepcopy(obj)
来源：http://ad.chemitech.net.cn

PHP:  unserialize(serialize($obj));
来源：http://zc.colortex.cn

JS:   structuredClone(obj)
来源：http://lc.nicolike.cn

TS:   structuredClone(obj)
来源：http://xo.shxzukj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://wm.shtwfgs.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://oy.newstarts.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://bz.wgjwhj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://am.haigaiapp.cn

[K06] 解析 URL 查询串
来源：http://kj.hnjuh.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hm.nicolike.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hm.wgjwhj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ky.newstarts.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yf.yuntaijiaju.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://rd.huixiangedu.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://sn.jianghongdianzi.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://oo.newstarts.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ug.nicolike.cn

[K07] 进制转换
来源：http://oa.szsharing.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ef.asd995.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://jg.chemitech.net.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ct.yuntaijiaju.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ah.huixiangedu.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://uk.nszjky.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://qx.nszjky.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://fz.yuntaijiaju.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://cw.gzmigu.cn

[K08] 二进制序列化（非 JSON）
来源：http://sy.521024.cn

Py:   pickle.dumps(obj)
来源：http://fp.521024.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://yr.panjiajie.cn

JS:   v8.serialize(obj)        // Node
来源：http://fv.szxytkj.cn

TS:   v8.serialize(obj)        // Node
来源：http://cv.hahajie.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mq.chemitech.net.cn

Go:   encoding/gob
来源：http://xy.haigaiapp.cn

Ruby: Marshal.dump(obj)
来源：http://nx.nszjky.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qy.huixinmuqiang.cn

================================================================================
来源：http://nf.9csxet.cn

L. 网络请求
来源：http://hg.bookmarksfly.cn

================================================================================
来源：http://sb.hnjuh.cn

[L01] 发送 GET 请求
来源：http://jw.9csxet.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jr.panjiajie.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://lu.hahajie.cn

JS:   await fetch(url)
来源：http://mj.jianghongdianzi.cn

TS:   await fetch(url)
来源：http://nj.yuntaijiaju.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://pz.jctech888.com.cn

Go:   resp, err := http.Get(url)
来源：http://bu.jianghongdianzi.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ta.shxzskj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://uh.asd995.cn

[L02] 发送 POST JSON
来源：http://py.muxihuayi.cn

Py:   requests.post(url, json={"a": 1})
来源：http://md.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://rp.szxytkj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ak.szxytkj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zs.yuexingan06.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://bn.shxzukj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://tm.panjiajie.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://gj.gzmigu.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://fo.nicolike.cn

[L03] 设置自定义请求头
来源：http://ta.haigaiapp.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://qh.huixiangedu.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hk.bjjhwx.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tr.nicolike.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ih.yuntaijiaju.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ux.chemitech.net.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ev.9csxet.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://tp.gzmigu.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://fp.huixinmuqiang.cn

[L04] 设置超时
来源：http://pl.huanxung.cn

Py:   requests.get(url, timeout=5)
来源：http://sy.szxytkj.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://zh.gzmigu.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nu.colortex.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ps.nicolike.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://zr.521024.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://nl.nicolike.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ml.hahajie.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ul.bookmarksfly.cn

[L05] 上传文件（multipart）
来源：http://xf.muxihuayi.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ax.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://fr.panjiajie.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://fm.shxzskj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://rj.lnxyls.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://fn.yuntaijiaju.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://au.shxzskj.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://jn.szsharing.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://bj.lnxyls.cn

[L06] 解析响应为 JSON
来源：http://he.jctech888.com.cn

Py:   resp.json()
来源：http://ze.lnxyls.cn

PHP:  json_decode($body, true);
来源：http://cn.lnxyls.cn

JS:   await resp.json()
来源：http://wn.muxihuayi.cn

TS:   await resp.json()
来源：http://nr.huixinmuqiang.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://rh.yuexingan06.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://xr.bookmarksfly.cn

Ruby: JSON.parse(resp.body)
来源：http://fk.shxzskj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ia.huixinmuqiang.cn

[L07] 处理 HTTP 状态码
来源：http://uu.bjjhwx.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://yd.colortex.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://nh.muxihuayi.cn

JS:   resp.ok;  resp.status
来源：http://jg.muxihuayi.cn

TS:   resp.ok;  resp.status
来源：http://pb.colortex.cn

Java: resp.statusCode()
来源：http://al.nszjky.cn

Go:   resp.StatusCode
来源：http://oo.colortex.cn

Ruby: resp.code.to_i
来源：http://zy.szsharing.cn

C#:   (int)resp.StatusCode
来源：http://wb.shtwfgs.cn

[L08] 并发请求多个地址
来源：http://xu.muxihuayi.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ab.colortex.cn

PHP:  curl_multi_init() 系列
来源：http://fz.haigaiapp.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hi.bookmarksfly.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kr.panjiajie.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://py.yuexingan06.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ai.yuntaijiaju.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://lj.shxzukj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://sf.wgjwhj.cn

================================================================================
来源：http://va.szsharing.cn

M. 命令行 / 进程 / 环境
来源：http://bm.nszjky.cn

================================================================================
来源：http://ul.szxytkj.cn

[M01] 读取命令行参数
来源：http://ut.yuexingan06.cn

Py:   sys.argv[1:]
来源：http://sv.haigaiapp.cn

PHP:  $argv;  $argc;
来源：http://fn.nicolike.cn

JS:   process.argv.slice(2)
来源：http://pk.huixinmuqiang.cn

TS:   process.argv.slice(2)
来源：http://aa.jianghongdianzi.cn

Java: args 数组（main 方法参数）
来源：http://bj.haigaiapp.cn

Go:   os.Args[1:]
来源：http://qc.hahajie.cn

Ruby: ARGV
来源：http://er.lnxyls.cn

C#:   args 数组（Main 方法参数）
来源：http://ub.bookmarksfly.cn

[M02] 读取环境变量
来源：http://hh.szxytkj.cn

Py:   os.environ.get("HOME")
来源：http://bi.yuexingan06.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://yw.jctech888.com.cn

JS:   process.env.HOME
来源：http://na.asd995.cn

TS:   process.env.HOME
来源：http://bk.haigaiapp.cn

Java: System.getenv("HOME")
来源：http://qn.huanxung.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://gw.panjiajie.cn

Ruby: ENV["HOME"]
来源：http://bd.huixiangedu.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://yu.521024.cn

[M03] 执行外部命令
来源：http://gn.szsharing.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://gv.shtwfgs.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://lx.huixinmuqiang.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://de.shxzskj.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ss.bjjhwx.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ug.panjiajie.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://qn.shxzskj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://fc.newstarts.cn

C#:   Process.Start("ls", "-l");
来源：http://oz.shtwfgs.cn

[M04] 获取当前工作目录
来源：http://yv.chemitech.net.cn

Py:   os.getcwd()
来源：http://ql.muxihuayi.cn

PHP:  getcwd();
来源：http://fd.yuexingan06.cn

JS:   process.cwd()
来源：http://ks.chemitech.net.cn

TS:   process.cwd()
来源：http://iw.haigaiapp.cn

Java: Path.of("").toAbsolutePath()
来源：http://km.huixiangedu.cn

Go:   os.Getwd()
来源：http://dc.gzmigu.cn

Ruby: Dir.pwd
来源：http://gc.shtwfgs.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ho.szxytkj.cn

[M05] 设置退出码
来源：http://ks.lnxyls.cn

Py:   sys.exit(1)
来源：http://zk.newstarts.cn

PHP:  exit(1);
来源：http://hl.shtwfgs.cn

JS:   process.exit(1)
来源：http://ts.shxzskj.cn

TS:   process.exit(1)
来源：http://hr.hahajie.cn

Java: System.exit(1)
来源：http://zk.colortex.cn

Go:   os.Exit(1)
来源：http://bs.shtwfgs.cn

Ruby: exit 1
来源：http://th.asd995.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mo.9csxet.cn

[M06] 向标准错误输出
来源：http://yj.newstarts.cn

Py:   print("err", file=sys.stderr)
来源：http://lb.yuexingan06.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://jk.huixiangedu.cn

JS:   console.error("err")
来源：http://bn.szxytkj.cn

TS:   console.error("err")
来源：http://lv.szxytkj.cn

Java: System.err.println("err")
来源：http://yw.bookmarksfly.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://fz.huixiangedu.cn

Ruby: warn "err"
来源：http://ze.szsharing.cn

C#:   Console.Error.WriteLine("err")
来源：http://uc.shxzskj.cn

[M07] 判断是否为主入口
来源：http://au.haigaiapp.cn

Py:   if __name__ == "__main__":
来源：http://hx.newstarts.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://oi.nicolike.cn

JS:   require.main === module
来源：http://oq.yuntaijiaju.cn

TS:   require.main === module
来源：http://fo.wgjwhj.cn

Java: public static void main(String[] args)
来源：http://aa.szxytkj.cn

Go:   func main()
来源：http://ly.nicolike.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://lt.asd995.cn

C#:   static void Main(string[] args)
来源：http://yl.huixiangedu.cn

[M08] 获取系统与运行时信息
来源：http://wh.hnjuh.cn

Py:   platform.system();  platform.python_version()
来源：http://az.nszjky.cn

PHP:  PHP_OS;  phpversion();
来源：http://qr.hnjuh.cn

JS:   process.platform;  process.version
来源：http://bv.521024.cn

TS:   process.platform;  process.version
来源：http://ca.jctech888.com.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ba.jctech888.com.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://hv.nszjky.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://fc.newstarts.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://db.yuntaijiaju.cn

================================================================================
来源：http://ak.521024.cn

N. 数据结构与算法
来源：http://gn.lnxyls.cn

================================================================================
来源：http://yy.huixiangedu.cn

[N01] 二分查找（有序数组）
来源：http://tr.521024.cn

Py:   bisect.bisect_left(arr, x)
来源：http://of.hahajie.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://yn.shxzukj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bk.panjiajie.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hw.huanxung.cn

Java: Arrays.binarySearch(arr, x)
来源：http://da.yuexingan06.cn

Go:   sort.SearchInts(arr, x)
来源：http://ve.huanxung.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://lh.huixiangedu.cn

C#:   Array.BinarySearch(arr, x)
来源：http://jy.jianghongdianzi.cn

[N02] 排序（工程实践用内置实现）
来源：http://wi.bookmarksfly.cn

Py:   sorted(arr);  arr.sort()
来源：http://kg.yuexingan06.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://vx.lnxyls.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ef.yuexingan06.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://od.jianghongdianzi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://lb.bookmarksfly.cn

Go:   slices.Sort(arr)
来源：http://re.hahajie.cn

Ruby: arr.sort
来源：http://kh.hahajie.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://pw.nicolike.cn

[N03] 快速排序（分治示例）
来源：http://xb.shtwfgs.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://am.szsharing.cn

PHP:  // 递归实现，或用 usort
来源：http://up.hahajie.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ha.521024.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fj.haigaiapp.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://pd.hnjuh.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://la.huixinmuqiang.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://fv.muxihuayi.cn

C#:   // 手写递归，或 Array.Sort
来源：http://qw.jctech888.com.cn

[N04] 斐波那契数列
来源：http://uh.haigaiapp.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://cs.colortex.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://kt.lnxyls.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://na.shxzskj.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ay.yuexingan06.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://kh.hnjuh.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://nt.muxihuayi.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://cf.shxzukj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://us.nicolike.cn

[N05] 最大公约数
来源：http://hy.haigaiapp.cn

Py:   math.gcd(a, b)
来源：http://ty.bjjhwx.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://fp.wgjwhj.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rn.nicolike.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dq.shxzskj.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://fl.shtwfgs.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wb.huanxung.cn

Ruby: a.gcd(b)
来源：http://oq.hnjuh.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://sr.colortex.cn

[N06] 判断回文字符串
来源：http://jb.szxytkj.cn

Py:   s == s[::-1]
来源：http://qg.chemitech.net.cn

PHP:  $s === strrev($s);
来源：http://rz.jctech888.com.cn

JS:   s === [...s].reverse().join("")
来源：http://rk.huixiangedu.cn

TS:   s === [...s].reverse().join("")
来源：http://lz.panjiajie.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://rk.asd995.cn

Go:   // 双指针从两端比较
来源：http://kq.shxzukj.cn

Ruby: s == s.reverse
来源：http://sb.huixiangedu.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://wb.muxihuayi.cn

[N07] 两数之和（返回下标）
来源：http://kj.shtwfgs.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://iq.wgjwhj.cn


<!-- 参考信息 -->