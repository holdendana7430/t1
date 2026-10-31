代发 wailian999

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://jz.chemitech.net.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gd.haigaiapp.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fq.nszjky.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://nr.9csxet.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://or.yuexingan06.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://yr.muxihuayi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://cy.shxzukj.cn

[J10] 取今天 / 本月第一天
来源：http://qa.hnjuh.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ss.asd995.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://zd.shxzukj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://pe.huixiangedu.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://yz.yuntaijiaju.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://gt.haigaiapp.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://os.nszjky.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://pk.huanxung.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://pz.szxytkj.cn

================================================================================
来源：http://li.lnxyls.cn

K. JSON 与序列化
来源：http://iq.521024.cn

================================================================================
来源：http://ts.jctech888.com.cn

[K01] 对象转 JSON 字符串
来源：http://ba.muxihuayi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://bp.jianghongdianzi.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://yd.haigaiapp.cn

JS:   JSON.stringify(obj)
来源：http://fs.chemitech.net.cn

TS:   JSON.stringify(obj)
来源：http://bw.shxzskj.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://xq.jctech888.com.cn

Go:   json.Marshal(obj)
来源：http://rb.szsharing.cn

Ruby: obj.to_json                                     // require "json"
来源：http://cl.nicolike.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ph.panjiajie.cn

[K02] JSON 字符串转对象
来源：http://oy.hahajie.cn

Py:   json.loads(s)
来源：http://kl.shxzskj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://jy.haigaiapp.cn

JS:   JSON.parse(s)
来源：http://xc.huixinmuqiang.cn

TS:   JSON.parse(s)
来源：http://bw.jianghongdianzi.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://sa.huanxung.cn

Go:   json.Unmarshal(data, &v)
来源：http://ex.shxzskj.cn

Ruby: JSON.parse(s)
来源：http://dl.huixinmuqiang.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://as.lnxyls.cn

[K03] JSON 美化输出（带缩进）
来源：http://rm.haigaiapp.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ul.gzmigu.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://rn.nicolike.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://tk.chemitech.net.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://zp.panjiajie.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://aq.yuntaijiaju.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://fo.chemitech.net.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ww.colortex.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://qw.bjjhwx.cn

[K04] 读取 JSON 文件
来源：http://xt.yuexingan06.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://te.newstarts.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://kb.9csxet.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bc.shxzskj.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dg.huanxung.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vo.shxzukj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://aq.bjjhwx.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://xy.szxytkj.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jn.jianghongdianzi.cn

[K05] 深拷贝对象
来源：http://oh.muxihuayi.cn

Py:   copy.deepcopy(obj)
来源：http://ay.colortex.cn

PHP:  unserialize(serialize($obj));
来源：http://xl.jianghongdianzi.cn

JS:   structuredClone(obj)
来源：http://zp.hahajie.cn

TS:   structuredClone(obj)
来源：http://ep.521024.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://cl.shxzukj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mz.colortex.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wv.lnxyls.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://pr.chemitech.net.cn

[K06] 解析 URL 查询串
来源：http://bk.szxytkj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rv.huixinmuqiang.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://pb.yuntaijiaju.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fb.nszjky.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qg.shxzukj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ch.nszjky.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://oc.shxzukj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://rd.bjjhwx.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://jl.haigaiapp.cn

[K07] 进制转换
来源：http://qm.bookmarksfly.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://yk.nszjky.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vr.huixinmuqiang.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://er.newstarts.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ma.shxzukj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ia.yuexingan06.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://gw.szsharing.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://aa.shxzukj.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://rs.wgjwhj.cn

[K08] 二进制序列化（非 JSON）
来源：http://tn.chemitech.net.cn

Py:   pickle.dumps(obj)
来源：http://jl.muxihuayi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://uq.newstarts.cn

JS:   v8.serialize(obj)        // Node
来源：http://jd.hnjuh.cn

TS:   v8.serialize(obj)        // Node
来源：http://im.szsharing.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://fz.huanxung.cn

Go:   encoding/gob
来源：http://us.wgjwhj.cn

Ruby: Marshal.dump(obj)
来源：http://qz.hahajie.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://cy.hahajie.cn

================================================================================
来源：http://dc.nicolike.cn

L. 网络请求
来源：http://xs.lnxyls.cn

================================================================================
来源：http://nb.shtwfgs.cn

[L01] 发送 GET 请求
来源：http://tf.nszjky.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://bm.shtwfgs.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ue.colortex.cn

JS:   await fetch(url)
来源：http://hv.hnjuh.cn

TS:   await fetch(url)
来源：http://ko.shxzskj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://lj.521024.cn

Go:   resp, err := http.Get(url)
来源：http://fo.jctech888.com.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://er.9csxet.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://vi.chemitech.net.cn

[L02] 发送 POST JSON
来源：http://zn.bjjhwx.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ou.huixiangedu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xg.haigaiapp.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kr.hnjuh.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xw.newstarts.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://fo.hnjuh.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://cn.hahajie.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://aj.521024.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://lz.haigaiapp.cn

[L03] 设置自定义请求头
来源：http://sp.bjjhwx.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://lg.asd995.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://im.jctech888.com.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zy.yuexingan06.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ot.521024.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hx.huixiangedu.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://az.panjiajie.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://cj.bookmarksfly.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hh.colortex.cn

[L04] 设置超时
来源：http://nr.haigaiapp.cn

Py:   requests.get(url, timeout=5)
来源：http://sn.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ly.shxzukj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nw.9csxet.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ru.panjiajie.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://tq.colortex.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ls.9csxet.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://un.chemitech.net.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://iv.newstarts.cn

[L05] 上传文件（multipart）
来源：http://ia.asd995.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zk.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ea.szsharing.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ge.yuntaijiaju.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://bf.bookmarksfly.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hd.lnxyls.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://kf.szsharing.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vh.huixinmuqiang.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://bu.szsharing.cn

[L06] 解析响应为 JSON
来源：http://mc.nicolike.cn

Py:   resp.json()
来源：http://re.chemitech.net.cn

PHP:  json_decode($body, true);
来源：http://uo.521024.cn

JS:   await resp.json()
来源：http://kd.asd995.cn

TS:   await resp.json()
来源：http://jr.jianghongdianzi.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://zo.haigaiapp.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://jo.nszjky.cn

Ruby: JSON.parse(resp.body)
来源：http://du.huixiangedu.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://oi.newstarts.cn

[L07] 处理 HTTP 状态码
来源：http://dr.yuntaijiaju.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hp.szsharing.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qe.jianghongdianzi.cn

JS:   resp.ok;  resp.status
来源：http://nm.huanxung.cn

TS:   resp.ok;  resp.status
来源：http://nf.shtwfgs.cn

Java: resp.statusCode()
来源：http://fw.colortex.cn

Go:   resp.StatusCode
来源：http://ia.newstarts.cn

Ruby: resp.code.to_i
来源：http://ph.chemitech.net.cn

C#:   (int)resp.StatusCode
来源：http://vs.shxzskj.cn

[L08] 并发请求多个地址
来源：http://eq.bookmarksfly.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://st.jianghongdianzi.cn

PHP:  curl_multi_init() 系列
来源：http://tb.shxzskj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qb.huanxung.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kb.shxzukj.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://no.521024.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://aq.521024.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://im.nicolike.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ia.bjjhwx.cn

================================================================================
来源：http://ln.gzmigu.cn

M. 命令行 / 进程 / 环境
来源：http://ay.huanxung.cn

================================================================================
来源：http://qb.asd995.cn

[M01] 读取命令行参数
来源：http://kc.asd995.cn

Py:   sys.argv[1:]
来源：http://nf.muxihuayi.cn

PHP:  $argv;  $argc;
来源：http://ll.yuntaijiaju.cn

JS:   process.argv.slice(2)
来源：http://ne.nicolike.cn

TS:   process.argv.slice(2)
来源：http://fc.nicolike.cn

Java: args 数组（main 方法参数）
来源：http://ao.szxytkj.cn

Go:   os.Args[1:]
来源：http://mg.muxihuayi.cn

Ruby: ARGV
来源：http://lx.szxytkj.cn

C#:   args 数组（Main 方法参数）
来源：http://yk.yuexingan06.cn

[M02] 读取环境变量
来源：http://ha.nicolike.cn

Py:   os.environ.get("HOME")
来源：http://qu.nicolike.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://jd.shxzskj.cn

JS:   process.env.HOME
来源：http://ka.521024.cn

TS:   process.env.HOME
来源：http://fc.shxzukj.cn

Java: System.getenv("HOME")
来源：http://vz.gzmigu.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://tf.9csxet.cn

Ruby: ENV["HOME"]
来源：http://nr.shxzskj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ul.gzmigu.cn

[M03] 执行外部命令
来源：http://xa.shxzskj.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://pd.jianghongdianzi.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ea.jctech888.com.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://bh.shxzukj.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ci.haigaiapp.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ov.chemitech.net.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://fj.chemitech.net.cn

Ruby: system("ls -l");  `ls -l`
来源：http://bw.huixiangedu.cn

C#:   Process.Start("ls", "-l");
来源：http://ip.asd995.cn

[M04] 获取当前工作目录
来源：http://fl.newstarts.cn

Py:   os.getcwd()
来源：http://gl.bjjhwx.cn

PHP:  getcwd();
来源：http://wv.shtwfgs.cn

JS:   process.cwd()
来源：http://oo.asd995.cn

TS:   process.cwd()
来源：http://qx.haigaiapp.cn

Java: Path.of("").toAbsolutePath()
来源：http://qm.szsharing.cn

Go:   os.Getwd()
来源：http://kc.hahajie.cn

Ruby: Dir.pwd
来源：http://yz.jctech888.com.cn

C#:   Directory.GetCurrentDirectory()
来源：http://vr.shtwfgs.cn

[M05] 设置退出码
来源：http://it.bookmarksfly.cn

Py:   sys.exit(1)
来源：http://sd.bookmarksfly.cn

PHP:  exit(1);
来源：http://fd.hnjuh.cn

JS:   process.exit(1)
来源：http://yh.colortex.cn

TS:   process.exit(1)
来源：http://jp.nszjky.cn

Java: System.exit(1)
来源：http://hg.521024.cn

Go:   os.Exit(1)
来源：http://gl.9csxet.cn

Ruby: exit 1
来源：http://uk.huanxung.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://eh.yuntaijiaju.cn

[M06] 向标准错误输出
来源：http://im.jianghongdianzi.cn

Py:   print("err", file=sys.stderr)
来源：http://qn.szsharing.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://lu.asd995.cn

JS:   console.error("err")
来源：http://bu.shxzukj.cn

TS:   console.error("err")
来源：http://co.asd995.cn

Java: System.err.println("err")
来源：http://wh.shtwfgs.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://er.colortex.cn

Ruby: warn "err"
来源：http://ex.muxihuayi.cn

C#:   Console.Error.WriteLine("err")
来源：http://tt.shxzskj.cn

[M07] 判断是否为主入口
来源：http://sz.shxzskj.cn

Py:   if __name__ == "__main__":
来源：http://gb.chemitech.net.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mu.nicolike.cn

JS:   require.main === module
来源：http://sq.szxytkj.cn

TS:   require.main === module
来源：http://ll.chemitech.net.cn

Java: public static void main(String[] args)
来源：http://ka.nicolike.cn

Go:   func main()
来源：http://xj.wgjwhj.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://at.newstarts.cn

C#:   static void Main(string[] args)
来源：http://jm.bjjhwx.cn

[M08] 获取系统与运行时信息
来源：http://iz.szxytkj.cn

Py:   platform.system();  platform.python_version()
来源：http://lc.huixinmuqiang.cn

PHP:  PHP_OS;  phpversion();
来源：http://ub.yuntaijiaju.cn

JS:   process.platform;  process.version
来源：http://jv.bjjhwx.cn

TS:   process.platform;  process.version
来源：http://ex.hahajie.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://do.szxytkj.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://uj.hnjuh.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://va.huanxung.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://kh.bjjhwx.cn

================================================================================
来源：http://ef.shtwfgs.cn

N. 数据结构与算法
来源：http://rv.panjiajie.cn

================================================================================
来源：http://ya.huixiangedu.cn

[N01] 二分查找（有序数组）
来源：http://hd.yuexingan06.cn

Py:   bisect.bisect_left(arr, x)
来源：http://jn.muxihuayi.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mk.huixiangedu.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gr.bookmarksfly.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rv.muxihuayi.cn

Java: Arrays.binarySearch(arr, x)
来源：http://yw.yuntaijiaju.cn

Go:   sort.SearchInts(arr, x)
来源：http://zv.huanxung.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://bo.shtwfgs.cn

C#:   Array.BinarySearch(arr, x)
来源：http://vm.lnxyls.cn

[N02] 排序（工程实践用内置实现）
来源：http://bg.hahajie.cn

Py:   sorted(arr);  arr.sort()
来源：http://ew.shxzukj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://rj.haigaiapp.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://bm.jctech888.com.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://vt.521024.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ij.shxzukj.cn

Go:   slices.Sort(arr)
来源：http://au.shxzskj.cn

Ruby: arr.sort
来源：http://jd.shtwfgs.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ib.hahajie.cn

[N03] 快速排序（分治示例）
来源：http://os.yuntaijiaju.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hk.jctech888.com.cn

PHP:  // 递归实现，或用 usort
来源：http://co.nicolike.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zo.newstarts.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rz.haigaiapp.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://nd.huixinmuqiang.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://oa.muxihuayi.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://dz.9csxet.cn

C#:   // 手写递归，或 Array.Sort
来源：http://gp.szxytkj.cn

[N04] 斐波那契数列
来源：http://jj.gzmigu.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://cw.bookmarksfly.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://rt.szsharing.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ox.chemitech.net.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wc.nicolike.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://nw.huixiangedu.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://yd.bookmarksfly.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://zx.asd995.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://zq.shtwfgs.cn

[N05] 最大公约数
来源：http://ng.bookmarksfly.cn

Py:   math.gcd(a, b)
来源：http://im.huanxung.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://dd.huanxung.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cd.hnjuh.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qi.gzmigu.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mc.haigaiapp.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://dq.huanxung.cn

Ruby: a.gcd(b)
来源：http://az.wgjwhj.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://bf.asd995.cn

[N06] 判断回文字符串
来源：http://ib.521024.cn

Py:   s == s[::-1]
来源：http://rh.asd995.cn

PHP:  $s === strrev($s);
来源：http://jo.huixinmuqiang.cn

JS:   s === [...s].reverse().join("")
来源：http://kt.bjjhwx.cn

TS:   s === [...s].reverse().join("")
来源：http://pl.muxihuayi.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ep.nicolike.cn

Go:   // 双指针从两端比较
来源：http://ky.yuexingan06.cn

Ruby: s == s.reverse
来源：http://dj.hnjuh.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://dk.huanxung.cn

[N07] 两数之和（返回下标）
来源：http://fo.newstarts.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ca.yuexingan06.cn


<!-- 参考信息 -->