代发 wailian999

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fr.hnjuh.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://da.newstarts.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ee.huixinmuqiang.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://sw.nszjky.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://pr.yuntaijiaju.cn

[K07] 进制转换
来源：http://eq.colortex.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hp.newstarts.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://su.chemitech.net.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://aa.yuntaijiaju.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://fu.yuntaijiaju.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xi.shxzskj.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://at.newstarts.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://cz.nszjky.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hj.panjiajie.cn

[K08] 二进制序列化（非 JSON）
来源：http://xh.jianghongdianzi.cn

Py:   pickle.dumps(obj)
来源：http://hy.nicolike.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://et.jianghongdianzi.cn

JS:   v8.serialize(obj)        // Node
来源：http://ve.521024.cn

TS:   v8.serialize(obj)        // Node
来源：http://hy.newstarts.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://xo.gzmigu.cn

Go:   encoding/gob
来源：http://nb.yuntaijiaju.cn

Ruby: Marshal.dump(obj)
来源：http://yo.shxzukj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://rc.haigaiapp.cn

================================================================================
来源：http://jg.jctech888.com.cn

L. 网络请求
来源：http://sf.jianghongdianzi.cn

================================================================================
来源：http://vu.gzmigu.cn

[L01] 发送 GET 请求
来源：http://bd.yuntaijiaju.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://in.9csxet.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://lc.521024.cn

JS:   await fetch(url)
来源：http://os.jianghongdianzi.cn

TS:   await fetch(url)
来源：http://if.9csxet.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://nf.huixiangedu.cn

Go:   resp, err := http.Get(url)
来源：http://cu.hahajie.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://tz.yuexingan06.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ps.jianghongdianzi.cn

[L02] 发送 POST JSON
来源：http://fu.jianghongdianzi.cn

Py:   requests.post(url, json={"a": 1})
来源：http://qc.nicolike.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hq.521024.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://in.huixiangedu.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gy.hnjuh.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://sy.lnxyls.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ls.huixinmuqiang.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://fg.shxzskj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://jh.szsharing.cn

[L03] 设置自定义请求头
来源：http://rh.haigaiapp.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://la.huixiangedu.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://gl.9csxet.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pz.colortex.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://oa.newstarts.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://st.asd995.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://eg.chemitech.net.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ny.shxzskj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://la.szxytkj.cn

[L04] 设置超时
来源：http://mu.wgjwhj.cn

Py:   requests.get(url, timeout=5)
来源：http://zv.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://pr.shxzskj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qw.9csxet.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ih.newstarts.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://lz.hahajie.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://qf.bookmarksfly.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://si.asd995.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://am.panjiajie.cn

[L05] 上传文件（multipart）
来源：http://xe.panjiajie.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ls.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://iy.shxzukj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://dy.haigaiapp.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://so.gzmigu.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wu.bjjhwx.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://bk.lnxyls.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://bh.lnxyls.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ty.shxzukj.cn

[L06] 解析响应为 JSON
来源：http://dk.jianghongdianzi.cn

Py:   resp.json()
来源：http://ae.muxihuayi.cn

PHP:  json_decode($body, true);
来源：http://ey.521024.cn

JS:   await resp.json()
来源：http://yn.yuexingan06.cn

TS:   await resp.json()
来源：http://iu.newstarts.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://lh.bookmarksfly.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wa.yuexingan06.cn

Ruby: JSON.parse(resp.body)
来源：http://ga.szxytkj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://cm.wgjwhj.cn

[L07] 处理 HTTP 状态码
来源：http://oq.nszjky.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://lx.521024.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://yh.haigaiapp.cn

JS:   resp.ok;  resp.status
来源：http://xi.szxytkj.cn

TS:   resp.ok;  resp.status
来源：http://or.szsharing.cn

Java: resp.statusCode()
来源：http://fz.shxzskj.cn

Go:   resp.StatusCode
来源：http://df.yuexingan06.cn

Ruby: resp.code.to_i
来源：http://bv.haigaiapp.cn

C#:   (int)resp.StatusCode
来源：http://mo.lnxyls.cn

[L08] 并发请求多个地址
来源：http://ir.bjjhwx.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hg.newstarts.cn

PHP:  curl_multi_init() 系列
来源：http://wu.shtwfgs.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pz.yuntaijiaju.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wm.wgjwhj.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://nm.521024.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hi.bookmarksfly.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://nc.shxzukj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://br.shtwfgs.cn

================================================================================
来源：http://ua.szsharing.cn

M. 命令行 / 进程 / 环境
来源：http://uy.jctech888.com.cn

================================================================================
来源：http://lm.szsharing.cn

[M01] 读取命令行参数
来源：http://eg.9csxet.cn

Py:   sys.argv[1:]
来源：http://bv.yuntaijiaju.cn

PHP:  $argv;  $argc;
来源：http://lt.shxzukj.cn

JS:   process.argv.slice(2)
来源：http://ow.nszjky.cn

TS:   process.argv.slice(2)
来源：http://qr.nszjky.cn

Java: args 数组（main 方法参数）
来源：http://hm.szsharing.cn

Go:   os.Args[1:]
来源：http://hm.asd995.cn

Ruby: ARGV
来源：http://tb.chemitech.net.cn

C#:   args 数组（Main 方法参数）
来源：http://jw.shxzukj.cn

[M02] 读取环境变量
来源：http://qa.szsharing.cn

Py:   os.environ.get("HOME")
来源：http://nv.colortex.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ho.huixiangedu.cn

JS:   process.env.HOME
来源：http://se.huixinmuqiang.cn

TS:   process.env.HOME
来源：http://jw.shtwfgs.cn

Java: System.getenv("HOME")
来源：http://rf.huanxung.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://iw.yuntaijiaju.cn

Ruby: ENV["HOME"]
来源：http://jw.shxzskj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://qx.yuexingan06.cn

[M03] 执行外部命令
来源：http://pu.gzmigu.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://zr.gzmigu.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://el.asd995.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://jb.hahajie.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://iy.chemitech.net.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://sg.nicolike.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://fk.newstarts.cn

Ruby: system("ls -l");  `ls -l`
来源：http://nk.nicolike.cn

C#:   Process.Start("ls", "-l");
来源：http://op.muxihuayi.cn

[M04] 获取当前工作目录
来源：http://xs.9csxet.cn

Py:   os.getcwd()
来源：http://uj.shxzukj.cn

PHP:  getcwd();
来源：http://ai.huixinmuqiang.cn

JS:   process.cwd()
来源：http://ol.szxytkj.cn

TS:   process.cwd()
来源：http://sj.asd995.cn

Java: Path.of("").toAbsolutePath()
来源：http://qw.bjjhwx.cn

Go:   os.Getwd()
来源：http://cj.hahajie.cn

Ruby: Dir.pwd
来源：http://sg.9csxet.cn

C#:   Directory.GetCurrentDirectory()
来源：http://mx.hnjuh.cn

[M05] 设置退出码
来源：http://ns.muxihuayi.cn

Py:   sys.exit(1)
来源：http://dm.huanxung.cn

PHP:  exit(1);
来源：http://uo.szsharing.cn

JS:   process.exit(1)
来源：http://jd.hahajie.cn

TS:   process.exit(1)
来源：http://se.hahajie.cn

Java: System.exit(1)
来源：http://kg.colortex.cn

Go:   os.Exit(1)
来源：http://av.huanxung.cn

Ruby: exit 1
来源：http://id.huanxung.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ha.huanxung.cn

[M06] 向标准错误输出
来源：http://dv.bookmarksfly.cn

Py:   print("err", file=sys.stderr)
来源：http://nl.9csxet.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://qx.521024.cn

JS:   console.error("err")
来源：http://li.szxytkj.cn

TS:   console.error("err")
来源：http://kb.muxihuayi.cn

Java: System.err.println("err")
来源：http://re.huanxung.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://qn.gzmigu.cn

Ruby: warn "err"
来源：http://vu.jianghongdianzi.cn

C#:   Console.Error.WriteLine("err")
来源：http://mf.521024.cn

[M07] 判断是否为主入口
来源：http://qf.panjiajie.cn

Py:   if __name__ == "__main__":
来源：http://sq.9csxet.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ra.9csxet.cn

JS:   require.main === module
来源：http://dg.shxzukj.cn

TS:   require.main === module
来源：http://kw.shxzukj.cn

Java: public static void main(String[] args)
来源：http://uu.yuexingan06.cn

Go:   func main()
来源：http://br.huixiangedu.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://pe.jianghongdianzi.cn

C#:   static void Main(string[] args)
来源：http://xd.newstarts.cn

[M08] 获取系统与运行时信息
来源：http://vd.hahajie.cn

Py:   platform.system();  platform.python_version()
来源：http://ul.yuexingan06.cn

PHP:  PHP_OS;  phpversion();
来源：http://wt.521024.cn

JS:   process.platform;  process.version
来源：http://wl.521024.cn

TS:   process.platform;  process.version
来源：http://xw.szxytkj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://yx.szxytkj.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ek.yuexingan06.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://yy.lnxyls.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ol.yuntaijiaju.cn

================================================================================
来源：http://mg.521024.cn

N. 数据结构与算法
来源：http://mq.newstarts.cn

================================================================================
来源：http://kh.haigaiapp.cn

[N01] 二分查找（有序数组）
来源：http://wp.colortex.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ix.shtwfgs.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ju.shxzskj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://by.hnjuh.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sv.nszjky.cn

Java: Arrays.binarySearch(arr, x)
来源：http://bt.szxytkj.cn

Go:   sort.SearchInts(arr, x)
来源：http://vq.wgjwhj.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://wz.hahajie.cn

C#:   Array.BinarySearch(arr, x)
来源：http://kz.hnjuh.cn

[N02] 排序（工程实践用内置实现）
来源：http://bs.gzmigu.cn

Py:   sorted(arr);  arr.sort()
来源：http://mf.muxihuayi.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ub.szxytkj.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://rl.huixiangedu.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://hx.huixinmuqiang.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wt.asd995.cn

Go:   slices.Sort(arr)
来源：http://nj.lnxyls.cn

Ruby: arr.sort
来源：http://yn.wgjwhj.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://pq.wgjwhj.cn

[N03] 快速排序（分治示例）
来源：http://gx.yuntaijiaju.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://du.shtwfgs.cn

PHP:  // 递归实现，或用 usort
来源：http://er.shxzskj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://iv.chemitech.net.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mp.haigaiapp.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://iq.colortex.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ve.colortex.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ib.jianghongdianzi.cn

C#:   // 手写递归，或 Array.Sort
来源：http://nq.gzmigu.cn

[N04] 斐波那契数列
来源：http://mf.colortex.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://jw.nicolike.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://uy.shtwfgs.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pr.hahajie.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kq.newstarts.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wh.jctech888.com.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://sb.chemitech.net.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://tu.haigaiapp.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ka.haigaiapp.cn

[N05] 最大公约数
来源：http://ij.haigaiapp.cn

Py:   math.gcd(a, b)
来源：http://ud.jianghongdianzi.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hq.haigaiapp.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://go.hahajie.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://va.shtwfgs.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://to.haigaiapp.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://xj.wgjwhj.cn

Ruby: a.gcd(b)
来源：http://sb.huixiangedu.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://tx.wgjwhj.cn

[N06] 判断回文字符串
来源：http://eq.gzmigu.cn

Py:   s == s[::-1]
来源：http://yf.lnxyls.cn

PHP:  $s === strrev($s);
来源：http://zr.nicolike.cn

JS:   s === [...s].reverse().join("")
来源：http://vd.colortex.cn

TS:   s === [...s].reverse().join("")
来源：http://lo.szsharing.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://vc.jctech888.com.cn

Go:   // 双指针从两端比较
来源：http://da.jianghongdianzi.cn

Ruby: s == s.reverse
来源：http://qa.yuntaijiaju.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ev.huixinmuqiang.cn

[N07] 两数之和（返回下标）
来源：http://lu.nszjky.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://eu.asd995.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://pa.jianghongdianzi.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://bo.shxzskj.cn

TS:   // 手写 Map<string, number>
来源：http://ny.jianghongdianzi.cn

Java: // 手写 HashMap
来源：http://ka.huixiangedu.cn

Go:   // 手写 map[int]int
来源：http://te.shxzukj.cn

Ruby: // 手写 Hash
来源：http://ne.hahajie.cn

C#:   // 手写 Dictionary<int, int>
来源：http://vq.szxytkj.cn

[N08] 生成全排列
来源：http://lv.hahajie.cn

Py:   itertools.permutations(arr)
来源：http://jo.hahajie.cn

PHP:  // 手写递归交换
来源：http://lk.asd995.cn

JS:   // 手写回溯递归
来源：http://hw.jianghongdianzi.cn

TS:   // 手写回溯递归
来源：http://pi.9csxet.cn

Java: // 手写回溯递归
来源：http://bz.panjiajie.cn

Go:   // 手写回溯递归
来源：http://cp.bookmarksfly.cn

Ruby: arr.permutation.to_a
来源：http://nd.yuexingan06.cn

C#:   // 手写回溯递归
来源：http://dm.chemitech.net.cn

[N09] 栈与队列
来源：http://zk.yuexingan06.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://lz.asd995.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ny.szsharing.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://nu.shxzukj.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mc.shxzukj.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://nc.shtwfgs.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://bd.asd995.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://fd.yuexingan06.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://bn.wgjwhj.cn

[N10] 链表节点定义
来源：http://xb.jianghongdianzi.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://xx.bookmarksfly.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://jr.huanxung.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://xy.shxzukj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://dn.huanxung.cn

Java: class Node { int v; Node next; }
来源：http://lu.gzmigu.cn

Go:   type Node struct { V int; Next *Node }
来源：http://sh.szsharing.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://sl.asd995.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://wq.lnxyls.cn

[N11] 二叉树中序遍历
来源：http://ja.chemitech.net.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ud.521024.cn

PHP:  // 手写递归函数
来源：http://qm.huixiangedu.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fi.9csxet.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dk.huanxung.cn

Java: // 手写递归
来源：http://ks.gzmigu.cn

Go:   // 手写递归
来源：http://mc.gzmigu.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://aw.hnjuh.cn

C#:   // 手写递归
来源：http://wg.colortex.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://zb.shtwfgs.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hj.panjiajie.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://iu.bookmarksfly.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jc.jctech888.com.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://az.szxytkj.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://vq.muxihuayi.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hc.chemitech.net.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ep.hahajie.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://yn.yuntaijiaju.cn

================================================================================
来源：http://yz.gzmigu.cn

O. 并发与异步
来源：http://gy.jianghongdianzi.cn

================================================================================
来源：http://dr.muxihuayi.cn

[O01] 启动一个线程
来源：http://nb.jctech888.com.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://nd.nszjky.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://do.asd995.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://dg.lnxyls.cn

TS:   // 同 JS
来源：http://ob.jctech888.com.cn

Java: new Thread(() -> f()).start()
来源：http://hq.szxytkj.cn

Go:   go f()
来源：http://xv.hahajie.cn

Ruby: Thread.new { f }
来源：http://rr.chemitech.net.cn

C#:   Task.Run(() => F());
来源：http://om.szsharing.cn

[O02] 使用线程池
来源：http://qg.bookmarksfly.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://kv.colortex.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ej.hahajie.cn

JS:   // worker_threads 线程池
来源：http://lm.shxzskj.cn


<!-- 参考信息 -->