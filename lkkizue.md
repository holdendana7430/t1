代发 wailian999

================================================================================
来源：http://ez.chemitech.net.cn

K. JSON 与序列化
来源：http://ex.yuexingan06.cn

================================================================================
来源：http://qc.asd995.cn

[K01] 对象转 JSON 字符串
来源：http://xi.jctech888.com.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://tg.panjiajie.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://aw.lnxyls.cn

JS:   JSON.stringify(obj)
来源：http://vi.yuexingan06.cn

TS:   JSON.stringify(obj)
来源：http://it.shxzukj.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://pd.shtwfgs.cn

Go:   json.Marshal(obj)
来源：http://rm.bjjhwx.cn

Ruby: obj.to_json                                     // require "json"
来源：http://sf.nszjky.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://dv.521024.cn

[K02] JSON 字符串转对象
来源：http://ze.muxihuayi.cn

Py:   json.loads(s)
来源：http://ne.panjiajie.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ml.nszjky.cn

JS:   JSON.parse(s)
来源：http://nv.shxzskj.cn

TS:   JSON.parse(s)
来源：http://ut.nicolike.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://xi.asd995.cn

Go:   json.Unmarshal(data, &v)
来源：http://wg.bookmarksfly.cn

Ruby: JSON.parse(s)
来源：http://xu.colortex.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://tr.huixinmuqiang.cn

[K03] JSON 美化输出（带缩进）
来源：http://my.szxytkj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://co.huixiangedu.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://di.shxzskj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://bo.asd995.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://bm.nszjky.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://vw.szxytkj.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ow.szxytkj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ll.newstarts.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://xt.chemitech.net.cn

[K04] 读取 JSON 文件
来源：http://be.shxzukj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://rz.yuexingan06.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://lc.wgjwhj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://by.nicolike.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://it.yuntaijiaju.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://rt.jctech888.com.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://sp.9csxet.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://vi.nicolike.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://eo.hahajie.cn

[K05] 深拷贝对象
来源：http://fx.wgjwhj.cn

Py:   copy.deepcopy(obj)
来源：http://me.shxzukj.cn

PHP:  unserialize(serialize($obj));
来源：http://eb.panjiajie.cn

JS:   structuredClone(obj)
来源：http://ic.shxzukj.cn

TS:   structuredClone(obj)
来源：http://cq.bookmarksfly.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://eh.muxihuayi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ds.muxihuayi.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://et.lnxyls.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://mx.huixiangedu.cn

[K06] 解析 URL 查询串
来源：http://iz.jctech888.com.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://pl.chemitech.net.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://bt.jianghongdianzi.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ph.haigaiapp.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xn.muxihuayi.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ji.haigaiapp.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://gr.nicolike.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://bd.chemitech.net.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ct.nszjky.cn

[K07] 进制转换
来源：http://cy.521024.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://tj.muxihuayi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://nk.hahajie.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://dg.muxihuayi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wn.jctech888.com.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://bm.szsharing.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://av.yuexingan06.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ia.huixiangedu.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://jp.wgjwhj.cn

[K08] 二进制序列化（非 JSON）
来源：http://qc.jctech888.com.cn

Py:   pickle.dumps(obj)
来源：http://cm.huixinmuqiang.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ix.szsharing.cn

JS:   v8.serialize(obj)        // Node
来源：http://nv.521024.cn

TS:   v8.serialize(obj)        // Node
来源：http://ws.hnjuh.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://bn.huixiangedu.cn

Go:   encoding/gob
来源：http://mq.colortex.cn

Ruby: Marshal.dump(obj)
来源：http://zt.nicolike.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ht.huanxung.cn

================================================================================
来源：http://dx.nszjky.cn

L. 网络请求
来源：http://qh.gzmigu.cn

================================================================================
来源：http://ya.jianghongdianzi.cn

[L01] 发送 GET 请求
来源：http://pl.9csxet.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xk.newstarts.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://yf.huixinmuqiang.cn

JS:   await fetch(url)
来源：http://fd.shxzukj.cn

TS:   await fetch(url)
来源：http://zd.szxytkj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://yq.521024.cn

Go:   resp, err := http.Get(url)
来源：http://rb.chemitech.net.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://bq.yuexingan06.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://kc.hahajie.cn

[L02] 发送 POST JSON
来源：http://kl.lnxyls.cn

Py:   requests.post(url, json={"a": 1})
来源：http://zd.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ug.panjiajie.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://st.yuntaijiaju.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yq.wgjwhj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://zs.panjiajie.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ck.wgjwhj.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://tz.hnjuh.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://kt.shxzskj.cn

[L03] 设置自定义请求头
来源：http://no.colortex.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://gc.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mh.shxzskj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://em.jctech888.com.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://si.hahajie.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://zv.jianghongdianzi.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://vz.jctech888.com.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ie.shxzukj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mc.jctech888.com.cn

[L04] 设置超时
来源：http://vi.lnxyls.cn

Py:   requests.get(url, timeout=5)
来源：http://ym.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://uh.521024.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uf.haigaiapp.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gx.hnjuh.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://cb.szsharing.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://va.shtwfgs.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://pt.panjiajie.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://uc.muxihuayi.cn

[L05] 上传文件（multipart）
来源：http://cn.bookmarksfly.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ox.szsharing.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://he.yuntaijiaju.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qx.szxytkj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ep.panjiajie.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://nb.lnxyls.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://gt.nicolike.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://fq.shtwfgs.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://sn.szxytkj.cn

[L06] 解析响应为 JSON
来源：http://qt.gzmigu.cn

Py:   resp.json()
来源：http://bd.panjiajie.cn

PHP:  json_decode($body, true);
来源：http://vw.jianghongdianzi.cn

JS:   await resp.json()
来源：http://lh.colortex.cn

TS:   await resp.json()
来源：http://rg.lnxyls.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://yn.lnxyls.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://yo.newstarts.cn

Ruby: JSON.parse(resp.body)
来源：http://zs.newstarts.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://vy.haigaiapp.cn

[L07] 处理 HTTP 状态码
来源：http://zm.panjiajie.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://cx.bookmarksfly.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://eu.huixiangedu.cn

JS:   resp.ok;  resp.status
来源：http://ql.shxzskj.cn

TS:   resp.ok;  resp.status
来源：http://ib.yuntaijiaju.cn

Java: resp.statusCode()
来源：http://ft.hahajie.cn

Go:   resp.StatusCode
来源：http://jk.shxzskj.cn

Ruby: resp.code.to_i
来源：http://zd.bookmarksfly.cn

C#:   (int)resp.StatusCode
来源：http://ke.9csxet.cn

[L08] 并发请求多个地址
来源：http://mf.panjiajie.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://yt.szxytkj.cn

PHP:  curl_multi_init() 系列
来源：http://wq.szxytkj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lc.haigaiapp.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lk.hnjuh.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ld.panjiajie.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://yy.newstarts.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://op.nicolike.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://eh.shtwfgs.cn

================================================================================
来源：http://sj.gzmigu.cn

M. 命令行 / 进程 / 环境
来源：http://sz.chemitech.net.cn

================================================================================
来源：http://pb.huixiangedu.cn

[M01] 读取命令行参数
来源：http://gr.yuexingan06.cn

Py:   sys.argv[1:]
来源：http://iq.gzmigu.cn

PHP:  $argv;  $argc;
来源：http://ui.panjiajie.cn

JS:   process.argv.slice(2)
来源：http://zq.nszjky.cn

TS:   process.argv.slice(2)
来源：http://ux.shtwfgs.cn

Java: args 数组（main 方法参数）
来源：http://lr.colortex.cn

Go:   os.Args[1:]
来源：http://hn.chemitech.net.cn

Ruby: ARGV
来源：http://ba.wgjwhj.cn

C#:   args 数组（Main 方法参数）
来源：http://hs.yuntaijiaju.cn

[M02] 读取环境变量
来源：http://ap.huixinmuqiang.cn

Py:   os.environ.get("HOME")
来源：http://hd.bjjhwx.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://dk.hahajie.cn

JS:   process.env.HOME
来源：http://vt.szxytkj.cn

TS:   process.env.HOME
来源：http://ri.hnjuh.cn

Java: System.getenv("HOME")
来源：http://fv.shxzukj.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://gy.521024.cn

Ruby: ENV["HOME"]
来源：http://am.jianghongdianzi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://kl.newstarts.cn

[M03] 执行外部命令
来源：http://kc.jctech888.com.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://br.gzmigu.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://vy.bookmarksfly.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://nc.panjiajie.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://yz.521024.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hi.shxzukj.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ss.gzmigu.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ft.521024.cn

C#:   Process.Start("ls", "-l");
来源：http://sp.panjiajie.cn

[M04] 获取当前工作目录
来源：http://tw.huixinmuqiang.cn

Py:   os.getcwd()
来源：http://it.asd995.cn

PHP:  getcwd();
来源：http://of.szsharing.cn

JS:   process.cwd()
来源：http://qe.bjjhwx.cn

TS:   process.cwd()
来源：http://rg.bookmarksfly.cn

Java: Path.of("").toAbsolutePath()
来源：http://pw.colortex.cn

Go:   os.Getwd()
来源：http://nq.haigaiapp.cn

Ruby: Dir.pwd
来源：http://uf.jctech888.com.cn

C#:   Directory.GetCurrentDirectory()
来源：http://sj.lnxyls.cn

[M05] 设置退出码
来源：http://el.szsharing.cn

Py:   sys.exit(1)
来源：http://mr.wgjwhj.cn

PHP:  exit(1);
来源：http://jf.lnxyls.cn

JS:   process.exit(1)
来源：http://rn.hnjuh.cn

TS:   process.exit(1)
来源：http://fp.shxzukj.cn

Java: System.exit(1)
来源：http://qy.huixiangedu.cn

Go:   os.Exit(1)
来源：http://jq.bookmarksfly.cn

Ruby: exit 1
来源：http://cy.jctech888.com.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://io.newstarts.cn

[M06] 向标准错误输出
来源：http://yv.gzmigu.cn

Py:   print("err", file=sys.stderr)
来源：http://rh.nicolike.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ap.haigaiapp.cn

JS:   console.error("err")
来源：http://hp.huanxung.cn

TS:   console.error("err")
来源：http://bz.szsharing.cn

Java: System.err.println("err")
来源：http://vl.jianghongdianzi.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://xy.shxzskj.cn

Ruby: warn "err"
来源：http://mt.hnjuh.cn

C#:   Console.Error.WriteLine("err")
来源：http://wi.huixinmuqiang.cn

[M07] 判断是否为主入口
来源：http://op.jctech888.com.cn

Py:   if __name__ == "__main__":
来源：http://ua.szsharing.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://gn.huanxung.cn

JS:   require.main === module
来源：http://ia.yuexingan06.cn

TS:   require.main === module
来源：http://hk.lnxyls.cn

Java: public static void main(String[] args)
来源：http://bu.haigaiapp.cn

Go:   func main()
来源：http://jk.lnxyls.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://yd.asd995.cn

C#:   static void Main(string[] args)
来源：http://og.bookmarksfly.cn

[M08] 获取系统与运行时信息
来源：http://wf.hahajie.cn

Py:   platform.system();  platform.python_version()
来源：http://jz.bookmarksfly.cn

PHP:  PHP_OS;  phpversion();
来源：http://gv.szxytkj.cn

JS:   process.platform;  process.version
来源：http://na.521024.cn

TS:   process.platform;  process.version
来源：http://vt.yuexingan06.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://nd.huixinmuqiang.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://yt.wgjwhj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://bu.panjiajie.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://wo.521024.cn

================================================================================
来源：http://en.jctech888.com.cn

N. 数据结构与算法
来源：http://xe.shxzskj.cn

================================================================================
来源：http://ey.shtwfgs.cn

[N01] 二分查找（有序数组）
来源：http://sp.shxzskj.cn

Py:   bisect.bisect_left(arr, x)
来源：http://wa.szxytkj.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://rm.huixiangedu.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://so.jctech888.com.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://av.wgjwhj.cn

Java: Arrays.binarySearch(arr, x)
来源：http://vs.lnxyls.cn

Go:   sort.SearchInts(arr, x)
来源：http://gs.wgjwhj.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://df.wgjwhj.cn

C#:   Array.BinarySearch(arr, x)
来源：http://mp.nicolike.cn

[N02] 排序（工程实践用内置实现）
来源：http://ms.panjiajie.cn

Py:   sorted(arr);  arr.sort()
来源：http://sh.lnxyls.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://tv.jianghongdianzi.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://cq.bjjhwx.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://nq.panjiajie.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ae.yuexingan06.cn

Go:   slices.Sort(arr)
来源：http://xu.nszjky.cn

Ruby: arr.sort
来源：http://tz.szsharing.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://jk.shxzukj.cn

[N03] 快速排序（分治示例）
来源：http://df.asd995.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wq.jctech888.com.cn

PHP:  // 递归实现，或用 usort
来源：http://cm.hahajie.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bs.haigaiapp.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ma.huixiangedu.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://pk.haigaiapp.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://tt.yuntaijiaju.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hv.9csxet.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ql.hnjuh.cn

[N04] 斐波那契数列
来源：http://co.nicolike.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://gq.jianghongdianzi.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://tv.chemitech.net.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gf.bjjhwx.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yv.shxzskj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mo.panjiajie.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://sq.chemitech.net.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://cn.gzmigu.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wd.newstarts.cn

[N05] 最大公约数
来源：http://sr.nicolike.cn

Py:   math.gcd(a, b)
来源：http://qk.nicolike.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://fg.haigaiapp.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wy.shtwfgs.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ux.bookmarksfly.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://yf.bookmarksfly.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ad.gzmigu.cn

Ruby: a.gcd(b)
来源：http://ou.lnxyls.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ez.huixinmuqiang.cn

[N06] 判断回文字符串
来源：http://po.szxytkj.cn

Py:   s == s[::-1]
来源：http://sa.9csxet.cn

PHP:  $s === strrev($s);
来源：http://nj.haigaiapp.cn

JS:   s === [...s].reverse().join("")
来源：http://rd.9csxet.cn

TS:   s === [...s].reverse().join("")
来源：http://ka.521024.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ko.yuntaijiaju.cn

Go:   // 双指针从两端比较
来源：http://cn.muxihuayi.cn

Ruby: s == s.reverse
来源：http://xg.shxzukj.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ix.9csxet.cn

[N07] 两数之和（返回下标）
来源：http://zj.szsharing.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://xx.bjjhwx.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://xs.nszjky.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://he.jctech888.com.cn

TS:   // 手写 Map<string, number>
来源：http://ai.bookmarksfly.cn

Java: // 手写 HashMap
来源：http://or.yuexingan06.cn

Go:   // 手写 map[int]int
来源：http://zn.panjiajie.cn

Ruby: // 手写 Hash
来源：http://nr.newstarts.cn

C#:   // 手写 Dictionary<int, int>
来源：http://nh.jctech888.com.cn

[N08] 生成全排列
来源：http://oy.huixinmuqiang.cn

Py:   itertools.permutations(arr)
来源：http://zs.bookmarksfly.cn

PHP:  // 手写递归交换
来源：http://uu.shtwfgs.cn

JS:   // 手写回溯递归
来源：http://ct.colortex.cn

TS:   // 手写回溯递归
来源：http://by.yuexingan06.cn

Java: // 手写回溯递归
来源：http://qb.bookmarksfly.cn

Go:   // 手写回溯递归
来源：http://oi.hnjuh.cn

Ruby: arr.permutation.to_a
来源：http://uu.huanxung.cn

C#:   // 手写回溯递归
来源：http://uj.shxzskj.cn


<!-- 参考信息 -->