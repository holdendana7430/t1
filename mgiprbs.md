代发 wailian999

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://sc.wgjwhj.cn

[K03] JSON 美化输出（带缩进）
来源：http://ik.muxihuayi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://gz.szxytkj.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://uo.9csxet.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://nm.szsharing.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://qb.yuexingan06.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://nx.huixiangedu.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://pp.hnjuh.cn

Ruby: JSON.pretty_generate(obj)
来源：http://qx.hahajie.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wz.szsharing.cn

[K04] 读取 JSON 文件
来源：http://uc.gzmigu.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ke.wgjwhj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://bd.hnjuh.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dd.asd995.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cl.shxzskj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hh.9csxet.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://gd.huixinmuqiang.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ln.521024.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://sn.wgjwhj.cn

[K05] 深拷贝对象
来源：http://ga.haigaiapp.cn

Py:   copy.deepcopy(obj)
来源：http://vh.huanxung.cn

PHP:  unserialize(serialize($obj));
来源：http://ts.nicolike.cn

JS:   structuredClone(obj)
来源：http://su.bookmarksfly.cn

TS:   structuredClone(obj)
来源：http://iz.jctech888.com.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://nw.huixinmuqiang.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://lu.wgjwhj.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://pu.hnjuh.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ym.haigaiapp.cn

[K06] 解析 URL 查询串
来源：http://ps.panjiajie.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://nf.521024.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wt.bookmarksfly.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pf.huanxung.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hr.szsharing.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://xn.hnjuh.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://wk.chemitech.net.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://om.szxytkj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://gn.hnjuh.cn

[K07] 进制转换
来源：http://ei.szxytkj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://di.shxzukj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://sa.hahajie.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://of.asd995.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://rk.bookmarksfly.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://sg.nszjky.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://fc.9csxet.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qo.bookmarksfly.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ff.nicolike.cn

[K08] 二进制序列化（非 JSON）
来源：http://dy.521024.cn

Py:   pickle.dumps(obj)
来源：http://lt.huanxung.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ed.haigaiapp.cn

JS:   v8.serialize(obj)        // Node
来源：http://kw.gzmigu.cn

TS:   v8.serialize(obj)        // Node
来源：http://of.haigaiapp.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://dj.newstarts.cn

Go:   encoding/gob
来源：http://ua.huixinmuqiang.cn

Ruby: Marshal.dump(obj)
来源：http://xj.colortex.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://oa.asd995.cn

================================================================================
来源：http://no.jianghongdianzi.cn

L. 网络请求
来源：http://fq.jianghongdianzi.cn

================================================================================
来源：http://ql.shxzukj.cn

[L01] 发送 GET 请求
来源：http://wq.szsharing.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://br.asd995.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ck.yuexingan06.cn

JS:   await fetch(url)
来源：http://up.asd995.cn

TS:   await fetch(url)
来源：http://vp.nicolike.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://fh.yuexingan06.cn

Go:   resp, err := http.Get(url)
来源：http://ng.huanxung.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://mw.huanxung.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://zl.haigaiapp.cn

[L02] 发送 POST JSON
来源：http://tn.hnjuh.cn

Py:   requests.post(url, json={"a": 1})
来源：http://yh.nicolike.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://rs.huanxung.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xy.shtwfgs.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://za.shtwfgs.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qw.shtwfgs.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://bl.shtwfgs.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://td.huanxung.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wc.bjjhwx.cn

[L03] 设置自定义请求头
来源：http://cc.9csxet.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://vr.szxytkj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://lv.huanxung.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qx.szsharing.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cl.shxzskj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://xn.hahajie.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://go.wgjwhj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wf.nszjky.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://in.szsharing.cn

[L04] 设置超时
来源：http://na.lnxyls.cn

Py:   requests.get(url, timeout=5)
来源：http://tp.huixiangedu.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xq.hahajie.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jj.chemitech.net.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mx.yuexingan06.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://xp.chemitech.net.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://js.newstarts.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wi.szxytkj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://dy.bookmarksfly.cn

[L05] 上传文件（multipart）
来源：http://wm.wgjwhj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://xy.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://zc.szxytkj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wy.huanxung.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://md.jianghongdianzi.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://lz.szsharing.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://gp.haigaiapp.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://rr.bookmarksfly.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wx.9csxet.cn

[L06] 解析响应为 JSON
来源：http://xv.jctech888.com.cn

Py:   resp.json()
来源：http://qo.gzmigu.cn

PHP:  json_decode($body, true);
来源：http://la.haigaiapp.cn

JS:   await resp.json()
来源：http://ic.colortex.cn

TS:   await resp.json()
来源：http://gl.chemitech.net.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://yy.lnxyls.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://fu.huixinmuqiang.cn

Ruby: JSON.parse(resp.body)
来源：http://ab.szsharing.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://bs.huixinmuqiang.cn

[L07] 处理 HTTP 状态码
来源：http://qk.nicolike.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://lk.jctech888.com.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://cn.huanxung.cn

JS:   resp.ok;  resp.status
来源：http://vx.shxzukj.cn

TS:   resp.ok;  resp.status
来源：http://ng.9csxet.cn

Java: resp.statusCode()
来源：http://yi.nicolike.cn

Go:   resp.StatusCode
来源：http://it.shxzskj.cn

Ruby: resp.code.to_i
来源：http://xg.9csxet.cn

C#:   (int)resp.StatusCode
来源：http://hr.huixinmuqiang.cn

[L08] 并发请求多个地址
来源：http://dw.bjjhwx.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://fq.gzmigu.cn

PHP:  curl_multi_init() 系列
来源：http://oj.wgjwhj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fe.lnxyls.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://un.szxytkj.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://jp.huixinmuqiang.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://nk.bjjhwx.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://xt.9csxet.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ui.nicolike.cn

================================================================================
来源：http://fy.chemitech.net.cn

M. 命令行 / 进程 / 环境
来源：http://vu.huixiangedu.cn

================================================================================
来源：http://bl.muxihuayi.cn

[M01] 读取命令行参数
来源：http://nt.nszjky.cn

Py:   sys.argv[1:]
来源：http://ed.chemitech.net.cn

PHP:  $argv;  $argc;
来源：http://yk.panjiajie.cn

JS:   process.argv.slice(2)
来源：http://as.colortex.cn

TS:   process.argv.slice(2)
来源：http://ch.jctech888.com.cn

Java: args 数组（main 方法参数）
来源：http://yu.lnxyls.cn

Go:   os.Args[1:]
来源：http://lk.huanxung.cn

Ruby: ARGV
来源：http://rm.haigaiapp.cn

C#:   args 数组（Main 方法参数）
来源：http://gd.gzmigu.cn

[M02] 读取环境变量
来源：http://cf.9csxet.cn

Py:   os.environ.get("HOME")
来源：http://nr.asd995.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ew.bookmarksfly.cn

JS:   process.env.HOME
来源：http://to.lnxyls.cn

TS:   process.env.HOME
来源：http://uj.muxihuayi.cn

Java: System.getenv("HOME")
来源：http://sh.szxytkj.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://nc.huixinmuqiang.cn

Ruby: ENV["HOME"]
来源：http://fy.asd995.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://tv.chemitech.net.cn

[M03] 执行外部命令
来源：http://ye.lnxyls.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mv.szsharing.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://tr.gzmigu.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://hc.huanxung.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://sp.panjiajie.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ht.shxzukj.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ct.panjiajie.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ij.haigaiapp.cn

C#:   Process.Start("ls", "-l");
来源：http://zz.szsharing.cn

[M04] 获取当前工作目录
来源：http://uu.haigaiapp.cn

Py:   os.getcwd()
来源：http://kv.jianghongdianzi.cn

PHP:  getcwd();
来源：http://qc.colortex.cn

JS:   process.cwd()
来源：http://oa.chemitech.net.cn

TS:   process.cwd()
来源：http://jd.wgjwhj.cn

Java: Path.of("").toAbsolutePath()
来源：http://me.huixinmuqiang.cn

Go:   os.Getwd()
来源：http://gh.colortex.cn

Ruby: Dir.pwd
来源：http://hs.colortex.cn

C#:   Directory.GetCurrentDirectory()
来源：http://vk.huanxung.cn

[M05] 设置退出码
来源：http://nb.huixiangedu.cn

Py:   sys.exit(1)
来源：http://by.gzmigu.cn

PHP:  exit(1);
来源：http://bk.huixinmuqiang.cn

JS:   process.exit(1)
来源：http://iu.yuntaijiaju.cn

TS:   process.exit(1)
来源：http://kl.shtwfgs.cn

Java: System.exit(1)
来源：http://si.szxytkj.cn

Go:   os.Exit(1)
来源：http://iy.szxytkj.cn

Ruby: exit 1
来源：http://ls.bjjhwx.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ci.bookmarksfly.cn

[M06] 向标准错误输出
来源：http://md.wgjwhj.cn

Py:   print("err", file=sys.stderr)
来源：http://cd.nicolike.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://hn.yuntaijiaju.cn

JS:   console.error("err")
来源：http://cg.nszjky.cn

TS:   console.error("err")
来源：http://gr.yuexingan06.cn

Java: System.err.println("err")
来源：http://ag.huixiangedu.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://fr.yuntaijiaju.cn

Ruby: warn "err"
来源：http://fx.gzmigu.cn

C#:   Console.Error.WriteLine("err")
来源：http://pf.gzmigu.cn

[M07] 判断是否为主入口
来源：http://le.shxzukj.cn

Py:   if __name__ == "__main__":
来源：http://oo.wgjwhj.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://gh.huanxung.cn

JS:   require.main === module
来源：http://hc.yuexingan06.cn

TS:   require.main === module
来源：http://es.yuexingan06.cn

Java: public static void main(String[] args)
来源：http://rm.yuexingan06.cn

Go:   func main()
来源：http://ku.shxzukj.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://au.jctech888.com.cn

C#:   static void Main(string[] args)
来源：http://je.asd995.cn

[M08] 获取系统与运行时信息
来源：http://di.shxzskj.cn

Py:   platform.system();  platform.python_version()
来源：http://rk.shxzukj.cn

PHP:  PHP_OS;  phpversion();
来源：http://qg.nicolike.cn

JS:   process.platform;  process.version
来源：http://dw.shxzukj.cn

TS:   process.platform;  process.version
来源：http://rs.9csxet.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://cr.nicolike.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://zm.huixiangedu.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://kt.shxzskj.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://rb.521024.cn

================================================================================
来源：http://um.huixinmuqiang.cn

N. 数据结构与算法
来源：http://iu.chemitech.net.cn

================================================================================
来源：http://tm.lnxyls.cn

[N01] 二分查找（有序数组）
来源：http://vi.hnjuh.cn

Py:   bisect.bisect_left(arr, x)
来源：http://zj.wgjwhj.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://au.shtwfgs.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ke.panjiajie.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://id.wgjwhj.cn

Java: Arrays.binarySearch(arr, x)
来源：http://rb.szxytkj.cn

Go:   sort.SearchInts(arr, x)
来源：http://ag.nszjky.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://jn.bookmarksfly.cn

C#:   Array.BinarySearch(arr, x)
来源：http://zl.huanxung.cn

[N02] 排序（工程实践用内置实现）
来源：http://hp.gzmigu.cn

Py:   sorted(arr);  arr.sort()
来源：http://rn.yuntaijiaju.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://jo.bjjhwx.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://tx.hahajie.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://xx.bjjhwx.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://vp.jianghongdianzi.cn

Go:   slices.Sort(arr)
来源：http://ae.9csxet.cn

Ruby: arr.sort
来源：http://rl.panjiajie.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://oq.huixinmuqiang.cn

[N03] 快速排序（分治示例）
来源：http://hh.nicolike.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://su.9csxet.cn

PHP:  // 递归实现，或用 usort
来源：http://ml.asd995.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fn.hahajie.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gt.muxihuayi.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://zu.yuexingan06.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://re.yuexingan06.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://zy.jianghongdianzi.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ej.szxytkj.cn

[N04] 斐波那契数列
来源：http://ey.nicolike.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://uf.asd995.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://xt.hahajie.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ms.hahajie.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ou.szsharing.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ns.shtwfgs.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://rw.newstarts.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ld.nszjky.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://zu.jctech888.com.cn

[N05] 最大公约数
来源：http://vd.nicolike.cn

Py:   math.gcd(a, b)
来源：http://iz.nszjky.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://tz.jctech888.com.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pt.lnxyls.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fz.bookmarksfly.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://vc.bookmarksfly.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://pd.asd995.cn

Ruby: a.gcd(b)
来源：http://qp.wgjwhj.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://xp.gzmigu.cn

[N06] 判断回文字符串
来源：http://qk.yuexingan06.cn

Py:   s == s[::-1]
来源：http://is.521024.cn

PHP:  $s === strrev($s);
来源：http://zi.521024.cn

JS:   s === [...s].reverse().join("")
来源：http://fm.yuexingan06.cn

TS:   s === [...s].reverse().join("")
来源：http://dk.muxihuayi.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ea.jctech888.com.cn

Go:   // 双指针从两端比较
来源：http://az.jianghongdianzi.cn

Ruby: s == s.reverse
来源：http://qt.yuexingan06.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://kf.wgjwhj.cn

[N07] 两数之和（返回下标）
来源：http://vl.jctech888.com.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ti.hnjuh.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://uz.bookmarksfly.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://mk.hnjuh.cn

TS:   // 手写 Map<string, number>
来源：http://fa.521024.cn

Java: // 手写 HashMap
来源：http://rj.szxytkj.cn

Go:   // 手写 map[int]int
来源：http://gl.shtwfgs.cn

Ruby: // 手写 Hash
来源：http://al.hahajie.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ge.jianghongdianzi.cn

[N08] 生成全排列
来源：http://vn.haigaiapp.cn

Py:   itertools.permutations(arr)
来源：http://zf.newstarts.cn

PHP:  // 手写递归交换
来源：http://ee.szsharing.cn

JS:   // 手写回溯递归
来源：http://yk.panjiajie.cn

TS:   // 手写回溯递归
来源：http://bw.gzmigu.cn

Java: // 手写回溯递归
来源：http://xy.9csxet.cn

Go:   // 手写回溯递归
来源：http://vm.yuntaijiaju.cn

Ruby: arr.permutation.to_a
来源：http://rg.lnxyls.cn

C#:   // 手写回溯递归
来源：http://pe.nszjky.cn

[N09] 栈与队列
来源：http://my.521024.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hl.bjjhwx.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ej.9csxet.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://bb.szxytkj.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://io.jctech888.com.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://nd.lnxyls.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mg.9csxet.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://yd.9csxet.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://af.asd995.cn

[N10] 链表节点定义
来源：http://zy.521024.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ew.shxzskj.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://eq.nszjky.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://dt.9csxet.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://dq.jctech888.com.cn

Java: class Node { int v; Node next; }
来源：http://zv.yuntaijiaju.cn

Go:   type Node struct { V int; Next *Node }
来源：http://oo.shtwfgs.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://zh.shxzukj.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://yd.bjjhwx.cn

[N11] 二叉树中序遍历
来源：http://jm.shxzskj.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ga.nicolike.cn


<!-- 参考信息 -->