代发 wailian999

[K02] JSON 字符串转对象
来源：http://rc.jctech888.com.cn

Py:   json.loads(s)
来源：http://cf.szsharing.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ja.chemitech.net.cn

JS:   JSON.parse(s)
来源：http://xl.nszjky.cn

TS:   JSON.parse(s)
来源：http://zc.nszjky.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wg.huixiangedu.cn

Go:   json.Unmarshal(data, &v)
来源：http://jg.huixinmuqiang.cn

Ruby: JSON.parse(s)
来源：http://oi.yuntaijiaju.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://tz.shtwfgs.cn

[K03] JSON 美化输出（带缩进）
来源：http://op.521024.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://kg.shxzskj.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://co.jianghongdianzi.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://qc.shtwfgs.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://pr.nicolike.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://tx.jctech888.com.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://cp.szxytkj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://xm.huanxung.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ul.lnxyls.cn

[K04] 读取 JSON 文件
来源：http://ga.szxytkj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://bv.muxihuayi.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://sq.bookmarksfly.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jy.hahajie.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nd.nicolike.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ju.shxzukj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://pm.nszjky.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://qs.521024.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://as.9csxet.cn

[K05] 深拷贝对象
来源：http://jr.lnxyls.cn

Py:   copy.deepcopy(obj)
来源：http://aj.szxytkj.cn

PHP:  unserialize(serialize($obj));
来源：http://xf.jctech888.com.cn

JS:   structuredClone(obj)
来源：http://jq.szsharing.cn

TS:   structuredClone(obj)
来源：http://fq.colortex.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://yk.shxzskj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://oo.panjiajie.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://nv.colortex.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://wq.521024.cn

[K06] 解析 URL 查询串
来源：http://ul.huixiangedu.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ek.bjjhwx.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mt.bjjhwx.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kf.yuntaijiaju.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://et.shtwfgs.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://pa.shxzukj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://wh.huanxung.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ls.hnjuh.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://sg.bjjhwx.cn

[K07] 进制转换
来源：http://jh.yuntaijiaju.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://un.jctech888.com.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://kd.hahajie.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://qi.shtwfgs.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://fe.hnjuh.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://yb.lnxyls.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ml.huanxung.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://pv.chemitech.net.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://pt.521024.cn

[K08] 二进制序列化（非 JSON）
来源：http://kt.huixinmuqiang.cn

Py:   pickle.dumps(obj)
来源：http://ob.jianghongdianzi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://lv.bookmarksfly.cn

JS:   v8.serialize(obj)        // Node
来源：http://zr.shtwfgs.cn

TS:   v8.serialize(obj)        // Node
来源：http://kn.panjiajie.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://gw.yuexingan06.cn

Go:   encoding/gob
来源：http://xp.haigaiapp.cn

Ruby: Marshal.dump(obj)
来源：http://pb.nicolike.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://cc.szxytkj.cn

================================================================================
来源：http://bv.huanxung.cn

L. 网络请求
来源：http://dn.bookmarksfly.cn

================================================================================
来源：http://th.huanxung.cn

[L01] 发送 GET 请求
来源：http://hp.nicolike.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://sw.yuexingan06.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xi.asd995.cn

JS:   await fetch(url)
来源：http://jz.bjjhwx.cn

TS:   await fetch(url)
来源：http://pt.nicolike.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://aw.chemitech.net.cn

Go:   resp, err := http.Get(url)
来源：http://vg.nszjky.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://nh.shxzskj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://tr.bookmarksfly.cn

[L02] 发送 POST JSON
来源：http://rq.shxzukj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ty.haigaiapp.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ov.jctech888.com.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gj.szxytkj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rd.shtwfgs.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ag.bookmarksfly.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://dd.newstarts.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://yt.shtwfgs.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wj.nszjky.cn

[L03] 设置自定义请求头
来源：http://gk.haigaiapp.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://qw.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ml.huanxung.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xh.shtwfgs.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vd.jctech888.com.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://xd.haigaiapp.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ai.muxihuayi.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://kz.haigaiapp.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://pl.lnxyls.cn

[L04] 设置超时
来源：http://dz.nszjky.cn

Py:   requests.get(url, timeout=5)
来源：http://ae.nszjky.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://jm.521024.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dh.bookmarksfly.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ux.yuexingan06.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://zo.asd995.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://av.bookmarksfly.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ak.gzmigu.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://zj.nicolike.cn

[L05] 上传文件（multipart）
来源：http://fr.chemitech.net.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mf.haigaiapp.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wi.hahajie.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gm.huixinmuqiang.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ek.asd995.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://qp.haigaiapp.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://yy.chemitech.net.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ns.newstarts.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ab.lnxyls.cn

[L06] 解析响应为 JSON
来源：http://ik.yuntaijiaju.cn

Py:   resp.json()
来源：http://tl.panjiajie.cn

PHP:  json_decode($body, true);
来源：http://wg.wgjwhj.cn

JS:   await resp.json()
来源：http://ka.huixinmuqiang.cn

TS:   await resp.json()
来源：http://dd.shxzskj.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://qy.shtwfgs.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wp.szsharing.cn

Ruby: JSON.parse(resp.body)
来源：http://en.shtwfgs.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://la.newstarts.cn

[L07] 处理 HTTP 状态码
来源：http://al.szxytkj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://by.shxzukj.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://rt.hahajie.cn

JS:   resp.ok;  resp.status
来源：http://gh.muxihuayi.cn

TS:   resp.ok;  resp.status
来源：http://xu.lnxyls.cn

Java: resp.statusCode()
来源：http://tg.hahajie.cn

Go:   resp.StatusCode
来源：http://qn.shtwfgs.cn

Ruby: resp.code.to_i
来源：http://iz.shxzukj.cn

C#:   (int)resp.StatusCode
来源：http://hs.9csxet.cn

[L08] 并发请求多个地址
来源：http://qk.jianghongdianzi.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://fb.yuntaijiaju.cn

PHP:  curl_multi_init() 系列
来源：http://qa.yuntaijiaju.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zq.shxzskj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sz.bookmarksfly.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://dd.jctech888.com.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ee.jctech888.com.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://op.bjjhwx.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://bs.newstarts.cn

================================================================================
来源：http://gv.colortex.cn

M. 命令行 / 进程 / 环境
来源：http://iq.yuntaijiaju.cn

================================================================================
来源：http://oe.szxytkj.cn

[M01] 读取命令行参数
来源：http://iv.gzmigu.cn

Py:   sys.argv[1:]
来源：http://yh.lnxyls.cn

PHP:  $argv;  $argc;
来源：http://jh.lnxyls.cn

JS:   process.argv.slice(2)
来源：http://tn.jianghongdianzi.cn

TS:   process.argv.slice(2)
来源：http://ky.asd995.cn

Java: args 数组（main 方法参数）
来源：http://rg.bjjhwx.cn

Go:   os.Args[1:]
来源：http://dz.nicolike.cn

Ruby: ARGV
来源：http://gk.szxytkj.cn

C#:   args 数组（Main 方法参数）
来源：http://gl.newstarts.cn

[M02] 读取环境变量
来源：http://cz.szsharing.cn

Py:   os.environ.get("HOME")
来源：http://sx.shxzukj.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://xf.huanxung.cn

JS:   process.env.HOME
来源：http://ao.521024.cn

TS:   process.env.HOME
来源：http://vg.shxzskj.cn

Java: System.getenv("HOME")
来源：http://sk.asd995.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://gl.szxytkj.cn

Ruby: ENV["HOME"]
来源：http://pq.hahajie.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://sa.gzmigu.cn

[M03] 执行外部命令
来源：http://pr.hahajie.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://dg.szsharing.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://fu.shxzukj.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://fv.shxzskj.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://xl.haigaiapp.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://rl.huixiangedu.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://yb.lnxyls.cn

Ruby: system("ls -l");  `ls -l`
来源：http://mi.jianghongdianzi.cn

C#:   Process.Start("ls", "-l");
来源：http://mg.huanxung.cn

[M04] 获取当前工作目录
来源：http://by.asd995.cn

Py:   os.getcwd()
来源：http://qq.shtwfgs.cn

PHP:  getcwd();
来源：http://gj.9csxet.cn

JS:   process.cwd()
来源：http://ww.panjiajie.cn

TS:   process.cwd()
来源：http://iv.bjjhwx.cn

Java: Path.of("").toAbsolutePath()
来源：http://ow.nszjky.cn

Go:   os.Getwd()
来源：http://mj.newstarts.cn

Ruby: Dir.pwd
来源：http://jc.huanxung.cn

C#:   Directory.GetCurrentDirectory()
来源：http://pv.szsharing.cn

[M05] 设置退出码
来源：http://ti.jctech888.com.cn

Py:   sys.exit(1)
来源：http://zk.nicolike.cn

PHP:  exit(1);
来源：http://ur.nicolike.cn

JS:   process.exit(1)
来源：http://kv.hnjuh.cn

TS:   process.exit(1)
来源：http://wo.muxihuayi.cn

Java: System.exit(1)
来源：http://sy.yuntaijiaju.cn

Go:   os.Exit(1)
来源：http://we.panjiajie.cn

Ruby: exit 1
来源：http://nx.muxihuayi.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ov.gzmigu.cn

[M06] 向标准错误输出
来源：http://cg.newstarts.cn

Py:   print("err", file=sys.stderr)
来源：http://jw.shxzskj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://wj.huanxung.cn

JS:   console.error("err")
来源：http://jj.panjiajie.cn

TS:   console.error("err")
来源：http://bb.panjiajie.cn

Java: System.err.println("err")
来源：http://iu.bookmarksfly.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://gn.nszjky.cn

Ruby: warn "err"
来源：http://or.yuexingan06.cn

C#:   Console.Error.WriteLine("err")
来源：http://oj.bookmarksfly.cn

[M07] 判断是否为主入口
来源：http://ed.lnxyls.cn

Py:   if __name__ == "__main__":
来源：http://bo.wgjwhj.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ux.asd995.cn

JS:   require.main === module
来源：http://ej.wgjwhj.cn

TS:   require.main === module
来源：http://gp.shxzskj.cn

Java: public static void main(String[] args)
来源：http://zs.lnxyls.cn

Go:   func main()
来源：http://yk.asd995.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://fr.bjjhwx.cn

C#:   static void Main(string[] args)
来源：http://ob.9csxet.cn

[M08] 获取系统与运行时信息
来源：http://pm.lnxyls.cn

Py:   platform.system();  platform.python_version()
来源：http://zi.yuntaijiaju.cn

PHP:  PHP_OS;  phpversion();
来源：http://hp.huixiangedu.cn

JS:   process.platform;  process.version
来源：http://lw.hnjuh.cn

TS:   process.platform;  process.version
来源：http://jn.shtwfgs.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://kk.haigaiapp.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://jz.nszjky.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://kh.newstarts.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://nj.colortex.cn

================================================================================
来源：http://yk.asd995.cn

N. 数据结构与算法
来源：http://qh.wgjwhj.cn

================================================================================
来源：http://nc.szxytkj.cn

[N01] 二分查找（有序数组）
来源：http://ti.gzmigu.cn

Py:   bisect.bisect_left(arr, x)
来源：http://li.lnxyls.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://le.bookmarksfly.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xk.szxytkj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vj.szsharing.cn

Java: Arrays.binarySearch(arr, x)
来源：http://yn.wgjwhj.cn

Go:   sort.SearchInts(arr, x)
来源：http://lf.huixiangedu.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ye.521024.cn

C#:   Array.BinarySearch(arr, x)
来源：http://kh.yuexingan06.cn

[N02] 排序（工程实践用内置实现）
来源：http://zd.gzmigu.cn

Py:   sorted(arr);  arr.sort()
来源：http://cm.szxytkj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ul.9csxet.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ua.hnjuh.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://yj.jctech888.com.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://dr.lnxyls.cn

Go:   slices.Sort(arr)
来源：http://jx.jianghongdianzi.cn

Ruby: arr.sort
来源：http://dx.szsharing.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ru.colortex.cn

[N03] 快速排序（分治示例）
来源：http://ro.shtwfgs.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://fl.muxihuayi.cn

PHP:  // 递归实现，或用 usort
来源：http://nr.shxzukj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kn.jctech888.com.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ld.shxzskj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ir.521024.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://uf.nszjky.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hg.bookmarksfly.cn

C#:   // 手写递归，或 Array.Sort
来源：http://fa.huanxung.cn

[N04] 斐波那契数列
来源：http://ie.bjjhwx.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ww.hnjuh.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ql.yuntaijiaju.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nf.asd995.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tp.gzmigu.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://vz.wgjwhj.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://zs.jianghongdianzi.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://nx.hnjuh.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://th.muxihuayi.cn

[N05] 最大公约数
来源：http://tw.huixiangedu.cn

Py:   math.gcd(a, b)
来源：http://zi.lnxyls.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wi.wgjwhj.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://if.huixinmuqiang.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://uf.hahajie.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://gq.szxytkj.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ia.huixiangedu.cn

Ruby: a.gcd(b)
来源：http://pl.asd995.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://jx.shxzskj.cn

[N06] 判断回文字符串
来源：http://kd.panjiajie.cn

Py:   s == s[::-1]
来源：http://hf.newstarts.cn

PHP:  $s === strrev($s);
来源：http://vr.nszjky.cn

JS:   s === [...s].reverse().join("")
来源：http://yi.shtwfgs.cn

TS:   s === [...s].reverse().join("")
来源：http://fe.hahajie.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hj.hnjuh.cn

Go:   // 双指针从两端比较
来源：http://kt.szxytkj.cn

Ruby: s == s.reverse
来源：http://av.jianghongdianzi.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://en.nicolike.cn

[N07] 两数之和（返回下标）
来源：http://eh.hahajie.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://jy.521024.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://bh.521024.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://zu.huanxung.cn

TS:   // 手写 Map<string, number>
来源：http://fi.lnxyls.cn

Java: // 手写 HashMap
来源：http://ny.haigaiapp.cn

Go:   // 手写 map[int]int
来源：http://uy.nicolike.cn

Ruby: // 手写 Hash
来源：http://px.szsharing.cn

C#:   // 手写 Dictionary<int, int>
来源：http://id.colortex.cn

[N08] 生成全排列
来源：http://ml.yuntaijiaju.cn

Py:   itertools.permutations(arr)
来源：http://eu.bjjhwx.cn

PHP:  // 手写递归交换
来源：http://sr.jianghongdianzi.cn

JS:   // 手写回溯递归
来源：http://jg.yuexingan06.cn

TS:   // 手写回溯递归
来源：http://mi.lnxyls.cn

Java: // 手写回溯递归
来源：http://gb.nicolike.cn

Go:   // 手写回溯递归
来源：http://xh.yuntaijiaju.cn

Ruby: arr.permutation.to_a
来源：http://kj.szxytkj.cn

C#:   // 手写回溯递归
来源：http://io.chemitech.net.cn

[N09] 栈与队列
来源：http://cp.bjjhwx.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://bp.haigaiapp.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wk.yuntaijiaju.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mr.panjiajie.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://fn.panjiajie.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ie.hnjuh.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://yk.jctech888.com.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://le.huixinmuqiang.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://io.lnxyls.cn

[N10] 链表节点定义
来源：http://gg.jctech888.com.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://dd.9csxet.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://jg.yuntaijiaju.cn


<!-- 参考信息 -->