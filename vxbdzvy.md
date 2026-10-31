代发 wailian999

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mn.huixiangedu.cn

Go:   json.Marshal(obj)
来源：http://qq.shtwfgs.cn

Ruby: obj.to_json                                     // require "json"
来源：http://rg.huixinmuqiang.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://et.szxytkj.cn

[K02] JSON 字符串转对象
来源：http://ot.haigaiapp.cn

Py:   json.loads(s)
来源：http://hf.huanxung.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://dc.panjiajie.cn

JS:   JSON.parse(s)
来源：http://yx.nszjky.cn

TS:   JSON.parse(s)
来源：http://vi.newstarts.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://aa.shxzukj.cn

Go:   json.Unmarshal(data, &v)
来源：http://uk.jctech888.com.cn

Ruby: JSON.parse(s)
来源：http://cj.huixiangedu.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://db.colortex.cn

[K03] JSON 美化输出（带缩进）
来源：http://lh.nicolike.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://lj.panjiajie.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://fq.asd995.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://bf.9csxet.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://mu.szsharing.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ll.muxihuayi.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ny.shxzukj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://nj.panjiajie.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://oc.gzmigu.cn

[K04] 读取 JSON 文件
来源：http://qu.newstarts.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://zw.yuntaijiaju.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://nj.asd995.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yz.jctech888.com.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xk.huixiangedu.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ox.hahajie.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://jk.szxytkj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://lx.shtwfgs.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://bv.yuexingan06.cn

[K05] 深拷贝对象
来源：http://ot.huanxung.cn

Py:   copy.deepcopy(obj)
来源：http://pv.huixinmuqiang.cn

PHP:  unserialize(serialize($obj));
来源：http://kv.colortex.cn

JS:   structuredClone(obj)
来源：http://rn.haigaiapp.cn

TS:   structuredClone(obj)
来源：http://op.szsharing.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://kp.panjiajie.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ui.bjjhwx.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://et.asd995.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://kl.colortex.cn

[K06] 解析 URL 查询串
来源：http://nv.521024.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://sz.newstarts.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zq.muxihuayi.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jy.9csxet.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gn.muxihuayi.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://we.shtwfgs.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://kj.bookmarksfly.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wn.chemitech.net.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zz.huanxung.cn

[K07] 进制转换
来源：http://uo.szsharing.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://yz.muxihuayi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hc.haigaiapp.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://yf.haigaiapp.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://tu.newstarts.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://qd.huanxung.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ve.yuntaijiaju.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://vn.szxytkj.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://is.hnjuh.cn

[K08] 二进制序列化（非 JSON）
来源：http://le.szsharing.cn

Py:   pickle.dumps(obj)
来源：http://hx.hnjuh.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://wl.nicolike.cn

JS:   v8.serialize(obj)        // Node
来源：http://bl.jctech888.com.cn

TS:   v8.serialize(obj)        // Node
来源：http://jz.asd995.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wl.bjjhwx.cn

Go:   encoding/gob
来源：http://uv.huixiangedu.cn

Ruby: Marshal.dump(obj)
来源：http://xk.asd995.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mi.huixinmuqiang.cn

================================================================================
来源：http://rn.9csxet.cn

L. 网络请求
来源：http://mh.gzmigu.cn

================================================================================
来源：http://zi.huixiangedu.cn

[L01] 发送 GET 请求
来源：http://ly.nszjky.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hb.huixinmuqiang.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://qt.haigaiapp.cn

JS:   await fetch(url)
来源：http://jv.szsharing.cn

TS:   await fetch(url)
来源：http://py.asd995.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://js.newstarts.cn

Go:   resp, err := http.Get(url)
来源：http://wz.panjiajie.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://qz.yuexingan06.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hq.yuexingan06.cn

[L02] 发送 POST JSON
来源：http://lc.yuexingan06.cn

Py:   requests.post(url, json={"a": 1})
来源：http://fz.panjiajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://uw.jctech888.com.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bu.shtwfgs.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dw.9csxet.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://pd.muxihuayi.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wa.newstarts.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ed.shxzukj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://vo.shxzukj.cn

[L03] 设置自定义请求头
来源：http://eu.yuexingan06.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ww.521024.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://be.panjiajie.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rq.asd995.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xg.nicolike.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://yc.huixinmuqiang.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ib.huixiangedu.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://lz.colortex.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://zp.jianghongdianzi.cn

[L04] 设置超时
来源：http://xq.shxzukj.cn

Py:   requests.get(url, timeout=5)
来源：http://xl.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://cb.colortex.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qa.haigaiapp.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zx.521024.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://gj.9csxet.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://sr.shxzskj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://se.shxzukj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://dl.newstarts.cn

[L05] 上传文件（multipart）
来源：http://hb.chemitech.net.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://qt.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ma.jianghongdianzi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://yt.szxytkj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mr.newstarts.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://xl.yuntaijiaju.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://df.yuntaijiaju.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://uc.yuexingan06.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ay.asd995.cn

[L06] 解析响应为 JSON
来源：http://kn.9csxet.cn

Py:   resp.json()
来源：http://bp.bjjhwx.cn

PHP:  json_decode($body, true);
来源：http://ai.hahajie.cn

JS:   await resp.json()
来源：http://fv.huixinmuqiang.cn

TS:   await resp.json()
来源：http://aq.bookmarksfly.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://aq.9csxet.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hq.nszjky.cn

Ruby: JSON.parse(resp.body)
来源：http://cu.colortex.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://im.muxihuayi.cn

[L07] 处理 HTTP 状态码
来源：http://ai.jctech888.com.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://vm.colortex.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://vi.jctech888.com.cn

JS:   resp.ok;  resp.status
来源：http://tv.colortex.cn

TS:   resp.ok;  resp.status
来源：http://mk.colortex.cn

Java: resp.statusCode()
来源：http://fp.9csxet.cn

Go:   resp.StatusCode
来源：http://nq.huanxung.cn

Ruby: resp.code.to_i
来源：http://zt.hnjuh.cn

C#:   (int)resp.StatusCode
来源：http://jv.huanxung.cn

[L08] 并发请求多个地址
来源：http://sh.hnjuh.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://kk.nicolike.cn

PHP:  curl_multi_init() 系列
来源：http://jd.wgjwhj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qt.haigaiapp.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ve.521024.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://jl.muxihuayi.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://as.nszjky.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://kz.jianghongdianzi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://bi.lnxyls.cn

================================================================================
来源：http://cs.huanxung.cn

M. 命令行 / 进程 / 环境
来源：http://pm.gzmigu.cn

================================================================================
来源：http://ad.huixinmuqiang.cn

[M01] 读取命令行参数
来源：http://fb.9csxet.cn

Py:   sys.argv[1:]
来源：http://so.hnjuh.cn

PHP:  $argv;  $argc;
来源：http://fr.shtwfgs.cn

JS:   process.argv.slice(2)
来源：http://de.huanxung.cn

TS:   process.argv.slice(2)
来源：http://pd.shtwfgs.cn

Java: args 数组（main 方法参数）
来源：http://aq.shxzukj.cn

Go:   os.Args[1:]
来源：http://vh.jianghongdianzi.cn

Ruby: ARGV
来源：http://nd.chemitech.net.cn

C#:   args 数组（Main 方法参数）
来源：http://hd.yuexingan06.cn

[M02] 读取环境变量
来源：http://pu.szxytkj.cn

Py:   os.environ.get("HOME")
来源：http://wl.newstarts.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hv.colortex.cn

JS:   process.env.HOME
来源：http://wh.shxzukj.cn

TS:   process.env.HOME
来源：http://xq.bjjhwx.cn

Java: System.getenv("HOME")
来源：http://ii.huixinmuqiang.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://qd.yuntaijiaju.cn

Ruby: ENV["HOME"]
来源：http://rz.521024.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://xo.newstarts.cn

[M03] 执行外部命令
来源：http://xm.huanxung.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hs.bjjhwx.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://gs.shtwfgs.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://cq.haigaiapp.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://tr.asd995.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://bq.jianghongdianzi.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://pc.shxzukj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ks.shtwfgs.cn

C#:   Process.Start("ls", "-l");
来源：http://bd.shtwfgs.cn

[M04] 获取当前工作目录
来源：http://mx.wgjwhj.cn

Py:   os.getcwd()
来源：http://bf.huanxung.cn

PHP:  getcwd();
来源：http://dx.hahajie.cn

JS:   process.cwd()
来源：http://xb.shtwfgs.cn

TS:   process.cwd()
来源：http://fi.wgjwhj.cn

Java: Path.of("").toAbsolutePath()
来源：http://kx.szsharing.cn

Go:   os.Getwd()
来源：http://zq.nszjky.cn

Ruby: Dir.pwd
来源：http://al.jianghongdianzi.cn

C#:   Directory.GetCurrentDirectory()
来源：http://vd.wgjwhj.cn

[M05] 设置退出码
来源：http://bm.521024.cn

Py:   sys.exit(1)
来源：http://gs.asd995.cn

PHP:  exit(1);
来源：http://te.nicolike.cn

JS:   process.exit(1)
来源：http://cf.colortex.cn

TS:   process.exit(1)
来源：http://tp.panjiajie.cn

Java: System.exit(1)
来源：http://mj.wgjwhj.cn

Go:   os.Exit(1)
来源：http://ap.bjjhwx.cn

Ruby: exit 1
来源：http://ei.huixiangedu.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://zl.lnxyls.cn

[M06] 向标准错误输出
来源：http://jl.yuntaijiaju.cn

Py:   print("err", file=sys.stderr)
来源：http://jk.yuexingan06.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ff.shxzskj.cn

JS:   console.error("err")
来源：http://aq.shtwfgs.cn

TS:   console.error("err")
来源：http://yc.colortex.cn

Java: System.err.println("err")
来源：http://ck.nszjky.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://sa.muxihuayi.cn

Ruby: warn "err"
来源：http://eb.nszjky.cn

C#:   Console.Error.WriteLine("err")
来源：http://kq.gzmigu.cn

[M07] 判断是否为主入口
来源：http://vy.yuntaijiaju.cn

Py:   if __name__ == "__main__":
来源：http://jc.asd995.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wo.newstarts.cn

JS:   require.main === module
来源：http://sa.colortex.cn

TS:   require.main === module
来源：http://lp.haigaiapp.cn

Java: public static void main(String[] args)
来源：http://og.shxzukj.cn

Go:   func main()
来源：http://nz.nicolike.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://pu.haigaiapp.cn

C#:   static void Main(string[] args)
来源：http://hj.huixiangedu.cn

[M08] 获取系统与运行时信息
来源：http://tn.wgjwhj.cn

Py:   platform.system();  platform.python_version()
来源：http://je.huanxung.cn

PHP:  PHP_OS;  phpversion();
来源：http://ma.huixiangedu.cn

JS:   process.platform;  process.version
来源：http://xo.haigaiapp.cn

TS:   process.platform;  process.version
来源：http://up.newstarts.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ro.shxzukj.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ds.bjjhwx.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ro.shtwfgs.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://zp.gzmigu.cn

================================================================================
来源：http://jz.haigaiapp.cn

N. 数据结构与算法
来源：http://bx.jianghongdianzi.cn

================================================================================
来源：http://vd.yuexingan06.cn

[N01] 二分查找（有序数组）
来源：http://nd.asd995.cn

Py:   bisect.bisect_left(arr, x)
来源：http://oq.shxzskj.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://yo.hnjuh.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://da.gzmigu.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zy.haigaiapp.cn

Java: Arrays.binarySearch(arr, x)
来源：http://np.shtwfgs.cn

Go:   sort.SearchInts(arr, x)
来源：http://di.bookmarksfly.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://jj.chemitech.net.cn

C#:   Array.BinarySearch(arr, x)
来源：http://tl.bjjhwx.cn

[N02] 排序（工程实践用内置实现）
来源：http://ad.nszjky.cn

Py:   sorted(arr);  arr.sort()
来源：http://cv.huixinmuqiang.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://za.9csxet.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://am.wgjwhj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://jv.gzmigu.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://bg.521024.cn

Go:   slices.Sort(arr)
来源：http://bu.szsharing.cn

Ruby: arr.sort
来源：http://lr.hahajie.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://xu.gzmigu.cn

[N03] 快速排序（分治示例）
来源：http://nb.yuexingan06.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://jl.yuexingan06.cn

PHP:  // 递归实现，或用 usort
来源：http://wj.bookmarksfly.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zg.shxzukj.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bn.gzmigu.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ih.colortex.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ys.chemitech.net.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ku.huixiangedu.cn

C#:   // 手写递归，或 Array.Sort
来源：http://cy.huanxung.cn

[N04] 斐波那契数列
来源：http://uu.huanxung.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://xc.bjjhwx.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://dh.hnjuh.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wh.huixiangedu.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mm.shtwfgs.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ji.gzmigu.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ac.bjjhwx.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ko.panjiajie.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ue.hahajie.cn

[N05] 最大公约数
来源：http://ro.chemitech.net.cn

Py:   math.gcd(a, b)
来源：http://mm.haigaiapp.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://az.jctech888.com.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://as.huixiangedu.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ib.szsharing.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://oa.hnjuh.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hy.shxzukj.cn

Ruby: a.gcd(b)
来源：http://cq.yuexingan06.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hj.shxzukj.cn

[N06] 判断回文字符串
来源：http://nj.huixinmuqiang.cn

Py:   s == s[::-1]
来源：http://cd.lnxyls.cn

PHP:  $s === strrev($s);
来源：http://hb.hahajie.cn

JS:   s === [...s].reverse().join("")
来源：http://mz.huixiangedu.cn

TS:   s === [...s].reverse().join("")
来源：http://kj.newstarts.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://vm.chemitech.net.cn

Go:   // 双指针从两端比较
来源：http://nu.hahajie.cn

Ruby: s == s.reverse
来源：http://he.521024.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ng.gzmigu.cn

[N07] 两数之和（返回下标）
来源：http://hx.szxytkj.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://xi.lnxyls.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jb.colortex.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ds.nicolike.cn

TS:   // 手写 Map<string, number>
来源：http://ew.gzmigu.cn

Java: // 手写 HashMap
来源：http://mr.jctech888.com.cn

Go:   // 手写 map[int]int
来源：http://iw.newstarts.cn

Ruby: // 手写 Hash
来源：http://in.newstarts.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ih.nicolike.cn

[N08] 生成全排列
来源：http://wo.chemitech.net.cn

Py:   itertools.permutations(arr)
来源：http://lv.wgjwhj.cn

PHP:  // 手写递归交换
来源：http://pi.9csxet.cn

JS:   // 手写回溯递归
来源：http://tg.shxzukj.cn

TS:   // 手写回溯递归
来源：http://jz.shxzskj.cn

Java: // 手写回溯递归
来源：http://lk.shxzskj.cn

Go:   // 手写回溯递归
来源：http://ez.huanxung.cn

Ruby: arr.permutation.to_a
来源：http://vf.nicolike.cn

C#:   // 手写回溯递归
来源：http://sr.szsharing.cn

[N09] 栈与队列
来源：http://ei.yuexingan06.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://km.jctech888.com.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://bh.panjiajie.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ly.szxytkj.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://cd.521024.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ms.shxzskj.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://rg.szsharing.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://rp.bookmarksfly.cn


<!-- 参考信息 -->