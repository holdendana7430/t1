代发 wailian999

[K02] JSON 字符串转对象
来源：http://ra.huixiangedu.cn

Py:   json.loads(s)
来源：http://ex.asd995.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://da.huixinmuqiang.cn

JS:   JSON.parse(s)
来源：http://au.jctech888.com.cn

TS:   JSON.parse(s)
来源：http://xf.colortex.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qz.chemitech.net.cn

Go:   json.Unmarshal(data, &v)
来源：http://ne.nszjky.cn

Ruby: JSON.parse(s)
来源：http://uw.asd995.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://bd.jctech888.com.cn

[K03] JSON 美化输出（带缩进）
来源：http://nx.shtwfgs.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://di.colortex.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://rc.szsharing.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ip.nszjky.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://cx.szsharing.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://im.panjiajie.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://sh.panjiajie.cn

Ruby: JSON.pretty_generate(obj)
来源：http://nx.jctech888.com.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://xr.muxihuayi.cn

[K04] 读取 JSON 文件
来源：http://de.colortex.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ds.haigaiapp.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://kn.newstarts.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vy.521024.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zy.asd995.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://zy.huanxung.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://cb.huixinmuqiang.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://gc.bookmarksfly.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hi.nszjky.cn

[K05] 深拷贝对象
来源：http://uf.nicolike.cn

Py:   copy.deepcopy(obj)
来源：http://es.szsharing.cn

PHP:  unserialize(serialize($obj));
来源：http://je.muxihuayi.cn

JS:   structuredClone(obj)
来源：http://xi.shxzskj.cn

TS:   structuredClone(obj)
来源：http://rx.nicolike.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ud.bookmarksfly.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://un.huixiangedu.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://xg.jctech888.com.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://qq.jianghongdianzi.cn

[K06] 解析 URL 查询串
来源：http://pz.gzmigu.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rs.521024.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://vu.szsharing.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bp.nicolike.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zb.huixinmuqiang.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ls.haigaiapp.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://pb.haigaiapp.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ve.colortex.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ou.wgjwhj.cn

[K07] 进制转换
来源：http://hx.shtwfgs.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://bk.9csxet.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://tb.muxihuayi.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://fo.newstarts.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://df.bookmarksfly.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://bd.haigaiapp.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ay.huixinmuqiang.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://yy.nicolike.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ru.jctech888.com.cn

[K08] 二进制序列化（非 JSON）
来源：http://xv.shtwfgs.cn

Py:   pickle.dumps(obj)
来源：http://hw.szsharing.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://uc.gzmigu.cn

JS:   v8.serialize(obj)        // Node
来源：http://yv.gzmigu.cn

TS:   v8.serialize(obj)        // Node
来源：http://jb.shtwfgs.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://sy.nicolike.cn

Go:   encoding/gob
来源：http://kv.yuexingan06.cn

Ruby: Marshal.dump(obj)
来源：http://cj.bjjhwx.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://oi.yuntaijiaju.cn

================================================================================
来源：http://ul.haigaiapp.cn

L. 网络请求
来源：http://et.szxytkj.cn

================================================================================
来源：http://kc.shtwfgs.cn

[L01] 发送 GET 请求
来源：http://aj.huanxung.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jh.hahajie.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ag.shtwfgs.cn

JS:   await fetch(url)
来源：http://yh.9csxet.cn

TS:   await fetch(url)
来源：http://pj.huanxung.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://si.shtwfgs.cn

Go:   resp, err := http.Get(url)
来源：http://fm.newstarts.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://rv.9csxet.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://nx.bjjhwx.cn

[L02] 发送 POST JSON
来源：http://ig.muxihuayi.cn

Py:   requests.post(url, json={"a": 1})
来源：http://bl.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://tx.shxzskj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bf.szxytkj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rz.huixiangedu.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qs.shxzskj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://pn.asd995.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ni.nicolike.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://do.shxzskj.cn

[L03] 设置自定义请求头
来源：http://qk.yuexingan06.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://il.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ms.asd995.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nv.yuexingan06.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zf.haigaiapp.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://xb.wgjwhj.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://sk.lnxyls.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://uh.jctech888.com.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://qr.lnxyls.cn

[L04] 设置超时
来源：http://jj.panjiajie.cn

Py:   requests.get(url, timeout=5)
来源：http://po.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xo.huixiangedu.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mt.9csxet.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vv.nszjky.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ae.haigaiapp.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ef.shxzukj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://fg.huixiangedu.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ef.shxzukj.cn

[L05] 上传文件（multipart）
来源：http://tc.muxihuayi.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://iu.yuntaijiaju.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://xk.bookmarksfly.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://rm.huixinmuqiang.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://cq.bookmarksfly.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://tg.colortex.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mq.wgjwhj.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://tb.shtwfgs.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://jt.muxihuayi.cn

[L06] 解析响应为 JSON
来源：http://mr.huixinmuqiang.cn

Py:   resp.json()
来源：http://fj.huixinmuqiang.cn

PHP:  json_decode($body, true);
来源：http://wm.hnjuh.cn

JS:   await resp.json()
来源：http://fe.9csxet.cn

TS:   await resp.json()
来源：http://ep.hahajie.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://kx.shxzskj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ji.yuntaijiaju.cn

Ruby: JSON.parse(resp.body)
来源：http://fy.shxzukj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://na.shxzukj.cn

[L07] 处理 HTTP 状态码
来源：http://zv.hahajie.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://gt.nszjky.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mu.yuntaijiaju.cn

JS:   resp.ok;  resp.status
来源：http://et.panjiajie.cn

TS:   resp.ok;  resp.status
来源：http://pe.wgjwhj.cn

Java: resp.statusCode()
来源：http://mp.colortex.cn

Go:   resp.StatusCode
来源：http://pl.shtwfgs.cn

Ruby: resp.code.to_i
来源：http://bb.huanxung.cn

C#:   (int)resp.StatusCode
来源：http://hg.shxzukj.cn

[L08] 并发请求多个地址
来源：http://ga.gzmigu.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://yi.nszjky.cn

PHP:  curl_multi_init() 系列
来源：http://zs.bjjhwx.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qk.hnjuh.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fr.jctech888.com.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://im.newstarts.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://sr.panjiajie.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://uw.newstarts.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ov.jianghongdianzi.cn

================================================================================
来源：http://xb.bjjhwx.cn

M. 命令行 / 进程 / 环境
来源：http://uo.muxihuayi.cn

================================================================================
来源：http://xg.asd995.cn

[M01] 读取命令行参数
来源：http://sa.haigaiapp.cn

Py:   sys.argv[1:]
来源：http://tp.gzmigu.cn

PHP:  $argv;  $argc;
来源：http://ns.jianghongdianzi.cn

JS:   process.argv.slice(2)
来源：http://lb.shxzukj.cn

TS:   process.argv.slice(2)
来源：http://pw.jctech888.com.cn

Java: args 数组（main 方法参数）
来源：http://od.hnjuh.cn

Go:   os.Args[1:]
来源：http://bt.haigaiapp.cn

Ruby: ARGV
来源：http://yk.panjiajie.cn

C#:   args 数组（Main 方法参数）
来源：http://gd.szsharing.cn

[M02] 读取环境变量
来源：http://ff.huixinmuqiang.cn

Py:   os.environ.get("HOME")
来源：http://up.shtwfgs.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://at.lnxyls.cn

JS:   process.env.HOME
来源：http://kq.shxzukj.cn

TS:   process.env.HOME
来源：http://cr.shxzskj.cn

Java: System.getenv("HOME")
来源：http://ed.jianghongdianzi.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vb.9csxet.cn

Ruby: ENV["HOME"]
来源：http://wc.haigaiapp.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ol.bjjhwx.cn

[M03] 执行外部命令
来源：http://yv.colortex.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mx.hahajie.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://pl.szxytkj.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://lc.hnjuh.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://cb.hahajie.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://jt.panjiajie.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ds.panjiajie.cn

Ruby: system("ls -l");  `ls -l`
来源：http://gp.panjiajie.cn

C#:   Process.Start("ls", "-l");
来源：http://qp.szsharing.cn

[M04] 获取当前工作目录
来源：http://sz.521024.cn

Py:   os.getcwd()
来源：http://hv.huixinmuqiang.cn

PHP:  getcwd();
来源：http://cj.szsharing.cn

JS:   process.cwd()
来源：http://sr.jianghongdianzi.cn

TS:   process.cwd()
来源：http://cy.bookmarksfly.cn

Java: Path.of("").toAbsolutePath()
来源：http://al.yuntaijiaju.cn

Go:   os.Getwd()
来源：http://bb.521024.cn

Ruby: Dir.pwd
来源：http://tp.gzmigu.cn

C#:   Directory.GetCurrentDirectory()
来源：http://xb.521024.cn

[M05] 设置退出码
来源：http://es.huanxung.cn

Py:   sys.exit(1)
来源：http://zk.chemitech.net.cn

PHP:  exit(1);
来源：http://zn.wgjwhj.cn

JS:   process.exit(1)
来源：http://ht.jctech888.com.cn

TS:   process.exit(1)
来源：http://ml.shtwfgs.cn

Java: System.exit(1)
来源：http://wl.huixinmuqiang.cn

Go:   os.Exit(1)
来源：http://hm.gzmigu.cn

Ruby: exit 1
来源：http://pw.9csxet.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://th.gzmigu.cn

[M06] 向标准错误输出
来源：http://yc.asd995.cn

Py:   print("err", file=sys.stderr)
来源：http://wc.haigaiapp.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ul.newstarts.cn

JS:   console.error("err")
来源：http://xf.szsharing.cn

TS:   console.error("err")
来源：http://uj.muxihuayi.cn

Java: System.err.println("err")
来源：http://wi.jctech888.com.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://zk.nszjky.cn

Ruby: warn "err"
来源：http://to.yuexingan06.cn

C#:   Console.Error.WriteLine("err")
来源：http://vj.lnxyls.cn

[M07] 判断是否为主入口
来源：http://br.shxzskj.cn

Py:   if __name__ == "__main__":
来源：http://zf.huixinmuqiang.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://zl.chemitech.net.cn

JS:   require.main === module
来源：http://ty.wgjwhj.cn

TS:   require.main === module
来源：http://pj.panjiajie.cn

Java: public static void main(String[] args)
来源：http://gx.yuntaijiaju.cn

Go:   func main()
来源：http://rx.shxzukj.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://tf.yuntaijiaju.cn

C#:   static void Main(string[] args)
来源：http://ap.9csxet.cn

[M08] 获取系统与运行时信息
来源：http://dt.jctech888.com.cn

Py:   platform.system();  platform.python_version()
来源：http://nm.colortex.cn

PHP:  PHP_OS;  phpversion();
来源：http://qk.huixinmuqiang.cn

JS:   process.platform;  process.version
来源：http://ei.shxzskj.cn

TS:   process.platform;  process.version
来源：http://dw.wgjwhj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://bc.jctech888.com.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://xh.bjjhwx.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://jg.shxzukj.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://sq.huixiangedu.cn

================================================================================
来源：http://fz.muxihuayi.cn

N. 数据结构与算法
来源：http://vr.jianghongdianzi.cn

================================================================================
来源：http://zq.9csxet.cn

[N01] 二分查找（有序数组）
来源：http://yu.hahajie.cn

Py:   bisect.bisect_left(arr, x)
来源：http://gi.521024.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://pd.huixinmuqiang.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xh.newstarts.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wv.muxihuayi.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ut.nicolike.cn

Go:   sort.SearchInts(arr, x)
来源：http://sy.521024.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://xa.bjjhwx.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ek.lnxyls.cn

[N02] 排序（工程实践用内置实现）
来源：http://oz.yuexingan06.cn

Py:   sorted(arr);  arr.sort()
来源：http://tz.lnxyls.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://jh.jctech888.com.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://cu.gzmigu.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://cg.nszjky.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://yz.yuexingan06.cn

Go:   slices.Sort(arr)
来源：http://nw.bjjhwx.cn

Ruby: arr.sort
来源：http://gb.hnjuh.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ni.bookmarksfly.cn

[N03] 快速排序（分治示例）
来源：http://pa.jianghongdianzi.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://bz.shxzskj.cn

PHP:  // 递归实现，或用 usort
来源：http://bk.yuntaijiaju.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jj.asd995.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pg.gzmigu.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://kq.szsharing.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://qv.bookmarksfly.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://pl.9csxet.cn

C#:   // 手写递归，或 Array.Sort
来源：http://oq.shxzskj.cn

[N04] 斐波那契数列
来源：http://kp.shxzukj.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ic.jctech888.com.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://vm.gzmigu.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://if.jctech888.com.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kz.shxzukj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ck.yuntaijiaju.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://uk.yuntaijiaju.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://yl.newstarts.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ke.szxytkj.cn

[N05] 最大公约数
来源：http://qw.521024.cn

Py:   math.gcd(a, b)
来源：http://mk.gzmigu.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://og.bookmarksfly.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rw.huixinmuqiang.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ad.asd995.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ug.gzmigu.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://qw.nicolike.cn

Ruby: a.gcd(b)
来源：http://xp.lnxyls.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ek.521024.cn

[N06] 判断回文字符串
来源：http://vd.yuntaijiaju.cn

Py:   s == s[::-1]
来源：http://vm.nicolike.cn

PHP:  $s === strrev($s);
来源：http://ps.muxihuayi.cn

JS:   s === [...s].reverse().join("")
来源：http://ou.shtwfgs.cn

TS:   s === [...s].reverse().join("")
来源：http://be.newstarts.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://lx.hnjuh.cn

Go:   // 双指针从两端比较
来源：http://sg.9csxet.cn

Ruby: s == s.reverse
来源：http://nw.nszjky.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://bp.bookmarksfly.cn

[N07] 两数之和（返回下标）
来源：http://xf.huanxung.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ea.colortex.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ab.nszjky.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://es.chemitech.net.cn

TS:   // 手写 Map<string, number>
来源：http://sp.bjjhwx.cn

Java: // 手写 HashMap
来源：http://gu.newstarts.cn

Go:   // 手写 map[int]int
来源：http://cx.huixiangedu.cn

Ruby: // 手写 Hash
来源：http://pt.newstarts.cn

C#:   // 手写 Dictionary<int, int>
来源：http://oz.shxzskj.cn

[N08] 生成全排列
来源：http://vq.huixiangedu.cn

Py:   itertools.permutations(arr)
来源：http://jf.shxzskj.cn

PHP:  // 手写递归交换
来源：http://fh.yuntaijiaju.cn

JS:   // 手写回溯递归
来源：http://rf.jianghongdianzi.cn

TS:   // 手写回溯递归
来源：http://vu.szxytkj.cn

Java: // 手写回溯递归
来源：http://oe.shxzskj.cn

Go:   // 手写回溯递归
来源：http://ef.nszjky.cn

Ruby: arr.permutation.to_a
来源：http://is.colortex.cn

C#:   // 手写回溯递归
来源：http://yq.gzmigu.cn

[N09] 栈与队列
来源：http://me.newstarts.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://bi.bookmarksfly.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://sq.lnxyls.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://bu.muxihuayi.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://gh.asd995.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://rn.haigaiapp.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://qv.yuexingan06.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://kb.nicolike.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://gb.nicolike.cn

[N10] 链表节点定义
来源：http://rx.hnjuh.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://io.jianghongdianzi.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://nj.jctech888.com.cn


<!-- 参考信息 -->