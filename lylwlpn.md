代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://fp.huixinmuqiang.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ge.shtwfgs.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qk.hnjuh.cn

[J10] 取今天 / 本月第一天
来源：http://pu.muxihuayi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://en.yuexingan06.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://gv.wgjwhj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://tp.colortex.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://eo.bjjhwx.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://uu.jctech888.com.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ft.9csxet.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://tw.yuexingan06.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://lm.wgjwhj.cn

================================================================================
来源：http://xr.huixinmuqiang.cn

K. JSON 与序列化
来源：http://kv.9csxet.cn

================================================================================
来源：http://ma.chemitech.net.cn

[K01] 对象转 JSON 字符串
来源：http://lf.shtwfgs.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ws.bookmarksfly.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://lf.asd995.cn

JS:   JSON.stringify(obj)
来源：http://ni.521024.cn

TS:   JSON.stringify(obj)
来源：http://hx.nicolike.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://bu.jctech888.com.cn

Go:   json.Marshal(obj)
来源：http://tz.newstarts.cn

Ruby: obj.to_json                                     // require "json"
来源：http://jq.wgjwhj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://qy.chemitech.net.cn

[K02] JSON 字符串转对象
来源：http://iz.hahajie.cn

Py:   json.loads(s)
来源：http://ai.hahajie.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hl.9csxet.cn

JS:   JSON.parse(s)
来源：http://iy.nicolike.cn

TS:   JSON.parse(s)
来源：http://tf.9csxet.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vw.yuntaijiaju.cn

Go:   json.Unmarshal(data, &v)
来源：http://fv.huixiangedu.cn

Ruby: JSON.parse(s)
来源：http://gg.szsharing.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://yh.521024.cn

[K03] JSON 美化输出（带缩进）
来源：http://cy.bookmarksfly.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://lv.wgjwhj.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://xi.shxzukj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ob.jctech888.com.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://cl.szsharing.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wv.newstarts.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://kl.wgjwhj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://wb.lnxyls.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ve.haigaiapp.cn

[K04] 读取 JSON 文件
来源：http://es.huixinmuqiang.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://et.huixinmuqiang.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://kh.asd995.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fv.szsharing.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://is.newstarts.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mc.panjiajie.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://kg.huixiangedu.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://an.chemitech.net.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ox.gzmigu.cn

[K05] 深拷贝对象
来源：http://ha.colortex.cn

Py:   copy.deepcopy(obj)
来源：http://ci.nszjky.cn

PHP:  unserialize(serialize($obj));
来源：http://io.hnjuh.cn

JS:   structuredClone(obj)
来源：http://vz.szsharing.cn

TS:   structuredClone(obj)
来源：http://hb.huixinmuqiang.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://te.huixinmuqiang.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://bp.gzmigu.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://gc.nszjky.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://nx.hahajie.cn

[K06] 解析 URL 查询串
来源：http://qd.bjjhwx.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wf.9csxet.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://si.hnjuh.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hm.haigaiapp.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pv.huixiangedu.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://va.shxzskj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://cx.chemitech.net.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://cy.newstarts.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mf.gzmigu.cn

[K07] 进制转换
来源：http://lo.shxzukj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ti.bookmarksfly.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://so.asd995.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ae.muxihuayi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://iu.haigaiapp.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ya.asd995.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://qf.muxihuayi.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://cq.asd995.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://xx.yuntaijiaju.cn

[K08] 二进制序列化（非 JSON）
来源：http://eu.haigaiapp.cn

Py:   pickle.dumps(obj)
来源：http://vc.hnjuh.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://gq.yuexingan06.cn

JS:   v8.serialize(obj)        // Node
来源：http://ny.521024.cn

TS:   v8.serialize(obj)        // Node
来源：http://iv.szsharing.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mw.szsharing.cn

Go:   encoding/gob
来源：http://cf.asd995.cn

Ruby: Marshal.dump(obj)
来源：http://lw.nicolike.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ma.wgjwhj.cn

================================================================================
来源：http://dl.bjjhwx.cn

L. 网络请求
来源：http://dg.lnxyls.cn

================================================================================
来源：http://em.yuexingan06.cn

[L01] 发送 GET 请求
来源：http://cy.szsharing.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://gr.yuexingan06.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://em.jianghongdianzi.cn

JS:   await fetch(url)
来源：http://ff.yuexingan06.cn

TS:   await fetch(url)
来源：http://ri.hnjuh.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ui.szsharing.cn

Go:   resp, err := http.Get(url)
来源：http://ov.huixiangedu.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://be.szxytkj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://al.jianghongdianzi.cn

[L02] 发送 POST JSON
来源：http://sy.newstarts.cn

Py:   requests.post(url, json={"a": 1})
来源：http://kp.521024.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hx.haigaiapp.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rf.panjiajie.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ns.huixiangedu.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://uc.panjiajie.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qi.newstarts.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://bx.newstarts.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xc.huixinmuqiang.cn

[L03] 设置自定义请求头
来源：http://eg.haigaiapp.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://af.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://yx.shtwfgs.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yi.hnjuh.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ik.shxzskj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://gv.huanxung.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://qw.gzmigu.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wf.haigaiapp.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://pd.yuntaijiaju.cn

[L04] 设置超时
来源：http://pc.nicolike.cn

Py:   requests.get(url, timeout=5)
来源：http://pi.nszjky.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://cy.jianghongdianzi.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vz.521024.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xm.szsharing.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://gk.bjjhwx.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://nb.jctech888.com.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://yl.haigaiapp.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://nq.bookmarksfly.cn

[L05] 上传文件（multipart）
来源：http://ln.huixinmuqiang.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://fg.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://tv.haigaiapp.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://en.wgjwhj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://qy.huixinmuqiang.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://oq.shtwfgs.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ha.yuexingan06.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://dl.nicolike.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ef.huixinmuqiang.cn

[L06] 解析响应为 JSON
来源：http://ew.bjjhwx.cn

Py:   resp.json()
来源：http://jr.huixiangedu.cn

PHP:  json_decode($body, true);
来源：http://fo.lnxyls.cn

JS:   await resp.json()
来源：http://ab.jianghongdianzi.cn

TS:   await resp.json()
来源：http://us.shxzskj.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://kb.asd995.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hy.wgjwhj.cn

Ruby: JSON.parse(resp.body)
来源：http://ts.9csxet.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ah.hnjuh.cn

[L07] 处理 HTTP 状态码
来源：http://aq.hnjuh.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ir.wgjwhj.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://jw.muxihuayi.cn

JS:   resp.ok;  resp.status
来源：http://cp.jianghongdianzi.cn

TS:   resp.ok;  resp.status
来源：http://pa.chemitech.net.cn

Java: resp.statusCode()
来源：http://qh.colortex.cn

Go:   resp.StatusCode
来源：http://ge.bookmarksfly.cn

Ruby: resp.code.to_i
来源：http://zk.asd995.cn

C#:   (int)resp.StatusCode
来源：http://wv.hahajie.cn

[L08] 并发请求多个地址
来源：http://iq.nszjky.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://cg.9csxet.cn

PHP:  curl_multi_init() 系列
来源：http://hl.jctech888.com.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tu.colortex.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zv.jctech888.com.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://lj.yuexingan06.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ca.huixinmuqiang.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://tk.chemitech.net.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://dk.huixinmuqiang.cn

================================================================================
来源：http://rk.bookmarksfly.cn

M. 命令行 / 进程 / 环境
来源：http://yi.chemitech.net.cn

================================================================================
来源：http://sz.gzmigu.cn

[M01] 读取命令行参数
来源：http://zk.shtwfgs.cn

Py:   sys.argv[1:]
来源：http://yl.huanxung.cn

PHP:  $argv;  $argc;
来源：http://re.shtwfgs.cn

JS:   process.argv.slice(2)
来源：http://va.jianghongdianzi.cn

TS:   process.argv.slice(2)
来源：http://ia.hnjuh.cn

Java: args 数组（main 方法参数）
来源：http://lq.9csxet.cn

Go:   os.Args[1:]
来源：http://ak.szxytkj.cn

Ruby: ARGV
来源：http://rc.bjjhwx.cn

C#:   args 数组（Main 方法参数）
来源：http://rp.hahajie.cn

[M02] 读取环境变量
来源：http://ya.hahajie.cn

Py:   os.environ.get("HOME")
来源：http://jp.huixinmuqiang.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ia.huanxung.cn

JS:   process.env.HOME
来源：http://mf.gzmigu.cn

TS:   process.env.HOME
来源：http://qh.newstarts.cn

Java: System.getenv("HOME")
来源：http://mq.chemitech.net.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://zs.shxzukj.cn

Ruby: ENV["HOME"]
来源：http://wn.shtwfgs.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://nh.shtwfgs.cn

[M03] 执行外部命令
来源：http://oh.shtwfgs.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hr.newstarts.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wd.nicolike.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://so.panjiajie.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://xb.shtwfgs.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://so.yuntaijiaju.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://am.panjiajie.cn

Ruby: system("ls -l");  `ls -l`
来源：http://nc.yuntaijiaju.cn

C#:   Process.Start("ls", "-l");
来源：http://am.jianghongdianzi.cn

[M04] 获取当前工作目录
来源：http://tu.shxzukj.cn

Py:   os.getcwd()
来源：http://mc.shtwfgs.cn

PHP:  getcwd();
来源：http://bs.shxzskj.cn

JS:   process.cwd()
来源：http://ru.jianghongdianzi.cn

TS:   process.cwd()
来源：http://ez.yuexingan06.cn

Java: Path.of("").toAbsolutePath()
来源：http://jw.huixiangedu.cn

Go:   os.Getwd()
来源：http://cp.9csxet.cn

Ruby: Dir.pwd
来源：http://tc.yuexingan06.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ik.yuntaijiaju.cn

[M05] 设置退出码
来源：http://xf.hnjuh.cn

Py:   sys.exit(1)
来源：http://rd.chemitech.net.cn

PHP:  exit(1);
来源：http://aa.lnxyls.cn

JS:   process.exit(1)
来源：http://yi.nicolike.cn

TS:   process.exit(1)
来源：http://hl.jctech888.com.cn

Java: System.exit(1)
来源：http://et.jctech888.com.cn

Go:   os.Exit(1)
来源：http://me.hnjuh.cn

Ruby: exit 1
来源：http://ul.newstarts.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wp.521024.cn

[M06] 向标准错误输出
来源：http://lq.yuntaijiaju.cn

Py:   print("err", file=sys.stderr)
来源：http://tw.yuexingan06.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ch.lnxyls.cn

JS:   console.error("err")
来源：http://rv.hahajie.cn

TS:   console.error("err")
来源：http://xj.szsharing.cn

Java: System.err.println("err")
来源：http://hd.lnxyls.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ms.huixiangedu.cn

Ruby: warn "err"
来源：http://zg.shxzukj.cn

C#:   Console.Error.WriteLine("err")
来源：http://vs.jctech888.com.cn

[M07] 判断是否为主入口
来源：http://os.jctech888.com.cn

Py:   if __name__ == "__main__":
来源：http://nw.asd995.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://dx.huixiangedu.cn

JS:   require.main === module
来源：http://dj.shxzukj.cn

TS:   require.main === module
来源：http://bc.szxytkj.cn

Java: public static void main(String[] args)
来源：http://wt.yuexingan06.cn

Go:   func main()
来源：http://bi.shtwfgs.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://qp.panjiajie.cn

C#:   static void Main(string[] args)
来源：http://nb.muxihuayi.cn

[M08] 获取系统与运行时信息
来源：http://uo.gzmigu.cn

Py:   platform.system();  platform.python_version()
来源：http://ke.asd995.cn

PHP:  PHP_OS;  phpversion();
来源：http://al.jianghongdianzi.cn

JS:   process.platform;  process.version
来源：http://gv.lnxyls.cn

TS:   process.platform;  process.version
来源：http://mx.bjjhwx.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ib.haigaiapp.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://kh.bjjhwx.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://pn.nicolike.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ev.huixiangedu.cn

================================================================================
来源：http://ri.huixiangedu.cn

N. 数据结构与算法
来源：http://hu.bjjhwx.cn

================================================================================
来源：http://eu.jianghongdianzi.cn

[N01] 二分查找（有序数组）
来源：http://fy.jianghongdianzi.cn

Py:   bisect.bisect_left(arr, x)
来源：http://zf.shtwfgs.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://nl.bookmarksfly.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zk.jctech888.com.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ct.lnxyls.cn

Java: Arrays.binarySearch(arr, x)
来源：http://pp.bjjhwx.cn

Go:   sort.SearchInts(arr, x)
来源：http://yl.shxzskj.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://vb.asd995.cn

C#:   Array.BinarySearch(arr, x)
来源：http://vl.szsharing.cn

[N02] 排序（工程实践用内置实现）
来源：http://su.colortex.cn

Py:   sorted(arr);  arr.sort()
来源：http://wx.panjiajie.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ps.haigaiapp.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://yj.gzmigu.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://mg.nszjky.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://is.hahajie.cn

Go:   slices.Sort(arr)
来源：http://ki.nicolike.cn

Ruby: arr.sort
来源：http://xu.bjjhwx.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ub.huixinmuqiang.cn

[N03] 快速排序（分治示例）
来源：http://sz.jctech888.com.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.asd995.cn

PHP:  // 递归实现，或用 usort
来源：http://pl.haigaiapp.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sz.bjjhwx.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hk.bjjhwx.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://bb.bookmarksfly.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://nt.colortex.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://uh.nicolike.cn

C#:   // 手写递归，或 Array.Sort
来源：http://jp.9csxet.cn

[N04] 斐波那契数列
来源：http://pj.jianghongdianzi.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zf.szsharing.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ow.jianghongdianzi.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rh.bjjhwx.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://eg.huixiangedu.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://xd.yuexingan06.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ec.lnxyls.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://tw.521024.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://am.bookmarksfly.cn

[N05] 最大公约数
来源：http://ks.muxihuayi.cn

Py:   math.gcd(a, b)
来源：http://om.shxzukj.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://gt.yuexingan06.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://iy.hahajie.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yg.asd995.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hb.yuexingan06.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ch.lnxyls.cn

Ruby: a.gcd(b)
来源：http://hx.hnjuh.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://fv.huixiangedu.cn

[N06] 判断回文字符串
来源：http://xd.haigaiapp.cn

Py:   s == s[::-1]
来源：http://qi.nicolike.cn

PHP:  $s === strrev($s);
来源：http://mr.hahajie.cn

JS:   s === [...s].reverse().join("")
来源：http://yp.yuexingan06.cn

TS:   s === [...s].reverse().join("")
来源：http://fq.hnjuh.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wg.shtwfgs.cn

Go:   // 双指针从两端比较
来源：http://yu.yuntaijiaju.cn

Ruby: s == s.reverse
来源：http://bb.huixinmuqiang.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://yu.haigaiapp.cn

[N07] 两数之和（返回下标）
来源：http://yq.shxzskj.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ic.muxihuayi.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ka.shxzukj.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://mb.huixiangedu.cn

TS:   // 手写 Map<string, number>
来源：http://nh.hahajie.cn

Java: // 手写 HashMap
来源：http://rs.hnjuh.cn


<!-- 参考信息 -->