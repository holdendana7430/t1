代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://es.muxihuayi.cn

[K07] 进制转换
来源：http://pw.muxihuayi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://yy.shtwfgs.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://cd.shxzskj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://rx.hahajie.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://nz.wgjwhj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ac.huixinmuqiang.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://bv.haigaiapp.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://um.chemitech.net.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wa.521024.cn

[K08] 二进制序列化（非 JSON）
来源：http://zi.chemitech.net.cn

Py:   pickle.dumps(obj)
来源：http://ki.gzmigu.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://fo.wgjwhj.cn

JS:   v8.serialize(obj)        // Node
来源：http://cn.huixinmuqiang.cn

TS:   v8.serialize(obj)        // Node
来源：http://cd.colortex.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://gb.nszjky.cn

Go:   encoding/gob
来源：http://ls.bookmarksfly.cn

Ruby: Marshal.dump(obj)
来源：http://hg.yuntaijiaju.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://do.gzmigu.cn

================================================================================
来源：http://pz.bjjhwx.cn

L. 网络请求
来源：http://hq.yuexingan06.cn

================================================================================
来源：http://lp.jctech888.com.cn

[L01] 发送 GET 请求
来源：http://ff.nicolike.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://zq.jctech888.com.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://dp.huanxung.cn

JS:   await fetch(url)
来源：http://di.nszjky.cn

TS:   await fetch(url)
来源：http://fp.huixinmuqiang.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://kn.szxytkj.cn

Go:   resp, err := http.Get(url)
来源：http://vo.newstarts.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://gg.9csxet.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://nd.colortex.cn

[L02] 发送 POST JSON
来源：http://rq.chemitech.net.cn

Py:   requests.post(url, json={"a": 1})
来源：http://jx.wgjwhj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://pi.shxzukj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://eb.yuntaijiaju.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ia.bookmarksfly.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ar.nszjky.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://za.szsharing.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ge.newstarts.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://lu.panjiajie.cn

[L03] 设置自定义请求头
来源：http://jv.521024.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://zi.shtwfgs.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hq.asd995.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://af.panjiajie.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ax.szsharing.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wc.lnxyls.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://on.huanxung.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ih.huixinmuqiang.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://gs.shtwfgs.cn

[L04] 设置超时
来源：http://gb.newstarts.cn

Py:   requests.get(url, timeout=5)
来源：http://bi.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://cc.muxihuayi.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gi.shxzskj.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fc.asd995.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://fx.shxzukj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ta.huixiangedu.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://le.gzmigu.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://xq.huanxung.cn

[L05] 上传文件（multipart）
来源：http://bi.hahajie.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://vr.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://js.hahajie.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hf.shxzukj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://pe.panjiajie.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://fq.jianghongdianzi.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://kr.hnjuh.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wb.jctech888.com.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://oy.jctech888.com.cn

[L06] 解析响应为 JSON
来源：http://ua.huixinmuqiang.cn

Py:   resp.json()
来源：http://gn.muxihuayi.cn

PHP:  json_decode($body, true);
来源：http://nd.jctech888.com.cn

JS:   await resp.json()
来源：http://ua.shxzukj.cn

TS:   await resp.json()
来源：http://vb.hahajie.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://eh.muxihuayi.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://zf.bjjhwx.cn

Ruby: JSON.parse(resp.body)
来源：http://uy.shxzskj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://nb.shxzskj.cn

[L07] 处理 HTTP 状态码
来源：http://dc.gzmigu.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://js.colortex.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://os.szxytkj.cn

JS:   resp.ok;  resp.status
来源：http://mk.newstarts.cn

TS:   resp.ok;  resp.status
来源：http://ji.wgjwhj.cn

Java: resp.statusCode()
来源：http://qa.wgjwhj.cn

Go:   resp.StatusCode
来源：http://dg.nicolike.cn

Ruby: resp.code.to_i
来源：http://cv.yuexingan06.cn

C#:   (int)resp.StatusCode
来源：http://bf.521024.cn

[L08] 并发请求多个地址
来源：http://ur.shtwfgs.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://el.yuexingan06.cn

PHP:  curl_multi_init() 系列
来源：http://pa.nszjky.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qs.szsharing.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://po.nicolike.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ra.jctech888.com.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://og.nicolike.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zm.yuexingan06.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://so.hahajie.cn

================================================================================
来源：http://ux.bookmarksfly.cn

M. 命令行 / 进程 / 环境
来源：http://bz.chemitech.net.cn

================================================================================
来源：http://sw.lnxyls.cn

[M01] 读取命令行参数
来源：http://vf.panjiajie.cn

Py:   sys.argv[1:]
来源：http://zl.muxihuayi.cn

PHP:  $argv;  $argc;
来源：http://qm.szsharing.cn

JS:   process.argv.slice(2)
来源：http://sl.shxzukj.cn

TS:   process.argv.slice(2)
来源：http://rs.lnxyls.cn

Java: args 数组（main 方法参数）
来源：http://ik.yuntaijiaju.cn

Go:   os.Args[1:]
来源：http://zo.9csxet.cn

Ruby: ARGV
来源：http://ep.9csxet.cn

C#:   args 数组（Main 方法参数）
来源：http://gl.panjiajie.cn

[M02] 读取环境变量
来源：http://jw.yuntaijiaju.cn

Py:   os.environ.get("HOME")
来源：http://yl.yuntaijiaju.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://qo.huanxung.cn

JS:   process.env.HOME
来源：http://zu.bjjhwx.cn

TS:   process.env.HOME
来源：http://rc.hahajie.cn

Java: System.getenv("HOME")
来源：http://pa.shtwfgs.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ah.asd995.cn

Ruby: ENV["HOME"]
来源：http://hm.shxzskj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://pz.colortex.cn

[M03] 执行外部命令
来源：http://uv.haigaiapp.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://nm.gzmigu.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://pp.9csxet.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://cd.muxihuayi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ru.shxzskj.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://oa.szsharing.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ln.wgjwhj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://rr.huixinmuqiang.cn

C#:   Process.Start("ls", "-l");
来源：http://vd.huanxung.cn

[M04] 获取当前工作目录
来源：http://ab.huixinmuqiang.cn

Py:   os.getcwd()
来源：http://rg.huixiangedu.cn

PHP:  getcwd();
来源：http://xw.hahajie.cn

JS:   process.cwd()
来源：http://hy.shxzukj.cn

TS:   process.cwd()
来源：http://aq.nicolike.cn

Java: Path.of("").toAbsolutePath()
来源：http://qg.shxzskj.cn

Go:   os.Getwd()
来源：http://bd.shtwfgs.cn

Ruby: Dir.pwd
来源：http://cr.huixinmuqiang.cn

C#:   Directory.GetCurrentDirectory()
来源：http://sy.hahajie.cn

[M05] 设置退出码
来源：http://ix.haigaiapp.cn

Py:   sys.exit(1)
来源：http://xj.szsharing.cn

PHP:  exit(1);
来源：http://at.521024.cn

JS:   process.exit(1)
来源：http://ni.panjiajie.cn

TS:   process.exit(1)
来源：http://fx.bjjhwx.cn

Java: System.exit(1)
来源：http://af.szxytkj.cn

Go:   os.Exit(1)
来源：http://we.nicolike.cn

Ruby: exit 1
来源：http://em.szsharing.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://pq.jctech888.com.cn

[M06] 向标准错误输出
来源：http://ib.9csxet.cn

Py:   print("err", file=sys.stderr)
来源：http://wj.yuexingan06.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://sv.jianghongdianzi.cn

JS:   console.error("err")
来源：http://ms.yuntaijiaju.cn

TS:   console.error("err")
来源：http://gs.huanxung.cn

Java: System.err.println("err")
来源：http://dq.haigaiapp.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.newstarts.cn

Ruby: warn "err"
来源：http://cw.huixiangedu.cn

C#:   Console.Error.WriteLine("err")
来源：http://ql.yuntaijiaju.cn

[M07] 判断是否为主入口
来源：http://wo.nszjky.cn

Py:   if __name__ == "__main__":
来源：http://ql.shtwfgs.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ky.yuntaijiaju.cn

JS:   require.main === module
来源：http://qb.huanxung.cn

TS:   require.main === module
来源：http://si.newstarts.cn

Java: public static void main(String[] args)
来源：http://sw.panjiajie.cn

Go:   func main()
来源：http://ke.hahajie.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://oc.bookmarksfly.cn

C#:   static void Main(string[] args)
来源：http://in.jianghongdianzi.cn

[M08] 获取系统与运行时信息
来源：http://pw.hahajie.cn

Py:   platform.system();  platform.python_version()
来源：http://qp.521024.cn

PHP:  PHP_OS;  phpversion();
来源：http://ad.shxzukj.cn

JS:   process.platform;  process.version
来源：http://st.jctech888.com.cn

TS:   process.platform;  process.version
来源：http://pt.nszjky.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://kc.jctech888.com.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://bn.yuexingan06.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://vd.jctech888.com.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://gi.shxzukj.cn

================================================================================
来源：http://fv.yuexingan06.cn

N. 数据结构与算法
来源：http://oo.hnjuh.cn

================================================================================
来源：http://mw.wgjwhj.cn

[N01] 二分查找（有序数组）
来源：http://pr.jctech888.com.cn

Py:   bisect.bisect_left(arr, x)
来源：http://cz.521024.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://dj.muxihuayi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ry.panjiajie.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://uz.chemitech.net.cn

Java: Arrays.binarySearch(arr, x)
来源：http://or.lnxyls.cn

Go:   sort.SearchInts(arr, x)
来源：http://ds.9csxet.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://yc.asd995.cn

C#:   Array.BinarySearch(arr, x)
来源：http://as.gzmigu.cn

[N02] 排序（工程实践用内置实现）
来源：http://im.haigaiapp.cn

Py:   sorted(arr);  arr.sort()
来源：http://wz.shxzskj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://xm.shxzukj.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://mt.jctech888.com.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://wi.521024.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://qt.jctech888.com.cn

Go:   slices.Sort(arr)
来源：http://qt.yuexingan06.cn

Ruby: arr.sort
来源：http://bz.521024.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ly.szsharing.cn

[N03] 快速排序（分治示例）
来源：http://kk.jctech888.com.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://qi.bookmarksfly.cn

PHP:  // 递归实现，或用 usort
来源：http://bu.yuntaijiaju.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gg.9csxet.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://br.szsharing.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ke.shxzukj.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wm.yuexingan06.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://nw.bjjhwx.cn

C#:   // 手写递归，或 Array.Sort
来源：http://dz.gzmigu.cn

[N04] 斐波那契数列
来源：http://es.nicolike.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://aj.jctech888.com.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://cb.bookmarksfly.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mp.huanxung.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zc.yuexingan06.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://jx.nicolike.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://sp.shxzskj.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://qo.shtwfgs.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://yo.newstarts.cn

[N05] 最大公约数
来源：http://tj.bookmarksfly.cn

Py:   math.gcd(a, b)
来源：http://lq.szsharing.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://sp.lnxyls.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kc.wgjwhj.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zp.haigaiapp.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://bf.wgjwhj.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://pi.huixinmuqiang.cn

Ruby: a.gcd(b)
来源：http://uv.nszjky.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ol.szxytkj.cn

[N06] 判断回文字符串
来源：http://aj.bjjhwx.cn

Py:   s == s[::-1]
来源：http://yu.shtwfgs.cn

PHP:  $s === strrev($s);
来源：http://uw.wgjwhj.cn

JS:   s === [...s].reverse().join("")
来源：http://xg.szsharing.cn

TS:   s === [...s].reverse().join("")
来源：http://hz.huixinmuqiang.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ib.shxzukj.cn

Go:   // 双指针从两端比较
来源：http://jl.huixinmuqiang.cn

Ruby: s == s.reverse
来源：http://jw.yuntaijiaju.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ey.bookmarksfly.cn

[N07] 两数之和（返回下标）
来源：http://vc.nszjky.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hm.jctech888.com.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://xk.hnjuh.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://pw.jianghongdianzi.cn

TS:   // 手写 Map<string, number>
来源：http://fo.shxzskj.cn

Java: // 手写 HashMap
来源：http://xs.hahajie.cn

Go:   // 手写 map[int]int
来源：http://zn.huanxung.cn

Ruby: // 手写 Hash
来源：http://bk.jianghongdianzi.cn

C#:   // 手写 Dictionary<int, int>
来源：http://gm.nszjky.cn

[N08] 生成全排列
来源：http://zm.lnxyls.cn

Py:   itertools.permutations(arr)
来源：http://ic.wgjwhj.cn

PHP:  // 手写递归交换
来源：http://mi.gzmigu.cn

JS:   // 手写回溯递归
来源：http://mi.asd995.cn

TS:   // 手写回溯递归
来源：http://cn.panjiajie.cn

Java: // 手写回溯递归
来源：http://mk.shtwfgs.cn

Go:   // 手写回溯递归
来源：http://xr.jctech888.com.cn

Ruby: arr.permutation.to_a
来源：http://jr.bookmarksfly.cn

C#:   // 手写回溯递归
来源：http://vw.huixinmuqiang.cn

[N09] 栈与队列
来源：http://sd.nicolike.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://vb.bjjhwx.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://pw.bjjhwx.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ad.jianghongdianzi.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://an.huanxung.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://fu.wgjwhj.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wi.jianghongdianzi.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://iv.szsharing.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://fq.shxzskj.cn

[N10] 链表节点定义
来源：http://vx.haigaiapp.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qq.huixiangedu.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://vz.nicolike.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://zv.shtwfgs.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://yt.wgjwhj.cn

Java: class Node { int v; Node next; }
来源：http://jf.hnjuh.cn

Go:   type Node struct { V int; Next *Node }
来源：http://fz.nicolike.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://fn.9csxet.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://xj.shtwfgs.cn

[N11] 二叉树中序遍历
来源：http://te.szxytkj.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ex.shtwfgs.cn

PHP:  // 手写递归函数
来源：http://jj.huixinmuqiang.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wd.hahajie.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hq.asd995.cn

Java: // 手写递归
来源：http://dp.nszjky.cn

Go:   // 手写递归
来源：http://xx.bjjhwx.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ks.asd995.cn

C#:   // 手写递归
来源：http://pq.panjiajie.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://dl.haigaiapp.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ei.shxzukj.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://yb.muxihuayi.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rj.gzmigu.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vo.jctech888.com.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://bq.muxihuayi.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://yr.huixinmuqiang.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://sr.lnxyls.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://rk.hnjuh.cn

================================================================================
来源：http://vh.newstarts.cn

O. 并发与异步
来源：http://cd.yuntaijiaju.cn

================================================================================
来源：http://dt.nicolike.cn

[O01] 启动一个线程
来源：http://mk.bjjhwx.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://uj.huixiangedu.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://dh.colortex.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://fg.haigaiapp.cn

TS:   // 同 JS
来源：http://fc.chemitech.net.cn

Java: new Thread(() -> f()).start()
来源：http://vs.asd995.cn

Go:   go f()
来源：http://ml.szsharing.cn

Ruby: Thread.new { f }
来源：http://ie.szxytkj.cn

C#:   Task.Run(() => F());
来源：http://qo.521024.cn

[O02] 使用线程池
来源：http://he.jianghongdianzi.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://sq.szxytkj.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ha.newstarts.cn

JS:   // worker_threads 线程池
来源：http://yj.shtwfgs.cn

TS:   // worker_threads 线程池
来源：http://kg.huanxung.cn

Java: Executors.newFixedThreadPool(4)
来源：http://wy.panjiajie.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://sn.hnjuh.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://vq.jctech888.com.cn


<!-- 参考信息 -->