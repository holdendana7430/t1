代发 wailian999

Java: // 手写拷贝构造，或序列化往返
来源：http://pi.chemitech.net.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://br.hahajie.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zf.gzmigu.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://cw.chemitech.net.cn

[K06] 解析 URL 查询串
来源：http://ew.szsharing.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ma.shxzukj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://qf.lnxyls.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://db.newstarts.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qc.bjjhwx.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://il.szxytkj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://hs.521024.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mr.bookmarksfly.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://es.shxzukj.cn

[K07] 进制转换
来源：http://ty.wgjwhj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://cl.bookmarksfly.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://eg.bjjhwx.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://nu.gzmigu.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://pk.nicolike.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wh.szxytkj.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://th.jianghongdianzi.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://io.shxzukj.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ib.colortex.cn

[K08] 二进制序列化（非 JSON）
来源：http://ba.szxytkj.cn

Py:   pickle.dumps(obj)
来源：http://gj.9csxet.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://aj.yuntaijiaju.cn

JS:   v8.serialize(obj)        // Node
来源：http://fm.yuntaijiaju.cn

TS:   v8.serialize(obj)        // Node
来源：http://by.nicolike.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://pm.521024.cn

Go:   encoding/gob
来源：http://yg.shtwfgs.cn

Ruby: Marshal.dump(obj)
来源：http://nb.yuexingan06.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ri.jianghongdianzi.cn

================================================================================
来源：http://ps.wgjwhj.cn

L. 网络请求
来源：http://qd.chemitech.net.cn

================================================================================
来源：http://cj.jianghongdianzi.cn

[L01] 发送 GET 请求
来源：http://iv.521024.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://dl.bookmarksfly.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://pl.szxytkj.cn

JS:   await fetch(url)
来源：http://ft.newstarts.cn

TS:   await fetch(url)
来源：http://ud.nszjky.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ys.jianghongdianzi.cn

Go:   resp, err := http.Get(url)
来源：http://sx.asd995.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://wp.bjjhwx.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://fw.huixinmuqiang.cn

[L02] 发送 POST JSON
来源：http://op.haigaiapp.cn

Py:   requests.post(url, json={"a": 1})
来源：http://bj.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hv.chemitech.net.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://uf.nszjky.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vh.9csxet.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vw.yuntaijiaju.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://gh.shxzskj.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://jk.yuntaijiaju.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://iv.521024.cn

[L03] 设置自定义请求头
来源：http://qk.nicolike.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://az.hnjuh.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://xn.lnxyls.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bh.huixiangedu.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ek.szsharing.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://rs.lnxyls.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://rk.521024.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://uf.yuexingan06.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://lo.bookmarksfly.cn

[L04] 设置超时
来源：http://ex.shxzukj.cn

Py:   requests.get(url, timeout=5)
来源：http://kp.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://fb.colortex.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ml.haigaiapp.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qq.newstarts.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://yq.szsharing.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://rz.bjjhwx.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://gw.shtwfgs.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://rn.haigaiapp.cn

[L05] 上传文件（multipart）
来源：http://cn.chemitech.net.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://xb.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://dg.szsharing.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://lv.newstarts.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://yn.yuexingan06.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://lp.chemitech.net.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://lk.colortex.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://lb.huanxung.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://zd.wgjwhj.cn

[L06] 解析响应为 JSON
来源：http://iy.newstarts.cn

Py:   resp.json()
来源：http://qi.huixiangedu.cn

PHP:  json_decode($body, true);
来源：http://ag.shxzskj.cn

JS:   await resp.json()
来源：http://iq.szxytkj.cn

TS:   await resp.json()
来源：http://km.gzmigu.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://fp.yuexingan06.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://cj.colortex.cn

Ruby: JSON.parse(resp.body)
来源：http://uk.shxzukj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://qg.szxytkj.cn

[L07] 处理 HTTP 状态码
来源：http://ma.lnxyls.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://rb.nicolike.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ru.shtwfgs.cn

JS:   resp.ok;  resp.status
来源：http://qq.newstarts.cn

TS:   resp.ok;  resp.status
来源：http://um.hnjuh.cn

Java: resp.statusCode()
来源：http://li.chemitech.net.cn

Go:   resp.StatusCode
来源：http://ui.shxzukj.cn

Ruby: resp.code.to_i
来源：http://tf.muxihuayi.cn

C#:   (int)resp.StatusCode
来源：http://xh.haigaiapp.cn

[L08] 并发请求多个地址
来源：http://ew.shxzskj.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://rs.newstarts.cn

PHP:  curl_multi_init() 系列
来源：http://ct.huixiangedu.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rj.nicolike.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nk.lnxyls.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://lo.gzmigu.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://cm.huixiangedu.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://pq.szxytkj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xt.szxytkj.cn

================================================================================
来源：http://ph.shxzukj.cn

M. 命令行 / 进程 / 环境
来源：http://jn.wgjwhj.cn

================================================================================
来源：http://zx.szsharing.cn

[M01] 读取命令行参数
来源：http://qm.yuexingan06.cn

Py:   sys.argv[1:]
来源：http://sz.colortex.cn

PHP:  $argv;  $argc;
来源：http://gl.bjjhwx.cn

JS:   process.argv.slice(2)
来源：http://gy.shtwfgs.cn

TS:   process.argv.slice(2)
来源：http://fc.huanxung.cn

Java: args 数组（main 方法参数）
来源：http://re.szsharing.cn

Go:   os.Args[1:]
来源：http://ma.panjiajie.cn

Ruby: ARGV
来源：http://qd.yuntaijiaju.cn

C#:   args 数组（Main 方法参数）
来源：http://et.shxzukj.cn

[M02] 读取环境变量
来源：http://pl.huixinmuqiang.cn

Py:   os.environ.get("HOME")
来源：http://vr.chemitech.net.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://jq.newstarts.cn

JS:   process.env.HOME
来源：http://nt.szsharing.cn

TS:   process.env.HOME
来源：http://iw.shtwfgs.cn

Java: System.getenv("HOME")
来源：http://nx.chemitech.net.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ah.huixinmuqiang.cn

Ruby: ENV["HOME"]
来源：http://pg.lnxyls.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://fz.9csxet.cn

[M03] 执行外部命令
来源：http://kz.huanxung.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ve.shxzskj.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://my.nicolike.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://mq.shxzskj.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ld.yuexingan06.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mj.bjjhwx.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://jn.hahajie.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ue.yuexingan06.cn

C#:   Process.Start("ls", "-l");
来源：http://qi.9csxet.cn

[M04] 获取当前工作目录
来源：http://at.huixiangedu.cn

Py:   os.getcwd()
来源：http://lq.wgjwhj.cn

PHP:  getcwd();
来源：http://qn.bjjhwx.cn

JS:   process.cwd()
来源：http://nx.haigaiapp.cn

TS:   process.cwd()
来源：http://ei.huixinmuqiang.cn

Java: Path.of("").toAbsolutePath()
来源：http://yb.lnxyls.cn

Go:   os.Getwd()
来源：http://ie.chemitech.net.cn

Ruby: Dir.pwd
来源：http://hk.9csxet.cn

C#:   Directory.GetCurrentDirectory()
来源：http://wm.haigaiapp.cn

[M05] 设置退出码
来源：http://jc.chemitech.net.cn

Py:   sys.exit(1)
来源：http://tq.shxzskj.cn

PHP:  exit(1);
来源：http://xo.newstarts.cn

JS:   process.exit(1)
来源：http://fd.yuntaijiaju.cn

TS:   process.exit(1)
来源：http://re.huixinmuqiang.cn

Java: System.exit(1)
来源：http://ey.lnxyls.cn

Go:   os.Exit(1)
来源：http://ta.yuntaijiaju.cn

Ruby: exit 1
来源：http://xn.szxytkj.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://tw.nicolike.cn

[M06] 向标准错误输出
来源：http://bd.nszjky.cn

Py:   print("err", file=sys.stderr)
来源：http://zo.yuexingan06.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://wv.nszjky.cn

JS:   console.error("err")
来源：http://na.asd995.cn

TS:   console.error("err")
来源：http://bq.panjiajie.cn

Java: System.err.println("err")
来源：http://yy.nicolike.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.asd995.cn

Ruby: warn "err"
来源：http://hp.huixinmuqiang.cn

C#:   Console.Error.WriteLine("err")
来源：http://ax.bjjhwx.cn

[M07] 判断是否为主入口
来源：http://pb.jianghongdianzi.cn

Py:   if __name__ == "__main__":
来源：http://ev.asd995.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://fm.jianghongdianzi.cn

JS:   require.main === module
来源：http://yv.newstarts.cn

TS:   require.main === module
来源：http://nv.bjjhwx.cn

Java: public static void main(String[] args)
来源：http://az.asd995.cn

Go:   func main()
来源：http://gg.huanxung.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hw.chemitech.net.cn

C#:   static void Main(string[] args)
来源：http://en.hnjuh.cn

[M08] 获取系统与运行时信息
来源：http://jp.colortex.cn

Py:   platform.system();  platform.python_version()
来源：http://du.huanxung.cn

PHP:  PHP_OS;  phpversion();
来源：http://ws.szsharing.cn

JS:   process.platform;  process.version
来源：http://ca.jianghongdianzi.cn

TS:   process.platform;  process.version
来源：http://oe.panjiajie.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hf.yuexingan06.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://bi.bjjhwx.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ob.muxihuayi.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://uo.shxzskj.cn

================================================================================
来源：http://te.newstarts.cn

N. 数据结构与算法
来源：http://ol.colortex.cn

================================================================================
来源：http://hf.asd995.cn

[N01] 二分查找（有序数组）
来源：http://wf.jctech888.com.cn

Py:   bisect.bisect_left(arr, x)
来源：http://kn.bookmarksfly.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://vn.hnjuh.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://km.haigaiapp.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ru.chemitech.net.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ki.haigaiapp.cn

Go:   sort.SearchInts(arr, x)
来源：http://qc.bookmarksfly.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://su.yuexingan06.cn

C#:   Array.BinarySearch(arr, x)
来源：http://yh.chemitech.net.cn

[N02] 排序（工程实践用内置实现）
来源：http://gu.huanxung.cn

Py:   sorted(arr);  arr.sort()
来源：http://yc.nszjky.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://kb.bookmarksfly.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ms.szxytkj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ru.shxzskj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://cv.nszjky.cn

Go:   slices.Sort(arr)
来源：http://yj.521024.cn

Ruby: arr.sort
来源：http://ue.haigaiapp.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://fz.newstarts.cn

[N03] 快速排序（分治示例）
来源：http://nk.shtwfgs.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://te.muxihuayi.cn

PHP:  // 递归实现，或用 usort
来源：http://dr.jianghongdianzi.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gg.huixiangedu.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nn.haigaiapp.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ay.huixinmuqiang.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://pq.szsharing.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://kz.hnjuh.cn

C#:   // 手写递归，或 Array.Sort
来源：http://me.chemitech.net.cn

[N04] 斐波那契数列
来源：http://pv.wgjwhj.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zd.nszjky.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wz.huixinmuqiang.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://av.bjjhwx.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jg.gzmigu.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://dl.bjjhwx.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://lv.newstarts.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://vx.muxihuayi.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://pk.colortex.cn

[N05] 最大公约数
来源：http://em.newstarts.cn

Py:   math.gcd(a, b)
来源：http://qm.gzmigu.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://el.hahajie.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wr.shxzskj.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://af.bjjhwx.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wf.lnxyls.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://fu.chemitech.net.cn

Ruby: a.gcd(b)
来源：http://ez.9csxet.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://in.gzmigu.cn

[N06] 判断回文字符串
来源：http://ud.szsharing.cn

Py:   s == s[::-1]
来源：http://xn.shxzskj.cn

PHP:  $s === strrev($s);
来源：http://zx.shxzukj.cn

JS:   s === [...s].reverse().join("")
来源：http://mh.shtwfgs.cn

TS:   s === [...s].reverse().join("")
来源：http://lv.bjjhwx.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wg.9csxet.cn

Go:   // 双指针从两端比较
来源：http://yi.haigaiapp.cn

Ruby: s == s.reverse
来源：http://vm.hahajie.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://vy.bookmarksfly.cn

[N07] 两数之和（返回下标）
来源：http://ls.gzmigu.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://zx.szxytkj.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://zc.yuntaijiaju.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://xl.9csxet.cn

TS:   // 手写 Map<string, number>
来源：http://rq.jianghongdianzi.cn

Java: // 手写 HashMap
来源：http://mt.huanxung.cn

Go:   // 手写 map[int]int
来源：http://xp.asd995.cn

Ruby: // 手写 Hash
来源：http://fz.hnjuh.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ii.9csxet.cn

[N08] 生成全排列
来源：http://uh.gzmigu.cn

Py:   itertools.permutations(arr)
来源：http://qk.yuntaijiaju.cn

PHP:  // 手写递归交换
来源：http://bm.colortex.cn

JS:   // 手写回溯递归
来源：http://sb.gzmigu.cn

TS:   // 手写回溯递归
来源：http://ou.wgjwhj.cn

Java: // 手写回溯递归
来源：http://ts.panjiajie.cn

Go:   // 手写回溯递归
来源：http://yb.nszjky.cn

Ruby: arr.permutation.to_a
来源：http://ot.yuntaijiaju.cn

C#:   // 手写回溯递归
来源：http://av.shxzukj.cn

[N09] 栈与队列
来源：http://sg.nszjky.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://fh.shtwfgs.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wq.chemitech.net.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ha.yuexingan06.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://bh.gzmigu.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://fo.szxytkj.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ga.shxzukj.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hw.shxzskj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://dp.panjiajie.cn

[N10] 链表节点定义
来源：http://er.nicolike.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://zo.panjiajie.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://yl.huixiangedu.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ef.jianghongdianzi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://fq.bookmarksfly.cn

Java: class Node { int v; Node next; }
来源：http://fi.jctech888.com.cn

Go:   type Node struct { V int; Next *Node }
来源：http://tg.yuntaijiaju.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://xs.szxytkj.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://tq.hnjuh.cn

[N11] 二叉树中序遍历
来源：http://ue.521024.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://kt.shtwfgs.cn

PHP:  // 手写递归函数
来源：http://rr.shtwfgs.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ak.muxihuayi.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vp.muxihuayi.cn

Java: // 手写递归
来源：http://sg.nicolike.cn

Go:   // 手写递归
来源：http://qc.asd995.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ii.newstarts.cn

C#:   // 手写递归
来源：http://uv.yuntaijiaju.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://pn.colortex.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://nb.yuexingan06.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ii.shxzukj.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yq.jianghongdianzi.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://uq.newstarts.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ju.521024.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://zm.shxzukj.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://xj.szsharing.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://av.jianghongdianzi.cn

================================================================================
来源：http://by.521024.cn

O. 并发与异步
来源：http://oe.bookmarksfly.cn

================================================================================
来源：http://df.nicolike.cn

[O01] 启动一个线程
来源：http://qe.shxzskj.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://il.nszjky.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://kz.hnjuh.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://uw.muxihuayi.cn

TS:   // 同 JS
来源：http://la.yuexingan06.cn


<!-- 参考信息 -->