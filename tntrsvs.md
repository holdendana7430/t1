代发 wailian999

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nf.521024.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://sd.szsharing.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://cn.nicolike.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://gn.haigaiapp.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ls.yuexingan06.cn

[K07] 进制转换
来源：http://fl.muxihuayi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hs.nicolike.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://yc.bjjhwx.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://lp.muxihuayi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://su.huixinmuqiang.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://uz.szsharing.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ae.yuntaijiaju.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mm.bjjhwx.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://rm.wgjwhj.cn

[K08] 二进制序列化（非 JSON）
来源：http://ox.nicolike.cn

Py:   pickle.dumps(obj)
来源：http://yz.hahajie.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://mm.newstarts.cn

JS:   v8.serialize(obj)        // Node
来源：http://gd.hnjuh.cn

TS:   v8.serialize(obj)        // Node
来源：http://dt.newstarts.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://fe.szxytkj.cn

Go:   encoding/gob
来源：http://dv.chemitech.net.cn

Ruby: Marshal.dump(obj)
来源：http://wz.muxihuayi.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://li.wgjwhj.cn

================================================================================
来源：http://pc.wgjwhj.cn

L. 网络请求
来源：http://qs.muxihuayi.cn

================================================================================
来源：http://es.nszjky.cn

[L01] 发送 GET 请求
来源：http://ld.gzmigu.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://sz.nicolike.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://cx.jianghongdianzi.cn

JS:   await fetch(url)
来源：http://ih.szxytkj.cn

TS:   await fetch(url)
来源：http://hb.nszjky.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ec.colortex.cn

Go:   resp, err := http.Get(url)
来源：http://xq.wgjwhj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ro.shxzukj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://de.shtwfgs.cn

[L02] 发送 POST JSON
来源：http://ac.jctech888.com.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ij.shtwfgs.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://at.yuexingan06.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fj.lnxyls.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yv.szsharing.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://rv.shxzskj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://fu.521024.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://dc.colortex.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://qy.hahajie.cn

[L03] 设置自定义请求头
来源：http://gb.szxytkj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://zv.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://on.yuexingan06.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rm.hnjuh.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dk.jianghongdianzi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://fe.hnjuh.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://dd.huanxung.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://io.nicolike.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://bu.hahajie.cn

[L04] 设置超时
来源：http://ym.shtwfgs.cn

Py:   requests.get(url, timeout=5)
来源：http://oj.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ig.haigaiapp.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ln.haigaiapp.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dp.bjjhwx.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://zb.muxihuayi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mz.nicolike.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ou.wgjwhj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ou.huixiangedu.cn

[L05] 上传文件（multipart）
来源：http://ab.gzmigu.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://xz.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://sn.panjiajie.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gv.muxihuayi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ih.hnjuh.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://cf.wgjwhj.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ug.panjiajie.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://aj.huixinmuqiang.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://tg.lnxyls.cn

[L06] 解析响应为 JSON
来源：http://vs.lnxyls.cn

Py:   resp.json()
来源：http://yf.bookmarksfly.cn

PHP:  json_decode($body, true);
来源：http://us.panjiajie.cn

JS:   await resp.json()
来源：http://az.gzmigu.cn

TS:   await resp.json()
来源：http://ev.yuntaijiaju.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ij.muxihuayi.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://kv.haigaiapp.cn

Ruby: JSON.parse(resp.body)
来源：http://bk.bookmarksfly.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://cr.huixinmuqiang.cn

[L07] 处理 HTTP 状态码
来源：http://ht.haigaiapp.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://to.huanxung.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://kn.521024.cn

JS:   resp.ok;  resp.status
来源：http://um.muxihuayi.cn

TS:   resp.ok;  resp.status
来源：http://os.hahajie.cn

Java: resp.statusCode()
来源：http://gv.muxihuayi.cn

Go:   resp.StatusCode
来源：http://cm.shxzskj.cn

Ruby: resp.code.to_i
来源：http://zq.hnjuh.cn

C#:   (int)resp.StatusCode
来源：http://kp.hnjuh.cn

[L08] 并发请求多个地址
来源：http://ze.jctech888.com.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mq.newstarts.cn

PHP:  curl_multi_init() 系列
来源：http://ar.nicolike.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hv.huixiangedu.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vk.jctech888.com.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mj.bookmarksfly.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://to.huixiangedu.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hd.shtwfgs.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://na.jianghongdianzi.cn

================================================================================
来源：http://le.szsharing.cn

M. 命令行 / 进程 / 环境
来源：http://qg.szsharing.cn

================================================================================
来源：http://dv.hnjuh.cn

[M01] 读取命令行参数
来源：http://xb.521024.cn

Py:   sys.argv[1:]
来源：http://oj.newstarts.cn

PHP:  $argv;  $argc;
来源：http://ce.huanxung.cn

JS:   process.argv.slice(2)
来源：http://es.lnxyls.cn

TS:   process.argv.slice(2)
来源：http://zx.hnjuh.cn

Java: args 数组（main 方法参数）
来源：http://fx.nicolike.cn

Go:   os.Args[1:]
来源：http://kw.bjjhwx.cn

Ruby: ARGV
来源：http://gu.bjjhwx.cn

C#:   args 数组（Main 方法参数）
来源：http://tw.chemitech.net.cn

[M02] 读取环境变量
来源：http://ef.nicolike.cn

Py:   os.environ.get("HOME")
来源：http://zu.jctech888.com.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://av.9csxet.cn

JS:   process.env.HOME
来源：http://kh.shtwfgs.cn

TS:   process.env.HOME
来源：http://fo.9csxet.cn

Java: System.getenv("HOME")
来源：http://xh.nszjky.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://lx.gzmigu.cn

Ruby: ENV["HOME"]
来源：http://xe.jianghongdianzi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://en.szxytkj.cn

[M03] 执行外部命令
来源：http://qe.hahajie.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ty.szxytkj.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zy.panjiajie.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://gv.szxytkj.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://xg.nszjky.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ls.chemitech.net.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://pe.newstarts.cn

Ruby: system("ls -l");  `ls -l`
来源：http://uo.shtwfgs.cn

C#:   Process.Start("ls", "-l");
来源：http://zf.bjjhwx.cn

[M04] 获取当前工作目录
来源：http://kf.wgjwhj.cn

Py:   os.getcwd()
来源：http://vt.wgjwhj.cn

PHP:  getcwd();
来源：http://af.bjjhwx.cn

JS:   process.cwd()
来源：http://kp.bjjhwx.cn

TS:   process.cwd()
来源：http://vl.yuexingan06.cn

Java: Path.of("").toAbsolutePath()
来源：http://ns.shtwfgs.cn

Go:   os.Getwd()
来源：http://fm.hahajie.cn

Ruby: Dir.pwd
来源：http://ek.bjjhwx.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ml.muxihuayi.cn

[M05] 设置退出码
来源：http://wf.chemitech.net.cn

Py:   sys.exit(1)
来源：http://yl.colortex.cn

PHP:  exit(1);
来源：http://zo.wgjwhj.cn

JS:   process.exit(1)
来源：http://uq.yuexingan06.cn

TS:   process.exit(1)
来源：http://li.colortex.cn

Java: System.exit(1)
来源：http://aw.szsharing.cn

Go:   os.Exit(1)
来源：http://cm.shtwfgs.cn

Ruby: exit 1
来源：http://za.hahajie.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://yq.szxytkj.cn

[M06] 向标准错误输出
来源：http://ga.hnjuh.cn

Py:   print("err", file=sys.stderr)
来源：http://gu.huanxung.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://vs.hahajie.cn

JS:   console.error("err")
来源：http://aw.muxihuayi.cn

TS:   console.error("err")
来源：http://rg.muxihuayi.cn

Java: System.err.println("err")
来源：http://bt.bookmarksfly.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://xv.haigaiapp.cn

Ruby: warn "err"
来源：http://vi.shxzskj.cn

C#:   Console.Error.WriteLine("err")
来源：http://sk.jianghongdianzi.cn

[M07] 判断是否为主入口
来源：http://xr.bookmarksfly.cn

Py:   if __name__ == "__main__":
来源：http://hl.newstarts.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://fo.newstarts.cn

JS:   require.main === module
来源：http://ii.lnxyls.cn

TS:   require.main === module
来源：http://xd.szxytkj.cn

Java: public static void main(String[] args)
来源：http://sm.9csxet.cn

Go:   func main()
来源：http://yq.jianghongdianzi.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wp.szxytkj.cn

C#:   static void Main(string[] args)
来源：http://cw.521024.cn

[M08] 获取系统与运行时信息
来源：http://sy.huixinmuqiang.cn

Py:   platform.system();  platform.python_version()
来源：http://nv.newstarts.cn

PHP:  PHP_OS;  phpversion();
来源：http://vf.nszjky.cn

JS:   process.platform;  process.version
来源：http://qc.colortex.cn

TS:   process.platform;  process.version
来源：http://ls.haigaiapp.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://jl.jianghongdianzi.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://kj.bjjhwx.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://uc.521024.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://gm.wgjwhj.cn

================================================================================
来源：http://sp.haigaiapp.cn

N. 数据结构与算法
来源：http://iu.jctech888.com.cn

================================================================================
来源：http://xt.chemitech.net.cn

[N01] 二分查找（有序数组）
来源：http://sw.gzmigu.cn

Py:   bisect.bisect_left(arr, x)
来源：http://sv.bookmarksfly.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ce.bookmarksfly.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://oy.newstarts.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dd.9csxet.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ug.szxytkj.cn

Go:   sort.SearchInts(arr, x)
来源：http://xn.nszjky.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://cb.yuexingan06.cn

C#:   Array.BinarySearch(arr, x)
来源：http://wo.panjiajie.cn

[N02] 排序（工程实践用内置实现）
来源：http://sq.huixinmuqiang.cn

Py:   sorted(arr);  arr.sort()
来源：http://rd.szsharing.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://lt.huanxung.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ho.jianghongdianzi.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://sx.hnjuh.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://kr.521024.cn

Go:   slices.Sort(arr)
来源：http://dn.gzmigu.cn

Ruby: arr.sort
来源：http://yb.hnjuh.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://kn.lnxyls.cn

[N03] 快速排序（分治示例）
来源：http://xr.shxzskj.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://zo.panjiajie.cn

PHP:  // 递归实现，或用 usort
来源：http://tl.9csxet.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mf.huixiangedu.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ii.huixiangedu.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mf.jianghongdianzi.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://zs.wgjwhj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wm.shtwfgs.cn

C#:   // 手写递归，或 Array.Sort
来源：http://vy.9csxet.cn

[N04] 斐波那契数列
来源：http://ya.huixiangedu.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://vp.szsharing.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://dl.nszjky.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qc.asd995.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wj.hnjuh.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://gq.hahajie.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://yw.haigaiapp.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://yj.gzmigu.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hy.huixiangedu.cn

[N05] 最大公约数
来源：http://nq.asd995.cn

Py:   math.gcd(a, b)
来源：http://ow.wgjwhj.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://db.lnxyls.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ka.newstarts.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ol.9csxet.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ys.panjiajie.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://oz.nicolike.cn

Ruby: a.gcd(b)
来源：http://dm.jctech888.com.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ss.huixinmuqiang.cn

[N06] 判断回文字符串
来源：http://mc.szsharing.cn

Py:   s == s[::-1]
来源：http://bi.hahajie.cn

PHP:  $s === strrev($s);
来源：http://lj.chemitech.net.cn

JS:   s === [...s].reverse().join("")
来源：http://qy.nicolike.cn

TS:   s === [...s].reverse().join("")
来源：http://nl.jctech888.com.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://gj.gzmigu.cn

Go:   // 双指针从两端比较
来源：http://li.huixinmuqiang.cn

Ruby: s == s.reverse
来源：http://ck.yuexingan06.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://yl.colortex.cn

[N07] 两数之和（返回下标）
来源：http://hy.haigaiapp.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://dj.colortex.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jn.hnjuh.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://bo.lnxyls.cn

TS:   // 手写 Map<string, number>
来源：http://je.muxihuayi.cn

Java: // 手写 HashMap
来源：http://rs.yuntaijiaju.cn

Go:   // 手写 map[int]int
来源：http://pu.yuntaijiaju.cn

Ruby: // 手写 Hash
来源：http://in.lnxyls.cn

C#:   // 手写 Dictionary<int, int>
来源：http://xj.huanxung.cn

[N08] 生成全排列
来源：http://cs.haigaiapp.cn

Py:   itertools.permutations(arr)
来源：http://rd.wgjwhj.cn

PHP:  // 手写递归交换
来源：http://qe.huixiangedu.cn

JS:   // 手写回溯递归
来源：http://zf.521024.cn

TS:   // 手写回溯递归
来源：http://kp.nszjky.cn

Java: // 手写回溯递归
来源：http://ht.nicolike.cn

Go:   // 手写回溯递归
来源：http://nn.lnxyls.cn

Ruby: arr.permutation.to_a
来源：http://vl.bookmarksfly.cn

C#:   // 手写回溯递归
来源：http://vg.colortex.cn

[N09] 栈与队列
来源：http://zy.jianghongdianzi.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://rc.hnjuh.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mm.huanxung.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://bp.lnxyls.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://li.huixiangedu.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://cv.nszjky.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://yg.hnjuh.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://jb.lnxyls.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://uf.asd995.cn

[N10] 链表节点定义
来源：http://is.lnxyls.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://bg.szxytkj.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ey.shtwfgs.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://nj.lnxyls.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://dy.jctech888.com.cn

Java: class Node { int v; Node next; }
来源：http://ae.haigaiapp.cn

Go:   type Node struct { V int; Next *Node }
来源：http://el.jctech888.com.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://rn.gzmigu.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://qd.yuntaijiaju.cn

[N11] 二叉树中序遍历
来源：http://wz.shxzukj.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://yw.colortex.cn

PHP:  // 手写递归函数
来源：http://op.szsharing.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ux.9csxet.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://um.szxytkj.cn

Java: // 手写递归
来源：http://zu.nszjky.cn

Go:   // 手写递归
来源：http://ws.9csxet.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://we.chemitech.net.cn

C#:   // 手写递归
来源：http://po.asd995.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://et.521024.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://uj.wgjwhj.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://rs.lnxyls.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ck.hahajie.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fp.asd995.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://nw.9csxet.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://kp.nszjky.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://em.gzmigu.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://he.muxihuayi.cn

================================================================================
来源：http://di.yuntaijiaju.cn

O. 并发与异步
来源：http://he.asd995.cn

================================================================================
来源：http://sr.shtwfgs.cn

[O01] 启动一个线程
来源：http://yp.huixiangedu.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hm.shxzukj.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://al.muxihuayi.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://pz.muxihuayi.cn

TS:   // 同 JS
来源：http://qh.huixiangedu.cn

Java: new Thread(() -> f()).start()
来源：http://hh.newstarts.cn

Go:   go f()
来源：http://ix.bookmarksfly.cn

Ruby: Thread.new { f }
来源：http://am.yuntaijiaju.cn

C#:   Task.Run(() => F());
来源：http://mq.gzmigu.cn

[O02] 使用线程池
来源：http://px.gzmigu.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://nm.szxytkj.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://zd.haigaiapp.cn

JS:   // worker_threads 线程池
来源：http://ak.hahajie.cn


<!-- 参考信息 -->