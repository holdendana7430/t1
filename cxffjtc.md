代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://id.huixinmuqiang.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://uj.9csxet.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://cj.jianghongdianzi.cn

[J10] 取今天 / 本月第一天
来源：http://fv.jianghongdianzi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ci.shxzukj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://kj.yuntaijiaju.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://jt.bjjhwx.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://pc.gzmigu.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://cp.bjjhwx.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://qv.lnxyls.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://pl.gzmigu.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hw.panjiajie.cn

================================================================================
来源：http://ew.lnxyls.cn

K. JSON 与序列化
来源：http://yg.huixiangedu.cn

================================================================================
来源：http://yl.colortex.cn

[K01] 对象转 JSON 字符串
来源：http://ij.yuexingan06.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://sz.yuntaijiaju.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://cz.jctech888.com.cn

JS:   JSON.stringify(obj)
来源：http://ku.asd995.cn

TS:   JSON.stringify(obj)
来源：http://bn.panjiajie.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://pa.jctech888.com.cn

Go:   json.Marshal(obj)
来源：http://vv.lnxyls.cn

Ruby: obj.to_json                                     // require "json"
来源：http://nr.asd995.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://nu.hnjuh.cn

[K02] JSON 字符串转对象
来源：http://fe.panjiajie.cn

Py:   json.loads(s)
来源：http://ok.szxytkj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wh.wgjwhj.cn

JS:   JSON.parse(s)
来源：http://uo.hahajie.cn

TS:   JSON.parse(s)
来源：http://aj.gzmigu.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wl.colortex.cn

Go:   json.Unmarshal(data, &v)
来源：http://wy.colortex.cn

Ruby: JSON.parse(s)
来源：http://sd.colortex.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hu.haigaiapp.cn

[K03] JSON 美化输出（带缩进）
来源：http://qs.lnxyls.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://my.nicolike.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wa.shxzskj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://fc.haigaiapp.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ae.9csxet.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://el.shtwfgs.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vy.jianghongdianzi.cn

Ruby: JSON.pretty_generate(obj)
来源：http://lq.9csxet.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://vn.nicolike.cn

[K04] 读取 JSON 文件
来源：http://ih.szxytkj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://dd.bjjhwx.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://dq.muxihuayi.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kz.shxzukj.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nv.haigaiapp.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://it.shxzskj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ge.huixinmuqiang.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://sz.asd995.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://tm.bjjhwx.cn

[K05] 深拷贝对象
来源：http://ju.521024.cn

Py:   copy.deepcopy(obj)
来源：http://kn.asd995.cn

PHP:  unserialize(serialize($obj));
来源：http://ia.9csxet.cn

JS:   structuredClone(obj)
来源：http://ee.haigaiapp.cn

TS:   structuredClone(obj)
来源：http://lu.colortex.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://is.jianghongdianzi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://re.bjjhwx.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wd.haigaiapp.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ej.yuntaijiaju.cn

[K06] 解析 URL 查询串
来源：http://xi.szsharing.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ht.shxzskj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ix.muxihuayi.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://eq.jianghongdianzi.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jp.chemitech.net.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hm.huixinmuqiang.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ge.szxytkj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vs.nszjky.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://yl.shtwfgs.cn

[K07] 进制转换
来源：http://yg.szsharing.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://nx.yuntaijiaju.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://fs.jctech888.com.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://vy.yuntaijiaju.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://jy.haigaiapp.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://go.szxytkj.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wb.huixinmuqiang.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://jy.muxihuayi.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ji.gzmigu.cn

[K08] 二进制序列化（非 JSON）
来源：http://iy.jctech888.com.cn

Py:   pickle.dumps(obj)
来源：http://sa.nicolike.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://qw.bookmarksfly.cn

JS:   v8.serialize(obj)        // Node
来源：http://fd.wgjwhj.cn

TS:   v8.serialize(obj)        // Node
来源：http://si.shxzukj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://pd.nszjky.cn

Go:   encoding/gob
来源：http://en.lnxyls.cn

Ruby: Marshal.dump(obj)
来源：http://ox.chemitech.net.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://gk.9csxet.cn

================================================================================
来源：http://hy.521024.cn

L. 网络请求
来源：http://zp.szsharing.cn

================================================================================
来源：http://uv.huixiangedu.cn

[L01] 发送 GET 请求
来源：http://nc.huixiangedu.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://sl.huixinmuqiang.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ov.hahajie.cn

JS:   await fetch(url)
来源：http://eb.521024.cn

TS:   await fetch(url)
来源：http://bz.colortex.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://bs.panjiajie.cn

Go:   resp, err := http.Get(url)
来源：http://vp.521024.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://fx.wgjwhj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://an.jctech888.com.cn

[L02] 发送 POST JSON
来源：http://eq.shxzukj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ue.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wq.colortex.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ar.chemitech.net.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bb.newstarts.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://cd.asd995.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jh.gzmigu.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://zz.hnjuh.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://oj.9csxet.cn

[L03] 设置自定义请求头
来源：http://jt.chemitech.net.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://sr.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://zl.asd995.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ji.muxihuayi.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://km.gzmigu.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wn.muxihuayi.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://xy.asd995.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ie.wgjwhj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hb.lnxyls.cn

[L04] 设置超时
来源：http://vy.bjjhwx.cn

Py:   requests.get(url, timeout=5)
来源：http://kr.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://gy.jianghongdianzi.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://in.yuntaijiaju.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pt.lnxyls.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://jg.wgjwhj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://pn.asd995.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://in.lnxyls.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ks.nicolike.cn

[L05] 上传文件（multipart）
来源：http://je.hahajie.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://yr.haigaiapp.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://vu.521024.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://su.521024.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://rn.huixiangedu.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ot.yuexingan06.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://rx.nicolike.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://sy.521024.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ht.huixiangedu.cn

[L06] 解析响应为 JSON
来源：http://jc.muxihuayi.cn

Py:   resp.json()
来源：http://zf.bjjhwx.cn

PHP:  json_decode($body, true);
来源：http://mu.huixiangedu.cn

JS:   await resp.json()
来源：http://pc.lnxyls.cn

TS:   await resp.json()
来源：http://wu.shxzukj.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ag.asd995.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://kp.gzmigu.cn

Ruby: JSON.parse(resp.body)
来源：http://ed.shxzskj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://qx.jianghongdianzi.cn

[L07] 处理 HTTP 状态码
来源：http://xb.colortex.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://qu.shxzskj.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://bb.shxzukj.cn

JS:   resp.ok;  resp.status
来源：http://tf.521024.cn

TS:   resp.ok;  resp.status
来源：http://pj.9csxet.cn

Java: resp.statusCode()
来源：http://vz.panjiajie.cn

Go:   resp.StatusCode
来源：http://nr.panjiajie.cn

Ruby: resp.code.to_i
来源：http://ds.nicolike.cn

C#:   (int)resp.StatusCode
来源：http://ef.jctech888.com.cn

[L08] 并发请求多个地址
来源：http://ra.bjjhwx.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ue.jctech888.com.cn

PHP:  curl_multi_init() 系列
来源：http://nq.521024.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fh.yuntaijiaju.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hu.hahajie.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mi.colortex.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://rv.panjiajie.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mc.haigaiapp.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ff.hnjuh.cn

================================================================================
来源：http://dh.newstarts.cn

M. 命令行 / 进程 / 环境
来源：http://tn.szsharing.cn

================================================================================
来源：http://dp.huanxung.cn

[M01] 读取命令行参数
来源：http://jx.yuntaijiaju.cn

Py:   sys.argv[1:]
来源：http://bp.huanxung.cn

PHP:  $argv;  $argc;
来源：http://zn.shxzskj.cn

JS:   process.argv.slice(2)
来源：http://ot.haigaiapp.cn

TS:   process.argv.slice(2)
来源：http://qm.nicolike.cn

Java: args 数组（main 方法参数）
来源：http://ru.colortex.cn

Go:   os.Args[1:]
来源：http://is.shxzskj.cn

Ruby: ARGV
来源：http://lh.9csxet.cn

C#:   args 数组（Main 方法参数）
来源：http://fo.huixinmuqiang.cn

[M02] 读取环境变量
来源：http://ov.huixiangedu.cn

Py:   os.environ.get("HOME")
来源：http://ei.newstarts.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://vr.wgjwhj.cn

JS:   process.env.HOME
来源：http://eo.jianghongdianzi.cn

TS:   process.env.HOME
来源：http://gz.chemitech.net.cn

Java: System.getenv("HOME")
来源：http://dx.huixiangedu.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ky.lnxyls.cn

Ruby: ENV["HOME"]
来源：http://ue.panjiajie.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://jv.yuexingan06.cn

[M03] 执行外部命令
来源：http://gq.lnxyls.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mf.yuntaijiaju.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://lf.wgjwhj.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://np.huixiangedu.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://lm.szsharing.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://vv.yuntaijiaju.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://lk.szsharing.cn

Ruby: system("ls -l");  `ls -l`
来源：http://tm.chemitech.net.cn

C#:   Process.Start("ls", "-l");
来源：http://jc.yuntaijiaju.cn

[M04] 获取当前工作目录
来源：http://xo.wgjwhj.cn

Py:   os.getcwd()
来源：http://vc.szxytkj.cn

PHP:  getcwd();
来源：http://oe.lnxyls.cn

JS:   process.cwd()
来源：http://uf.newstarts.cn

TS:   process.cwd()
来源：http://tw.yuntaijiaju.cn

Java: Path.of("").toAbsolutePath()
来源：http://iz.huixiangedu.cn

Go:   os.Getwd()
来源：http://xs.yuexingan06.cn

Ruby: Dir.pwd
来源：http://qm.jianghongdianzi.cn

C#:   Directory.GetCurrentDirectory()
来源：http://fs.panjiajie.cn

[M05] 设置退出码
来源：http://pv.newstarts.cn

Py:   sys.exit(1)
来源：http://kj.bjjhwx.cn

PHP:  exit(1);
来源：http://pv.hnjuh.cn

JS:   process.exit(1)
来源：http://eq.huixinmuqiang.cn

TS:   process.exit(1)
来源：http://qj.huixinmuqiang.cn

Java: System.exit(1)
来源：http://le.huanxung.cn

Go:   os.Exit(1)
来源：http://hk.lnxyls.cn

Ruby: exit 1
来源：http://xq.shxzukj.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://sj.gzmigu.cn

[M06] 向标准错误输出
来源：http://ju.hahajie.cn

Py:   print("err", file=sys.stderr)
来源：http://rx.haigaiapp.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://cv.huanxung.cn

JS:   console.error("err")
来源：http://ml.shtwfgs.cn

TS:   console.error("err")
来源：http://qu.nszjky.cn

Java: System.err.println("err")
来源：http://im.9csxet.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://jm.shxzskj.cn

Ruby: warn "err"
来源：http://tb.szxytkj.cn

C#:   Console.Error.WriteLine("err")
来源：http://gb.hahajie.cn

[M07] 判断是否为主入口
来源：http://vj.newstarts.cn

Py:   if __name__ == "__main__":
来源：http://ht.nicolike.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hw.yuexingan06.cn

JS:   require.main === module
来源：http://it.shxzskj.cn

TS:   require.main === module
来源：http://uw.lnxyls.cn

Java: public static void main(String[] args)
来源：http://en.bjjhwx.cn

Go:   func main()
来源：http://ta.yuexingan06.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://yh.wgjwhj.cn

C#:   static void Main(string[] args)
来源：http://ee.yuexingan06.cn

[M08] 获取系统与运行时信息
来源：http://cx.gzmigu.cn

Py:   platform.system();  platform.python_version()
来源：http://xk.yuntaijiaju.cn

PHP:  PHP_OS;  phpversion();
来源：http://zt.jianghongdianzi.cn

JS:   process.platform;  process.version
来源：http://qn.haigaiapp.cn

TS:   process.platform;  process.version
来源：http://es.bjjhwx.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://yq.huixinmuqiang.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://yi.jctech888.com.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://fr.lnxyls.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ps.shtwfgs.cn

================================================================================
来源：http://bx.yuexingan06.cn

N. 数据结构与算法
来源：http://ym.hahajie.cn

================================================================================
来源：http://fx.hahajie.cn

[N01] 二分查找（有序数组）
来源：http://rx.huanxung.cn

Py:   bisect.bisect_left(arr, x)
来源：http://nb.asd995.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://qg.521024.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cr.nicolike.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://uh.gzmigu.cn

Java: Arrays.binarySearch(arr, x)
来源：http://eg.nszjky.cn

Go:   sort.SearchInts(arr, x)
来源：http://va.nszjky.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://pw.yuexingan06.cn

C#:   Array.BinarySearch(arr, x)
来源：http://me.colortex.cn

[N02] 排序（工程实践用内置实现）
来源：http://gb.shtwfgs.cn

Py:   sorted(arr);  arr.sort()
来源：http://cx.9csxet.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://yx.521024.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://go.jianghongdianzi.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://nm.wgjwhj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://pv.huixinmuqiang.cn

Go:   slices.Sort(arr)
来源：http://zi.hnjuh.cn

Ruby: arr.sort
来源：http://cp.colortex.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://rn.hahajie.cn

[N03] 快速排序（分治示例）
来源：http://sd.gzmigu.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mi.yuntaijiaju.cn

PHP:  // 递归实现，或用 usort
来源：http://jd.huixiangedu.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sm.nicolike.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ou.huanxung.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://vd.asd995.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://py.chemitech.net.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://cp.bjjhwx.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ie.huanxung.cn

[N04] 斐波那契数列
来源：http://md.9csxet.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://md.huanxung.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://xo.colortex.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wc.yuntaijiaju.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vf.muxihuayi.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wj.jianghongdianzi.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://xz.newstarts.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://zh.panjiajie.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://jv.shxzukj.cn

[N05] 最大公约数
来源：http://xn.521024.cn

Py:   math.gcd(a, b)
来源：http://kl.bjjhwx.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://vt.huixinmuqiang.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xn.hahajie.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tq.panjiajie.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mp.jianghongdianzi.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ds.521024.cn

Ruby: a.gcd(b)
来源：http://lt.bjjhwx.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://vv.gzmigu.cn

[N06] 判断回文字符串
来源：http://fv.huanxung.cn

Py:   s == s[::-1]
来源：http://qq.bjjhwx.cn

PHP:  $s === strrev($s);
来源：http://jf.szsharing.cn

JS:   s === [...s].reverse().join("")
来源：http://oy.huanxung.cn

TS:   s === [...s].reverse().join("")
来源：http://zt.chemitech.net.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://gk.huixiangedu.cn

Go:   // 双指针从两端比较
来源：http://ek.wgjwhj.cn

Ruby: s == s.reverse
来源：http://sm.muxihuayi.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://oc.huixinmuqiang.cn

[N07] 两数之和（返回下标）
来源：http://xn.bjjhwx.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://gu.jctech888.com.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://sz.shxzskj.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://be.muxihuayi.cn

TS:   // 手写 Map<string, number>
来源：http://fl.hnjuh.cn

Java: // 手写 HashMap
来源：http://nc.yuexingan06.cn


<!-- 参考信息 -->