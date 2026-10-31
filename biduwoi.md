代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://he.lnxyls.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://nd.nicolike.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jw.newstarts.cn

[J10] 取今天 / 本月第一天
来源：http://vi.hnjuh.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://se.hahajie.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://gy.gzmigu.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://fo.haigaiapp.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ka.szsharing.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://jk.huixinmuqiang.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://oy.nicolike.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://cg.521024.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ud.huixinmuqiang.cn

================================================================================
来源：http://jq.huanxung.cn

K. JSON 与序列化
来源：http://st.shxzukj.cn

================================================================================
来源：http://qq.huanxung.cn

[K01] 对象转 JSON 字符串
来源：http://pr.lnxyls.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://no.jctech888.com.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://oq.shxzukj.cn

JS:   JSON.stringify(obj)
来源：http://zd.nicolike.cn

TS:   JSON.stringify(obj)
来源：http://fm.nicolike.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://cl.haigaiapp.cn

Go:   json.Marshal(obj)
来源：http://xc.huixinmuqiang.cn

Ruby: obj.to_json                                     // require "json"
来源：http://aa.shtwfgs.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://no.shxzukj.cn

[K02] JSON 字符串转对象
来源：http://ke.wgjwhj.cn

Py:   json.loads(s)
来源：http://or.9csxet.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hi.lnxyls.cn

JS:   JSON.parse(s)
来源：http://yk.gzmigu.cn

TS:   JSON.parse(s)
来源：http://ay.bjjhwx.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qq.shxzskj.cn

Go:   json.Unmarshal(data, &v)
来源：http://gh.yuntaijiaju.cn

Ruby: JSON.parse(s)
来源：http://uz.shxzukj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://xb.9csxet.cn

[K03] JSON 美化输出（带缩进）
来源：http://zm.nicolike.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://fb.asd995.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://iu.newstarts.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ul.nicolike.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://df.muxihuayi.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://np.huixinmuqiang.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://if.asd995.cn

Ruby: JSON.pretty_generate(obj)
来源：http://kl.panjiajie.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://pd.shtwfgs.cn

[K04] 读取 JSON 文件
来源：http://vx.huixinmuqiang.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ww.huixinmuqiang.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ay.shxzukj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ke.szsharing.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://oz.nszjky.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://qu.yuexingan06.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ym.9csxet.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://yo.521024.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://kp.nszjky.cn

[K05] 深拷贝对象
来源：http://vc.asd995.cn

Py:   copy.deepcopy(obj)
来源：http://er.jctech888.com.cn

PHP:  unserialize(serialize($obj));
来源：http://eo.hahajie.cn

JS:   structuredClone(obj)
来源：http://vy.huixiangedu.cn

TS:   structuredClone(obj)
来源：http://ky.gzmigu.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://hq.hahajie.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://fr.lnxyls.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://iu.newstarts.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://qo.bookmarksfly.cn

[K06] 解析 URL 查询串
来源：http://wv.shxzskj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://qs.lnxyls.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zc.szxytkj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wh.bjjhwx.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xc.shxzukj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://an.nszjky.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://oh.shtwfgs.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://jo.hnjuh.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://pj.jctech888.com.cn

[K07] 进制转换
来源：http://pt.newstarts.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://rw.muxihuayi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://kh.asd995.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://qh.asd995.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://nf.521024.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://dj.chemitech.net.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://vc.huixiangedu.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ak.521024.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://du.szsharing.cn

[K08] 二进制序列化（非 JSON）
来源：http://ws.wgjwhj.cn

Py:   pickle.dumps(obj)
来源：http://xc.haigaiapp.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://kd.jctech888.com.cn

JS:   v8.serialize(obj)        // Node
来源：http://fh.haigaiapp.cn

TS:   v8.serialize(obj)        // Node
来源：http://mx.jctech888.com.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://af.huixiangedu.cn

Go:   encoding/gob
来源：http://rg.shtwfgs.cn

Ruby: Marshal.dump(obj)
来源：http://ig.jianghongdianzi.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://iu.newstarts.cn

================================================================================
来源：http://st.bookmarksfly.cn

L. 网络请求
来源：http://gi.bjjhwx.cn

================================================================================
来源：http://nd.panjiajie.cn

[L01] 发送 GET 请求
来源：http://jn.shxzukj.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://rb.wgjwhj.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://jy.muxihuayi.cn

JS:   await fetch(url)
来源：http://hp.wgjwhj.cn

TS:   await fetch(url)
来源：http://by.lnxyls.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ae.szsharing.cn

Go:   resp, err := http.Get(url)
来源：http://uf.muxihuayi.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://yw.huixinmuqiang.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://gd.9csxet.cn

[L02] 发送 POST JSON
来源：http://qv.muxihuayi.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ih.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://da.asd995.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hx.wgjwhj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dl.muxihuayi.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://uf.chemitech.net.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://gy.yuexingan06.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://tx.szxytkj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://vv.bjjhwx.cn

[L03] 设置自定义请求头
来源：http://hj.muxihuayi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mx.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ej.shxzukj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://di.shtwfgs.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://un.bookmarksfly.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://pz.wgjwhj.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://lk.muxihuayi.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://zh.panjiajie.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://xv.shxzskj.cn

[L04] 设置超时
来源：http://ni.muxihuayi.cn

Py:   requests.get(url, timeout=5)
来源：http://qa.szsharing.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ww.chemitech.net.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tn.nicolike.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://aq.panjiajie.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ke.shtwfgs.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://rq.yuntaijiaju.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://vc.newstarts.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hy.szsharing.cn

[L05] 上传文件（multipart）
来源：http://hv.szsharing.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ul.haigaiapp.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://xq.shxzukj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://po.bookmarksfly.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://rj.haigaiapp.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://xh.wgjwhj.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://sq.huanxung.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ge.huixiangedu.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://tl.bjjhwx.cn

[L06] 解析响应为 JSON
来源：http://yr.yuntaijiaju.cn

Py:   resp.json()
来源：http://rb.jctech888.com.cn

PHP:  json_decode($body, true);
来源：http://jn.huanxung.cn

JS:   await resp.json()
来源：http://ne.asd995.cn

TS:   await resp.json()
来源：http://cu.yuexingan06.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://lk.newstarts.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ue.lnxyls.cn

Ruby: JSON.parse(resp.body)
来源：http://nc.shxzskj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://fj.bjjhwx.cn

[L07] 处理 HTTP 状态码
来源：http://bu.9csxet.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://su.chemitech.net.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ew.gzmigu.cn

JS:   resp.ok;  resp.status
来源：http://ie.9csxet.cn

TS:   resp.ok;  resp.status
来源：http://qi.newstarts.cn

Java: resp.statusCode()
来源：http://sv.521024.cn

Go:   resp.StatusCode
来源：http://sb.yuexingan06.cn

Ruby: resp.code.to_i
来源：http://lg.nicolike.cn

C#:   (int)resp.StatusCode
来源：http://ey.hahajie.cn

[L08] 并发请求多个地址
来源：http://ix.panjiajie.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ak.yuntaijiaju.cn

PHP:  curl_multi_init() 系列
来源：http://wa.shxzukj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vn.nicolike.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zs.colortex.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://kc.jianghongdianzi.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ot.newstarts.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://yc.jctech888.com.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mw.chemitech.net.cn

================================================================================
来源：http://jl.9csxet.cn

M. 命令行 / 进程 / 环境
来源：http://fj.huanxung.cn

================================================================================
来源：http://op.huanxung.cn

[M01] 读取命令行参数
来源：http://xb.bookmarksfly.cn

Py:   sys.argv[1:]
来源：http://qg.shxzskj.cn

PHP:  $argv;  $argc;
来源：http://vw.haigaiapp.cn

JS:   process.argv.slice(2)
来源：http://xi.yuntaijiaju.cn

TS:   process.argv.slice(2)
来源：http://we.huixiangedu.cn

Java: args 数组（main 方法参数）
来源：http://cd.colortex.cn

Go:   os.Args[1:]
来源：http://oy.9csxet.cn

Ruby: ARGV
来源：http://qh.521024.cn

C#:   args 数组（Main 方法参数）
来源：http://rq.bookmarksfly.cn

[M02] 读取环境变量
来源：http://rp.wgjwhj.cn

Py:   os.environ.get("HOME")
来源：http://sl.hahajie.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zt.szxytkj.cn

JS:   process.env.HOME
来源：http://ow.szxytkj.cn

TS:   process.env.HOME
来源：http://bk.wgjwhj.cn

Java: System.getenv("HOME")
来源：http://ns.nicolike.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ps.gzmigu.cn

Ruby: ENV["HOME"]
来源：http://rh.yuexingan06.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ph.hnjuh.cn

[M03] 执行外部命令
来源：http://nv.bjjhwx.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://gh.shxzskj.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://yx.bookmarksfly.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://zv.muxihuayi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://jz.shxzukj.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://xk.hnjuh.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://vi.huanxung.cn

Ruby: system("ls -l");  `ls -l`
来源：http://pz.521024.cn

C#:   Process.Start("ls", "-l");
来源：http://pu.szxytkj.cn

[M04] 获取当前工作目录
来源：http://zo.wgjwhj.cn

Py:   os.getcwd()
来源：http://sh.hnjuh.cn

PHP:  getcwd();
来源：http://hq.wgjwhj.cn

JS:   process.cwd()
来源：http://lf.hnjuh.cn

TS:   process.cwd()
来源：http://pk.gzmigu.cn

Java: Path.of("").toAbsolutePath()
来源：http://og.jctech888.com.cn

Go:   os.Getwd()
来源：http://do.colortex.cn

Ruby: Dir.pwd
来源：http://sg.colortex.cn

C#:   Directory.GetCurrentDirectory()
来源：http://hb.jctech888.com.cn

[M05] 设置退出码
来源：http://ig.yuntaijiaju.cn

Py:   sys.exit(1)
来源：http://zw.colortex.cn

PHP:  exit(1);
来源：http://ul.newstarts.cn

JS:   process.exit(1)
来源：http://di.hahajie.cn

TS:   process.exit(1)
来源：http://lo.haigaiapp.cn

Java: System.exit(1)
来源：http://ry.huanxung.cn

Go:   os.Exit(1)
来源：http://jf.huanxung.cn

Ruby: exit 1
来源：http://xe.szsharing.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://oj.shtwfgs.cn

[M06] 向标准错误输出
来源：http://lf.haigaiapp.cn

Py:   print("err", file=sys.stderr)
来源：http://fp.hahajie.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://yc.gzmigu.cn

JS:   console.error("err")
来源：http://im.bookmarksfly.cn

TS:   console.error("err")
来源：http://op.colortex.cn

Java: System.err.println("err")
来源：http://fv.hnjuh.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://qz.shtwfgs.cn

Ruby: warn "err"
来源：http://ja.muxihuayi.cn

C#:   Console.Error.WriteLine("err")
来源：http://xj.521024.cn

[M07] 判断是否为主入口
来源：http://ps.huixiangedu.cn

Py:   if __name__ == "__main__":
来源：http://vp.szsharing.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://un.colortex.cn

JS:   require.main === module
来源：http://fg.521024.cn

TS:   require.main === module
来源：http://vj.szxytkj.cn

Java: public static void main(String[] args)
来源：http://bu.nszjky.cn

Go:   func main()
来源：http://op.jctech888.com.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://gl.huixinmuqiang.cn

C#:   static void Main(string[] args)
来源：http://re.jianghongdianzi.cn

[M08] 获取系统与运行时信息
来源：http://jj.nicolike.cn

Py:   platform.system();  platform.python_version()
来源：http://ru.shxzukj.cn

PHP:  PHP_OS;  phpversion();
来源：http://mp.gzmigu.cn

JS:   process.platform;  process.version
来源：http://zh.nszjky.cn

TS:   process.platform;  process.version
来源：http://nb.asd995.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ef.wgjwhj.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://yt.huixiangedu.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ci.9csxet.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://nk.jianghongdianzi.cn

================================================================================
来源：http://uo.panjiajie.cn

N. 数据结构与算法
来源：http://et.hnjuh.cn

================================================================================
来源：http://pt.shxzskj.cn

[N01] 二分查找（有序数组）
来源：http://hh.nicolike.cn

Py:   bisect.bisect_left(arr, x)
来源：http://jf.shxzukj.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://zp.colortex.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://no.chemitech.net.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ie.chemitech.net.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ss.huixinmuqiang.cn

Go:   sort.SearchInts(arr, x)
来源：http://da.shxzskj.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://lr.szxytkj.cn

C#:   Array.BinarySearch(arr, x)
来源：http://hc.nicolike.cn

[N02] 排序（工程实践用内置实现）
来源：http://eq.asd995.cn

Py:   sorted(arr);  arr.sort()
来源：http://cq.huixinmuqiang.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wy.hahajie.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ny.jctech888.com.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://qh.haigaiapp.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://sl.shxzukj.cn

Go:   slices.Sort(arr)
来源：http://po.muxihuayi.cn

Ruby: arr.sort
来源：http://gx.jctech888.com.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ja.shxzukj.cn

[N03] 快速排序（分治示例）
来源：http://oo.lnxyls.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://dr.shtwfgs.cn

PHP:  // 递归实现，或用 usort
来源：http://lz.521024.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wm.huixinmuqiang.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gb.nicolike.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://xn.bookmarksfly.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ce.wgjwhj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://na.jctech888.com.cn

C#:   // 手写递归，或 Array.Sort
来源：http://du.hahajie.cn

[N04] 斐波那契数列
来源：http://mh.gzmigu.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://fc.huixiangedu.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://nq.yuntaijiaju.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ob.panjiajie.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rr.bjjhwx.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://qv.9csxet.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ka.wgjwhj.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ar.jianghongdianzi.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://po.szxytkj.cn

[N05] 最大公约数
来源：http://nn.hnjuh.cn

Py:   math.gcd(a, b)
来源：http://ko.bookmarksfly.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://lz.nszjky.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sq.jctech888.com.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cl.haigaiapp.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zd.shxzukj.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://qx.shxzskj.cn

Ruby: a.gcd(b)
来源：http://wf.hnjuh.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://gn.haigaiapp.cn

[N06] 判断回文字符串
来源：http://qf.asd995.cn

Py:   s == s[::-1]
来源：http://nt.chemitech.net.cn

PHP:  $s === strrev($s);
来源：http://rv.shtwfgs.cn

JS:   s === [...s].reverse().join("")
来源：http://bx.521024.cn

TS:   s === [...s].reverse().join("")
来源：http://jj.gzmigu.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://kb.bjjhwx.cn

Go:   // 双指针从两端比较
来源：http://ns.hnjuh.cn

Ruby: s == s.reverse
来源：http://ug.yuntaijiaju.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://os.yuexingan06.cn

[N07] 两数之和（返回下标）
来源：http://ve.shxzskj.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://uf.gzmigu.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://lz.nicolike.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://gs.huanxung.cn

TS:   // 手写 Map<string, number>
来源：http://jz.huixiangedu.cn

Java: // 手写 HashMap
来源：http://yb.muxihuayi.cn


<!-- 参考信息 -->