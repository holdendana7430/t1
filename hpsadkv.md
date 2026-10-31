代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://go.bookmarksfly.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://hm.huixiangedu.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ay.lnxyls.cn

[J10] 取今天 / 本月第一天
来源：http://pq.huanxung.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://aw.huixiangedu.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://tq.shtwfgs.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qo.shxzskj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://yv.hnjuh.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mi.bookmarksfly.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://kb.shtwfgs.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vg.hnjuh.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://qw.colortex.cn

================================================================================
来源：http://bh.shtwfgs.cn

K. JSON 与序列化
来源：http://rl.panjiajie.cn

================================================================================
来源：http://ch.lnxyls.cn

[K01] 对象转 JSON 字符串
来源：http://od.nicolike.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hd.asd995.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ii.nicolike.cn

JS:   JSON.stringify(obj)
来源：http://bo.jianghongdianzi.cn

TS:   JSON.stringify(obj)
来源：http://pp.huixinmuqiang.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ps.wgjwhj.cn

Go:   json.Marshal(obj)
来源：http://ty.nicolike.cn

Ruby: obj.to_json                                     // require "json"
来源：http://jz.9csxet.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://zv.muxihuayi.cn

[K02] JSON 字符串转对象
来源：http://xx.gzmigu.cn

Py:   json.loads(s)
来源：http://bq.bjjhwx.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://cz.yuexingan06.cn

JS:   JSON.parse(s)
来源：http://cp.jctech888.com.cn

TS:   JSON.parse(s)
来源：http://ch.lnxyls.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://sg.yuntaijiaju.cn

Go:   json.Unmarshal(data, &v)
来源：http://lt.shxzskj.cn

Ruby: JSON.parse(s)
来源：http://iq.lnxyls.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zy.521024.cn

[K03] JSON 美化输出（带缩进）
来源：http://qc.hnjuh.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://da.muxihuayi.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ym.jianghongdianzi.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://gs.shxzskj.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://xk.huixiangedu.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ac.nszjky.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://fo.bjjhwx.cn

Ruby: JSON.pretty_generate(obj)
来源：http://nh.9csxet.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://jo.haigaiapp.cn

[K04] 读取 JSON 文件
来源：http://kh.gzmigu.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ak.wgjwhj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://dk.jianghongdianzi.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vl.huixiangedu.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bd.521024.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ly.huanxung.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ts.hnjuh.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://iz.shtwfgs.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wk.bjjhwx.cn

[K05] 深拷贝对象
来源：http://ku.newstarts.cn

Py:   copy.deepcopy(obj)
来源：http://vy.jctech888.com.cn

PHP:  unserialize(serialize($obj));
来源：http://ls.wgjwhj.cn

JS:   structuredClone(obj)
来源：http://gz.jctech888.com.cn

TS:   structuredClone(obj)
来源：http://rw.huanxung.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://hf.bjjhwx.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ue.huanxung.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://qk.newstarts.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://mq.szsharing.cn

[K06] 解析 URL 查询串
来源：http://iu.jianghongdianzi.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ev.bjjhwx.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://el.shxzukj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rz.asd995.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xm.nicolike.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://kx.szxytkj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://je.nszjky.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://te.huanxung.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://og.chemitech.net.cn

[K07] 进制转换
来源：http://gx.9csxet.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://pi.9csxet.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://tk.lnxyls.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ez.asd995.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://lc.newstarts.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mp.panjiajie.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://fe.chemitech.net.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://gz.nszjky.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://sm.colortex.cn

[K08] 二进制序列化（非 JSON）
来源：http://il.nicolike.cn

Py:   pickle.dumps(obj)
来源：http://xq.yuntaijiaju.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://lf.asd995.cn

JS:   v8.serialize(obj)        // Node
来源：http://zu.asd995.cn

TS:   v8.serialize(obj)        // Node
来源：http://zl.521024.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://db.colortex.cn

Go:   encoding/gob
来源：http://ln.jctech888.com.cn

Ruby: Marshal.dump(obj)
来源：http://tz.szsharing.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://jf.asd995.cn

================================================================================
来源：http://ju.hahajie.cn

L. 网络请求
来源：http://ew.shxzskj.cn

================================================================================
来源：http://gy.gzmigu.cn

[L01] 发送 GET 请求
来源：http://cq.gzmigu.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://uy.colortex.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://yv.hahajie.cn

JS:   await fetch(url)
来源：http://ef.bjjhwx.cn

TS:   await fetch(url)
来源：http://uc.muxihuayi.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://fo.huixiangedu.cn

Go:   resp, err := http.Get(url)
来源：http://sc.szsharing.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://zu.nszjky.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://fn.gzmigu.cn

[L02] 发送 POST JSON
来源：http://lv.shtwfgs.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ya.panjiajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://uk.9csxet.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xc.szxytkj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ne.jctech888.com.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://th.szsharing.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://xr.nszjky.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://cb.bjjhwx.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://gw.szxytkj.cn

[L03] 设置自定义请求头
来源：http://zd.hahajie.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://se.szsharing.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hx.asd995.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://of.panjiajie.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wd.chemitech.net.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://zk.shxzukj.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://rx.huixiangedu.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qb.hnjuh.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://qv.521024.cn

[L04] 设置超时
来源：http://af.muxihuayi.cn

Py:   requests.get(url, timeout=5)
来源：http://ve.szsharing.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ba.bjjhwx.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dl.panjiajie.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ib.huixiangedu.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://xt.hahajie.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://qa.jianghongdianzi.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://jf.colortex.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://en.colortex.cn

[L05] 上传文件（multipart）
来源：http://wg.wgjwhj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zq.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://qx.yuexingan06.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hb.huanxung.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://kq.hahajie.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://fy.shtwfgs.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://dq.yuntaijiaju.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://gz.521024.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ip.muxihuayi.cn

[L06] 解析响应为 JSON
来源：http://ti.bookmarksfly.cn

Py:   resp.json()
来源：http://xo.szxytkj.cn

PHP:  json_decode($body, true);
来源：http://sd.yuexingan06.cn

JS:   await resp.json()
来源：http://jk.521024.cn

TS:   await resp.json()
来源：http://yc.yuexingan06.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://xa.haigaiapp.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ad.shtwfgs.cn

Ruby: JSON.parse(resp.body)
来源：http://ti.shxzukj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://uh.shtwfgs.cn

[L07] 处理 HTTP 状态码
来源：http://to.wgjwhj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://kb.panjiajie.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://fc.hahajie.cn

JS:   resp.ok;  resp.status
来源：http://em.shxzukj.cn

TS:   resp.ok;  resp.status
来源：http://xw.shxzukj.cn

Java: resp.statusCode()
来源：http://dd.bookmarksfly.cn

Go:   resp.StatusCode
来源：http://bv.szxytkj.cn

Ruby: resp.code.to_i
来源：http://lz.shxzskj.cn

C#:   (int)resp.StatusCode
来源：http://kb.bjjhwx.cn

[L08] 并发请求多个地址
来源：http://ry.muxihuayi.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://lt.huixiangedu.cn

PHP:  curl_multi_init() 系列
来源：http://lv.gzmigu.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yc.hnjuh.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ba.shxzskj.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://gy.panjiajie.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://oo.shxzskj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://rj.huanxung.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://he.hahajie.cn

================================================================================
来源：http://kc.lnxyls.cn

M. 命令行 / 进程 / 环境
来源：http://ka.shxzskj.cn

================================================================================
来源：http://ls.muxihuayi.cn

[M01] 读取命令行参数
来源：http://sd.huanxung.cn

Py:   sys.argv[1:]
来源：http://kd.asd995.cn

PHP:  $argv;  $argc;
来源：http://wr.lnxyls.cn

JS:   process.argv.slice(2)
来源：http://fv.521024.cn

TS:   process.argv.slice(2)
来源：http://ke.yuntaijiaju.cn

Java: args 数组（main 方法参数）
来源：http://xb.panjiajie.cn

Go:   os.Args[1:]
来源：http://aq.bjjhwx.cn

Ruby: ARGV
来源：http://hw.chemitech.net.cn

C#:   args 数组（Main 方法参数）
来源：http://uf.shxzukj.cn

[M02] 读取环境变量
来源：http://xs.hnjuh.cn

Py:   os.environ.get("HOME")
来源：http://um.jctech888.com.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://li.hahajie.cn

JS:   process.env.HOME
来源：http://bg.asd995.cn

TS:   process.env.HOME
来源：http://xy.muxihuayi.cn

Java: System.getenv("HOME")
来源：http://ok.jianghongdianzi.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://pc.yuexingan06.cn

Ruby: ENV["HOME"]
来源：http://wz.jctech888.com.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ku.yuntaijiaju.cn

[M03] 执行外部命令
来源：http://bd.shxzukj.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://fw.hnjuh.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://vs.shtwfgs.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://vs.muxihuayi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://wt.asd995.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://it.huanxung.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://sg.nszjky.cn

Ruby: system("ls -l");  `ls -l`
来源：http://py.nszjky.cn

C#:   Process.Start("ls", "-l");
来源：http://xr.haigaiapp.cn

[M04] 获取当前工作目录
来源：http://jq.jianghongdianzi.cn

Py:   os.getcwd()
来源：http://rs.gzmigu.cn

PHP:  getcwd();
来源：http://ce.wgjwhj.cn

JS:   process.cwd()
来源：http://os.szsharing.cn

TS:   process.cwd()
来源：http://io.huixiangedu.cn

Java: Path.of("").toAbsolutePath()
来源：http://in.shtwfgs.cn

Go:   os.Getwd()
来源：http://bm.hnjuh.cn

Ruby: Dir.pwd
来源：http://vi.colortex.cn

C#:   Directory.GetCurrentDirectory()
来源：http://vu.nicolike.cn

[M05] 设置退出码
来源：http://sm.nicolike.cn

Py:   sys.exit(1)
来源：http://xa.hahajie.cn

PHP:  exit(1);
来源：http://mi.shxzskj.cn

JS:   process.exit(1)
来源：http://un.shxzskj.cn

TS:   process.exit(1)
来源：http://td.newstarts.cn

Java: System.exit(1)
来源：http://mo.haigaiapp.cn

Go:   os.Exit(1)
来源：http://mr.yuexingan06.cn

Ruby: exit 1
来源：http://zy.9csxet.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://va.hnjuh.cn

[M06] 向标准错误输出
来源：http://hf.huixinmuqiang.cn

Py:   print("err", file=sys.stderr)
来源：http://jk.asd995.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://qy.yuexingan06.cn

JS:   console.error("err")
来源：http://gg.asd995.cn

TS:   console.error("err")
来源：http://mf.lnxyls.cn

Java: System.err.println("err")
来源：http://gw.huanxung.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://qm.nszjky.cn

Ruby: warn "err"
来源：http://hy.9csxet.cn

C#:   Console.Error.WriteLine("err")
来源：http://ib.hnjuh.cn

[M07] 判断是否为主入口
来源：http://ct.chemitech.net.cn

Py:   if __name__ == "__main__":
来源：http://zn.wgjwhj.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://bn.huanxung.cn

JS:   require.main === module
来源：http://ub.nszjky.cn

TS:   require.main === module
来源：http://ex.newstarts.cn

Java: public static void main(String[] args)
来源：http://oa.haigaiapp.cn

Go:   func main()
来源：http://vg.szsharing.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://co.chemitech.net.cn

C#:   static void Main(string[] args)
来源：http://hz.gzmigu.cn

[M08] 获取系统与运行时信息
来源：http://ii.shxzukj.cn

Py:   platform.system();  platform.python_version()
来源：http://cl.asd995.cn

PHP:  PHP_OS;  phpversion();
来源：http://ms.haigaiapp.cn

JS:   process.platform;  process.version
来源：http://aw.shxzskj.cn

TS:   process.platform;  process.version
来源：http://om.newstarts.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://dm.hahajie.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://zf.shxzukj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://zt.colortex.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://mi.panjiajie.cn

================================================================================
来源：http://zu.wgjwhj.cn

N. 数据结构与算法
来源：http://nu.hnjuh.cn

================================================================================
来源：http://uj.shxzukj.cn

[N01] 二分查找（有序数组）
来源：http://kx.haigaiapp.cn

Py:   bisect.bisect_left(arr, x)
来源：http://en.muxihuayi.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wi.yuntaijiaju.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cz.nicolike.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://un.shxzskj.cn

Java: Arrays.binarySearch(arr, x)
来源：http://zn.wgjwhj.cn

Go:   sort.SearchInts(arr, x)
来源：http://dq.shxzukj.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://sk.hnjuh.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ry.nicolike.cn

[N02] 排序（工程实践用内置实现）
来源：http://uw.bookmarksfly.cn

Py:   sorted(arr);  arr.sort()
来源：http://hc.szsharing.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hp.chemitech.net.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://gi.jianghongdianzi.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://uv.hnjuh.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ez.muxihuayi.cn

Go:   slices.Sort(arr)
来源：http://ep.newstarts.cn

Ruby: arr.sort
来源：http://oc.shxzukj.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://gv.asd995.cn

[N03] 快速排序（分治示例）
来源：http://al.yuntaijiaju.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://kg.huixinmuqiang.cn

PHP:  // 递归实现，或用 usort
来源：http://xc.panjiajie.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hs.szxytkj.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ht.shxzskj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ap.hahajie.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://dc.shxzskj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://st.shxzukj.cn

C#:   // 手写递归，或 Array.Sort
来源：http://fd.shtwfgs.cn

[N04] 斐波那契数列
来源：http://so.yuexingan06.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://si.huixiangedu.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://cz.panjiajie.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://la.szxytkj.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bj.newstarts.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://qd.nicolike.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://tp.yuexingan06.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ys.bookmarksfly.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://da.asd995.cn

[N05] 最大公约数
来源：http://em.szsharing.cn

Py:   math.gcd(a, b)
来源：http://ct.bookmarksfly.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://zm.521024.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ue.jianghongdianzi.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qg.asd995.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://fg.hahajie.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ra.lnxyls.cn

Ruby: a.gcd(b)
来源：http://mz.colortex.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mm.shxzukj.cn

[N06] 判断回文字符串
来源：http://oc.colortex.cn

Py:   s == s[::-1]
来源：http://ov.panjiajie.cn

PHP:  $s === strrev($s);
来源：http://wb.nicolike.cn

JS:   s === [...s].reverse().join("")
来源：http://aa.chemitech.net.cn

TS:   s === [...s].reverse().join("")
来源：http://ul.yuexingan06.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xs.huixiangedu.cn

Go:   // 双指针从两端比较
来源：http://oo.huanxung.cn

Ruby: s == s.reverse
来源：http://dg.jianghongdianzi.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://dk.haigaiapp.cn

[N07] 两数之和（返回下标）
来源：http://di.hnjuh.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ap.wgjwhj.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://eb.nszjky.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://vl.colortex.cn

TS:   // 手写 Map<string, number>
来源：http://ql.521024.cn

Java: // 手写 HashMap
来源：http://sr.szxytkj.cn


<!-- 参考信息 -->