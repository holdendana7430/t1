代发 wailian999

[K02] JSON 字符串转对象
来源：http://qw.yuexingan06.cn

Py:   json.loads(s)
来源：http://hi.colortex.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ti.shxzukj.cn

JS:   JSON.parse(s)
来源：http://jo.yuntaijiaju.cn

TS:   JSON.parse(s)
来源：http://oe.shxzukj.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ms.gzmigu.cn

Go:   json.Unmarshal(data, &v)
来源：http://uf.huixiangedu.cn

Ruby: JSON.parse(s)
来源：http://zs.yuntaijiaju.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hr.panjiajie.cn

[K03] JSON 美化输出（带缩进）
来源：http://vf.lnxyls.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://cl.nicolike.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://if.panjiajie.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ap.chemitech.net.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://oy.shxzukj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://bb.chemitech.net.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://nh.panjiajie.cn

Ruby: JSON.pretty_generate(obj)
来源：http://bx.hnjuh.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ib.huixiangedu.cn

[K04] 读取 JSON 文件
来源：http://dm.bookmarksfly.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://qx.panjiajie.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wy.shxzukj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://or.nicolike.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wk.muxihuayi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://rd.nszjky.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://sw.hahajie.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://po.hnjuh.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://zq.colortex.cn

[K05] 深拷贝对象
来源：http://ay.huixiangedu.cn

Py:   copy.deepcopy(obj)
来源：http://fi.nicolike.cn

PHP:  unserialize(serialize($obj));
来源：http://vs.lnxyls.cn

JS:   structuredClone(obj)
来源：http://pg.panjiajie.cn

TS:   structuredClone(obj)
来源：http://sn.huixinmuqiang.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://dq.bookmarksfly.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qw.panjiajie.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://fo.hnjuh.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://mf.jctech888.com.cn

[K06] 解析 URL 查询串
来源：http://lf.huanxung.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://oc.nszjky.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://be.bjjhwx.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tn.muxihuayi.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fr.colortex.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://jc.jianghongdianzi.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://om.nszjky.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://yj.colortex.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://jr.jctech888.com.cn

[K07] 进制转换
来源：http://mg.muxihuayi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://kd.shxzskj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://oq.chemitech.net.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://lz.9csxet.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://vv.jianghongdianzi.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://cd.shxzukj.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://xp.wgjwhj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ia.huixiangedu.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://xb.bjjhwx.cn

[K08] 二进制序列化（非 JSON）
来源：http://xl.lnxyls.cn

Py:   pickle.dumps(obj)
来源：http://mn.hnjuh.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ce.newstarts.cn

JS:   v8.serialize(obj)        // Node
来源：http://tv.hahajie.cn

TS:   v8.serialize(obj)        // Node
来源：http://tt.bjjhwx.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://yj.panjiajie.cn

Go:   encoding/gob
来源：http://eg.nicolike.cn

Ruby: Marshal.dump(obj)
来源：http://rk.shxzukj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://pu.jianghongdianzi.cn

================================================================================
来源：http://xb.wgjwhj.cn

L. 网络请求
来源：http://uf.huixiangedu.cn

================================================================================
来源：http://kg.huixinmuqiang.cn

[L01] 发送 GET 请求
来源：http://po.colortex.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://dk.nicolike.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://bq.shxzskj.cn

JS:   await fetch(url)
来源：http://vw.szxytkj.cn

TS:   await fetch(url)
来源：http://sq.nszjky.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://oo.yuntaijiaju.cn

Go:   resp, err := http.Get(url)
来源：http://fl.colortex.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://fo.shxzukj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://bq.jctech888.com.cn

[L02] 发送 POST JSON
来源：http://ic.hnjuh.cn

Py:   requests.post(url, json={"a": 1})
来源：http://rn.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://cd.asd995.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rd.nszjky.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ay.shxzskj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://rz.jctech888.com.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ou.shxzukj.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wk.bookmarksfly.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://au.chemitech.net.cn

[L03] 设置自定义请求头
来源：http://in.bjjhwx.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://cu.szxytkj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://kf.newstarts.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://en.newstarts.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ug.shtwfgs.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://zc.huanxung.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://qh.huixinmuqiang.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://vy.huixiangedu.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://lr.huixiangedu.cn

[L04] 设置超时
来源：http://zl.bookmarksfly.cn

Py:   requests.get(url, timeout=5)
来源：http://ig.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://yk.hnjuh.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dl.shtwfgs.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ka.hnjuh.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://si.yuntaijiaju.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://vv.9csxet.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://xq.shxzukj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mq.gzmigu.cn

[L05] 上传文件（multipart）
来源：http://km.bookmarksfly.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://kx.wgjwhj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ky.muxihuayi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://km.9csxet.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://nw.huixinmuqiang.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vw.panjiajie.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hd.panjiajie.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://cn.szxytkj.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://qx.lnxyls.cn

[L06] 解析响应为 JSON
来源：http://he.shxzukj.cn

Py:   resp.json()
来源：http://eh.yuntaijiaju.cn

PHP:  json_decode($body, true);
来源：http://js.bookmarksfly.cn

JS:   await resp.json()
来源：http://ee.shxzukj.cn

TS:   await resp.json()
来源：http://uc.hahajie.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ti.huixinmuqiang.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wd.szsharing.cn

Ruby: JSON.parse(resp.body)
来源：http://mu.lnxyls.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://pn.panjiajie.cn

[L07] 处理 HTTP 状态码
来源：http://wu.huixiangedu.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://rm.haigaiapp.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://op.hahajie.cn

JS:   resp.ok;  resp.status
来源：http://af.huanxung.cn

TS:   resp.ok;  resp.status
来源：http://ua.shxzskj.cn

Java: resp.statusCode()
来源：http://fc.huanxung.cn

Go:   resp.StatusCode
来源：http://oe.chemitech.net.cn

Ruby: resp.code.to_i
来源：http://ag.wgjwhj.cn

C#:   (int)resp.StatusCode
来源：http://zr.nicolike.cn

[L08] 并发请求多个地址
来源：http://be.nicolike.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wu.asd995.cn

PHP:  curl_multi_init() 系列
来源：http://nh.szsharing.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://td.newstarts.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://en.newstarts.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://nw.huanxung.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://vw.hahajie.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hp.newstarts.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://pe.asd995.cn

================================================================================
来源：http://kk.wgjwhj.cn

M. 命令行 / 进程 / 环境
来源：http://ej.muxihuayi.cn

================================================================================
来源：http://zw.huixinmuqiang.cn

[M01] 读取命令行参数
来源：http://ky.hnjuh.cn

Py:   sys.argv[1:]
来源：http://er.nszjky.cn

PHP:  $argv;  $argc;
来源：http://ju.jianghongdianzi.cn

JS:   process.argv.slice(2)
来源：http://wf.jctech888.com.cn

TS:   process.argv.slice(2)
来源：http://vh.nszjky.cn

Java: args 数组（main 方法参数）
来源：http://op.newstarts.cn

Go:   os.Args[1:]
来源：http://pa.newstarts.cn

Ruby: ARGV
来源：http://ee.wgjwhj.cn

C#:   args 数组（Main 方法参数）
来源：http://av.lnxyls.cn

[M02] 读取环境变量
来源：http://ow.panjiajie.cn

Py:   os.environ.get("HOME")
来源：http://yr.huixinmuqiang.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zx.shxzskj.cn

JS:   process.env.HOME
来源：http://ns.shxzskj.cn

TS:   process.env.HOME
来源：http://ns.bjjhwx.cn

Java: System.getenv("HOME")
来源：http://ox.huixiangedu.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://yl.colortex.cn

Ruby: ENV["HOME"]
来源：http://xo.521024.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://br.wgjwhj.cn

[M03] 执行外部命令
来源：http://yo.521024.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://pu.shtwfgs.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://iz.shtwfgs.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://jl.yuntaijiaju.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://tl.colortex.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://cm.521024.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://qi.shtwfgs.cn

Ruby: system("ls -l");  `ls -l`
来源：http://xn.gzmigu.cn

C#:   Process.Start("ls", "-l");
来源：http://wv.hahajie.cn

[M04] 获取当前工作目录
来源：http://kz.gzmigu.cn

Py:   os.getcwd()
来源：http://fq.lnxyls.cn

PHP:  getcwd();
来源：http://se.newstarts.cn

JS:   process.cwd()
来源：http://pw.asd995.cn

TS:   process.cwd()
来源：http://lk.panjiajie.cn

Java: Path.of("").toAbsolutePath()
来源：http://az.shxzskj.cn

Go:   os.Getwd()
来源：http://dw.shxzskj.cn

Ruby: Dir.pwd
来源：http://tr.gzmigu.cn

C#:   Directory.GetCurrentDirectory()
来源：http://xx.shxzukj.cn

[M05] 设置退出码
来源：http://ht.panjiajie.cn

Py:   sys.exit(1)
来源：http://sf.shtwfgs.cn

PHP:  exit(1);
来源：http://jb.nicolike.cn

JS:   process.exit(1)
来源：http://it.huanxung.cn

TS:   process.exit(1)
来源：http://or.newstarts.cn

Java: System.exit(1)
来源：http://dx.yuntaijiaju.cn

Go:   os.Exit(1)
来源：http://lk.wgjwhj.cn

Ruby: exit 1
来源：http://dx.bookmarksfly.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://iq.asd995.cn

[M06] 向标准错误输出
来源：http://lw.newstarts.cn

Py:   print("err", file=sys.stderr)
来源：http://fq.huixinmuqiang.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://sk.gzmigu.cn

JS:   console.error("err")
来源：http://ah.huixiangedu.cn

TS:   console.error("err")
来源：http://ru.shtwfgs.cn

Java: System.err.println("err")
来源：http://oy.yuntaijiaju.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://zn.lnxyls.cn

Ruby: warn "err"
来源：http://fw.yuntaijiaju.cn

C#:   Console.Error.WriteLine("err")
来源：http://xz.yuntaijiaju.cn

[M07] 判断是否为主入口
来源：http://xc.hahajie.cn

Py:   if __name__ == "__main__":
来源：http://in.shxzukj.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ja.yuntaijiaju.cn

JS:   require.main === module
来源：http://kf.jctech888.com.cn

TS:   require.main === module
来源：http://ev.jctech888.com.cn

Java: public static void main(String[] args)
来源：http://tz.huanxung.cn

Go:   func main()
来源：http://vo.hahajie.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://pi.panjiajie.cn

C#:   static void Main(string[] args)
来源：http://xr.asd995.cn

[M08] 获取系统与运行时信息
来源：http://gl.szxytkj.cn

Py:   platform.system();  platform.python_version()
来源：http://ai.szsharing.cn

PHP:  PHP_OS;  phpversion();
来源：http://rd.nszjky.cn

JS:   process.platform;  process.version
来源：http://rc.panjiajie.cn

TS:   process.platform;  process.version
来源：http://ko.hahajie.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://aq.panjiajie.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://xl.nszjky.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://kx.jianghongdianzi.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ie.newstarts.cn

================================================================================
来源：http://dn.newstarts.cn

N. 数据结构与算法
来源：http://mf.huixinmuqiang.cn

================================================================================
来源：http://mp.panjiajie.cn

[N01] 二分查找（有序数组）
来源：http://um.bookmarksfly.cn

Py:   bisect.bisect_left(arr, x)
来源：http://qz.lnxyls.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ar.huixinmuqiang.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fg.yuntaijiaju.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ff.panjiajie.cn

Java: Arrays.binarySearch(arr, x)
来源：http://lr.nszjky.cn

Go:   sort.SearchInts(arr, x)
来源：http://jg.bjjhwx.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://kk.colortex.cn

C#:   Array.BinarySearch(arr, x)
来源：http://rw.yuexingan06.cn

[N02] 排序（工程实践用内置实现）
来源：http://tc.shtwfgs.cn

Py:   sorted(arr);  arr.sort()
来源：http://jp.hahajie.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://nz.yuexingan06.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://jh.huixinmuqiang.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://pf.nicolike.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hq.gzmigu.cn

Go:   slices.Sort(arr)
来源：http://wt.lnxyls.cn

Ruby: arr.sort
来源：http://rw.nszjky.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://sm.shxzukj.cn

[N03] 快速排序（分治示例）
来源：http://tt.muxihuayi.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://pd.huixiangedu.cn

PHP:  // 递归实现，或用 usort
来源：http://zf.shxzukj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://af.asd995.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vm.nszjky.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://lt.muxihuayi.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://tp.huixiangedu.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://jc.yuexingan06.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ll.newstarts.cn

[N04] 斐波那契数列
来源：http://sv.bjjhwx.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ct.shxzukj.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://eo.bjjhwx.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cu.muxihuayi.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ng.colortex.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mq.shxzskj.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://gb.chemitech.net.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://yp.muxihuayi.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://lc.521024.cn

[N05] 最大公约数
来源：http://mt.shxzskj.cn

Py:   math.gcd(a, b)
来源：http://kh.gzmigu.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://nt.asd995.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bt.jianghongdianzi.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nj.shtwfgs.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://pn.jctech888.com.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://sg.nszjky.cn

Ruby: a.gcd(b)
来源：http://nx.9csxet.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://vv.szsharing.cn

[N06] 判断回文字符串
来源：http://yf.lnxyls.cn

Py:   s == s[::-1]
来源：http://ni.521024.cn

PHP:  $s === strrev($s);
来源：http://rz.huixiangedu.cn

JS:   s === [...s].reverse().join("")
来源：http://rt.lnxyls.cn

TS:   s === [...s].reverse().join("")
来源：http://in.nicolike.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://in.yuexingan06.cn

Go:   // 双指针从两端比较
来源：http://aj.jianghongdianzi.cn

Ruby: s == s.reverse
来源：http://qe.gzmigu.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://jw.yuexingan06.cn

[N07] 两数之和（返回下标）
来源：http://gl.nszjky.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://fr.nszjky.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ct.hnjuh.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://sp.szsharing.cn

TS:   // 手写 Map<string, number>
来源：http://gu.bjjhwx.cn

Java: // 手写 HashMap
来源：http://kt.huixinmuqiang.cn

Go:   // 手写 map[int]int
来源：http://fc.szxytkj.cn

Ruby: // 手写 Hash
来源：http://cx.nszjky.cn

C#:   // 手写 Dictionary<int, int>
来源：http://rj.nszjky.cn

[N08] 生成全排列
来源：http://dm.shtwfgs.cn

Py:   itertools.permutations(arr)
来源：http://zb.shtwfgs.cn

PHP:  // 手写递归交换
来源：http://mp.newstarts.cn

JS:   // 手写回溯递归
来源：http://cd.wgjwhj.cn

TS:   // 手写回溯递归
来源：http://ib.nszjky.cn

Java: // 手写回溯递归
来源：http://ka.9csxet.cn

Go:   // 手写回溯递归
来源：http://lq.shxzskj.cn

Ruby: arr.permutation.to_a
来源：http://te.nicolike.cn

C#:   // 手写回溯递归
来源：http://qv.chemitech.net.cn

[N09] 栈与队列
来源：http://qc.hahajie.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://lr.wgjwhj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://qw.newstarts.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://lz.gzmigu.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ww.shxzukj.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://tv.muxihuayi.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ax.newstarts.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ey.yuntaijiaju.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ut.panjiajie.cn

[N10] 链表节点定义
来源：http://ze.asd995.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ng.yuexingan06.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://aw.jctech888.com.cn


<!-- 参考信息 -->