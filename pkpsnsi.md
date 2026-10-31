代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://yq.asd995.cn

[K07] 进制转换
来源：http://of.521024.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://no.hahajie.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ic.huixinmuqiang.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://pq.shtwfgs.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ae.huixiangedu.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mn.muxihuayi.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://sk.yuexingan06.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://xy.panjiajie.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hj.shtwfgs.cn

[K08] 二进制序列化（非 JSON）
来源：http://zr.chemitech.net.cn

Py:   pickle.dumps(obj)
来源：http://dk.panjiajie.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://eo.hnjuh.cn

JS:   v8.serialize(obj)        // Node
来源：http://bf.wgjwhj.cn

TS:   v8.serialize(obj)        // Node
来源：http://ix.yuntaijiaju.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://yq.bjjhwx.cn

Go:   encoding/gob
来源：http://sd.huixinmuqiang.cn

Ruby: Marshal.dump(obj)
来源：http://sg.yuntaijiaju.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://aq.jctech888.com.cn

================================================================================
来源：http://vp.shtwfgs.cn

L. 网络请求
来源：http://ek.asd995.cn

================================================================================
来源：http://fp.jctech888.com.cn

[L01] 发送 GET 请求
来源：http://gd.wgjwhj.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://dd.bookmarksfly.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://az.muxihuayi.cn

JS:   await fetch(url)
来源：http://ke.asd995.cn

TS:   await fetch(url)
来源：http://lv.huanxung.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mg.9csxet.cn

Go:   resp, err := http.Get(url)
来源：http://vo.bjjhwx.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://hn.yuexingan06.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://jo.jianghongdianzi.cn

[L02] 发送 POST JSON
来源：http://nq.szsharing.cn

Py:   requests.post(url, json={"a": 1})
来源：http://lg.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://oa.szxytkj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ea.hahajie.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bk.huixiangedu.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://nd.wgjwhj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://np.chemitech.net.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://cr.bjjhwx.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://yt.nicolike.cn

[L03] 设置自定义请求头
来源：http://wg.shxzskj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://vn.szxytkj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://it.colortex.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ef.bookmarksfly.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dx.szsharing.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://xu.yuexingan06.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://sm.521024.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://jp.nszjky.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://dk.9csxet.cn

[L04] 设置超时
来源：http://xy.haigaiapp.cn

Py:   requests.get(url, timeout=5)
来源：http://uq.521024.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://gm.yuexingan06.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uh.wgjwhj.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pr.nicolike.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://xt.wgjwhj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ni.gzmigu.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://up.huanxung.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://gu.bookmarksfly.cn

[L05] 上传文件（multipart）
来源：http://iz.huixinmuqiang.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://id.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://yt.521024.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://rd.haigaiapp.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://dj.newstarts.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ek.muxihuayi.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://gk.gzmigu.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://zh.szxytkj.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://er.newstarts.cn

[L06] 解析响应为 JSON
来源：http://cw.jctech888.com.cn

Py:   resp.json()
来源：http://nm.bookmarksfly.cn

PHP:  json_decode($body, true);
来源：http://dx.jctech888.com.cn

JS:   await resp.json()
来源：http://qg.panjiajie.cn

TS:   await resp.json()
来源：http://df.jctech888.com.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://nl.shxzskj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://lp.muxihuayi.cn

Ruby: JSON.parse(resp.body)
来源：http://ud.bjjhwx.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ox.muxihuayi.cn

[L07] 处理 HTTP 状态码
来源：http://cd.gzmigu.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ad.yuexingan06.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://bi.chemitech.net.cn

JS:   resp.ok;  resp.status
来源：http://tm.shxzskj.cn

TS:   resp.ok;  resp.status
来源：http://iz.yuexingan06.cn

Java: resp.statusCode()
来源：http://xg.hnjuh.cn

Go:   resp.StatusCode
来源：http://mz.9csxet.cn

Ruby: resp.code.to_i
来源：http://zr.nicolike.cn

C#:   (int)resp.StatusCode
来源：http://hi.hahajie.cn

[L08] 并发请求多个地址
来源：http://fi.bjjhwx.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ni.jianghongdianzi.cn

PHP:  curl_multi_init() 系列
来源：http://ga.haigaiapp.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tl.jianghongdianzi.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mp.haigaiapp.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://xl.huanxung.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mr.newstarts.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vp.shtwfgs.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://je.bjjhwx.cn

================================================================================
来源：http://el.haigaiapp.cn

M. 命令行 / 进程 / 环境
来源：http://ti.haigaiapp.cn

================================================================================
来源：http://ev.newstarts.cn

[M01] 读取命令行参数
来源：http://cv.jianghongdianzi.cn

Py:   sys.argv[1:]
来源：http://ci.huixiangedu.cn

PHP:  $argv;  $argc;
来源：http://gg.chemitech.net.cn

JS:   process.argv.slice(2)
来源：http://ex.gzmigu.cn

TS:   process.argv.slice(2)
来源：http://tt.huixinmuqiang.cn

Java: args 数组（main 方法参数）
来源：http://dz.shxzukj.cn

Go:   os.Args[1:]
来源：http://pz.nszjky.cn

Ruby: ARGV
来源：http://mf.chemitech.net.cn

C#:   args 数组（Main 方法参数）
来源：http://ob.521024.cn

[M02] 读取环境变量
来源：http://fc.yuexingan06.cn

Py:   os.environ.get("HOME")
来源：http://ao.szsharing.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://gq.chemitech.net.cn

JS:   process.env.HOME
来源：http://vx.jianghongdianzi.cn

TS:   process.env.HOME
来源：http://in.asd995.cn

Java: System.getenv("HOME")
来源：http://sp.huanxung.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://zn.hahajie.cn

Ruby: ENV["HOME"]
来源：http://xn.huixiangedu.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://dn.yuntaijiaju.cn

[M03] 执行外部命令
来源：http://ie.szsharing.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://aa.nszjky.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ak.shxzskj.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://jm.yuntaijiaju.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://bz.szsharing.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://uo.bookmarksfly.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://bj.521024.cn

Ruby: system("ls -l");  `ls -l`
来源：http://rn.lnxyls.cn

C#:   Process.Start("ls", "-l");
来源：http://xt.lnxyls.cn

[M04] 获取当前工作目录
来源：http://cs.asd995.cn

Py:   os.getcwd()
来源：http://gy.lnxyls.cn

PHP:  getcwd();
来源：http://oa.jianghongdianzi.cn

JS:   process.cwd()
来源：http://qt.huixinmuqiang.cn

TS:   process.cwd()
来源：http://bo.bjjhwx.cn

Java: Path.of("").toAbsolutePath()
来源：http://ft.yuntaijiaju.cn

Go:   os.Getwd()
来源：http://um.szsharing.cn

Ruby: Dir.pwd
来源：http://zx.hnjuh.cn

C#:   Directory.GetCurrentDirectory()
来源：http://sb.yuexingan06.cn

[M05] 设置退出码
来源：http://so.yuntaijiaju.cn

Py:   sys.exit(1)
来源：http://fx.gzmigu.cn

PHP:  exit(1);
来源：http://yf.szsharing.cn

JS:   process.exit(1)
来源：http://cb.nszjky.cn

TS:   process.exit(1)
来源：http://oy.9csxet.cn

Java: System.exit(1)
来源：http://iy.huixiangedu.cn

Go:   os.Exit(1)
来源：http://mg.wgjwhj.cn

Ruby: exit 1
来源：http://jl.muxihuayi.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://tp.shxzukj.cn

[M06] 向标准错误输出
来源：http://aj.nicolike.cn

Py:   print("err", file=sys.stderr)
来源：http://hh.hnjuh.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://qa.panjiajie.cn

JS:   console.error("err")
来源：http://er.jctech888.com.cn

TS:   console.error("err")
来源：http://vo.colortex.cn

Java: System.err.println("err")
来源：http://tc.asd995.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://kf.szsharing.cn

Ruby: warn "err"
来源：http://jt.szsharing.cn

C#:   Console.Error.WriteLine("err")
来源：http://pj.huixiangedu.cn

[M07] 判断是否为主入口
来源：http://ia.wgjwhj.cn

Py:   if __name__ == "__main__":
来源：http://as.yuexingan06.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hm.colortex.cn

JS:   require.main === module
来源：http://go.hahajie.cn

TS:   require.main === module
来源：http://sg.yuntaijiaju.cn

Java: public static void main(String[] args)
来源：http://xo.lnxyls.cn

Go:   func main()
来源：http://ra.hahajie.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://tb.muxihuayi.cn

C#:   static void Main(string[] args)
来源：http://vd.9csxet.cn

[M08] 获取系统与运行时信息
来源：http://el.wgjwhj.cn

Py:   platform.system();  platform.python_version()
来源：http://gs.hahajie.cn

PHP:  PHP_OS;  phpversion();
来源：http://me.huanxung.cn

JS:   process.platform;  process.version
来源：http://pt.jianghongdianzi.cn

TS:   process.platform;  process.version
来源：http://rt.9csxet.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://sa.huixinmuqiang.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://tu.gzmigu.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ki.haigaiapp.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://kn.shtwfgs.cn

================================================================================
来源：http://iu.jctech888.com.cn

N. 数据结构与算法
来源：http://ye.panjiajie.cn

================================================================================
来源：http://va.gzmigu.cn

[N01] 二分查找（有序数组）
来源：http://fy.shxzskj.cn

Py:   bisect.bisect_left(arr, x)
来源：http://oo.huixiangedu.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://xw.nszjky.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sy.haigaiapp.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pu.colortex.cn

Java: Arrays.binarySearch(arr, x)
来源：http://mn.wgjwhj.cn

Go:   sort.SearchInts(arr, x)
来源：http://zp.yuexingan06.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ck.shxzukj.cn

C#:   Array.BinarySearch(arr, x)
来源：http://qr.asd995.cn

[N02] 排序（工程实践用内置实现）
来源：http://cn.haigaiapp.cn

Py:   sorted(arr);  arr.sort()
来源：http://hl.bjjhwx.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ur.jctech888.com.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://qg.muxihuayi.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://cd.wgjwhj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://iv.szxytkj.cn

Go:   slices.Sort(arr)
来源：http://eq.521024.cn

Ruby: arr.sort
来源：http://kp.521024.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ov.bjjhwx.cn

[N03] 快速排序（分治示例）
来源：http://rk.nicolike.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://fw.szsharing.cn

PHP:  // 递归实现，或用 usort
来源：http://zd.nszjky.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ep.521024.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gb.shtwfgs.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://qb.jianghongdianzi.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wd.jianghongdianzi.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://re.hnjuh.cn

C#:   // 手写递归，或 Array.Sort
来源：http://gh.shtwfgs.cn

[N04] 斐波那契数列
来源：http://hs.jctech888.com.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://xt.hnjuh.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://sk.chemitech.net.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sw.shxzukj.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gs.shtwfgs.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://jf.shtwfgs.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://nq.yuntaijiaju.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://gs.panjiajie.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://yu.yuntaijiaju.cn

[N05] 最大公约数
来源：http://gd.szxytkj.cn

Py:   math.gcd(a, b)
来源：http://bo.bjjhwx.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://jl.jianghongdianzi.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bx.bjjhwx.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bs.muxihuayi.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://bu.gzmigu.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wk.wgjwhj.cn

Ruby: a.gcd(b)
来源：http://fa.huanxung.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://na.muxihuayi.cn

[N06] 判断回文字符串
来源：http://sg.bjjhwx.cn

Py:   s == s[::-1]
来源：http://uh.jianghongdianzi.cn

PHP:  $s === strrev($s);
来源：http://ns.huixinmuqiang.cn

JS:   s === [...s].reverse().join("")
来源：http://df.jctech888.com.cn

TS:   s === [...s].reverse().join("")
来源：http://ew.lnxyls.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://zu.yuexingan06.cn

Go:   // 双指针从两端比较
来源：http://wj.9csxet.cn

Ruby: s == s.reverse
来源：http://yu.shxzskj.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://jx.colortex.cn

[N07] 两数之和（返回下标）
来源：http://ti.newstarts.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://rg.9csxet.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://nw.panjiajie.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://eq.panjiajie.cn

TS:   // 手写 Map<string, number>
来源：http://ei.521024.cn

Java: // 手写 HashMap
来源：http://tb.yuntaijiaju.cn

Go:   // 手写 map[int]int
来源：http://pn.yuntaijiaju.cn

Ruby: // 手写 Hash
来源：http://ow.wgjwhj.cn

C#:   // 手写 Dictionary<int, int>
来源：http://it.nszjky.cn

[N08] 生成全排列
来源：http://pd.hahajie.cn

Py:   itertools.permutations(arr)
来源：http://fm.huanxung.cn

PHP:  // 手写递归交换
来源：http://vv.shxzskj.cn

JS:   // 手写回溯递归
来源：http://bz.colortex.cn

TS:   // 手写回溯递归
来源：http://go.newstarts.cn

Java: // 手写回溯递归
来源：http://gl.gzmigu.cn

Go:   // 手写回溯递归
来源：http://nq.hahajie.cn

Ruby: arr.permutation.to_a
来源：http://sj.lnxyls.cn

C#:   // 手写回溯递归
来源：http://vu.521024.cn

[N09] 栈与队列
来源：http://oh.chemitech.net.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://oc.9csxet.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://rm.nicolike.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://im.szsharing.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://xb.yuntaijiaju.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://uz.gzmigu.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ju.huanxung.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ex.szxytkj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://uh.nicolike.cn

[N10] 链表节点定义
来源：http://qh.newstarts.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://pq.jctech888.com.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ij.nicolike.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://rn.muxihuayi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ke.bjjhwx.cn

Java: class Node { int v; Node next; }
来源：http://sl.muxihuayi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://cd.huanxung.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ok.newstarts.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://gp.haigaiapp.cn

[N11] 二叉树中序遍历
来源：http://mw.gzmigu.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://yq.521024.cn

PHP:  // 手写递归函数
来源：http://sj.bjjhwx.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://za.yuntaijiaju.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://iw.yuexingan06.cn

Java: // 手写递归
来源：http://jb.huixinmuqiang.cn

Go:   // 手写递归
来源：http://sw.bookmarksfly.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://uu.nszjky.cn

C#:   // 手写递归
来源：http://ql.chemitech.net.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://id.bookmarksfly.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://bg.chemitech.net.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ht.shxzukj.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nu.colortex.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ee.hnjuh.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://oa.asd995.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://oq.panjiajie.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://uc.bjjhwx.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://eg.wgjwhj.cn

================================================================================
来源：http://am.szsharing.cn

O. 并发与异步
来源：http://hu.huixinmuqiang.cn

================================================================================
来源：http://rg.nicolike.cn

[O01] 启动一个线程
来源：http://uy.gzmigu.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://bh.lnxyls.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://cp.shxzskj.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://jx.jctech888.com.cn

TS:   // 同 JS
来源：http://az.gzmigu.cn

Java: new Thread(() -> f()).start()
来源：http://hx.asd995.cn

Go:   go f()
来源：http://tv.hnjuh.cn

Ruby: Thread.new { f }
来源：http://lo.huixiangedu.cn

C#:   Task.Run(() => F());
来源：http://fr.szsharing.cn

[O02] 使用线程池
来源：http://cr.hahajie.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://bj.huanxung.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://dq.shxzukj.cn

JS:   // worker_threads 线程池
来源：http://gm.huixinmuqiang.cn

TS:   // worker_threads 线程池
来源：http://df.huixinmuqiang.cn

Java: Executors.newFixedThreadPool(4)
来源：http://rd.panjiajie.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wr.huixiangedu.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://up.jianghongdianzi.cn


<!-- 参考信息 -->