代发 wailian999

================================================================================
来源：http://bw.hahajie.cn

K. JSON 与序列化
来源：http://vq.colortex.cn

================================================================================
来源：http://oc.muxihuayi.cn

[K01] 对象转 JSON 字符串
来源：http://jg.yuexingan06.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://gm.wgjwhj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://oq.yuntaijiaju.cn

JS:   JSON.stringify(obj)
来源：http://xn.hnjuh.cn

TS:   JSON.stringify(obj)
来源：http://zx.huixiangedu.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://vv.panjiajie.cn

Go:   json.Marshal(obj)
来源：http://on.bookmarksfly.cn

Ruby: obj.to_json                                     // require "json"
来源：http://vk.jianghongdianzi.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ht.chemitech.net.cn

[K02] JSON 字符串转对象
来源：http://vi.nicolike.cn

Py:   json.loads(s)
来源：http://bz.hahajie.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://fn.bookmarksfly.cn

JS:   JSON.parse(s)
来源：http://cl.newstarts.cn

TS:   JSON.parse(s)
来源：http://he.haigaiapp.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://rb.jctech888.com.cn

Go:   json.Unmarshal(data, &v)
来源：http://sq.yuntaijiaju.cn

Ruby: JSON.parse(s)
来源：http://kp.chemitech.net.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://en.9csxet.cn

[K03] JSON 美化输出（带缩进）
来源：http://pu.nszjky.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mj.colortex.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://kq.colortex.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://yr.yuntaijiaju.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://vr.chemitech.net.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://zx.gzmigu.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://fy.huanxung.cn

Ruby: JSON.pretty_generate(obj)
来源：http://jr.muxihuayi.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://dz.chemitech.net.cn

[K04] 读取 JSON 文件
来源：http://rn.gzmigu.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://rd.huixinmuqiang.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://xg.panjiajie.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vz.yuntaijiaju.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pb.gzmigu.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wt.huixiangedu.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://qg.szsharing.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://vd.huanxung.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://or.jctech888.com.cn

[K05] 深拷贝对象
来源：http://ve.haigaiapp.cn

Py:   copy.deepcopy(obj)
来源：http://iv.huanxung.cn

PHP:  unserialize(serialize($obj));
来源：http://me.521024.cn

JS:   structuredClone(obj)
来源：http://ty.wgjwhj.cn

TS:   structuredClone(obj)
来源：http://mh.bjjhwx.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ch.yuntaijiaju.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://vb.bookmarksfly.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://za.lnxyls.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://rc.szsharing.cn

[K06] 解析 URL 查询串
来源：http://nd.szxytkj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mk.muxihuayi.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://al.chemitech.net.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ta.yuntaijiaju.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uu.bookmarksfly.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wi.hahajie.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://gu.shxzukj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ev.wgjwhj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zz.shxzskj.cn

[K07] 进制转换
来源：http://fj.panjiajie.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ds.huixinmuqiang.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://zo.huanxung.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ix.521024.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://tf.szxytkj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://pz.szsharing.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://cs.haigaiapp.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://vu.521024.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hs.yuntaijiaju.cn

[K08] 二进制序列化（非 JSON）
来源：http://zk.panjiajie.cn

Py:   pickle.dumps(obj)
来源：http://nn.bookmarksfly.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://sd.huanxung.cn

JS:   v8.serialize(obj)        // Node
来源：http://rq.yuntaijiaju.cn

TS:   v8.serialize(obj)        // Node
来源：http://dx.huanxung.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://pf.muxihuayi.cn

Go:   encoding/gob
来源：http://ww.jianghongdianzi.cn

Ruby: Marshal.dump(obj)
来源：http://xz.gzmigu.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://aj.panjiajie.cn

================================================================================
来源：http://pt.szsharing.cn

L. 网络请求
来源：http://ww.colortex.cn

================================================================================
来源：http://xc.bjjhwx.cn

[L01] 发送 GET 请求
来源：http://ak.9csxet.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://qw.shxzukj.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hm.szxytkj.cn

JS:   await fetch(url)
来源：http://tb.panjiajie.cn

TS:   await fetch(url)
来源：http://sf.asd995.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hj.yuexingan06.cn

Go:   resp, err := http.Get(url)
来源：http://hz.muxihuayi.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://pj.wgjwhj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ac.yuntaijiaju.cn

[L02] 发送 POST JSON
来源：http://er.521024.cn

Py:   requests.post(url, json={"a": 1})
来源：http://kq.asd995.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ax.szsharing.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pr.huixiangedu.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lf.yuexingan06.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wq.huixinmuqiang.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qg.huanxung.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://fo.hahajie.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://nq.yuexingan06.cn

[L03] 设置自定义请求头
来源：http://yf.jianghongdianzi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://sb.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://de.shxzskj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jc.shxzskj.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nn.haigaiapp.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://va.hnjuh.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://aw.szxytkj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qz.colortex.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mi.haigaiapp.cn

[L04] 设置超时
来源：http://ps.bjjhwx.cn

Py:   requests.get(url, timeout=5)
来源：http://qi.521024.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ao.chemitech.net.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zt.shxzukj.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zs.panjiajie.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://jn.hnjuh.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ho.yuntaijiaju.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ww.jianghongdianzi.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://rg.chemitech.net.cn

[L05] 上传文件（multipart）
来源：http://nv.huixiangedu.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://kb.haigaiapp.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://yz.wgjwhj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hi.hahajie.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://vq.wgjwhj.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://el.newstarts.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://jr.colortex.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://io.bjjhwx.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ky.521024.cn

[L06] 解析响应为 JSON
来源：http://xo.huixinmuqiang.cn

Py:   resp.json()
来源：http://ba.szxytkj.cn

PHP:  json_decode($body, true);
来源：http://dr.newstarts.cn

JS:   await resp.json()
来源：http://af.shxzukj.cn

TS:   await resp.json()
来源：http://qo.yuexingan06.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://yv.shxzskj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ss.9csxet.cn

Ruby: JSON.parse(resp.body)
来源：http://iu.haigaiapp.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ld.hnjuh.cn

[L07] 处理 HTTP 状态码
来源：http://nd.lnxyls.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://vi.521024.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://xx.shxzukj.cn

JS:   resp.ok;  resp.status
来源：http://rn.szsharing.cn

TS:   resp.ok;  resp.status
来源：http://xi.nicolike.cn

Java: resp.statusCode()
来源：http://it.asd995.cn

Go:   resp.StatusCode
来源：http://at.huixinmuqiang.cn

Ruby: resp.code.to_i
来源：http://ug.gzmigu.cn

C#:   (int)resp.StatusCode
来源：http://wb.hahajie.cn

[L08] 并发请求多个地址
来源：http://yn.nicolike.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://to.hnjuh.cn

PHP:  curl_multi_init() 系列
来源：http://dc.newstarts.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rl.huanxung.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://os.huixiangedu.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://sm.newstarts.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://tc.bjjhwx.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://yr.panjiajie.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://md.yuexingan06.cn

================================================================================
来源：http://pl.asd995.cn

M. 命令行 / 进程 / 环境
来源：http://mi.shxzskj.cn

================================================================================
来源：http://bb.huanxung.cn

[M01] 读取命令行参数
来源：http://rp.wgjwhj.cn

Py:   sys.argv[1:]
来源：http://va.yuexingan06.cn

PHP:  $argv;  $argc;
来源：http://pd.yuntaijiaju.cn

JS:   process.argv.slice(2)
来源：http://lq.huixinmuqiang.cn

TS:   process.argv.slice(2)
来源：http://fd.shtwfgs.cn

Java: args 数组（main 方法参数）
来源：http://xe.haigaiapp.cn

Go:   os.Args[1:]
来源：http://mg.muxihuayi.cn

Ruby: ARGV
来源：http://vu.huixinmuqiang.cn

C#:   args 数组（Main 方法参数）
来源：http://vy.521024.cn

[M02] 读取环境变量
来源：http://pl.hnjuh.cn

Py:   os.environ.get("HOME")
来源：http://uq.huanxung.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://pp.jianghongdianzi.cn

JS:   process.env.HOME
来源：http://uh.hnjuh.cn

TS:   process.env.HOME
来源：http://wb.panjiajie.cn

Java: System.getenv("HOME")
来源：http://nr.gzmigu.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://pk.521024.cn

Ruby: ENV["HOME"]
来源：http://qn.nicolike.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://cq.lnxyls.cn

[M03] 执行外部命令
来源：http://jm.nicolike.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wy.newstarts.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://cd.9csxet.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://qz.9csxet.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://rw.bookmarksfly.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://tz.gzmigu.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://xq.hnjuh.cn

Ruby: system("ls -l");  `ls -l`
来源：http://px.huixiangedu.cn

C#:   Process.Start("ls", "-l");
来源：http://aa.szxytkj.cn

[M04] 获取当前工作目录
来源：http://mc.haigaiapp.cn

Py:   os.getcwd()
来源：http://du.szxytkj.cn

PHP:  getcwd();
来源：http://el.newstarts.cn

JS:   process.cwd()
来源：http://yd.muxihuayi.cn

TS:   process.cwd()
来源：http://ld.hnjuh.cn

Java: Path.of("").toAbsolutePath()
来源：http://xt.huixiangedu.cn

Go:   os.Getwd()
来源：http://au.haigaiapp.cn

Ruby: Dir.pwd
来源：http://xx.9csxet.cn

C#:   Directory.GetCurrentDirectory()
来源：http://pu.chemitech.net.cn

[M05] 设置退出码
来源：http://xj.nicolike.cn

Py:   sys.exit(1)
来源：http://bb.szsharing.cn

PHP:  exit(1);
来源：http://tx.gzmigu.cn

JS:   process.exit(1)
来源：http://zz.asd995.cn

TS:   process.exit(1)
来源：http://gp.nszjky.cn

Java: System.exit(1)
来源：http://mw.shxzukj.cn

Go:   os.Exit(1)
来源：http://jj.yuexingan06.cn

Ruby: exit 1
来源：http://ft.panjiajie.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://vk.yuntaijiaju.cn

[M06] 向标准错误输出
来源：http://go.huanxung.cn

Py:   print("err", file=sys.stderr)
来源：http://mc.chemitech.net.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://xv.yuexingan06.cn

JS:   console.error("err")
来源：http://xm.huanxung.cn

TS:   console.error("err")
来源：http://dj.haigaiapp.cn

Java: System.err.println("err")
来源：http://qh.haigaiapp.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://dx.shxzukj.cn

Ruby: warn "err"
来源：http://si.szxytkj.cn

C#:   Console.Error.WriteLine("err")
来源：http://ai.hahajie.cn

[M07] 判断是否为主入口
来源：http://rr.asd995.cn

Py:   if __name__ == "__main__":
来源：http://of.colortex.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ec.haigaiapp.cn

JS:   require.main === module
来源：http://qa.shtwfgs.cn

TS:   require.main === module
来源：http://bw.shtwfgs.cn

Java: public static void main(String[] args)
来源：http://bs.muxihuayi.cn

Go:   func main()
来源：http://jx.bookmarksfly.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://bx.hnjuh.cn

C#:   static void Main(string[] args)
来源：http://pf.yuntaijiaju.cn

[M08] 获取系统与运行时信息
来源：http://cg.muxihuayi.cn

Py:   platform.system();  platform.python_version()
来源：http://ki.bookmarksfly.cn

PHP:  PHP_OS;  phpversion();
来源：http://mf.huixinmuqiang.cn

JS:   process.platform;  process.version
来源：http://zt.newstarts.cn

TS:   process.platform;  process.version
来源：http://fh.lnxyls.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://rj.huixiangedu.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://td.shxzukj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://gs.wgjwhj.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://kl.jctech888.com.cn

================================================================================
来源：http://ni.hahajie.cn

N. 数据结构与算法
来源：http://nj.nszjky.cn

================================================================================
来源：http://ak.huanxung.cn

[N01] 二分查找（有序数组）
来源：http://oo.bookmarksfly.cn

Py:   bisect.bisect_left(arr, x)
来源：http://hz.panjiajie.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ad.chemitech.net.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ax.yuexingan06.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pu.521024.cn

Java: Arrays.binarySearch(arr, x)
来源：http://xf.hahajie.cn

Go:   sort.SearchInts(arr, x)
来源：http://yx.yuntaijiaju.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://fu.szxytkj.cn

C#:   Array.BinarySearch(arr, x)
来源：http://hu.lnxyls.cn

[N02] 排序（工程实践用内置实现）
来源：http://tb.colortex.cn

Py:   sorted(arr);  arr.sort()
来源：http://cr.lnxyls.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://kk.colortex.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://qs.521024.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://tl.newstarts.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ee.nicolike.cn

Go:   slices.Sort(arr)
来源：http://tg.shtwfgs.cn

Ruby: arr.sort
来源：http://ce.huanxung.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://zp.nszjky.cn

[N03] 快速排序（分治示例）
来源：http://hd.newstarts.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://sh.szsharing.cn

PHP:  // 递归实现，或用 usort
来源：http://pc.colortex.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fl.chemitech.net.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hc.chemitech.net.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://kj.huanxung.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ez.jianghongdianzi.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://jh.szsharing.cn

C#:   // 手写递归，或 Array.Sort
来源：http://us.9csxet.cn

[N04] 斐波那契数列
来源：http://ss.panjiajie.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://he.szxytkj.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mu.chemitech.net.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wl.yuexingan06.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pl.shxzukj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ci.shxzskj.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://gf.bjjhwx.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://im.wgjwhj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://bi.shxzskj.cn

[N05] 最大公约数
来源：http://fu.colortex.cn

Py:   math.gcd(a, b)
来源：http://rd.bookmarksfly.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ee.jctech888.com.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://uh.haigaiapp.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cy.newstarts.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mw.hnjuh.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://bb.huixinmuqiang.cn

Ruby: a.gcd(b)
来源：http://xd.bookmarksfly.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://sf.yuexingan06.cn

[N06] 判断回文字符串
来源：http://qn.muxihuayi.cn

Py:   s == s[::-1]
来源：http://ry.jianghongdianzi.cn

PHP:  $s === strrev($s);
来源：http://fb.shxzukj.cn

JS:   s === [...s].reverse().join("")
来源：http://oa.muxihuayi.cn

TS:   s === [...s].reverse().join("")
来源：http://rz.huixinmuqiang.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://bi.chemitech.net.cn

Go:   // 双指针从两端比较
来源：http://pf.yuntaijiaju.cn

Ruby: s == s.reverse
来源：http://ec.colortex.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://fs.wgjwhj.cn

[N07] 两数之和（返回下标）
来源：http://pp.yuexingan06.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ye.lnxyls.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://uv.yuexingan06.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://yh.szsharing.cn

TS:   // 手写 Map<string, number>
来源：http://dg.jianghongdianzi.cn

Java: // 手写 HashMap
来源：http://vn.shtwfgs.cn

Go:   // 手写 map[int]int
来源：http://eq.asd995.cn

Ruby: // 手写 Hash
来源：http://vu.yuexingan06.cn

C#:   // 手写 Dictionary<int, int>
来源：http://tm.shxzskj.cn

[N08] 生成全排列
来源：http://mm.9csxet.cn

Py:   itertools.permutations(arr)
来源：http://qx.hahajie.cn

PHP:  // 手写递归交换
来源：http://se.9csxet.cn

JS:   // 手写回溯递归
来源：http://rw.lnxyls.cn

TS:   // 手写回溯递归
来源：http://ax.colortex.cn

Java: // 手写回溯递归
来源：http://gu.wgjwhj.cn

Go:   // 手写回溯递归
来源：http://no.wgjwhj.cn

Ruby: arr.permutation.to_a
来源：http://ts.szsharing.cn

C#:   // 手写回溯递归
来源：http://qg.bookmarksfly.cn


<!-- 参考信息 -->