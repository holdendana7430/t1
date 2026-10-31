代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hw.panjiajie.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://bu.shxzskj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://pb.jianghongdianzi.cn

[J10] 取今天 / 本月第一天
来源：http://rj.hahajie.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://cy.bookmarksfly.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://pi.huanxung.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://he.szsharing.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://jb.hahajie.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ah.wgjwhj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xb.bookmarksfly.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://rp.gzmigu.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://nk.yuexingan06.cn

================================================================================
来源：http://fp.jctech888.com.cn

K. JSON 与序列化
来源：http://ii.asd995.cn

================================================================================
来源：http://xx.shxzukj.cn

[K01] 对象转 JSON 字符串
来源：http://pv.shxzukj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ud.colortex.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://gt.hahajie.cn

JS:   JSON.stringify(obj)
来源：http://ti.haigaiapp.cn

TS:   JSON.stringify(obj)
来源：http://nd.nicolike.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ad.lnxyls.cn

Go:   json.Marshal(obj)
来源：http://ji.jianghongdianzi.cn

Ruby: obj.to_json                                     // require "json"
来源：http://yx.bookmarksfly.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://nz.shxzukj.cn

[K02] JSON 字符串转对象
来源：http://oi.gzmigu.cn

Py:   json.loads(s)
来源：http://ed.yuntaijiaju.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://rs.jianghongdianzi.cn

JS:   JSON.parse(s)
来源：http://pa.huixinmuqiang.cn

TS:   JSON.parse(s)
来源：http://gu.chemitech.net.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mf.521024.cn

Go:   json.Unmarshal(data, &v)
来源：http://em.panjiajie.cn

Ruby: JSON.parse(s)
来源：http://as.shtwfgs.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://oc.hahajie.cn

[K03] JSON 美化输出（带缩进）
来源：http://qa.newstarts.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mu.asd995.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ha.huixinmuqiang.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://kk.newstarts.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://da.newstarts.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://es.lnxyls.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hu.lnxyls.cn

Ruby: JSON.pretty_generate(obj)
来源：http://rs.huanxung.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hm.bjjhwx.cn

[K04] 读取 JSON 文件
来源：http://ww.asd995.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://bu.yuntaijiaju.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wp.colortex.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://et.asd995.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wk.colortex.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://lj.huixinmuqiang.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mw.huixiangedu.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://jc.shxzskj.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ak.shxzskj.cn

[K05] 深拷贝对象
来源：http://cg.haigaiapp.cn

Py:   copy.deepcopy(obj)
来源：http://mv.shxzukj.cn

PHP:  unserialize(serialize($obj));
来源：http://dt.szsharing.cn

JS:   structuredClone(obj)
来源：http://zs.szxytkj.cn

TS:   structuredClone(obj)
来源：http://vx.hnjuh.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://it.asd995.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ad.colortex.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://tn.jianghongdianzi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://nw.asd995.cn

[K06] 解析 URL 查询串
来源：http://jo.muxihuayi.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xl.gzmigu.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://dq.yuntaijiaju.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ur.shxzskj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://op.jctech888.com.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://iy.9csxet.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://bx.yuexingan06.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://zk.panjiajie.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://yb.hahajie.cn

[K07] 进制转换
来源：http://by.shtwfgs.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://jd.haigaiapp.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://qa.hahajie.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://bh.bookmarksfly.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ej.muxihuayi.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://qx.huixinmuqiang.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://qa.haigaiapp.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ns.shxzskj.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://qr.colortex.cn

[K08] 二进制序列化（非 JSON）
来源：http://ip.nszjky.cn

Py:   pickle.dumps(obj)
来源：http://bl.521024.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://nj.9csxet.cn

JS:   v8.serialize(obj)        // Node
来源：http://hq.shxzukj.cn

TS:   v8.serialize(obj)        // Node
来源：http://tz.521024.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mh.9csxet.cn

Go:   encoding/gob
来源：http://lz.9csxet.cn

Ruby: Marshal.dump(obj)
来源：http://fz.gzmigu.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hk.shtwfgs.cn

================================================================================
来源：http://ux.huixiangedu.cn

L. 网络请求
来源：http://vt.huixiangedu.cn

================================================================================
来源：http://uk.muxihuayi.cn

[L01] 发送 GET 请求
来源：http://yp.521024.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://te.huixiangedu.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://sd.huixinmuqiang.cn

JS:   await fetch(url)
来源：http://gs.yuexingan06.cn

TS:   await fetch(url)
来源：http://sy.chemitech.net.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://fn.huixiangedu.cn

Go:   resp, err := http.Get(url)
来源：http://cb.nicolike.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://zz.szsharing.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://zb.huixinmuqiang.cn

[L02] 发送 POST JSON
来源：http://jw.colortex.cn

Py:   requests.post(url, json={"a": 1})
来源：http://nn.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://kr.szxytkj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qb.shtwfgs.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jb.lnxyls.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://lv.lnxyls.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://tl.newstarts.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://pe.chemitech.net.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://pj.hahajie.cn

[L03] 设置自定义请求头
来源：http://ou.asd995.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ey.yuntaijiaju.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ir.yuexingan06.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qf.colortex.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zr.hahajie.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://xh.yuexingan06.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://nf.9csxet.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://bf.yuntaijiaju.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hs.shtwfgs.cn

[L04] 设置超时
来源：http://lu.szxytkj.cn

Py:   requests.get(url, timeout=5)
来源：http://zz.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://je.521024.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://va.huanxung.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xz.wgjwhj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ik.nicolike.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://or.yuntaijiaju.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://rf.jianghongdianzi.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://gp.9csxet.cn

[L05] 上传文件（multipart）
来源：http://vm.panjiajie.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://xi.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ij.gzmigu.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hb.hnjuh.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ua.haigaiapp.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vd.nszjky.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://sh.szxytkj.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wo.shxzskj.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://bu.lnxyls.cn

[L06] 解析响应为 JSON
来源：http://rl.chemitech.net.cn

Py:   resp.json()
来源：http://lb.jianghongdianzi.cn

PHP:  json_decode($body, true);
来源：http://zi.nszjky.cn

JS:   await resp.json()
来源：http://ve.haigaiapp.cn

TS:   await resp.json()
来源：http://qg.bjjhwx.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://bz.jctech888.com.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://gf.bjjhwx.cn

Ruby: JSON.parse(resp.body)
来源：http://sp.jctech888.com.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ct.bjjhwx.cn

[L07] 处理 HTTP 状态码
来源：http://zs.nszjky.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wc.wgjwhj.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://cf.huanxung.cn

JS:   resp.ok;  resp.status
来源：http://ni.yuntaijiaju.cn

TS:   resp.ok;  resp.status
来源：http://qa.asd995.cn

Java: resp.statusCode()
来源：http://bi.asd995.cn

Go:   resp.StatusCode
来源：http://ug.jianghongdianzi.cn

Ruby: resp.code.to_i
来源：http://cd.jianghongdianzi.cn

C#:   (int)resp.StatusCode
来源：http://uz.lnxyls.cn

[L08] 并发请求多个地址
来源：http://ek.panjiajie.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mn.panjiajie.cn

PHP:  curl_multi_init() 系列
来源：http://yr.shxzukj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jj.huixiangedu.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://we.yuntaijiaju.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://lo.szsharing.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ae.521024.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://kf.nszjky.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://zj.hahajie.cn

================================================================================
来源：http://fa.bjjhwx.cn

M. 命令行 / 进程 / 环境
来源：http://fa.shxzskj.cn

================================================================================
来源：http://iq.huanxung.cn

[M01] 读取命令行参数
来源：http://zs.szsharing.cn

Py:   sys.argv[1:]
来源：http://rs.521024.cn

PHP:  $argv;  $argc;
来源：http://gy.huixinmuqiang.cn

JS:   process.argv.slice(2)
来源：http://il.muxihuayi.cn

TS:   process.argv.slice(2)
来源：http://zc.haigaiapp.cn

Java: args 数组（main 方法参数）
来源：http://iu.shxzukj.cn

Go:   os.Args[1:]
来源：http://ks.jianghongdianzi.cn

Ruby: ARGV
来源：http://wf.shxzukj.cn

C#:   args 数组（Main 方法参数）
来源：http://yu.szsharing.cn

[M02] 读取环境变量
来源：http://zb.huixinmuqiang.cn

Py:   os.environ.get("HOME")
来源：http://kb.colortex.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://va.colortex.cn

JS:   process.env.HOME
来源：http://if.huanxung.cn

TS:   process.env.HOME
来源：http://lv.lnxyls.cn

Java: System.getenv("HOME")
来源：http://hv.asd995.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://bo.bjjhwx.cn

Ruby: ENV["HOME"]
来源：http://we.chemitech.net.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://qu.shxzskj.cn

[M03] 执行外部命令
来源：http://xp.haigaiapp.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://cv.shxzukj.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ym.nszjky.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://xd.szxytkj.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://nz.panjiajie.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://kk.huixiangedu.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://nf.shxzukj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://yl.haigaiapp.cn

C#:   Process.Start("ls", "-l");
来源：http://bn.shxzukj.cn

[M04] 获取当前工作目录
来源：http://hf.huanxung.cn

Py:   os.getcwd()
来源：http://vf.szsharing.cn

PHP:  getcwd();
来源：http://lq.nicolike.cn

JS:   process.cwd()
来源：http://td.yuexingan06.cn

TS:   process.cwd()
来源：http://qg.chemitech.net.cn

Java: Path.of("").toAbsolutePath()
来源：http://py.yuexingan06.cn

Go:   os.Getwd()
来源：http://uy.nicolike.cn

Ruby: Dir.pwd
来源：http://oz.9csxet.cn

C#:   Directory.GetCurrentDirectory()
来源：http://sk.asd995.cn

[M05] 设置退出码
来源：http://tm.colortex.cn

Py:   sys.exit(1)
来源：http://en.asd995.cn

PHP:  exit(1);
来源：http://kt.hahajie.cn

JS:   process.exit(1)
来源：http://cu.shtwfgs.cn

TS:   process.exit(1)
来源：http://es.haigaiapp.cn

Java: System.exit(1)
来源：http://kj.shxzukj.cn

Go:   os.Exit(1)
来源：http://jj.chemitech.net.cn

Ruby: exit 1
来源：http://sy.hnjuh.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://qc.shtwfgs.cn

[M06] 向标准错误输出
来源：http://ib.yuntaijiaju.cn

Py:   print("err", file=sys.stderr)
来源：http://uv.521024.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://aj.jctech888.com.cn

JS:   console.error("err")
来源：http://it.szsharing.cn

TS:   console.error("err")
来源：http://uz.chemitech.net.cn

Java: System.err.println("err")
来源：http://rm.szsharing.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://fg.chemitech.net.cn

Ruby: warn "err"
来源：http://vy.muxihuayi.cn

C#:   Console.Error.WriteLine("err")
来源：http://xp.newstarts.cn

[M07] 判断是否为主入口
来源：http://gt.huanxung.cn

Py:   if __name__ == "__main__":
来源：http://px.huixinmuqiang.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ur.shxzukj.cn

JS:   require.main === module
来源：http://qk.wgjwhj.cn

TS:   require.main === module
来源：http://tv.hahajie.cn

Java: public static void main(String[] args)
来源：http://nd.shxzukj.cn

Go:   func main()
来源：http://pw.jianghongdianzi.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://sw.shtwfgs.cn

C#:   static void Main(string[] args)
来源：http://qa.nicolike.cn

[M08] 获取系统与运行时信息
来源：http://ab.panjiajie.cn

Py:   platform.system();  platform.python_version()
来源：http://ql.asd995.cn

PHP:  PHP_OS;  phpversion();
来源：http://rq.bjjhwx.cn

JS:   process.platform;  process.version
来源：http://uf.wgjwhj.cn

TS:   process.platform;  process.version
来源：http://tx.szsharing.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://aj.colortex.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://mt.521024.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://lj.wgjwhj.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://of.hnjuh.cn

================================================================================
来源：http://ib.panjiajie.cn

N. 数据结构与算法
来源：http://hs.muxihuayi.cn

================================================================================
来源：http://sk.nszjky.cn

[N01] 二分查找（有序数组）
来源：http://ya.panjiajie.cn

Py:   bisect.bisect_left(arr, x)
来源：http://dm.bjjhwx.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://di.huanxung.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zv.nicolike.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xt.bjjhwx.cn

Java: Arrays.binarySearch(arr, x)
来源：http://wv.nicolike.cn

Go:   sort.SearchInts(arr, x)
来源：http://my.bjjhwx.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://dq.yuntaijiaju.cn

C#:   Array.BinarySearch(arr, x)
来源：http://tc.bjjhwx.cn

[N02] 排序（工程实践用内置实现）
来源：http://yr.shtwfgs.cn

Py:   sorted(arr);  arr.sort()
来源：http://gl.shxzukj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://yt.nszjky.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://kj.szsharing.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://dc.huixinmuqiang.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ru.asd995.cn

Go:   slices.Sort(arr)
来源：http://wa.newstarts.cn

Ruby: arr.sort
来源：http://wv.bjjhwx.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://tb.lnxyls.cn

[N03] 快速排序（分治示例）
来源：http://dh.bjjhwx.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mm.jianghongdianzi.cn

PHP:  // 递归实现，或用 usort
来源：http://ln.newstarts.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bp.huixiangedu.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xf.bookmarksfly.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://cy.chemitech.net.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://xt.colortex.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://da.hnjuh.cn

C#:   // 手写递归，或 Array.Sort
来源：http://yv.szxytkj.cn

[N04] 斐波那契数列
来源：http://oe.yuexingan06.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://nq.asd995.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ax.hahajie.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hv.shxzukj.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xq.9csxet.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://xn.huixinmuqiang.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://kc.muxihuayi.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ud.bookmarksfly.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://so.bjjhwx.cn

[N05] 最大公约数
来源：http://fo.colortex.cn

Py:   math.gcd(a, b)
来源：http://kj.bjjhwx.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://he.huixiangedu.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ci.szxytkj.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://op.yuntaijiaju.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ak.shxzskj.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ao.lnxyls.cn

Ruby: a.gcd(b)
来源：http://cd.yuntaijiaju.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hc.jianghongdianzi.cn

[N06] 判断回文字符串
来源：http://mi.colortex.cn

Py:   s == s[::-1]
来源：http://kz.haigaiapp.cn

PHP:  $s === strrev($s);
来源：http://vp.chemitech.net.cn

JS:   s === [...s].reverse().join("")
来源：http://fq.muxihuayi.cn

TS:   s === [...s].reverse().join("")
来源：http://gy.hnjuh.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://gu.shtwfgs.cn

Go:   // 双指针从两端比较
来源：http://gs.lnxyls.cn

Ruby: s == s.reverse
来源：http://ex.bookmarksfly.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://sb.gzmigu.cn

[N07] 两数之和（返回下标）
来源：http://dl.521024.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ox.shxzskj.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ro.asd995.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://zp.shtwfgs.cn

TS:   // 手写 Map<string, number>
来源：http://lt.shxzskj.cn

Java: // 手写 HashMap
来源：http://mu.hnjuh.cn


<!-- 参考信息 -->