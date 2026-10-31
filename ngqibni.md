代发 wailian999

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://pm.wgjwhj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fo.newstarts.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pv.nszjky.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://co.jianghongdianzi.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://yd.panjiajie.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://gq.nszjky.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ch.521024.cn

[J10] 取今天 / 本月第一天
来源：http://dk.wgjwhj.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://zf.nicolike.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mj.yuexingan06.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://up.521024.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://vx.asd995.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://bi.panjiajie.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://fh.gzmigu.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wh.jctech888.com.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://gw.nszjky.cn

================================================================================
来源：http://eg.521024.cn

K. JSON 与序列化
来源：http://qi.yuexingan06.cn

================================================================================
来源：http://by.hnjuh.cn

[K01] 对象转 JSON 字符串
来源：http://wt.yuntaijiaju.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://av.shxzskj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://gy.shxzukj.cn

JS:   JSON.stringify(obj)
来源：http://ma.9csxet.cn

TS:   JSON.stringify(obj)
来源：http://cf.lnxyls.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hn.yuntaijiaju.cn

Go:   json.Marshal(obj)
来源：http://nl.haigaiapp.cn

Ruby: obj.to_json                                     // require "json"
来源：http://kz.asd995.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://zd.newstarts.cn

[K02] JSON 字符串转对象
来源：http://of.huixiangedu.cn

Py:   json.loads(s)
来源：http://df.bjjhwx.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://vx.jctech888.com.cn

JS:   JSON.parse(s)
来源：http://ee.wgjwhj.cn

TS:   JSON.parse(s)
来源：http://fv.521024.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://fc.huanxung.cn

Go:   json.Unmarshal(data, &v)
来源：http://in.hnjuh.cn

Ruby: JSON.parse(s)
来源：http://wm.hahajie.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zh.huixiangedu.cn

[K03] JSON 美化输出（带缩进）
来源：http://ur.9csxet.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ar.jctech888.com.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://xj.panjiajie.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://vs.521024.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://pl.szxytkj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://zi.newstarts.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ik.wgjwhj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://hv.bookmarksfly.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://bt.chemitech.net.cn

[K04] 读取 JSON 文件
来源：http://ir.521024.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://kk.shxzukj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://gy.jctech888.com.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zw.shtwfgs.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yz.chemitech.net.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mc.szsharing.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://kz.lnxyls.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://bo.bjjhwx.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jf.nszjky.cn

[K05] 深拷贝对象
来源：http://ni.hnjuh.cn

Py:   copy.deepcopy(obj)
来源：http://jb.panjiajie.cn

PHP:  unserialize(serialize($obj));
来源：http://uz.muxihuayi.cn

JS:   structuredClone(obj)
来源：http://si.muxihuayi.cn

TS:   structuredClone(obj)
来源：http://oq.szxytkj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://mn.huanxung.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zu.huixiangedu.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://du.nszjky.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://sh.szxytkj.cn

[K06] 解析 URL 查询串
来源：http://jf.nicolike.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://th.gzmigu.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wr.bjjhwx.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://oj.szsharing.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xy.szsharing.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ja.nicolike.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://nb.bookmarksfly.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://sw.nszjky.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://gu.colortex.cn

[K07] 进制转换
来源：http://oj.huixinmuqiang.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://bz.asd995.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://jy.wgjwhj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://pz.panjiajie.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ni.szxytkj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://tt.521024.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://gw.huanxung.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://bv.hahajie.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://up.hnjuh.cn

[K08] 二进制序列化（非 JSON）
来源：http://kt.huixiangedu.cn

Py:   pickle.dumps(obj)
来源：http://xe.gzmigu.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ce.chemitech.net.cn

JS:   v8.serialize(obj)        // Node
来源：http://hh.521024.cn

TS:   v8.serialize(obj)        // Node
来源：http://wy.hahajie.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://vv.haigaiapp.cn

Go:   encoding/gob
来源：http://sg.nszjky.cn

Ruby: Marshal.dump(obj)
来源：http://uz.colortex.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ce.shxzskj.cn

================================================================================
来源：http://ue.wgjwhj.cn

L. 网络请求
来源：http://xg.shtwfgs.cn

================================================================================
来源：http://om.panjiajie.cn

[L01] 发送 GET 请求
来源：http://hi.nicolike.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://yg.bjjhwx.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://rf.9csxet.cn

JS:   await fetch(url)
来源：http://yv.gzmigu.cn

TS:   await fetch(url)
来源：http://jq.gzmigu.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ig.yuexingan06.cn

Go:   resp, err := http.Get(url)
来源：http://kl.hahajie.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://dr.gzmigu.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://vk.yuexingan06.cn

[L02] 发送 POST JSON
来源：http://bs.chemitech.net.cn

Py:   requests.post(url, json={"a": 1})
来源：http://fj.yuntaijiaju.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://uo.panjiajie.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xb.hahajie.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qo.lnxyls.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://td.shxzukj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ss.panjiajie.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://jp.huixinmuqiang.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ed.jianghongdianzi.cn

[L03] 设置自定义请求头
来源：http://qq.hnjuh.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hr.wgjwhj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://be.yuntaijiaju.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wc.muxihuayi.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cc.yuexingan06.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://qm.shtwfgs.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wu.huixinmuqiang.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://bs.szsharing.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://tl.asd995.cn

[L04] 设置超时
来源：http://oa.szxytkj.cn

Py:   requests.get(url, timeout=5)
来源：http://zn.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xu.colortex.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jh.nszjky.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ei.hahajie.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://jv.yuntaijiaju.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ya.521024.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://io.panjiajie.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://kk.bookmarksfly.cn

[L05] 上传文件（multipart）
来源：http://ar.colortex.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ns.wgjwhj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://du.newstarts.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ge.shxzukj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://zt.bookmarksfly.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://kg.chemitech.net.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://qj.huixiangedu.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ff.bookmarksfly.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ya.wgjwhj.cn

[L06] 解析响应为 JSON
来源：http://ol.colortex.cn

Py:   resp.json()
来源：http://vr.chemitech.net.cn

PHP:  json_decode($body, true);
来源：http://ne.shxzukj.cn

JS:   await resp.json()
来源：http://le.jctech888.com.cn

TS:   await resp.json()
来源：http://vz.huanxung.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://xa.muxihuayi.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://fi.nicolike.cn

Ruby: JSON.parse(resp.body)
来源：http://as.szsharing.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://qu.yuexingan06.cn

[L07] 处理 HTTP 状态码
来源：http://el.szxytkj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://td.521024.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://gm.9csxet.cn

JS:   resp.ok;  resp.status
来源：http://ss.chemitech.net.cn

TS:   resp.ok;  resp.status
来源：http://am.shxzukj.cn

Java: resp.statusCode()
来源：http://kf.muxihuayi.cn

Go:   resp.StatusCode
来源：http://le.huanxung.cn

Ruby: resp.code.to_i
来源：http://sw.jctech888.com.cn

C#:   (int)resp.StatusCode
来源：http://nk.chemitech.net.cn

[L08] 并发请求多个地址
来源：http://in.hahajie.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ds.jctech888.com.cn

PHP:  curl_multi_init() 系列
来源：http://hj.wgjwhj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tq.jctech888.com.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tl.9csxet.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://oa.hnjuh.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://zz.521024.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://cv.chemitech.net.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://oc.gzmigu.cn

================================================================================
来源：http://vs.colortex.cn

M. 命令行 / 进程 / 环境
来源：http://wm.shtwfgs.cn

================================================================================
来源：http://lu.newstarts.cn

[M01] 读取命令行参数
来源：http://oy.szxytkj.cn

Py:   sys.argv[1:]
来源：http://ip.gzmigu.cn

PHP:  $argv;  $argc;
来源：http://om.newstarts.cn

JS:   process.argv.slice(2)
来源：http://nb.shxzukj.cn

TS:   process.argv.slice(2)
来源：http://do.panjiajie.cn

Java: args 数组（main 方法参数）
来源：http://fx.huanxung.cn

Go:   os.Args[1:]
来源：http://el.huixiangedu.cn

Ruby: ARGV
来源：http://nu.bjjhwx.cn

C#:   args 数组（Main 方法参数）
来源：http://uu.shxzskj.cn

[M02] 读取环境变量
来源：http://zo.yuntaijiaju.cn

Py:   os.environ.get("HOME")
来源：http://fp.huanxung.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://qw.bjjhwx.cn

JS:   process.env.HOME
来源：http://ul.hnjuh.cn

TS:   process.env.HOME
来源：http://bp.wgjwhj.cn

Java: System.getenv("HOME")
来源：http://px.nicolike.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://rx.colortex.cn

Ruby: ENV["HOME"]
来源：http://xu.hahajie.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://si.521024.cn

[M03] 执行外部命令
来源：http://yh.newstarts.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://yn.shxzskj.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://rf.hnjuh.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://gy.nicolike.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://sc.shxzukj.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://fk.huixiangedu.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://gc.wgjwhj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://kq.gzmigu.cn

C#:   Process.Start("ls", "-l");
来源：http://wz.colortex.cn

[M04] 获取当前工作目录
来源：http://da.shtwfgs.cn

Py:   os.getcwd()
来源：http://kr.521024.cn

PHP:  getcwd();
来源：http://gx.hnjuh.cn

JS:   process.cwd()
来源：http://sq.521024.cn

TS:   process.cwd()
来源：http://fe.newstarts.cn

Java: Path.of("").toAbsolutePath()
来源：http://ty.shxzskj.cn

Go:   os.Getwd()
来源：http://zq.hahajie.cn

Ruby: Dir.pwd
来源：http://ju.yuexingan06.cn

C#:   Directory.GetCurrentDirectory()
来源：http://hx.szsharing.cn

[M05] 设置退出码
来源：http://kv.jianghongdianzi.cn

Py:   sys.exit(1)
来源：http://yp.shxzskj.cn

PHP:  exit(1);
来源：http://ad.newstarts.cn

JS:   process.exit(1)
来源：http://es.asd995.cn

TS:   process.exit(1)
来源：http://hp.panjiajie.cn

Java: System.exit(1)
来源：http://dp.huanxung.cn

Go:   os.Exit(1)
来源：http://hi.asd995.cn

Ruby: exit 1
来源：http://ho.yuexingan06.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://sp.szxytkj.cn

[M06] 向标准错误输出
来源：http://yi.wgjwhj.cn

Py:   print("err", file=sys.stderr)
来源：http://bb.shxzskj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ck.huixiangedu.cn

JS:   console.error("err")
来源：http://yg.bookmarksfly.cn

TS:   console.error("err")
来源：http://el.shtwfgs.cn

Java: System.err.println("err")
来源：http://tb.bookmarksfly.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ft.muxihuayi.cn

Ruby: warn "err"
来源：http://dg.gzmigu.cn

C#:   Console.Error.WriteLine("err")
来源：http://zy.gzmigu.cn

[M07] 判断是否为主入口
来源：http://xz.hnjuh.cn

Py:   if __name__ == "__main__":
来源：http://qn.jianghongdianzi.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://vs.huixinmuqiang.cn

JS:   require.main === module
来源：http://xg.szsharing.cn

TS:   require.main === module
来源：http://ej.jianghongdianzi.cn

Java: public static void main(String[] args)
来源：http://rb.szxytkj.cn

Go:   func main()
来源：http://eg.colortex.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://xo.huanxung.cn

C#:   static void Main(string[] args)
来源：http://kh.bookmarksfly.cn

[M08] 获取系统与运行时信息
来源：http://xa.muxihuayi.cn

Py:   platform.system();  platform.python_version()
来源：http://ss.bjjhwx.cn

PHP:  PHP_OS;  phpversion();
来源：http://uw.9csxet.cn

JS:   process.platform;  process.version
来源：http://xv.chemitech.net.cn

TS:   process.platform;  process.version
来源：http://or.chemitech.net.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://me.lnxyls.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://xg.bjjhwx.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://lu.521024.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://pq.9csxet.cn

================================================================================
来源：http://jp.huixiangedu.cn

N. 数据结构与算法
来源：http://iy.chemitech.net.cn

================================================================================
来源：http://wj.huixinmuqiang.cn

[N01] 二分查找（有序数组）
来源：http://xj.lnxyls.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ca.shtwfgs.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ru.asd995.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xx.huixiangedu.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://np.muxihuayi.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ut.521024.cn

Go:   sort.SearchInts(arr, x)
来源：http://vz.newstarts.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://sg.haigaiapp.cn

C#:   Array.BinarySearch(arr, x)
来源：http://mx.9csxet.cn

[N02] 排序（工程实践用内置实现）
来源：http://sz.yuntaijiaju.cn

Py:   sorted(arr);  arr.sort()
来源：http://jp.muxihuayi.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ge.huixiangedu.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://hw.huixiangedu.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://xi.521024.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://vq.muxihuayi.cn

Go:   slices.Sort(arr)
来源：http://wv.yuexingan06.cn

Ruby: arr.sort
来源：http://pf.newstarts.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://qp.bookmarksfly.cn

[N03] 快速排序（分治示例）
来源：http://qg.panjiajie.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://bo.bjjhwx.cn

PHP:  // 递归实现，或用 usort
来源：http://qj.hnjuh.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zr.panjiajie.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gd.yuntaijiaju.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wc.jianghongdianzi.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://tx.shxzskj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://uj.hahajie.cn

C#:   // 手写递归，或 Array.Sort
来源：http://fs.panjiajie.cn

[N04] 斐波那契数列
来源：http://th.bookmarksfly.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ld.asd995.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mf.huixinmuqiang.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ll.huanxung.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ui.jctech888.com.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://vn.bjjhwx.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mi.shxzukj.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mz.hahajie.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://yk.chemitech.net.cn

[N05] 最大公约数
来源：http://qa.szsharing.cn

Py:   math.gcd(a, b)
来源：http://fm.yuexingan06.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://tm.huanxung.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://eg.yuexingan06.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lc.jianghongdianzi.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ia.gzmigu.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://bh.nszjky.cn

Ruby: a.gcd(b)
来源：http://za.panjiajie.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://fz.bookmarksfly.cn

[N06] 判断回文字符串
来源：http://zt.newstarts.cn

Py:   s == s[::-1]
来源：http://cy.9csxet.cn

PHP:  $s === strrev($s);
来源：http://id.lnxyls.cn

JS:   s === [...s].reverse().join("")
来源：http://na.yuntaijiaju.cn

TS:   s === [...s].reverse().join("")
来源：http://or.shxzukj.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wv.hahajie.cn

Go:   // 双指针从两端比较
来源：http://uh.hahajie.cn

Ruby: s == s.reverse
来源：http://mw.szsharing.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://mg.chemitech.net.cn

[N07] 两数之和（返回下标）
来源：http://pq.szxytkj.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://is.jctech888.com.cn


<!-- 参考信息 -->