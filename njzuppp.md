代发 wailian999

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://va.jianghongdianzi.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://yp.hnjuh.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://fn.szxytkj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ep.colortex.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://gu.nszjky.cn

[K07] 进制转换
来源：http://aw.bjjhwx.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://da.hnjuh.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://yo.szxytkj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://kw.hnjuh.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://yp.muxihuayi.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://tr.chemitech.net.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://jf.nicolike.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://sm.jctech888.com.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://lr.newstarts.cn

[K08] 二进制序列化（非 JSON）
来源：http://su.gzmigu.cn

Py:   pickle.dumps(obj)
来源：http://wb.shxzskj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://tm.jctech888.com.cn

JS:   v8.serialize(obj)        // Node
来源：http://yi.hahajie.cn

TS:   v8.serialize(obj)        // Node
来源：http://mr.shxzskj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://nh.colortex.cn

Go:   encoding/gob
来源：http://yl.haigaiapp.cn

Ruby: Marshal.dump(obj)
来源：http://xj.shxzukj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ze.chemitech.net.cn

================================================================================
来源：http://yr.wgjwhj.cn

L. 网络请求
来源：http://if.jianghongdianzi.cn

================================================================================
来源：http://dl.jctech888.com.cn

[L01] 发送 GET 请求
来源：http://xa.wgjwhj.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://un.huixiangedu.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://or.shxzskj.cn

JS:   await fetch(url)
来源：http://bl.521024.cn

TS:   await fetch(url)
来源：http://vp.asd995.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qh.huixinmuqiang.cn

Go:   resp, err := http.Get(url)
来源：http://bk.bjjhwx.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://fg.hahajie.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://sz.gzmigu.cn

[L02] 发送 POST JSON
来源：http://or.9csxet.cn

Py:   requests.post(url, json={"a": 1})
来源：http://pu.szsharing.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://em.yuntaijiaju.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tm.szxytkj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://oa.gzmigu.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ap.huanxung.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jn.jctech888.com.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ot.9csxet.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wt.gzmigu.cn

[L03] 设置自定义请求头
来源：http://jx.chemitech.net.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://qw.huixiangedu.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://so.colortex.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ut.nszjky.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zw.yuntaijiaju.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://pd.jctech888.com.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://yh.huixiangedu.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://gv.nicolike.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ev.shtwfgs.cn

[L04] 设置超时
来源：http://wy.yuntaijiaju.cn

Py:   requests.get(url, timeout=5)
来源：http://td.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://cy.shxzukj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://id.newstarts.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ls.muxihuayi.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ww.szxytkj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://rf.bookmarksfly.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://zm.bjjhwx.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://xy.panjiajie.cn

[L05] 上传文件（multipart）
来源：http://ki.yuexingan06.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://yd.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hv.shxzskj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://cv.szxytkj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://bz.bookmarksfly.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://kl.nicolike.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://za.yuntaijiaju.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://yu.521024.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://dz.asd995.cn

[L06] 解析响应为 JSON
来源：http://hc.yuntaijiaju.cn

Py:   resp.json()
来源：http://bb.9csxet.cn

PHP:  json_decode($body, true);
来源：http://fb.colortex.cn

JS:   await resp.json()
来源：http://qe.9csxet.cn

TS:   await resp.json()
来源：http://pg.nszjky.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://nj.szsharing.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://gb.shtwfgs.cn

Ruby: JSON.parse(resp.body)
来源：http://iw.hnjuh.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ps.yuntaijiaju.cn

[L07] 处理 HTTP 状态码
来源：http://ga.bookmarksfly.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ns.bookmarksfly.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wt.newstarts.cn

JS:   resp.ok;  resp.status
来源：http://qs.hahajie.cn

TS:   resp.ok;  resp.status
来源：http://qa.shtwfgs.cn

Java: resp.statusCode()
来源：http://ea.521024.cn

Go:   resp.StatusCode
来源：http://ja.bjjhwx.cn

Ruby: resp.code.to_i
来源：http://ur.521024.cn

C#:   (int)resp.StatusCode
来源：http://uu.newstarts.cn

[L08] 并发请求多个地址
来源：http://ua.szsharing.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hl.9csxet.cn

PHP:  curl_multi_init() 系列
来源：http://ww.jctech888.com.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rt.lnxyls.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nr.newstarts.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://gv.nicolike.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://jw.gzmigu.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wc.colortex.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://vg.newstarts.cn

================================================================================
来源：http://bn.huixiangedu.cn

M. 命令行 / 进程 / 环境
来源：http://nn.muxihuayi.cn

================================================================================
来源：http://vj.panjiajie.cn

[M01] 读取命令行参数
来源：http://qg.muxihuayi.cn

Py:   sys.argv[1:]
来源：http://pz.yuexingan06.cn

PHP:  $argv;  $argc;
来源：http://xl.szsharing.cn

JS:   process.argv.slice(2)
来源：http://ox.asd995.cn

TS:   process.argv.slice(2)
来源：http://yi.szsharing.cn

Java: args 数组（main 方法参数）
来源：http://ed.bookmarksfly.cn

Go:   os.Args[1:]
来源：http://mr.huixinmuqiang.cn

Ruby: ARGV
来源：http://ud.huixiangedu.cn

C#:   args 数组（Main 方法参数）
来源：http://td.yuntaijiaju.cn

[M02] 读取环境变量
来源：http://hp.hahajie.cn

Py:   os.environ.get("HOME")
来源：http://aq.bjjhwx.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ir.521024.cn

JS:   process.env.HOME
来源：http://jd.521024.cn

TS:   process.env.HOME
来源：http://oo.yuexingan06.cn

Java: System.getenv("HOME")
来源：http://xw.muxihuayi.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://un.shtwfgs.cn

Ruby: ENV["HOME"]
来源：http://qn.chemitech.net.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://do.shtwfgs.cn

[M03] 执行外部命令
来源：http://mw.bjjhwx.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mi.hnjuh.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hk.colortex.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://zl.yuexingan06.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://cq.jctech888.com.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://dq.haigaiapp.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://fq.shxzskj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ar.colortex.cn

C#:   Process.Start("ls", "-l");
来源：http://py.newstarts.cn

[M04] 获取当前工作目录
来源：http://rm.chemitech.net.cn

Py:   os.getcwd()
来源：http://rn.haigaiapp.cn

PHP:  getcwd();
来源：http://nh.jctech888.com.cn

JS:   process.cwd()
来源：http://ph.gzmigu.cn

TS:   process.cwd()
来源：http://dp.521024.cn

Java: Path.of("").toAbsolutePath()
来源：http://os.521024.cn

Go:   os.Getwd()
来源：http://ei.haigaiapp.cn

Ruby: Dir.pwd
来源：http://ij.yuexingan06.cn

C#:   Directory.GetCurrentDirectory()
来源：http://fr.521024.cn

[M05] 设置退出码
来源：http://zd.hnjuh.cn

Py:   sys.exit(1)
来源：http://hz.shxzukj.cn

PHP:  exit(1);
来源：http://ri.huanxung.cn

JS:   process.exit(1)
来源：http://vh.szsharing.cn

TS:   process.exit(1)
来源：http://fo.9csxet.cn

Java: System.exit(1)
来源：http://si.newstarts.cn

Go:   os.Exit(1)
来源：http://hc.nicolike.cn

Ruby: exit 1
来源：http://sf.gzmigu.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://rv.yuexingan06.cn

[M06] 向标准错误输出
来源：http://zf.shtwfgs.cn

Py:   print("err", file=sys.stderr)
来源：http://lb.521024.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://px.huixiangedu.cn

JS:   console.error("err")
来源：http://ih.wgjwhj.cn

TS:   console.error("err")
来源：http://xk.shxzukj.cn

Java: System.err.println("err")
来源：http://qa.shxzukj.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://qy.colortex.cn

Ruby: warn "err"
来源：http://oe.colortex.cn

C#:   Console.Error.WriteLine("err")
来源：http://di.colortex.cn

[M07] 判断是否为主入口
来源：http://eo.nicolike.cn

Py:   if __name__ == "__main__":
来源：http://ym.yuntaijiaju.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://pq.huanxung.cn

JS:   require.main === module
来源：http://cu.lnxyls.cn

TS:   require.main === module
来源：http://hd.newstarts.cn

Java: public static void main(String[] args)
来源：http://cd.jctech888.com.cn

Go:   func main()
来源：http://wv.huixinmuqiang.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://pf.521024.cn

C#:   static void Main(string[] args)
来源：http://wk.newstarts.cn

[M08] 获取系统与运行时信息
来源：http://km.yuntaijiaju.cn

Py:   platform.system();  platform.python_version()
来源：http://bz.shxzukj.cn

PHP:  PHP_OS;  phpversion();
来源：http://hu.jianghongdianzi.cn

JS:   process.platform;  process.version
来源：http://gj.lnxyls.cn

TS:   process.platform;  process.version
来源：http://zq.muxihuayi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ny.bjjhwx.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://xq.hnjuh.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://zb.bjjhwx.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ec.521024.cn

================================================================================
来源：http://na.shtwfgs.cn

N. 数据结构与算法
来源：http://ff.9csxet.cn

================================================================================
来源：http://bl.gzmigu.cn

[N01] 二分查找（有序数组）
来源：http://uj.lnxyls.cn

Py:   bisect.bisect_left(arr, x)
来源：http://vg.gzmigu.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://lb.lnxyls.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gy.hnjuh.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vn.szxytkj.cn

Java: Arrays.binarySearch(arr, x)
来源：http://yi.asd995.cn

Go:   sort.SearchInts(arr, x)
来源：http://hg.huixiangedu.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://tz.jctech888.com.cn

C#:   Array.BinarySearch(arr, x)
来源：http://pm.wgjwhj.cn

[N02] 排序（工程实践用内置实现）
来源：http://ew.asd995.cn

Py:   sorted(arr);  arr.sort()
来源：http://on.panjiajie.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ee.gzmigu.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://yv.lnxyls.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://tj.lnxyls.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://iv.huixiangedu.cn

Go:   slices.Sort(arr)
来源：http://jr.hnjuh.cn

Ruby: arr.sort
来源：http://jb.gzmigu.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://nw.hnjuh.cn

[N03] 快速排序（分治示例）
来源：http://ji.huixiangedu.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://id.yuntaijiaju.cn

PHP:  // 递归实现，或用 usort
来源：http://qs.asd995.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hd.shtwfgs.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ej.jctech888.com.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://xw.shxzukj.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hl.yuexingan06.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://bm.lnxyls.cn

C#:   // 手写递归，或 Array.Sort
来源：http://xw.wgjwhj.cn

[N04] 斐波那契数列
来源：http://xo.521024.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://tw.shxzukj.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://aw.shxzskj.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://io.asd995.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tk.huixiangedu.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://qx.nszjky.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://zn.nszjky.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://fs.panjiajie.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hr.bjjhwx.cn

[N05] 最大公约数
来源：http://vk.lnxyls.cn

Py:   math.gcd(a, b)
来源：http://qa.jctech888.com.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://nr.szsharing.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wc.9csxet.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ja.shtwfgs.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mv.shtwfgs.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ir.colortex.cn

Ruby: a.gcd(b)
来源：http://jy.wgjwhj.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://uo.bjjhwx.cn

[N06] 判断回文字符串
来源：http://ju.newstarts.cn

Py:   s == s[::-1]
来源：http://dm.huixiangedu.cn

PHP:  $s === strrev($s);
来源：http://hr.haigaiapp.cn

JS:   s === [...s].reverse().join("")
来源：http://rh.newstarts.cn

TS:   s === [...s].reverse().join("")
来源：http://wa.gzmigu.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://vb.huixinmuqiang.cn

Go:   // 双指针从两端比较
来源：http://rt.hahajie.cn

Ruby: s == s.reverse
来源：http://cq.bjjhwx.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://wc.colortex.cn

[N07] 两数之和（返回下标）
来源：http://xb.521024.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mv.lnxyls.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://xh.shtwfgs.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://jy.shxzskj.cn

TS:   // 手写 Map<string, number>
来源：http://qg.huixinmuqiang.cn

Java: // 手写 HashMap
来源：http://sx.hahajie.cn

Go:   // 手写 map[int]int
来源：http://ho.hnjuh.cn

Ruby: // 手写 Hash
来源：http://sc.colortex.cn

C#:   // 手写 Dictionary<int, int>
来源：http://rb.nszjky.cn

[N08] 生成全排列
来源：http://hh.nicolike.cn

Py:   itertools.permutations(arr)
来源：http://ls.yuexingan06.cn

PHP:  // 手写递归交换
来源：http://ht.9csxet.cn

JS:   // 手写回溯递归
来源：http://gq.haigaiapp.cn

TS:   // 手写回溯递归
来源：http://at.asd995.cn

Java: // 手写回溯递归
来源：http://sj.chemitech.net.cn

Go:   // 手写回溯递归
来源：http://dq.jctech888.com.cn

Ruby: arr.permutation.to_a
来源：http://fa.lnxyls.cn

C#:   // 手写回溯递归
来源：http://dp.hahajie.cn

[N09] 栈与队列
来源：http://wx.shxzskj.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://tk.huixiangedu.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://he.asd995.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hk.nicolike.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://iv.bjjhwx.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://he.asd995.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://gi.huixinmuqiang.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ny.nicolike.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ya.yuntaijiaju.cn

[N10] 链表节点定义
来源：http://mz.jctech888.com.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://fl.panjiajie.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://lf.nszjky.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://xv.jctech888.com.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://jp.szsharing.cn

Java: class Node { int v; Node next; }
来源：http://zi.haigaiapp.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ti.jctech888.com.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://vb.shxzukj.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ie.yuntaijiaju.cn

[N11] 二叉树中序遍历
来源：http://vt.szsharing.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://qe.yuntaijiaju.cn

PHP:  // 手写递归函数
来源：http://qk.shxzukj.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://st.nszjky.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cm.jctech888.com.cn

Java: // 手写递归
来源：http://sx.9csxet.cn

Go:   // 手写递归
来源：http://kg.shtwfgs.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hv.yuexingan06.cn

C#:   // 手写递归
来源：http://tk.shxzukj.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://xb.521024.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://cm.521024.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://no.shxzskj.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ju.9csxet.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ic.szsharing.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://qm.wgjwhj.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ny.haigaiapp.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ps.chemitech.net.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ws.haigaiapp.cn

================================================================================
来源：http://qd.shxzukj.cn

O. 并发与异步
来源：http://la.muxihuayi.cn

================================================================================
来源：http://qt.haigaiapp.cn

[O01] 启动一个线程
来源：http://mz.huixinmuqiang.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://eg.bookmarksfly.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://vi.gzmigu.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://vt.yuntaijiaju.cn

TS:   // 同 JS
来源：http://eu.huixiangedu.cn

Java: new Thread(() -> f()).start()
来源：http://ww.hahajie.cn

Go:   go f()
来源：http://uz.yuntaijiaju.cn

Ruby: Thread.new { f }
来源：http://nf.newstarts.cn

C#:   Task.Run(() => F());
来源：http://by.hnjuh.cn

[O02] 使用线程池
来源：http://xk.chemitech.net.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://sw.bjjhwx.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://yk.panjiajie.cn

JS:   // worker_threads 线程池
来源：http://uz.yuntaijiaju.cn


<!-- 参考信息 -->