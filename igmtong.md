代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://tb.lnxyls.cn

[K07] 进制转换
来源：http://xt.shxzskj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ju.nicolike.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vb.haigaiapp.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://du.9csxet.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://rd.hnjuh.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://cv.newstarts.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://tr.nicolike.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ir.yuexingan06.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hg.szsharing.cn

[K08] 二进制序列化（非 JSON）
来源：http://ih.hnjuh.cn

Py:   pickle.dumps(obj)
来源：http://wv.bjjhwx.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://eg.jctech888.com.cn

JS:   v8.serialize(obj)        // Node
来源：http://yb.huanxung.cn

TS:   v8.serialize(obj)        // Node
来源：http://vj.newstarts.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://cj.9csxet.cn

Go:   encoding/gob
来源：http://no.asd995.cn

Ruby: Marshal.dump(obj)
来源：http://ff.hnjuh.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://fo.bookmarksfly.cn

================================================================================
来源：http://cm.chemitech.net.cn

L. 网络请求
来源：http://oq.bjjhwx.cn

================================================================================
来源：http://sg.lnxyls.cn

[L01] 发送 GET 请求
来源：http://tm.huanxung.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://vk.nszjky.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://oz.bookmarksfly.cn

JS:   await fetch(url)
来源：http://ms.panjiajie.cn

TS:   await fetch(url)
来源：http://ss.haigaiapp.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://vs.nszjky.cn

Go:   resp, err := http.Get(url)
来源：http://iy.huanxung.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://po.nicolike.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://uy.hahajie.cn

[L02] 发送 POST JSON
来源：http://oy.huanxung.cn

Py:   requests.post(url, json={"a": 1})
来源：http://qi.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://kk.shxzukj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ov.newstarts.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jo.nszjky.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ok.huanxung.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://pw.panjiajie.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://jj.panjiajie.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://kr.jctech888.com.cn

[L03] 设置自定义请求头
来源：http://ok.hahajie.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ck.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://dw.shxzskj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qr.yuntaijiaju.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hu.panjiajie.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://vo.szxytkj.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ly.hnjuh.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://yt.9csxet.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://sr.asd995.cn

[L04] 设置超时
来源：http://nf.chemitech.net.cn

Py:   requests.get(url, timeout=5)
来源：http://ab.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ol.chemitech.net.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://iw.newstarts.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yx.nszjky.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://yv.shxzukj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://sq.muxihuayi.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ad.panjiajie.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qk.nicolike.cn

[L05] 上传文件（multipart）
来源：http://zq.shtwfgs.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://po.521024.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://jj.9csxet.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://vm.hahajie.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ab.haigaiapp.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://bw.asd995.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ol.szxytkj.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://js.huanxung.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://pq.szxytkj.cn

[L06] 解析响应为 JSON
来源：http://ix.521024.cn

Py:   resp.json()
来源：http://dg.521024.cn

PHP:  json_decode($body, true);
来源：http://cw.szxytkj.cn

JS:   await resp.json()
来源：http://ng.muxihuayi.cn

TS:   await resp.json()
来源：http://bc.chemitech.net.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://uq.panjiajie.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mf.521024.cn

Ruby: JSON.parse(resp.body)
来源：http://np.shxzskj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://vx.gzmigu.cn

[L07] 处理 HTTP 状态码
来源：http://ha.hahajie.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://bf.wgjwhj.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://uw.muxihuayi.cn

JS:   resp.ok;  resp.status
来源：http://wb.jctech888.com.cn

TS:   resp.ok;  resp.status
来源：http://vh.bjjhwx.cn

Java: resp.statusCode()
来源：http://dn.bjjhwx.cn

Go:   resp.StatusCode
来源：http://we.hnjuh.cn

Ruby: resp.code.to_i
来源：http://kx.nicolike.cn

C#:   (int)resp.StatusCode
来源：http://pr.9csxet.cn

[L08] 并发请求多个地址
来源：http://hu.newstarts.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://oq.nszjky.cn

PHP:  curl_multi_init() 系列
来源：http://gb.jctech888.com.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nb.9csxet.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ai.szxytkj.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://xb.shxzskj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://he.shtwfgs.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zb.shxzukj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://zk.hahajie.cn

================================================================================
来源：http://kg.szsharing.cn

M. 命令行 / 进程 / 环境
来源：http://nh.colortex.cn

================================================================================
来源：http://ue.shtwfgs.cn

[M01] 读取命令行参数
来源：http://yy.asd995.cn

Py:   sys.argv[1:]
来源：http://yk.521024.cn

PHP:  $argv;  $argc;
来源：http://dm.bookmarksfly.cn

JS:   process.argv.slice(2)
来源：http://tx.huixiangedu.cn

TS:   process.argv.slice(2)
来源：http://fh.chemitech.net.cn

Java: args 数组（main 方法参数）
来源：http://go.newstarts.cn

Go:   os.Args[1:]
来源：http://by.huanxung.cn

Ruby: ARGV
来源：http://rf.521024.cn

C#:   args 数组（Main 方法参数）
来源：http://qs.newstarts.cn

[M02] 读取环境变量
来源：http://me.jianghongdianzi.cn

Py:   os.environ.get("HOME")
来源：http://fu.yuexingan06.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://tl.hahajie.cn

JS:   process.env.HOME
来源：http://an.521024.cn

TS:   process.env.HOME
来源：http://pu.wgjwhj.cn

Java: System.getenv("HOME")
来源：http://vs.colortex.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://iu.szsharing.cn

Ruby: ENV["HOME"]
来源：http://xw.muxihuayi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mo.yuexingan06.cn

[M03] 执行外部命令
来源：http://xi.yuntaijiaju.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wp.shxzukj.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://qx.huixiangedu.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://az.yuntaijiaju.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://jb.bjjhwx.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hm.muxihuayi.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://di.colortex.cn

Ruby: system("ls -l");  `ls -l`
来源：http://dk.shtwfgs.cn

C#:   Process.Start("ls", "-l");
来源：http://ho.szxytkj.cn

[M04] 获取当前工作目录
来源：http://xw.shtwfgs.cn

Py:   os.getcwd()
来源：http://yf.shtwfgs.cn

PHP:  getcwd();
来源：http://yp.hahajie.cn

JS:   process.cwd()
来源：http://sv.bookmarksfly.cn

TS:   process.cwd()
来源：http://if.shtwfgs.cn

Java: Path.of("").toAbsolutePath()
来源：http://ww.bookmarksfly.cn

Go:   os.Getwd()
来源：http://gv.hnjuh.cn

Ruby: Dir.pwd
来源：http://jl.hnjuh.cn

C#:   Directory.GetCurrentDirectory()
来源：http://bj.shtwfgs.cn

[M05] 设置退出码
来源：http://um.9csxet.cn

Py:   sys.exit(1)
来源：http://nj.szxytkj.cn

PHP:  exit(1);
来源：http://qp.shxzukj.cn

JS:   process.exit(1)
来源：http://ne.lnxyls.cn

TS:   process.exit(1)
来源：http://vg.yuntaijiaju.cn

Java: System.exit(1)
来源：http://lo.lnxyls.cn

Go:   os.Exit(1)
来源：http://jd.shxzukj.cn

Ruby: exit 1
来源：http://pf.haigaiapp.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ej.colortex.cn

[M06] 向标准错误输出
来源：http://by.haigaiapp.cn

Py:   print("err", file=sys.stderr)
来源：http://sy.yuntaijiaju.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://vg.newstarts.cn

JS:   console.error("err")
来源：http://ar.hnjuh.cn

TS:   console.error("err")
来源：http://tg.huixinmuqiang.cn

Java: System.err.println("err")
来源：http://xy.newstarts.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://vk.huanxung.cn

Ruby: warn "err"
来源：http://jp.9csxet.cn

C#:   Console.Error.WriteLine("err")
来源：http://ho.yuexingan06.cn

[M07] 判断是否为主入口
来源：http://ka.shxzskj.cn

Py:   if __name__ == "__main__":
来源：http://rl.521024.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://zq.521024.cn

JS:   require.main === module
来源：http://mv.shxzukj.cn

TS:   require.main === module
来源：http://xf.yuexingan06.cn

Java: public static void main(String[] args)
来源：http://xe.nszjky.cn

Go:   func main()
来源：http://mt.szxytkj.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://uw.bjjhwx.cn

C#:   static void Main(string[] args)
来源：http://rd.huanxung.cn

[M08] 获取系统与运行时信息
来源：http://cn.huixiangedu.cn

Py:   platform.system();  platform.python_version()
来源：http://sf.gzmigu.cn

PHP:  PHP_OS;  phpversion();
来源：http://tv.wgjwhj.cn

JS:   process.platform;  process.version
来源：http://ra.bjjhwx.cn

TS:   process.platform;  process.version
来源：http://wp.shxzskj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ri.bookmarksfly.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://up.muxihuayi.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://pd.lnxyls.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://rh.hahajie.cn

================================================================================
来源：http://cs.gzmigu.cn

N. 数据结构与算法
来源：http://mg.szsharing.cn

================================================================================
来源：http://qr.hnjuh.cn

[N01] 二分查找（有序数组）
来源：http://om.lnxyls.cn

Py:   bisect.bisect_left(arr, x)
来源：http://fv.newstarts.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://xm.bookmarksfly.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pa.szsharing.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ig.jianghongdianzi.cn

Java: Arrays.binarySearch(arr, x)
来源：http://jm.huixiangedu.cn

Go:   sort.SearchInts(arr, x)
来源：http://js.jianghongdianzi.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://gc.muxihuayi.cn

C#:   Array.BinarySearch(arr, x)
来源：http://tg.panjiajie.cn

[N02] 排序（工程实践用内置实现）
来源：http://vy.panjiajie.cn

Py:   sorted(arr);  arr.sort()
来源：http://lp.chemitech.net.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://km.hnjuh.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://jv.9csxet.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ai.9csxet.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mh.bookmarksfly.cn

Go:   slices.Sort(arr)
来源：http://ii.huixinmuqiang.cn

Ruby: arr.sort
来源：http://wq.panjiajie.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://fa.chemitech.net.cn

[N03] 快速排序（分治示例）
来源：http://qx.szsharing.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ib.haigaiapp.cn

PHP:  // 递归实现，或用 usort
来源：http://ka.yuntaijiaju.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dm.huanxung.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cp.colortex.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://sf.jctech888.com.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://xg.hnjuh.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ee.haigaiapp.cn

C#:   // 手写递归，或 Array.Sort
来源：http://rg.szxytkj.cn

[N04] 斐波那契数列
来源：http://se.muxihuayi.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://tr.huixinmuqiang.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ig.bjjhwx.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jg.chemitech.net.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://le.shxzskj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ih.shxzukj.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://gb.yuntaijiaju.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://su.521024.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://pa.bookmarksfly.cn

[N05] 最大公约数
来源：http://ro.bjjhwx.cn

Py:   math.gcd(a, b)
来源：http://sl.huixiangedu.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://lw.newstarts.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pc.huixiangedu.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bq.chemitech.net.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ym.yuntaijiaju.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://bh.szsharing.cn

Ruby: a.gcd(b)
来源：http://uj.haigaiapp.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mw.shxzskj.cn

[N06] 判断回文字符串
来源：http://xo.lnxyls.cn

Py:   s == s[::-1]
来源：http://of.szsharing.cn

PHP:  $s === strrev($s);
来源：http://va.jianghongdianzi.cn

JS:   s === [...s].reverse().join("")
来源：http://ga.jianghongdianzi.cn

TS:   s === [...s].reverse().join("")
来源：http://ol.szxytkj.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://jy.bookmarksfly.cn

Go:   // 双指针从两端比较
来源：http://vo.nicolike.cn

Ruby: s == s.reverse
来源：http://nq.hahajie.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://yq.bookmarksfly.cn

[N07] 两数之和（返回下标）
来源：http://ub.bjjhwx.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ft.shxzukj.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://rr.nicolike.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://xz.szsharing.cn

TS:   // 手写 Map<string, number>
来源：http://rj.lnxyls.cn

Java: // 手写 HashMap
来源：http://pf.lnxyls.cn

Go:   // 手写 map[int]int
来源：http://hi.bjjhwx.cn

Ruby: // 手写 Hash
来源：http://ah.huanxung.cn

C#:   // 手写 Dictionary<int, int>
来源：http://fv.wgjwhj.cn

[N08] 生成全排列
来源：http://zd.9csxet.cn

Py:   itertools.permutations(arr)
来源：http://be.521024.cn

PHP:  // 手写递归交换
来源：http://jn.szsharing.cn

JS:   // 手写回溯递归
来源：http://vt.lnxyls.cn

TS:   // 手写回溯递归
来源：http://vy.panjiajie.cn

Java: // 手写回溯递归
来源：http://lo.wgjwhj.cn

Go:   // 手写回溯递归
来源：http://kd.muxihuayi.cn

Ruby: arr.permutation.to_a
来源：http://hw.lnxyls.cn

C#:   // 手写回溯递归
来源：http://vb.nicolike.cn

[N09] 栈与队列
来源：http://su.lnxyls.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wd.szxytkj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ub.jctech888.com.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://rp.asd995.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://jt.huanxung.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://zh.shxzskj.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://gi.nicolike.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://da.huixinmuqiang.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://tq.jctech888.com.cn

[N10] 链表节点定义
来源：http://nl.shxzukj.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://os.szsharing.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://be.nszjky.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://jd.muxihuayi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hp.nszjky.cn

Java: class Node { int v; Node next; }
来源：http://sd.shtwfgs.cn

Go:   type Node struct { V int; Next *Node }
来源：http://fj.lnxyls.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ql.9csxet.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://iq.huanxung.cn

[N11] 二叉树中序遍历
来源：http://fl.huanxung.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://kh.wgjwhj.cn

PHP:  // 手写递归函数
来源：http://hi.szsharing.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ud.chemitech.net.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mz.lnxyls.cn

Java: // 手写递归
来源：http://sz.huixiangedu.cn

Go:   // 手写递归
来源：http://zn.haigaiapp.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://dh.wgjwhj.cn

C#:   // 手写递归
来源：http://hz.shxzukj.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://bl.wgjwhj.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://lv.haigaiapp.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://zk.huanxung.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ia.wgjwhj.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://io.colortex.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://tu.jctech888.com.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://xs.bjjhwx.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://gk.huixiangedu.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://zu.bookmarksfly.cn

================================================================================
来源：http://el.huanxung.cn

O. 并发与异步
来源：http://lx.gzmigu.cn

================================================================================
来源：http://fh.hnjuh.cn

[O01] 启动一个线程
来源：http://ki.shtwfgs.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://lc.nszjky.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ph.huanxung.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://kv.colortex.cn

TS:   // 同 JS
来源：http://is.nicolike.cn

Java: new Thread(() -> f()).start()
来源：http://lj.bjjhwx.cn

Go:   go f()
来源：http://rf.gzmigu.cn

Ruby: Thread.new { f }
来源：http://vl.colortex.cn

C#:   Task.Run(() => F());
来源：http://in.wgjwhj.cn

[O02] 使用线程池
来源：http://zo.bookmarksfly.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://lt.bookmarksfly.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://su.lnxyls.cn

JS:   // worker_threads 线程池
来源：http://ph.asd995.cn

TS:   // worker_threads 线程池
来源：http://to.muxihuayi.cn

Java: Executors.newFixedThreadPool(4)
来源：http://kw.shxzukj.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://qn.bjjhwx.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://kl.jianghongdianzi.cn


<!-- 参考信息 -->