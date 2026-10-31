代发 wailian999

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://do.shxzskj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ro.panjiajie.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ql.szsharing.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://nc.bjjhwx.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wq.nszjky.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://oe.chemitech.net.cn

[K08] 二进制序列化（非 JSON）
来源：http://eu.hahajie.cn

Py:   pickle.dumps(obj)
来源：http://hf.yuexingan06.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://zg.szsharing.cn

JS:   v8.serialize(obj)        // Node
来源：http://vn.muxihuayi.cn

TS:   v8.serialize(obj)        // Node
来源：http://jf.jianghongdianzi.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://gy.gzmigu.cn

Go:   encoding/gob
来源：http://rn.yuntaijiaju.cn

Ruby: Marshal.dump(obj)
来源：http://su.huixinmuqiang.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ja.bookmarksfly.cn

================================================================================
来源：http://he.huixinmuqiang.cn

L. 网络请求
来源：http://cc.hnjuh.cn

================================================================================
来源：http://ze.szsharing.cn

[L01] 发送 GET 请求
来源：http://sr.asd995.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://da.hnjuh.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://dg.hahajie.cn

JS:   await fetch(url)
来源：http://hi.muxihuayi.cn

TS:   await fetch(url)
来源：http://hy.9csxet.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://en.yuntaijiaju.cn

Go:   resp, err := http.Get(url)
来源：http://qi.jctech888.com.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://sj.bjjhwx.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://di.hahajie.cn

[L02] 发送 POST JSON
来源：http://qe.hahajie.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ev.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qf.jctech888.com.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wl.hahajie.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ej.jctech888.com.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hi.hahajie.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://xi.shxzskj.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://iv.shxzukj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://az.jianghongdianzi.cn

[L03] 设置自定义请求头
来源：http://sy.szsharing.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://lv.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ju.newstarts.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sr.colortex.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cc.asd995.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ms.colortex.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wm.9csxet.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ns.wgjwhj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ak.colortex.cn

[L04] 设置超时
来源：http://nf.huixiangedu.cn

Py:   requests.get(url, timeout=5)
来源：http://hr.nszjky.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ga.asd995.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://eu.wgjwhj.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jt.newstarts.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://gz.shxzskj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xq.huanxung.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ga.nszjky.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://nh.shxzskj.cn

[L05] 上传文件（multipart）
来源：http://jy.nicolike.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://lg.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://zy.bjjhwx.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qj.chemitech.net.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mc.panjiajie.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://qf.nicolike.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ah.panjiajie.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://op.nicolike.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://nz.wgjwhj.cn

[L06] 解析响应为 JSON
来源：http://hn.bookmarksfly.cn

Py:   resp.json()
来源：http://qv.newstarts.cn

PHP:  json_decode($body, true);
来源：http://lr.huixinmuqiang.cn

JS:   await resp.json()
来源：http://gp.colortex.cn

TS:   await resp.json()
来源：http://uq.yuexingan06.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://uu.haigaiapp.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://gb.521024.cn

Ruby: JSON.parse(resp.body)
来源：http://cl.gzmigu.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://fw.gzmigu.cn

[L07] 处理 HTTP 状态码
来源：http://jp.gzmigu.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://is.muxihuayi.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://im.wgjwhj.cn

JS:   resp.ok;  resp.status
来源：http://sc.bookmarksfly.cn

TS:   resp.ok;  resp.status
来源：http://oe.asd995.cn

Java: resp.statusCode()
来源：http://cv.haigaiapp.cn

Go:   resp.StatusCode
来源：http://ll.nszjky.cn

Ruby: resp.code.to_i
来源：http://hh.jctech888.com.cn

C#:   (int)resp.StatusCode
来源：http://ya.szsharing.cn

[L08] 并发请求多个地址
来源：http://vh.521024.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://eh.muxihuayi.cn

PHP:  curl_multi_init() 系列
来源：http://jz.wgjwhj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gs.jianghongdianzi.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ey.bookmarksfly.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://vy.nszjky.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://tc.jctech888.com.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://kq.szsharing.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://yl.chemitech.net.cn

================================================================================
来源：http://oy.nicolike.cn

M. 命令行 / 进程 / 环境
来源：http://ou.wgjwhj.cn

================================================================================
来源：http://qv.shxzskj.cn

[M01] 读取命令行参数
来源：http://bc.szsharing.cn

Py:   sys.argv[1:]
来源：http://kd.chemitech.net.cn

PHP:  $argv;  $argc;
来源：http://ze.huixinmuqiang.cn

JS:   process.argv.slice(2)
来源：http://ec.chemitech.net.cn

TS:   process.argv.slice(2)
来源：http://ro.muxihuayi.cn

Java: args 数组（main 方法参数）
来源：http://as.chemitech.net.cn

Go:   os.Args[1:]
来源：http://bn.yuntaijiaju.cn

Ruby: ARGV
来源：http://fi.hahajie.cn

C#:   args 数组（Main 方法参数）
来源：http://zp.muxihuayi.cn

[M02] 读取环境变量
来源：http://cw.shtwfgs.cn

Py:   os.environ.get("HOME")
来源：http://wn.bjjhwx.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://kq.haigaiapp.cn

JS:   process.env.HOME
来源：http://ef.hnjuh.cn

TS:   process.env.HOME
来源：http://xi.chemitech.net.cn

Java: System.getenv("HOME")
来源：http://pk.newstarts.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ft.bjjhwx.cn

Ruby: ENV["HOME"]
来源：http://qs.lnxyls.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ih.lnxyls.cn

[M03] 执行外部命令
来源：http://wu.shxzukj.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://nq.szxytkj.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://kn.huixiangedu.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://yw.muxihuayi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://vq.lnxyls.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://jx.521024.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://gl.hnjuh.cn

Ruby: system("ls -l");  `ls -l`
来源：http://hc.shtwfgs.cn

C#:   Process.Start("ls", "-l");
来源：http://ar.lnxyls.cn

[M04] 获取当前工作目录
来源：http://og.asd995.cn

Py:   os.getcwd()
来源：http://je.bjjhwx.cn

PHP:  getcwd();
来源：http://ty.newstarts.cn

JS:   process.cwd()
来源：http://mb.shxzukj.cn

TS:   process.cwd()
来源：http://tv.lnxyls.cn

Java: Path.of("").toAbsolutePath()
来源：http://ak.haigaiapp.cn

Go:   os.Getwd()
来源：http://sl.chemitech.net.cn

Ruby: Dir.pwd
来源：http://xb.jctech888.com.cn

C#:   Directory.GetCurrentDirectory()
来源：http://xy.shtwfgs.cn

[M05] 设置退出码
来源：http://el.521024.cn

Py:   sys.exit(1)
来源：http://qt.bookmarksfly.cn

PHP:  exit(1);
来源：http://gd.bookmarksfly.cn

JS:   process.exit(1)
来源：http://dz.szxytkj.cn

TS:   process.exit(1)
来源：http://vc.gzmigu.cn

Java: System.exit(1)
来源：http://sy.newstarts.cn

Go:   os.Exit(1)
来源：http://ca.colortex.cn

Ruby: exit 1
来源：http://sk.yuexingan06.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://dz.9csxet.cn

[M06] 向标准错误输出
来源：http://rp.chemitech.net.cn

Py:   print("err", file=sys.stderr)
来源：http://vd.jianghongdianzi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://sj.shxzukj.cn

JS:   console.error("err")
来源：http://xq.hahajie.cn

TS:   console.error("err")
来源：http://os.521024.cn

Java: System.err.println("err")
来源：http://zk.haigaiapp.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://rw.yuexingan06.cn

Ruby: warn "err"
来源：http://lq.lnxyls.cn

C#:   Console.Error.WriteLine("err")
来源：http://bd.bjjhwx.cn

[M07] 判断是否为主入口
来源：http://qv.newstarts.cn

Py:   if __name__ == "__main__":
来源：http://er.bjjhwx.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ux.521024.cn

JS:   require.main === module
来源：http://kg.521024.cn

TS:   require.main === module
来源：http://yz.panjiajie.cn

Java: public static void main(String[] args)
来源：http://ty.asd995.cn

Go:   func main()
来源：http://bq.haigaiapp.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://cq.lnxyls.cn

C#:   static void Main(string[] args)
来源：http://kf.bjjhwx.cn

[M08] 获取系统与运行时信息
来源：http://ds.huanxung.cn

Py:   platform.system();  platform.python_version()
来源：http://qi.521024.cn

PHP:  PHP_OS;  phpversion();
来源：http://xh.wgjwhj.cn

JS:   process.platform;  process.version
来源：http://eu.shtwfgs.cn

TS:   process.platform;  process.version
来源：http://qt.nszjky.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://tu.huixiangedu.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://xw.huixiangedu.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ml.muxihuayi.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://cw.asd995.cn

================================================================================
来源：http://id.shxzukj.cn

N. 数据结构与算法
来源：http://hn.gzmigu.cn

================================================================================
来源：http://ln.gzmigu.cn

[N01] 二分查找（有序数组）
来源：http://wc.szxytkj.cn

Py:   bisect.bisect_left(arr, x)
来源：http://cm.szsharing.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ao.9csxet.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xv.9csxet.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sy.colortex.cn

Java: Arrays.binarySearch(arr, x)
来源：http://eq.yuexingan06.cn

Go:   sort.SearchInts(arr, x)
来源：http://td.yuntaijiaju.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://mt.9csxet.cn

C#:   Array.BinarySearch(arr, x)
来源：http://hf.newstarts.cn

[N02] 排序（工程实践用内置实现）
来源：http://ml.shxzukj.cn

Py:   sorted(arr);  arr.sort()
来源：http://ts.shtwfgs.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://yk.huanxung.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://mq.9csxet.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://yh.gzmigu.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://op.yuexingan06.cn

Go:   slices.Sort(arr)
来源：http://yq.hnjuh.cn

Ruby: arr.sort
来源：http://qr.hahajie.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://km.huixinmuqiang.cn

[N03] 快速排序（分治示例）
来源：http://cl.huixinmuqiang.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://jf.huixiangedu.cn

PHP:  // 递归实现，或用 usort
来源：http://pb.lnxyls.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gh.bookmarksfly.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ox.lnxyls.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://es.gzmigu.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://cx.nicolike.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://jm.jianghongdianzi.cn

C#:   // 手写递归，或 Array.Sort
来源：http://rn.szxytkj.cn

[N04] 斐波那契数列
来源：http://pt.huixiangedu.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://fv.asd995.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://bs.lnxyls.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://oh.hnjuh.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://un.gzmigu.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://xu.gzmigu.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://qs.521024.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://lu.huixiangedu.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://pg.asd995.cn

[N05] 最大公约数
来源：http://yr.bookmarksfly.cn

Py:   math.gcd(a, b)
来源：http://yt.huixinmuqiang.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://iy.huanxung.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ni.hahajie.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://eh.huanxung.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wb.bookmarksfly.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://jp.szsharing.cn

Ruby: a.gcd(b)
来源：http://km.shxzukj.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://sa.shxzskj.cn

[N06] 判断回文字符串
来源：http://wi.shxzukj.cn

Py:   s == s[::-1]
来源：http://ec.hahajie.cn

PHP:  $s === strrev($s);
来源：http://no.huixiangedu.cn

JS:   s === [...s].reverse().join("")
来源：http://dw.yuexingan06.cn

TS:   s === [...s].reverse().join("")
来源：http://kz.nszjky.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://po.lnxyls.cn

Go:   // 双指针从两端比较
来源：http://ku.yuntaijiaju.cn

Ruby: s == s.reverse
来源：http://mc.asd995.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ru.panjiajie.cn

[N07] 两数之和（返回下标）
来源：http://rm.lnxyls.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ja.nszjky.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://lg.huanxung.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://lx.muxihuayi.cn

TS:   // 手写 Map<string, number>
来源：http://fc.huixiangedu.cn

Java: // 手写 HashMap
来源：http://rd.yuexingan06.cn

Go:   // 手写 map[int]int
来源：http://fv.jianghongdianzi.cn

Ruby: // 手写 Hash
来源：http://hs.hahajie.cn

C#:   // 手写 Dictionary<int, int>
来源：http://bv.yuexingan06.cn

[N08] 生成全排列
来源：http://qj.newstarts.cn

Py:   itertools.permutations(arr)
来源：http://ef.huixiangedu.cn

PHP:  // 手写递归交换
来源：http://hj.shxzskj.cn

JS:   // 手写回溯递归
来源：http://mq.hnjuh.cn

TS:   // 手写回溯递归
来源：http://ma.jctech888.com.cn

Java: // 手写回溯递归
来源：http://vb.jianghongdianzi.cn

Go:   // 手写回溯递归
来源：http://dl.9csxet.cn

Ruby: arr.permutation.to_a
来源：http://ns.nszjky.cn

C#:   // 手写回溯递归
来源：http://lz.bookmarksfly.cn

[N09] 栈与队列
来源：http://by.huixiangedu.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://tm.nszjky.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://pv.jianghongdianzi.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://lw.chemitech.net.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ar.nszjky.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hg.nicolike.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://xs.gzmigu.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://dq.lnxyls.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://dr.lnxyls.cn

[N10] 链表节点定义
来源：http://bg.nszjky.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ek.bjjhwx.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://pr.hahajie.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://kq.panjiajie.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mp.muxihuayi.cn

Java: class Node { int v; Node next; }
来源：http://ms.huixiangedu.cn

Go:   type Node struct { V int; Next *Node }
来源：http://bd.shxzukj.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://hb.gzmigu.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://xg.gzmigu.cn

[N11] 二叉树中序遍历
来源：http://rm.bookmarksfly.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://im.newstarts.cn

PHP:  // 手写递归函数
来源：http://mm.panjiajie.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jy.shxzukj.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fb.lnxyls.cn

Java: // 手写递归
来源：http://hg.szsharing.cn

Go:   // 手写递归
来源：http://om.muxihuayi.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://uz.nszjky.cn

C#:   // 手写递归
来源：http://by.shtwfgs.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://kh.521024.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://fd.nicolike.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://fq.yuexingan06.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://eu.jianghongdianzi.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jk.jianghongdianzi.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://dc.nicolike.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ae.szsharing.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://xx.huanxung.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://dk.nszjky.cn

================================================================================
来源：http://fj.asd995.cn

O. 并发与异步
来源：http://tg.yuntaijiaju.cn

================================================================================
来源：http://ny.yuexingan06.cn

[O01] 启动一个线程
来源：http://am.newstarts.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ov.huixinmuqiang.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://vu.colortex.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://tr.nszjky.cn

TS:   // 同 JS
来源：http://xf.bjjhwx.cn

Java: new Thread(() -> f()).start()
来源：http://uk.lnxyls.cn

Go:   go f()
来源：http://lb.asd995.cn

Ruby: Thread.new { f }
来源：http://tn.shxzukj.cn

C#:   Task.Run(() => F());
来源：http://hs.newstarts.cn

[O02] 使用线程池
来源：http://ka.hnjuh.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://yq.asd995.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ct.yuexingan06.cn

JS:   // worker_threads 线程池
来源：http://yf.521024.cn

TS:   // worker_threads 线程池
来源：http://xl.bjjhwx.cn

Java: Executors.newFixedThreadPool(4)
来源：http://hw.szsharing.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ox.newstarts.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://vk.haigaiapp.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://aw.wgjwhj.cn

[O03] 加锁保护共享数据
来源：http://ky.haigaiapp.cn

Py:   with lock: shared += 1
来源：http://am.szsharing.cn

PHP:  // 用 flock() 做文件锁
来源：http://ob.gzmigu.cn


<!-- 参考信息 -->