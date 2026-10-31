代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://pc.shxzukj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://kw.shtwfgs.cn

JS:   JSON.stringify(obj)
来源：http://av.jctech888.com.cn

TS:   JSON.stringify(obj)
来源：http://gx.huixiangedu.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://kq.asd995.cn

Go:   json.Marshal(obj)
来源：http://co.huanxung.cn

Ruby: obj.to_json                                     // require "json"
来源：http://sc.9csxet.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ah.newstarts.cn

[K02] JSON 字符串转对象
来源：http://mi.huixiangedu.cn

Py:   json.loads(s)
来源：http://ki.jctech888.com.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://nd.nicolike.cn

JS:   JSON.parse(s)
来源：http://px.muxihuayi.cn

TS:   JSON.parse(s)
来源：http://mf.szxytkj.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ss.yuntaijiaju.cn

Go:   json.Unmarshal(data, &v)
来源：http://jp.shxzukj.cn

Ruby: JSON.parse(s)
来源：http://gw.jianghongdianzi.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://eq.chemitech.net.cn

[K03] JSON 美化输出（带缩进）
来源：http://ov.colortex.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://js.szsharing.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://il.asd995.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://cz.yuexingan06.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://mp.szsharing.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ew.yuexingan06.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ew.szsharing.cn

Ruby: JSON.pretty_generate(obj)
来源：http://gb.bjjhwx.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://qd.haigaiapp.cn

[K04] 读取 JSON 文件
来源：http://uo.szsharing.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ec.yuntaijiaju.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://kx.huixiangedu.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fx.nszjky.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lw.huixinmuqiang.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mm.huixiangedu.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://lt.jianghongdianzi.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://jt.szsharing.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://tu.yuexingan06.cn

[K05] 深拷贝对象
来源：http://kw.lnxyls.cn

Py:   copy.deepcopy(obj)
来源：http://nw.bookmarksfly.cn

PHP:  unserialize(serialize($obj));
来源：http://rr.bjjhwx.cn

JS:   structuredClone(obj)
来源：http://mq.szxytkj.cn

TS:   structuredClone(obj)
来源：http://ih.huanxung.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://rw.huixinmuqiang.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ms.haigaiapp.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ei.chemitech.net.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://xt.huanxung.cn

[K06] 解析 URL 查询串
来源：http://iv.shxzukj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://li.chemitech.net.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ax.huanxung.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://eo.nszjky.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gq.panjiajie.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ei.yuntaijiaju.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://as.szsharing.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://dj.lnxyls.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://el.yuexingan06.cn

[K07] 进制转换
来源：http://em.wgjwhj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://by.chemitech.net.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ln.huixinmuqiang.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://lg.shtwfgs.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://fh.hnjuh.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://yi.huanxung.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://vx.nicolike.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ro.9csxet.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://na.nszjky.cn

[K08] 二进制序列化（非 JSON）
来源：http://hp.jianghongdianzi.cn

Py:   pickle.dumps(obj)
来源：http://kg.newstarts.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://kl.shtwfgs.cn

JS:   v8.serialize(obj)        // Node
来源：http://yb.jctech888.com.cn

TS:   v8.serialize(obj)        // Node
来源：http://ay.huixinmuqiang.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://kn.huanxung.cn

Go:   encoding/gob
来源：http://ia.9csxet.cn

Ruby: Marshal.dump(obj)
来源：http://sx.hahajie.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://sa.nicolike.cn

================================================================================
来源：http://yg.bjjhwx.cn

L. 网络请求
来源：http://hf.shtwfgs.cn

================================================================================
来源：http://hs.nicolike.cn

[L01] 发送 GET 请求
来源：http://qe.jianghongdianzi.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ci.nszjky.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vo.chemitech.net.cn

JS:   await fetch(url)
来源：http://dg.nszjky.cn

TS:   await fetch(url)
来源：http://fa.chemitech.net.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://uf.shtwfgs.cn

Go:   resp, err := http.Get(url)
来源：http://ti.jctech888.com.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://tq.muxihuayi.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ng.muxihuayi.cn

[L02] 发送 POST JSON
来源：http://gy.hnjuh.cn

Py:   requests.post(url, json={"a": 1})
来源：http://va.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://tb.panjiajie.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://le.shtwfgs.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xa.newstarts.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://xb.jctech888.com.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ah.shtwfgs.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mc.hahajie.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://rp.9csxet.cn

[L03] 设置自定义请求头
来源：http://jw.gzmigu.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://jx.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://bo.yuntaijiaju.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tk.asd995.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ft.shtwfgs.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://lj.jctech888.com.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://vr.asd995.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://tr.yuexingan06.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ht.jianghongdianzi.cn

[L04] 设置超时
来源：http://cw.huixinmuqiang.cn

Py:   requests.get(url, timeout=5)
来源：http://aq.haigaiapp.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xr.hahajie.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://na.wgjwhj.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yl.huixinmuqiang.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://lw.asd995.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://bg.newstarts.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://oz.colortex.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://jo.9csxet.cn

[L05] 上传文件（multipart）
来源：http://rj.jctech888.com.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ly.hnjuh.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://yq.panjiajie.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://vn.yuntaijiaju.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://nr.bjjhwx.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ll.wgjwhj.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ou.panjiajie.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ix.yuntaijiaju.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://sw.lnxyls.cn

[L06] 解析响应为 JSON
来源：http://ff.shtwfgs.cn

Py:   resp.json()
来源：http://wy.newstarts.cn

PHP:  json_decode($body, true);
来源：http://do.jctech888.com.cn

JS:   await resp.json()
来源：http://pl.szxytkj.cn

TS:   await resp.json()
来源：http://vp.wgjwhj.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://so.jctech888.com.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://vo.nicolike.cn

Ruby: JSON.parse(resp.body)
来源：http://xk.wgjwhj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://pe.hahajie.cn

[L07] 处理 HTTP 状态码
来源：http://ex.shxzukj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://zw.muxihuayi.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://bl.wgjwhj.cn

JS:   resp.ok;  resp.status
来源：http://qj.huixinmuqiang.cn

TS:   resp.ok;  resp.status
来源：http://iy.bookmarksfly.cn

Java: resp.statusCode()
来源：http://fk.bjjhwx.cn

Go:   resp.StatusCode
来源：http://ho.hahajie.cn

Ruby: resp.code.to_i
来源：http://mc.jctech888.com.cn

C#:   (int)resp.StatusCode
来源：http://ss.yuntaijiaju.cn

[L08] 并发请求多个地址
来源：http://tt.hnjuh.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hv.muxihuayi.cn

PHP:  curl_multi_init() 系列
来源：http://cr.shtwfgs.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://io.yuexingan06.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qx.wgjwhj.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://gu.9csxet.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://xk.newstarts.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://uz.shtwfgs.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hj.bookmarksfly.cn

================================================================================
来源：http://kc.szsharing.cn

M. 命令行 / 进程 / 环境
来源：http://vb.gzmigu.cn

================================================================================
来源：http://sx.yuexingan06.cn

[M01] 读取命令行参数
来源：http://kb.wgjwhj.cn

Py:   sys.argv[1:]
来源：http://wf.newstarts.cn

PHP:  $argv;  $argc;
来源：http://bj.lnxyls.cn

JS:   process.argv.slice(2)
来源：http://py.nicolike.cn

TS:   process.argv.slice(2)
来源：http://cj.szxytkj.cn

Java: args 数组（main 方法参数）
来源：http://ze.yuexingan06.cn

Go:   os.Args[1:]
来源：http://mv.yuexingan06.cn

Ruby: ARGV
来源：http://jk.hnjuh.cn

C#:   args 数组（Main 方法参数）
来源：http://gt.9csxet.cn

[M02] 读取环境变量
来源：http://mv.521024.cn

Py:   os.environ.get("HOME")
来源：http://ix.chemitech.net.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://tz.nszjky.cn

JS:   process.env.HOME
来源：http://gf.shxzukj.cn

TS:   process.env.HOME
来源：http://vq.chemitech.net.cn

Java: System.getenv("HOME")
来源：http://kj.shxzukj.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ny.hahajie.cn

Ruby: ENV["HOME"]
来源：http://hy.bookmarksfly.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://fv.wgjwhj.cn

[M03] 执行外部命令
来源：http://jz.huixiangedu.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wd.shxzskj.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hb.lnxyls.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://at.szxytkj.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://uy.9csxet.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://kc.shxzskj.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ga.muxihuayi.cn

Ruby: system("ls -l");  `ls -l`
来源：http://eb.bookmarksfly.cn

C#:   Process.Start("ls", "-l");
来源：http://qm.nicolike.cn

[M04] 获取当前工作目录
来源：http://vq.huanxung.cn

Py:   os.getcwd()
来源：http://jq.szxytkj.cn

PHP:  getcwd();
来源：http://fq.huanxung.cn

JS:   process.cwd()
来源：http://of.newstarts.cn

TS:   process.cwd()
来源：http://aw.chemitech.net.cn

Java: Path.of("").toAbsolutePath()
来源：http://er.muxihuayi.cn

Go:   os.Getwd()
来源：http://zz.asd995.cn

Ruby: Dir.pwd
来源：http://tf.nszjky.cn

C#:   Directory.GetCurrentDirectory()
来源：http://wb.nszjky.cn

[M05] 设置退出码
来源：http://ai.huixinmuqiang.cn

Py:   sys.exit(1)
来源：http://gb.huixiangedu.cn

PHP:  exit(1);
来源：http://ew.gzmigu.cn

JS:   process.exit(1)
来源：http://bf.panjiajie.cn

TS:   process.exit(1)
来源：http://kw.muxihuayi.cn

Java: System.exit(1)
来源：http://sq.haigaiapp.cn

Go:   os.Exit(1)
来源：http://sr.nszjky.cn

Ruby: exit 1
来源：http://wt.yuntaijiaju.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ss.shtwfgs.cn

[M06] 向标准错误输出
来源：http://hn.shxzskj.cn

Py:   print("err", file=sys.stderr)
来源：http://ft.huanxung.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://kv.lnxyls.cn

JS:   console.error("err")
来源：http://qy.muxihuayi.cn

TS:   console.error("err")
来源：http://kb.huixiangedu.cn

Java: System.err.println("err")
来源：http://xw.huixiangedu.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://jc.szxytkj.cn

Ruby: warn "err"
来源：http://ut.9csxet.cn

C#:   Console.Error.WriteLine("err")
来源：http://ix.huixinmuqiang.cn

[M07] 判断是否为主入口
来源：http://fm.nicolike.cn

Py:   if __name__ == "__main__":
来源：http://zh.wgjwhj.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://rp.colortex.cn

JS:   require.main === module
来源：http://gl.wgjwhj.cn

TS:   require.main === module
来源：http://qx.jianghongdianzi.cn

Java: public static void main(String[] args)
来源：http://nf.asd995.cn

Go:   func main()
来源：http://ho.asd995.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://yf.huixiangedu.cn

C#:   static void Main(string[] args)
来源：http://jl.haigaiapp.cn

[M08] 获取系统与运行时信息
来源：http://zk.haigaiapp.cn

Py:   platform.system();  platform.python_version()
来源：http://xu.huixinmuqiang.cn

PHP:  PHP_OS;  phpversion();
来源：http://zl.szsharing.cn

JS:   process.platform;  process.version
来源：http://tj.jianghongdianzi.cn

TS:   process.platform;  process.version
来源：http://gj.huixiangedu.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xk.521024.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://lr.nicolike.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://sq.shtwfgs.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ag.lnxyls.cn

================================================================================
来源：http://ny.chemitech.net.cn

N. 数据结构与算法
来源：http://kn.bookmarksfly.cn

================================================================================
来源：http://tt.huanxung.cn

[N01] 二分查找（有序数组）
来源：http://vo.szsharing.cn

Py:   bisect.bisect_left(arr, x)
来源：http://kg.haigaiapp.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://bk.521024.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ew.chemitech.net.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vq.muxihuayi.cn

Java: Arrays.binarySearch(arr, x)
来源：http://mc.huixinmuqiang.cn

Go:   sort.SearchInts(arr, x)
来源：http://bz.szsharing.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://te.haigaiapp.cn

C#:   Array.BinarySearch(arr, x)
来源：http://xy.shtwfgs.cn

[N02] 排序（工程实践用内置实现）
来源：http://vq.muxihuayi.cn

Py:   sorted(arr);  arr.sort()
来源：http://ui.hahajie.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://uq.huixiangedu.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://lf.9csxet.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://zm.shtwfgs.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://oq.haigaiapp.cn

Go:   slices.Sort(arr)
来源：http://im.shxzukj.cn

Ruby: arr.sort
来源：http://jz.huixiangedu.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ii.521024.cn

[N03] 快速排序（分治示例）
来源：http://nd.gzmigu.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ax.colortex.cn

PHP:  // 递归实现，或用 usort
来源：http://ne.bjjhwx.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wk.bjjhwx.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://do.huixinmuqiang.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hv.szsharing.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://av.muxihuayi.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://zf.hnjuh.cn

C#:   // 手写递归，或 Array.Sort
来源：http://jp.yuntaijiaju.cn

[N04] 斐波那契数列
来源：http://cw.newstarts.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://du.yuntaijiaju.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://bi.bookmarksfly.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ho.wgjwhj.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ij.nicolike.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://yu.jctech888.com.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://kf.haigaiapp.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hm.jctech888.com.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://kg.bookmarksfly.cn

[N05] 最大公约数
来源：http://yi.newstarts.cn

Py:   math.gcd(a, b)
来源：http://es.hahajie.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hu.jianghongdianzi.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xk.yuntaijiaju.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bz.gzmigu.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://yl.nicolike.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://an.lnxyls.cn

Ruby: a.gcd(b)
来源：http://qh.huixinmuqiang.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mo.huanxung.cn

[N06] 判断回文字符串
来源：http://mx.yuexingan06.cn

Py:   s == s[::-1]
来源：http://rm.yuexingan06.cn

PHP:  $s === strrev($s);
来源：http://fk.lnxyls.cn

JS:   s === [...s].reverse().join("")
来源：http://ew.hnjuh.cn

TS:   s === [...s].reverse().join("")
来源：http://un.huixiangedu.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://se.jctech888.com.cn

Go:   // 双指针从两端比较
来源：http://ar.shtwfgs.cn

Ruby: s == s.reverse
来源：http://rc.haigaiapp.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://yu.wgjwhj.cn

[N07] 两数之和（返回下标）
来源：http://os.muxihuayi.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://un.huanxung.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ql.shxzukj.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://lf.hahajie.cn

TS:   // 手写 Map<string, number>
来源：http://xx.9csxet.cn

Java: // 手写 HashMap
来源：http://df.szxytkj.cn

Go:   // 手写 map[int]int
来源：http://kh.wgjwhj.cn

Ruby: // 手写 Hash
来源：http://fp.haigaiapp.cn

C#:   // 手写 Dictionary<int, int>
来源：http://yu.nicolike.cn

[N08] 生成全排列
来源：http://rk.jctech888.com.cn

Py:   itertools.permutations(arr)
来源：http://fb.huixiangedu.cn

PHP:  // 手写递归交换
来源：http://sf.9csxet.cn

JS:   // 手写回溯递归
来源：http://pi.colortex.cn

TS:   // 手写回溯递归
来源：http://oo.szsharing.cn

Java: // 手写回溯递归
来源：http://hp.szxytkj.cn

Go:   // 手写回溯递归
来源：http://te.shtwfgs.cn

Ruby: arr.permutation.to_a
来源：http://hf.yuntaijiaju.cn

C#:   // 手写回溯递归
来源：http://om.yuexingan06.cn

[N09] 栈与队列
来源：http://ms.yuexingan06.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ep.hahajie.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://lj.shxzukj.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://fr.haigaiapp.cn


<!-- 参考信息 -->