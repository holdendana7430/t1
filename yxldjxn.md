代发 wailian999

Java: // 手写拷贝构造，或序列化往返
来源：http://bw.9csxet.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://io.nszjky.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://dj.nszjky.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://nt.colortex.cn

[K06] 解析 URL 查询串
来源：http://hf.yuntaijiaju.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mi.hahajie.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://jl.9csxet.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ce.newstarts.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dy.yuexingan06.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://fp.bjjhwx.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://bq.chemitech.net.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://jg.asd995.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://tn.yuexingan06.cn

[K07] 进制转换
来源：http://en.nicolike.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://fr.nicolike.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://au.nszjky.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ky.chemitech.net.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://lg.shxzukj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://uj.jctech888.com.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ih.shtwfgs.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://fy.nicolike.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://vz.yuntaijiaju.cn

[K08] 二进制序列化（非 JSON）
来源：http://fs.521024.cn

Py:   pickle.dumps(obj)
来源：http://su.shxzskj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ng.jctech888.com.cn

JS:   v8.serialize(obj)        // Node
来源：http://fa.521024.cn

TS:   v8.serialize(obj)        // Node
来源：http://fs.shtwfgs.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://yq.bookmarksfly.cn

Go:   encoding/gob
来源：http://zi.huixiangedu.cn

Ruby: Marshal.dump(obj)
来源：http://rf.hahajie.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://km.hnjuh.cn

================================================================================
来源：http://sf.nszjky.cn

L. 网络请求
来源：http://mt.huixinmuqiang.cn

================================================================================
来源：http://dw.colortex.cn

[L01] 发送 GET 请求
来源：http://dk.shxzskj.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mm.haigaiapp.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hr.asd995.cn

JS:   await fetch(url)
来源：http://aw.newstarts.cn

TS:   await fetch(url)
来源：http://pl.jianghongdianzi.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://lk.haigaiapp.cn

Go:   resp, err := http.Get(url)
来源：http://iz.yuntaijiaju.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ha.haigaiapp.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://lm.shxzskj.cn

[L02] 发送 POST JSON
来源：http://rs.huixinmuqiang.cn

Py:   requests.post(url, json={"a": 1})
来源：http://gj.hnjuh.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://bh.shxzskj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://td.shxzukj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hl.shxzukj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://sd.newstarts.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://tm.bjjhwx.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://qu.huanxung.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ao.chemitech.net.cn

[L03] 设置自定义请求头
来源：http://vh.chemitech.net.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://bd.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://na.lnxyls.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ey.gzmigu.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mu.panjiajie.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://gh.hnjuh.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://gu.jianghongdianzi.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://pi.huanxung.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://nj.haigaiapp.cn

[L04] 设置超时
来源：http://dq.nicolike.cn

Py:   requests.get(url, timeout=5)
来源：http://cl.wgjwhj.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ec.colortex.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hn.lnxyls.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qh.shtwfgs.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://jz.shxzukj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://tp.shxzskj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ut.huixinmuqiang.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qy.hnjuh.cn

[L05] 上传文件（multipart）
来源：http://ih.wgjwhj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://rl.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ul.9csxet.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://vv.nszjky.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://vx.huanxung.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://lf.shtwfgs.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://rd.haigaiapp.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://pt.hahajie.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://dc.yuntaijiaju.cn

[L06] 解析响应为 JSON
来源：http://hg.hnjuh.cn

Py:   resp.json()
来源：http://ik.newstarts.cn

PHP:  json_decode($body, true);
来源：http://fz.szxytkj.cn

JS:   await resp.json()
来源：http://bg.szxytkj.cn

TS:   await resp.json()
来源：http://ea.wgjwhj.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mo.panjiajie.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://qi.panjiajie.cn

Ruby: JSON.parse(resp.body)
来源：http://kx.gzmigu.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://vd.gzmigu.cn

[L07] 处理 HTTP 状态码
来源：http://vc.colortex.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://lu.yuntaijiaju.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://bk.lnxyls.cn

JS:   resp.ok;  resp.status
来源：http://ge.jctech888.com.cn

TS:   resp.ok;  resp.status
来源：http://dp.shxzskj.cn

Java: resp.statusCode()
来源：http://ej.yuexingan06.cn

Go:   resp.StatusCode
来源：http://ar.shxzskj.cn

Ruby: resp.code.to_i
来源：http://gg.jianghongdianzi.cn

C#:   (int)resp.StatusCode
来源：http://qu.colortex.cn

[L08] 并发请求多个地址
来源：http://gp.huanxung.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://vv.huanxung.cn

PHP:  curl_multi_init() 系列
来源：http://wx.haigaiapp.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jg.shtwfgs.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ri.asd995.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ds.huanxung.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://fl.jctech888.com.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://pb.jctech888.com.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://vq.szxytkj.cn

================================================================================
来源：http://bd.szsharing.cn

M. 命令行 / 进程 / 环境
来源：http://hd.huixiangedu.cn

================================================================================
来源：http://or.szxytkj.cn

[M01] 读取命令行参数
来源：http://cs.shxzskj.cn

Py:   sys.argv[1:]
来源：http://ok.9csxet.cn

PHP:  $argv;  $argc;
来源：http://dy.9csxet.cn

JS:   process.argv.slice(2)
来源：http://iw.colortex.cn

TS:   process.argv.slice(2)
来源：http://aw.shtwfgs.cn

Java: args 数组（main 方法参数）
来源：http://rj.huixinmuqiang.cn

Go:   os.Args[1:]
来源：http://xg.muxihuayi.cn

Ruby: ARGV
来源：http://ue.szxytkj.cn

C#:   args 数组（Main 方法参数）
来源：http://ft.chemitech.net.cn

[M02] 读取环境变量
来源：http://mw.colortex.cn

Py:   os.environ.get("HOME")
来源：http://hw.gzmigu.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://sn.bookmarksfly.cn

JS:   process.env.HOME
来源：http://tu.yuexingan06.cn

TS:   process.env.HOME
来源：http://wn.colortex.cn

Java: System.getenv("HOME")
来源：http://js.nicolike.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://tq.asd995.cn

Ruby: ENV["HOME"]
来源：http://kf.9csxet.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://gc.wgjwhj.cn

[M03] 执行外部命令
来源：http://fk.asd995.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://un.nicolike.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ld.bjjhwx.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://kq.huanxung.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://gj.gzmigu.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://qj.colortex.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://nv.hnjuh.cn

Ruby: system("ls -l");  `ls -l`
来源：http://rw.521024.cn

C#:   Process.Start("ls", "-l");
来源：http://qf.huixinmuqiang.cn

[M04] 获取当前工作目录
来源：http://kl.yuntaijiaju.cn

Py:   os.getcwd()
来源：http://oj.jctech888.com.cn

PHP:  getcwd();
来源：http://ux.bjjhwx.cn

JS:   process.cwd()
来源：http://gu.wgjwhj.cn

TS:   process.cwd()
来源：http://ym.panjiajie.cn

Java: Path.of("").toAbsolutePath()
来源：http://ef.muxihuayi.cn

Go:   os.Getwd()
来源：http://rx.shtwfgs.cn

Ruby: Dir.pwd
来源：http://ya.shxzukj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ml.hahajie.cn

[M05] 设置退出码
来源：http://zj.bookmarksfly.cn

Py:   sys.exit(1)
来源：http://ir.hahajie.cn

PHP:  exit(1);
来源：http://gj.muxihuayi.cn

JS:   process.exit(1)
来源：http://om.newstarts.cn

TS:   process.exit(1)
来源：http://of.nicolike.cn

Java: System.exit(1)
来源：http://nu.shxzukj.cn

Go:   os.Exit(1)
来源：http://vv.shtwfgs.cn

Ruby: exit 1
来源：http://rc.chemitech.net.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ym.huanxung.cn

[M06] 向标准错误输出
来源：http://wv.shxzukj.cn

Py:   print("err", file=sys.stderr)
来源：http://tn.huixiangedu.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://rx.521024.cn

JS:   console.error("err")
来源：http://rs.newstarts.cn

TS:   console.error("err")
来源：http://ss.bjjhwx.cn

Java: System.err.println("err")
来源：http://pl.shtwfgs.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://cn.bjjhwx.cn

Ruby: warn "err"
来源：http://br.huanxung.cn

C#:   Console.Error.WriteLine("err")
来源：http://aa.shtwfgs.cn

[M07] 判断是否为主入口
来源：http://fg.gzmigu.cn

Py:   if __name__ == "__main__":
来源：http://jj.jctech888.com.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hl.chemitech.net.cn

JS:   require.main === module
来源：http://hs.huixinmuqiang.cn

TS:   require.main === module
来源：http://zv.shtwfgs.cn

Java: public static void main(String[] args)
来源：http://ip.yuexingan06.cn

Go:   func main()
来源：http://wk.bjjhwx.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://da.huixiangedu.cn

C#:   static void Main(string[] args)
来源：http://si.bookmarksfly.cn

[M08] 获取系统与运行时信息
来源：http://nl.haigaiapp.cn

Py:   platform.system();  platform.python_version()
来源：http://eo.asd995.cn

PHP:  PHP_OS;  phpversion();
来源：http://bb.huixiangedu.cn

JS:   process.platform;  process.version
来源：http://as.asd995.cn

TS:   process.platform;  process.version
来源：http://vq.shxzukj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ex.colortex.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ta.wgjwhj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://nq.jianghongdianzi.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://bl.9csxet.cn

================================================================================
来源：http://ej.9csxet.cn

N. 数据结构与算法
来源：http://zv.huixiangedu.cn

================================================================================
来源：http://qz.wgjwhj.cn

[N01] 二分查找（有序数组）
来源：http://og.gzmigu.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ns.asd995.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://fm.huixinmuqiang.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wz.shxzukj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jk.hahajie.cn

Java: Arrays.binarySearch(arr, x)
来源：http://lp.szxytkj.cn

Go:   sort.SearchInts(arr, x)
来源：http://fa.hahajie.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ie.huixiangedu.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ud.hnjuh.cn

[N02] 排序（工程实践用内置实现）
来源：http://vx.huanxung.cn

Py:   sorted(arr);  arr.sort()
来源：http://xz.szsharing.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://zm.lnxyls.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://xb.shxzskj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ve.nszjky.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://tt.muxihuayi.cn

Go:   slices.Sort(arr)
来源：http://ek.asd995.cn

Ruby: arr.sort
来源：http://ry.hnjuh.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://fh.colortex.cn

[N03] 快速排序（分治示例）
来源：http://ix.wgjwhj.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://rc.huixinmuqiang.cn

PHP:  // 递归实现，或用 usort
来源：http://cn.521024.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lq.jianghongdianzi.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ze.jianghongdianzi.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ed.shtwfgs.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://pf.yuexingan06.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://pu.hnjuh.cn

C#:   // 手写递归，或 Array.Sort
来源：http://do.shxzukj.cn

[N04] 斐波那契数列
来源：http://ze.nszjky.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://xs.jianghongdianzi.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://rm.huanxung.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ni.gzmigu.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qz.muxihuayi.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ql.bookmarksfly.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://zf.9csxet.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wm.9csxet.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://fk.nszjky.cn

[N05] 最大公约数
来源：http://zn.bjjhwx.cn

Py:   math.gcd(a, b)
来源：http://cy.gzmigu.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://lq.gzmigu.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qb.shxzukj.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://co.jctech888.com.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ye.nszjky.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://da.bookmarksfly.cn

Ruby: a.gcd(b)
来源：http://ro.9csxet.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://xd.shtwfgs.cn

[N06] 判断回文字符串
来源：http://ql.gzmigu.cn

Py:   s == s[::-1]
来源：http://ze.shtwfgs.cn

PHP:  $s === strrev($s);
来源：http://dr.9csxet.cn

JS:   s === [...s].reverse().join("")
来源：http://ew.panjiajie.cn

TS:   s === [...s].reverse().join("")
来源：http://ha.gzmigu.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://qf.bookmarksfly.cn

Go:   // 双指针从两端比较
来源：http://gc.gzmigu.cn

Ruby: s == s.reverse
来源：http://pr.bookmarksfly.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://xu.nszjky.cn

[N07] 两数之和（返回下标）
来源：http://ou.lnxyls.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://jb.yuexingan06.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ro.yuntaijiaju.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://mv.newstarts.cn

TS:   // 手写 Map<string, number>
来源：http://jq.huanxung.cn

Java: // 手写 HashMap
来源：http://ml.haigaiapp.cn

Go:   // 手写 map[int]int
来源：http://ua.shtwfgs.cn

Ruby: // 手写 Hash
来源：http://yo.9csxet.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ba.muxihuayi.cn

[N08] 生成全排列
来源：http://kn.jctech888.com.cn

Py:   itertools.permutations(arr)
来源：http://tq.newstarts.cn

PHP:  // 手写递归交换
来源：http://cd.chemitech.net.cn

JS:   // 手写回溯递归
来源：http://ns.jianghongdianzi.cn

TS:   // 手写回溯递归
来源：http://ey.huixiangedu.cn

Java: // 手写回溯递归
来源：http://fm.newstarts.cn

Go:   // 手写回溯递归
来源：http://tj.newstarts.cn

Ruby: arr.permutation.to_a
来源：http://fr.nszjky.cn

C#:   // 手写回溯递归
来源：http://ya.haigaiapp.cn

[N09] 栈与队列
来源：http://bc.gzmigu.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://be.shtwfgs.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://jc.colortex.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://cq.bookmarksfly.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://pb.bookmarksfly.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mu.gzmigu.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://br.jianghongdianzi.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://jx.panjiajie.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hn.shtwfgs.cn

[N10] 链表节点定义
来源：http://lv.nicolike.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://sy.yuexingan06.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://no.shxzskj.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ds.nszjky.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://cx.yuntaijiaju.cn

Java: class Node { int v; Node next; }
来源：http://bc.asd995.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ug.huanxung.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://qa.9csxet.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://in.huixiangedu.cn

[N11] 二叉树中序遍历
来源：http://ul.asd995.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://uf.jctech888.com.cn

PHP:  // 手写递归函数
来源：http://ie.bookmarksfly.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xr.panjiajie.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ly.shxzskj.cn

Java: // 手写递归
来源：http://cz.nszjky.cn

Go:   // 手写递归
来源：http://ik.chemitech.net.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://oo.jianghongdianzi.cn

C#:   // 手写递归
来源：http://el.lnxyls.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mh.colortex.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wx.chemitech.net.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ok.nszjky.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sr.newstarts.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bn.huanxung.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ry.shtwfgs.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://dr.yuntaijiaju.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://xi.bookmarksfly.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://rr.jctech888.com.cn

================================================================================
来源：http://ey.jianghongdianzi.cn

O. 并发与异步
来源：http://ty.hahajie.cn

================================================================================
来源：http://zh.nszjky.cn

[O01] 启动一个线程
来源：http://gm.nicolike.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://go.huixiangedu.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://fi.hnjuh.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://sp.9csxet.cn

TS:   // 同 JS
来源：http://ao.yuexingan06.cn


<!-- 参考信息 -->