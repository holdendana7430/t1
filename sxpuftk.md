代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://bk.nszjky.cn

[K07] 进制转换
来源：http://kh.hnjuh.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://jb.yuntaijiaju.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://jt.shxzukj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://gs.asd995.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://bc.bookmarksfly.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://fl.huixiangedu.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://xz.gzmigu.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://su.muxihuayi.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ut.wgjwhj.cn

[K08] 二进制序列化（非 JSON）
来源：http://mp.jianghongdianzi.cn

Py:   pickle.dumps(obj)
来源：http://eg.nicolike.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://il.huixiangedu.cn

JS:   v8.serialize(obj)        // Node
来源：http://ee.newstarts.cn

TS:   v8.serialize(obj)        // Node
来源：http://ra.shxzukj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://yh.jctech888.com.cn

Go:   encoding/gob
来源：http://qa.bjjhwx.cn

Ruby: Marshal.dump(obj)
来源：http://qd.szsharing.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://lg.szsharing.cn

================================================================================
来源：http://bb.colortex.cn

L. 网络请求
来源：http://sj.shxzukj.cn

================================================================================
来源：http://mo.9csxet.cn

[L01] 发送 GET 请求
来源：http://kt.muxihuayi.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://bd.gzmigu.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://gt.nicolike.cn

JS:   await fetch(url)
来源：http://xw.muxihuayi.cn

TS:   await fetch(url)
来源：http://tw.shxzukj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://zz.chemitech.net.cn

Go:   resp, err := http.Get(url)
来源：http://uv.nszjky.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://eg.yuexingan06.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ni.9csxet.cn

[L02] 发送 POST JSON
来源：http://ta.szxytkj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://py.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://rx.haigaiapp.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sh.hnjuh.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fi.521024.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ah.yuexingan06.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qf.9csxet.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://qy.jianghongdianzi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ux.colortex.cn

[L03] 设置自定义请求头
来源：http://yt.szsharing.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://oh.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mb.chemitech.net.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ee.nszjky.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cv.9csxet.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://dq.wgjwhj.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.szsharing.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qk.9csxet.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mp.nszjky.cn

[L04] 设置超时
来源：http://ny.yuexingan06.cn

Py:   requests.get(url, timeout=5)
来源：http://aa.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ya.chemitech.net.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hn.huixiangedu.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hm.nicolike.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://nd.szxytkj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://kj.jctech888.com.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://zj.asd995.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://go.hahajie.cn

[L05] 上传文件（multipart）
来源：http://mv.asd995.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://of.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ca.haigaiapp.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ve.szsharing.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://dl.bjjhwx.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://aa.asd995.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://uk.haigaiapp.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://dp.nszjky.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://pg.huixinmuqiang.cn

[L06] 解析响应为 JSON
来源：http://lt.jctech888.com.cn

Py:   resp.json()
来源：http://xc.newstarts.cn

PHP:  json_decode($body, true);
来源：http://rj.huixinmuqiang.cn

JS:   await resp.json()
来源：http://qr.yuexingan06.cn

TS:   await resp.json()
来源：http://fe.nszjky.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://en.lnxyls.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://fw.chemitech.net.cn

Ruby: JSON.parse(resp.body)
来源：http://ro.shtwfgs.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ct.shtwfgs.cn

[L07] 处理 HTTP 状态码
来源：http://je.lnxyls.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ag.wgjwhj.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://of.lnxyls.cn

JS:   resp.ok;  resp.status
来源：http://yl.yuexingan06.cn

TS:   resp.ok;  resp.status
来源：http://qv.hnjuh.cn

Java: resp.statusCode()
来源：http://jl.szsharing.cn

Go:   resp.StatusCode
来源：http://qt.colortex.cn

Ruby: resp.code.to_i
来源：http://xc.jianghongdianzi.cn

C#:   (int)resp.StatusCode
来源：http://ml.szxytkj.cn

[L08] 并发请求多个地址
来源：http://ig.haigaiapp.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://vg.shxzukj.cn

PHP:  curl_multi_init() 系列
来源：http://uc.521024.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://uh.hahajie.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fz.jctech888.com.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hx.huanxung.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hw.9csxet.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://qn.shxzukj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://gd.nicolike.cn

================================================================================
来源：http://uh.huixinmuqiang.cn

M. 命令行 / 进程 / 环境
来源：http://aw.colortex.cn

================================================================================
来源：http://rj.nicolike.cn

[M01] 读取命令行参数
来源：http://li.muxihuayi.cn

Py:   sys.argv[1:]
来源：http://rr.newstarts.cn

PHP:  $argv;  $argc;
来源：http://ep.nszjky.cn

JS:   process.argv.slice(2)
来源：http://yj.shxzskj.cn

TS:   process.argv.slice(2)
来源：http://vq.hnjuh.cn

Java: args 数组（main 方法参数）
来源：http://vv.shxzskj.cn

Go:   os.Args[1:]
来源：http://xg.yuexingan06.cn

Ruby: ARGV
来源：http://co.haigaiapp.cn

C#:   args 数组（Main 方法参数）
来源：http://qm.521024.cn

[M02] 读取环境变量
来源：http://rw.shxzukj.cn

Py:   os.environ.get("HOME")
来源：http://he.huanxung.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mk.shxzskj.cn

JS:   process.env.HOME
来源：http://ac.yuexingan06.cn

TS:   process.env.HOME
来源：http://pr.hnjuh.cn

Java: System.getenv("HOME")
来源：http://ml.gzmigu.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://dr.hahajie.cn

Ruby: ENV["HOME"]
来源：http://fu.yuntaijiaju.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://it.shtwfgs.cn

[M03] 执行外部命令
来源：http://xj.chemitech.net.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://jo.jctech888.com.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://dd.newstarts.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ru.bookmarksfly.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://yd.asd995.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ek.huixiangedu.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://im.huixinmuqiang.cn

Ruby: system("ls -l");  `ls -l`
来源：http://zy.newstarts.cn

C#:   Process.Start("ls", "-l");
来源：http://sy.9csxet.cn

[M04] 获取当前工作目录
来源：http://zg.muxihuayi.cn

Py:   os.getcwd()
来源：http://fv.szxytkj.cn

PHP:  getcwd();
来源：http://oy.yuexingan06.cn

JS:   process.cwd()
来源：http://tg.muxihuayi.cn

TS:   process.cwd()
来源：http://rh.shxzukj.cn

Java: Path.of("").toAbsolutePath()
来源：http://xi.shxzskj.cn

Go:   os.Getwd()
来源：http://dn.haigaiapp.cn

Ruby: Dir.pwd
来源：http://vb.huixinmuqiang.cn

C#:   Directory.GetCurrentDirectory()
来源：http://up.shxzukj.cn

[M05] 设置退出码
来源：http://lv.asd995.cn

Py:   sys.exit(1)
来源：http://fq.521024.cn

PHP:  exit(1);
来源：http://eb.gzmigu.cn

JS:   process.exit(1)
来源：http://nc.colortex.cn

TS:   process.exit(1)
来源：http://pt.asd995.cn

Java: System.exit(1)
来源：http://lv.newstarts.cn

Go:   os.Exit(1)
来源：http://fm.shxzukj.cn

Ruby: exit 1
来源：http://wt.bookmarksfly.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://nc.huanxung.cn

[M06] 向标准错误输出
来源：http://pb.9csxet.cn

Py:   print("err", file=sys.stderr)
来源：http://or.lnxyls.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://hr.colortex.cn

JS:   console.error("err")
来源：http://uf.bjjhwx.cn

TS:   console.error("err")
来源：http://cg.muxihuayi.cn

Java: System.err.println("err")
来源：http://ls.nszjky.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://pn.newstarts.cn

Ruby: warn "err"
来源：http://yq.colortex.cn

C#:   Console.Error.WriteLine("err")
来源：http://vd.panjiajie.cn

[M07] 判断是否为主入口
来源：http://oi.lnxyls.cn

Py:   if __name__ == "__main__":
来源：http://pu.bjjhwx.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://dc.jianghongdianzi.cn

JS:   require.main === module
来源：http://sv.521024.cn

TS:   require.main === module
来源：http://yp.szxytkj.cn

Java: public static void main(String[] args)
来源：http://rp.shtwfgs.cn

Go:   func main()
来源：http://ry.szxytkj.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://fh.nszjky.cn

C#:   static void Main(string[] args)
来源：http://vu.shtwfgs.cn

[M08] 获取系统与运行时信息
来源：http://pj.panjiajie.cn

Py:   platform.system();  platform.python_version()
来源：http://dq.bookmarksfly.cn

PHP:  PHP_OS;  phpversion();
来源：http://zc.521024.cn

JS:   process.platform;  process.version
来源：http://jx.newstarts.cn

TS:   process.platform;  process.version
来源：http://kj.newstarts.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ws.yuexingan06.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://bv.bookmarksfly.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://bx.bookmarksfly.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://xv.jctech888.com.cn

================================================================================
来源：http://jx.nszjky.cn

N. 数据结构与算法
来源：http://xx.newstarts.cn

================================================================================
来源：http://pc.9csxet.cn

[N01] 二分查找（有序数组）
来源：http://gh.nicolike.cn

Py:   bisect.bisect_left(arr, x)
来源：http://wy.haigaiapp.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://fz.szxytkj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fg.shtwfgs.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wu.newstarts.cn

Java: Arrays.binarySearch(arr, x)
来源：http://af.bjjhwx.cn

Go:   sort.SearchInts(arr, x)
来源：http://of.yuntaijiaju.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://mm.panjiajie.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ow.nicolike.cn

[N02] 排序（工程实践用内置实现）
来源：http://qw.colortex.cn

Py:   sorted(arr);  arr.sort()
来源：http://ev.huixiangedu.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://tz.panjiajie.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ly.gzmigu.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://cp.9csxet.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://sl.asd995.cn

Go:   slices.Sort(arr)
来源：http://rl.newstarts.cn

Ruby: arr.sort
来源：http://bf.nicolike.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://yo.nszjky.cn

[N03] 快速排序（分治示例）
来源：http://ei.hahajie.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ik.hahajie.cn

PHP:  // 递归实现，或用 usort
来源：http://jy.huixinmuqiang.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ld.gzmigu.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cu.wgjwhj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://xb.hnjuh.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://yh.panjiajie.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://zv.huanxung.cn

C#:   // 手写递归，或 Array.Sort
来源：http://xp.haigaiapp.cn

[N04] 斐波那契数列
来源：http://tu.lnxyls.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://dc.szxytkj.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ag.newstarts.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fs.hahajie.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ca.lnxyls.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://pt.haigaiapp.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://dn.bjjhwx.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://uq.huixinmuqiang.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://iw.hahajie.cn

[N05] 最大公约数
来源：http://kj.bjjhwx.cn

Py:   math.gcd(a, b)
来源：http://av.muxihuayi.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://nb.huixinmuqiang.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wx.szsharing.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qm.wgjwhj.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://rk.bjjhwx.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://no.bookmarksfly.cn

Ruby: a.gcd(b)
来源：http://cq.szsharing.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ka.panjiajie.cn

[N06] 判断回文字符串
来源：http://hw.colortex.cn

Py:   s == s[::-1]
来源：http://sj.haigaiapp.cn

PHP:  $s === strrev($s);
来源：http://lu.hahajie.cn

JS:   s === [...s].reverse().join("")
来源：http://no.huanxung.cn

TS:   s === [...s].reverse().join("")
来源：http://ci.huixinmuqiang.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xl.asd995.cn

Go:   // 双指针从两端比较
来源：http://mw.nszjky.cn

Ruby: s == s.reverse
来源：http://vr.shxzskj.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://tb.lnxyls.cn

[N07] 两数之和（返回下标）
来源：http://lz.panjiajie.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hn.szsharing.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://dj.yuexingan06.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://gx.asd995.cn

TS:   // 手写 Map<string, number>
来源：http://kd.colortex.cn

Java: // 手写 HashMap
来源：http://wm.nicolike.cn

Go:   // 手写 map[int]int
来源：http://mz.haigaiapp.cn

Ruby: // 手写 Hash
来源：http://ot.bjjhwx.cn

C#:   // 手写 Dictionary<int, int>
来源：http://wx.nszjky.cn

[N08] 生成全排列
来源：http://ak.newstarts.cn

Py:   itertools.permutations(arr)
来源：http://aq.huixinmuqiang.cn

PHP:  // 手写递归交换
来源：http://bp.hnjuh.cn

JS:   // 手写回溯递归
来源：http://ra.yuntaijiaju.cn

TS:   // 手写回溯递归
来源：http://ev.hahajie.cn

Java: // 手写回溯递归
来源：http://ss.hahajie.cn

Go:   // 手写回溯递归
来源：http://bu.yuexingan06.cn

Ruby: arr.permutation.to_a
来源：http://ee.szxytkj.cn

C#:   // 手写回溯递归
来源：http://jw.gzmigu.cn

[N09] 栈与队列
来源：http://qj.wgjwhj.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ru.jctech888.com.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://yi.lnxyls.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ug.newstarts.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://xv.szsharing.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ou.asd995.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://pp.jctech888.com.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wf.huanxung.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://tx.nszjky.cn

[N10] 链表节点定义
来源：http://tr.jianghongdianzi.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ni.huixiangedu.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://yh.yuexingan06.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://xq.newstarts.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://kp.jctech888.com.cn

Java: class Node { int v; Node next; }
来源：http://lp.colortex.cn

Go:   type Node struct { V int; Next *Node }
来源：http://oo.bjjhwx.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://qx.shtwfgs.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://lt.huixinmuqiang.cn

[N11] 二叉树中序遍历
来源：http://sk.szxytkj.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://lf.521024.cn

PHP:  // 手写递归函数
来源：http://kk.bjjhwx.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://iv.lnxyls.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yw.szxytkj.cn

Java: // 手写递归
来源：http://aw.haigaiapp.cn

Go:   // 手写递归
来源：http://ym.asd995.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://go.nszjky.cn

C#:   // 手写递归
来源：http://da.jctech888.com.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://xu.hnjuh.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://lp.haigaiapp.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ue.huixiangedu.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qx.huixiangedu.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ek.huixinmuqiang.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://zi.bjjhwx.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://fb.wgjwhj.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ag.yuntaijiaju.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://kk.shxzukj.cn

================================================================================
来源：http://wa.yuntaijiaju.cn

O. 并发与异步
来源：http://aw.muxihuayi.cn

================================================================================
来源：http://ct.muxihuayi.cn

[O01] 启动一个线程
来源：http://te.yuexingan06.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://tg.chemitech.net.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://sq.huixinmuqiang.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://zp.shxzukj.cn

TS:   // 同 JS
来源：http://wg.9csxet.cn

Java: new Thread(() -> f()).start()
来源：http://ny.shtwfgs.cn

Go:   go f()
来源：http://fa.haigaiapp.cn

Ruby: Thread.new { f }
来源：http://dw.9csxet.cn

C#:   Task.Run(() => F());
来源：http://bt.szsharing.cn

[O02] 使用线程池
来源：http://zu.huanxung.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://qa.jctech888.com.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://vx.shtwfgs.cn

JS:   // worker_threads 线程池
来源：http://rt.huanxung.cn

TS:   // worker_threads 线程池
来源：http://hp.gzmigu.cn

Java: Executors.newFixedThreadPool(4)
来源：http://jg.wgjwhj.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://nm.shxzskj.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://rx.shtwfgs.cn


<!-- 参考信息 -->