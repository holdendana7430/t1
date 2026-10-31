代发 wailian999

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ci.huixiangedu.cn

Go:   json.Marshal(obj)
来源：http://tz.wgjwhj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ct.hnjuh.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://tc.521024.cn

[K02] JSON 字符串转对象
来源：http://tr.jctech888.com.cn

Py:   json.loads(s)
来源：http://gm.colortex.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://nc.szsharing.cn

JS:   JSON.parse(s)
来源：http://zp.muxihuayi.cn

TS:   JSON.parse(s)
来源：http://zm.huixinmuqiang.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://oi.521024.cn

Go:   json.Unmarshal(data, &v)
来源：http://fy.shtwfgs.cn

Ruby: JSON.parse(s)
来源：http://of.newstarts.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://td.hahajie.cn

[K03] JSON 美化输出（带缩进）
来源：http://sl.jianghongdianzi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wb.shxzskj.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ui.panjiajie.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://od.asd995.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://sj.asd995.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://fs.asd995.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ey.szxytkj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://yk.haigaiapp.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://oe.hnjuh.cn

[K04] 读取 JSON 文件
来源：http://yz.szxytkj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://fo.gzmigu.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ov.yuntaijiaju.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wc.huanxung.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tp.hahajie.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://qy.nszjky.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wb.chemitech.net.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://kz.huanxung.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://xa.shxzskj.cn

[K05] 深拷贝对象
来源：http://im.muxihuayi.cn

Py:   copy.deepcopy(obj)
来源：http://wr.gzmigu.cn

PHP:  unserialize(serialize($obj));
来源：http://td.shxzukj.cn

JS:   structuredClone(obj)
来源：http://ic.bookmarksfly.cn

TS:   structuredClone(obj)
来源：http://qj.hnjuh.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://qi.muxihuayi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wi.szsharing.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://uv.9csxet.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://qp.muxihuayi.cn

[K06] 解析 URL 查询串
来源：http://rj.lnxyls.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://fb.lnxyls.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://gh.521024.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jc.shxzskj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zi.shtwfgs.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://bl.huanxung.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://mg.gzmigu.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://fe.huanxung.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://pv.haigaiapp.cn

[K07] 进制转换
来源：http://wc.colortex.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://jk.hnjuh.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://qr.szsharing.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ux.shtwfgs.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://bp.shtwfgs.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://jk.shtwfgs.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ud.newstarts.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mi.muxihuayi.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wf.521024.cn

[K08] 二进制序列化（非 JSON）
来源：http://hc.newstarts.cn

Py:   pickle.dumps(obj)
来源：http://aa.lnxyls.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://bo.colortex.cn

JS:   v8.serialize(obj)        // Node
来源：http://zo.huixinmuqiang.cn

TS:   v8.serialize(obj)        // Node
来源：http://pq.wgjwhj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://tz.szsharing.cn

Go:   encoding/gob
来源：http://wm.newstarts.cn

Ruby: Marshal.dump(obj)
来源：http://qm.9csxet.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://pk.hahajie.cn

================================================================================
来源：http://mb.nicolike.cn

L. 网络请求
来源：http://ou.9csxet.cn

================================================================================
来源：http://eg.jctech888.com.cn

[L01] 发送 GET 请求
来源：http://wl.asd995.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ro.colortex.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vg.bjjhwx.cn

JS:   await fetch(url)
来源：http://xu.szsharing.cn

TS:   await fetch(url)
来源：http://fr.jctech888.com.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://nr.muxihuayi.cn

Go:   resp, err := http.Get(url)
来源：http://gm.chemitech.net.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://me.szsharing.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://eb.shxzskj.cn

[L02] 发送 POST JSON
来源：http://ky.colortex.cn

Py:   requests.post(url, json={"a": 1})
来源：http://eg.asd995.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://il.colortex.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mr.chemitech.net.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fq.szxytkj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vh.muxihuayi.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ye.jctech888.com.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://qj.9csxet.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wg.yuntaijiaju.cn

[L03] 设置自定义请求头
来源：http://lh.bookmarksfly.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://lt.nicolike.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://jn.shxzukj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bg.yuexingan06.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://om.hnjuh.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://oe.jianghongdianzi.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://sc.wgjwhj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://of.nicolike.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://aq.jctech888.com.cn

[L04] 设置超时
来源：http://vt.chemitech.net.cn

Py:   requests.get(url, timeout=5)
来源：http://qc.szxytkj.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://al.shxzukj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ah.bookmarksfly.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nt.nszjky.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://js.nszjky.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ja.nszjky.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://lk.chemitech.net.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://xi.jctech888.com.cn

[L05] 上传文件（multipart）
来源：http://js.huixinmuqiang.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://es.huixiangedu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://qc.huixiangedu.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ro.shxzskj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://om.9csxet.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://bd.huixinmuqiang.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://zw.jctech888.com.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://oc.asd995.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://bd.hnjuh.cn

[L06] 解析响应为 JSON
来源：http://rj.muxihuayi.cn

Py:   resp.json()
来源：http://mk.yuexingan06.cn

PHP:  json_decode($body, true);
来源：http://ma.muxihuayi.cn

JS:   await resp.json()
来源：http://oi.9csxet.cn

TS:   await resp.json()
来源：http://qc.jianghongdianzi.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hx.huanxung.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://eq.hnjuh.cn

Ruby: JSON.parse(resp.body)
来源：http://dc.nszjky.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://yu.yuexingan06.cn

[L07] 处理 HTTP 状态码
来源：http://xw.bookmarksfly.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://pd.colortex.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://zl.nicolike.cn

JS:   resp.ok;  resp.status
来源：http://cq.jctech888.com.cn

TS:   resp.ok;  resp.status
来源：http://xp.newstarts.cn

Java: resp.statusCode()
来源：http://en.9csxet.cn

Go:   resp.StatusCode
来源：http://ni.gzmigu.cn

Ruby: resp.code.to_i
来源：http://lw.huixiangedu.cn

C#:   (int)resp.StatusCode
来源：http://mx.hahajie.cn

[L08] 并发请求多个地址
来源：http://fc.huixinmuqiang.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://we.huixiangedu.cn

PHP:  curl_multi_init() 系列
来源：http://kg.huixiangedu.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fj.chemitech.net.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gs.huanxung.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ay.jctech888.com.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://kl.jctech888.com.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://lc.szsharing.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mr.bjjhwx.cn

================================================================================
来源：http://nv.colortex.cn

M. 命令行 / 进程 / 环境
来源：http://la.nicolike.cn

================================================================================
来源：http://co.asd995.cn

[M01] 读取命令行参数
来源：http://ik.huanxung.cn

Py:   sys.argv[1:]
来源：http://ok.shxzukj.cn

PHP:  $argv;  $argc;
来源：http://ee.panjiajie.cn

JS:   process.argv.slice(2)
来源：http://iu.shxzskj.cn

TS:   process.argv.slice(2)
来源：http://xx.hnjuh.cn

Java: args 数组（main 方法参数）
来源：http://kp.521024.cn

Go:   os.Args[1:]
来源：http://ad.521024.cn

Ruby: ARGV
来源：http://ar.muxihuayi.cn

C#:   args 数组（Main 方法参数）
来源：http://gj.hnjuh.cn

[M02] 读取环境变量
来源：http://uk.huixiangedu.cn

Py:   os.environ.get("HOME")
来源：http://fr.521024.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ck.colortex.cn

JS:   process.env.HOME
来源：http://kg.szxytkj.cn

TS:   process.env.HOME
来源：http://ui.hnjuh.cn

Java: System.getenv("HOME")
来源：http://as.hnjuh.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://dm.bjjhwx.cn

Ruby: ENV["HOME"]
来源：http://pr.huanxung.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://bx.asd995.cn

[M03] 执行外部命令
来源：http://wa.hahajie.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hh.panjiajie.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://yh.huixiangedu.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ha.muxihuayi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://kt.bjjhwx.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wy.yuexingan06.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://fb.yuntaijiaju.cn

Ruby: system("ls -l");  `ls -l`
来源：http://mg.chemitech.net.cn

C#:   Process.Start("ls", "-l");
来源：http://ic.shxzukj.cn

[M04] 获取当前工作目录
来源：http://xl.hahajie.cn

Py:   os.getcwd()
来源：http://lv.colortex.cn

PHP:  getcwd();
来源：http://ua.shxzskj.cn

JS:   process.cwd()
来源：http://bs.panjiajie.cn

TS:   process.cwd()
来源：http://sf.hnjuh.cn

Java: Path.of("").toAbsolutePath()
来源：http://yf.yuntaijiaju.cn

Go:   os.Getwd()
来源：http://ig.jctech888.com.cn

Ruby: Dir.pwd
来源：http://xv.chemitech.net.cn

C#:   Directory.GetCurrentDirectory()
来源：http://uq.huixiangedu.cn

[M05] 设置退出码
来源：http://db.szxytkj.cn

Py:   sys.exit(1)
来源：http://yj.hahajie.cn

PHP:  exit(1);
来源：http://gb.newstarts.cn

JS:   process.exit(1)
来源：http://bo.szxytkj.cn

TS:   process.exit(1)
来源：http://gk.huanxung.cn

Java: System.exit(1)
来源：http://dd.nicolike.cn

Go:   os.Exit(1)
来源：http://nc.lnxyls.cn

Ruby: exit 1
来源：http://nk.huixiangedu.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://oj.yuntaijiaju.cn

[M06] 向标准错误输出
来源：http://yf.haigaiapp.cn

Py:   print("err", file=sys.stderr)
来源：http://lp.hnjuh.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://vy.chemitech.net.cn

JS:   console.error("err")
来源：http://lz.szxytkj.cn

TS:   console.error("err")
来源：http://mn.shxzukj.cn

Java: System.err.println("err")
来源：http://pr.hnjuh.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wi.huanxung.cn

Ruby: warn "err"
来源：http://ik.colortex.cn

C#:   Console.Error.WriteLine("err")
来源：http://ei.shxzukj.cn

[M07] 判断是否为主入口
来源：http://xn.shxzukj.cn

Py:   if __name__ == "__main__":
来源：http://gz.hahajie.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://qo.muxihuayi.cn

JS:   require.main === module
来源：http://oa.9csxet.cn

TS:   require.main === module
来源：http://wp.szxytkj.cn

Java: public static void main(String[] args)
来源：http://ui.shtwfgs.cn

Go:   func main()
来源：http://xs.521024.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mk.wgjwhj.cn

C#:   static void Main(string[] args)
来源：http://oa.shxzukj.cn

[M08] 获取系统与运行时信息
来源：http://ju.nicolike.cn

Py:   platform.system();  platform.python_version()
来源：http://up.muxihuayi.cn

PHP:  PHP_OS;  phpversion();
来源：http://mw.huixinmuqiang.cn

JS:   process.platform;  process.version
来源：http://te.shxzukj.cn

TS:   process.platform;  process.version
来源：http://ac.shxzukj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xj.lnxyls.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://hw.panjiajie.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://dp.nszjky.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://xi.chemitech.net.cn

================================================================================
来源：http://zx.nszjky.cn

N. 数据结构与算法
来源：http://jq.bjjhwx.cn

================================================================================
来源：http://pj.jianghongdianzi.cn

[N01] 二分查找（有序数组）
来源：http://nj.jctech888.com.cn

Py:   bisect.bisect_left(arr, x)
来源：http://mi.shxzukj.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mn.wgjwhj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gn.huixinmuqiang.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mc.huanxung.cn

Java: Arrays.binarySearch(arr, x)
来源：http://aq.huanxung.cn

Go:   sort.SearchInts(arr, x)
来源：http://vi.nicolike.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://bj.shtwfgs.cn

C#:   Array.BinarySearch(arr, x)
来源：http://uc.huixiangedu.cn

[N02] 排序（工程实践用内置实现）
来源：http://ks.9csxet.cn

Py:   sorted(arr);  arr.sort()
来源：http://am.9csxet.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mu.chemitech.net.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://vq.nicolike.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://pl.shxzukj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ui.521024.cn

Go:   slices.Sort(arr)
来源：http://hm.szxytkj.cn

Ruby: arr.sort
来源：http://mf.gzmigu.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://vi.asd995.cn

[N03] 快速排序（分治示例）
来源：http://nb.bjjhwx.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://np.wgjwhj.cn

PHP:  // 递归实现，或用 usort
来源：http://vz.wgjwhj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ac.panjiajie.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lx.asd995.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://bg.yuntaijiaju.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ab.chemitech.net.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://sp.bjjhwx.cn

C#:   // 手写递归，或 Array.Sort
来源：http://aq.yuexingan06.cn

[N04] 斐波那契数列
来源：http://jo.newstarts.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://tw.nicolike.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://tb.haigaiapp.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sc.bookmarksfly.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rk.bjjhwx.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://an.chemitech.net.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hv.nszjky.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ba.chemitech.net.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mg.nszjky.cn

[N05] 最大公约数
来源：http://yb.shtwfgs.cn

Py:   math.gcd(a, b)
来源：http://rp.9csxet.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://fo.haigaiapp.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dy.521024.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fj.521024.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://cc.asd995.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://nu.huixiangedu.cn

Ruby: a.gcd(b)
来源：http://jc.huanxung.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ln.521024.cn

[N06] 判断回文字符串
来源：http://io.shxzukj.cn

Py:   s == s[::-1]
来源：http://qq.jianghongdianzi.cn

PHP:  $s === strrev($s);
来源：http://mj.nicolike.cn

JS:   s === [...s].reverse().join("")
来源：http://qw.jianghongdianzi.cn

TS:   s === [...s].reverse().join("")
来源：http://lb.shxzukj.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mc.haigaiapp.cn

Go:   // 双指针从两端比较
来源：http://ir.yuexingan06.cn

Ruby: s == s.reverse
来源：http://jq.521024.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://cl.gzmigu.cn

[N07] 两数之和（返回下标）
来源：http://qu.haigaiapp.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ee.haigaiapp.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://fu.szxytkj.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://oh.bookmarksfly.cn

TS:   // 手写 Map<string, number>
来源：http://dx.asd995.cn

Java: // 手写 HashMap
来源：http://mi.bookmarksfly.cn

Go:   // 手写 map[int]int
来源：http://ee.gzmigu.cn

Ruby: // 手写 Hash
来源：http://jf.jianghongdianzi.cn

C#:   // 手写 Dictionary<int, int>
来源：http://iw.huixinmuqiang.cn

[N08] 生成全排列
来源：http://ro.bookmarksfly.cn

Py:   itertools.permutations(arr)
来源：http://eb.jianghongdianzi.cn

PHP:  // 手写递归交换
来源：http://fs.hnjuh.cn

JS:   // 手写回溯递归
来源：http://ov.yuntaijiaju.cn

TS:   // 手写回溯递归
来源：http://jl.asd995.cn

Java: // 手写回溯递归
来源：http://ri.wgjwhj.cn

Go:   // 手写回溯递归
来源：http://tb.szsharing.cn

Ruby: arr.permutation.to_a
来源：http://ex.shxzukj.cn

C#:   // 手写回溯递归
来源：http://up.nicolike.cn

[N09] 栈与队列
来源：http://rz.muxihuayi.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://zr.colortex.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mj.gzmigu.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://pi.521024.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ep.hahajie.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://dz.nszjky.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ll.huixiangedu.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://zr.bookmarksfly.cn


<!-- 参考信息 -->