代发 wailian999

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://bz.9csxet.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://pj.huixinmuqiang.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://jo.gzmigu.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://gf.9csxet.cn

================================================================================
来源：http://iq.9csxet.cn

K. JSON 与序列化
来源：http://ia.newstarts.cn

================================================================================
来源：http://ur.gzmigu.cn

[K01] 对象转 JSON 字符串
来源：http://qp.hahajie.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://bg.hnjuh.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://bk.shxzskj.cn

JS:   JSON.stringify(obj)
来源：http://hz.colortex.cn

TS:   JSON.stringify(obj)
来源：http://aq.jianghongdianzi.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://rm.9csxet.cn

Go:   json.Marshal(obj)
来源：http://jt.yuntaijiaju.cn

Ruby: obj.to_json                                     // require "json"
来源：http://vq.hahajie.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://lt.nicolike.cn

[K02] JSON 字符串转对象
来源：http://jh.asd995.cn

Py:   json.loads(s)
来源：http://ag.nicolike.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://xg.nszjky.cn

JS:   JSON.parse(s)
来源：http://uv.shxzskj.cn

TS:   JSON.parse(s)
来源：http://il.yuntaijiaju.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ov.jctech888.com.cn

Go:   json.Unmarshal(data, &v)
来源：http://px.nszjky.cn

Ruby: JSON.parse(s)
来源：http://wh.huixiangedu.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://bw.newstarts.cn

[K03] JSON 美化输出（带缩进）
来源：http://sa.nicolike.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://oy.colortex.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qa.lnxyls.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://yg.bjjhwx.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://oj.yuntaijiaju.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://rl.hnjuh.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mb.szsharing.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ad.wgjwhj.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://qb.szxytkj.cn

[K04] 读取 JSON 文件
来源：http://lx.huixiangedu.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://lw.newstarts.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://zs.muxihuayi.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dt.9csxet.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kz.huixinmuqiang.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://nf.panjiajie.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://nc.newstarts.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ec.nicolike.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://zj.jctech888.com.cn

[K05] 深拷贝对象
来源：http://bl.huanxung.cn

Py:   copy.deepcopy(obj)
来源：http://ed.huixiangedu.cn

PHP:  unserialize(serialize($obj));
来源：http://bj.panjiajie.cn

JS:   structuredClone(obj)
来源：http://jy.yuntaijiaju.cn

TS:   structuredClone(obj)
来源：http://pz.szsharing.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://oi.szsharing.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wt.haigaiapp.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://dt.jianghongdianzi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://qz.asd995.cn

[K06] 解析 URL 查询串
来源：http://eh.shxzskj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rd.shtwfgs.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://kp.yuntaijiaju.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dm.521024.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zj.nicolike.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://xr.521024.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://cm.muxihuayi.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://sj.asd995.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hh.yuntaijiaju.cn

[K07] 进制转换
来源：http://pe.hahajie.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://di.nicolike.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://nn.szxytkj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://jd.bjjhwx.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://xs.newstarts.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://cg.huixinmuqiang.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ca.9csxet.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ll.huanxung.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://lb.huanxung.cn

[K08] 二进制序列化（非 JSON）
来源：http://qq.jctech888.com.cn

Py:   pickle.dumps(obj)
来源：http://sw.huixiangedu.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://yd.colortex.cn

JS:   v8.serialize(obj)        // Node
来源：http://mg.nicolike.cn

TS:   v8.serialize(obj)        // Node
来源：http://ae.yuexingan06.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://cf.wgjwhj.cn

Go:   encoding/gob
来源：http://io.521024.cn

Ruby: Marshal.dump(obj)
来源：http://ev.szxytkj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://cd.hnjuh.cn

================================================================================
来源：http://ff.shxzukj.cn

L. 网络请求
来源：http://vh.gzmigu.cn

================================================================================
来源：http://do.szsharing.cn

[L01] 发送 GET 请求
来源：http://hp.jianghongdianzi.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://fi.asd995.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://rc.521024.cn

JS:   await fetch(url)
来源：http://qn.hahajie.cn

TS:   await fetch(url)
来源：http://iq.yuntaijiaju.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://vn.huanxung.cn

Go:   resp, err := http.Get(url)
来源：http://sz.shxzukj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://gs.jianghongdianzi.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://uu.newstarts.cn

[L02] 发送 POST JSON
来源：http://oe.szxytkj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ia.yuntaijiaju.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qr.chemitech.net.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://eo.huixinmuqiang.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dt.bookmarksfly.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://gn.newstarts.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jw.yuexingan06.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://pr.szxytkj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://rc.colortex.cn

[L03] 设置自定义请求头
来源：http://ck.jctech888.com.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://yw.panjiajie.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://zl.szsharing.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sj.jianghongdianzi.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qb.newstarts.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://jl.haigaiapp.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ql.wgjwhj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wg.jianghongdianzi.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://vt.panjiajie.cn

[L04] 设置超时
来源：http://vx.newstarts.cn

Py:   requests.get(url, timeout=5)
来源：http://zw.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://fw.yuexingan06.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lm.shxzskj.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uv.wgjwhj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://vk.huanxung.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://rg.bjjhwx.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://qn.lnxyls.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://fn.wgjwhj.cn

[L05] 上传文件（multipart）
来源：http://ws.hahajie.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://dx.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://tb.hnjuh.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mp.gzmigu.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://zq.jctech888.com.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://qs.asd995.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ad.yuntaijiaju.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ev.newstarts.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://av.yuexingan06.cn

[L06] 解析响应为 JSON
来源：http://oj.huixiangedu.cn

Py:   resp.json()
来源：http://qg.panjiajie.cn

PHP:  json_decode($body, true);
来源：http://pe.yuexingan06.cn

JS:   await resp.json()
来源：http://wf.lnxyls.cn

TS:   await resp.json()
来源：http://ah.newstarts.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://nw.gzmigu.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://tt.colortex.cn

Ruby: JSON.parse(resp.body)
来源：http://ys.szxytkj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://me.gzmigu.cn

[L07] 处理 HTTP 状态码
来源：http://hs.nszjky.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ub.huixinmuqiang.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ya.hnjuh.cn

JS:   resp.ok;  resp.status
来源：http://dh.shxzskj.cn

TS:   resp.ok;  resp.status
来源：http://ns.szsharing.cn

Java: resp.statusCode()
来源：http://jj.521024.cn

Go:   resp.StatusCode
来源：http://er.huixinmuqiang.cn

Ruby: resp.code.to_i
来源：http://gd.yuexingan06.cn

C#:   (int)resp.StatusCode
来源：http://kj.bjjhwx.cn

[L08] 并发请求多个地址
来源：http://ah.szxytkj.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://lt.bookmarksfly.cn

PHP:  curl_multi_init() 系列
来源：http://jl.muxihuayi.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://iz.asd995.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://po.bjjhwx.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://qt.521024.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wc.nicolike.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://yw.shxzskj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ih.hnjuh.cn

================================================================================
来源：http://mk.panjiajie.cn

M. 命令行 / 进程 / 环境
来源：http://tx.huanxung.cn

================================================================================
来源：http://tq.hahajie.cn

[M01] 读取命令行参数
来源：http://ar.jianghongdianzi.cn

Py:   sys.argv[1:]
来源：http://oh.huixiangedu.cn

PHP:  $argv;  $argc;
来源：http://uw.chemitech.net.cn

JS:   process.argv.slice(2)
来源：http://kh.521024.cn

TS:   process.argv.slice(2)
来源：http://mk.szsharing.cn

Java: args 数组（main 方法参数）
来源：http://yh.nszjky.cn

Go:   os.Args[1:]
来源：http://az.huixinmuqiang.cn

Ruby: ARGV
来源：http://hw.lnxyls.cn

C#:   args 数组（Main 方法参数）
来源：http://ee.521024.cn

[M02] 读取环境变量
来源：http://jg.jctech888.com.cn

Py:   os.environ.get("HOME")
来源：http://ix.panjiajie.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ur.szsharing.cn

JS:   process.env.HOME
来源：http://fp.jctech888.com.cn

TS:   process.env.HOME
来源：http://wu.bookmarksfly.cn

Java: System.getenv("HOME")
来源：http://bo.szsharing.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://xs.shtwfgs.cn

Ruby: ENV["HOME"]
来源：http://vm.muxihuayi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://vn.shtwfgs.cn

[M03] 执行外部命令
来源：http://wh.wgjwhj.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ly.shtwfgs.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://tw.haigaiapp.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://xe.szsharing.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://lp.asd995.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://pp.9csxet.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://jm.lnxyls.cn

Ruby: system("ls -l");  `ls -l`
来源：http://yc.hahajie.cn

C#:   Process.Start("ls", "-l");
来源：http://ow.jianghongdianzi.cn

[M04] 获取当前工作目录
来源：http://vw.lnxyls.cn

Py:   os.getcwd()
来源：http://ie.newstarts.cn

PHP:  getcwd();
来源：http://pv.shxzukj.cn

JS:   process.cwd()
来源：http://bn.lnxyls.cn

TS:   process.cwd()
来源：http://cw.jianghongdianzi.cn

Java: Path.of("").toAbsolutePath()
来源：http://tw.colortex.cn

Go:   os.Getwd()
来源：http://ke.muxihuayi.cn

Ruby: Dir.pwd
来源：http://kj.muxihuayi.cn

C#:   Directory.GetCurrentDirectory()
来源：http://tv.huixiangedu.cn

[M05] 设置退出码
来源：http://kt.muxihuayi.cn

Py:   sys.exit(1)
来源：http://ca.huixiangedu.cn

PHP:  exit(1);
来源：http://ep.hahajie.cn

JS:   process.exit(1)
来源：http://vx.hahajie.cn

TS:   process.exit(1)
来源：http://tp.chemitech.net.cn

Java: System.exit(1)
来源：http://gu.muxihuayi.cn

Go:   os.Exit(1)
来源：http://kj.521024.cn

Ruby: exit 1
来源：http://ny.lnxyls.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hu.nicolike.cn

[M06] 向标准错误输出
来源：http://hs.szxytkj.cn

Py:   print("err", file=sys.stderr)
来源：http://an.hnjuh.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://gb.huixinmuqiang.cn

JS:   console.error("err")
来源：http://qm.huanxung.cn

TS:   console.error("err")
来源：http://bj.wgjwhj.cn

Java: System.err.println("err")
来源：http://ot.jctech888.com.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://fe.yuntaijiaju.cn

Ruby: warn "err"
来源：http://cy.nicolike.cn

C#:   Console.Error.WriteLine("err")
来源：http://re.szxytkj.cn

[M07] 判断是否为主入口
来源：http://eg.nszjky.cn

Py:   if __name__ == "__main__":
来源：http://lb.9csxet.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://aa.521024.cn

JS:   require.main === module
来源：http://tn.asd995.cn

TS:   require.main === module
来源：http://mp.9csxet.cn

Java: public static void main(String[] args)
来源：http://iu.wgjwhj.cn

Go:   func main()
来源：http://nd.panjiajie.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://gv.shtwfgs.cn

C#:   static void Main(string[] args)
来源：http://sx.shtwfgs.cn

[M08] 获取系统与运行时信息
来源：http://tw.newstarts.cn

Py:   platform.system();  platform.python_version()
来源：http://wm.gzmigu.cn

PHP:  PHP_OS;  phpversion();
来源：http://ov.yuexingan06.cn

JS:   process.platform;  process.version
来源：http://fo.jianghongdianzi.cn

TS:   process.platform;  process.version
来源：http://lw.colortex.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://jz.shxzskj.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://kl.panjiajie.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ay.chemitech.net.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://qr.jctech888.com.cn

================================================================================
来源：http://gy.jianghongdianzi.cn

N. 数据结构与算法
来源：http://io.yuntaijiaju.cn

================================================================================
来源：http://aw.szxytkj.cn

[N01] 二分查找（有序数组）
来源：http://zm.jianghongdianzi.cn

Py:   bisect.bisect_left(arr, x)
来源：http://cx.lnxyls.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://uh.asd995.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ul.521024.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://uc.521024.cn

Java: Arrays.binarySearch(arr, x)
来源：http://tx.nszjky.cn

Go:   sort.SearchInts(arr, x)
来源：http://ol.shtwfgs.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://nw.szxytkj.cn

C#:   Array.BinarySearch(arr, x)
来源：http://hw.yuexingan06.cn

[N02] 排序（工程实践用内置实现）
来源：http://av.nszjky.cn

Py:   sorted(arr);  arr.sort()
来源：http://df.chemitech.net.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://dj.9csxet.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://wg.asd995.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://wo.521024.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://fg.gzmigu.cn

Go:   slices.Sort(arr)
来源：http://oe.yuexingan06.cn

Ruby: arr.sort
来源：http://bg.szsharing.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://cp.nszjky.cn

[N03] 快速排序（分治示例）
来源：http://rd.jctech888.com.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ey.huixinmuqiang.cn

PHP:  // 递归实现，或用 usort
来源：http://sw.huixiangedu.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mn.chemitech.net.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uy.jianghongdianzi.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://sz.szsharing.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ie.jctech888.com.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ma.521024.cn

C#:   // 手写递归，或 Array.Sort
来源：http://xm.asd995.cn

[N04] 斐波那契数列
来源：http://dc.jctech888.com.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://fy.shtwfgs.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ef.szxytkj.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://da.bjjhwx.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wz.panjiajie.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://vq.muxihuayi.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://fr.szsharing.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://kn.wgjwhj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://yw.hnjuh.cn

[N05] 最大公约数
来源：http://cp.huanxung.cn

Py:   math.gcd(a, b)
来源：http://pt.szsharing.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://xl.hnjuh.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ka.gzmigu.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xd.lnxyls.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://pa.colortex.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://dh.9csxet.cn

Ruby: a.gcd(b)
来源：http://jg.9csxet.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://tf.szsharing.cn

[N06] 判断回文字符串
来源：http://vj.huanxung.cn

Py:   s == s[::-1]
来源：http://wm.nszjky.cn

PHP:  $s === strrev($s);
来源：http://mc.szxytkj.cn

JS:   s === [...s].reverse().join("")
来源：http://rg.szxytkj.cn

TS:   s === [...s].reverse().join("")
来源：http://kr.nszjky.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://tf.szsharing.cn

Go:   // 双指针从两端比较
来源：http://cw.asd995.cn

Ruby: s == s.reverse
来源：http://ub.bjjhwx.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ht.wgjwhj.cn

[N07] 两数之和（返回下标）
来源：http://ny.huixiangedu.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://bf.szxytkj.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://sc.bookmarksfly.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ti.muxihuayi.cn

TS:   // 手写 Map<string, number>
来源：http://ad.521024.cn

Java: // 手写 HashMap
来源：http://ve.huixiangedu.cn

Go:   // 手写 map[int]int
来源：http://rr.szxytkj.cn

Ruby: // 手写 Hash
来源：http://ma.gzmigu.cn

C#:   // 手写 Dictionary<int, int>
来源：http://em.9csxet.cn

[N08] 生成全排列
来源：http://co.hnjuh.cn

Py:   itertools.permutations(arr)
来源：http://qq.bookmarksfly.cn

PHP:  // 手写递归交换
来源：http://mh.asd995.cn

JS:   // 手写回溯递归
来源：http://ff.huixinmuqiang.cn

TS:   // 手写回溯递归
来源：http://ne.hahajie.cn


<!-- 参考信息 -->