代发 wailian999

Py:   date.today();  date.today().replace(day=1)
来源：http://jm.panjiajie.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://dg.nszjky.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ix.9csxet.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://sk.szsharing.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://df.wgjwhj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ju.bjjhwx.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://an.chemitech.net.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://bl.nicolike.cn

================================================================================
来源：http://sr.szxytkj.cn

K. JSON 与序列化
来源：http://pb.shtwfgs.cn

================================================================================
来源：http://jo.jianghongdianzi.cn

[K01] 对象转 JSON 字符串
来源：http://qa.szsharing.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://uc.panjiajie.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://oy.nicolike.cn

JS:   JSON.stringify(obj)
来源：http://vr.gzmigu.cn

TS:   JSON.stringify(obj)
来源：http://fb.huixinmuqiang.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://st.shxzukj.cn

Go:   json.Marshal(obj)
来源：http://fa.panjiajie.cn

Ruby: obj.to_json                                     // require "json"
来源：http://kb.newstarts.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://il.shtwfgs.cn

[K02] JSON 字符串转对象
来源：http://hs.521024.cn

Py:   json.loads(s)
来源：http://dw.haigaiapp.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mk.hahajie.cn

JS:   JSON.parse(s)
来源：http://is.huixinmuqiang.cn

TS:   JSON.parse(s)
来源：http://zr.lnxyls.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ir.jianghongdianzi.cn

Go:   json.Unmarshal(data, &v)
来源：http://qg.huixiangedu.cn

Ruby: JSON.parse(s)
来源：http://yw.newstarts.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ko.jianghongdianzi.cn

[K03] JSON 美化输出（带缩进）
来源：http://nh.colortex.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://zn.hnjuh.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://fw.yuexingan06.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ze.bjjhwx.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ju.gzmigu.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qg.szsharing.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://sv.colortex.cn

Ruby: JSON.pretty_generate(obj)
来源：http://nb.yuexingan06.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://jx.shtwfgs.cn

[K04] 读取 JSON 文件
来源：http://ij.chemitech.net.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://lv.shtwfgs.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ai.hahajie.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fu.9csxet.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ie.bookmarksfly.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://cz.haigaiapp.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://up.jctech888.com.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://yh.nicolike.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://rq.521024.cn

[K05] 深拷贝对象
来源：http://op.huixinmuqiang.cn

Py:   copy.deepcopy(obj)
来源：http://da.yuexingan06.cn

PHP:  unserialize(serialize($obj));
来源：http://ob.jianghongdianzi.cn

JS:   structuredClone(obj)
来源：http://lk.colortex.cn

TS:   structuredClone(obj)
来源：http://vc.lnxyls.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://kb.hahajie.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qf.gzmigu.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ln.bjjhwx.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://kp.newstarts.cn

[K06] 解析 URL 查询串
来源：http://xw.haigaiapp.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xp.lnxyls.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zm.huixinmuqiang.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gt.shxzskj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vg.szxytkj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mu.muxihuayi.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://oj.gzmigu.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://zs.shxzukj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://bk.jctech888.com.cn

[K07] 进制转换
来源：http://gf.newstarts.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://xd.huanxung.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hr.haigaiapp.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ht.huixinmuqiang.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://sh.shxzukj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mg.gzmigu.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://tc.wgjwhj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://jk.chemitech.net.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://pz.nszjky.cn

[K08] 二进制序列化（非 JSON）
来源：http://xj.haigaiapp.cn

Py:   pickle.dumps(obj)
来源：http://pz.huixinmuqiang.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://cj.panjiajie.cn

JS:   v8.serialize(obj)        // Node
来源：http://hv.bookmarksfly.cn

TS:   v8.serialize(obj)        // Node
来源：http://lo.shxzukj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://xx.shxzskj.cn

Go:   encoding/gob
来源：http://je.shxzskj.cn

Ruby: Marshal.dump(obj)
来源：http://oo.newstarts.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wj.gzmigu.cn

================================================================================
来源：http://sl.newstarts.cn

L. 网络请求
来源：http://jy.nszjky.cn

================================================================================
来源：http://xy.gzmigu.cn

[L01] 发送 GET 请求
来源：http://on.huixinmuqiang.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://du.muxihuayi.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://gy.jianghongdianzi.cn

JS:   await fetch(url)
来源：http://mh.asd995.cn

TS:   await fetch(url)
来源：http://ms.bookmarksfly.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://fu.gzmigu.cn

Go:   resp, err := http.Get(url)
来源：http://pq.newstarts.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://tk.shtwfgs.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://xr.huixiangedu.cn

[L02] 发送 POST JSON
来源：http://sp.haigaiapp.cn

Py:   requests.post(url, json={"a": 1})
来源：http://pw.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://vd.huixinmuqiang.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kx.wgjwhj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ao.yuexingan06.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://nk.lnxyls.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ea.wgjwhj.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://bd.bjjhwx.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://aw.yuexingan06.cn

[L03] 设置自定义请求头
来源：http://bx.jianghongdianzi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://cd.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://uy.huixinmuqiang.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://io.hnjuh.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://af.panjiajie.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ak.asd995.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://pk.hnjuh.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://zh.yuexingan06.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://bw.huanxung.cn

[L04] 设置超时
来源：http://vv.huanxung.cn

Py:   requests.get(url, timeout=5)
来源：http://ls.haigaiapp.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://nz.gzmigu.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vi.panjiajie.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vt.jianghongdianzi.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ne.nicolike.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://yh.9csxet.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://pi.lnxyls.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ft.lnxyls.cn

[L05] 上传文件（multipart）
来源：http://jp.huixiangedu.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://yt.521024.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://zi.colortex.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://zn.panjiajie.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://pn.newstarts.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://at.hnjuh.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://fj.muxihuayi.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://oy.yuexingan06.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://md.jianghongdianzi.cn

[L06] 解析响应为 JSON
来源：http://uc.haigaiapp.cn

Py:   resp.json()
来源：http://nv.huixinmuqiang.cn

PHP:  json_decode($body, true);
来源：http://tg.lnxyls.cn

JS:   await resp.json()
来源：http://oa.9csxet.cn

TS:   await resp.json()
来源：http://bt.bookmarksfly.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://pp.huixinmuqiang.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://oj.szsharing.cn

Ruby: JSON.parse(resp.body)
来源：http://zx.hahajie.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ft.bjjhwx.cn

[L07] 处理 HTTP 状态码
来源：http://wd.chemitech.net.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://kw.huanxung.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://eo.huixiangedu.cn

JS:   resp.ok;  resp.status
来源：http://kz.lnxyls.cn

TS:   resp.ok;  resp.status
来源：http://qj.bjjhwx.cn

Java: resp.statusCode()
来源：http://yx.huanxung.cn

Go:   resp.StatusCode
来源：http://mr.huanxung.cn

Ruby: resp.code.to_i
来源：http://mt.yuexingan06.cn

C#:   (int)resp.StatusCode
来源：http://ud.yuexingan06.cn

[L08] 并发请求多个地址
来源：http://nl.shxzukj.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://yi.9csxet.cn

PHP:  curl_multi_init() 系列
来源：http://it.shxzskj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://co.nszjky.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ge.panjiajie.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ro.szsharing.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ms.521024.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ct.nszjky.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://bn.nicolike.cn

================================================================================
来源：http://gj.bjjhwx.cn

M. 命令行 / 进程 / 环境
来源：http://sr.jianghongdianzi.cn

================================================================================
来源：http://ve.huixiangedu.cn

[M01] 读取命令行参数
来源：http://ts.chemitech.net.cn

Py:   sys.argv[1:]
来源：http://ox.521024.cn

PHP:  $argv;  $argc;
来源：http://ir.shxzukj.cn

JS:   process.argv.slice(2)
来源：http://oc.huanxung.cn

TS:   process.argv.slice(2)
来源：http://rf.haigaiapp.cn

Java: args 数组（main 方法参数）
来源：http://uw.hahajie.cn

Go:   os.Args[1:]
来源：http://iz.muxihuayi.cn

Ruby: ARGV
来源：http://xu.chemitech.net.cn

C#:   args 数组（Main 方法参数）
来源：http://ga.asd995.cn

[M02] 读取环境变量
来源：http://eb.jianghongdianzi.cn

Py:   os.environ.get("HOME")
来源：http://sb.521024.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://in.colortex.cn

JS:   process.env.HOME
来源：http://bq.yuexingan06.cn

TS:   process.env.HOME
来源：http://wm.newstarts.cn

Java: System.getenv("HOME")
来源：http://xp.gzmigu.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ci.huixiangedu.cn

Ruby: ENV["HOME"]
来源：http://ru.wgjwhj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://bm.jctech888.com.cn

[M03] 执行外部命令
来源：http://aw.jctech888.com.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://au.colortex.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zs.szxytkj.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://np.huixinmuqiang.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ba.hahajie.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://by.hnjuh.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ri.hahajie.cn

Ruby: system("ls -l");  `ls -l`
来源：http://rs.bookmarksfly.cn

C#:   Process.Start("ls", "-l");
来源：http://gk.huanxung.cn

[M04] 获取当前工作目录
来源：http://mw.yuexingan06.cn

Py:   os.getcwd()
来源：http://am.lnxyls.cn

PHP:  getcwd();
来源：http://or.521024.cn

JS:   process.cwd()
来源：http://jq.bjjhwx.cn

TS:   process.cwd()
来源：http://rl.9csxet.cn

Java: Path.of("").toAbsolutePath()
来源：http://gc.lnxyls.cn

Go:   os.Getwd()
来源：http://uz.huixinmuqiang.cn

Ruby: Dir.pwd
来源：http://sx.hahajie.cn

C#:   Directory.GetCurrentDirectory()
来源：http://oc.haigaiapp.cn

[M05] 设置退出码
来源：http://ei.shxzskj.cn

Py:   sys.exit(1)
来源：http://os.szxytkj.cn

PHP:  exit(1);
来源：http://gy.nszjky.cn

JS:   process.exit(1)
来源：http://ed.huixinmuqiang.cn

TS:   process.exit(1)
来源：http://ji.huixinmuqiang.cn

Java: System.exit(1)
来源：http://mz.wgjwhj.cn

Go:   os.Exit(1)
来源：http://hb.szsharing.cn

Ruby: exit 1
来源：http://nh.gzmigu.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://as.hnjuh.cn

[M06] 向标准错误输出
来源：http://ba.huixinmuqiang.cn

Py:   print("err", file=sys.stderr)
来源：http://qz.hahajie.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://bs.yuexingan06.cn

JS:   console.error("err")
来源：http://by.hahajie.cn

TS:   console.error("err")
来源：http://ya.szxytkj.cn

Java: System.err.println("err")
来源：http://jq.szxytkj.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://re.wgjwhj.cn

Ruby: warn "err"
来源：http://ha.jctech888.com.cn

C#:   Console.Error.WriteLine("err")
来源：http://cs.hahajie.cn

[M07] 判断是否为主入口
来源：http://ms.yuexingan06.cn

Py:   if __name__ == "__main__":
来源：http://xa.panjiajie.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wy.yuexingan06.cn

JS:   require.main === module
来源：http://rq.jianghongdianzi.cn

TS:   require.main === module
来源：http://ba.bookmarksfly.cn

Java: public static void main(String[] args)
来源：http://wq.jctech888.com.cn

Go:   func main()
来源：http://cb.newstarts.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://xo.huanxung.cn

C#:   static void Main(string[] args)
来源：http://mq.asd995.cn

[M08] 获取系统与运行时信息
来源：http://jk.newstarts.cn

Py:   platform.system();  platform.python_version()
来源：http://ux.szxytkj.cn

PHP:  PHP_OS;  phpversion();
来源：http://lt.huanxung.cn

JS:   process.platform;  process.version
来源：http://nk.asd995.cn

TS:   process.platform;  process.version
来源：http://sj.wgjwhj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://tx.shxzukj.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://eo.shtwfgs.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://by.hahajie.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://oc.jctech888.com.cn

================================================================================
来源：http://ev.shxzskj.cn

N. 数据结构与算法
来源：http://ny.newstarts.cn

================================================================================
来源：http://is.yuntaijiaju.cn

[N01] 二分查找（有序数组）
来源：http://xv.chemitech.net.cn

Py:   bisect.bisect_left(arr, x)
来源：http://sr.szxytkj.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ga.nicolike.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ws.bookmarksfly.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hj.yuntaijiaju.cn

Java: Arrays.binarySearch(arr, x)
来源：http://mr.shtwfgs.cn

Go:   sort.SearchInts(arr, x)
来源：http://ja.wgjwhj.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://jp.huixiangedu.cn

C#:   Array.BinarySearch(arr, x)
来源：http://gw.wgjwhj.cn

[N02] 排序（工程实践用内置实现）
来源：http://br.gzmigu.cn

Py:   sorted(arr);  arr.sort()
来源：http://vi.bjjhwx.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://bv.hahajie.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://yi.colortex.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://bs.lnxyls.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://og.shxzskj.cn

Go:   slices.Sort(arr)
来源：http://wq.yuntaijiaju.cn

Ruby: arr.sort
来源：http://an.bjjhwx.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://fn.nicolike.cn

[N03] 快速排序（分治示例）
来源：http://dp.szxytkj.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://uu.wgjwhj.cn

PHP:  // 递归实现，或用 usort
来源：http://ma.bjjhwx.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ju.bjjhwx.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lj.hnjuh.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ly.panjiajie.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://uo.haigaiapp.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wr.jianghongdianzi.cn

C#:   // 手写递归，或 Array.Sort
来源：http://xo.hnjuh.cn

[N04] 斐波那契数列
来源：http://ea.nszjky.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ku.shxzskj.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hn.bjjhwx.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://iq.nszjky.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wc.szxytkj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://um.huanxung.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wp.panjiajie.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ea.jianghongdianzi.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ee.shtwfgs.cn

[N05] 最大公约数
来源：http://nt.newstarts.cn

Py:   math.gcd(a, b)
来源：http://hx.huixiangedu.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://oo.yuntaijiaju.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mz.colortex.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qt.yuexingan06.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://rv.nicolike.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ml.wgjwhj.cn

Ruby: a.gcd(b)
来源：http://xx.lnxyls.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://gl.muxihuayi.cn

[N06] 判断回文字符串
来源：http://to.521024.cn

Py:   s == s[::-1]
来源：http://nc.521024.cn

PHP:  $s === strrev($s);
来源：http://sd.lnxyls.cn

JS:   s === [...s].reverse().join("")
来源：http://dk.muxihuayi.cn

TS:   s === [...s].reverse().join("")
来源：http://ys.bookmarksfly.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://zl.yuexingan06.cn

Go:   // 双指针从两端比较
来源：http://nn.nszjky.cn

Ruby: s == s.reverse
来源：http://ht.bjjhwx.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://fs.hahajie.cn

[N07] 两数之和（返回下标）
来源：http://ou.bjjhwx.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://yk.haigaiapp.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wt.muxihuayi.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ep.muxihuayi.cn

TS:   // 手写 Map<string, number>
来源：http://qn.shxzskj.cn

Java: // 手写 HashMap
来源：http://ua.nicolike.cn

Go:   // 手写 map[int]int
来源：http://dl.huixiangedu.cn

Ruby: // 手写 Hash
来源：http://ki.huixinmuqiang.cn

C#:   // 手写 Dictionary<int, int>
来源：http://uq.shtwfgs.cn

[N08] 生成全排列
来源：http://mf.shxzskj.cn


<!-- 参考信息 -->