代发 wailian999

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ak.521024.cn

[K03] JSON 美化输出（带缩进）
来源：http://ot.muxihuayi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://tn.huanxung.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://md.panjiajie.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ru.wgjwhj.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://fa.colortex.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ws.haigaiapp.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://tz.wgjwhj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://tj.gzmigu.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://lz.huanxung.cn

[K04] 读取 JSON 文件
来源：http://dg.chemitech.net.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://na.newstarts.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://db.asd995.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jn.haigaiapp.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nu.9csxet.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://yr.nszjky.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://lm.huixiangedu.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://vo.hnjuh.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://lr.gzmigu.cn

[K05] 深拷贝对象
来源：http://vz.wgjwhj.cn

Py:   copy.deepcopy(obj)
来源：http://mi.muxihuayi.cn

PHP:  unserialize(serialize($obj));
来源：http://jw.nszjky.cn

JS:   structuredClone(obj)
来源：http://nt.lnxyls.cn

TS:   structuredClone(obj)
来源：http://dg.panjiajie.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ue.szxytkj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://fy.jctech888.com.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hn.huixiangedu.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://uh.asd995.cn

[K06] 解析 URL 查询串
来源：http://kn.nicolike.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://fh.newstarts.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ph.hahajie.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cp.huanxung.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uw.chemitech.net.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://eh.shxzukj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ws.lnxyls.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://fi.yuexingan06.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://qq.9csxet.cn

[K07] 进制转换
来源：http://av.huixiangedu.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://bl.nicolike.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://gx.newstarts.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://jq.chemitech.net.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://dk.huixinmuqiang.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://cr.bjjhwx.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mi.colortex.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://jl.jctech888.com.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://xu.panjiajie.cn

[K08] 二进制序列化（非 JSON）
来源：http://xt.haigaiapp.cn

Py:   pickle.dumps(obj)
来源：http://rp.shtwfgs.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://sz.shxzskj.cn

JS:   v8.serialize(obj)        // Node
来源：http://yc.yuntaijiaju.cn

TS:   v8.serialize(obj)        // Node
来源：http://mn.jctech888.com.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wr.9csxet.cn

Go:   encoding/gob
来源：http://dg.lnxyls.cn

Ruby: Marshal.dump(obj)
来源：http://td.asd995.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ot.nszjky.cn

================================================================================
来源：http://kv.muxihuayi.cn

L. 网络请求
来源：http://cy.huanxung.cn

================================================================================
来源：http://iy.panjiajie.cn

[L01] 发送 GET 请求
来源：http://ig.huixinmuqiang.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://qk.szsharing.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://df.hahajie.cn

JS:   await fetch(url)
来源：http://lu.szxytkj.cn

TS:   await fetch(url)
来源：http://pg.shxzukj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://lk.colortex.cn

Go:   resp, err := http.Get(url)
来源：http://ay.gzmigu.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://bo.wgjwhj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://zu.bjjhwx.cn

[L02] 发送 POST JSON
来源：http://dv.yuntaijiaju.cn

Py:   requests.post(url, json={"a": 1})
来源：http://zv.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://oi.jianghongdianzi.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ls.muxihuayi.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://uo.haigaiapp.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ah.jianghongdianzi.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://kw.521024.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://po.bookmarksfly.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://zh.9csxet.cn

[L03] 设置自定义请求头
来源：http://sw.gzmigu.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://os.nicolike.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://xs.shxzskj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ps.haigaiapp.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wp.panjiajie.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ls.yuexingan06.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wk.yuntaijiaju.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://st.colortex.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ki.shtwfgs.cn

[L04] 设置超时
来源：http://ud.muxihuayi.cn

Py:   requests.get(url, timeout=5)
来源：http://rs.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://by.gzmigu.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ch.hahajie.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ta.lnxyls.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://jk.bjjhwx.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://jz.panjiajie.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://nr.shtwfgs.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://tg.bjjhwx.cn

[L05] 上传文件（multipart）
来源：http://ll.jianghongdianzi.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://kb.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ti.shtwfgs.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://tp.chemitech.net.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://nl.newstarts.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vk.huixinmuqiang.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://cx.bookmarksfly.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://xz.nszjky.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://dy.panjiajie.cn

[L06] 解析响应为 JSON
来源：http://sd.szsharing.cn

Py:   resp.json()
来源：http://sz.haigaiapp.cn

PHP:  json_decode($body, true);
来源：http://wt.gzmigu.cn

JS:   await resp.json()
来源：http://dl.colortex.cn

TS:   await resp.json()
来源：http://vd.hnjuh.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://lo.521024.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://rv.lnxyls.cn

Ruby: JSON.parse(resp.body)
来源：http://ha.bjjhwx.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://xb.shxzukj.cn

[L07] 处理 HTTP 状态码
来源：http://hy.gzmigu.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://do.nicolike.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://da.shtwfgs.cn

JS:   resp.ok;  resp.status
来源：http://ne.yuexingan06.cn

TS:   resp.ok;  resp.status
来源：http://vw.hnjuh.cn

Java: resp.statusCode()
来源：http://nw.nszjky.cn

Go:   resp.StatusCode
来源：http://xc.gzmigu.cn

Ruby: resp.code.to_i
来源：http://qy.hahajie.cn

C#:   (int)resp.StatusCode
来源：http://oc.bjjhwx.cn

[L08] 并发请求多个地址
来源：http://bw.huixinmuqiang.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://dw.hahajie.cn

PHP:  curl_multi_init() 系列
来源：http://fn.hnjuh.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kt.lnxyls.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://uz.yuntaijiaju.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://of.bjjhwx.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mz.asd995.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wv.shtwfgs.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://no.hahajie.cn

================================================================================
来源：http://ur.szsharing.cn

M. 命令行 / 进程 / 环境
来源：http://px.panjiajie.cn

================================================================================
来源：http://qb.yuexingan06.cn

[M01] 读取命令行参数
来源：http://ml.nicolike.cn

Py:   sys.argv[1:]
来源：http://ox.chemitech.net.cn

PHP:  $argv;  $argc;
来源：http://cp.gzmigu.cn

JS:   process.argv.slice(2)
来源：http://iz.jctech888.com.cn

TS:   process.argv.slice(2)
来源：http://sv.shxzskj.cn

Java: args 数组（main 方法参数）
来源：http://ww.newstarts.cn

Go:   os.Args[1:]
来源：http://wc.yuexingan06.cn

Ruby: ARGV
来源：http://ml.huixinmuqiang.cn

C#:   args 数组（Main 方法参数）
来源：http://vs.yuntaijiaju.cn

[M02] 读取环境变量
来源：http://fc.huanxung.cn

Py:   os.environ.get("HOME")
来源：http://nk.huanxung.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rg.9csxet.cn

JS:   process.env.HOME
来源：http://rr.gzmigu.cn

TS:   process.env.HOME
来源：http://rz.szxytkj.cn

Java: System.getenv("HOME")
来源：http://vb.huixinmuqiang.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://sb.hahajie.cn

Ruby: ENV["HOME"]
来源：http://zl.szxytkj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://xw.haigaiapp.cn

[M03] 执行外部命令
来源：http://rx.colortex.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://tt.9csxet.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://dw.wgjwhj.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://vs.yuntaijiaju.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ja.asd995.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://uj.shxzskj.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://cu.hnjuh.cn

Ruby: system("ls -l");  `ls -l`
来源：http://qi.haigaiapp.cn

C#:   Process.Start("ls", "-l");
来源：http://wd.bjjhwx.cn

[M04] 获取当前工作目录
来源：http://nv.huixinmuqiang.cn

Py:   os.getcwd()
来源：http://bq.wgjwhj.cn

PHP:  getcwd();
来源：http://ra.nicolike.cn

JS:   process.cwd()
来源：http://mm.shtwfgs.cn

TS:   process.cwd()
来源：http://rb.huixinmuqiang.cn

Java: Path.of("").toAbsolutePath()
来源：http://yv.shtwfgs.cn

Go:   os.Getwd()
来源：http://fq.asd995.cn

Ruby: Dir.pwd
来源：http://lk.9csxet.cn

C#:   Directory.GetCurrentDirectory()
来源：http://yv.panjiajie.cn

[M05] 设置退出码
来源：http://dj.newstarts.cn

Py:   sys.exit(1)
来源：http://wx.jianghongdianzi.cn

PHP:  exit(1);
来源：http://qe.yuexingan06.cn

JS:   process.exit(1)
来源：http://ii.hahajie.cn

TS:   process.exit(1)
来源：http://at.shxzukj.cn

Java: System.exit(1)
来源：http://xl.haigaiapp.cn

Go:   os.Exit(1)
来源：http://ey.521024.cn

Ruby: exit 1
来源：http://dw.nszjky.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ic.yuexingan06.cn

[M06] 向标准错误输出
来源：http://ca.haigaiapp.cn

Py:   print("err", file=sys.stderr)
来源：http://rc.bjjhwx.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://eu.huanxung.cn

JS:   console.error("err")
来源：http://ej.muxihuayi.cn

TS:   console.error("err")
来源：http://at.colortex.cn

Java: System.err.println("err")
来源：http://ut.nszjky.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://zt.yuexingan06.cn

Ruby: warn "err"
来源：http://og.haigaiapp.cn

C#:   Console.Error.WriteLine("err")
来源：http://xh.huixinmuqiang.cn

[M07] 判断是否为主入口
来源：http://zo.gzmigu.cn

Py:   if __name__ == "__main__":
来源：http://jn.bookmarksfly.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://no.szsharing.cn

JS:   require.main === module
来源：http://kg.haigaiapp.cn

TS:   require.main === module
来源：http://ck.jianghongdianzi.cn

Java: public static void main(String[] args)
来源：http://yx.lnxyls.cn

Go:   func main()
来源：http://hb.9csxet.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ke.jianghongdianzi.cn

C#:   static void Main(string[] args)
来源：http://xm.shxzskj.cn

[M08] 获取系统与运行时信息
来源：http://hg.9csxet.cn

Py:   platform.system();  platform.python_version()
来源：http://jg.yuexingan06.cn

PHP:  PHP_OS;  phpversion();
来源：http://jr.bookmarksfly.cn

JS:   process.platform;  process.version
来源：http://fa.huanxung.cn

TS:   process.platform;  process.version
来源：http://pm.yuntaijiaju.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://vl.shxzskj.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://zs.jianghongdianzi.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ih.newstarts.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://tu.lnxyls.cn

================================================================================
来源：http://ac.yuntaijiaju.cn

N. 数据结构与算法
来源：http://bo.shxzukj.cn

================================================================================
来源：http://fu.bjjhwx.cn

[N01] 二分查找（有序数组）
来源：http://sc.panjiajie.cn

Py:   bisect.bisect_left(arr, x)
来源：http://jf.yuexingan06.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://jp.jctech888.com.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://le.bookmarksfly.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rh.szxytkj.cn

Java: Arrays.binarySearch(arr, x)
来源：http://be.asd995.cn

Go:   sort.SearchInts(arr, x)
来源：http://hc.panjiajie.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://im.jctech888.com.cn

C#:   Array.BinarySearch(arr, x)
来源：http://sn.asd995.cn

[N02] 排序（工程实践用内置实现）
来源：http://bu.lnxyls.cn

Py:   sorted(arr);  arr.sort()
来源：http://tt.jctech888.com.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ap.shxzskj.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://dp.bjjhwx.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://qn.jctech888.com.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://xu.szsharing.cn

Go:   slices.Sort(arr)
来源：http://ou.yuexingan06.cn

Ruby: arr.sort
来源：http://vv.chemitech.net.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://pt.shtwfgs.cn

[N03] 快速排序（分治示例）
来源：http://gn.yuexingan06.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://sa.hahajie.cn

PHP:  // 递归实现，或用 usort
来源：http://yt.shxzukj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fa.bookmarksfly.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jz.nszjky.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://tc.nszjky.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hl.hahajie.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wf.huanxung.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ld.bookmarksfly.cn

[N04] 斐波那契数列
来源：http://bz.jianghongdianzi.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://sp.gzmigu.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ka.panjiajie.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zs.szxytkj.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qe.wgjwhj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hl.huixinmuqiang.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://jg.yuexingan06.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://av.lnxyls.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ke.521024.cn

[N05] 最大公约数
来源：http://dc.shxzskj.cn

Py:   math.gcd(a, b)
来源：http://qr.shxzskj.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://tv.bookmarksfly.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lc.jctech888.com.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fh.colortex.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://qc.yuexingan06.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://an.shxzskj.cn

Ruby: a.gcd(b)
来源：http://lm.muxihuayi.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://zb.asd995.cn

[N06] 判断回文字符串
来源：http://xy.muxihuayi.cn

Py:   s == s[::-1]
来源：http://bj.muxihuayi.cn

PHP:  $s === strrev($s);
来源：http://dz.haigaiapp.cn

JS:   s === [...s].reverse().join("")
来源：http://pa.hnjuh.cn

TS:   s === [...s].reverse().join("")
来源：http://br.huixinmuqiang.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hi.newstarts.cn

Go:   // 双指针从两端比较
来源：http://fk.colortex.cn

Ruby: s == s.reverse
来源：http://wr.yuntaijiaju.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://nl.jianghongdianzi.cn

[N07] 两数之和（返回下标）
来源：http://xo.jctech888.com.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://zn.bjjhwx.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ti.haigaiapp.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://pi.bjjhwx.cn

TS:   // 手写 Map<string, number>
来源：http://ig.yuexingan06.cn

Java: // 手写 HashMap
来源：http://wd.shtwfgs.cn

Go:   // 手写 map[int]int
来源：http://fx.shtwfgs.cn

Ruby: // 手写 Hash
来源：http://mn.huanxung.cn

C#:   // 手写 Dictionary<int, int>
来源：http://eo.shtwfgs.cn

[N08] 生成全排列
来源：http://wj.bjjhwx.cn

Py:   itertools.permutations(arr)
来源：http://ew.nicolike.cn

PHP:  // 手写递归交换
来源：http://bf.huixinmuqiang.cn

JS:   // 手写回溯递归
来源：http://vg.newstarts.cn

TS:   // 手写回溯递归
来源：http://kp.nicolike.cn

Java: // 手写回溯递归
来源：http://ps.lnxyls.cn

Go:   // 手写回溯递归
来源：http://xe.yuntaijiaju.cn

Ruby: arr.permutation.to_a
来源：http://cn.9csxet.cn

C#:   // 手写回溯递归
来源：http://mn.huanxung.cn

[N09] 栈与队列
来源：http://de.huixinmuqiang.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://pc.bjjhwx.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ug.9csxet.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ri.szxytkj.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://rd.jianghongdianzi.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mh.huixiangedu.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wz.nicolike.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://jz.521024.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://kv.nicolike.cn

[N10] 链表节点定义
来源：http://ke.haigaiapp.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://op.huixinmuqiang.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://uz.huixiangedu.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://pq.jctech888.com.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ls.huanxung.cn

Java: class Node { int v; Node next; }
来源：http://fj.shxzukj.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ga.gzmigu.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://yh.szsharing.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ns.muxihuayi.cn

[N11] 二叉树中序遍历
来源：http://ls.nicolike.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://fz.jianghongdianzi.cn


<!-- 参考信息 -->