代发 wailian999

[K06] 解析 URL 查询串
来源：http://mz.lnxyls.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://dx.9csxet.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://pl.muxihuayi.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gl.gzmigu.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://du.huixiangedu.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://nv.newstarts.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://sb.9csxet.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://kq.nicolike.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://pp.colortex.cn

[K07] 进制转换
来源：http://sh.szsharing.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://cm.huanxung.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://id.panjiajie.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ij.szsharing.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wp.panjiajie.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://yd.nicolike.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://qs.asd995.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://yx.muxihuayi.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://qu.szxytkj.cn

[K08] 二进制序列化（非 JSON）
来源：http://jc.shxzukj.cn

Py:   pickle.dumps(obj)
来源：http://vl.hnjuh.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://tg.szxytkj.cn

JS:   v8.serialize(obj)        // Node
来源：http://qd.shtwfgs.cn

TS:   v8.serialize(obj)        // Node
来源：http://or.521024.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://cn.bookmarksfly.cn

Go:   encoding/gob
来源：http://aj.nszjky.cn

Ruby: Marshal.dump(obj)
来源：http://wn.bookmarksfly.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://cr.huixinmuqiang.cn

================================================================================
来源：http://mw.9csxet.cn

L. 网络请求
来源：http://ty.hnjuh.cn

================================================================================
来源：http://dl.9csxet.cn

[L01] 发送 GET 请求
来源：http://bx.haigaiapp.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://zp.gzmigu.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://or.newstarts.cn

JS:   await fetch(url)
来源：http://wx.521024.cn

TS:   await fetch(url)
来源：http://vb.chemitech.net.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ea.hahajie.cn

Go:   resp, err := http.Get(url)
来源：http://wv.hnjuh.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://fc.shxzskj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://zy.chemitech.net.cn

[L02] 发送 POST JSON
来源：http://us.wgjwhj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://mg.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://zl.szxytkj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ti.haigaiapp.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sk.huixinmuqiang.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ps.shtwfgs.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ac.jianghongdianzi.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://dy.muxihuayi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ao.asd995.cn

[L03] 设置自定义请求头
来源：http://rf.jianghongdianzi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://fs.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ll.shxzskj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ba.colortex.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fw.jianghongdianzi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://js.bjjhwx.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://pe.nszjky.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://yh.shtwfgs.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hy.yuntaijiaju.cn

[L04] 设置超时
来源：http://fm.lnxyls.cn

Py:   requests.get(url, timeout=5)
来源：http://ab.haigaiapp.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://vx.wgjwhj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gy.lnxyls.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zq.huixiangedu.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://nn.nszjky.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://zz.asd995.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://oh.yuexingan06.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ez.szxytkj.cn

[L05] 上传文件（multipart）
来源：http://it.bookmarksfly.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://pb.asd995.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://kb.muxihuayi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://pn.lnxyls.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://cy.wgjwhj.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ho.nszjky.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://el.asd995.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://yk.nszjky.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ds.szxytkj.cn

[L06] 解析响应为 JSON
来源：http://jo.shtwfgs.cn

Py:   resp.json()
来源：http://in.chemitech.net.cn

PHP:  json_decode($body, true);
来源：http://or.colortex.cn

JS:   await resp.json()
来源：http://ds.newstarts.cn

TS:   await resp.json()
来源：http://pv.nszjky.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ir.shxzskj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://bt.panjiajie.cn

Ruby: JSON.parse(resp.body)
来源：http://cb.panjiajie.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://vg.yuntaijiaju.cn

[L07] 处理 HTTP 状态码
来源：http://ry.huixiangedu.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://de.huixinmuqiang.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://fa.shxzukj.cn

JS:   resp.ok;  resp.status
来源：http://ih.chemitech.net.cn

TS:   resp.ok;  resp.status
来源：http://ni.haigaiapp.cn

Java: resp.statusCode()
来源：http://sd.szsharing.cn

Go:   resp.StatusCode
来源：http://av.gzmigu.cn

Ruby: resp.code.to_i
来源：http://jm.huanxung.cn

C#:   (int)resp.StatusCode
来源：http://dh.asd995.cn

[L08] 并发请求多个地址
来源：http://xe.huixiangedu.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ui.colortex.cn

PHP:  curl_multi_init() 系列
来源：http://tq.asd995.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ax.asd995.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nc.nicolike.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://uc.yuexingan06.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://op.newstarts.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://tm.szxytkj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://yj.wgjwhj.cn

================================================================================
来源：http://xs.bjjhwx.cn

M. 命令行 / 进程 / 环境
来源：http://zd.colortex.cn

================================================================================
来源：http://eg.shxzskj.cn

[M01] 读取命令行参数
来源：http://cr.shxzukj.cn

Py:   sys.argv[1:]
来源：http://no.chemitech.net.cn

PHP:  $argv;  $argc;
来源：http://uo.huixiangedu.cn

JS:   process.argv.slice(2)
来源：http://cz.huixinmuqiang.cn

TS:   process.argv.slice(2)
来源：http://kj.shtwfgs.cn

Java: args 数组（main 方法参数）
来源：http://wk.9csxet.cn

Go:   os.Args[1:]
来源：http://cg.chemitech.net.cn

Ruby: ARGV
来源：http://zu.huixinmuqiang.cn

C#:   args 数组（Main 方法参数）
来源：http://ur.wgjwhj.cn

[M02] 读取环境变量
来源：http://fq.nicolike.cn

Py:   os.environ.get("HOME")
来源：http://pb.szxytkj.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://xg.huixinmuqiang.cn

JS:   process.env.HOME
来源：http://dc.huixinmuqiang.cn

TS:   process.env.HOME
来源：http://wu.9csxet.cn

Java: System.getenv("HOME")
来源：http://mr.huixinmuqiang.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://bv.jctech888.com.cn

Ruby: ENV["HOME"]
来源：http://yf.asd995.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://xu.nszjky.cn

[M03] 执行外部命令
来源：http://bk.colortex.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://rl.hnjuh.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ae.521024.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://qw.haigaiapp.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ur.yuntaijiaju.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ed.9csxet.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ft.nicolike.cn

Ruby: system("ls -l");  `ls -l`
来源：http://wa.bookmarksfly.cn

C#:   Process.Start("ls", "-l");
来源：http://oe.nicolike.cn

[M04] 获取当前工作目录
来源：http://ae.nicolike.cn

Py:   os.getcwd()
来源：http://uc.asd995.cn

PHP:  getcwd();
来源：http://bu.szsharing.cn

JS:   process.cwd()
来源：http://ak.lnxyls.cn

TS:   process.cwd()
来源：http://tw.huanxung.cn

Java: Path.of("").toAbsolutePath()
来源：http://ur.521024.cn

Go:   os.Getwd()
来源：http://yw.yuntaijiaju.cn

Ruby: Dir.pwd
来源：http://pu.shxzskj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://br.nszjky.cn

[M05] 设置退出码
来源：http://ez.jianghongdianzi.cn

Py:   sys.exit(1)
来源：http://vq.shxzskj.cn

PHP:  exit(1);
来源：http://fj.yuexingan06.cn

JS:   process.exit(1)
来源：http://ox.hnjuh.cn

TS:   process.exit(1)
来源：http://jp.colortex.cn

Java: System.exit(1)
来源：http://eq.chemitech.net.cn

Go:   os.Exit(1)
来源：http://hd.nszjky.cn

Ruby: exit 1
来源：http://cp.huanxung.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://fm.colortex.cn

[M06] 向标准错误输出
来源：http://zh.yuexingan06.cn

Py:   print("err", file=sys.stderr)
来源：http://lm.bookmarksfly.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://oo.huixinmuqiang.cn

JS:   console.error("err")
来源：http://rq.wgjwhj.cn

TS:   console.error("err")
来源：http://zj.jianghongdianzi.cn

Java: System.err.println("err")
来源：http://np.jianghongdianzi.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ee.yuntaijiaju.cn

Ruby: warn "err"
来源：http://kx.chemitech.net.cn

C#:   Console.Error.WriteLine("err")
来源：http://fa.szxytkj.cn

[M07] 判断是否为主入口
来源：http://lz.chemitech.net.cn

Py:   if __name__ == "__main__":
来源：http://vr.huixinmuqiang.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://gu.lnxyls.cn

JS:   require.main === module
来源：http://ny.bjjhwx.cn

TS:   require.main === module
来源：http://ju.yuntaijiaju.cn

Java: public static void main(String[] args)
来源：http://wl.lnxyls.cn

Go:   func main()
来源：http://fh.lnxyls.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://np.huixiangedu.cn

C#:   static void Main(string[] args)
来源：http://mx.yuexingan06.cn

[M08] 获取系统与运行时信息
来源：http://ys.hnjuh.cn

Py:   platform.system();  platform.python_version()
来源：http://ju.muxihuayi.cn

PHP:  PHP_OS;  phpversion();
来源：http://vd.hahajie.cn

JS:   process.platform;  process.version
来源：http://sj.nszjky.cn

TS:   process.platform;  process.version
来源：http://se.asd995.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://fb.huixinmuqiang.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://fl.hnjuh.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://qk.huanxung.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://tj.panjiajie.cn

================================================================================
来源：http://qh.shtwfgs.cn

N. 数据结构与算法
来源：http://wf.asd995.cn

================================================================================
来源：http://mw.bookmarksfly.cn

[N01] 二分查找（有序数组）
来源：http://mv.newstarts.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ze.shxzskj.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ur.yuntaijiaju.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ht.shxzskj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yf.jianghongdianzi.cn

Java: Arrays.binarySearch(arr, x)
来源：http://mi.wgjwhj.cn

Go:   sort.SearchInts(arr, x)
来源：http://ac.yuntaijiaju.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ml.yuexingan06.cn

C#:   Array.BinarySearch(arr, x)
来源：http://qc.szxytkj.cn

[N02] 排序（工程实践用内置实现）
来源：http://iv.yuntaijiaju.cn

Py:   sorted(arr);  arr.sort()
来源：http://or.521024.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ao.newstarts.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://rw.haigaiapp.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://eb.wgjwhj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://rz.chemitech.net.cn

Go:   slices.Sort(arr)
来源：http://jh.9csxet.cn

Ruby: arr.sort
来源：http://fj.hnjuh.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://my.bjjhwx.cn

[N03] 快速排序（分治示例）
来源：http://uc.jctech888.com.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://xq.huixiangedu.cn

PHP:  // 递归实现，或用 usort
来源：http://cs.wgjwhj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zk.asd995.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kc.haigaiapp.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://sn.huixinmuqiang.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://cl.huanxung.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wj.haigaiapp.cn

C#:   // 手写递归，或 Array.Sort
来源：http://pt.nszjky.cn

[N04] 斐波那契数列
来源：http://nn.huanxung.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qp.shxzukj.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ex.521024.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hk.wgjwhj.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jv.521024.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://nu.lnxyls.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://xy.wgjwhj.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://dn.newstarts.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ea.yuexingan06.cn

[N05] 最大公约数
来源：http://ij.asd995.cn

Py:   math.gcd(a, b)
来源：http://rc.jctech888.com.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://sk.shxzukj.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://os.jianghongdianzi.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lt.wgjwhj.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://al.yuntaijiaju.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://pw.jianghongdianzi.cn

Ruby: a.gcd(b)
来源：http://hb.newstarts.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://yq.wgjwhj.cn

[N06] 判断回文字符串
来源：http://sw.bjjhwx.cn

Py:   s == s[::-1]
来源：http://te.shtwfgs.cn

PHP:  $s === strrev($s);
来源：http://wv.bookmarksfly.cn

JS:   s === [...s].reverse().join("")
来源：http://en.nicolike.cn

TS:   s === [...s].reverse().join("")
来源：http://ak.yuntaijiaju.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://tq.jctech888.com.cn

Go:   // 双指针从两端比较
来源：http://bq.521024.cn

Ruby: s == s.reverse
来源：http://hl.panjiajie.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://vs.panjiajie.cn

[N07] 两数之和（返回下标）
来源：http://vv.muxihuayi.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://yw.521024.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ml.bookmarksfly.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ww.chemitech.net.cn

TS:   // 手写 Map<string, number>
来源：http://hi.muxihuayi.cn

Java: // 手写 HashMap
来源：http://mu.wgjwhj.cn

Go:   // 手写 map[int]int
来源：http://np.panjiajie.cn

Ruby: // 手写 Hash
来源：http://ck.wgjwhj.cn

C#:   // 手写 Dictionary<int, int>
来源：http://po.gzmigu.cn

[N08] 生成全排列
来源：http://va.lnxyls.cn

Py:   itertools.permutations(arr)
来源：http://ly.yuexingan06.cn

PHP:  // 手写递归交换
来源：http://ud.jianghongdianzi.cn

JS:   // 手写回溯递归
来源：http://dp.9csxet.cn

TS:   // 手写回溯递归
来源：http://uk.asd995.cn

Java: // 手写回溯递归
来源：http://yj.huixiangedu.cn

Go:   // 手写回溯递归
来源：http://px.asd995.cn

Ruby: arr.permutation.to_a
来源：http://iu.nszjky.cn

C#:   // 手写回溯递归
来源：http://nq.shxzukj.cn

[N09] 栈与队列
来源：http://fx.hahajie.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wj.hnjuh.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://bn.szsharing.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mb.wgjwhj.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://tn.muxihuayi.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://xy.hahajie.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ew.wgjwhj.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://am.hnjuh.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://vt.521024.cn

[N10] 链表节点定义
来源：http://jj.jctech888.com.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://io.szsharing.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://gi.nszjky.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hp.yuntaijiaju.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://jg.huixinmuqiang.cn

Java: class Node { int v; Node next; }
来源：http://wi.szsharing.cn

Go:   type Node struct { V int; Next *Node }
来源：http://wa.521024.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ru.panjiajie.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ea.yuntaijiaju.cn

[N11] 二叉树中序遍历
来源：http://ue.szsharing.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://av.haigaiapp.cn

PHP:  // 手写递归函数
来源：http://mo.lnxyls.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wh.huixiangedu.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yr.shtwfgs.cn

Java: // 手写递归
来源：http://mz.shxzukj.cn

Go:   // 手写递归
来源：http://hu.huixinmuqiang.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ac.hnjuh.cn

C#:   // 手写递归
来源：http://ec.hahajie.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://tv.asd995.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://dj.hnjuh.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wv.9csxet.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vf.yuntaijiaju.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gy.yuntaijiaju.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://db.nszjky.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ud.gzmigu.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://nq.521024.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://di.muxihuayi.cn

================================================================================
来源：http://gr.nicolike.cn

O. 并发与异步
来源：http://ni.haigaiapp.cn

================================================================================
来源：http://xv.9csxet.cn

[O01] 启动一个线程
来源：http://oe.asd995.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wj.521024.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://cl.bjjhwx.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://rg.9csxet.cn

TS:   // 同 JS
来源：http://lw.colortex.cn

Java: new Thread(() -> f()).start()
来源：http://rg.shxzskj.cn

Go:   go f()
来源：http://kg.shtwfgs.cn

Ruby: Thread.new { f }
来源：http://nm.huanxung.cn

C#:   Task.Run(() => F());
来源：http://oo.jianghongdianzi.cn


<!-- 参考信息 -->