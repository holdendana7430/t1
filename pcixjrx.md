代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://js.chemitech.net.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://rs.jianghongdianzi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ua.nicolike.cn

[J10] 取今天 / 本月第一天
来源：http://ed.lnxyls.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://iz.bookmarksfly.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ib.yuntaijiaju.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://be.hnjuh.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://op.9csxet.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ep.shxzukj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ts.bookmarksfly.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://kk.newstarts.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://bq.shtwfgs.cn

================================================================================
来源：http://kr.bjjhwx.cn

K. JSON 与序列化
来源：http://ix.chemitech.net.cn

================================================================================
来源：http://wx.shxzskj.cn

[K01] 对象转 JSON 字符串
来源：http://lk.lnxyls.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://jh.panjiajie.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://fs.shxzukj.cn

JS:   JSON.stringify(obj)
来源：http://hl.huixiangedu.cn

TS:   JSON.stringify(obj)
来源：http://dc.bjjhwx.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hx.lnxyls.cn

Go:   json.Marshal(obj)
来源：http://ez.szsharing.cn

Ruby: obj.to_json                                     // require "json"
来源：http://cm.muxihuayi.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://lp.521024.cn

[K02] JSON 字符串转对象
来源：http://tf.huixiangedu.cn

Py:   json.loads(s)
来源：http://ka.shtwfgs.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ux.nszjky.cn

JS:   JSON.parse(s)
来源：http://uq.lnxyls.cn

TS:   JSON.parse(s)
来源：http://vv.9csxet.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://sg.colortex.cn

Go:   json.Unmarshal(data, &v)
来源：http://fi.szxytkj.cn

Ruby: JSON.parse(s)
来源：http://ou.shxzskj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://jo.shtwfgs.cn

[K03] JSON 美化输出（带缩进）
来源：http://jz.huixinmuqiang.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://us.asd995.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://zd.huanxung.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://vy.jctech888.com.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://fx.shxzukj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://be.chemitech.net.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://qm.yuntaijiaju.cn

Ruby: JSON.pretty_generate(obj)
来源：http://wf.nszjky.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://co.wgjwhj.cn

[K04] 读取 JSON 文件
来源：http://gn.bookmarksfly.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://vg.asd995.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ev.nszjky.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sb.9csxet.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://un.huixinmuqiang.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://uk.szxytkj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://tg.shtwfgs.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://sc.huixinmuqiang.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://nr.shxzskj.cn

[K05] 深拷贝对象
来源：http://aa.gzmigu.cn

Py:   copy.deepcopy(obj)
来源：http://lr.yuexingan06.cn

PHP:  unserialize(serialize($obj));
来源：http://kf.muxihuayi.cn

JS:   structuredClone(obj)
来源：http://wu.huixinmuqiang.cn

TS:   structuredClone(obj)
来源：http://sq.szxytkj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://zl.shxzskj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://of.szsharing.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://kz.huixinmuqiang.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://dx.huixinmuqiang.cn

[K06] 解析 URL 查询串
来源：http://uz.shtwfgs.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ik.huanxung.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://no.yuntaijiaju.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jn.nicolike.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ib.szxytkj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://eg.asd995.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://mq.chemitech.net.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://bn.huixiangedu.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ql.shxzskj.cn

[K07] 进制转换
来源：http://cd.yuexingan06.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://sn.huanxung.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wv.szxytkj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ld.9csxet.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://bo.huixiangedu.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://cb.9csxet.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://yv.huanxung.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ku.9csxet.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://oe.haigaiapp.cn

[K08] 二进制序列化（非 JSON）
来源：http://ls.bookmarksfly.cn

Py:   pickle.dumps(obj)
来源：http://yt.szxytkj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://qk.yuexingan06.cn

JS:   v8.serialize(obj)        // Node
来源：http://qe.chemitech.net.cn

TS:   v8.serialize(obj)        // Node
来源：http://eg.szsharing.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://gh.nszjky.cn

Go:   encoding/gob
来源：http://bi.huanxung.cn

Ruby: Marshal.dump(obj)
来源：http://in.bjjhwx.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qp.521024.cn

================================================================================
来源：http://pd.jctech888.com.cn

L. 网络请求
来源：http://nu.asd995.cn

================================================================================
来源：http://hl.9csxet.cn

[L01] 发送 GET 请求
来源：http://pn.wgjwhj.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://no.yuexingan06.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://al.shxzskj.cn

JS:   await fetch(url)
来源：http://lc.huixiangedu.cn

TS:   await fetch(url)
来源：http://ad.wgjwhj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ep.panjiajie.cn

Go:   resp, err := http.Get(url)
来源：http://ao.huixiangedu.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://kx.shxzskj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ic.huixiangedu.cn

[L02] 发送 POST JSON
来源：http://pb.bookmarksfly.cn

Py:   requests.post(url, json={"a": 1})
来源：http://hh.panjiajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://fp.nszjky.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ue.lnxyls.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tq.9csxet.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://gl.wgjwhj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jj.asd995.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://sc.muxihuayi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://vl.nicolike.cn

[L03] 设置自定义请求头
来源：http://bg.wgjwhj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://sg.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://nj.szxytkj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hu.nicolike.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://el.muxihuayi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://yr.asd995.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://pb.szxytkj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ql.jianghongdianzi.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ox.hahajie.cn

[L04] 设置超时
来源：http://op.gzmigu.cn

Py:   requests.get(url, timeout=5)
来源：http://zi.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ma.hahajie.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ge.hahajie.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ez.chemitech.net.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://aq.huixinmuqiang.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://sl.gzmigu.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://cw.shtwfgs.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://rj.lnxyls.cn

[L05] 上传文件（multipart）
来源：http://vo.yuexingan06.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ht.szsharing.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://xs.521024.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ci.huixinmuqiang.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://td.newstarts.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://aw.huixiangedu.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://vz.haigaiapp.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ec.bjjhwx.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://im.nicolike.cn

[L06] 解析响应为 JSON
来源：http://lo.9csxet.cn

Py:   resp.json()
来源：http://al.9csxet.cn

PHP:  json_decode($body, true);
来源：http://np.bookmarksfly.cn

JS:   await resp.json()
来源：http://rl.huanxung.cn

TS:   await resp.json()
来源：http://ez.521024.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://pe.jianghongdianzi.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://aq.newstarts.cn

Ruby: JSON.parse(resp.body)
来源：http://bz.521024.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://yk.nicolike.cn

[L07] 处理 HTTP 状态码
来源：http://iy.yuntaijiaju.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://jw.wgjwhj.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://tf.hnjuh.cn

JS:   resp.ok;  resp.status
来源：http://qs.wgjwhj.cn

TS:   resp.ok;  resp.status
来源：http://rp.szxytkj.cn

Java: resp.statusCode()
来源：http://os.szxytkj.cn

Go:   resp.StatusCode
来源：http://ql.wgjwhj.cn

Ruby: resp.code.to_i
来源：http://qg.lnxyls.cn

C#:   (int)resp.StatusCode
来源：http://ht.wgjwhj.cn

[L08] 并发请求多个地址
来源：http://ut.nicolike.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mi.huixiangedu.cn

PHP:  curl_multi_init() 系列
来源：http://va.nicolike.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cf.jctech888.com.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gc.panjiajie.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wx.haigaiapp.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://nl.shtwfgs.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://bd.nszjky.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://qp.huixiangedu.cn

================================================================================
来源：http://ed.hnjuh.cn

M. 命令行 / 进程 / 环境
来源：http://it.lnxyls.cn

================================================================================
来源：http://oe.panjiajie.cn

[M01] 读取命令行参数
来源：http://kc.bjjhwx.cn

Py:   sys.argv[1:]
来源：http://cx.hahajie.cn

PHP:  $argv;  $argc;
来源：http://uz.newstarts.cn

JS:   process.argv.slice(2)
来源：http://ud.wgjwhj.cn

TS:   process.argv.slice(2)
来源：http://xf.bookmarksfly.cn

Java: args 数组（main 方法参数）
来源：http://qc.9csxet.cn

Go:   os.Args[1:]
来源：http://yk.huixiangedu.cn

Ruby: ARGV
来源：http://iu.lnxyls.cn

C#:   args 数组（Main 方法参数）
来源：http://ha.9csxet.cn

[M02] 读取环境变量
来源：http://jf.yuexingan06.cn

Py:   os.environ.get("HOME")
来源：http://yq.shxzskj.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://fg.jctech888.com.cn

JS:   process.env.HOME
来源：http://ei.bjjhwx.cn

TS:   process.env.HOME
来源：http://io.bjjhwx.cn

Java: System.getenv("HOME")
来源：http://yf.shtwfgs.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ft.shtwfgs.cn

Ruby: ENV["HOME"]
来源：http://pw.shtwfgs.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://oq.bookmarksfly.cn

[M03] 执行外部命令
来源：http://bc.lnxyls.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ag.gzmigu.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://gl.gzmigu.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://kf.shtwfgs.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://hi.huixinmuqiang.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ho.jctech888.com.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://cl.huixiangedu.cn

Ruby: system("ls -l");  `ls -l`
来源：http://go.nicolike.cn

C#:   Process.Start("ls", "-l");
来源：http://sy.jianghongdianzi.cn

[M04] 获取当前工作目录
来源：http://ip.szsharing.cn

Py:   os.getcwd()
来源：http://bn.haigaiapp.cn

PHP:  getcwd();
来源：http://vz.hahajie.cn

JS:   process.cwd()
来源：http://yl.shtwfgs.cn

TS:   process.cwd()
来源：http://sh.shtwfgs.cn

Java: Path.of("").toAbsolutePath()
来源：http://ei.shtwfgs.cn

Go:   os.Getwd()
来源：http://gg.nicolike.cn

Ruby: Dir.pwd
来源：http://gi.nszjky.cn

C#:   Directory.GetCurrentDirectory()
来源：http://db.9csxet.cn

[M05] 设置退出码
来源：http://sw.haigaiapp.cn

Py:   sys.exit(1)
来源：http://vn.wgjwhj.cn

PHP:  exit(1);
来源：http://md.nszjky.cn

JS:   process.exit(1)
来源：http://bl.huixiangedu.cn

TS:   process.exit(1)
来源：http://ba.muxihuayi.cn

Java: System.exit(1)
来源：http://fj.wgjwhj.cn

Go:   os.Exit(1)
来源：http://op.wgjwhj.cn

Ruby: exit 1
来源：http://el.szsharing.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://xs.huixiangedu.cn

[M06] 向标准错误输出
来源：http://pl.jctech888.com.cn

Py:   print("err", file=sys.stderr)
来源：http://wo.hahajie.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://qo.jctech888.com.cn

JS:   console.error("err")
来源：http://iq.shtwfgs.cn

TS:   console.error("err")
来源：http://bs.shxzukj.cn

Java: System.err.println("err")
来源：http://gc.shxzskj.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ho.huanxung.cn

Ruby: warn "err"
来源：http://sp.muxihuayi.cn

C#:   Console.Error.WriteLine("err")
来源：http://my.shxzukj.cn

[M07] 判断是否为主入口
来源：http://qh.jctech888.com.cn

Py:   if __name__ == "__main__":
来源：http://js.huixiangedu.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://yf.newstarts.cn

JS:   require.main === module
来源：http://kn.colortex.cn

TS:   require.main === module
来源：http://mj.hahajie.cn

Java: public static void main(String[] args)
来源：http://ie.chemitech.net.cn

Go:   func main()
来源：http://qp.muxihuayi.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://bu.jctech888.com.cn

C#:   static void Main(string[] args)
来源：http://qg.jctech888.com.cn

[M08] 获取系统与运行时信息
来源：http://fk.colortex.cn

Py:   platform.system();  platform.python_version()
来源：http://av.szxytkj.cn

PHP:  PHP_OS;  phpversion();
来源：http://ux.colortex.cn

JS:   process.platform;  process.version
来源：http://hx.nszjky.cn

TS:   process.platform;  process.version
来源：http://ay.bjjhwx.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ha.shtwfgs.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://dd.nszjky.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://xz.szsharing.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://gn.hnjuh.cn

================================================================================
来源：http://yl.hahajie.cn

N. 数据结构与算法
来源：http://xu.hnjuh.cn

================================================================================
来源：http://xs.haigaiapp.cn

[N01] 二分查找（有序数组）
来源：http://ui.bjjhwx.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ex.newstarts.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://sv.shxzukj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xm.muxihuayi.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dr.huixinmuqiang.cn

Java: Arrays.binarySearch(arr, x)
来源：http://rh.yuexingan06.cn

Go:   sort.SearchInts(arr, x)
来源：http://pj.jctech888.com.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://nx.panjiajie.cn

C#:   Array.BinarySearch(arr, x)
来源：http://oy.szsharing.cn

[N02] 排序（工程实践用内置实现）
来源：http://yw.bookmarksfly.cn

Py:   sorted(arr);  arr.sort()
来源：http://jh.lnxyls.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://yk.shxzskj.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://if.panjiajie.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://br.bjjhwx.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://dm.szsharing.cn

Go:   slices.Sort(arr)
来源：http://nn.hahajie.cn

Ruby: arr.sort
来源：http://vc.hnjuh.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ji.jctech888.com.cn

[N03] 快速排序（分治示例）
来源：http://mj.hnjuh.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://li.shtwfgs.cn

PHP:  // 递归实现，或用 usort
来源：http://go.jctech888.com.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gz.haigaiapp.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gu.shtwfgs.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://lv.nszjky.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://oc.jctech888.com.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://yy.shxzskj.cn

C#:   // 手写递归，或 Array.Sort
来源：http://bq.shtwfgs.cn

[N04] 斐波那契数列
来源：http://yz.shxzukj.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://nm.bookmarksfly.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://dy.hahajie.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wi.asd995.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ca.shxzskj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://jw.9csxet.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hm.chemitech.net.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://uq.bookmarksfly.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ig.huixiangedu.cn

[N05] 最大公约数
来源：http://pc.shtwfgs.cn

Py:   math.gcd(a, b)
来源：http://sk.huanxung.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://rk.521024.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ep.panjiajie.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vn.shtwfgs.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://jt.haigaiapp.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://vu.szxytkj.cn

Ruby: a.gcd(b)
来源：http://sq.huixinmuqiang.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wd.shxzukj.cn

[N06] 判断回文字符串
来源：http://dn.newstarts.cn

Py:   s == s[::-1]
来源：http://em.colortex.cn

PHP:  $s === strrev($s);
来源：http://kd.huanxung.cn

JS:   s === [...s].reverse().join("")
来源：http://uu.yuexingan06.cn

TS:   s === [...s].reverse().join("")
来源：http://by.asd995.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xb.shxzukj.cn

Go:   // 双指针从两端比较
来源：http://jr.shxzukj.cn

Ruby: s == s.reverse
来源：http://gt.chemitech.net.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://fr.newstarts.cn

[N07] 两数之和（返回下标）
来源：http://re.shxzskj.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hy.huanxung.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://al.lnxyls.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://gh.szxytkj.cn

TS:   // 手写 Map<string, number>
来源：http://bz.hahajie.cn

Java: // 手写 HashMap
来源：http://ep.szxytkj.cn


<!-- 参考信息 -->