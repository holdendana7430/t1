代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ng.huanxung.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://fh.hnjuh.cn

JS:   JSON.stringify(obj)
来源：http://ad.hahajie.cn

TS:   JSON.stringify(obj)
来源：http://qg.nicolike.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://zl.panjiajie.cn

Go:   json.Marshal(obj)
来源：http://lp.9csxet.cn

Ruby: obj.to_json                                     // require "json"
来源：http://on.hnjuh.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://kq.jctech888.com.cn

[K02] JSON 字符串转对象
来源：http://tm.nicolike.cn

Py:   json.loads(s)
来源：http://jo.yuexingan06.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://qg.asd995.cn

JS:   JSON.parse(s)
来源：http://wn.colortex.cn

TS:   JSON.parse(s)
来源：http://vu.nszjky.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://sg.muxihuayi.cn

Go:   json.Unmarshal(data, &v)
来源：http://js.wgjwhj.cn

Ruby: JSON.parse(s)
来源：http://nc.newstarts.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ek.huixiangedu.cn

[K03] JSON 美化输出（带缩进）
来源：http://tw.bookmarksfly.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://yx.hnjuh.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://vd.huanxung.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://wx.bookmarksfly.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ot.colortex.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ly.hahajie.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xz.huixiangedu.cn

Ruby: JSON.pretty_generate(obj)
来源：http://hp.bjjhwx.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ce.shxzskj.cn

[K04] 读取 JSON 文件
来源：http://ly.chemitech.net.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wr.521024.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://zf.shxzskj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ns.hnjuh.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lu.yuexingan06.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://gh.muxihuayi.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ls.colortex.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://fi.shxzukj.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ey.shxzukj.cn

[K05] 深拷贝对象
来源：http://aw.shtwfgs.cn

Py:   copy.deepcopy(obj)
来源：http://po.colortex.cn

PHP:  unserialize(serialize($obj));
来源：http://pk.shxzukj.cn

JS:   structuredClone(obj)
来源：http://hu.huixinmuqiang.cn

TS:   structuredClone(obj)
来源：http://to.yuexingan06.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://xq.lnxyls.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://fj.asd995.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://te.lnxyls.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://un.jianghongdianzi.cn

[K06] 解析 URL 查询串
来源：http://yi.yuntaijiaju.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://uh.yuntaijiaju.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://xo.muxihuayi.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mf.bjjhwx.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cy.yuexingan06.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ys.hnjuh.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://px.newstarts.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://oo.haigaiapp.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://qs.haigaiapp.cn

[K07] 进制转换
来源：http://zm.huixinmuqiang.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://qu.521024.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://gs.szxytkj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://er.asd995.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://eu.huixinmuqiang.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://en.hnjuh.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://tm.521024.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://zd.wgjwhj.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://zm.szxytkj.cn

[K08] 二进制序列化（非 JSON）
来源：http://fc.bookmarksfly.cn

Py:   pickle.dumps(obj)
来源：http://xa.wgjwhj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://mt.shxzukj.cn

JS:   v8.serialize(obj)        // Node
来源：http://ex.jianghongdianzi.cn

TS:   v8.serialize(obj)        // Node
来源：http://wj.nicolike.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ux.shtwfgs.cn

Go:   encoding/gob
来源：http://zr.hnjuh.cn

Ruby: Marshal.dump(obj)
来源：http://ug.hnjuh.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qy.muxihuayi.cn

================================================================================
来源：http://id.szxytkj.cn

L. 网络请求
来源：http://fr.haigaiapp.cn

================================================================================
来源：http://nb.lnxyls.cn

[L01] 发送 GET 请求
来源：http://ae.shxzskj.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xi.panjiajie.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://qx.szxytkj.cn

JS:   await fetch(url)
来源：http://dg.hahajie.cn

TS:   await fetch(url)
来源：http://ur.yuexingan06.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://im.9csxet.cn

Go:   resp, err := http.Get(url)
来源：http://yq.newstarts.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://pj.muxihuayi.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://xv.nicolike.cn

[L02] 发送 POST JSON
来源：http://tv.nszjky.cn

Py:   requests.post(url, json={"a": 1})
来源：http://bo.nicolike.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://zz.huixinmuqiang.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://eg.nicolike.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bx.yuexingan06.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://jq.szsharing.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://or.huanxung.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://rz.panjiajie.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wg.huixiangedu.cn

[L03] 设置自定义请求头
来源：http://wg.asd995.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://im.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mk.panjiajie.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tj.huixinmuqiang.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hj.shtwfgs.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ak.newstarts.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://pd.shxzukj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://gt.wgjwhj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://pc.jianghongdianzi.cn

[L04] 设置超时
来源：http://xs.szxytkj.cn

Py:   requests.get(url, timeout=5)
来源：http://fe.hnjuh.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://kb.bookmarksfly.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://sl.521024.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://br.gzmigu.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ov.wgjwhj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://dy.asd995.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ll.szxytkj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://au.nszjky.cn

[L05] 上传文件（multipart）
来源：http://cs.huanxung.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://xk.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ze.asd995.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://vz.shxzskj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://nu.szsharing.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://yp.bookmarksfly.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ra.hahajie.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://se.hahajie.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://cc.nicolike.cn

[L06] 解析响应为 JSON
来源：http://gj.panjiajie.cn

Py:   resp.json()
来源：http://rr.huixiangedu.cn

PHP:  json_decode($body, true);
来源：http://ba.yuexingan06.cn

JS:   await resp.json()
来源：http://gu.shxzskj.cn

TS:   await resp.json()
来源：http://xt.9csxet.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ek.lnxyls.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ze.chemitech.net.cn

Ruby: JSON.parse(resp.body)
来源：http://vq.9csxet.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://jj.nicolike.cn

[L07] 处理 HTTP 状态码
来源：http://xx.asd995.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://tp.yuexingan06.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://oa.521024.cn

JS:   resp.ok;  resp.status
来源：http://zg.chemitech.net.cn

TS:   resp.ok;  resp.status
来源：http://hf.huanxung.cn

Java: resp.statusCode()
来源：http://td.bjjhwx.cn

Go:   resp.StatusCode
来源：http://bu.newstarts.cn

Ruby: resp.code.to_i
来源：http://kb.huixiangedu.cn

C#:   (int)resp.StatusCode
来源：http://qw.muxihuayi.cn

[L08] 并发请求多个地址
来源：http://nt.521024.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ol.szxytkj.cn

PHP:  curl_multi_init() 系列
来源：http://wl.chemitech.net.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pz.521024.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://aw.wgjwhj.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://lw.shxzukj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://fs.lnxyls.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://rz.521024.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xc.nicolike.cn

================================================================================
来源：http://yg.yuntaijiaju.cn

M. 命令行 / 进程 / 环境
来源：http://bo.shxzukj.cn

================================================================================
来源：http://qf.colortex.cn

[M01] 读取命令行参数
来源：http://bi.gzmigu.cn

Py:   sys.argv[1:]
来源：http://ax.haigaiapp.cn

PHP:  $argv;  $argc;
来源：http://py.haigaiapp.cn

JS:   process.argv.slice(2)
来源：http://sj.szxytkj.cn

TS:   process.argv.slice(2)
来源：http://xu.shxzukj.cn

Java: args 数组（main 方法参数）
来源：http://ji.shxzukj.cn

Go:   os.Args[1:]
来源：http://sq.panjiajie.cn

Ruby: ARGV
来源：http://ps.huixinmuqiang.cn

C#:   args 数组（Main 方法参数）
来源：http://mp.shxzskj.cn

[M02] 读取环境变量
来源：http://ob.yuexingan06.cn

Py:   os.environ.get("HOME")
来源：http://pl.bjjhwx.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://sf.newstarts.cn

JS:   process.env.HOME
来源：http://gq.haigaiapp.cn

TS:   process.env.HOME
来源：http://ys.huanxung.cn

Java: System.getenv("HOME")
来源：http://kd.yuexingan06.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://rr.yuntaijiaju.cn

Ruby: ENV["HOME"]
来源：http://mc.jctech888.com.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wd.jianghongdianzi.cn

[M03] 执行外部命令
来源：http://iq.9csxet.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://jw.huanxung.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ff.9csxet.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://yi.lnxyls.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ep.nicolike.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://bk.yuexingan06.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://yb.shxzskj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://og.szsharing.cn

C#:   Process.Start("ls", "-l");
来源：http://xg.gzmigu.cn

[M04] 获取当前工作目录
来源：http://eh.huixiangedu.cn

Py:   os.getcwd()
来源：http://jq.jctech888.com.cn

PHP:  getcwd();
来源：http://tl.yuntaijiaju.cn

JS:   process.cwd()
来源：http://gj.nszjky.cn

TS:   process.cwd()
来源：http://gw.huixinmuqiang.cn

Java: Path.of("").toAbsolutePath()
来源：http://hq.shxzskj.cn

Go:   os.Getwd()
来源：http://dx.lnxyls.cn

Ruby: Dir.pwd
来源：http://kp.lnxyls.cn

C#:   Directory.GetCurrentDirectory()
来源：http://iy.szxytkj.cn

[M05] 设置退出码
来源：http://ir.colortex.cn

Py:   sys.exit(1)
来源：http://vf.yuexingan06.cn

PHP:  exit(1);
来源：http://lh.lnxyls.cn

JS:   process.exit(1)
来源：http://lr.newstarts.cn

TS:   process.exit(1)
来源：http://gq.wgjwhj.cn

Java: System.exit(1)
来源：http://up.bjjhwx.cn

Go:   os.Exit(1)
来源：http://nf.newstarts.cn

Ruby: exit 1
来源：http://ak.huixiangedu.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ob.9csxet.cn

[M06] 向标准错误输出
来源：http://fm.jianghongdianzi.cn

Py:   print("err", file=sys.stderr)
来源：http://co.hnjuh.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://zo.szsharing.cn

JS:   console.error("err")
来源：http://tr.shxzskj.cn

TS:   console.error("err")
来源：http://vn.colortex.cn

Java: System.err.println("err")
来源：http://pq.gzmigu.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://sw.lnxyls.cn

Ruby: warn "err"
来源：http://ze.huanxung.cn

C#:   Console.Error.WriteLine("err")
来源：http://av.huanxung.cn

[M07] 判断是否为主入口
来源：http://mk.bookmarksfly.cn

Py:   if __name__ == "__main__":
来源：http://zj.yuexingan06.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://rg.nicolike.cn

JS:   require.main === module
来源：http://lf.9csxet.cn

TS:   require.main === module
来源：http://fb.jctech888.com.cn

Java: public static void main(String[] args)
来源：http://aw.colortex.cn

Go:   func main()
来源：http://rz.nszjky.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ao.yuntaijiaju.cn

C#:   static void Main(string[] args)
来源：http://cm.bookmarksfly.cn

[M08] 获取系统与运行时信息
来源：http://um.521024.cn

Py:   platform.system();  platform.python_version()
来源：http://mc.hnjuh.cn

PHP:  PHP_OS;  phpversion();
来源：http://jl.nicolike.cn

JS:   process.platform;  process.version
来源：http://nn.shxzukj.cn

TS:   process.platform;  process.version
来源：http://dl.yuntaijiaju.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://kb.colortex.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://hj.huanxung.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://yo.lnxyls.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://hr.shxzskj.cn

================================================================================
来源：http://qo.gzmigu.cn

N. 数据结构与算法
来源：http://qn.bjjhwx.cn

================================================================================
来源：http://cl.gzmigu.cn

[N01] 二分查找（有序数组）
来源：http://al.shtwfgs.cn

Py:   bisect.bisect_left(arr, x)
来源：http://yp.asd995.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://uf.shtwfgs.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dy.yuexingan06.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jt.hahajie.cn

Java: Arrays.binarySearch(arr, x)
来源：http://xm.panjiajie.cn

Go:   sort.SearchInts(arr, x)
来源：http://jx.asd995.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://st.521024.cn

C#:   Array.BinarySearch(arr, x)
来源：http://wr.huixiangedu.cn

[N02] 排序（工程实践用内置实现）
来源：http://uz.nszjky.cn

Py:   sorted(arr);  arr.sort()
来源：http://mv.huanxung.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://si.jianghongdianzi.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ud.wgjwhj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://vr.bookmarksfly.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://lz.chemitech.net.cn

Go:   slices.Sort(arr)
来源：http://dp.haigaiapp.cn

Ruby: arr.sort
来源：http://gf.nszjky.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://vh.wgjwhj.cn

[N03] 快速排序（分治示例）
来源：http://ia.szsharing.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://dc.muxihuayi.cn

PHP:  // 递归实现，或用 usort
来源：http://dy.9csxet.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ga.gzmigu.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ec.bjjhwx.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://oy.szsharing.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mn.newstarts.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://fa.yuntaijiaju.cn

C#:   // 手写递归，或 Array.Sort
来源：http://vc.huixiangedu.cn

[N04] 斐波那契数列
来源：http://do.szsharing.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ch.huixiangedu.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://gh.521024.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://te.asd995.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pc.gzmigu.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://je.jctech888.com.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://zu.panjiajie.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://nf.521024.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://fh.huanxung.cn

[N05] 最大公约数
来源：http://xm.jianghongdianzi.cn

Py:   math.gcd(a, b)
来源：http://os.521024.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ff.bjjhwx.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tt.huanxung.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://al.hnjuh.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://pt.wgjwhj.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://bk.huixinmuqiang.cn

Ruby: a.gcd(b)
来源：http://jn.huixiangedu.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://pr.521024.cn

[N06] 判断回文字符串
来源：http://fv.nszjky.cn

Py:   s == s[::-1]
来源：http://ee.nszjky.cn

PHP:  $s === strrev($s);
来源：http://zu.shtwfgs.cn

JS:   s === [...s].reverse().join("")
来源：http://ev.muxihuayi.cn

TS:   s === [...s].reverse().join("")
来源：http://bm.521024.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://rm.jianghongdianzi.cn

Go:   // 双指针从两端比较
来源：http://bu.nicolike.cn

Ruby: s == s.reverse
来源：http://hd.colortex.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://fp.huixiangedu.cn

[N07] 两数之和（返回下标）
来源：http://io.lnxyls.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://nv.bjjhwx.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://xe.shtwfgs.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://bs.9csxet.cn

TS:   // 手写 Map<string, number>
来源：http://gd.hnjuh.cn

Java: // 手写 HashMap
来源：http://rj.jctech888.com.cn

Go:   // 手写 map[int]int
来源：http://kv.chemitech.net.cn

Ruby: // 手写 Hash
来源：http://ji.shxzukj.cn

C#:   // 手写 Dictionary<int, int>
来源：http://fy.lnxyls.cn

[N08] 生成全排列
来源：http://jb.gzmigu.cn

Py:   itertools.permutations(arr)
来源：http://aj.yuntaijiaju.cn

PHP:  // 手写递归交换
来源：http://qx.nszjky.cn

JS:   // 手写回溯递归
来源：http://rg.wgjwhj.cn

TS:   // 手写回溯递归
来源：http://qw.hnjuh.cn

Java: // 手写回溯递归
来源：http://wd.bjjhwx.cn

Go:   // 手写回溯递归
来源：http://je.bjjhwx.cn

Ruby: arr.permutation.to_a
来源：http://xq.huixiangedu.cn

C#:   // 手写回溯递归
来源：http://qp.colortex.cn

[N09] 栈与队列
来源：http://ae.bookmarksfly.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://vy.gzmigu.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://iv.newstarts.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://bw.panjiajie.cn


<!-- 参考信息 -->