代发 wailian999

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ro.newstarts.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mu.szxytkj.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ei.haigaiapp.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ap.shxzukj.cn

================================================================================
来源：http://el.shxzskj.cn

K. JSON 与序列化
来源：http://gn.chemitech.net.cn

================================================================================
来源：http://qs.asd995.cn

[K01] 对象转 JSON 字符串
来源：http://pw.nicolike.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ag.shxzskj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://zm.shtwfgs.cn

JS:   JSON.stringify(obj)
来源：http://kz.jianghongdianzi.cn

TS:   JSON.stringify(obj)
来源：http://vc.521024.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://xx.chemitech.net.cn

Go:   json.Marshal(obj)
来源：http://xg.haigaiapp.cn

Ruby: obj.to_json                                     // require "json"
来源：http://rb.muxihuayi.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://hm.nszjky.cn

[K02] JSON 字符串转对象
来源：http://sc.521024.cn

Py:   json.loads(s)
来源：http://wo.colortex.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://au.szxytkj.cn

JS:   JSON.parse(s)
来源：http://gd.shxzskj.cn

TS:   JSON.parse(s)
来源：http://rd.bookmarksfly.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ee.muxihuayi.cn

Go:   json.Unmarshal(data, &v)
来源：http://na.lnxyls.cn

Ruby: JSON.parse(s)
来源：http://rh.haigaiapp.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qi.nszjky.cn

[K03] JSON 美化输出（带缩进）
来源：http://qv.huanxung.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://bb.lnxyls.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://br.muxihuayi.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ws.bjjhwx.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://lb.panjiajie.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://kq.newstarts.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://jt.colortex.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ea.huixinmuqiang.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://fa.nszjky.cn

[K04] 读取 JSON 文件
来源：http://ax.shtwfgs.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://gk.haigaiapp.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ek.bjjhwx.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nd.jctech888.com.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zb.nszjky.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://za.huixiangedu.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://sc.yuexingan06.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://cf.huanxung.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ui.nicolike.cn

[K05] 深拷贝对象
来源：http://ef.asd995.cn

Py:   copy.deepcopy(obj)
来源：http://ox.yuntaijiaju.cn

PHP:  unserialize(serialize($obj));
来源：http://yp.asd995.cn

JS:   structuredClone(obj)
来源：http://wr.haigaiapp.cn

TS:   structuredClone(obj)
来源：http://dr.9csxet.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://tj.bookmarksfly.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://rr.yuexingan06.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://in.jianghongdianzi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ve.panjiajie.cn

[K06] 解析 URL 查询串
来源：http://cq.gzmigu.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ka.9csxet.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ku.bookmarksfly.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kp.panjiajie.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xt.bjjhwx.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hc.9csxet.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://uc.szsharing.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ev.haigaiapp.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://lo.yuexingan06.cn

[K07] 进制转换
来源：http://cx.shxzukj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://yr.jianghongdianzi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://cd.hahajie.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://qg.shxzskj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://lh.shtwfgs.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://uy.yuntaijiaju.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://nl.nicolike.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://of.nszjky.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://cd.wgjwhj.cn

[K08] 二进制序列化（非 JSON）
来源：http://ng.lnxyls.cn

Py:   pickle.dumps(obj)
来源：http://sv.jctech888.com.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://kz.szsharing.cn

JS:   v8.serialize(obj)        // Node
来源：http://lc.shxzskj.cn

TS:   v8.serialize(obj)        // Node
来源：http://ur.shxzukj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://bf.bookmarksfly.cn

Go:   encoding/gob
来源：http://cc.yuexingan06.cn

Ruby: Marshal.dump(obj)
来源：http://be.colortex.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://yv.nicolike.cn

================================================================================
来源：http://mb.shtwfgs.cn

L. 网络请求
来源：http://mm.9csxet.cn

================================================================================
来源：http://sp.panjiajie.cn

[L01] 发送 GET 请求
来源：http://cl.jianghongdianzi.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ir.wgjwhj.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hu.szsharing.cn

JS:   await fetch(url)
来源：http://qv.haigaiapp.cn

TS:   await fetch(url)
来源：http://le.asd995.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hn.huixinmuqiang.cn

Go:   resp, err := http.Get(url)
来源：http://kx.hnjuh.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://io.huixinmuqiang.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://sx.nszjky.cn

[L02] 发送 POST JSON
来源：http://pn.haigaiapp.cn

Py:   requests.post(url, json={"a": 1})
来源：http://dw.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://rf.huanxung.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xb.newstarts.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://og.bookmarksfly.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ok.shtwfgs.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://io.asd995.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://vg.panjiajie.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://oy.newstarts.cn

[L03] 设置自定义请求头
来源：http://xz.hahajie.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://jx.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://rf.chemitech.net.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rj.shxzskj.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://di.colortex.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://kz.panjiajie.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://gu.panjiajie.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://lt.huanxung.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ch.lnxyls.cn

[L04] 设置超时
来源：http://lu.yuexingan06.cn

Py:   requests.get(url, timeout=5)
来源：http://kg.521024.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://cd.hnjuh.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vt.huixiangedu.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ny.lnxyls.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://cx.yuntaijiaju.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://io.huanxung.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://lr.jctech888.com.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://bi.9csxet.cn

[L05] 上传文件（multipart）
来源：http://ey.szxytkj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://bg.nszjky.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://bt.lnxyls.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://yg.huanxung.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://my.bjjhwx.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mt.szsharing.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://oh.newstarts.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://bu.yuexingan06.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wk.hahajie.cn

[L06] 解析响应为 JSON
来源：http://ed.lnxyls.cn

Py:   resp.json()
来源：http://tb.asd995.cn

PHP:  json_decode($body, true);
来源：http://zp.521024.cn

JS:   await resp.json()
来源：http://dy.shxzskj.cn

TS:   await resp.json()
来源：http://pi.colortex.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ya.hahajie.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://bb.yuexingan06.cn

Ruby: JSON.parse(resp.body)
来源：http://jg.huixinmuqiang.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://jj.gzmigu.cn

[L07] 处理 HTTP 状态码
来源：http://vf.szsharing.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ju.shxzskj.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://fp.colortex.cn

JS:   resp.ok;  resp.status
来源：http://qq.newstarts.cn

TS:   resp.ok;  resp.status
来源：http://we.huixiangedu.cn

Java: resp.statusCode()
来源：http://hs.szsharing.cn

Go:   resp.StatusCode
来源：http://nu.shtwfgs.cn

Ruby: resp.code.to_i
来源：http://gh.huanxung.cn

C#:   (int)resp.StatusCode
来源：http://zg.chemitech.net.cn

[L08] 并发请求多个地址
来源：http://qh.panjiajie.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mv.gzmigu.cn

PHP:  curl_multi_init() 系列
来源：http://fd.521024.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nx.bookmarksfly.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://eo.shxzukj.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wk.haigaiapp.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://vs.hnjuh.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://or.newstarts.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://so.huanxung.cn

================================================================================
来源：http://gz.yuntaijiaju.cn

M. 命令行 / 进程 / 环境
来源：http://kx.wgjwhj.cn

================================================================================
来源：http://tc.nszjky.cn

[M01] 读取命令行参数
来源：http://xv.asd995.cn

Py:   sys.argv[1:]
来源：http://ak.wgjwhj.cn

PHP:  $argv;  $argc;
来源：http://rr.chemitech.net.cn

JS:   process.argv.slice(2)
来源：http://cp.huixinmuqiang.cn

TS:   process.argv.slice(2)
来源：http://pn.wgjwhj.cn

Java: args 数组（main 方法参数）
来源：http://qu.shtwfgs.cn

Go:   os.Args[1:]
来源：http://wz.nszjky.cn

Ruby: ARGV
来源：http://vy.asd995.cn

C#:   args 数组（Main 方法参数）
来源：http://ck.szsharing.cn

[M02] 读取环境变量
来源：http://ag.colortex.cn

Py:   os.environ.get("HOME")
来源：http://xm.hahajie.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ee.colortex.cn

JS:   process.env.HOME
来源：http://qv.521024.cn

TS:   process.env.HOME
来源：http://tf.lnxyls.cn

Java: System.getenv("HOME")
来源：http://cz.nicolike.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://uz.newstarts.cn

Ruby: ENV["HOME"]
来源：http://db.wgjwhj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://nt.bjjhwx.cn

[M03] 执行外部命令
来源：http://vw.muxihuayi.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://sk.gzmigu.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://fa.colortex.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://tv.panjiajie.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://bc.jianghongdianzi.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://vo.haigaiapp.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ut.hahajie.cn

Ruby: system("ls -l");  `ls -l`
来源：http://of.shxzskj.cn

C#:   Process.Start("ls", "-l");
来源：http://yd.chemitech.net.cn

[M04] 获取当前工作目录
来源：http://rw.gzmigu.cn

Py:   os.getcwd()
来源：http://xe.wgjwhj.cn

PHP:  getcwd();
来源：http://or.521024.cn

JS:   process.cwd()
来源：http://zb.huixinmuqiang.cn

TS:   process.cwd()
来源：http://rr.huixiangedu.cn

Java: Path.of("").toAbsolutePath()
来源：http://dl.521024.cn

Go:   os.Getwd()
来源：http://ui.gzmigu.cn

Ruby: Dir.pwd
来源：http://aw.jctech888.com.cn

C#:   Directory.GetCurrentDirectory()
来源：http://pt.colortex.cn

[M05] 设置退出码
来源：http://co.panjiajie.cn

Py:   sys.exit(1)
来源：http://qd.szsharing.cn

PHP:  exit(1);
来源：http://li.9csxet.cn

JS:   process.exit(1)
来源：http://vk.huanxung.cn

TS:   process.exit(1)
来源：http://yw.muxihuayi.cn

Java: System.exit(1)
来源：http://zu.521024.cn

Go:   os.Exit(1)
来源：http://qi.hnjuh.cn

Ruby: exit 1
来源：http://er.shxzukj.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://dm.panjiajie.cn

[M06] 向标准错误输出
来源：http://lq.muxihuayi.cn

Py:   print("err", file=sys.stderr)
来源：http://rd.huixiangedu.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://pd.gzmigu.cn

JS:   console.error("err")
来源：http://cf.huixinmuqiang.cn

TS:   console.error("err")
来源：http://vd.nszjky.cn

Java: System.err.println("err")
来源：http://po.yuexingan06.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://kb.newstarts.cn

Ruby: warn "err"
来源：http://qd.521024.cn

C#:   Console.Error.WriteLine("err")
来源：http://xy.newstarts.cn

[M07] 判断是否为主入口
来源：http://qz.nicolike.cn

Py:   if __name__ == "__main__":
来源：http://ax.yuntaijiaju.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://yf.haigaiapp.cn

JS:   require.main === module
来源：http://cw.hnjuh.cn

TS:   require.main === module
来源：http://za.chemitech.net.cn

Java: public static void main(String[] args)
来源：http://vl.shxzukj.cn

Go:   func main()
来源：http://mq.szxytkj.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ay.gzmigu.cn

C#:   static void Main(string[] args)
来源：http://on.asd995.cn

[M08] 获取系统与运行时信息
来源：http://uo.9csxet.cn

Py:   platform.system();  platform.python_version()
来源：http://kq.yuexingan06.cn

PHP:  PHP_OS;  phpversion();
来源：http://yk.nszjky.cn

JS:   process.platform;  process.version
来源：http://bs.shxzukj.cn

TS:   process.platform;  process.version
来源：http://ng.hahajie.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://re.szsharing.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://tx.asd995.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://jn.haigaiapp.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://bq.hahajie.cn

================================================================================
来源：http://el.bookmarksfly.cn

N. 数据结构与算法
来源：http://nv.bookmarksfly.cn

================================================================================
来源：http://kp.colortex.cn

[N01] 二分查找（有序数组）
来源：http://em.521024.cn

Py:   bisect.bisect_left(arr, x)
来源：http://dd.521024.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://rk.shxzskj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gk.nicolike.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://eu.nicolike.cn

Java: Arrays.binarySearch(arr, x)
来源：http://pq.bookmarksfly.cn

Go:   sort.SearchInts(arr, x)
来源：http://ac.newstarts.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://jq.huanxung.cn

C#:   Array.BinarySearch(arr, x)
来源：http://yv.szsharing.cn

[N02] 排序（工程实践用内置实现）
来源：http://fo.shtwfgs.cn

Py:   sorted(arr);  arr.sort()
来源：http://fl.yuexingan06.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://tx.nicolike.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://wp.panjiajie.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://xm.gzmigu.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://up.chemitech.net.cn

Go:   slices.Sort(arr)
来源：http://xb.jctech888.com.cn

Ruby: arr.sort
来源：http://vq.9csxet.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://jd.newstarts.cn

[N03] 快速排序（分治示例）
来源：http://zh.521024.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mc.lnxyls.cn

PHP:  // 递归实现，或用 usort
来源：http://tc.nicolike.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qa.nszjky.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mw.9csxet.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://xe.gzmigu.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://tv.nszjky.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://to.huixiangedu.cn

C#:   // 手写递归，或 Array.Sort
来源：http://mv.shtwfgs.cn

[N04] 斐波那契数列
来源：http://lj.yuntaijiaju.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://uf.521024.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://kq.hnjuh.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dz.nicolike.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xz.panjiajie.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://eb.muxihuayi.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://nn.yuntaijiaju.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://cs.haigaiapp.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://bb.szsharing.cn

[N05] 最大公约数
来源：http://cj.panjiajie.cn

Py:   math.gcd(a, b)
来源：http://ny.huanxung.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ep.huanxung.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ot.szxytkj.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ik.szsharing.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://qm.szxytkj.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ly.nszjky.cn

Ruby: a.gcd(b)
来源：http://jx.muxihuayi.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://gt.wgjwhj.cn

[N06] 判断回文字符串
来源：http://kw.bookmarksfly.cn

Py:   s == s[::-1]
来源：http://gi.huixinmuqiang.cn

PHP:  $s === strrev($s);
来源：http://eu.huanxung.cn

JS:   s === [...s].reverse().join("")
来源：http://tn.bjjhwx.cn

TS:   s === [...s].reverse().join("")
来源：http://vi.hnjuh.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ns.colortex.cn

Go:   // 双指针从两端比较
来源：http://kp.nicolike.cn

Ruby: s == s.reverse
来源：http://kc.asd995.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ri.jianghongdianzi.cn

[N07] 两数之和（返回下标）
来源：http://we.yuntaijiaju.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://dt.shxzukj.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://cn.szsharing.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://cr.panjiajie.cn

TS:   // 手写 Map<string, number>
来源：http://qd.chemitech.net.cn

Java: // 手写 HashMap
来源：http://be.9csxet.cn

Go:   // 手写 map[int]int
来源：http://om.panjiajie.cn

Ruby: // 手写 Hash
来源：http://ei.521024.cn

C#:   // 手写 Dictionary<int, int>
来源：http://dn.muxihuayi.cn

[N08] 生成全排列
来源：http://ja.szxytkj.cn

Py:   itertools.permutations(arr)
来源：http://xd.panjiajie.cn

PHP:  // 手写递归交换
来源：http://ax.shxzskj.cn

JS:   // 手写回溯递归
来源：http://xo.521024.cn

TS:   // 手写回溯递归
来源：http://ya.newstarts.cn


<!-- 参考信息 -->