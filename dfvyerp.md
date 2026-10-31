代发 wailian999

Java: // 手写拷贝构造，或序列化往返
来源：http://fv.yuexingan06.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ji.jianghongdianzi.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://bw.chemitech.net.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://xs.jianghongdianzi.cn

[K06] 解析 URL 查询串
来源：http://ml.yuntaijiaju.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://bg.panjiajie.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://vb.lnxyls.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dn.bjjhwx.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pf.panjiajie.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://kc.szxytkj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://it.521024.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ay.panjiajie.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mx.shtwfgs.cn

[K07] 进制转换
来源：http://xd.bookmarksfly.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://zl.szxytkj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://cl.bjjhwx.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://cr.szsharing.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ly.wgjwhj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xz.panjiajie.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ol.chemitech.net.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://lt.muxihuayi.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://rp.jianghongdianzi.cn

[K08] 二进制序列化（非 JSON）
来源：http://gw.chemitech.net.cn

Py:   pickle.dumps(obj)
来源：http://ks.bookmarksfly.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://dj.jianghongdianzi.cn

JS:   v8.serialize(obj)        // Node
来源：http://tb.9csxet.cn

TS:   v8.serialize(obj)        // Node
来源：http://yg.lnxyls.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://bg.yuexingan06.cn

Go:   encoding/gob
来源：http://qm.wgjwhj.cn

Ruby: Marshal.dump(obj)
来源：http://gm.yuntaijiaju.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://fg.9csxet.cn

================================================================================
来源：http://qk.colortex.cn

L. 网络请求
来源：http://nk.jctech888.com.cn

================================================================================
来源：http://tv.shtwfgs.cn

[L01] 发送 GET 请求
来源：http://vc.chemitech.net.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://zs.wgjwhj.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://rj.shxzukj.cn

JS:   await fetch(url)
来源：http://bs.521024.cn

TS:   await fetch(url)
来源：http://hf.bjjhwx.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hy.hnjuh.cn

Go:   resp, err := http.Get(url)
来源：http://aa.bookmarksfly.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://xl.nszjky.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://qm.szxytkj.cn

[L02] 发送 POST JSON
来源：http://ep.nicolike.cn

Py:   requests.post(url, json={"a": 1})
来源：http://dz.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://dp.yuexingan06.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sh.muxihuayi.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cr.panjiajie.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ss.szsharing.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ns.haigaiapp.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://us.huixiangedu.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wu.panjiajie.cn

[L03] 设置自定义请求头
来源：http://gr.yuntaijiaju.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://vk.szsharing.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://bl.newstarts.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://oy.jctech888.com.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ga.shtwfgs.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://pt.hnjuh.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://vr.jianghongdianzi.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ph.hahajie.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://pi.chemitech.net.cn

[L04] 设置超时
来源：http://ld.hahajie.cn

Py:   requests.get(url, timeout=5)
来源：http://tf.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://rd.haigaiapp.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rc.asd995.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xj.szsharing.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://zl.szsharing.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://eb.9csxet.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://zy.wgjwhj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qv.shxzskj.cn

[L05] 上传文件（multipart）
来源：http://jj.bookmarksfly.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://qj.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://rr.huixiangedu.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://fb.yuexingan06.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ye.huixinmuqiang.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://rm.hahajie.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://xq.521024.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://gx.szxytkj.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://he.wgjwhj.cn

[L06] 解析响应为 JSON
来源：http://kp.521024.cn

Py:   resp.json()
来源：http://ff.521024.cn

PHP:  json_decode($body, true);
来源：http://rg.szxytkj.cn

JS:   await resp.json()
来源：http://ho.yuexingan06.cn

TS:   await resp.json()
来源：http://xl.hahajie.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ke.chemitech.net.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://co.lnxyls.cn

Ruby: JSON.parse(resp.body)
来源：http://pn.chemitech.net.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://yr.chemitech.net.cn

[L07] 处理 HTTP 状态码
来源：http://fd.9csxet.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://rp.asd995.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://by.bookmarksfly.cn

JS:   resp.ok;  resp.status
来源：http://ix.szxytkj.cn

TS:   resp.ok;  resp.status
来源：http://if.yuexingan06.cn

Java: resp.statusCode()
来源：http://dv.haigaiapp.cn

Go:   resp.StatusCode
来源：http://kj.lnxyls.cn

Ruby: resp.code.to_i
来源：http://bv.hahajie.cn

C#:   (int)resp.StatusCode
来源：http://wj.hnjuh.cn

[L08] 并发请求多个地址
来源：http://it.bookmarksfly.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ht.wgjwhj.cn

PHP:  curl_multi_init() 系列
来源：http://ch.shtwfgs.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ka.panjiajie.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dt.huanxung.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://lw.lnxyls.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ym.shtwfgs.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://xq.wgjwhj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://eg.chemitech.net.cn

================================================================================
来源：http://tc.colortex.cn

M. 命令行 / 进程 / 环境
来源：http://wx.huixiangedu.cn

================================================================================
来源：http://gp.colortex.cn

[M01] 读取命令行参数
来源：http://yr.shtwfgs.cn

Py:   sys.argv[1:]
来源：http://sd.bookmarksfly.cn

PHP:  $argv;  $argc;
来源：http://rf.hnjuh.cn

JS:   process.argv.slice(2)
来源：http://gl.yuntaijiaju.cn

TS:   process.argv.slice(2)
来源：http://ge.haigaiapp.cn

Java: args 数组（main 方法参数）
来源：http://wl.lnxyls.cn

Go:   os.Args[1:]
来源：http://xx.yuexingan06.cn

Ruby: ARGV
来源：http://mr.lnxyls.cn

C#:   args 数组（Main 方法参数）
来源：http://fk.colortex.cn

[M02] 读取环境变量
来源：http://pq.asd995.cn

Py:   os.environ.get("HOME")
来源：http://un.colortex.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zl.asd995.cn

JS:   process.env.HOME
来源：http://cr.hahajie.cn

TS:   process.env.HOME
来源：http://wv.nicolike.cn

Java: System.getenv("HOME")
来源：http://rk.hahajie.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://yi.gzmigu.cn

Ruby: ENV["HOME"]
来源：http://hs.521024.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://lk.huanxung.cn

[M03] 执行外部命令
来源：http://ji.panjiajie.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://rf.szsharing.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://rw.newstarts.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://nn.haigaiapp.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://xk.jianghongdianzi.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hf.szsharing.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://wv.bjjhwx.cn

Ruby: system("ls -l");  `ls -l`
来源：http://th.huanxung.cn

C#:   Process.Start("ls", "-l");
来源：http://rc.yuexingan06.cn

[M04] 获取当前工作目录
来源：http://kp.shxzukj.cn

Py:   os.getcwd()
来源：http://zk.gzmigu.cn

PHP:  getcwd();
来源：http://ar.shxzukj.cn

JS:   process.cwd()
来源：http://qy.yuntaijiaju.cn

TS:   process.cwd()
来源：http://pg.bookmarksfly.cn

Java: Path.of("").toAbsolutePath()
来源：http://mq.521024.cn

Go:   os.Getwd()
来源：http://bt.jianghongdianzi.cn

Ruby: Dir.pwd
来源：http://lj.nicolike.cn

C#:   Directory.GetCurrentDirectory()
来源：http://vj.nicolike.cn

[M05] 设置退出码
来源：http://wy.chemitech.net.cn

Py:   sys.exit(1)
来源：http://bd.panjiajie.cn

PHP:  exit(1);
来源：http://nv.wgjwhj.cn

JS:   process.exit(1)
来源：http://jh.huixinmuqiang.cn

TS:   process.exit(1)
来源：http://sc.huixinmuqiang.cn

Java: System.exit(1)
来源：http://vu.bookmarksfly.cn

Go:   os.Exit(1)
来源：http://fp.yuntaijiaju.cn

Ruby: exit 1
来源：http://es.shxzskj.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://sy.jianghongdianzi.cn

[M06] 向标准错误输出
来源：http://np.panjiajie.cn

Py:   print("err", file=sys.stderr)
来源：http://nx.shxzukj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://lx.huixiangedu.cn

JS:   console.error("err")
来源：http://sy.shtwfgs.cn

TS:   console.error("err")
来源：http://gi.hahajie.cn

Java: System.err.println("err")
来源：http://ch.colortex.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://js.bookmarksfly.cn

Ruby: warn "err"
来源：http://jo.bookmarksfly.cn

C#:   Console.Error.WriteLine("err")
来源：http://wq.huixiangedu.cn

[M07] 判断是否为主入口
来源：http://tz.chemitech.net.cn

Py:   if __name__ == "__main__":
来源：http://tu.jianghongdianzi.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://rh.hnjuh.cn

JS:   require.main === module
来源：http://wb.9csxet.cn

TS:   require.main === module
来源：http://aa.bjjhwx.cn

Java: public static void main(String[] args)
来源：http://ez.jianghongdianzi.cn

Go:   func main()
来源：http://wv.szsharing.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wx.colortex.cn

C#:   static void Main(string[] args)
来源：http://ls.9csxet.cn

[M08] 获取系统与运行时信息
来源：http://vu.nicolike.cn

Py:   platform.system();  platform.python_version()
来源：http://wf.szxytkj.cn

PHP:  PHP_OS;  phpversion();
来源：http://ni.newstarts.cn

JS:   process.platform;  process.version
来源：http://hy.shxzukj.cn

TS:   process.platform;  process.version
来源：http://rw.colortex.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://um.wgjwhj.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://yx.yuexingan06.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://cb.lnxyls.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://to.yuexingan06.cn

================================================================================
来源：http://dp.panjiajie.cn

N. 数据结构与算法
来源：http://fp.szsharing.cn

================================================================================
来源：http://vt.nicolike.cn

[N01] 二分查找（有序数组）
来源：http://mc.colortex.cn

Py:   bisect.bisect_left(arr, x)
来源：http://cj.colortex.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://cm.shtwfgs.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rl.chemitech.net.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://to.chemitech.net.cn

Java: Arrays.binarySearch(arr, x)
来源：http://cx.huanxung.cn

Go:   sort.SearchInts(arr, x)
来源：http://gn.newstarts.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://cy.huanxung.cn

C#:   Array.BinarySearch(arr, x)
来源：http://uh.521024.cn

[N02] 排序（工程实践用内置实现）
来源：http://hj.szxytkj.cn

Py:   sorted(arr);  arr.sort()
来源：http://df.shxzskj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://uo.muxihuayi.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://na.lnxyls.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ti.szxytkj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ne.nszjky.cn

Go:   slices.Sort(arr)
来源：http://gb.haigaiapp.cn

Ruby: arr.sort
来源：http://oy.asd995.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://xe.asd995.cn

[N03] 快速排序（分治示例）
来源：http://hm.hnjuh.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://qb.szxytkj.cn

PHP:  // 递归实现，或用 usort
来源：http://zt.colortex.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qt.jctech888.com.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ji.nszjky.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://nu.asd995.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ef.bookmarksfly.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ts.colortex.cn

C#:   // 手写递归，或 Array.Sort
来源：http://nm.bookmarksfly.cn

[N04] 斐波那契数列
来源：http://vb.yuexingan06.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://nb.gzmigu.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ej.newstarts.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mi.asd995.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://is.9csxet.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ns.hahajie.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ax.yuexingan06.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://yh.yuexingan06.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hr.newstarts.cn

[N05] 最大公约数
来源：http://kq.szsharing.cn

Py:   math.gcd(a, b)
来源：http://ws.lnxyls.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ro.nszjky.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qt.szsharing.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mc.hahajie.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://du.szxytkj.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://nv.jctech888.com.cn

Ruby: a.gcd(b)
来源：http://ag.shxzukj.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://gv.muxihuayi.cn

[N06] 判断回文字符串
来源：http://ny.newstarts.cn

Py:   s == s[::-1]
来源：http://cs.521024.cn

PHP:  $s === strrev($s);
来源：http://jb.9csxet.cn

JS:   s === [...s].reverse().join("")
来源：http://tx.nicolike.cn

TS:   s === [...s].reverse().join("")
来源：http://gz.nicolike.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ht.lnxyls.cn

Go:   // 双指针从两端比较
来源：http://iz.wgjwhj.cn

Ruby: s == s.reverse
来源：http://hd.nicolike.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://vg.521024.cn

[N07] 两数之和（返回下标）
来源：http://qj.haigaiapp.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://la.huixiangedu.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ma.nszjky.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ch.huanxung.cn

TS:   // 手写 Map<string, number>
来源：http://ts.asd995.cn

Java: // 手写 HashMap
来源：http://sc.chemitech.net.cn

Go:   // 手写 map[int]int
来源：http://ud.muxihuayi.cn

Ruby: // 手写 Hash
来源：http://xj.hahajie.cn

C#:   // 手写 Dictionary<int, int>
来源：http://iq.panjiajie.cn

[N08] 生成全排列
来源：http://wm.newstarts.cn

Py:   itertools.permutations(arr)
来源：http://bk.jctech888.com.cn

PHP:  // 手写递归交换
来源：http://eq.shxzskj.cn

JS:   // 手写回溯递归
来源：http://tu.nicolike.cn

TS:   // 手写回溯递归
来源：http://bo.521024.cn

Java: // 手写回溯递归
来源：http://th.szsharing.cn

Go:   // 手写回溯递归
来源：http://is.nicolike.cn

Ruby: arr.permutation.to_a
来源：http://mw.wgjwhj.cn

C#:   // 手写回溯递归
来源：http://ig.yuntaijiaju.cn

[N09] 栈与队列
来源：http://qu.yuntaijiaju.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://pt.nicolike.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://bg.hnjuh.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://xk.haigaiapp.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://zw.newstarts.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://xz.bookmarksfly.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://rc.521024.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://jp.huanxung.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://bt.asd995.cn

[N10] 链表节点定义
来源：http://ti.hahajie.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://au.chemitech.net.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://nu.jianghongdianzi.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://zg.lnxyls.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ye.yuexingan06.cn

Java: class Node { int v; Node next; }
来源：http://uj.wgjwhj.cn

Go:   type Node struct { V int; Next *Node }
来源：http://vg.huanxung.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ww.szsharing.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ub.huixiangedu.cn

[N11] 二叉树中序遍历
来源：http://tm.hnjuh.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ji.gzmigu.cn

PHP:  // 手写递归函数
来源：http://oz.huixiangedu.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mk.shtwfgs.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://uj.yuexingan06.cn

Java: // 手写递归
来源：http://gy.asd995.cn

Go:   // 手写递归
来源：http://iy.yuntaijiaju.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ey.yuntaijiaju.cn

C#:   // 手写递归
来源：http://lf.521024.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mn.hahajie.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://es.yuntaijiaju.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://dp.jctech888.com.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dq.jianghongdianzi.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fh.nicolike.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://zk.wgjwhj.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://zg.lnxyls.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://pt.gzmigu.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://uh.lnxyls.cn

================================================================================
来源：http://za.gzmigu.cn

O. 并发与异步
来源：http://al.huixinmuqiang.cn

================================================================================
来源：http://ht.wgjwhj.cn

[O01] 启动一个线程
来源：http://xw.shxzskj.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://bh.szsharing.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ef.szsharing.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://cf.bjjhwx.cn

TS:   // 同 JS
来源：http://sw.jianghongdianzi.cn


<!-- 参考信息 -->