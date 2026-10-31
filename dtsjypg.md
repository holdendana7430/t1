代发 wailian999

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dx.panjiajie.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://fe.jianghongdianzi.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ll.gzmigu.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://le.haigaiapp.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://vy.muxihuayi.cn

[K07] 进制转换
来源：http://bq.yuntaijiaju.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://db.yuexingan06.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://pk.nicolike.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://it.jctech888.com.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://fw.shxzskj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://kj.shxzskj.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://cw.asd995.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ty.colortex.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://zg.szxytkj.cn

[K08] 二进制序列化（非 JSON）
来源：http://yi.gzmigu.cn

Py:   pickle.dumps(obj)
来源：http://hc.nicolike.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://cl.jctech888.com.cn

JS:   v8.serialize(obj)        // Node
来源：http://dd.wgjwhj.cn

TS:   v8.serialize(obj)        // Node
来源：http://hv.huanxung.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://bq.asd995.cn

Go:   encoding/gob
来源：http://oj.huixiangedu.cn

Ruby: Marshal.dump(obj)
来源：http://tp.huanxung.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ey.huixiangedu.cn

================================================================================
来源：http://ns.chemitech.net.cn

L. 网络请求
来源：http://bm.jctech888.com.cn

================================================================================
来源：http://hy.521024.cn

[L01] 发送 GET 请求
来源：http://sd.9csxet.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ws.nszjky.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://at.hahajie.cn

JS:   await fetch(url)
来源：http://pv.szsharing.cn

TS:   await fetch(url)
来源：http://to.huanxung.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://gt.chemitech.net.cn

Go:   resp, err := http.Get(url)
来源：http://wy.nszjky.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ch.hahajie.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://os.haigaiapp.cn

[L02] 发送 POST JSON
来源：http://du.chemitech.net.cn

Py:   requests.post(url, json={"a": 1})
来源：http://zx.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://nq.yuexingan06.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vo.newstarts.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ly.chemitech.net.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://kb.huixinmuqiang.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://xc.huanxung.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ah.colortex.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://cb.asd995.cn

[L03] 设置自定义请求头
来源：http://ca.jctech888.com.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mo.521024.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hr.muxihuayi.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ul.huanxung.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wx.hnjuh.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://tb.bookmarksfly.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://bt.nszjky.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://us.shxzskj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://eg.nszjky.cn

[L04] 设置超时
来源：http://di.hahajie.cn

Py:   requests.get(url, timeout=5)
来源：http://rr.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://os.huixiangedu.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ji.asd995.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lg.hnjuh.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://su.szxytkj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.panjiajie.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ls.newstarts.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ug.9csxet.cn

[L05] 上传文件（multipart）
来源：http://hz.colortex.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://vz.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://zs.szxytkj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://zi.panjiajie.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://pz.szxytkj.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mj.huixiangedu.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ks.jctech888.com.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ke.hnjuh.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://dk.haigaiapp.cn

[L06] 解析响应为 JSON
来源：http://km.szxytkj.cn

Py:   resp.json()
来源：http://tv.9csxet.cn

PHP:  json_decode($body, true);
来源：http://cn.bookmarksfly.cn

JS:   await resp.json()
来源：http://is.shtwfgs.cn

TS:   await resp.json()
来源：http://mo.shxzukj.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://tq.shxzskj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://vz.szxytkj.cn

Ruby: JSON.parse(resp.body)
来源：http://sj.huixiangedu.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://rh.lnxyls.cn

[L07] 处理 HTTP 状态码
来源：http://bw.jianghongdianzi.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hy.shtwfgs.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ak.nszjky.cn

JS:   resp.ok;  resp.status
来源：http://sh.wgjwhj.cn

TS:   resp.ok;  resp.status
来源：http://ha.huixinmuqiang.cn

Java: resp.statusCode()
来源：http://mt.wgjwhj.cn

Go:   resp.StatusCode
来源：http://eb.haigaiapp.cn

Ruby: resp.code.to_i
来源：http://tv.haigaiapp.cn

C#:   (int)resp.StatusCode
来源：http://mf.haigaiapp.cn

[L08] 并发请求多个地址
来源：http://uh.panjiajie.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://sm.hnjuh.cn

PHP:  curl_multi_init() 系列
来源：http://td.shxzukj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hm.yuexingan06.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wp.chemitech.net.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hi.newstarts.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://dl.nszjky.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://qn.chemitech.net.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://jk.jctech888.com.cn

================================================================================
来源：http://bj.jianghongdianzi.cn

M. 命令行 / 进程 / 环境
来源：http://kf.huixinmuqiang.cn

================================================================================
来源：http://xj.hahajie.cn

[M01] 读取命令行参数
来源：http://zm.gzmigu.cn

Py:   sys.argv[1:]
来源：http://bv.yuexingan06.cn

PHP:  $argv;  $argc;
来源：http://zf.shtwfgs.cn

JS:   process.argv.slice(2)
来源：http://wt.yuexingan06.cn

TS:   process.argv.slice(2)
来源：http://mt.bookmarksfly.cn

Java: args 数组（main 方法参数）
来源：http://sv.nszjky.cn

Go:   os.Args[1:]
来源：http://br.shxzukj.cn

Ruby: ARGV
来源：http://qs.nszjky.cn

C#:   args 数组（Main 方法参数）
来源：http://iz.shxzskj.cn

[M02] 读取环境变量
来源：http://dr.nszjky.cn

Py:   os.environ.get("HOME")
来源：http://sc.9csxet.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zv.huixinmuqiang.cn

JS:   process.env.HOME
来源：http://vr.bjjhwx.cn

TS:   process.env.HOME
来源：http://kt.panjiajie.cn

Java: System.getenv("HOME")
来源：http://iw.shtwfgs.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://pv.huanxung.cn

Ruby: ENV["HOME"]
来源：http://wr.nicolike.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://bo.yuexingan06.cn

[M03] 执行外部命令
来源：http://su.nszjky.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://gs.huixiangedu.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://id.gzmigu.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ti.muxihuayi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://cw.asd995.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ct.panjiajie.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ms.colortex.cn

Ruby: system("ls -l");  `ls -l`
来源：http://pq.szxytkj.cn

C#:   Process.Start("ls", "-l");
来源：http://at.colortex.cn

[M04] 获取当前工作目录
来源：http://om.521024.cn

Py:   os.getcwd()
来源：http://sl.bookmarksfly.cn

PHP:  getcwd();
来源：http://ut.asd995.cn

JS:   process.cwd()
来源：http://cn.chemitech.net.cn

TS:   process.cwd()
来源：http://ya.muxihuayi.cn

Java: Path.of("").toAbsolutePath()
来源：http://yu.huixinmuqiang.cn

Go:   os.Getwd()
来源：http://fi.hahajie.cn

Ruby: Dir.pwd
来源：http://pa.nicolike.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ms.hnjuh.cn

[M05] 设置退出码
来源：http://dm.huanxung.cn

Py:   sys.exit(1)
来源：http://ab.bjjhwx.cn

PHP:  exit(1);
来源：http://xy.huixinmuqiang.cn

JS:   process.exit(1)
来源：http://uf.gzmigu.cn

TS:   process.exit(1)
来源：http://km.huanxung.cn

Java: System.exit(1)
来源：http://pd.szxytkj.cn

Go:   os.Exit(1)
来源：http://gl.shtwfgs.cn

Ruby: exit 1
来源：http://sk.yuntaijiaju.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://zd.yuntaijiaju.cn

[M06] 向标准错误输出
来源：http://xs.nicolike.cn

Py:   print("err", file=sys.stderr)
来源：http://jh.hnjuh.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://zl.9csxet.cn

JS:   console.error("err")
来源：http://gi.jianghongdianzi.cn

TS:   console.error("err")
来源：http://ik.hahajie.cn

Java: System.err.println("err")
来源：http://ze.hahajie.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ma.jianghongdianzi.cn

Ruby: warn "err"
来源：http://qr.nszjky.cn

C#:   Console.Error.WriteLine("err")
来源：http://et.9csxet.cn

[M07] 判断是否为主入口
来源：http://pl.shtwfgs.cn

Py:   if __name__ == "__main__":
来源：http://cc.haigaiapp.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://np.gzmigu.cn

JS:   require.main === module
来源：http://hf.szxytkj.cn

TS:   require.main === module
来源：http://rn.lnxyls.cn

Java: public static void main(String[] args)
来源：http://mq.521024.cn

Go:   func main()
来源：http://fs.jianghongdianzi.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ks.muxihuayi.cn

C#:   static void Main(string[] args)
来源：http://kn.hnjuh.cn

[M08] 获取系统与运行时信息
来源：http://kf.bookmarksfly.cn

Py:   platform.system();  platform.python_version()
来源：http://ov.haigaiapp.cn

PHP:  PHP_OS;  phpversion();
来源：http://kv.bookmarksfly.cn

JS:   process.platform;  process.version
来源：http://jf.yuntaijiaju.cn

TS:   process.platform;  process.version
来源：http://jt.shtwfgs.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://gt.szxytkj.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ys.shtwfgs.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ve.gzmigu.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://vj.panjiajie.cn

================================================================================
来源：http://ai.asd995.cn

N. 数据结构与算法
来源：http://vk.jianghongdianzi.cn

================================================================================
来源：http://pb.haigaiapp.cn

[N01] 二分查找（有序数组）
来源：http://su.huixinmuqiang.cn

Py:   bisect.bisect_left(arr, x)
来源：http://fw.yuexingan06.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://uh.wgjwhj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pu.wgjwhj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dh.huixinmuqiang.cn

Java: Arrays.binarySearch(arr, x)
来源：http://sd.asd995.cn

Go:   sort.SearchInts(arr, x)
来源：http://nn.panjiajie.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://jj.panjiajie.cn

C#:   Array.BinarySearch(arr, x)
来源：http://uj.szxytkj.cn

[N02] 排序（工程实践用内置实现）
来源：http://mn.newstarts.cn

Py:   sorted(arr);  arr.sort()
来源：http://oq.hnjuh.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ii.nszjky.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://jz.colortex.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://km.nszjky.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mx.jctech888.com.cn

Go:   slices.Sort(arr)
来源：http://by.bjjhwx.cn

Ruby: arr.sort
来源：http://qw.huixinmuqiang.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://za.huixiangedu.cn

[N03] 快速排序（分治示例）
来源：http://bh.haigaiapp.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://zd.nicolike.cn

PHP:  // 递归实现，或用 usort
来源：http://jz.wgjwhj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qw.asd995.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cd.colortex.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://bw.haigaiapp.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://qe.hnjuh.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ap.shxzskj.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ho.asd995.cn

[N04] 斐波那契数列
来源：http://qp.hnjuh.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://kz.shxzskj.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mu.shxzukj.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zu.9csxet.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ro.hahajie.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://yv.lnxyls.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://nn.nszjky.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://nd.jianghongdianzi.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://yp.asd995.cn

[N05] 最大公约数
来源：http://lz.szsharing.cn

Py:   math.gcd(a, b)
来源：http://lo.nszjky.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ct.huixiangedu.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xr.shxzukj.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kx.9csxet.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ze.nszjky.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://gp.jianghongdianzi.cn

Ruby: a.gcd(b)
来源：http://xm.chemitech.net.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://yr.hahajie.cn

[N06] 判断回文字符串
来源：http://nx.9csxet.cn

Py:   s == s[::-1]
来源：http://pv.chemitech.net.cn

PHP:  $s === strrev($s);
来源：http://ab.gzmigu.cn

JS:   s === [...s].reverse().join("")
来源：http://mq.haigaiapp.cn

TS:   s === [...s].reverse().join("")
来源：http://wz.hnjuh.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://me.jianghongdianzi.cn

Go:   // 双指针从两端比较
来源：http://rb.haigaiapp.cn

Ruby: s == s.reverse
来源：http://ev.panjiajie.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://au.huixiangedu.cn

[N07] 两数之和（返回下标）
来源：http://ok.9csxet.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://bp.haigaiapp.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://dy.gzmigu.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ht.9csxet.cn

TS:   // 手写 Map<string, number>
来源：http://wf.nszjky.cn

Java: // 手写 HashMap
来源：http://oy.shxzukj.cn

Go:   // 手写 map[int]int
来源：http://qw.huixinmuqiang.cn

Ruby: // 手写 Hash
来源：http://dy.yuexingan06.cn

C#:   // 手写 Dictionary<int, int>
来源：http://lj.521024.cn

[N08] 生成全排列
来源：http://ep.hnjuh.cn

Py:   itertools.permutations(arr)
来源：http://xc.wgjwhj.cn

PHP:  // 手写递归交换
来源：http://fx.nszjky.cn

JS:   // 手写回溯递归
来源：http://lu.bjjhwx.cn

TS:   // 手写回溯递归
来源：http://qp.jianghongdianzi.cn

Java: // 手写回溯递归
来源：http://gn.shtwfgs.cn

Go:   // 手写回溯递归
来源：http://ub.gzmigu.cn

Ruby: arr.permutation.to_a
来源：http://pl.huixinmuqiang.cn

C#:   // 手写回溯递归
来源：http://bj.szsharing.cn

[N09] 栈与队列
来源：http://tg.szxytkj.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://eq.colortex.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ky.colortex.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://on.colortex.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://xl.szsharing.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wp.muxihuayi.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://iu.bjjhwx.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://tc.szxytkj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://bi.panjiajie.cn

[N10] 链表节点定义
来源：http://qf.yuntaijiaju.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ky.bjjhwx.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://bx.521024.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://bq.bjjhwx.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://jb.lnxyls.cn

Java: class Node { int v; Node next; }
来源：http://hg.huanxung.cn

Go:   type Node struct { V int; Next *Node }
来源：http://iv.bookmarksfly.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://uy.wgjwhj.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://eq.nicolike.cn

[N11] 二叉树中序遍历
来源：http://jb.hahajie.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://jz.hahajie.cn

PHP:  // 手写递归函数
来源：http://jw.bjjhwx.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vn.wgjwhj.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xs.jctech888.com.cn

Java: // 手写递归
来源：http://nn.521024.cn

Go:   // 手写递归
来源：http://iq.colortex.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://gr.newstarts.cn

C#:   // 手写递归
来源：http://hh.bjjhwx.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ff.hahajie.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ky.panjiajie.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://lh.panjiajie.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cp.szsharing.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dk.chemitech.net.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://kr.521024.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ql.9csxet.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://bb.szsharing.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://tu.chemitech.net.cn

================================================================================
来源：http://an.gzmigu.cn

O. 并发与异步
来源：http://nl.wgjwhj.cn

================================================================================
来源：http://ck.gzmigu.cn

[O01] 启动一个线程
来源：http://ax.chemitech.net.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://cw.yuntaijiaju.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://dc.yuexingan06.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://qn.chemitech.net.cn

TS:   // 同 JS
来源：http://tj.shxzukj.cn

Java: new Thread(() -> f()).start()
来源：http://dw.haigaiapp.cn

Go:   go f()
来源：http://or.szxytkj.cn

Ruby: Thread.new { f }
来源：http://ka.huixinmuqiang.cn

C#:   Task.Run(() => F());
来源：http://kd.huanxung.cn

[O02] 使用线程池
来源：http://pk.shxzukj.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://zx.colortex.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://lr.huixinmuqiang.cn

JS:   // worker_threads 线程池
来源：http://zp.yuntaijiaju.cn


<!-- 参考信息 -->