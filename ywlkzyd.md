代发 wailian999

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://eu.huixinmuqiang.cn

Go:   json.Marshal(obj)
来源：http://iu.bjjhwx.cn

Ruby: obj.to_json                                     // require "json"
来源：http://dr.chemitech.net.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://cz.muxihuayi.cn

[K02] JSON 字符串转对象
来源：http://bj.hahajie.cn

Py:   json.loads(s)
来源：http://bd.lnxyls.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ox.hahajie.cn

JS:   JSON.parse(s)
来源：http://de.shxzskj.cn

TS:   JSON.parse(s)
来源：http://rr.haigaiapp.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://rp.szsharing.cn

Go:   json.Unmarshal(data, &v)
来源：http://ei.shxzukj.cn

Ruby: JSON.parse(s)
来源：http://bi.bookmarksfly.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://lq.gzmigu.cn

[K03] JSON 美化输出（带缩进）
来源：http://py.shtwfgs.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hx.huanxung.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://di.wgjwhj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://zk.huanxung.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://re.chemitech.net.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://or.jianghongdianzi.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://zx.bookmarksfly.cn

Ruby: JSON.pretty_generate(obj)
来源：http://xc.bookmarksfly.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://nk.hahajie.cn

[K04] 读取 JSON 文件
来源：http://eu.9csxet.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wa.colortex.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://tc.hnjuh.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hd.szsharing.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://in.lnxyls.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://iq.hahajie.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://pv.szxytkj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://kz.huanxung.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://xz.szxytkj.cn

[K05] 深拷贝对象
来源：http://mj.521024.cn

Py:   copy.deepcopy(obj)
来源：http://ie.wgjwhj.cn

PHP:  unserialize(serialize($obj));
来源：http://sd.szsharing.cn

JS:   structuredClone(obj)
来源：http://xe.nicolike.cn

TS:   structuredClone(obj)
来源：http://li.nicolike.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://bi.newstarts.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zd.chemitech.net.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://xu.muxihuayi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ce.nszjky.cn

[K06] 解析 URL 查询串
来源：http://fj.jctech888.com.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://gl.shxzukj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://or.wgjwhj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ag.nszjky.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ds.huixinmuqiang.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://dk.panjiajie.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://au.asd995.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vl.huixinmuqiang.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://yb.colortex.cn

[K07] 进制转换
来源：http://pu.szsharing.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://zx.newstarts.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://bm.lnxyls.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://on.bjjhwx.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://zj.yuntaijiaju.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://vu.asd995.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ks.9csxet.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://cc.huixiangedu.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://bc.yuexingan06.cn

[K08] 二进制序列化（非 JSON）
来源：http://sx.muxihuayi.cn

Py:   pickle.dumps(obj)
来源：http://ll.huixinmuqiang.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://wt.jianghongdianzi.cn

JS:   v8.serialize(obj)        // Node
来源：http://ur.muxihuayi.cn

TS:   v8.serialize(obj)        // Node
来源：http://lq.hahajie.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ak.bjjhwx.cn

Go:   encoding/gob
来源：http://jp.9csxet.cn

Ruby: Marshal.dump(obj)
来源：http://aa.yuexingan06.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://di.nszjky.cn

================================================================================
来源：http://ea.521024.cn

L. 网络请求
来源：http://do.asd995.cn

================================================================================
来源：http://nc.huixiangedu.cn

[L01] 发送 GET 请求
来源：http://do.521024.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jr.panjiajie.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://le.shxzukj.cn

JS:   await fetch(url)
来源：http://ym.nszjky.cn

TS:   await fetch(url)
来源：http://mi.hahajie.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hv.yuntaijiaju.cn

Go:   resp, err := http.Get(url)
来源：http://il.bjjhwx.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://qc.nszjky.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://fj.bjjhwx.cn

[L02] 发送 POST JSON
来源：http://pa.bjjhwx.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ma.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://jd.newstarts.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ai.szxytkj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bp.gzmigu.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://op.huixiangedu.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ml.colortex.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://er.shxzskj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://bc.chemitech.net.cn

[L03] 设置自定义请求头
来源：http://cq.9csxet.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://su.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://bb.hnjuh.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kr.panjiajie.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qw.chemitech.net.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://cb.shxzskj.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://fr.haigaiapp.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ts.asd995.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://og.szxytkj.cn

[L04] 设置超时
来源：http://qw.lnxyls.cn

Py:   requests.get(url, timeout=5)
来源：http://ne.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://zf.9csxet.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://oz.bookmarksfly.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ng.muxihuayi.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://jx.colortex.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://jg.newstarts.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hh.shxzskj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://dh.newstarts.cn

[L05] 上传文件（multipart）
来源：http://yy.hnjuh.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://jz.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://cd.bookmarksfly.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://xs.asd995.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://rd.521024.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://os.bjjhwx.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ye.chemitech.net.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://lv.wgjwhj.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://is.asd995.cn

[L06] 解析响应为 JSON
来源：http://sw.bjjhwx.cn

Py:   resp.json()
来源：http://sv.jianghongdianzi.cn

PHP:  json_decode($body, true);
来源：http://nu.hahajie.cn

JS:   await resp.json()
来源：http://rf.lnxyls.cn

TS:   await resp.json()
来源：http://di.huixiangedu.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ij.bookmarksfly.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://rq.chemitech.net.cn

Ruby: JSON.parse(resp.body)
来源：http://fr.chemitech.net.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mz.szxytkj.cn

[L07] 处理 HTTP 状态码
来源：http://hl.yuexingan06.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://tm.hnjuh.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://sy.muxihuayi.cn

JS:   resp.ok;  resp.status
来源：http://ib.huixiangedu.cn

TS:   resp.ok;  resp.status
来源：http://om.huixiangedu.cn

Java: resp.statusCode()
来源：http://mg.newstarts.cn

Go:   resp.StatusCode
来源：http://sq.521024.cn

Ruby: resp.code.to_i
来源：http://bc.jctech888.com.cn

C#:   (int)resp.StatusCode
来源：http://tn.521024.cn

[L08] 并发请求多个地址
来源：http://ai.wgjwhj.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://la.asd995.cn

PHP:  curl_multi_init() 系列
来源：http://mo.bookmarksfly.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hg.lnxyls.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wa.panjiajie.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://qx.chemitech.net.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://gy.shxzukj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://kl.szsharing.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://zg.shxzukj.cn

================================================================================
来源：http://df.huixinmuqiang.cn

M. 命令行 / 进程 / 环境
来源：http://fv.nicolike.cn

================================================================================
来源：http://pn.shxzukj.cn

[M01] 读取命令行参数
来源：http://ps.9csxet.cn

Py:   sys.argv[1:]
来源：http://vd.shtwfgs.cn

PHP:  $argv;  $argc;
来源：http://av.huixinmuqiang.cn

JS:   process.argv.slice(2)
来源：http://zs.huixinmuqiang.cn

TS:   process.argv.slice(2)
来源：http://nw.shxzukj.cn

Java: args 数组（main 方法参数）
来源：http://yj.hnjuh.cn

Go:   os.Args[1:]
来源：http://sb.asd995.cn

Ruby: ARGV
来源：http://tc.chemitech.net.cn

C#:   args 数组（Main 方法参数）
来源：http://gw.9csxet.cn

[M02] 读取环境变量
来源：http://ff.hnjuh.cn

Py:   os.environ.get("HOME")
来源：http://zi.gzmigu.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://fu.hahajie.cn

JS:   process.env.HOME
来源：http://nk.nszjky.cn

TS:   process.env.HOME
来源：http://zl.szsharing.cn

Java: System.getenv("HOME")
来源：http://fi.nicolike.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://et.panjiajie.cn

Ruby: ENV["HOME"]
来源：http://qx.szsharing.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://zl.shtwfgs.cn

[M03] 执行外部命令
来源：http://bc.huanxung.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://dq.9csxet.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://rx.shxzukj.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://xk.newstarts.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://oh.haigaiapp.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://pw.gzmigu.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://vu.nszjky.cn

Ruby: system("ls -l");  `ls -l`
来源：http://yp.shtwfgs.cn

C#:   Process.Start("ls", "-l");
来源：http://uk.521024.cn

[M04] 获取当前工作目录
来源：http://ua.haigaiapp.cn

Py:   os.getcwd()
来源：http://cr.bjjhwx.cn

PHP:  getcwd();
来源：http://nz.wgjwhj.cn

JS:   process.cwd()
来源：http://xx.huixiangedu.cn

TS:   process.cwd()
来源：http://nt.bookmarksfly.cn

Java: Path.of("").toAbsolutePath()
来源：http://mi.shxzukj.cn

Go:   os.Getwd()
来源：http://mq.lnxyls.cn

Ruby: Dir.pwd
来源：http://do.panjiajie.cn

C#:   Directory.GetCurrentDirectory()
来源：http://gb.yuntaijiaju.cn

[M05] 设置退出码
来源：http://yq.bookmarksfly.cn

Py:   sys.exit(1)
来源：http://vw.jctech888.com.cn

PHP:  exit(1);
来源：http://mw.yuexingan06.cn

JS:   process.exit(1)
来源：http://ti.wgjwhj.cn

TS:   process.exit(1)
来源：http://ur.yuntaijiaju.cn

Java: System.exit(1)
来源：http://mv.nszjky.cn

Go:   os.Exit(1)
来源：http://gr.muxihuayi.cn

Ruby: exit 1
来源：http://dn.nicolike.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://cd.nicolike.cn

[M06] 向标准错误输出
来源：http://la.wgjwhj.cn

Py:   print("err", file=sys.stderr)
来源：http://fq.hahajie.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ki.wgjwhj.cn

JS:   console.error("err")
来源：http://us.huanxung.cn

TS:   console.error("err")
来源：http://xi.huixinmuqiang.cn

Java: System.err.println("err")
来源：http://im.shxzukj.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://jw.shtwfgs.cn

Ruby: warn "err"
来源：http://bm.huanxung.cn

C#:   Console.Error.WriteLine("err")
来源：http://cv.521024.cn

[M07] 判断是否为主入口
来源：http://kv.huanxung.cn

Py:   if __name__ == "__main__":
来源：http://pu.9csxet.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ti.haigaiapp.cn

JS:   require.main === module
来源：http://hk.9csxet.cn

TS:   require.main === module
来源：http://tp.gzmigu.cn

Java: public static void main(String[] args)
来源：http://km.panjiajie.cn

Go:   func main()
来源：http://jz.huixinmuqiang.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://lf.yuntaijiaju.cn

C#:   static void Main(string[] args)
来源：http://hw.hahajie.cn

[M08] 获取系统与运行时信息
来源：http://nd.hnjuh.cn

Py:   platform.system();  platform.python_version()
来源：http://px.shtwfgs.cn

PHP:  PHP_OS;  phpversion();
来源：http://mv.huixiangedu.cn

JS:   process.platform;  process.version
来源：http://vo.huanxung.cn

TS:   process.platform;  process.version
来源：http://eh.newstarts.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ht.panjiajie.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ll.chemitech.net.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://oj.shxzskj.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://as.asd995.cn

================================================================================
来源：http://lf.szsharing.cn

N. 数据结构与算法
来源：http://ot.nicolike.cn

================================================================================
来源：http://js.muxihuayi.cn

[N01] 二分查找（有序数组）
来源：http://wz.jctech888.com.cn

Py:   bisect.bisect_left(arr, x)
来源：http://nz.nicolike.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://xx.chemitech.net.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sd.yuexingan06.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.hnjuh.cn

Java: Arrays.binarySearch(arr, x)
来源：http://gz.asd995.cn

Go:   sort.SearchInts(arr, x)
来源：http://ky.521024.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://fx.huanxung.cn

C#:   Array.BinarySearch(arr, x)
来源：http://sd.hnjuh.cn

[N02] 排序（工程实践用内置实现）
来源：http://qb.lnxyls.cn

Py:   sorted(arr);  arr.sort()
来源：http://md.asd995.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://kn.szxytkj.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ag.lnxyls.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://og.szxytkj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://lw.hnjuh.cn

Go:   slices.Sort(arr)
来源：http://rv.bookmarksfly.cn

Ruby: arr.sort
来源：http://ii.huixinmuqiang.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://bm.asd995.cn

[N03] 快速排序（分治示例）
来源：http://id.shxzukj.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wn.huixinmuqiang.cn

PHP:  // 递归实现，或用 usort
来源：http://sg.yuexingan06.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qh.newstarts.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rt.bjjhwx.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://pf.jianghongdianzi.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ez.shtwfgs.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://sa.asd995.cn

C#:   // 手写递归，或 Array.Sort
来源：http://zt.nszjky.cn

[N04] 斐波那契数列
来源：http://lb.huixiangedu.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://uo.bookmarksfly.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://te.lnxyls.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xv.lnxyls.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sj.nicolike.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://tn.gzmigu.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ax.nicolike.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ou.huixinmuqiang.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://rn.colortex.cn

[N05] 最大公约数
来源：http://je.shtwfgs.cn

Py:   math.gcd(a, b)
来源：http://qh.nszjky.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://bu.9csxet.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dh.wgjwhj.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://za.szsharing.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://jw.chemitech.net.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://zk.lnxyls.cn

Ruby: a.gcd(b)
来源：http://js.gzmigu.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://pl.haigaiapp.cn

[N06] 判断回文字符串
来源：http://zk.yuntaijiaju.cn

Py:   s == s[::-1]
来源：http://qs.lnxyls.cn

PHP:  $s === strrev($s);
来源：http://zs.gzmigu.cn

JS:   s === [...s].reverse().join("")
来源：http://ab.huixinmuqiang.cn

TS:   s === [...s].reverse().join("")
来源：http://gc.chemitech.net.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ce.asd995.cn

Go:   // 双指针从两端比较
来源：http://pu.lnxyls.cn

Ruby: s == s.reverse
来源：http://wq.nicolike.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://yb.shtwfgs.cn

[N07] 两数之和（返回下标）
来源：http://bb.shtwfgs.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://in.yuexingan06.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://qn.newstarts.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://py.yuntaijiaju.cn

TS:   // 手写 Map<string, number>
来源：http://rk.bjjhwx.cn

Java: // 手写 HashMap
来源：http://vo.shxzskj.cn

Go:   // 手写 map[int]int
来源：http://vt.asd995.cn

Ruby: // 手写 Hash
来源：http://ee.lnxyls.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ks.shxzskj.cn

[N08] 生成全排列
来源：http://dj.szsharing.cn

Py:   itertools.permutations(arr)
来源：http://ka.szxytkj.cn

PHP:  // 手写递归交换
来源：http://af.newstarts.cn

JS:   // 手写回溯递归
来源：http://fc.huanxung.cn

TS:   // 手写回溯递归
来源：http://xx.9csxet.cn

Java: // 手写回溯递归
来源：http://om.shtwfgs.cn

Go:   // 手写回溯递归
来源：http://ha.huixiangedu.cn

Ruby: arr.permutation.to_a
来源：http://bt.lnxyls.cn

C#:   // 手写回溯递归
来源：http://pd.huanxung.cn

[N09] 栈与队列
来源：http://jl.huanxung.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://vv.huixinmuqiang.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://yx.asd995.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://sk.bookmarksfly.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://xi.huanxung.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://pg.hnjuh.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://nu.521024.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://fa.shxzskj.cn


<!-- 参考信息 -->