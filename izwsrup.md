代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ch.shxzskj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://qt.9csxet.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://fa.yuntaijiaju.cn

[J10] 取今天 / 本月第一天
来源：http://ci.yuntaijiaju.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ok.nszjky.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://qf.nszjky.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://dg.bookmarksfly.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://nt.9csxet.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://np.panjiajie.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wy.szsharing.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://iu.hnjuh.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://gd.newstarts.cn

================================================================================
来源：http://tr.hnjuh.cn

K. JSON 与序列化
来源：http://xx.521024.cn

================================================================================
来源：http://al.huixiangedu.cn

[K01] 对象转 JSON 字符串
来源：http://ni.muxihuayi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://gs.hnjuh.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wf.colortex.cn

JS:   JSON.stringify(obj)
来源：http://jg.yuexingan06.cn

TS:   JSON.stringify(obj)
来源：http://sl.lnxyls.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://qc.hnjuh.cn

Go:   json.Marshal(obj)
来源：http://oc.szxytkj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://sm.shtwfgs.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://px.bookmarksfly.cn

[K02] JSON 字符串转对象
来源：http://bb.yuexingan06.cn

Py:   json.loads(s)
来源：http://dn.521024.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://su.newstarts.cn

JS:   JSON.parse(s)
来源：http://pl.huixinmuqiang.cn

TS:   JSON.parse(s)
来源：http://hl.hnjuh.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mc.hnjuh.cn

Go:   json.Unmarshal(data, &v)
来源：http://oi.haigaiapp.cn

Ruby: JSON.parse(s)
来源：http://bl.wgjwhj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://cp.szsharing.cn

[K03] JSON 美化输出（带缩进）
来源：http://he.haigaiapp.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://fh.szsharing.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://oc.bookmarksfly.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://nr.hnjuh.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://wt.hnjuh.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ip.jctech888.com.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://zm.haigaiapp.cn

Ruby: JSON.pretty_generate(obj)
来源：http://bb.newstarts.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://rx.huixiangedu.cn

[K04] 读取 JSON 文件
来源：http://rb.9csxet.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://sp.9csxet.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://gq.hnjuh.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pq.haigaiapp.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xi.shxzskj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://px.shxzskj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://uo.wgjwhj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://pf.gzmigu.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://pb.huixinmuqiang.cn

[K05] 深拷贝对象
来源：http://bu.jctech888.com.cn

Py:   copy.deepcopy(obj)
来源：http://uk.colortex.cn

PHP:  unserialize(serialize($obj));
来源：http://tt.panjiajie.cn

JS:   structuredClone(obj)
来源：http://sp.asd995.cn

TS:   structuredClone(obj)
来源：http://vb.nicolike.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://aj.huixiangedu.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://yt.haigaiapp.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://gw.nszjky.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ce.gzmigu.cn

[K06] 解析 URL 查询串
来源：http://lo.chemitech.net.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wj.shxzskj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hy.lnxyls.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rq.yuexingan06.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vf.huixiangedu.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wv.huixiangedu.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://wh.panjiajie.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://xm.huanxung.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://xf.szsharing.cn

[K07] 进制转换
来源：http://vd.yuexingan06.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://bf.yuntaijiaju.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://zv.colortex.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://zx.huixiangedu.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://zf.szxytkj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://vu.521024.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://gq.muxihuayi.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://pr.jctech888.com.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://bv.9csxet.cn

[K08] 二进制序列化（非 JSON）
来源：http://jx.shtwfgs.cn

Py:   pickle.dumps(obj)
来源：http://ec.colortex.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://yp.newstarts.cn

JS:   v8.serialize(obj)        // Node
来源：http://mj.szxytkj.cn

TS:   v8.serialize(obj)        // Node
来源：http://mf.521024.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://tj.shxzukj.cn

Go:   encoding/gob
来源：http://ue.szxytkj.cn

Ruby: Marshal.dump(obj)
来源：http://lh.lnxyls.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://pm.bookmarksfly.cn

================================================================================
来源：http://ke.shxzukj.cn

L. 网络请求
来源：http://xw.haigaiapp.cn

================================================================================
来源：http://hp.colortex.cn

[L01] 发送 GET 请求
来源：http://jb.hahajie.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://lm.szsharing.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ns.shxzskj.cn

JS:   await fetch(url)
来源：http://tm.huixiangedu.cn

TS:   await fetch(url)
来源：http://oa.521024.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://th.shxzskj.cn

Go:   resp, err := http.Get(url)
来源：http://is.wgjwhj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ta.panjiajie.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://fl.yuexingan06.cn

[L02] 发送 POST JSON
来源：http://mk.bookmarksfly.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ni.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://fq.newstarts.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xm.jctech888.com.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xt.chemitech.net.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ts.muxihuayi.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ue.bjjhwx.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wc.jctech888.com.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://jt.panjiajie.cn

[L03] 设置自定义请求头
来源：http://sm.yuntaijiaju.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://li.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ef.muxihuayi.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gn.colortex.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://eu.9csxet.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://nx.yuntaijiaju.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://gj.yuexingan06.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ly.gzmigu.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://dm.nszjky.cn

[L04] 设置超时
来源：http://ke.chemitech.net.cn

Py:   requests.get(url, timeout=5)
来源：http://di.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://rs.newstarts.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://od.nicolike.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rx.huixinmuqiang.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://au.huixiangedu.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://br.huanxung.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://bx.nszjky.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://kz.yuexingan06.cn

[L05] 上传文件（multipart）
来源：http://tt.colortex.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wy.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://cd.colortex.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ec.wgjwhj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hm.gzmigu.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://lo.nszjky.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ey.huixiangedu.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://cc.asd995.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://aq.muxihuayi.cn

[L06] 解析响应为 JSON
来源：http://lg.szsharing.cn

Py:   resp.json()
来源：http://nk.bjjhwx.cn

PHP:  json_decode($body, true);
来源：http://fa.szxytkj.cn

JS:   await resp.json()
来源：http://db.yuexingan06.cn

TS:   await resp.json()
来源：http://es.panjiajie.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://qt.huanxung.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://rp.gzmigu.cn

Ruby: JSON.parse(resp.body)
来源：http://tw.asd995.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://tw.jianghongdianzi.cn

[L07] 处理 HTTP 状态码
来源：http://sv.shtwfgs.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://uj.szsharing.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://oq.nszjky.cn

JS:   resp.ok;  resp.status
来源：http://wg.asd995.cn

TS:   resp.ok;  resp.status
来源：http://wu.panjiajie.cn

Java: resp.statusCode()
来源：http://tb.colortex.cn

Go:   resp.StatusCode
来源：http://or.nszjky.cn

Ruby: resp.code.to_i
来源：http://hc.muxihuayi.cn

C#:   (int)resp.StatusCode
来源：http://ce.haigaiapp.cn

[L08] 并发请求多个地址
来源：http://sm.jctech888.com.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://gt.shtwfgs.cn

PHP:  curl_multi_init() 系列
来源：http://qp.9csxet.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ju.yuexingan06.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qg.newstarts.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://jb.chemitech.net.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://tv.hahajie.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://px.9csxet.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://od.hnjuh.cn

================================================================================
来源：http://kl.chemitech.net.cn

M. 命令行 / 进程 / 环境
来源：http://nb.nszjky.cn

================================================================================
来源：http://co.haigaiapp.cn

[M01] 读取命令行参数
来源：http://mg.bjjhwx.cn

Py:   sys.argv[1:]
来源：http://eg.szsharing.cn

PHP:  $argv;  $argc;
来源：http://of.wgjwhj.cn

JS:   process.argv.slice(2)
来源：http://rl.szxytkj.cn

TS:   process.argv.slice(2)
来源：http://ut.haigaiapp.cn

Java: args 数组（main 方法参数）
来源：http://ve.szsharing.cn

Go:   os.Args[1:]
来源：http://lg.huanxung.cn

Ruby: ARGV
来源：http://nj.colortex.cn

C#:   args 数组（Main 方法参数）
来源：http://ny.jctech888.com.cn

[M02] 读取环境变量
来源：http://xz.shxzskj.cn

Py:   os.environ.get("HOME")
来源：http://op.hnjuh.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zs.yuexingan06.cn

JS:   process.env.HOME
来源：http://qh.huixinmuqiang.cn

TS:   process.env.HOME
来源：http://ox.521024.cn

Java: System.getenv("HOME")
来源：http://np.yuexingan06.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://kd.huanxung.cn

Ruby: ENV["HOME"]
来源：http://ni.hahajie.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://bt.szxytkj.cn

[M03] 执行外部命令
来源：http://oe.shxzskj.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://to.nicolike.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://lt.yuexingan06.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://vi.asd995.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://oq.newstarts.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://yf.9csxet.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://sc.panjiajie.cn

Ruby: system("ls -l");  `ls -l`
来源：http://aa.shtwfgs.cn

C#:   Process.Start("ls", "-l");
来源：http://jp.jctech888.com.cn

[M04] 获取当前工作目录
来源：http://jm.yuexingan06.cn

Py:   os.getcwd()
来源：http://bb.muxihuayi.cn

PHP:  getcwd();
来源：http://kt.colortex.cn

JS:   process.cwd()
来源：http://lm.hahajie.cn

TS:   process.cwd()
来源：http://rf.huixiangedu.cn

Java: Path.of("").toAbsolutePath()
来源：http://ze.huixiangedu.cn

Go:   os.Getwd()
来源：http://mc.521024.cn

Ruby: Dir.pwd
来源：http://an.hnjuh.cn

C#:   Directory.GetCurrentDirectory()
来源：http://qf.9csxet.cn

[M05] 设置退出码
来源：http://dx.panjiajie.cn

Py:   sys.exit(1)
来源：http://ma.szsharing.cn

PHP:  exit(1);
来源：http://km.nszjky.cn

JS:   process.exit(1)
来源：http://ii.haigaiapp.cn

TS:   process.exit(1)
来源：http://mv.gzmigu.cn

Java: System.exit(1)
来源：http://qt.bookmarksfly.cn

Go:   os.Exit(1)
来源：http://or.yuntaijiaju.cn

Ruby: exit 1
来源：http://ge.bjjhwx.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ps.wgjwhj.cn

[M06] 向标准错误输出
来源：http://av.nicolike.cn

Py:   print("err", file=sys.stderr)
来源：http://oy.huanxung.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://tw.nszjky.cn

JS:   console.error("err")
来源：http://tw.newstarts.cn

TS:   console.error("err")
来源：http://uc.jianghongdianzi.cn

Java: System.err.println("err")
来源：http://yf.yuntaijiaju.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wl.szxytkj.cn

Ruby: warn "err"
来源：http://ns.hnjuh.cn

C#:   Console.Error.WriteLine("err")
来源：http://kr.hahajie.cn

[M07] 判断是否为主入口
来源：http://oj.bookmarksfly.cn

Py:   if __name__ == "__main__":
来源：http://tr.9csxet.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ms.nszjky.cn

JS:   require.main === module
来源：http://vd.yuexingan06.cn

TS:   require.main === module
来源：http://wr.colortex.cn

Java: public static void main(String[] args)
来源：http://qc.yuntaijiaju.cn

Go:   func main()
来源：http://zo.shxzukj.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ou.9csxet.cn

C#:   static void Main(string[] args)
来源：http://xe.szxytkj.cn

[M08] 获取系统与运行时信息
来源：http://jc.colortex.cn

Py:   platform.system();  platform.python_version()
来源：http://gs.hnjuh.cn

PHP:  PHP_OS;  phpversion();
来源：http://tb.asd995.cn

JS:   process.platform;  process.version
来源：http://sx.lnxyls.cn

TS:   process.platform;  process.version
来源：http://bm.hahajie.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://tk.wgjwhj.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://gh.nicolike.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ap.yuexingan06.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://om.yuexingan06.cn

================================================================================
来源：http://ww.huixiangedu.cn

N. 数据结构与算法
来源：http://tt.muxihuayi.cn

================================================================================
来源：http://ul.newstarts.cn

[N01] 二分查找（有序数组）
来源：http://ck.asd995.cn

Py:   bisect.bisect_left(arr, x)
来源：http://oh.yuexingan06.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mq.panjiajie.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xy.jctech888.com.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ab.huanxung.cn

Java: Arrays.binarySearch(arr, x)
来源：http://pi.bjjhwx.cn

Go:   sort.SearchInts(arr, x)
来源：http://xp.lnxyls.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://kb.chemitech.net.cn

C#:   Array.BinarySearch(arr, x)
来源：http://jd.9csxet.cn

[N02] 排序（工程实践用内置实现）
来源：http://ds.lnxyls.cn

Py:   sorted(arr);  arr.sort()
来源：http://em.bookmarksfly.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://lq.lnxyls.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://mq.colortex.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://qy.colortex.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://st.bookmarksfly.cn

Go:   slices.Sort(arr)
来源：http://wj.newstarts.cn

Ruby: arr.sort
来源：http://el.chemitech.net.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://in.chemitech.net.cn

[N03] 快速排序（分治示例）
来源：http://rq.jianghongdianzi.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://zs.szxytkj.cn

PHP:  // 递归实现，或用 usort
来源：http://hi.hahajie.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vt.szxytkj.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dc.gzmigu.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://by.szsharing.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://rr.hahajie.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://zh.colortex.cn

C#:   // 手写递归，或 Array.Sort
来源：http://jb.nicolike.cn

[N04] 斐波那契数列
来源：http://oi.hnjuh.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://to.huanxung.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://iv.colortex.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rv.nicolike.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nn.panjiajie.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://sf.szsharing.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://th.chemitech.net.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://yg.huixinmuqiang.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ry.panjiajie.cn

[N05] 最大公约数
来源：http://wp.huixinmuqiang.cn

Py:   math.gcd(a, b)
来源：http://eu.muxihuayi.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://bf.newstarts.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nl.shxzukj.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xp.huixiangedu.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://vu.haigaiapp.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://tc.bjjhwx.cn

Ruby: a.gcd(b)
来源：http://cj.9csxet.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://dg.nicolike.cn

[N06] 判断回文字符串
来源：http://se.bookmarksfly.cn

Py:   s == s[::-1]
来源：http://oc.huixiangedu.cn

PHP:  $s === strrev($s);
来源：http://nw.521024.cn

JS:   s === [...s].reverse().join("")
来源：http://ea.yuexingan06.cn

TS:   s === [...s].reverse().join("")
来源：http://jb.haigaiapp.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://sg.shtwfgs.cn

Go:   // 双指针从两端比较
来源：http://if.yuexingan06.cn

Ruby: s == s.reverse
来源：http://ie.shtwfgs.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://sn.huixiangedu.cn

[N07] 两数之和（返回下标）
来源：http://al.nszjky.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://xm.hahajie.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://af.hahajie.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://os.chemitech.net.cn

TS:   // 手写 Map<string, number>
来源：http://nn.haigaiapp.cn

Java: // 手写 HashMap
来源：http://ir.521024.cn


<!-- 参考信息 -->