代发 wailian999

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://un.colortex.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zg.nicolike.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kv.9csxet.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://kv.yuexingan06.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mq.shxzukj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ux.yuntaijiaju.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jj.shtwfgs.cn

[K05] 深拷贝对象
来源：http://yk.jctech888.com.cn

Py:   copy.deepcopy(obj)
来源：http://hr.yuexingan06.cn

PHP:  unserialize(serialize($obj));
来源：http://qh.lnxyls.cn

JS:   structuredClone(obj)
来源：http://hh.huixiangedu.cn

TS:   structuredClone(obj)
来源：http://yl.wgjwhj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://no.wgjwhj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://tb.nszjky.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mz.yuexingan06.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://zg.hahajie.cn

[K06] 解析 URL 查询串
来源：http://fj.hnjuh.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://pa.wgjwhj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zc.bjjhwx.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ar.huanxung.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ft.chemitech.net.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://pa.yuntaijiaju.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ri.newstarts.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wp.shxzukj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://od.hnjuh.cn

[K07] 进制转换
来源：http://ax.haigaiapp.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://gl.jianghongdianzi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://dw.shxzskj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://rv.hahajie.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://rs.lnxyls.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://dd.huixinmuqiang.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://pw.newstarts.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://lv.9csxet.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://rt.hahajie.cn

[K08] 二进制序列化（非 JSON）
来源：http://bt.bookmarksfly.cn

Py:   pickle.dumps(obj)
来源：http://af.gzmigu.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://km.hahajie.cn

JS:   v8.serialize(obj)        // Node
来源：http://ro.jianghongdianzi.cn

TS:   v8.serialize(obj)        // Node
来源：http://pa.shtwfgs.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ax.gzmigu.cn

Go:   encoding/gob
来源：http://lx.huixiangedu.cn

Ruby: Marshal.dump(obj)
来源：http://ll.bjjhwx.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ds.hahajie.cn

================================================================================
来源：http://bm.jianghongdianzi.cn

L. 网络请求
来源：http://iv.nszjky.cn

================================================================================
来源：http://et.shxzskj.cn

[L01] 发送 GET 请求
来源：http://kr.hahajie.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://rz.hnjuh.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://lm.szsharing.cn

JS:   await fetch(url)
来源：http://zc.shtwfgs.cn

TS:   await fetch(url)
来源：http://lh.shxzskj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://xm.hnjuh.cn

Go:   resp, err := http.Get(url)
来源：http://hm.yuexingan06.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://it.gzmigu.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://bi.jianghongdianzi.cn

[L02] 发送 POST JSON
来源：http://ws.chemitech.net.cn

Py:   requests.post(url, json={"a": 1})
来源：http://vb.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://gj.szsharing.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zm.huanxung.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wm.haigaiapp.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://sx.huixiangedu.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://dt.9csxet.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ki.colortex.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ok.huanxung.cn

[L03] 设置自定义请求头
来源：http://bw.lnxyls.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://tp.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ke.newstarts.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fi.hahajie.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xv.yuntaijiaju.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://gj.yuntaijiaju.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://lz.hnjuh.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://vf.colortex.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://vl.nszjky.cn

[L04] 设置超时
来源：http://uw.bjjhwx.cn

Py:   requests.get(url, timeout=5)
来源：http://ae.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://kr.hahajie.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ai.szsharing.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qx.huixiangedu.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://kc.bookmarksfly.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://bl.haigaiapp.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://lj.asd995.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://na.shxzukj.cn

[L05] 上传文件（multipart）
来源：http://cg.huanxung.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://vu.gzmigu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://bv.lnxyls.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://cd.lnxyls.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ov.shtwfgs.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://rn.jianghongdianzi.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://vc.szxytkj.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ih.shtwfgs.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ae.colortex.cn

[L06] 解析响应为 JSON
来源：http://gu.huixinmuqiang.cn

Py:   resp.json()
来源：http://as.asd995.cn

PHP:  json_decode($body, true);
来源：http://nk.lnxyls.cn

JS:   await resp.json()
来源：http://gz.muxihuayi.cn

TS:   await resp.json()
来源：http://rw.muxihuayi.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ud.huixiangedu.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://rr.huanxung.cn

Ruby: JSON.parse(resp.body)
来源：http://va.hnjuh.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://bv.jctech888.com.cn

[L07] 处理 HTTP 状态码
来源：http://nk.panjiajie.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://qx.shxzskj.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://vv.shtwfgs.cn

JS:   resp.ok;  resp.status
来源：http://nn.huanxung.cn

TS:   resp.ok;  resp.status
来源：http://xg.wgjwhj.cn

Java: resp.statusCode()
来源：http://mv.shtwfgs.cn

Go:   resp.StatusCode
来源：http://wo.shxzukj.cn

Ruby: resp.code.to_i
来源：http://rf.szxytkj.cn

C#:   (int)resp.StatusCode
来源：http://ng.huixinmuqiang.cn

[L08] 并发请求多个地址
来源：http://gb.bjjhwx.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://zv.panjiajie.cn

PHP:  curl_multi_init() 系列
来源：http://pi.shxzskj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nq.gzmigu.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ym.panjiajie.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ea.nicolike.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ea.yuexingan06.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mp.yuntaijiaju.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://rc.wgjwhj.cn

================================================================================
来源：http://ni.huixiangedu.cn

M. 命令行 / 进程 / 环境
来源：http://dj.gzmigu.cn

================================================================================
来源：http://or.hnjuh.cn

[M01] 读取命令行参数
来源：http://fu.nicolike.cn

Py:   sys.argv[1:]
来源：http://mf.shxzskj.cn

PHP:  $argv;  $argc;
来源：http://cp.jianghongdianzi.cn

JS:   process.argv.slice(2)
来源：http://za.chemitech.net.cn

TS:   process.argv.slice(2)
来源：http://sn.gzmigu.cn

Java: args 数组（main 方法参数）
来源：http://sa.bjjhwx.cn

Go:   os.Args[1:]
来源：http://rt.bjjhwx.cn

Ruby: ARGV
来源：http://qe.nicolike.cn

C#:   args 数组（Main 方法参数）
来源：http://nt.521024.cn

[M02] 读取环境变量
来源：http://gg.muxihuayi.cn

Py:   os.environ.get("HOME")
来源：http://eg.yuntaijiaju.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://nn.jctech888.com.cn

JS:   process.env.HOME
来源：http://li.panjiajie.cn

TS:   process.env.HOME
来源：http://eh.nicolike.cn

Java: System.getenv("HOME")
来源：http://nt.shxzskj.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://gn.chemitech.net.cn

Ruby: ENV["HOME"]
来源：http://jx.gzmigu.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://xx.shtwfgs.cn

[M03] 执行外部命令
来源：http://ey.9csxet.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://aa.bookmarksfly.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://dw.nszjky.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://lf.hnjuh.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://mn.asd995.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://yp.shtwfgs.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://cd.colortex.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ud.jctech888.com.cn

C#:   Process.Start("ls", "-l");
来源：http://mn.yuexingan06.cn

[M04] 获取当前工作目录
来源：http://mw.521024.cn

Py:   os.getcwd()
来源：http://av.shxzukj.cn

PHP:  getcwd();
来源：http://jp.shxzskj.cn

JS:   process.cwd()
来源：http://wd.bookmarksfly.cn

TS:   process.cwd()
来源：http://cy.bjjhwx.cn

Java: Path.of("").toAbsolutePath()
来源：http://hx.9csxet.cn

Go:   os.Getwd()
来源：http://lo.9csxet.cn

Ruby: Dir.pwd
来源：http://vq.wgjwhj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://oo.shxzukj.cn

[M05] 设置退出码
来源：http://mq.hnjuh.cn

Py:   sys.exit(1)
来源：http://pl.huixinmuqiang.cn

PHP:  exit(1);
来源：http://pv.nicolike.cn

JS:   process.exit(1)
来源：http://ne.newstarts.cn

TS:   process.exit(1)
来源：http://st.yuexingan06.cn

Java: System.exit(1)
来源：http://cb.chemitech.net.cn

Go:   os.Exit(1)
来源：http://cx.jianghongdianzi.cn

Ruby: exit 1
来源：http://bt.jianghongdianzi.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://gc.9csxet.cn

[M06] 向标准错误输出
来源：http://oa.nicolike.cn

Py:   print("err", file=sys.stderr)
来源：http://dr.shxzskj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://yd.haigaiapp.cn

JS:   console.error("err")
来源：http://oy.bookmarksfly.cn

TS:   console.error("err")
来源：http://dm.yuexingan06.cn

Java: System.err.println("err")
来源：http://rj.bjjhwx.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ev.huixinmuqiang.cn

Ruby: warn "err"
来源：http://cl.panjiajie.cn

C#:   Console.Error.WriteLine("err")
来源：http://fx.521024.cn

[M07] 判断是否为主入口
来源：http://rz.colortex.cn

Py:   if __name__ == "__main__":
来源：http://zm.jctech888.com.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://az.szxytkj.cn

JS:   require.main === module
来源：http://gu.hahajie.cn

TS:   require.main === module
来源：http://ts.shxzukj.cn

Java: public static void main(String[] args)
来源：http://bi.yuntaijiaju.cn

Go:   func main()
来源：http://nb.nicolike.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mo.chemitech.net.cn

C#:   static void Main(string[] args)
来源：http://de.wgjwhj.cn

[M08] 获取系统与运行时信息
来源：http://jp.hahajie.cn

Py:   platform.system();  platform.python_version()
来源：http://fi.muxihuayi.cn

PHP:  PHP_OS;  phpversion();
来源：http://mf.huixinmuqiang.cn

JS:   process.platform;  process.version
来源：http://hn.szxytkj.cn

TS:   process.platform;  process.version
来源：http://ul.shxzukj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://aj.521024.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://nw.bjjhwx.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://bi.szxytkj.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://vo.huanxung.cn

================================================================================
来源：http://cc.9csxet.cn

N. 数据结构与算法
来源：http://po.bjjhwx.cn

================================================================================
来源：http://sw.muxihuayi.cn

[N01] 二分查找（有序数组）
来源：http://fn.hahajie.cn

Py:   bisect.bisect_left(arr, x)
来源：http://eb.bookmarksfly.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://cy.bookmarksfly.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://go.haigaiapp.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ut.jianghongdianzi.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ie.521024.cn

Go:   sort.SearchInts(arr, x)
来源：http://hy.shxzukj.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://su.huanxung.cn

C#:   Array.BinarySearch(arr, x)
来源：http://vh.asd995.cn

[N02] 排序（工程实践用内置实现）
来源：http://ms.bjjhwx.cn

Py:   sorted(arr);  arr.sort()
来源：http://tm.panjiajie.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://fm.newstarts.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://er.huixinmuqiang.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://yv.haigaiapp.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://gm.gzmigu.cn

Go:   slices.Sort(arr)
来源：http://vm.huixinmuqiang.cn

Ruby: arr.sort
来源：http://ac.asd995.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://pd.bjjhwx.cn

[N03] 快速排序（分治示例）
来源：http://wz.shxzskj.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ka.huixiangedu.cn

PHP:  // 递归实现，或用 usort
来源：http://na.9csxet.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ln.szxytkj.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yw.hahajie.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://kk.haigaiapp.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://rr.muxihuayi.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://vf.jctech888.com.cn

C#:   // 手写递归，或 Array.Sort
来源：http://yk.shxzskj.cn

[N04] 斐波那契数列
来源：http://gh.bjjhwx.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hn.521024.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://xc.haigaiapp.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cs.gzmigu.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tm.nicolike.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://yi.jianghongdianzi.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ou.shtwfgs.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://sm.panjiajie.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://cz.newstarts.cn

[N05] 最大公约数
来源：http://uk.hahajie.cn

Py:   math.gcd(a, b)
来源：http://pv.shtwfgs.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://te.gzmigu.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jp.haigaiapp.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tv.szsharing.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ix.szxytkj.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ud.hahajie.cn

Ruby: a.gcd(b)
来源：http://lu.hahajie.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://gu.newstarts.cn

[N06] 判断回文字符串
来源：http://lg.9csxet.cn

Py:   s == s[::-1]
来源：http://in.yuntaijiaju.cn

PHP:  $s === strrev($s);
来源：http://mv.haigaiapp.cn

JS:   s === [...s].reverse().join("")
来源：http://eu.nszjky.cn

TS:   s === [...s].reverse().join("")
来源：http://cm.521024.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mb.chemitech.net.cn

Go:   // 双指针从两端比较
来源：http://ek.wgjwhj.cn

Ruby: s == s.reverse
来源：http://hp.nszjky.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://sw.newstarts.cn

[N07] 两数之和（返回下标）
来源：http://jh.hnjuh.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://yi.chemitech.net.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://gi.colortex.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://wk.bookmarksfly.cn

TS:   // 手写 Map<string, number>
来源：http://qi.huanxung.cn

Java: // 手写 HashMap
来源：http://no.gzmigu.cn

Go:   // 手写 map[int]int
来源：http://aj.panjiajie.cn

Ruby: // 手写 Hash
来源：http://es.bookmarksfly.cn

C#:   // 手写 Dictionary<int, int>
来源：http://wo.yuntaijiaju.cn

[N08] 生成全排列
来源：http://zi.wgjwhj.cn

Py:   itertools.permutations(arr)
来源：http://pj.yuntaijiaju.cn

PHP:  // 手写递归交换
来源：http://wo.nszjky.cn

JS:   // 手写回溯递归
来源：http://ln.jctech888.com.cn

TS:   // 手写回溯递归
来源：http://kl.huixinmuqiang.cn

Java: // 手写回溯递归
来源：http://mt.wgjwhj.cn

Go:   // 手写回溯递归
来源：http://fk.yuntaijiaju.cn

Ruby: arr.permutation.to_a
来源：http://cj.nszjky.cn

C#:   // 手写回溯递归
来源：http://oa.yuexingan06.cn

[N09] 栈与队列
来源：http://wy.gzmigu.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ro.huixinmuqiang.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://fc.gzmigu.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://gl.yuntaijiaju.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://xs.yuntaijiaju.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://lr.nicolike.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://kx.shxzukj.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ft.chemitech.net.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://or.newstarts.cn

[N10] 链表节点定义
来源：http://kq.panjiajie.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wx.haigaiapp.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ql.shxzskj.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://yl.lnxyls.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://by.521024.cn

Java: class Node { int v; Node next; }
来源：http://lw.yuntaijiaju.cn

Go:   type Node struct { V int; Next *Node }
来源：http://yr.jctech888.com.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ww.hnjuh.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://pg.jianghongdianzi.cn

[N11] 二叉树中序遍历
来源：http://sr.asd995.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://om.szxytkj.cn

PHP:  // 手写递归函数
来源：http://tx.nszjky.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ei.521024.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ak.hnjuh.cn

Java: // 手写递归
来源：http://hl.yuntaijiaju.cn

Go:   // 手写递归
来源：http://tf.hahajie.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://fb.jianghongdianzi.cn

C#:   // 手写递归
来源：http://xu.shxzskj.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://yp.huixinmuqiang.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://kg.newstarts.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mt.gzmigu.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ov.shxzukj.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://uy.hnjuh.cn


<!-- 参考信息 -->