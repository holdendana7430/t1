代发 wailian999

================================================================================
来源：http://gf.hahajie.cn

K. JSON 与序列化
来源：http://nk.muxihuayi.cn

================================================================================
来源：http://zz.jctech888.com.cn

[K01] 对象转 JSON 字符串
来源：http://tr.bookmarksfly.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://oi.haigaiapp.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mr.huixiangedu.cn

JS:   JSON.stringify(obj)
来源：http://ny.colortex.cn

TS:   JSON.stringify(obj)
来源：http://iq.newstarts.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ni.gzmigu.cn

Go:   json.Marshal(obj)
来源：http://al.huanxung.cn

Ruby: obj.to_json                                     // require "json"
来源：http://pe.chemitech.net.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://hl.muxihuayi.cn

[K02] JSON 字符串转对象
来源：http://ka.521024.cn

Py:   json.loads(s)
来源：http://zz.huanxung.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ej.521024.cn

JS:   JSON.parse(s)
来源：http://ix.newstarts.cn

TS:   JSON.parse(s)
来源：http://bk.newstarts.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://pr.521024.cn

Go:   json.Unmarshal(data, &v)
来源：http://md.shxzukj.cn

Ruby: JSON.parse(s)
来源：http://fk.wgjwhj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zj.shxzskj.cn

[K03] JSON 美化输出（带缩进）
来源：http://yq.hahajie.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://kf.muxihuayi.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://cx.jctech888.com.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://oa.shxzukj.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ls.hahajie.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://dy.hahajie.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ug.shxzskj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://tm.chemitech.net.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wb.bjjhwx.cn

[K04] 读取 JSON 文件
来源：http://dz.panjiajie.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://yr.hahajie.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://an.521024.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ge.nicolike.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nb.huixinmuqiang.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://af.colortex.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mm.asd995.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://gl.9csxet.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ju.chemitech.net.cn

[K05] 深拷贝对象
来源：http://vp.hnjuh.cn

Py:   copy.deepcopy(obj)
来源：http://wq.9csxet.cn

PHP:  unserialize(serialize($obj));
来源：http://as.newstarts.cn

JS:   structuredClone(obj)
来源：http://kz.yuntaijiaju.cn

TS:   structuredClone(obj)
来源：http://kg.colortex.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://oz.muxihuayi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://bc.muxihuayi.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zp.shxzskj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://rp.jctech888.com.cn

[K06] 解析 URL 查询串
来源：http://ey.colortex.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://sl.szsharing.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://co.jianghongdianzi.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xr.yuexingan06.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://iw.yuntaijiaju.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://bl.yuntaijiaju.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://bm.yuntaijiaju.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ly.szxytkj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://bq.muxihuayi.cn

[K07] 进制转换
来源：http://tn.nszjky.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://tf.colortex.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://dg.asd995.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://sl.jctech888.com.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://kx.hnjuh.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://uq.9csxet.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://tb.521024.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://so.huixiangedu.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://uw.szxytkj.cn

[K08] 二进制序列化（非 JSON）
来源：http://os.colortex.cn

Py:   pickle.dumps(obj)
来源：http://uk.521024.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ps.hnjuh.cn

JS:   v8.serialize(obj)        // Node
来源：http://gd.nszjky.cn

TS:   v8.serialize(obj)        // Node
来源：http://xu.bjjhwx.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://zz.jianghongdianzi.cn

Go:   encoding/gob
来源：http://dt.shtwfgs.cn

Ruby: Marshal.dump(obj)
来源：http://it.huixiangedu.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ch.jctech888.com.cn

================================================================================
来源：http://he.huanxung.cn

L. 网络请求
来源：http://px.newstarts.cn

================================================================================
来源：http://zi.shxzukj.cn

[L01] 发送 GET 请求
来源：http://iq.521024.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://sh.huixinmuqiang.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ns.bjjhwx.cn

JS:   await fetch(url)
来源：http://ov.lnxyls.cn

TS:   await fetch(url)
来源：http://yf.asd995.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://rd.szsharing.cn

Go:   resp, err := http.Get(url)
来源：http://bc.huanxung.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://zk.newstarts.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://sl.asd995.cn

[L02] 发送 POST JSON
来源：http://mm.shtwfgs.cn

Py:   requests.post(url, json={"a": 1})
来源：http://dp.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qo.asd995.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://eg.huixiangedu.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://aj.bjjhwx.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://lr.lnxyls.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hl.newstarts.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://sq.wgjwhj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ib.gzmigu.cn

[L03] 设置自定义请求头
来源：http://yv.521024.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://es.szxytkj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://yh.lnxyls.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dc.wgjwhj.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yo.shtwfgs.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://cd.panjiajie.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://sf.newstarts.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://yq.gzmigu.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://qu.szsharing.cn

[L04] 设置超时
来源：http://gg.muxihuayi.cn

Py:   requests.get(url, timeout=5)
来源：http://jl.szxytkj.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wt.jctech888.com.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lr.newstarts.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rk.asd995.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://tm.muxihuayi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://pj.newstarts.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://xm.shxzskj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ud.521024.cn

[L05] 上传文件（multipart）
来源：http://xn.muxihuayi.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://uj.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ix.jctech888.com.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://rn.asd995.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://yq.shxzskj.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hg.lnxyls.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ie.panjiajie.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ku.jianghongdianzi.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://gc.panjiajie.cn

[L06] 解析响应为 JSON
来源：http://tg.haigaiapp.cn

Py:   resp.json()
来源：http://hu.szxytkj.cn

PHP:  json_decode($body, true);
来源：http://ln.newstarts.cn

JS:   await resp.json()
来源：http://db.shxzskj.cn

TS:   await resp.json()
来源：http://ie.gzmigu.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ia.chemitech.net.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://jx.shxzukj.cn

Ruby: JSON.parse(resp.body)
来源：http://qw.hnjuh.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://tt.bjjhwx.cn

[L07] 处理 HTTP 状态码
来源：http://wj.gzmigu.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://lw.chemitech.net.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://co.bjjhwx.cn

JS:   resp.ok;  resp.status
来源：http://xa.nicolike.cn

TS:   resp.ok;  resp.status
来源：http://rc.szxytkj.cn

Java: resp.statusCode()
来源：http://hq.shtwfgs.cn

Go:   resp.StatusCode
来源：http://mv.bookmarksfly.cn

Ruby: resp.code.to_i
来源：http://ss.szxytkj.cn

C#:   (int)resp.StatusCode
来源：http://tx.colortex.cn

[L08] 并发请求多个地址
来源：http://zz.huixinmuqiang.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://vf.bookmarksfly.cn

PHP:  curl_multi_init() 系列
来源：http://ot.bookmarksfly.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ig.jianghongdianzi.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fv.chemitech.net.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://sp.huanxung.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://nn.haigaiapp.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vd.huixinmuqiang.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ej.nicolike.cn

================================================================================
来源：http://gr.huixinmuqiang.cn

M. 命令行 / 进程 / 环境
来源：http://ug.shtwfgs.cn

================================================================================
来源：http://sb.nicolike.cn

[M01] 读取命令行参数
来源：http://hj.huixinmuqiang.cn

Py:   sys.argv[1:]
来源：http://ml.jctech888.com.cn

PHP:  $argv;  $argc;
来源：http://nk.shxzskj.cn

JS:   process.argv.slice(2)
来源：http://ge.szsharing.cn

TS:   process.argv.slice(2)
来源：http://nn.muxihuayi.cn

Java: args 数组（main 方法参数）
来源：http://xg.huixiangedu.cn

Go:   os.Args[1:]
来源：http://pt.newstarts.cn

Ruby: ARGV
来源：http://wy.yuntaijiaju.cn

C#:   args 数组（Main 方法参数）
来源：http://kt.hnjuh.cn

[M02] 读取环境变量
来源：http://xn.muxihuayi.cn

Py:   os.environ.get("HOME")
来源：http://ql.szxytkj.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://lr.shtwfgs.cn

JS:   process.env.HOME
来源：http://aa.yuexingan06.cn

TS:   process.env.HOME
来源：http://em.huanxung.cn

Java: System.getenv("HOME")
来源：http://kz.nicolike.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://yz.muxihuayi.cn

Ruby: ENV["HOME"]
来源：http://ws.shxzskj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://fr.panjiajie.cn

[M03] 执行外部命令
来源：http://vn.gzmigu.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://sr.nicolike.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ny.shtwfgs.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ec.yuexingan06.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://be.521024.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://iv.hahajie.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://xj.newstarts.cn

Ruby: system("ls -l");  `ls -l`
来源：http://vi.bjjhwx.cn

C#:   Process.Start("ls", "-l");
来源：http://fg.panjiajie.cn

[M04] 获取当前工作目录
来源：http://fs.lnxyls.cn

Py:   os.getcwd()
来源：http://os.9csxet.cn

PHP:  getcwd();
来源：http://ur.wgjwhj.cn

JS:   process.cwd()
来源：http://dv.szsharing.cn

TS:   process.cwd()
来源：http://qy.gzmigu.cn

Java: Path.of("").toAbsolutePath()
来源：http://lc.nicolike.cn

Go:   os.Getwd()
来源：http://el.shxzukj.cn

Ruby: Dir.pwd
来源：http://xo.wgjwhj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://tb.hahajie.cn

[M05] 设置退出码
来源：http://ds.wgjwhj.cn

Py:   sys.exit(1)
来源：http://oh.wgjwhj.cn

PHP:  exit(1);
来源：http://gv.szxytkj.cn

JS:   process.exit(1)
来源：http://yi.wgjwhj.cn

TS:   process.exit(1)
来源：http://zs.huanxung.cn

Java: System.exit(1)
来源：http://ot.szxytkj.cn

Go:   os.Exit(1)
来源：http://en.nszjky.cn

Ruby: exit 1
来源：http://nb.muxihuayi.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://av.wgjwhj.cn

[M06] 向标准错误输出
来源：http://se.asd995.cn

Py:   print("err", file=sys.stderr)
来源：http://ce.shtwfgs.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://no.yuexingan06.cn

JS:   console.error("err")
来源：http://so.panjiajie.cn

TS:   console.error("err")
来源：http://ts.colortex.cn

Java: System.err.println("err")
来源：http://ju.jianghongdianzi.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://sc.hahajie.cn

Ruby: warn "err"
来源：http://yu.newstarts.cn

C#:   Console.Error.WriteLine("err")
来源：http://eg.colortex.cn

[M07] 判断是否为主入口
来源：http://bi.521024.cn

Py:   if __name__ == "__main__":
来源：http://ij.shtwfgs.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://tk.yuexingan06.cn

JS:   require.main === module
来源：http://gc.9csxet.cn

TS:   require.main === module
来源：http://nd.hahajie.cn

Java: public static void main(String[] args)
来源：http://sw.shxzukj.cn

Go:   func main()
来源：http://nq.yuntaijiaju.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://he.hnjuh.cn

C#:   static void Main(string[] args)
来源：http://ca.gzmigu.cn

[M08] 获取系统与运行时信息
来源：http://xs.yuntaijiaju.cn

Py:   platform.system();  platform.python_version()
来源：http://gv.nicolike.cn

PHP:  PHP_OS;  phpversion();
来源：http://mx.nicolike.cn

JS:   process.platform;  process.version
来源：http://va.huixinmuqiang.cn

TS:   process.platform;  process.version
来源：http://wy.panjiajie.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://rn.jianghongdianzi.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://vz.yuntaijiaju.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://qc.521024.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://qv.colortex.cn

================================================================================
来源：http://nk.shtwfgs.cn

N. 数据结构与算法
来源：http://um.9csxet.cn

================================================================================
来源：http://or.chemitech.net.cn

[N01] 二分查找（有序数组）
来源：http://gj.wgjwhj.cn

Py:   bisect.bisect_left(arr, x)
来源：http://wl.nszjky.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://df.shtwfgs.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jp.bookmarksfly.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://as.szxytkj.cn

Java: Arrays.binarySearch(arr, x)
来源：http://wm.panjiajie.cn

Go:   sort.SearchInts(arr, x)
来源：http://kx.jctech888.com.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://sb.shxzskj.cn

C#:   Array.BinarySearch(arr, x)
来源：http://el.colortex.cn

[N02] 排序（工程实践用内置实现）
来源：http://dl.colortex.cn

Py:   sorted(arr);  arr.sort()
来源：http://bq.szxytkj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://nx.521024.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://yl.shxzukj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://yf.9csxet.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://nj.nicolike.cn

Go:   slices.Sort(arr)
来源：http://so.hahajie.cn

Ruby: arr.sort
来源：http://ws.szsharing.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://az.huixiangedu.cn

[N03] 快速排序（分治示例）
来源：http://dy.bjjhwx.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ut.hnjuh.cn

PHP:  // 递归实现，或用 usort
来源：http://xg.muxihuayi.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ou.wgjwhj.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nt.nicolike.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://rg.nicolike.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ot.521024.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://bd.huixiangedu.cn

C#:   // 手写递归，或 Array.Sort
来源：http://rh.haigaiapp.cn

[N04] 斐波那契数列
来源：http://yr.9csxet.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ol.newstarts.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ix.panjiajie.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mn.huixinmuqiang.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gu.wgjwhj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://tl.chemitech.net.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://io.huixiangedu.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://qc.hahajie.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://qi.gzmigu.cn

[N05] 最大公约数
来源：http://ox.huixinmuqiang.cn

Py:   math.gcd(a, b)
来源：http://wu.bookmarksfly.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://xw.yuntaijiaju.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://po.shtwfgs.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mi.nszjky.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://eh.nszjky.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://kb.nszjky.cn

Ruby: a.gcd(b)
来源：http://ib.panjiajie.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://gz.yuexingan06.cn

[N06] 判断回文字符串
来源：http://cv.colortex.cn

Py:   s == s[::-1]
来源：http://lo.wgjwhj.cn

PHP:  $s === strrev($s);
来源：http://cs.wgjwhj.cn

JS:   s === [...s].reverse().join("")
来源：http://pt.yuntaijiaju.cn

TS:   s === [...s].reverse().join("")
来源：http://ub.huixiangedu.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ag.shxzukj.cn

Go:   // 双指针从两端比较
来源：http://zq.muxihuayi.cn

Ruby: s == s.reverse
来源：http://el.wgjwhj.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://og.nicolike.cn

[N07] 两数之和（返回下标）
来源：http://wx.shxzukj.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://xe.gzmigu.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ow.521024.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ci.yuntaijiaju.cn

TS:   // 手写 Map<string, number>
来源：http://wi.nszjky.cn

Java: // 手写 HashMap
来源：http://jt.shxzukj.cn

Go:   // 手写 map[int]int
来源：http://xs.jianghongdianzi.cn

Ruby: // 手写 Hash
来源：http://pv.bookmarksfly.cn

C#:   // 手写 Dictionary<int, int>
来源：http://os.chemitech.net.cn

[N08] 生成全排列
来源：http://tv.panjiajie.cn

Py:   itertools.permutations(arr)
来源：http://xx.521024.cn

PHP:  // 手写递归交换
来源：http://lw.hnjuh.cn

JS:   // 手写回溯递归
来源：http://us.shxzukj.cn

TS:   // 手写回溯递归
来源：http://it.521024.cn

Java: // 手写回溯递归
来源：http://jh.gzmigu.cn

Go:   // 手写回溯递归
来源：http://bm.yuexingan06.cn

Ruby: arr.permutation.to_a
来源：http://jj.shxzskj.cn

C#:   // 手写回溯递归
来源：http://uo.yuntaijiaju.cn


<!-- 参考信息 -->