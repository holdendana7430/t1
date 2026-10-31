代发 wailian999

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://xy.hnjuh.cn

Go:   json.Marshal(obj)
来源：http://ig.lnxyls.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ir.yuntaijiaju.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://sp.colortex.cn

[K02] JSON 字符串转对象
来源：http://vf.shxzukj.cn

Py:   json.loads(s)
来源：http://ss.szxytkj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://iv.hahajie.cn

JS:   JSON.parse(s)
来源：http://df.bjjhwx.cn

TS:   JSON.parse(s)
来源：http://jy.nszjky.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://dt.521024.cn

Go:   json.Unmarshal(data, &v)
来源：http://ha.jianghongdianzi.cn

Ruby: JSON.parse(s)
来源：http://gv.9csxet.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://rv.521024.cn

[K03] JSON 美化输出（带缩进）
来源：http://up.wgjwhj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://qc.yuntaijiaju.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://xd.521024.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://oj.jctech888.com.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://zz.yuexingan06.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://lc.yuexingan06.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ze.yuntaijiaju.cn

Ruby: JSON.pretty_generate(obj)
来源：http://bh.szsharing.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://gi.chemitech.net.cn

[K04] 读取 JSON 文件
来源：http://jy.shxzukj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://xd.newstarts.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://tc.yuntaijiaju.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vo.gzmigu.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://oh.szsharing.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wg.shxzskj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://bh.yuexingan06.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://fn.shxzskj.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://qp.colortex.cn

[K05] 深拷贝对象
来源：http://hs.wgjwhj.cn

Py:   copy.deepcopy(obj)
来源：http://ds.bookmarksfly.cn

PHP:  unserialize(serialize($obj));
来源：http://ym.yuntaijiaju.cn

JS:   structuredClone(obj)
来源：http://tc.huanxung.cn

TS:   structuredClone(obj)
来源：http://rd.huixinmuqiang.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://dn.asd995.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://yv.newstarts.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wh.szsharing.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://sf.jctech888.com.cn

[K06] 解析 URL 查询串
来源：http://bu.newstarts.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ot.asd995.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://lh.szxytkj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vs.huixiangedu.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nc.nicolike.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://lb.wgjwhj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ew.colortex.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://yz.haigaiapp.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://es.szsharing.cn

[K07] 进制转换
来源：http://xq.jctech888.com.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://yg.nicolike.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://tp.hahajie.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://pr.shxzskj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://xz.jctech888.com.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mz.szxytkj.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wv.yuntaijiaju.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qn.lnxyls.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ze.muxihuayi.cn

[K08] 二进制序列化（非 JSON）
来源：http://wf.521024.cn

Py:   pickle.dumps(obj)
来源：http://fy.haigaiapp.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://kd.asd995.cn

JS:   v8.serialize(obj)        // Node
来源：http://ic.shxzskj.cn

TS:   v8.serialize(obj)        // Node
来源：http://dn.asd995.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ys.huanxung.cn

Go:   encoding/gob
来源：http://hn.lnxyls.cn

Ruby: Marshal.dump(obj)
来源：http://ns.huixinmuqiang.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mx.asd995.cn

================================================================================
来源：http://it.bjjhwx.cn

L. 网络请求
来源：http://xa.bookmarksfly.cn

================================================================================
来源：http://se.szxytkj.cn

[L01] 发送 GET 请求
来源：http://to.hnjuh.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://um.jianghongdianzi.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://oa.haigaiapp.cn

JS:   await fetch(url)
来源：http://un.jctech888.com.cn

TS:   await fetch(url)
来源：http://xl.szsharing.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://bw.chemitech.net.cn

Go:   resp, err := http.Get(url)
来源：http://fx.bjjhwx.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://tb.szsharing.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ms.yuexingan06.cn

[L02] 发送 POST JSON
来源：http://ui.muxihuayi.cn

Py:   requests.post(url, json={"a": 1})
来源：http://xu.521024.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://lq.huixiangedu.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fs.bjjhwx.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pj.wgjwhj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://yc.newstarts.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://dm.asd995.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://vu.huixinmuqiang.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://yh.muxihuayi.cn

[L03] 设置自定义请求头
来源：http://yy.huixinmuqiang.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ka.shtwfgs.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ns.bookmarksfly.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wn.newstarts.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rk.huixiangedu.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://le.hahajie.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ua.shtwfgs.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://yv.shtwfgs.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://pp.bookmarksfly.cn

[L04] 设置超时
来源：http://bk.chemitech.net.cn

Py:   requests.get(url, timeout=5)
来源：http://qj.gzmigu.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://jd.panjiajie.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xk.newstarts.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dx.yuntaijiaju.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://gy.9csxet.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://zy.yuexingan06.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://gg.panjiajie.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://bd.gzmigu.cn

[L05] 上传文件（multipart）
来源：http://fr.panjiajie.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://nt.gzmigu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://gn.yuntaijiaju.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wq.huanxung.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://jc.hnjuh.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ci.muxihuayi.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://tz.yuexingan06.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://zr.nszjky.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ox.nszjky.cn

[L06] 解析响应为 JSON
来源：http://ac.colortex.cn

Py:   resp.json()
来源：http://gp.nszjky.cn

PHP:  json_decode($body, true);
来源：http://uk.521024.cn

JS:   await resp.json()
来源：http://ik.bjjhwx.cn

TS:   await resp.json()
来源：http://ht.lnxyls.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://tl.jianghongdianzi.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://eb.bookmarksfly.cn

Ruby: JSON.parse(resp.body)
来源：http://zc.shtwfgs.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://pt.shxzukj.cn

[L07] 处理 HTTP 状态码
来源：http://dn.huixiangedu.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://gg.shxzskj.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://yt.jianghongdianzi.cn

JS:   resp.ok;  resp.status
来源：http://mj.szxytkj.cn

TS:   resp.ok;  resp.status
来源：http://tr.shxzukj.cn

Java: resp.statusCode()
来源：http://ba.yuntaijiaju.cn

Go:   resp.StatusCode
来源：http://oy.haigaiapp.cn

Ruby: resp.code.to_i
来源：http://oo.nszjky.cn

C#:   (int)resp.StatusCode
来源：http://ka.szsharing.cn

[L08] 并发请求多个地址
来源：http://wj.szsharing.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mz.shxzskj.cn

PHP:  curl_multi_init() 系列
来源：http://bd.bookmarksfly.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lm.shxzskj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wg.jctech888.com.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://kb.chemitech.net.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wc.szsharing.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://me.muxihuayi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ou.lnxyls.cn

================================================================================
来源：http://jn.shxzukj.cn

M. 命令行 / 进程 / 环境
来源：http://kw.nszjky.cn

================================================================================
来源：http://qc.muxihuayi.cn

[M01] 读取命令行参数
来源：http://sa.muxihuayi.cn

Py:   sys.argv[1:]
来源：http://bw.huanxung.cn

PHP:  $argv;  $argc;
来源：http://ez.huixiangedu.cn

JS:   process.argv.slice(2)
来源：http://gd.hahajie.cn

TS:   process.argv.slice(2)
来源：http://rg.nszjky.cn

Java: args 数组（main 方法参数）
来源：http://un.asd995.cn

Go:   os.Args[1:]
来源：http://wn.szxytkj.cn

Ruby: ARGV
来源：http://kc.colortex.cn

C#:   args 数组（Main 方法参数）
来源：http://iv.shxzskj.cn

[M02] 读取环境变量
来源：http://qy.yuexingan06.cn

Py:   os.environ.get("HOME")
来源：http://ny.wgjwhj.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://sf.yuexingan06.cn

JS:   process.env.HOME
来源：http://db.jianghongdianzi.cn

TS:   process.env.HOME
来源：http://mf.huixinmuqiang.cn

Java: System.getenv("HOME")
来源：http://zt.chemitech.net.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://in.shxzukj.cn

Ruby: ENV["HOME"]
来源：http://jw.shxzskj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hs.newstarts.cn

[M03] 执行外部命令
来源：http://wn.huixiangedu.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://lo.521024.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zo.hnjuh.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://wr.jianghongdianzi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://bq.colortex.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://yi.yuexingan06.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://zu.wgjwhj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://bb.nicolike.cn

C#:   Process.Start("ls", "-l");
来源：http://tl.szxytkj.cn

[M04] 获取当前工作目录
来源：http://np.haigaiapp.cn

Py:   os.getcwd()
来源：http://yj.muxihuayi.cn

PHP:  getcwd();
来源：http://at.yuexingan06.cn

JS:   process.cwd()
来源：http://no.yuntaijiaju.cn

TS:   process.cwd()
来源：http://fk.hahajie.cn

Java: Path.of("").toAbsolutePath()
来源：http://mi.hahajie.cn

Go:   os.Getwd()
来源：http://op.jctech888.com.cn

Ruby: Dir.pwd
来源：http://xc.yuexingan06.cn

C#:   Directory.GetCurrentDirectory()
来源：http://mk.9csxet.cn

[M05] 设置退出码
来源：http://sn.shtwfgs.cn

Py:   sys.exit(1)
来源：http://ht.huixiangedu.cn

PHP:  exit(1);
来源：http://xv.szxytkj.cn

JS:   process.exit(1)
来源：http://aw.hnjuh.cn

TS:   process.exit(1)
来源：http://jm.shxzskj.cn

Java: System.exit(1)
来源：http://th.colortex.cn

Go:   os.Exit(1)
来源：http://zj.hahajie.cn

Ruby: exit 1
来源：http://pp.chemitech.net.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ob.muxihuayi.cn

[M06] 向标准错误输出
来源：http://ei.jctech888.com.cn

Py:   print("err", file=sys.stderr)
来源：http://zq.wgjwhj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://yi.9csxet.cn

JS:   console.error("err")
来源：http://ct.huanxung.cn

TS:   console.error("err")
来源：http://uu.gzmigu.cn

Java: System.err.println("err")
来源：http://ma.jianghongdianzi.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://yo.shtwfgs.cn

Ruby: warn "err"
来源：http://ou.wgjwhj.cn

C#:   Console.Error.WriteLine("err")
来源：http://gk.gzmigu.cn

[M07] 判断是否为主入口
来源：http://kx.bookmarksfly.cn

Py:   if __name__ == "__main__":
来源：http://bq.asd995.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://lm.lnxyls.cn

JS:   require.main === module
来源：http://wj.hahajie.cn

TS:   require.main === module
来源：http://nh.colortex.cn

Java: public static void main(String[] args)
来源：http://jl.9csxet.cn

Go:   func main()
来源：http://sa.szxytkj.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://bd.gzmigu.cn

C#:   static void Main(string[] args)
来源：http://dw.gzmigu.cn

[M08] 获取系统与运行时信息
来源：http://sq.nicolike.cn

Py:   platform.system();  platform.python_version()
来源：http://iz.yuntaijiaju.cn

PHP:  PHP_OS;  phpversion();
来源：http://sw.bookmarksfly.cn

JS:   process.platform;  process.version
来源：http://ve.nicolike.cn

TS:   process.platform;  process.version
来源：http://qr.nicolike.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://np.huixiangedu.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ad.haigaiapp.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://un.bjjhwx.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://rt.nszjky.cn

================================================================================
来源：http://dw.bjjhwx.cn

N. 数据结构与算法
来源：http://ji.panjiajie.cn

================================================================================
来源：http://kw.muxihuayi.cn

[N01] 二分查找（有序数组）
来源：http://br.muxihuayi.cn

Py:   bisect.bisect_left(arr, x)
来源：http://zv.muxihuayi.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://kw.asd995.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vy.bookmarksfly.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hf.shtwfgs.cn

Java: Arrays.binarySearch(arr, x)
来源：http://yu.wgjwhj.cn

Go:   sort.SearchInts(arr, x)
来源：http://hu.hahajie.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://lx.shxzukj.cn

C#:   Array.BinarySearch(arr, x)
来源：http://bu.szsharing.cn

[N02] 排序（工程实践用内置实现）
来源：http://sb.newstarts.cn

Py:   sorted(arr);  arr.sort()
来源：http://od.colortex.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://qb.hnjuh.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ba.jctech888.com.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://yr.haigaiapp.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://cv.muxihuayi.cn

Go:   slices.Sort(arr)
来源：http://qm.hahajie.cn

Ruby: arr.sort
来源：http://vx.newstarts.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://vh.wgjwhj.cn

[N03] 快速排序（分治示例）
来源：http://ng.huixiangedu.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ja.huixinmuqiang.cn

PHP:  // 递归实现，或用 usort
来源：http://nz.yuexingan06.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://oh.lnxyls.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vm.jctech888.com.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://zq.nszjky.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://tt.shxzukj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://px.yuexingan06.cn

C#:   // 手写递归，或 Array.Sort
来源：http://om.huixiangedu.cn

[N04] 斐波那契数列
来源：http://ya.521024.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://tq.nicolike.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://da.wgjwhj.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hc.huixiangedu.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lv.gzmigu.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://sj.shxzskj.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://cq.szsharing.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ek.jctech888.com.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://sb.asd995.cn

[N05] 最大公约数
来源：http://qn.hnjuh.cn

Py:   math.gcd(a, b)
来源：http://dt.jctech888.com.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://xl.9csxet.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sq.bookmarksfly.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://re.lnxyls.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://qw.huanxung.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://kd.yuntaijiaju.cn

Ruby: a.gcd(b)
来源：http://rm.hnjuh.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://js.gzmigu.cn

[N06] 判断回文字符串
来源：http://wz.jctech888.com.cn

Py:   s == s[::-1]
来源：http://ly.yuexingan06.cn

PHP:  $s === strrev($s);
来源：http://xk.newstarts.cn

JS:   s === [...s].reverse().join("")
来源：http://jy.yuexingan06.cn

TS:   s === [...s].reverse().join("")
来源：http://nv.shxzskj.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://uv.huixiangedu.cn

Go:   // 双指针从两端比较
来源：http://du.szxytkj.cn

Ruby: s == s.reverse
来源：http://uj.muxihuayi.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ff.bjjhwx.cn

[N07] 两数之和（返回下标）
来源：http://oy.huixinmuqiang.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://cl.huanxung.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jr.nszjky.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://tx.hahajie.cn

TS:   // 手写 Map<string, number>
来源：http://mx.bjjhwx.cn

Java: // 手写 HashMap
来源：http://kr.huixinmuqiang.cn

Go:   // 手写 map[int]int
来源：http://if.wgjwhj.cn

Ruby: // 手写 Hash
来源：http://ix.gzmigu.cn

C#:   // 手写 Dictionary<int, int>
来源：http://dc.shxzskj.cn

[N08] 生成全排列
来源：http://kw.lnxyls.cn

Py:   itertools.permutations(arr)
来源：http://sg.bjjhwx.cn

PHP:  // 手写递归交换
来源：http://yx.chemitech.net.cn

JS:   // 手写回溯递归
来源：http://uh.szxytkj.cn

TS:   // 手写回溯递归
来源：http://zj.haigaiapp.cn

Java: // 手写回溯递归
来源：http://ja.muxihuayi.cn

Go:   // 手写回溯递归
来源：http://ie.szsharing.cn

Ruby: arr.permutation.to_a
来源：http://qt.yuntaijiaju.cn

C#:   // 手写回溯递归
来源：http://nu.lnxyls.cn

[N09] 栈与队列
来源：http://lu.hahajie.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://vq.yuntaijiaju.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ep.shxzskj.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://sy.muxihuayi.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ix.yuexingan06.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://er.nicolike.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://cy.huixinmuqiang.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://er.hnjuh.cn


<!-- 参考信息 -->