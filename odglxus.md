代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wj.haigaiapp.cn

[K07] 进制转换
来源：http://mz.wgjwhj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://sf.lnxyls.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ia.huixinmuqiang.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://og.shxzskj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://yv.szxytkj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mz.muxihuayi.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://xk.yuntaijiaju.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://iu.9csxet.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ni.szsharing.cn

[K08] 二进制序列化（非 JSON）
来源：http://ob.shxzskj.cn

Py:   pickle.dumps(obj)
来源：http://ls.newstarts.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://tt.panjiajie.cn

JS:   v8.serialize(obj)        // Node
来源：http://ol.shxzukj.cn

TS:   v8.serialize(obj)        // Node
来源：http://bq.lnxyls.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://de.newstarts.cn

Go:   encoding/gob
来源：http://kd.muxihuayi.cn

Ruby: Marshal.dump(obj)
来源：http://vy.521024.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://lt.szxytkj.cn

================================================================================
来源：http://eq.jctech888.com.cn

L. 网络请求
来源：http://px.panjiajie.cn

================================================================================
来源：http://jw.huanxung.cn

[L01] 发送 GET 请求
来源：http://mu.yuexingan06.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://oi.panjiajie.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ey.huixiangedu.cn

JS:   await fetch(url)
来源：http://ap.hnjuh.cn

TS:   await fetch(url)
来源：http://eo.wgjwhj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://kz.nszjky.cn

Go:   resp, err := http.Get(url)
来源：http://sp.panjiajie.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://de.colortex.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://uz.huixinmuqiang.cn

[L02] 发送 POST JSON
来源：http://qb.nszjky.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ti.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://yq.panjiajie.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ue.asd995.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xf.panjiajie.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hs.newstarts.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://kl.9csxet.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://da.yuexingan06.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://za.hnjuh.cn

[L03] 设置自定义请求头
来源：http://dd.chemitech.net.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://xy.szxytkj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://jz.szsharing.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://oo.huixinmuqiang.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vn.yuexingan06.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://sy.9csxet.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jr.colortex.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://er.bookmarksfly.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://qw.haigaiapp.cn

[L04] 设置超时
来源：http://af.bjjhwx.cn

Py:   requests.get(url, timeout=5)
来源：http://zb.hnjuh.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://gw.haigaiapp.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ow.colortex.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rl.huixiangedu.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://bn.nszjky.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://dw.colortex.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://tq.szsharing.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qx.wgjwhj.cn

[L05] 上传文件（multipart）
来源：http://by.bjjhwx.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wn.huixiangedu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://zy.szxytkj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wl.huixinmuqiang.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://sz.521024.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://zz.jianghongdianzi.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ta.bookmarksfly.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://di.newstarts.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hg.chemitech.net.cn

[L06] 解析响应为 JSON
来源：http://lr.newstarts.cn

Py:   resp.json()
来源：http://mj.huixiangedu.cn

PHP:  json_decode($body, true);
来源：http://wf.nszjky.cn

JS:   await resp.json()
来源：http://ds.hnjuh.cn

TS:   await resp.json()
来源：http://kt.newstarts.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://id.yuntaijiaju.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://tn.nszjky.cn

Ruby: JSON.parse(resp.body)
来源：http://hq.nszjky.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://fd.shtwfgs.cn

[L07] 处理 HTTP 状态码
来源：http://mp.huanxung.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ay.hnjuh.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://uc.muxihuayi.cn

JS:   resp.ok;  resp.status
来源：http://nk.9csxet.cn

TS:   resp.ok;  resp.status
来源：http://ux.huixiangedu.cn

Java: resp.statusCode()
来源：http://on.huixiangedu.cn

Go:   resp.StatusCode
来源：http://zd.asd995.cn

Ruby: resp.code.to_i
来源：http://xa.yuntaijiaju.cn

C#:   (int)resp.StatusCode
来源：http://up.shxzukj.cn

[L08] 并发请求多个地址
来源：http://kp.wgjwhj.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ue.yuexingan06.cn

PHP:  curl_multi_init() 系列
来源：http://lj.bookmarksfly.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wb.colortex.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://du.521024.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ie.yuexingan06.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://sv.huanxung.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://pg.nicolike.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ni.shxzskj.cn

================================================================================
来源：http://wk.szsharing.cn

M. 命令行 / 进程 / 环境
来源：http://vr.colortex.cn

================================================================================
来源：http://kd.nszjky.cn

[M01] 读取命令行参数
来源：http://kl.lnxyls.cn

Py:   sys.argv[1:]
来源：http://tt.shxzskj.cn

PHP:  $argv;  $argc;
来源：http://mo.szsharing.cn

JS:   process.argv.slice(2)
来源：http://jv.nszjky.cn

TS:   process.argv.slice(2)
来源：http://ej.wgjwhj.cn

Java: args 数组（main 方法参数）
来源：http://ry.jctech888.com.cn

Go:   os.Args[1:]
来源：http://jc.huixiangedu.cn

Ruby: ARGV
来源：http://mr.nicolike.cn

C#:   args 数组（Main 方法参数）
来源：http://cy.shxzskj.cn

[M02] 读取环境变量
来源：http://hl.nicolike.cn

Py:   os.environ.get("HOME")
来源：http://eo.bjjhwx.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://fb.newstarts.cn

JS:   process.env.HOME
来源：http://tq.gzmigu.cn

TS:   process.env.HOME
来源：http://es.asd995.cn

Java: System.getenv("HOME")
来源：http://uv.gzmigu.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://en.huanxung.cn

Ruby: ENV["HOME"]
来源：http://pr.colortex.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://am.huanxung.cn

[M03] 执行外部命令
来源：http://uo.colortex.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wl.colortex.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://as.yuntaijiaju.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://li.huixiangedu.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://os.wgjwhj.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://rf.huixinmuqiang.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://go.yuexingan06.cn

Ruby: system("ls -l");  `ls -l`
来源：http://qa.muxihuayi.cn

C#:   Process.Start("ls", "-l");
来源：http://vo.haigaiapp.cn

[M04] 获取当前工作目录
来源：http://rx.asd995.cn

Py:   os.getcwd()
来源：http://jz.chemitech.net.cn

PHP:  getcwd();
来源：http://qq.bjjhwx.cn

JS:   process.cwd()
来源：http://qe.shtwfgs.cn

TS:   process.cwd()
来源：http://kk.huixiangedu.cn

Java: Path.of("").toAbsolutePath()
来源：http://vq.wgjwhj.cn

Go:   os.Getwd()
来源：http://ge.szsharing.cn

Ruby: Dir.pwd
来源：http://fy.hnjuh.cn

C#:   Directory.GetCurrentDirectory()
来源：http://pu.asd995.cn

[M05] 设置退出码
来源：http://qb.asd995.cn

Py:   sys.exit(1)
来源：http://fu.gzmigu.cn

PHP:  exit(1);
来源：http://sv.nszjky.cn

JS:   process.exit(1)
来源：http://kl.shtwfgs.cn

TS:   process.exit(1)
来源：http://tn.nicolike.cn

Java: System.exit(1)
来源：http://ya.haigaiapp.cn

Go:   os.Exit(1)
来源：http://lq.wgjwhj.cn

Ruby: exit 1
来源：http://ra.hahajie.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://po.nicolike.cn

[M06] 向标准错误输出
来源：http://hn.lnxyls.cn

Py:   print("err", file=sys.stderr)
来源：http://mi.jianghongdianzi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://pv.huanxung.cn

JS:   console.error("err")
来源：http://yi.huanxung.cn

TS:   console.error("err")
来源：http://ub.nicolike.cn

Java: System.err.println("err")
来源：http://ai.lnxyls.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ex.yuexingan06.cn

Ruby: warn "err"
来源：http://er.asd995.cn

C#:   Console.Error.WriteLine("err")
来源：http://ny.gzmigu.cn

[M07] 判断是否为主入口
来源：http://cz.jctech888.com.cn

Py:   if __name__ == "__main__":
来源：http://lw.lnxyls.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://lb.521024.cn

JS:   require.main === module
来源：http://gr.9csxet.cn

TS:   require.main === module
来源：http://no.lnxyls.cn

Java: public static void main(String[] args)
来源：http://af.yuntaijiaju.cn

Go:   func main()
来源：http://di.yuexingan06.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://nj.huanxung.cn

C#:   static void Main(string[] args)
来源：http://im.panjiajie.cn

[M08] 获取系统与运行时信息
来源：http://mj.shtwfgs.cn

Py:   platform.system();  platform.python_version()
来源：http://zj.panjiajie.cn

PHP:  PHP_OS;  phpversion();
来源：http://xl.haigaiapp.cn

JS:   process.platform;  process.version
来源：http://wr.shtwfgs.cn

TS:   process.platform;  process.version
来源：http://mx.lnxyls.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://sf.hahajie.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://tb.haigaiapp.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://if.haigaiapp.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://dv.shxzskj.cn

================================================================================
来源：http://sy.szxytkj.cn

N. 数据结构与算法
来源：http://ee.yuntaijiaju.cn

================================================================================
来源：http://wn.szsharing.cn

[N01] 二分查找（有序数组）
来源：http://jb.jctech888.com.cn

Py:   bisect.bisect_left(arr, x)
来源：http://fb.newstarts.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://df.yuexingan06.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kf.bookmarksfly.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://on.lnxyls.cn

Java: Arrays.binarySearch(arr, x)
来源：http://wu.nicolike.cn

Go:   sort.SearchInts(arr, x)
来源：http://uc.wgjwhj.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://hh.bjjhwx.cn

C#:   Array.BinarySearch(arr, x)
来源：http://xg.bjjhwx.cn

[N02] 排序（工程实践用内置实现）
来源：http://me.wgjwhj.cn

Py:   sorted(arr);  arr.sort()
来源：http://ls.lnxyls.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://zu.yuntaijiaju.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://zf.hnjuh.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://gt.hnjuh.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://go.bookmarksfly.cn

Go:   slices.Sort(arr)
来源：http://gt.nicolike.cn

Ruby: arr.sort
来源：http://jg.huixinmuqiang.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ij.521024.cn

[N03] 快速排序（分治示例）
来源：http://kf.chemitech.net.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://um.jctech888.com.cn

PHP:  // 递归实现，或用 usort
来源：http://ls.jianghongdianzi.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gg.wgjwhj.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zm.huanxung.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://pc.shxzukj.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://qi.huixiangedu.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ey.chemitech.net.cn

C#:   // 手写递归，或 Array.Sort
来源：http://xp.bookmarksfly.cn

[N04] 斐波那契数列
来源：http://uc.wgjwhj.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://tc.gzmigu.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://kh.nszjky.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://as.shxzukj.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://au.nszjky.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://xv.yuexingan06.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://yv.panjiajie.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://xo.wgjwhj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://zo.colortex.cn

[N05] 最大公约数
来源：http://qp.bookmarksfly.cn

Py:   math.gcd(a, b)
来源：http://wz.521024.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://jl.huanxung.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mk.huixinmuqiang.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ll.muxihuayi.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://nw.jctech888.com.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://nh.shxzukj.cn

Ruby: a.gcd(b)
来源：http://as.colortex.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://sp.shxzskj.cn

[N06] 判断回文字符串
来源：http://ry.huixiangedu.cn

Py:   s == s[::-1]
来源：http://dt.panjiajie.cn

PHP:  $s === strrev($s);
来源：http://qa.huixinmuqiang.cn

JS:   s === [...s].reverse().join("")
来源：http://ms.huixinmuqiang.cn

TS:   s === [...s].reverse().join("")
来源：http://hw.nszjky.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ed.9csxet.cn

Go:   // 双指针从两端比较
来源：http://ol.huanxung.cn

Ruby: s == s.reverse
来源：http://ni.nicolike.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://wp.chemitech.net.cn

[N07] 两数之和（返回下标）
来源：http://gm.huanxung.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://np.szxytkj.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://lj.shxzukj.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://vc.521024.cn

TS:   // 手写 Map<string, number>
来源：http://en.shxzskj.cn

Java: // 手写 HashMap
来源：http://ru.lnxyls.cn

Go:   // 手写 map[int]int
来源：http://fz.yuntaijiaju.cn

Ruby: // 手写 Hash
来源：http://ci.bookmarksfly.cn

C#:   // 手写 Dictionary<int, int>
来源：http://gi.hahajie.cn

[N08] 生成全排列
来源：http://oz.muxihuayi.cn

Py:   itertools.permutations(arr)
来源：http://uk.szxytkj.cn

PHP:  // 手写递归交换
来源：http://nt.huixinmuqiang.cn

JS:   // 手写回溯递归
来源：http://xk.newstarts.cn

TS:   // 手写回溯递归
来源：http://jr.nszjky.cn

Java: // 手写回溯递归
来源：http://jf.bjjhwx.cn

Go:   // 手写回溯递归
来源：http://ny.panjiajie.cn

Ruby: arr.permutation.to_a
来源：http://jr.nszjky.cn

C#:   // 手写回溯递归
来源：http://vh.huixiangedu.cn

[N09] 栈与队列
来源：http://lp.newstarts.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://uo.huixiangedu.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ly.gzmigu.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://fl.chemitech.net.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://qe.haigaiapp.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://bx.colortex.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://bm.521024.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://dh.panjiajie.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://qq.colortex.cn

[N10] 链表节点定义
来源：http://ba.521024.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mt.shxzskj.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://uc.jctech888.com.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://xc.yuexingan06.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ib.bjjhwx.cn

Java: class Node { int v; Node next; }
来源：http://so.huanxung.cn

Go:   type Node struct { V int; Next *Node }
来源：http://eq.hahajie.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ow.newstarts.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://rh.521024.cn

[N11] 二叉树中序遍历
来源：http://ao.huanxung.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ra.szsharing.cn

PHP:  // 手写递归函数
来源：http://xo.9csxet.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ev.yuexingan06.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ta.lnxyls.cn

Java: // 手写递归
来源：http://lp.gzmigu.cn

Go:   // 手写递归
来源：http://ku.chemitech.net.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://uj.panjiajie.cn

C#:   // 手写递归
来源：http://ux.huixinmuqiang.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mg.huanxung.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ll.hahajie.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://vd.szxytkj.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zu.lnxyls.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zj.yuntaijiaju.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://jp.panjiajie.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://yj.shtwfgs.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://gc.lnxyls.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ec.muxihuayi.cn

================================================================================
来源：http://ws.yuexingan06.cn

O. 并发与异步
来源：http://td.szsharing.cn

================================================================================
来源：http://zr.jianghongdianzi.cn

[O01] 启动一个线程
来源：http://qh.shxzukj.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://fb.nszjky.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wq.huanxung.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://zw.gzmigu.cn

TS:   // 同 JS
来源：http://qy.haigaiapp.cn

Java: new Thread(() -> f()).start()
来源：http://eg.chemitech.net.cn

Go:   go f()
来源：http://wl.shxzukj.cn

Ruby: Thread.new { f }
来源：http://ul.jianghongdianzi.cn

C#:   Task.Run(() => F());
来源：http://ky.521024.cn

[O02] 使用线程池
来源：http://jl.521024.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://dp.521024.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://tc.hnjuh.cn

JS:   // worker_threads 线程池
来源：http://or.jianghongdianzi.cn

TS:   // worker_threads 线程池
来源：http://hk.hnjuh.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ia.gzmigu.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ft.shxzskj.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://lz.muxihuayi.cn


<!-- 参考信息 -->