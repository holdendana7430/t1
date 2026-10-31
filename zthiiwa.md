代发 wailian999

[K02] JSON 字符串转对象
来源：http://qg.panjiajie.cn

Py:   json.loads(s)
来源：http://sc.colortex.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://sp.hnjuh.cn

JS:   JSON.parse(s)
来源：http://ix.jctech888.com.cn

TS:   JSON.parse(s)
来源：http://qh.newstarts.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ca.haigaiapp.cn

Go:   json.Unmarshal(data, &v)
来源：http://lq.chemitech.net.cn

Ruby: JSON.parse(s)
来源：http://nn.lnxyls.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ev.chemitech.net.cn

[K03] JSON 美化输出（带缩进）
来源：http://nd.shtwfgs.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://vo.wgjwhj.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://fo.shtwfgs.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://jv.huixiangedu.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ur.hahajie.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://zc.9csxet.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wx.521024.cn

Ruby: JSON.pretty_generate(obj)
来源：http://bt.chemitech.net.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://na.yuexingan06.cn

[K04] 读取 JSON 文件
来源：http://mz.colortex.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ee.chemitech.net.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://yz.gzmigu.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rh.yuexingan06.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://oq.hnjuh.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://az.shxzukj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hu.521024.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://gg.haigaiapp.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://vo.szxytkj.cn

[K05] 深拷贝对象
来源：http://me.lnxyls.cn

Py:   copy.deepcopy(obj)
来源：http://gy.yuntaijiaju.cn

PHP:  unserialize(serialize($obj));
来源：http://st.nszjky.cn

JS:   structuredClone(obj)
来源：http://gb.szxytkj.cn

TS:   structuredClone(obj)
来源：http://ed.shxzskj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://dd.wgjwhj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://na.huanxung.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zp.colortex.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://dv.asd995.cn

[K06] 解析 URL 查询串
来源：http://hj.shtwfgs.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://di.bookmarksfly.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://dm.chemitech.net.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wq.bjjhwx.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lj.szsharing.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://nn.shtwfgs.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ps.hnjuh.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://lw.9csxet.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://bk.bjjhwx.cn

[K07] 进制转换
来源：http://gq.wgjwhj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ij.panjiajie.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://np.gzmigu.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://tc.panjiajie.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://cm.panjiajie.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://si.colortex.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ws.szxytkj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://uv.haigaiapp.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://an.haigaiapp.cn

[K08] 二进制序列化（非 JSON）
来源：http://te.jctech888.com.cn

Py:   pickle.dumps(obj)
来源：http://sb.wgjwhj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://rk.hnjuh.cn

JS:   v8.serialize(obj)        // Node
来源：http://oq.jctech888.com.cn

TS:   v8.serialize(obj)        // Node
来源：http://yp.shxzskj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://xb.yuntaijiaju.cn

Go:   encoding/gob
来源：http://ms.521024.cn

Ruby: Marshal.dump(obj)
来源：http://mp.shxzukj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://na.bookmarksfly.cn

================================================================================
来源：http://vi.nszjky.cn

L. 网络请求
来源：http://xw.nicolike.cn

================================================================================
来源：http://pq.gzmigu.cn

[L01] 发送 GET 请求
来源：http://wr.muxihuayi.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://pd.bjjhwx.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vm.muxihuayi.cn

JS:   await fetch(url)
来源：http://ah.szxytkj.cn

TS:   await fetch(url)
来源：http://fy.gzmigu.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://na.colortex.cn

Go:   resp, err := http.Get(url)
来源：http://kr.shtwfgs.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://wo.yuntaijiaju.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://rx.newstarts.cn

[L02] 发送 POST JSON
来源：http://no.huixinmuqiang.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ez.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qu.shxzukj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pg.521024.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mw.huixinmuqiang.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ca.gzmigu.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://nk.newstarts.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://bz.hahajie.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ft.asd995.cn

[L03] 设置自定义请求头
来源：http://jv.nicolike.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://vd.nicolike.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://rn.lnxyls.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qd.521024.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fm.wgjwhj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://sm.szsharing.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://kq.huixinmuqiang.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://si.muxihuayi.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://dj.jctech888.com.cn

[L04] 设置超时
来源：http://us.huanxung.cn

Py:   requests.get(url, timeout=5)
来源：http://tr.panjiajie.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://og.wgjwhj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jr.huixinmuqiang.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dh.521024.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://cv.muxihuayi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://zw.huixinmuqiang.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://bg.shxzukj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://lz.szxytkj.cn

[L05] 上传文件（multipart）
来源：http://uo.jctech888.com.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://va.panjiajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://vr.yuexingan06.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://xy.wgjwhj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://bl.szsharing.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://kq.gzmigu.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://of.chemitech.net.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://yd.nicolike.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://cf.muxihuayi.cn

[L06] 解析响应为 JSON
来源：http://ic.muxihuayi.cn

Py:   resp.json()
来源：http://bf.yuntaijiaju.cn

PHP:  json_decode($body, true);
来源：http://fs.bookmarksfly.cn

JS:   await resp.json()
来源：http://kn.wgjwhj.cn

TS:   await resp.json()
来源：http://tq.yuntaijiaju.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://uf.newstarts.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://dx.hnjuh.cn

Ruby: JSON.parse(resp.body)
来源：http://py.wgjwhj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://nx.bjjhwx.cn

[L07] 处理 HTTP 状态码
来源：http://ow.shtwfgs.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://am.asd995.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://sw.521024.cn

JS:   resp.ok;  resp.status
来源：http://wm.huixiangedu.cn

TS:   resp.ok;  resp.status
来源：http://ja.jctech888.com.cn

Java: resp.statusCode()
来源：http://ms.521024.cn

Go:   resp.StatusCode
来源：http://qp.haigaiapp.cn

Ruby: resp.code.to_i
来源：http://lk.bookmarksfly.cn

C#:   (int)resp.StatusCode
来源：http://xi.yuntaijiaju.cn

[L08] 并发请求多个地址
来源：http://ab.haigaiapp.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://yg.chemitech.net.cn

PHP:  curl_multi_init() 系列
来源：http://gl.haigaiapp.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rb.hahajie.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wn.bookmarksfly.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://nh.jianghongdianzi.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wi.shxzskj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://id.huixinmuqiang.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://vv.jctech888.com.cn

================================================================================
来源：http://ox.hnjuh.cn

M. 命令行 / 进程 / 环境
来源：http://fz.nicolike.cn

================================================================================
来源：http://dk.gzmigu.cn

[M01] 读取命令行参数
来源：http://kn.gzmigu.cn

Py:   sys.argv[1:]
来源：http://df.shxzukj.cn

PHP:  $argv;  $argc;
来源：http://lf.haigaiapp.cn

JS:   process.argv.slice(2)
来源：http://qm.hnjuh.cn

TS:   process.argv.slice(2)
来源：http://rr.yuntaijiaju.cn

Java: args 数组（main 方法参数）
来源：http://ht.shxzukj.cn

Go:   os.Args[1:]
来源：http://ln.asd995.cn

Ruby: ARGV
来源：http://km.szxytkj.cn

C#:   args 数组（Main 方法参数）
来源：http://am.haigaiapp.cn

[M02] 读取环境变量
来源：http://cc.shxzukj.cn

Py:   os.environ.get("HOME")
来源：http://nf.newstarts.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://iq.521024.cn

JS:   process.env.HOME
来源：http://ga.muxihuayi.cn

TS:   process.env.HOME
来源：http://fe.yuntaijiaju.cn

Java: System.getenv("HOME")
来源：http://mo.haigaiapp.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://kw.bjjhwx.cn

Ruby: ENV["HOME"]
来源：http://aa.shxzukj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ev.bjjhwx.cn

[M03] 执行外部命令
来源：http://nx.shtwfgs.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mi.haigaiapp.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://pa.lnxyls.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://vc.521024.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://hl.szsharing.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mv.shxzukj.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://oj.asd995.cn

Ruby: system("ls -l");  `ls -l`
来源：http://fb.bookmarksfly.cn

C#:   Process.Start("ls", "-l");
来源：http://vc.shtwfgs.cn

[M04] 获取当前工作目录
来源：http://wo.haigaiapp.cn

Py:   os.getcwd()
来源：http://yr.szxytkj.cn

PHP:  getcwd();
来源：http://qv.szsharing.cn

JS:   process.cwd()
来源：http://kz.muxihuayi.cn

TS:   process.cwd()
来源：http://xy.szxytkj.cn

Java: Path.of("").toAbsolutePath()
来源：http://au.shtwfgs.cn

Go:   os.Getwd()
来源：http://ux.asd995.cn

Ruby: Dir.pwd
来源：http://ob.bjjhwx.cn

C#:   Directory.GetCurrentDirectory()
来源：http://go.huixiangedu.cn

[M05] 设置退出码
来源：http://vg.521024.cn

Py:   sys.exit(1)
来源：http://ov.jianghongdianzi.cn

PHP:  exit(1);
来源：http://jr.gzmigu.cn

JS:   process.exit(1)
来源：http://zf.szxytkj.cn

TS:   process.exit(1)
来源：http://wv.shxzukj.cn

Java: System.exit(1)
来源：http://pi.asd995.cn

Go:   os.Exit(1)
来源：http://ts.shxzskj.cn

Ruby: exit 1
来源：http://av.huanxung.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mx.haigaiapp.cn

[M06] 向标准错误输出
来源：http://jy.bjjhwx.cn

Py:   print("err", file=sys.stderr)
来源：http://ai.hnjuh.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://nn.nicolike.cn

JS:   console.error("err")
来源：http://um.colortex.cn

TS:   console.error("err")
来源：http://ie.521024.cn

Java: System.err.println("err")
来源：http://no.9csxet.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wm.521024.cn

Ruby: warn "err"
来源：http://bt.9csxet.cn

C#:   Console.Error.WriteLine("err")
来源：http://cm.chemitech.net.cn

[M07] 判断是否为主入口
来源：http://zu.gzmigu.cn

Py:   if __name__ == "__main__":
来源：http://uk.chemitech.net.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://pb.shxzukj.cn

JS:   require.main === module
来源：http://ub.colortex.cn

TS:   require.main === module
来源：http://bp.nicolike.cn

Java: public static void main(String[] args)
来源：http://ek.521024.cn

Go:   func main()
来源：http://jm.haigaiapp.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://dc.9csxet.cn

C#:   static void Main(string[] args)
来源：http://wn.huanxung.cn

[M08] 获取系统与运行时信息
来源：http://rz.shtwfgs.cn

Py:   platform.system();  platform.python_version()
来源：http://jw.nszjky.cn

PHP:  PHP_OS;  phpversion();
来源：http://an.9csxet.cn

JS:   process.platform;  process.version
来源：http://fv.shxzskj.cn

TS:   process.platform;  process.version
来源：http://jc.jianghongdianzi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ws.hnjuh.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://gg.chemitech.net.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://pj.9csxet.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://bq.gzmigu.cn

================================================================================
来源：http://lw.szxytkj.cn

N. 数据结构与算法
来源：http://ux.hahajie.cn

================================================================================
来源：http://yh.yuntaijiaju.cn

[N01] 二分查找（有序数组）
来源：http://xo.huixiangedu.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ca.shtwfgs.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://xo.huixiangedu.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lb.panjiajie.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xl.hahajie.cn

Java: Arrays.binarySearch(arr, x)
来源：http://oz.shxzskj.cn

Go:   sort.SearchInts(arr, x)
来源：http://ov.9csxet.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://tq.nicolike.cn

C#:   Array.BinarySearch(arr, x)
来源：http://uc.szsharing.cn

[N02] 排序（工程实践用内置实现）
来源：http://kg.szxytkj.cn

Py:   sorted(arr);  arr.sort()
来源：http://vs.521024.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://fm.jctech888.com.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://wh.nszjky.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://rf.huanxung.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://by.bookmarksfly.cn

Go:   slices.Sort(arr)
来源：http://sz.jctech888.com.cn

Ruby: arr.sort
来源：http://ac.bookmarksfly.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://mv.shxzskj.cn

[N03] 快速排序（分治示例）
来源：http://rk.shtwfgs.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://vc.szsharing.cn

PHP:  // 递归实现，或用 usort
来源：http://wm.bookmarksfly.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zo.jctech888.com.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://up.chemitech.net.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://pd.chemitech.net.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ln.gzmigu.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mq.muxihuayi.cn

C#:   // 手写递归，或 Array.Sort
来源：http://aq.lnxyls.cn

[N04] 斐波那契数列
来源：http://rw.yuntaijiaju.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://db.521024.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://gm.bjjhwx.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kh.huanxung.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://td.nicolike.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://bd.asd995.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ui.yuntaijiaju.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ao.szxytkj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ld.jianghongdianzi.cn

[N05] 最大公约数
来源：http://aa.szsharing.cn

Py:   math.gcd(a, b)
来源：http://gi.haigaiapp.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://az.gzmigu.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ho.panjiajie.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mg.haigaiapp.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://dd.panjiajie.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://tw.nszjky.cn

Ruby: a.gcd(b)
来源：http://re.newstarts.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://lt.huixiangedu.cn

[N06] 判断回文字符串
来源：http://bm.wgjwhj.cn

Py:   s == s[::-1]
来源：http://uc.hahajie.cn

PHP:  $s === strrev($s);
来源：http://ig.haigaiapp.cn

JS:   s === [...s].reverse().join("")
来源：http://nu.muxihuayi.cn

TS:   s === [...s].reverse().join("")
来源：http://es.lnxyls.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://of.panjiajie.cn

Go:   // 双指针从两端比较
来源：http://ev.colortex.cn

Ruby: s == s.reverse
来源：http://yp.jctech888.com.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://xt.9csxet.cn

[N07] 两数之和（返回下标）
来源：http://vn.panjiajie.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://lh.yuntaijiaju.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://gv.yuntaijiaju.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://zo.jianghongdianzi.cn

TS:   // 手写 Map<string, number>
来源：http://dv.nszjky.cn

Java: // 手写 HashMap
来源：http://rr.bjjhwx.cn

Go:   // 手写 map[int]int
来源：http://zz.bjjhwx.cn

Ruby: // 手写 Hash
来源：http://pt.chemitech.net.cn

C#:   // 手写 Dictionary<int, int>
来源：http://wu.yuexingan06.cn

[N08] 生成全排列
来源：http://nu.muxihuayi.cn

Py:   itertools.permutations(arr)
来源：http://rs.521024.cn

PHP:  // 手写递归交换
来源：http://qd.521024.cn

JS:   // 手写回溯递归
来源：http://fs.521024.cn

TS:   // 手写回溯递归
来源：http://gr.huixiangedu.cn

Java: // 手写回溯递归
来源：http://rr.muxihuayi.cn

Go:   // 手写回溯递归
来源：http://xu.asd995.cn

Ruby: arr.permutation.to_a
来源：http://fh.gzmigu.cn

C#:   // 手写回溯递归
来源：http://su.szsharing.cn

[N09] 栈与队列
来源：http://mh.szxytkj.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://gi.shtwfgs.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://dm.jianghongdianzi.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://oe.bjjhwx.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://lp.chemitech.net.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://tf.yuntaijiaju.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://zh.shtwfgs.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://cq.huanxung.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hf.shxzukj.cn

[N10] 链表节点定义
来源：http://tg.lnxyls.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://rk.chemitech.net.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://of.asd995.cn


<!-- 参考信息 -->