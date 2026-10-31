代发 wailian999

================================================================================
来源：http://xj.haigaiapp.cn

K. JSON 与序列化
来源：http://hu.bjjhwx.cn

================================================================================
来源：http://ob.jctech888.com.cn

[K01] 对象转 JSON 字符串
来源：http://kk.shxzskj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://lq.szsharing.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://vy.newstarts.cn

JS:   JSON.stringify(obj)
来源：http://zw.chemitech.net.cn

TS:   JSON.stringify(obj)
来源：http://yn.bjjhwx.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ee.yuntaijiaju.cn

Go:   json.Marshal(obj)
来源：http://qy.hnjuh.cn

Ruby: obj.to_json                                     // require "json"
来源：http://yb.hnjuh.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://hp.newstarts.cn

[K02] JSON 字符串转对象
来源：http://xs.nszjky.cn

Py:   json.loads(s)
来源：http://cz.hnjuh.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ov.wgjwhj.cn

JS:   JSON.parse(s)
来源：http://aq.wgjwhj.cn

TS:   JSON.parse(s)
来源：http://mo.bjjhwx.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://sa.haigaiapp.cn

Go:   json.Unmarshal(data, &v)
来源：http://im.nicolike.cn

Ruby: JSON.parse(s)
来源：http://ku.bjjhwx.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://lt.9csxet.cn

[K03] JSON 美化输出（带缩进）
来源：http://qy.colortex.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://fr.nszjky.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://io.hahajie.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://dz.bookmarksfly.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://aj.nicolike.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://sj.huixiangedu.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ml.huanxung.cn

Ruby: JSON.pretty_generate(obj)
来源：http://bz.lnxyls.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ri.bookmarksfly.cn

[K04] 读取 JSON 文件
来源：http://nr.9csxet.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ej.newstarts.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://tr.shtwfgs.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://oz.lnxyls.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tj.nicolike.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://zt.shtwfgs.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://nm.muxihuayi.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://lw.gzmigu.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://pv.9csxet.cn

[K05] 深拷贝对象
来源：http://fr.huixinmuqiang.cn

Py:   copy.deepcopy(obj)
来源：http://zi.huixinmuqiang.cn

PHP:  unserialize(serialize($obj));
来源：http://et.bjjhwx.cn

JS:   structuredClone(obj)
来源：http://nl.chemitech.net.cn

TS:   structuredClone(obj)
来源：http://ld.hnjuh.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://xh.shxzskj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ou.wgjwhj.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ws.hnjuh.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://yf.521024.cn

[K06] 解析 URL 查询串
来源：http://ix.huixiangedu.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://dk.jianghongdianzi.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://rd.muxihuayi.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gk.hnjuh.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bt.bookmarksfly.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://va.nicolike.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://pb.muxihuayi.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ps.jctech888.com.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://yw.wgjwhj.cn

[K07] 进制转换
来源：http://jd.521024.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://fd.chemitech.net.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ci.jctech888.com.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://fq.yuntaijiaju.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ns.shxzskj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xy.szsharing.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hw.lnxyls.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://he.muxihuayi.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://pc.newstarts.cn

[K08] 二进制序列化（非 JSON）
来源：http://hs.shxzukj.cn

Py:   pickle.dumps(obj)
来源：http://af.nicolike.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://fy.muxihuayi.cn

JS:   v8.serialize(obj)        // Node
来源：http://su.nicolike.cn

TS:   v8.serialize(obj)        // Node
来源：http://mm.newstarts.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://fo.lnxyls.cn

Go:   encoding/gob
来源：http://nt.yuntaijiaju.cn

Ruby: Marshal.dump(obj)
来源：http://qk.hahajie.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://dz.newstarts.cn

================================================================================
来源：http://dt.jctech888.com.cn

L. 网络请求
来源：http://xq.shtwfgs.cn

================================================================================
来源：http://kh.9csxet.cn

[L01] 发送 GET 请求
来源：http://lp.shtwfgs.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://cx.jctech888.com.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ml.lnxyls.cn

JS:   await fetch(url)
来源：http://ir.jianghongdianzi.cn

TS:   await fetch(url)
来源：http://sk.hnjuh.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qg.chemitech.net.cn

Go:   resp, err := http.Get(url)
来源：http://zk.haigaiapp.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://gi.panjiajie.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wv.huixinmuqiang.cn

[L02] 发送 POST JSON
来源：http://ee.huixiangedu.cn

Py:   requests.post(url, json={"a": 1})
来源：http://av.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qf.chemitech.net.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gi.yuntaijiaju.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yj.hahajie.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://re.wgjwhj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hd.hnjuh.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ql.shtwfgs.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://kv.huanxung.cn

[L03] 设置自定义请求头
来源：http://ln.muxihuayi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://iw.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://qr.szxytkj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wn.yuexingan06.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wq.muxihuayi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://es.panjiajie.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://zk.jctech888.com.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://zp.shxzukj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://pn.hahajie.cn

[L04] 设置超时
来源：http://if.bookmarksfly.cn

Py:   requests.get(url, timeout=5)
来源：http://an.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://sx.huanxung.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bw.nicolike.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ko.haigaiapp.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://pq.jianghongdianzi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://pq.521024.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://fv.hahajie.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qh.szxytkj.cn

[L05] 上传文件（multipart）
来源：http://cr.hnjuh.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://kw.yuntaijiaju.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://cy.shxzskj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ld.huixiangedu.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ck.chemitech.net.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://gq.shxzskj.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ec.yuexingan06.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wa.szsharing.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://fx.haigaiapp.cn

[L06] 解析响应为 JSON
来源：http://go.haigaiapp.cn

Py:   resp.json()
来源：http://uj.shxzukj.cn

PHP:  json_decode($body, true);
来源：http://wi.panjiajie.cn

JS:   await resp.json()
来源：http://as.huixinmuqiang.cn

TS:   await resp.json()
来源：http://cm.muxihuayi.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://bq.shxzskj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://qg.shxzskj.cn

Ruby: JSON.parse(resp.body)
来源：http://tk.shxzskj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://sc.shxzukj.cn

[L07] 处理 HTTP 状态码
来源：http://bk.shxzskj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://uy.yuntaijiaju.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://kj.huixiangedu.cn

JS:   resp.ok;  resp.status
来源：http://jh.wgjwhj.cn

TS:   resp.ok;  resp.status
来源：http://oq.9csxet.cn

Java: resp.statusCode()
来源：http://dm.colortex.cn

Go:   resp.StatusCode
来源：http://hl.521024.cn

Ruby: resp.code.to_i
来源：http://qa.nszjky.cn

C#:   (int)resp.StatusCode
来源：http://xb.521024.cn

[L08] 并发请求多个地址
来源：http://pc.bjjhwx.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://xu.muxihuayi.cn

PHP:  curl_multi_init() 系列
来源：http://tj.jctech888.com.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ae.huixinmuqiang.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ft.hnjuh.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://io.haigaiapp.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://vj.huanxung.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://nb.hnjuh.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://nv.huixinmuqiang.cn

================================================================================
来源：http://ve.haigaiapp.cn

M. 命令行 / 进程 / 环境
来源：http://mw.gzmigu.cn

================================================================================
来源：http://dz.9csxet.cn

[M01] 读取命令行参数
来源：http://ub.lnxyls.cn

Py:   sys.argv[1:]
来源：http://gp.nszjky.cn

PHP:  $argv;  $argc;
来源：http://uv.jianghongdianzi.cn

JS:   process.argv.slice(2)
来源：http://fp.colortex.cn

TS:   process.argv.slice(2)
来源：http://co.colortex.cn

Java: args 数组（main 方法参数）
来源：http://rz.panjiajie.cn

Go:   os.Args[1:]
来源：http://ow.jianghongdianzi.cn

Ruby: ARGV
来源：http://qz.yuntaijiaju.cn

C#:   args 数组（Main 方法参数）
来源：http://jb.bookmarksfly.cn

[M02] 读取环境变量
来源：http://ob.shxzskj.cn

Py:   os.environ.get("HOME")
来源：http://fn.szsharing.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zl.huixiangedu.cn

JS:   process.env.HOME
来源：http://tw.newstarts.cn

TS:   process.env.HOME
来源：http://rv.szxytkj.cn

Java: System.getenv("HOME")
来源：http://pk.bjjhwx.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://fx.shxzukj.cn

Ruby: ENV["HOME"]
来源：http://eg.hahajie.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://qk.huixinmuqiang.cn

[M03] 执行外部命令
来源：http://vb.muxihuayi.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vz.huixiangedu.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://sw.hnjuh.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ui.haigaiapp.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://tz.hnjuh.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://gg.szxytkj.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://vz.yuexingan06.cn

Ruby: system("ls -l");  `ls -l`
来源：http://jn.shtwfgs.cn

C#:   Process.Start("ls", "-l");
来源：http://sy.panjiajie.cn

[M04] 获取当前工作目录
来源：http://gg.shtwfgs.cn

Py:   os.getcwd()
来源：http://pp.muxihuayi.cn

PHP:  getcwd();
来源：http://ha.shtwfgs.cn

JS:   process.cwd()
来源：http://pv.szsharing.cn

TS:   process.cwd()
来源：http://ls.nszjky.cn

Java: Path.of("").toAbsolutePath()
来源：http://fx.asd995.cn

Go:   os.Getwd()
来源：http://wa.9csxet.cn

Ruby: Dir.pwd
来源：http://vn.huixiangedu.cn

C#:   Directory.GetCurrentDirectory()
来源：http://bg.shtwfgs.cn

[M05] 设置退出码
来源：http://ot.huanxung.cn

Py:   sys.exit(1)
来源：http://nf.yuexingan06.cn

PHP:  exit(1);
来源：http://zb.gzmigu.cn

JS:   process.exit(1)
来源：http://pg.jianghongdianzi.cn

TS:   process.exit(1)
来源：http://ns.muxihuayi.cn

Java: System.exit(1)
来源：http://qe.9csxet.cn

Go:   os.Exit(1)
来源：http://ps.gzmigu.cn

Ruby: exit 1
来源：http://dj.jianghongdianzi.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://fp.bookmarksfly.cn

[M06] 向标准错误输出
来源：http://jo.huixiangedu.cn

Py:   print("err", file=sys.stderr)
来源：http://wa.521024.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://tu.yuexingan06.cn

JS:   console.error("err")
来源：http://hs.nszjky.cn

TS:   console.error("err")
来源：http://qo.muxihuayi.cn

Java: System.err.println("err")
来源：http://ia.shxzskj.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://kd.panjiajie.cn

Ruby: warn "err"
来源：http://qy.szxytkj.cn

C#:   Console.Error.WriteLine("err")
来源：http://sr.jctech888.com.cn

[M07] 判断是否为主入口
来源：http://ev.yuntaijiaju.cn

Py:   if __name__ == "__main__":
来源：http://vi.szsharing.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://xv.shxzukj.cn

JS:   require.main === module
来源：http://il.panjiajie.cn

TS:   require.main === module
来源：http://ox.szxytkj.cn

Java: public static void main(String[] args)
来源：http://ib.yuntaijiaju.cn

Go:   func main()
来源：http://km.muxihuayi.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://cy.hahajie.cn

C#:   static void Main(string[] args)
来源：http://ic.panjiajie.cn

[M08] 获取系统与运行时信息
来源：http://tu.shxzskj.cn

Py:   platform.system();  platform.python_version()
来源：http://rf.huixiangedu.cn

PHP:  PHP_OS;  phpversion();
来源：http://es.yuexingan06.cn

JS:   process.platform;  process.version
来源：http://ej.chemitech.net.cn

TS:   process.platform;  process.version
来源：http://ae.yuexingan06.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mp.hnjuh.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://wd.nszjky.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://gz.shtwfgs.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ha.9csxet.cn

================================================================================
来源：http://ge.hnjuh.cn

N. 数据结构与算法
来源：http://ll.yuntaijiaju.cn

================================================================================
来源：http://fy.jianghongdianzi.cn

[N01] 二分查找（有序数组）
来源：http://fl.shxzukj.cn

Py:   bisect.bisect_left(arr, x)
来源：http://de.nicolike.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://yh.muxihuayi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ut.shxzukj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xs.chemitech.net.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ta.szsharing.cn

Go:   sort.SearchInts(arr, x)
来源：http://gp.jctech888.com.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://xt.gzmigu.cn

C#:   Array.BinarySearch(arr, x)
来源：http://tt.hnjuh.cn

[N02] 排序（工程实践用内置实现）
来源：http://rh.hahajie.cn

Py:   sorted(arr);  arr.sort()
来源：http://qj.shxzskj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://sy.521024.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://kz.bjjhwx.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://zf.haigaiapp.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://sj.colortex.cn

Go:   slices.Sort(arr)
来源：http://bx.gzmigu.cn

Ruby: arr.sort
来源：http://lk.bookmarksfly.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://qq.haigaiapp.cn

[N03] 快速排序（分治示例）
来源：http://qs.haigaiapp.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ei.hnjuh.cn

PHP:  // 递归实现，或用 usort
来源：http://at.yuntaijiaju.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ex.huixiangedu.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fs.huanxung.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://fs.chemitech.net.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hd.newstarts.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://bl.gzmigu.cn

C#:   // 手写递归，或 Array.Sort
来源：http://nz.szxytkj.cn

[N04] 斐波那契数列
来源：http://qn.huanxung.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qe.huixinmuqiang.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ku.asd995.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gq.yuntaijiaju.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kg.yuntaijiaju.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://tk.yuntaijiaju.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://nm.lnxyls.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://tg.wgjwhj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://yb.jianghongdianzi.cn

[N05] 最大公约数
来源：http://dy.nszjky.cn

Py:   math.gcd(a, b)
来源：http://ip.shxzskj.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://bm.huixiangedu.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bv.shxzukj.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yf.hnjuh.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://oq.newstarts.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://yn.huixiangedu.cn

Ruby: a.gcd(b)
来源：http://an.jianghongdianzi.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://kw.huixiangedu.cn

[N06] 判断回文字符串
来源：http://ig.nszjky.cn

Py:   s == s[::-1]
来源：http://tu.wgjwhj.cn

PHP:  $s === strrev($s);
来源：http://sz.bjjhwx.cn

JS:   s === [...s].reverse().join("")
来源：http://em.szxytkj.cn

TS:   s === [...s].reverse().join("")
来源：http://ef.bjjhwx.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ut.gzmigu.cn

Go:   // 双指针从两端比较
来源：http://bg.nszjky.cn

Ruby: s == s.reverse
来源：http://ps.shxzskj.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://kc.wgjwhj.cn

[N07] 两数之和（返回下标）
来源：http://yf.9csxet.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://fw.newstarts.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://nm.colortex.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://xb.bookmarksfly.cn

TS:   // 手写 Map<string, number>
来源：http://ag.shxzskj.cn

Java: // 手写 HashMap
来源：http://da.newstarts.cn

Go:   // 手写 map[int]int
来源：http://pc.huanxung.cn

Ruby: // 手写 Hash
来源：http://av.9csxet.cn

C#:   // 手写 Dictionary<int, int>
来源：http://pj.newstarts.cn

[N08] 生成全排列
来源：http://uk.gzmigu.cn

Py:   itertools.permutations(arr)
来源：http://yh.colortex.cn

PHP:  // 手写递归交换
来源：http://xx.huixiangedu.cn

JS:   // 手写回溯递归
来源：http://bj.hahajie.cn

TS:   // 手写回溯递归
来源：http://zu.shxzskj.cn

Java: // 手写回溯递归
来源：http://dy.hnjuh.cn

Go:   // 手写回溯递归
来源：http://vy.huanxung.cn

Ruby: arr.permutation.to_a
来源：http://fy.muxihuayi.cn

C#:   // 手写回溯递归
来源：http://mx.newstarts.cn


<!-- 参考信息 -->