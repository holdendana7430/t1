代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://uf.yuexingan06.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://yk.9csxet.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://eb.wgjwhj.cn

[J10] 取今天 / 本月第一天
来源：http://xm.panjiajie.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://lm.chemitech.net.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://oq.asd995.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ts.hahajie.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://tu.szxytkj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://jp.newstarts.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://sw.521024.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://eo.bjjhwx.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://lo.huixiangedu.cn

================================================================================
来源：http://se.haigaiapp.cn

K. JSON 与序列化
来源：http://we.szxytkj.cn

================================================================================
来源：http://xw.yuexingan06.cn

[K01] 对象转 JSON 字符串
来源：http://hb.9csxet.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://fq.huixinmuqiang.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://oq.jctech888.com.cn

JS:   JSON.stringify(obj)
来源：http://qd.shxzukj.cn

TS:   JSON.stringify(obj)
来源：http://tp.chemitech.net.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://cb.huixinmuqiang.cn

Go:   json.Marshal(obj)
来源：http://bf.yuntaijiaju.cn

Ruby: obj.to_json                                     // require "json"
来源：http://kf.hnjuh.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://sm.hahajie.cn

[K02] JSON 字符串转对象
来源：http://cn.yuntaijiaju.cn

Py:   json.loads(s)
来源：http://yf.nicolike.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://tl.colortex.cn

JS:   JSON.parse(s)
来源：http://qx.chemitech.net.cn

TS:   JSON.parse(s)
来源：http://hg.muxihuayi.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qb.shtwfgs.cn

Go:   json.Unmarshal(data, &v)
来源：http://er.yuexingan06.cn

Ruby: JSON.parse(s)
来源：http://ql.haigaiapp.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://lq.wgjwhj.cn

[K03] JSON 美化输出（带缩进）
来源：http://ao.szxytkj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://pd.9csxet.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://um.newstarts.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://kz.haigaiapp.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://mf.nicolike.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ut.nszjky.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://zi.muxihuayi.cn

Ruby: JSON.pretty_generate(obj)
来源：http://jd.hnjuh.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://vt.asd995.cn

[K04] 读取 JSON 文件
来源：http://co.lnxyls.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ho.szsharing.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://sz.hnjuh.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hl.nicolike.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://oh.hnjuh.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://qp.gzmigu.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://gc.muxihuayi.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://fk.panjiajie.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://gh.szsharing.cn

[K05] 深拷贝对象
来源：http://oe.huanxung.cn

Py:   copy.deepcopy(obj)
来源：http://zc.nicolike.cn

PHP:  unserialize(serialize($obj));
来源：http://mk.yuntaijiaju.cn

JS:   structuredClone(obj)
来源：http://lr.9csxet.cn

TS:   structuredClone(obj)
来源：http://or.bookmarksfly.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://fa.shtwfgs.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ud.hnjuh.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://rw.huixinmuqiang.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://hr.shxzukj.cn

[K06] 解析 URL 查询串
来源：http://cm.panjiajie.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ar.huixinmuqiang.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ab.shxzukj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nw.bjjhwx.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ou.gzmigu.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://qv.yuexingan06.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://mc.shxzukj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://tn.szxytkj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://fa.haigaiapp.cn

[K07] 进制转换
来源：http://rm.nszjky.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ha.huanxung.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://zk.newstarts.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://tq.9csxet.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://sj.nicolike.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://rm.nicolike.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://oa.huixinmuqiang.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://jm.shxzskj.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://pv.lnxyls.cn

[K08] 二进制序列化（非 JSON）
来源：http://du.521024.cn

Py:   pickle.dumps(obj)
来源：http://zt.newstarts.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://bf.yuexingan06.cn

JS:   v8.serialize(obj)        // Node
来源：http://fv.szxytkj.cn

TS:   v8.serialize(obj)        // Node
来源：http://md.shxzukj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://rz.asd995.cn

Go:   encoding/gob
来源：http://wh.szsharing.cn

Ruby: Marshal.dump(obj)
来源：http://ns.bjjhwx.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wc.9csxet.cn

================================================================================
来源：http://ts.521024.cn

L. 网络请求
来源：http://nb.yuexingan06.cn

================================================================================
来源：http://gb.shxzukj.cn

[L01] 发送 GET 请求
来源：http://ix.colortex.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://zi.shxzukj.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://fx.jctech888.com.cn

JS:   await fetch(url)
来源：http://nd.colortex.cn

TS:   await fetch(url)
来源：http://jm.wgjwhj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wy.521024.cn

Go:   resp, err := http.Get(url)
来源：http://qf.shxzukj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ph.shtwfgs.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://gq.nicolike.cn

[L02] 发送 POST JSON
来源：http://rk.gzmigu.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ri.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://yj.nicolike.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qb.yuexingan06.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ts.521024.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://zt.yuexingan06.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://lb.chemitech.net.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://my.9csxet.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://be.bookmarksfly.cn

[L03] 设置自定义请求头
来源：http://sx.hnjuh.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://py.hnjuh.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://tp.bookmarksfly.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sj.shxzskj.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://iw.shxzskj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ss.huixinmuqiang.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://zj.jianghongdianzi.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hx.bjjhwx.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://kg.panjiajie.cn

[L04] 设置超时
来源：http://pe.haigaiapp.cn

Py:   requests.get(url, timeout=5)
来源：http://gf.hnjuh.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wx.huixiangedu.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ua.gzmigu.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://iq.521024.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://en.hnjuh.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ut.jianghongdianzi.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://sj.shxzukj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://bo.newstarts.cn

[L05] 上传文件（multipart）
来源：http://kq.shxzskj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://xr.szsharing.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://at.jianghongdianzi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://cr.shxzskj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://po.huixinmuqiang.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ql.newstarts.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://tp.521024.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ik.hahajie.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://bu.gzmigu.cn

[L06] 解析响应为 JSON
来源：http://kh.jctech888.com.cn

Py:   resp.json()
来源：http://cl.nszjky.cn

PHP:  json_decode($body, true);
来源：http://nu.muxihuayi.cn

JS:   await resp.json()
来源：http://lz.lnxyls.cn

TS:   await resp.json()
来源：http://ei.nszjky.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ik.9csxet.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://jq.bookmarksfly.cn

Ruby: JSON.parse(resp.body)
来源：http://ns.lnxyls.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ax.nicolike.cn

[L07] 处理 HTTP 状态码
来源：http://jm.shxzskj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://uu.szxytkj.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://oq.shtwfgs.cn

JS:   resp.ok;  resp.status
来源：http://iy.bjjhwx.cn

TS:   resp.ok;  resp.status
来源：http://ay.nszjky.cn

Java: resp.statusCode()
来源：http://yh.gzmigu.cn

Go:   resp.StatusCode
来源：http://dk.chemitech.net.cn

Ruby: resp.code.to_i
来源：http://uk.yuexingan06.cn

C#:   (int)resp.StatusCode
来源：http://mo.szsharing.cn

[L08] 并发请求多个地址
来源：http://ll.chemitech.net.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://pv.521024.cn

PHP:  curl_multi_init() 系列
来源：http://pb.shxzukj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ic.9csxet.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://po.shxzskj.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://qp.szxytkj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qk.muxihuayi.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://cq.huanxung.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ui.jctech888.com.cn

================================================================================
来源：http://iw.yuntaijiaju.cn

M. 命令行 / 进程 / 环境
来源：http://cv.colortex.cn

================================================================================
来源：http://lh.asd995.cn

[M01] 读取命令行参数
来源：http://yk.szsharing.cn

Py:   sys.argv[1:]
来源：http://am.bookmarksfly.cn

PHP:  $argv;  $argc;
来源：http://yq.shxzukj.cn

JS:   process.argv.slice(2)
来源：http://yp.hnjuh.cn

TS:   process.argv.slice(2)
来源：http://gl.szxytkj.cn

Java: args 数组（main 方法参数）
来源：http://gl.bookmarksfly.cn

Go:   os.Args[1:]
来源：http://qz.jianghongdianzi.cn

Ruby: ARGV
来源：http://al.asd995.cn

C#:   args 数组（Main 方法参数）
来源：http://fx.521024.cn

[M02] 读取环境变量
来源：http://qv.shxzukj.cn

Py:   os.environ.get("HOME")
来源：http://ae.colortex.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ro.szxytkj.cn

JS:   process.env.HOME
来源：http://zp.huixiangedu.cn

TS:   process.env.HOME
来源：http://no.panjiajie.cn

Java: System.getenv("HOME")
来源：http://fi.panjiajie.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://nh.9csxet.cn

Ruby: ENV["HOME"]
来源：http://wu.hahajie.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://pz.colortex.cn

[M03] 执行外部命令
来源：http://cl.bookmarksfly.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://se.hahajie.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://cm.nicolike.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://rg.szsharing.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://io.yuntaijiaju.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://pm.9csxet.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://al.asd995.cn

Ruby: system("ls -l");  `ls -l`
来源：http://fb.hahajie.cn

C#:   Process.Start("ls", "-l");
来源：http://yx.muxihuayi.cn

[M04] 获取当前工作目录
来源：http://wl.lnxyls.cn

Py:   os.getcwd()
来源：http://vq.newstarts.cn

PHP:  getcwd();
来源：http://qq.bjjhwx.cn

JS:   process.cwd()
来源：http://kr.yuntaijiaju.cn

TS:   process.cwd()
来源：http://kl.huanxung.cn

Java: Path.of("").toAbsolutePath()
来源：http://rs.bookmarksfly.cn

Go:   os.Getwd()
来源：http://gi.jianghongdianzi.cn

Ruby: Dir.pwd
来源：http://ke.bjjhwx.cn

C#:   Directory.GetCurrentDirectory()
来源：http://nv.szsharing.cn

[M05] 设置退出码
来源：http://qr.chemitech.net.cn

Py:   sys.exit(1)
来源：http://iw.newstarts.cn

PHP:  exit(1);
来源：http://nc.szxytkj.cn

JS:   process.exit(1)
来源：http://zb.chemitech.net.cn

TS:   process.exit(1)
来源：http://fk.szxytkj.cn

Java: System.exit(1)
来源：http://gp.huanxung.cn

Go:   os.Exit(1)
来源：http://zf.gzmigu.cn

Ruby: exit 1
来源：http://th.hnjuh.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://xe.hnjuh.cn

[M06] 向标准错误输出
来源：http://ur.panjiajie.cn

Py:   print("err", file=sys.stderr)
来源：http://lg.chemitech.net.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://nc.chemitech.net.cn

JS:   console.error("err")
来源：http://kc.szsharing.cn

TS:   console.error("err")
来源：http://ic.bookmarksfly.cn

Java: System.err.println("err")
来源：http://eh.jctech888.com.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://vc.shtwfgs.cn

Ruby: warn "err"
来源：http://sk.haigaiapp.cn

C#:   Console.Error.WriteLine("err")
来源：http://gk.huixiangedu.cn

[M07] 判断是否为主入口
来源：http://hu.huanxung.cn

Py:   if __name__ == "__main__":
来源：http://js.szsharing.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ap.nicolike.cn

JS:   require.main === module
来源：http://gc.szsharing.cn

TS:   require.main === module
来源：http://cq.bjjhwx.cn

Java: public static void main(String[] args)
来源：http://lo.haigaiapp.cn

Go:   func main()
来源：http://gw.hnjuh.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://pi.szsharing.cn

C#:   static void Main(string[] args)
来源：http://by.panjiajie.cn

[M08] 获取系统与运行时信息
来源：http://al.hahajie.cn

Py:   platform.system();  platform.python_version()
来源：http://iq.lnxyls.cn

PHP:  PHP_OS;  phpversion();
来源：http://hk.bjjhwx.cn

JS:   process.platform;  process.version
来源：http://rj.huixinmuqiang.cn

TS:   process.platform;  process.version
来源：http://ph.jctech888.com.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ps.yuntaijiaju.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ef.yuntaijiaju.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://lr.nicolike.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://zy.chemitech.net.cn

================================================================================
来源：http://od.chemitech.net.cn

N. 数据结构与算法
来源：http://qj.huixinmuqiang.cn

================================================================================
来源：http://xa.shxzukj.cn

[N01] 二分查找（有序数组）
来源：http://lj.nszjky.cn

Py:   bisect.bisect_left(arr, x)
来源：http://du.bjjhwx.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ph.9csxet.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ia.wgjwhj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hy.colortex.cn

Java: Arrays.binarySearch(arr, x)
来源：http://xr.newstarts.cn

Go:   sort.SearchInts(arr, x)
来源：http://ii.shxzukj.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://tr.hnjuh.cn

C#:   Array.BinarySearch(arr, x)
来源：http://er.haigaiapp.cn

[N02] 排序（工程实践用内置实现）
来源：http://bs.bookmarksfly.cn

Py:   sorted(arr);  arr.sort()
来源：http://og.muxihuayi.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mk.hnjuh.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://fm.asd995.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://my.jctech888.com.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ua.jctech888.com.cn

Go:   slices.Sort(arr)
来源：http://ll.jctech888.com.cn

Ruby: arr.sort
来源：http://cd.bjjhwx.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://wl.panjiajie.cn

[N03] 快速排序（分治示例）
来源：http://rk.hahajie.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://un.bookmarksfly.cn

PHP:  // 递归实现，或用 usort
来源：http://us.szsharing.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jf.hahajie.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cx.shtwfgs.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://dn.521024.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://kn.colortex.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://fc.panjiajie.cn

C#:   // 手写递归，或 Array.Sort
来源：http://tp.wgjwhj.cn

[N04] 斐波那契数列
来源：http://tr.bjjhwx.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wc.huixinmuqiang.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://jr.nicolike.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lt.panjiajie.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ye.yuntaijiaju.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://pv.szsharing.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://oz.9csxet.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://fg.huanxung.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://go.521024.cn

[N05] 最大公约数
来源：http://sm.shxzskj.cn

Py:   math.gcd(a, b)
来源：http://wz.shxzskj.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://jm.bookmarksfly.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kg.gzmigu.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dd.huanxung.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://gk.bjjhwx.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://cu.colortex.cn

Ruby: a.gcd(b)
来源：http://hj.muxihuayi.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://cn.asd995.cn

[N06] 判断回文字符串
来源：http://jf.huixinmuqiang.cn

Py:   s == s[::-1]
来源：http://lp.shxzskj.cn

PHP:  $s === strrev($s);
来源：http://ag.muxihuayi.cn

JS:   s === [...s].reverse().join("")
来源：http://so.521024.cn

TS:   s === [...s].reverse().join("")
来源：http://av.yuntaijiaju.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://tf.huixiangedu.cn

Go:   // 双指针从两端比较
来源：http://ft.jctech888.com.cn

Ruby: s == s.reverse
来源：http://we.yuexingan06.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://yb.colortex.cn

[N07] 两数之和（返回下标）
来源：http://ko.colortex.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ec.yuexingan06.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://me.jianghongdianzi.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://nx.9csxet.cn

TS:   // 手写 Map<string, number>
来源：http://rh.yuexingan06.cn

Java: // 手写 HashMap
来源：http://od.newstarts.cn


<!-- 参考信息 -->