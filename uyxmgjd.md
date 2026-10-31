代发 wailian999

[K02] JSON 字符串转对象
来源：http://gc.shxzskj.cn

Py:   json.loads(s)
来源：http://sz.bjjhwx.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ho.nicolike.cn

JS:   JSON.parse(s)
来源：http://nc.lnxyls.cn

TS:   JSON.parse(s)
来源：http://ur.chemitech.net.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vs.bjjhwx.cn

Go:   json.Unmarshal(data, &v)
来源：http://az.yuexingan06.cn

Ruby: JSON.parse(s)
来源：http://oe.panjiajie.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://nk.szxytkj.cn

[K03] JSON 美化输出（带缩进）
来源：http://hh.szxytkj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ih.asd995.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ci.huanxung.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://fm.huixiangedu.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://kc.wgjwhj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://iw.hahajie.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hy.muxihuayi.cn

Ruby: JSON.pretty_generate(obj)
来源：http://jc.shxzukj.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://yt.colortex.cn

[K04] 读取 JSON 文件
来源：http://zp.521024.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jl.huanxung.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://to.shxzskj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ai.huixinmuqiang.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ac.jianghongdianzi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://fo.huixiangedu.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://kp.asd995.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://td.shxzukj.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wz.panjiajie.cn

[K05] 深拷贝对象
来源：http://zz.521024.cn

Py:   copy.deepcopy(obj)
来源：http://ll.asd995.cn

PHP:  unserialize(serialize($obj));
来源：http://ce.nszjky.cn

JS:   structuredClone(obj)
来源：http://ga.panjiajie.cn

TS:   structuredClone(obj)
来源：http://lk.lnxyls.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://hl.haigaiapp.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://pk.nicolike.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://dy.shtwfgs.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://sf.panjiajie.cn

[K06] 解析 URL 查询串
来源：http://ho.chemitech.net.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://fg.gzmigu.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://kq.huixiangedu.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uy.jianghongdianzi.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ol.lnxyls.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://sf.gzmigu.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://xi.bjjhwx.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vv.nszjky.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://pz.bookmarksfly.cn

[K07] 进制转换
来源：http://uq.jianghongdianzi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://lk.nszjky.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://nq.colortex.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ot.521024.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://cj.yuntaijiaju.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://nn.bookmarksfly.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://xi.521024.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://vg.chemitech.net.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://am.nszjky.cn

[K08] 二进制序列化（非 JSON）
来源：http://sl.panjiajie.cn

Py:   pickle.dumps(obj)
来源：http://ps.nszjky.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://vp.lnxyls.cn

JS:   v8.serialize(obj)        // Node
来源：http://yg.shxzskj.cn

TS:   v8.serialize(obj)        // Node
来源：http://jz.huixinmuqiang.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ps.haigaiapp.cn

Go:   encoding/gob
来源：http://xi.szxytkj.cn

Ruby: Marshal.dump(obj)
来源：http://qc.nszjky.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mr.lnxyls.cn

================================================================================
来源：http://ev.huixinmuqiang.cn

L. 网络请求
来源：http://up.yuntaijiaju.cn

================================================================================
来源：http://ph.chemitech.net.cn

[L01] 发送 GET 请求
来源：http://ad.jctech888.com.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ht.szsharing.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xk.yuexingan06.cn

JS:   await fetch(url)
来源：http://px.521024.cn

TS:   await fetch(url)
来源：http://oj.yuexingan06.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hs.hahajie.cn

Go:   resp, err := http.Get(url)
来源：http://yo.huixiangedu.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://cs.huanxung.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ro.newstarts.cn

[L02] 发送 POST JSON
来源：http://iv.bookmarksfly.cn

Py:   requests.post(url, json={"a": 1})
来源：http://sn.hnjuh.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://gr.shxzukj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://al.colortex.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vi.bjjhwx.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://uu.bjjhwx.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://vs.colortex.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ms.bookmarksfly.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://sp.bjjhwx.cn

[L03] 设置自定义请求头
来源：http://gt.jctech888.com.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://qy.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://dq.shxzskj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fl.asd995.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ff.szsharing.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mx.hnjuh.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ml.shxzskj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://cu.jctech888.com.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://vh.huixiangedu.cn

[L04] 设置超时
来源：http://pf.9csxet.cn

Py:   requests.get(url, timeout=5)
来源：http://gz.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://sv.gzmigu.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://od.muxihuayi.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hh.szxytkj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://bl.colortex.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://tz.colortex.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://rw.szxytkj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://aw.jianghongdianzi.cn

[L05] 上传文件（multipart）
来源：http://fg.colortex.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wc.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ah.hnjuh.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://jv.wgjwhj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://vs.gzmigu.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mx.shxzskj.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ce.jctech888.com.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://zz.colortex.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://yq.yuntaijiaju.cn

[L06] 解析响应为 JSON
来源：http://zn.nicolike.cn

Py:   resp.json()
来源：http://og.huanxung.cn

PHP:  json_decode($body, true);
来源：http://xi.bjjhwx.cn

JS:   await resp.json()
来源：http://tp.yuntaijiaju.cn

TS:   await resp.json()
来源：http://li.wgjwhj.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://tr.bjjhwx.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://rf.9csxet.cn

Ruby: JSON.parse(resp.body)
来源：http://tt.panjiajie.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ka.shxzskj.cn

[L07] 处理 HTTP 状态码
来源：http://xi.jctech888.com.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://zt.nicolike.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://zc.hahajie.cn

JS:   resp.ok;  resp.status
来源：http://gk.jianghongdianzi.cn

TS:   resp.ok;  resp.status
来源：http://am.lnxyls.cn

Java: resp.statusCode()
来源：http://gz.huixinmuqiang.cn

Go:   resp.StatusCode
来源：http://uy.gzmigu.cn

Ruby: resp.code.to_i
来源：http://og.jctech888.com.cn

C#:   (int)resp.StatusCode
来源：http://wu.colortex.cn

[L08] 并发请求多个地址
来源：http://si.yuexingan06.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://qu.szsharing.cn

PHP:  curl_multi_init() 系列
来源：http://cl.colortex.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://on.szxytkj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yj.yuntaijiaju.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://xd.9csxet.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qq.asd995.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zy.jianghongdianzi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ft.bjjhwx.cn

================================================================================
来源：http://ec.muxihuayi.cn

M. 命令行 / 进程 / 环境
来源：http://yj.hnjuh.cn

================================================================================
来源：http://ci.huixiangedu.cn

[M01] 读取命令行参数
来源：http://pr.9csxet.cn

Py:   sys.argv[1:]
来源：http://qo.huixinmuqiang.cn

PHP:  $argv;  $argc;
来源：http://zy.521024.cn

JS:   process.argv.slice(2)
来源：http://hs.shxzskj.cn

TS:   process.argv.slice(2)
来源：http://iu.9csxet.cn

Java: args 数组（main 方法参数）
来源：http://cj.shtwfgs.cn

Go:   os.Args[1:]
来源：http://zl.521024.cn

Ruby: ARGV
来源：http://ap.jianghongdianzi.cn

C#:   args 数组（Main 方法参数）
来源：http://xl.hnjuh.cn

[M02] 读取环境变量
来源：http://cd.newstarts.cn

Py:   os.environ.get("HOME")
来源：http://vr.yuexingan06.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://bz.nszjky.cn

JS:   process.env.HOME
来源：http://np.jianghongdianzi.cn

TS:   process.env.HOME
来源：http://cy.haigaiapp.cn

Java: System.getenv("HOME")
来源：http://zz.gzmigu.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://iw.newstarts.cn

Ruby: ENV["HOME"]
来源：http://hy.bookmarksfly.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://eq.huixiangedu.cn

[M03] 执行外部命令
来源：http://us.bjjhwx.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://zm.shxzskj.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://kd.bjjhwx.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://qo.shtwfgs.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://vw.huanxung.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://oa.chemitech.net.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://mc.chemitech.net.cn

Ruby: system("ls -l");  `ls -l`
来源：http://qu.9csxet.cn

C#:   Process.Start("ls", "-l");
来源：http://gm.panjiajie.cn

[M04] 获取当前工作目录
来源：http://yc.panjiajie.cn

Py:   os.getcwd()
来源：http://fs.szsharing.cn

PHP:  getcwd();
来源：http://el.huixiangedu.cn

JS:   process.cwd()
来源：http://sh.shxzskj.cn

TS:   process.cwd()
来源：http://vl.szsharing.cn

Java: Path.of("").toAbsolutePath()
来源：http://sb.bjjhwx.cn

Go:   os.Getwd()
来源：http://nc.shtwfgs.cn

Ruby: Dir.pwd
来源：http://be.huanxung.cn

C#:   Directory.GetCurrentDirectory()
来源：http://fe.asd995.cn

[M05] 设置退出码
来源：http://ib.bookmarksfly.cn

Py:   sys.exit(1)
来源：http://kv.bookmarksfly.cn

PHP:  exit(1);
来源：http://ez.gzmigu.cn

JS:   process.exit(1)
来源：http://di.huixiangedu.cn

TS:   process.exit(1)
来源：http://vw.jctech888.com.cn

Java: System.exit(1)
来源：http://vf.shxzukj.cn

Go:   os.Exit(1)
来源：http://qd.shxzukj.cn

Ruby: exit 1
来源：http://fd.szxytkj.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://vv.shtwfgs.cn

[M06] 向标准错误输出
来源：http://ys.yuexingan06.cn

Py:   print("err", file=sys.stderr)
来源：http://av.shxzskj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://la.yuntaijiaju.cn

JS:   console.error("err")
来源：http://ia.bookmarksfly.cn

TS:   console.error("err")
来源：http://wh.panjiajie.cn

Java: System.err.println("err")
来源：http://om.shtwfgs.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://zk.shxzukj.cn

Ruby: warn "err"
来源：http://iy.yuexingan06.cn

C#:   Console.Error.WriteLine("err")
来源：http://aq.huixiangedu.cn

[M07] 判断是否为主入口
来源：http://mq.shtwfgs.cn

Py:   if __name__ == "__main__":
来源：http://vf.newstarts.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://xi.huixiangedu.cn

JS:   require.main === module
来源：http://de.yuexingan06.cn

TS:   require.main === module
来源：http://po.gzmigu.cn

Java: public static void main(String[] args)
来源：http://ky.nszjky.cn

Go:   func main()
来源：http://uv.hnjuh.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://sw.hnjuh.cn

C#:   static void Main(string[] args)
来源：http://dm.yuexingan06.cn

[M08] 获取系统与运行时信息
来源：http://oc.nszjky.cn

Py:   platform.system();  platform.python_version()
来源：http://ho.panjiajie.cn

PHP:  PHP_OS;  phpversion();
来源：http://hq.bookmarksfly.cn

JS:   process.platform;  process.version
来源：http://ac.haigaiapp.cn

TS:   process.platform;  process.version
来源：http://lp.nicolike.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ax.gzmigu.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://yt.521024.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ou.lnxyls.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://tp.hnjuh.cn

================================================================================
来源：http://og.jianghongdianzi.cn

N. 数据结构与算法
来源：http://ne.shxzskj.cn

================================================================================
来源：http://rz.chemitech.net.cn

[N01] 二分查找（有序数组）
来源：http://qr.newstarts.cn

Py:   bisect.bisect_left(arr, x)
来源：http://eb.shxzskj.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://bv.nszjky.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vv.huixinmuqiang.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://au.huanxung.cn

Java: Arrays.binarySearch(arr, x)
来源：http://wt.szxytkj.cn

Go:   sort.SearchInts(arr, x)
来源：http://wt.panjiajie.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://cs.gzmigu.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ph.haigaiapp.cn

[N02] 排序（工程实践用内置实现）
来源：http://dc.jianghongdianzi.cn

Py:   sorted(arr);  arr.sort()
来源：http://ja.9csxet.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://po.muxihuayi.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ck.panjiajie.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://oo.wgjwhj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ps.huixinmuqiang.cn

Go:   slices.Sort(arr)
来源：http://tf.wgjwhj.cn

Ruby: arr.sort
来源：http://kj.hnjuh.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://wj.hnjuh.cn

[N03] 快速排序（分治示例）
来源：http://rn.yuntaijiaju.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://pc.9csxet.cn

PHP:  // 递归实现，或用 usort
来源：http://ck.hahajie.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://im.jctech888.com.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sv.hahajie.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://av.yuexingan06.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://us.huixiangedu.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://oe.shxzskj.cn

C#:   // 手写递归，或 Array.Sort
来源：http://cs.nicolike.cn

[N04] 斐波那契数列
来源：http://gy.hnjuh.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qc.wgjwhj.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://qn.colortex.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bk.hnjuh.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bo.chemitech.net.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://yr.muxihuayi.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://sf.newstarts.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://rh.nicolike.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://gf.nszjky.cn

[N05] 最大公约数
来源：http://nd.muxihuayi.cn

Py:   math.gcd(a, b)
来源：http://tl.szxytkj.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://up.asd995.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tr.hahajie.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://po.jianghongdianzi.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ce.9csxet.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://qj.huanxung.cn

Ruby: a.gcd(b)
来源：http://cg.lnxyls.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://eq.hnjuh.cn

[N06] 判断回文字符串
来源：http://dt.yuexingan06.cn

Py:   s == s[::-1]
来源：http://bl.haigaiapp.cn

PHP:  $s === strrev($s);
来源：http://yb.jianghongdianzi.cn

JS:   s === [...s].reverse().join("")
来源：http://pf.shtwfgs.cn

TS:   s === [...s].reverse().join("")
来源：http://fs.colortex.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xq.nicolike.cn

Go:   // 双指针从两端比较
来源：http://ux.asd995.cn

Ruby: s == s.reverse
来源：http://ft.gzmigu.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://me.hnjuh.cn

[N07] 两数之和（返回下标）
来源：http://xj.shxzskj.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://fa.9csxet.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ua.muxihuayi.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://om.huanxung.cn

TS:   // 手写 Map<string, number>
来源：http://uu.huixiangedu.cn

Java: // 手写 HashMap
来源：http://yx.asd995.cn

Go:   // 手写 map[int]int
来源：http://jb.hahajie.cn

Ruby: // 手写 Hash
来源：http://rn.newstarts.cn

C#:   // 手写 Dictionary<int, int>
来源：http://va.asd995.cn

[N08] 生成全排列
来源：http://ui.bjjhwx.cn

Py:   itertools.permutations(arr)
来源：http://wq.9csxet.cn

PHP:  // 手写递归交换
来源：http://qx.huixinmuqiang.cn

JS:   // 手写回溯递归
来源：http://nc.huanxung.cn

TS:   // 手写回溯递归
来源：http://er.shtwfgs.cn

Java: // 手写回溯递归
来源：http://tj.wgjwhj.cn

Go:   // 手写回溯递归
来源：http://qn.wgjwhj.cn

Ruby: arr.permutation.to_a
来源：http://jg.9csxet.cn

C#:   // 手写回溯递归
来源：http://vs.bookmarksfly.cn

[N09] 栈与队列
来源：http://kw.haigaiapp.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://cx.nszjky.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://uj.jctech888.com.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://up.shtwfgs.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://yd.jctech888.com.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://pg.shxzukj.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://fv.yuexingan06.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://gn.muxihuayi.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://sp.jianghongdianzi.cn

[N10] 链表节点定义
来源：http://ra.asd995.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mj.jianghongdianzi.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://tz.huixiangedu.cn


<!-- 参考信息 -->