代发 wailian999

[K06] 解析 URL 查询串
来源：http://hl.yuexingan06.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://of.521024.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://yi.jianghongdianzi.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uc.szsharing.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wo.muxihuayi.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://jc.szsharing.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://fj.nszjky.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://yf.muxihuayi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mp.shtwfgs.cn

[K07] 进制转换
来源：http://uf.shtwfgs.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ip.szxytkj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://lx.nicolike.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ax.chemitech.net.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://uq.muxihuayi.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://yb.hahajie.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ff.521024.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ob.huixiangedu.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://by.hnjuh.cn

[K08] 二进制序列化（非 JSON）
来源：http://be.szsharing.cn

Py:   pickle.dumps(obj)
来源：http://lf.lnxyls.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://vl.jctech888.com.cn

JS:   v8.serialize(obj)        // Node
来源：http://ty.haigaiapp.cn

TS:   v8.serialize(obj)        // Node
来源：http://ci.haigaiapp.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ya.shxzskj.cn

Go:   encoding/gob
来源：http://qi.yuexingan06.cn

Ruby: Marshal.dump(obj)
来源：http://kx.colortex.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ax.jctech888.com.cn

================================================================================
来源：http://kr.gzmigu.cn

L. 网络请求
来源：http://dj.szsharing.cn

================================================================================
来源：http://tf.yuexingan06.cn

[L01] 发送 GET 请求
来源：http://ms.521024.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://fh.shxzskj.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vd.shtwfgs.cn

JS:   await fetch(url)
来源：http://hb.huanxung.cn

TS:   await fetch(url)
来源：http://tq.szsharing.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ap.haigaiapp.cn

Go:   resp, err := http.Get(url)
来源：http://gq.shxzukj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://pd.szxytkj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://dq.panjiajie.cn

[L02] 发送 POST JSON
来源：http://fe.bookmarksfly.cn

Py:   requests.post(url, json={"a": 1})
来源：http://bh.hnjuh.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://rm.chemitech.net.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qz.wgjwhj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ch.shxzskj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ef.bjjhwx.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.asd995.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://vg.nszjky.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://zk.chemitech.net.cn

[L03] 设置自定义请求头
来源：http://rx.nszjky.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ai.521024.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ln.nicolike.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://iy.yuntaijiaju.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sx.panjiajie.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://xy.huixinmuqiang.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jl.huanxung.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://jg.haigaiapp.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://uw.panjiajie.cn

[L04] 设置超时
来源：http://tu.shxzukj.cn

Py:   requests.get(url, timeout=5)
来源：http://wi.yuntaijiaju.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.nicolike.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pe.newstarts.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yh.yuntaijiaju.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://tl.shxzskj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://vx.shxzukj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://jf.jctech888.com.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ns.lnxyls.cn

[L05] 上传文件（multipart）
来源：http://nk.huixinmuqiang.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://oa.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ss.huixiangedu.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ut.huixiangedu.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://aj.newstarts.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://lu.hnjuh.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://tr.shtwfgs.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://sd.yuexingan06.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://se.shxzskj.cn

[L06] 解析响应为 JSON
来源：http://zc.newstarts.cn

Py:   resp.json()
来源：http://eo.muxihuayi.cn

PHP:  json_decode($body, true);
来源：http://ja.jianghongdianzi.cn

JS:   await resp.json()
来源：http://jl.muxihuayi.cn

TS:   await resp.json()
来源：http://fx.9csxet.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://uz.gzmigu.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://by.szsharing.cn

Ruby: JSON.parse(resp.body)
来源：http://zh.9csxet.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://qq.huixiangedu.cn

[L07] 处理 HTTP 状态码
来源：http://id.szxytkj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://qh.jianghongdianzi.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://tw.shxzskj.cn

JS:   resp.ok;  resp.status
来源：http://ik.panjiajie.cn

TS:   resp.ok;  resp.status
来源：http://au.gzmigu.cn

Java: resp.statusCode()
来源：http://qj.shxzukj.cn

Go:   resp.StatusCode
来源：http://lj.yuntaijiaju.cn

Ruby: resp.code.to_i
来源：http://cp.gzmigu.cn

C#:   (int)resp.StatusCode
来源：http://ak.shxzskj.cn

[L08] 并发请求多个地址
来源：http://rt.wgjwhj.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://je.chemitech.net.cn

PHP:  curl_multi_init() 系列
来源：http://oq.panjiajie.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wr.nszjky.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jp.521024.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ae.huixiangedu.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://kr.gzmigu.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wq.newstarts.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://yr.lnxyls.cn

================================================================================
来源：http://vi.panjiajie.cn

M. 命令行 / 进程 / 环境
来源：http://ip.huanxung.cn

================================================================================
来源：http://qx.panjiajie.cn

[M01] 读取命令行参数
来源：http://qz.9csxet.cn

Py:   sys.argv[1:]
来源：http://qa.newstarts.cn

PHP:  $argv;  $argc;
来源：http://zj.szxytkj.cn

JS:   process.argv.slice(2)
来源：http://fr.shxzukj.cn

TS:   process.argv.slice(2)
来源：http://dh.nicolike.cn

Java: args 数组（main 方法参数）
来源：http://aw.huixiangedu.cn

Go:   os.Args[1:]
来源：http://xb.521024.cn

Ruby: ARGV
来源：http://to.chemitech.net.cn

C#:   args 数组（Main 方法参数）
来源：http://xb.huanxung.cn

[M02] 读取环境变量
来源：http://ow.hahajie.cn

Py:   os.environ.get("HOME")
来源：http://vt.yuexingan06.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://kh.huanxung.cn

JS:   process.env.HOME
来源：http://ak.szsharing.cn

TS:   process.env.HOME
来源：http://be.shxzskj.cn

Java: System.getenv("HOME")
来源：http://up.9csxet.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://fz.gzmigu.cn

Ruby: ENV["HOME"]
来源：http://pl.shtwfgs.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ue.shxzukj.cn

[M03] 执行外部命令
来源：http://jm.yuexingan06.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://oi.hahajie.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://rq.nszjky.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ug.jianghongdianzi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://cg.jianghongdianzi.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://xl.bjjhwx.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://zx.bjjhwx.cn

Ruby: system("ls -l");  `ls -l`
来源：http://pw.shxzskj.cn

C#:   Process.Start("ls", "-l");
来源：http://fv.panjiajie.cn

[M04] 获取当前工作目录
来源：http://kz.shxzukj.cn

Py:   os.getcwd()
来源：http://ou.hahajie.cn

PHP:  getcwd();
来源：http://ls.bjjhwx.cn

JS:   process.cwd()
来源：http://wk.huanxung.cn

TS:   process.cwd()
来源：http://nr.panjiajie.cn

Java: Path.of("").toAbsolutePath()
来源：http://qn.panjiajie.cn

Go:   os.Getwd()
来源：http://bp.jctech888.com.cn

Ruby: Dir.pwd
来源：http://rs.bookmarksfly.cn

C#:   Directory.GetCurrentDirectory()
来源：http://zt.szxytkj.cn

[M05] 设置退出码
来源：http://ll.hnjuh.cn

Py:   sys.exit(1)
来源：http://kr.9csxet.cn

PHP:  exit(1);
来源：http://gn.szxytkj.cn

JS:   process.exit(1)
来源：http://tt.huixiangedu.cn

TS:   process.exit(1)
来源：http://re.panjiajie.cn

Java: System.exit(1)
来源：http://ox.yuntaijiaju.cn

Go:   os.Exit(1)
来源：http://kb.haigaiapp.cn

Ruby: exit 1
来源：http://lc.bjjhwx.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://yr.colortex.cn

[M06] 向标准错误输出
来源：http://wv.muxihuayi.cn

Py:   print("err", file=sys.stderr)
来源：http://mq.wgjwhj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://pd.panjiajie.cn

JS:   console.error("err")
来源：http://zo.huixiangedu.cn

TS:   console.error("err")
来源：http://ux.panjiajie.cn

Java: System.err.println("err")
来源：http://mw.szsharing.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://dh.shxzukj.cn

Ruby: warn "err"
来源：http://ng.gzmigu.cn

C#:   Console.Error.WriteLine("err")
来源：http://ge.jianghongdianzi.cn

[M07] 判断是否为主入口
来源：http://ti.wgjwhj.cn

Py:   if __name__ == "__main__":
来源：http://qz.asd995.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://iz.nicolike.cn

JS:   require.main === module
来源：http://rj.haigaiapp.cn

TS:   require.main === module
来源：http://ts.szsharing.cn

Java: public static void main(String[] args)
来源：http://xp.huixinmuqiang.cn

Go:   func main()
来源：http://sm.szxytkj.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://rm.hnjuh.cn

C#:   static void Main(string[] args)
来源：http://bu.nicolike.cn

[M08] 获取系统与运行时信息
来源：http://ac.yuexingan06.cn

Py:   platform.system();  platform.python_version()
来源：http://gx.panjiajie.cn

PHP:  PHP_OS;  phpversion();
来源：http://tp.jianghongdianzi.cn

JS:   process.platform;  process.version
来源：http://qa.521024.cn

TS:   process.platform;  process.version
来源：http://qd.hahajie.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://en.szxytkj.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://dw.nicolike.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://qr.jianghongdianzi.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://yp.colortex.cn

================================================================================
来源：http://hp.huixinmuqiang.cn

N. 数据结构与算法
来源：http://bq.gzmigu.cn

================================================================================
来源：http://ea.521024.cn

[N01] 二分查找（有序数组）
来源：http://aj.hnjuh.cn

Py:   bisect.bisect_left(arr, x)
来源：http://av.nicolike.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://lo.nszjky.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://go.jianghongdianzi.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://po.huixinmuqiang.cn

Java: Arrays.binarySearch(arr, x)
来源：http://zj.yuntaijiaju.cn

Go:   sort.SearchInts(arr, x)
来源：http://mj.muxihuayi.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://bh.szxytkj.cn

C#:   Array.BinarySearch(arr, x)
来源：http://fm.nicolike.cn

[N02] 排序（工程实践用内置实现）
来源：http://ex.huixinmuqiang.cn

Py:   sorted(arr);  arr.sort()
来源：http://zq.panjiajie.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://fh.shtwfgs.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://gu.haigaiapp.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://zo.asd995.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ns.newstarts.cn

Go:   slices.Sort(arr)
来源：http://aj.jctech888.com.cn

Ruby: arr.sort
来源：http://yx.jctech888.com.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://zg.huixinmuqiang.cn

[N03] 快速排序（分治示例）
来源：http://oa.huixinmuqiang.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://py.jianghongdianzi.cn

PHP:  // 递归实现，或用 usort
来源：http://be.colortex.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ld.yuexingan06.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ak.shxzukj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://kq.asd995.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://zz.9csxet.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xn.chemitech.net.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ph.shxzukj.cn

[N04] 斐波那契数列
来源：http://yv.asd995.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://vf.shxzskj.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://bt.shxzskj.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nl.yuexingan06.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fs.jianghongdianzi.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://yi.shxzskj.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://pn.newstarts.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ap.chemitech.net.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hj.hnjuh.cn

[N05] 最大公约数
来源：http://jo.huixinmuqiang.cn

Py:   math.gcd(a, b)
来源：http://si.newstarts.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ie.newstarts.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rg.shxzskj.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vk.shtwfgs.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://dl.9csxet.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://rw.shtwfgs.cn

Ruby: a.gcd(b)
来源：http://nl.nicolike.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://il.nszjky.cn

[N06] 判断回文字符串
来源：http://kb.jctech888.com.cn

Py:   s == s[::-1]
来源：http://dn.jctech888.com.cn

PHP:  $s === strrev($s);
来源：http://sf.lnxyls.cn

JS:   s === [...s].reverse().join("")
来源：http://bc.yuntaijiaju.cn

TS:   s === [...s].reverse().join("")
来源：http://kt.yuntaijiaju.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://nx.huanxung.cn

Go:   // 双指针从两端比较
来源：http://il.newstarts.cn

Ruby: s == s.reverse
来源：http://vp.bjjhwx.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://gd.hahajie.cn

[N07] 两数之和（返回下标）
来源：http://cy.huixinmuqiang.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mf.shxzukj.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ho.colortex.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ro.shxzskj.cn

TS:   // 手写 Map<string, number>
来源：http://dc.shtwfgs.cn

Java: // 手写 HashMap
来源：http://yo.jctech888.com.cn

Go:   // 手写 map[int]int
来源：http://kb.shxzukj.cn

Ruby: // 手写 Hash
来源：http://kh.gzmigu.cn

C#:   // 手写 Dictionary<int, int>
来源：http://wp.chemitech.net.cn

[N08] 生成全排列
来源：http://xa.wgjwhj.cn

Py:   itertools.permutations(arr)
来源：http://tw.colortex.cn

PHP:  // 手写递归交换
来源：http://ma.hnjuh.cn

JS:   // 手写回溯递归
来源：http://wq.huanxung.cn

TS:   // 手写回溯递归
来源：http://au.hahajie.cn

Java: // 手写回溯递归
来源：http://cg.521024.cn

Go:   // 手写回溯递归
来源：http://hy.muxihuayi.cn

Ruby: arr.permutation.to_a
来源：http://tg.bookmarksfly.cn

C#:   // 手写回溯递归
来源：http://kx.panjiajie.cn

[N09] 栈与队列
来源：http://yp.huanxung.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://pw.jctech888.com.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://rn.nicolike.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mv.gzmigu.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://iv.colortex.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://yb.jianghongdianzi.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://nj.nszjky.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://iz.colortex.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://uc.huixiangedu.cn

[N10] 链表节点定义
来源：http://mj.muxihuayi.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://tf.asd995.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://wu.bookmarksfly.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hf.asd995.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mn.bjjhwx.cn

Java: class Node { int v; Node next; }
来源：http://qj.hnjuh.cn

Go:   type Node struct { V int; Next *Node }
来源：http://uo.szxytkj.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://rv.jianghongdianzi.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://do.wgjwhj.cn

[N11] 二叉树中序遍历
来源：http://df.hnjuh.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://qh.bookmarksfly.cn

PHP:  // 手写递归函数
来源：http://gs.shxzskj.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://oq.panjiajie.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bf.shxzskj.cn

Java: // 手写递归
来源：http://gq.shtwfgs.cn

Go:   // 手写递归
来源：http://ah.colortex.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://cr.wgjwhj.cn

C#:   // 手写递归
来源：http://tz.huixiangedu.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hc.yuntaijiaju.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://zr.lnxyls.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://gz.huixiangedu.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tr.szsharing.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bm.szxytkj.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://pq.jctech888.com.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://dc.lnxyls.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://dd.muxihuayi.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://in.yuexingan06.cn

================================================================================
来源：http://jg.bookmarksfly.cn

O. 并发与异步
来源：http://sw.muxihuayi.cn

================================================================================
来源：http://gg.lnxyls.cn

[O01] 启动一个线程
来源：http://pa.huanxung.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://gk.hahajie.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://tv.shtwfgs.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://lq.newstarts.cn

TS:   // 同 JS
来源：http://aw.bjjhwx.cn

Java: new Thread(() -> f()).start()
来源：http://ri.muxihuayi.cn

Go:   go f()
来源：http://ux.bjjhwx.cn

Ruby: Thread.new { f }
来源：http://li.huixinmuqiang.cn

C#:   Task.Run(() => F());
来源：http://mq.newstarts.cn


<!-- 参考信息 -->