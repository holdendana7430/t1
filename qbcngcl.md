代发 wailian999

Py:   date.today();  date.today().replace(day=1)
来源：http://hr.panjiajie.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://jo.chemitech.net.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ib.shtwfgs.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ms.shtwfgs.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://oc.hahajie.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://rg.huanxung.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://tm.jianghongdianzi.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://yb.gzmigu.cn

================================================================================
来源：http://lk.wgjwhj.cn

K. JSON 与序列化
来源：http://vc.shxzukj.cn

================================================================================
来源：http://fm.shxzskj.cn

[K01] 对象转 JSON 字符串
来源：http://fj.hahajie.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://or.9csxet.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://nq.panjiajie.cn

JS:   JSON.stringify(obj)
来源：http://pc.asd995.cn

TS:   JSON.stringify(obj)
来源：http://ek.hnjuh.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://cm.panjiajie.cn

Go:   json.Marshal(obj)
来源：http://ve.nszjky.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ci.muxihuayi.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://al.gzmigu.cn

[K02] JSON 字符串转对象
来源：http://as.nszjky.cn

Py:   json.loads(s)
来源：http://pm.jianghongdianzi.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://fm.szxytkj.cn

JS:   JSON.parse(s)
来源：http://gx.asd995.cn

TS:   JSON.parse(s)
来源：http://de.haigaiapp.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://xp.szxytkj.cn

Go:   json.Unmarshal(data, &v)
来源：http://in.nicolike.cn

Ruby: JSON.parse(s)
来源：http://nl.yuexingan06.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hi.nszjky.cn

[K03] JSON 美化输出（带缩进）
来源：http://vy.colortex.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://zx.asd995.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://zd.chemitech.net.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ys.huanxung.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ht.jianghongdianzi.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://le.szsharing.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://gn.haigaiapp.cn

Ruby: JSON.pretty_generate(obj)
来源：http://hh.shxzukj.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://fo.bjjhwx.cn

[K04] 读取 JSON 文件
来源：http://ni.hahajie.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jk.nicolike.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wl.yuntaijiaju.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gd.muxihuayi.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vz.huixinmuqiang.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mi.shxzskj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://cv.521024.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://tc.muxihuayi.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://nz.9csxet.cn

[K05] 深拷贝对象
来源：http://kh.szsharing.cn

Py:   copy.deepcopy(obj)
来源：http://pi.shxzskj.cn

PHP:  unserialize(serialize($obj));
来源：http://si.chemitech.net.cn

JS:   structuredClone(obj)
来源：http://rv.haigaiapp.cn

TS:   structuredClone(obj)
来源：http://bz.shxzukj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://tl.yuexingan06.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://jv.lnxyls.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ll.jianghongdianzi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ci.nicolike.cn

[K06] 解析 URL 查询串
来源：http://ru.bookmarksfly.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://cc.muxihuayi.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://po.huanxung.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hh.bookmarksfly.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uu.shxzukj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mg.nszjky.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ff.nszjky.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://pm.huanxung.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://dd.yuexingan06.cn

[K07] 进制转换
来源：http://yd.huixiangedu.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://vf.szsharing.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://pq.yuntaijiaju.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://uj.asd995.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://au.lnxyls.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://gx.haigaiapp.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://yi.bjjhwx.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://no.szsharing.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://en.chemitech.net.cn

[K08] 二进制序列化（非 JSON）
来源：http://rj.shxzukj.cn

Py:   pickle.dumps(obj)
来源：http://iu.shxzskj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://lg.wgjwhj.cn

JS:   v8.serialize(obj)        // Node
来源：http://ar.lnxyls.cn

TS:   v8.serialize(obj)        // Node
来源：http://an.haigaiapp.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://eu.yuexingan06.cn

Go:   encoding/gob
来源：http://yq.huixiangedu.cn

Ruby: Marshal.dump(obj)
来源：http://xs.bookmarksfly.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wn.bjjhwx.cn

================================================================================
来源：http://lx.huixinmuqiang.cn

L. 网络请求
来源：http://pp.newstarts.cn

================================================================================
来源：http://cn.huixinmuqiang.cn

[L01] 发送 GET 请求
来源：http://jj.muxihuayi.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wu.colortex.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://dd.huanxung.cn

JS:   await fetch(url)
来源：http://gx.panjiajie.cn

TS:   await fetch(url)
来源：http://le.bjjhwx.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://sy.jctech888.com.cn

Go:   resp, err := http.Get(url)
来源：http://hs.szxytkj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://sp.haigaiapp.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://xw.jianghongdianzi.cn

[L02] 发送 POST JSON
来源：http://sp.colortex.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ne.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hf.panjiajie.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dy.shtwfgs.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kb.9csxet.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://tn.yuntaijiaju.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ut.9csxet.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://nf.muxihuayi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ap.gzmigu.cn

[L03] 设置自定义请求头
来源：http://se.521024.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://nu.szsharing.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://xx.gzmigu.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kl.panjiajie.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xe.jctech888.com.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://bh.bjjhwx.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://vf.jctech888.com.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://do.newstarts.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://at.bookmarksfly.cn

[L04] 设置超时
来源：http://cr.lnxyls.cn

Py:   requests.get(url, timeout=5)
来源：http://gf.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://kl.bookmarksfly.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://av.huixinmuqiang.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yu.shtwfgs.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://sn.nicolike.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ox.jianghongdianzi.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://vu.9csxet.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://re.shxzskj.cn

[L05] 上传文件（multipart）
来源：http://io.jctech888.com.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ld.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://bz.szxytkj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ay.9csxet.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ep.yuexingan06.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://bd.nicolike.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://pp.yuntaijiaju.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://us.szxytkj.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://la.szxytkj.cn

[L06] 解析响应为 JSON
来源：http://tt.chemitech.net.cn

Py:   resp.json()
来源：http://xn.hnjuh.cn

PHP:  json_decode($body, true);
来源：http://ss.muxihuayi.cn

JS:   await resp.json()
来源：http://pg.lnxyls.cn

TS:   await resp.json()
来源：http://uy.jianghongdianzi.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://zn.szsharing.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://es.bjjhwx.cn

Ruby: JSON.parse(resp.body)
来源：http://ef.colortex.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://sn.bookmarksfly.cn

[L07] 处理 HTTP 状态码
来源：http://fe.huanxung.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ki.nicolike.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://fc.szsharing.cn

JS:   resp.ok;  resp.status
来源：http://pj.haigaiapp.cn

TS:   resp.ok;  resp.status
来源：http://nw.panjiajie.cn

Java: resp.statusCode()
来源：http://fh.muxihuayi.cn

Go:   resp.StatusCode
来源：http://yz.muxihuayi.cn

Ruby: resp.code.to_i
来源：http://pm.9csxet.cn

C#:   (int)resp.StatusCode
来源：http://jr.521024.cn

[L08] 并发请求多个地址
来源：http://ed.colortex.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://kh.panjiajie.cn

PHP:  curl_multi_init() 系列
来源：http://tp.wgjwhj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://co.asd995.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sd.shxzukj.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ed.lnxyls.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://gy.muxihuayi.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://tv.asd995.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://jw.szsharing.cn

================================================================================
来源：http://ux.huixinmuqiang.cn

M. 命令行 / 进程 / 环境
来源：http://ri.nszjky.cn

================================================================================
来源：http://dc.jctech888.com.cn

[M01] 读取命令行参数
来源：http://rg.nicolike.cn

Py:   sys.argv[1:]
来源：http://iv.asd995.cn

PHP:  $argv;  $argc;
来源：http://gg.bjjhwx.cn

JS:   process.argv.slice(2)
来源：http://kl.bookmarksfly.cn

TS:   process.argv.slice(2)
来源：http://rx.szxytkj.cn

Java: args 数组（main 方法参数）
来源：http://if.haigaiapp.cn

Go:   os.Args[1:]
来源：http://va.hahajie.cn

Ruby: ARGV
来源：http://ua.newstarts.cn

C#:   args 数组（Main 方法参数）
来源：http://df.panjiajie.cn

[M02] 读取环境变量
来源：http://xt.newstarts.cn

Py:   os.environ.get("HOME")
来源：http://kd.jctech888.com.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://py.newstarts.cn

JS:   process.env.HOME
来源：http://ek.asd995.cn

TS:   process.env.HOME
来源：http://bk.huixinmuqiang.cn

Java: System.getenv("HOME")
来源：http://gg.shxzukj.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://pi.newstarts.cn

Ruby: ENV["HOME"]
来源：http://ko.huixiangedu.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://md.gzmigu.cn

[M03] 执行外部命令
来源：http://dh.nszjky.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://yl.shxzukj.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ug.yuexingan06.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://yc.muxihuayi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://nn.huixinmuqiang.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://dc.lnxyls.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://qz.nszjky.cn

Ruby: system("ls -l");  `ls -l`
来源：http://qw.9csxet.cn

C#:   Process.Start("ls", "-l");
来源：http://hd.szsharing.cn

[M04] 获取当前工作目录
来源：http://gk.jianghongdianzi.cn

Py:   os.getcwd()
来源：http://ft.huanxung.cn

PHP:  getcwd();
来源：http://cd.colortex.cn

JS:   process.cwd()
来源：http://uj.gzmigu.cn

TS:   process.cwd()
来源：http://xa.9csxet.cn

Java: Path.of("").toAbsolutePath()
来源：http://ln.521024.cn

Go:   os.Getwd()
来源：http://ao.shtwfgs.cn

Ruby: Dir.pwd
来源：http://ex.521024.cn

C#:   Directory.GetCurrentDirectory()
来源：http://vm.yuexingan06.cn

[M05] 设置退出码
来源：http://vh.bookmarksfly.cn

Py:   sys.exit(1)
来源：http://lq.shtwfgs.cn

PHP:  exit(1);
来源：http://an.huanxung.cn

JS:   process.exit(1)
来源：http://zm.huixiangedu.cn

TS:   process.exit(1)
来源：http://ov.huixinmuqiang.cn

Java: System.exit(1)
来源：http://eu.newstarts.cn

Go:   os.Exit(1)
来源：http://zy.szsharing.cn

Ruby: exit 1
来源：http://ph.szsharing.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://yl.hnjuh.cn

[M06] 向标准错误输出
来源：http://je.szxytkj.cn

Py:   print("err", file=sys.stderr)
来源：http://wd.shxzukj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://id.bjjhwx.cn

JS:   console.error("err")
来源：http://fe.bookmarksfly.cn

TS:   console.error("err")
来源：http://mo.jctech888.com.cn

Java: System.err.println("err")
来源：http://dm.nszjky.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://kt.hahajie.cn

Ruby: warn "err"
来源：http://ob.gzmigu.cn

C#:   Console.Error.WriteLine("err")
来源：http://yl.yuexingan06.cn

[M07] 判断是否为主入口
来源：http://gs.521024.cn

Py:   if __name__ == "__main__":
来源：http://mo.bookmarksfly.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://zl.lnxyls.cn

JS:   require.main === module
来源：http://dk.gzmigu.cn

TS:   require.main === module
来源：http://yh.jctech888.com.cn

Java: public static void main(String[] args)
来源：http://id.huixiangedu.cn

Go:   func main()
来源：http://hw.hahajie.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://dx.huixinmuqiang.cn

C#:   static void Main(string[] args)
来源：http://ns.newstarts.cn

[M08] 获取系统与运行时信息
来源：http://xy.bookmarksfly.cn

Py:   platform.system();  platform.python_version()
来源：http://jr.hahajie.cn

PHP:  PHP_OS;  phpversion();
来源：http://lv.9csxet.cn

JS:   process.platform;  process.version
来源：http://cu.asd995.cn

TS:   process.platform;  process.version
来源：http://mx.wgjwhj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://vj.shtwfgs.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://jp.huanxung.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://fg.shxzskj.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://dw.huanxung.cn

================================================================================
来源：http://zt.szxytkj.cn

N. 数据结构与算法
来源：http://vp.yuntaijiaju.cn

================================================================================
来源：http://ea.bookmarksfly.cn

[N01] 二分查找（有序数组）
来源：http://er.nszjky.cn

Py:   bisect.bisect_left(arr, x)
来源：http://vw.shtwfgs.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://vj.bjjhwx.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ei.bjjhwx.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xa.nszjky.cn

Java: Arrays.binarySearch(arr, x)
来源：http://pw.muxihuayi.cn

Go:   sort.SearchInts(arr, x)
来源：http://dw.chemitech.net.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://sw.huanxung.cn

C#:   Array.BinarySearch(arr, x)
来源：http://az.521024.cn

[N02] 排序（工程实践用内置实现）
来源：http://kb.panjiajie.cn

Py:   sorted(arr);  arr.sort()
来源：http://sz.haigaiapp.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://iu.panjiajie.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://fw.szxytkj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://xo.colortex.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://vg.panjiajie.cn

Go:   slices.Sort(arr)
来源：http://lb.hnjuh.cn

Ruby: arr.sort
来源：http://nv.wgjwhj.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://dt.hahajie.cn

[N03] 快速排序（分治示例）
来源：http://pi.521024.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ov.asd995.cn

PHP:  // 递归实现，或用 usort
来源：http://xe.newstarts.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nd.hnjuh.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qc.bookmarksfly.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ip.huanxung.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://fl.szsharing.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://pf.colortex.cn

C#:   // 手写递归，或 Array.Sort
来源：http://tu.bjjhwx.cn

[N04] 斐波那契数列
来源：http://qx.shxzskj.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://sz.yuexingan06.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ne.gzmigu.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bb.shtwfgs.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ft.asd995.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://bx.shxzukj.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ar.muxihuayi.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://pw.huixinmuqiang.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://xt.jctech888.com.cn

[N05] 最大公约数
来源：http://mm.huixinmuqiang.cn

Py:   math.gcd(a, b)
来源：http://bm.wgjwhj.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://lo.hahajie.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gn.asd995.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wt.wgjwhj.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wn.nicolike.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hk.gzmigu.cn

Ruby: a.gcd(b)
来源：http://sq.huanxung.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://dh.yuntaijiaju.cn

[N06] 判断回文字符串
来源：http://fh.bjjhwx.cn

Py:   s == s[::-1]
来源：http://ec.hahajie.cn

PHP:  $s === strrev($s);
来源：http://tg.szsharing.cn

JS:   s === [...s].reverse().join("")
来源：http://ol.gzmigu.cn

TS:   s === [...s].reverse().join("")
来源：http://yf.jianghongdianzi.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://zc.hahajie.cn

Go:   // 双指针从两端比较
来源：http://kl.shxzukj.cn

Ruby: s == s.reverse
来源：http://wr.nszjky.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://pz.shxzskj.cn

[N07] 两数之和（返回下标）
来源：http://xx.jctech888.com.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ww.hahajie.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://rn.asd995.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://nj.muxihuayi.cn

TS:   // 手写 Map<string, number>
来源：http://wh.shxzukj.cn

Java: // 手写 HashMap
来源：http://np.yuexingan06.cn

Go:   // 手写 map[int]int
来源：http://pc.lnxyls.cn

Ruby: // 手写 Hash
来源：http://mw.szsharing.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ev.nicolike.cn

[N08] 生成全排列
来源：http://or.huixinmuqiang.cn


<!-- 参考信息 -->