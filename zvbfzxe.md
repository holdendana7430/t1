代发 wailian999

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://qy.haigaiapp.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://fe.hnjuh.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ig.huixinmuqiang.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ch.szsharing.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qk.huixiangedu.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://zj.wgjwhj.cn

[K08] 二进制序列化（非 JSON）
来源：http://ys.chemitech.net.cn

Py:   pickle.dumps(obj)
来源：http://bi.hnjuh.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ng.szxytkj.cn

JS:   v8.serialize(obj)        // Node
来源：http://iw.huanxung.cn

TS:   v8.serialize(obj)        // Node
来源：http://rh.huixinmuqiang.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://uv.yuexingan06.cn

Go:   encoding/gob
来源：http://rt.colortex.cn

Ruby: Marshal.dump(obj)
来源：http://nw.yuexingan06.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://jn.gzmigu.cn

================================================================================
来源：http://or.panjiajie.cn

L. 网络请求
来源：http://em.huixinmuqiang.cn

================================================================================
来源：http://cn.hahajie.cn

[L01] 发送 GET 请求
来源：http://bi.hnjuh.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ze.shxzskj.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://tw.9csxet.cn

JS:   await fetch(url)
来源：http://nz.szsharing.cn

TS:   await fetch(url)
来源：http://xf.asd995.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://fl.shxzukj.cn

Go:   resp, err := http.Get(url)
来源：http://ng.newstarts.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ju.521024.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://rb.hnjuh.cn

[L02] 发送 POST JSON
来源：http://id.bookmarksfly.cn

Py:   requests.post(url, json={"a": 1})
来源：http://kj.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wd.lnxyls.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vx.jianghongdianzi.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://el.yuntaijiaju.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hy.asd995.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://sa.9csxet.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://bk.jctech888.com.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://cr.wgjwhj.cn

[L03] 设置自定义请求头
来源：http://oa.huixiangedu.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://sn.hnjuh.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://pe.muxihuayi.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ls.hnjuh.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wx.chemitech.net.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://bn.521024.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://lg.nszjky.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://nf.9csxet.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://nd.hahajie.cn

[L04] 设置超时
来源：http://cn.lnxyls.cn

Py:   requests.get(url, timeout=5)
来源：http://tj.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://nz.shxzskj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ck.chemitech.net.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lu.jctech888.com.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ln.colortex.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://eg.jctech888.com.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://zh.huixiangedu.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://to.jianghongdianzi.cn

[L05] 上传文件（multipart）
来源：http://vg.jianghongdianzi.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://vp.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://fv.yuexingan06.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://dp.newstarts.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://id.szxytkj.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://jn.huixinmuqiang.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://pt.huixinmuqiang.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://zz.haigaiapp.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://aw.huanxung.cn

[L06] 解析响应为 JSON
来源：http://rt.lnxyls.cn

Py:   resp.json()
来源：http://hl.wgjwhj.cn

PHP:  json_decode($body, true);
来源：http://bb.muxihuayi.cn

JS:   await resp.json()
来源：http://vj.shxzskj.cn

TS:   await resp.json()
来源：http://of.haigaiapp.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://nt.shxzukj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://rf.lnxyls.cn

Ruby: JSON.parse(resp.body)
来源：http://nj.gzmigu.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://me.nszjky.cn

[L07] 处理 HTTP 状态码
来源：http://cm.9csxet.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wa.shtwfgs.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ri.shxzukj.cn

JS:   resp.ok;  resp.status
来源：http://ln.asd995.cn

TS:   resp.ok;  resp.status
来源：http://vw.lnxyls.cn

Java: resp.statusCode()
来源：http://go.szxytkj.cn

Go:   resp.StatusCode
来源：http://jq.9csxet.cn

Ruby: resp.code.to_i
来源：http://jq.asd995.cn

C#:   (int)resp.StatusCode
来源：http://dj.panjiajie.cn

[L08] 并发请求多个地址
来源：http://lp.nszjky.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://op.huixiangedu.cn

PHP:  curl_multi_init() 系列
来源：http://ns.hnjuh.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jp.szxytkj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xy.szxytkj.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mc.nicolike.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ov.muxihuayi.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://gs.huixiangedu.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://az.nicolike.cn

================================================================================
来源：http://ab.9csxet.cn

M. 命令行 / 进程 / 环境
来源：http://jo.colortex.cn

================================================================================
来源：http://bq.9csxet.cn

[M01] 读取命令行参数
来源：http://lj.521024.cn

Py:   sys.argv[1:]
来源：http://ko.colortex.cn

PHP:  $argv;  $argc;
来源：http://oc.bookmarksfly.cn

JS:   process.argv.slice(2)
来源：http://lr.bjjhwx.cn

TS:   process.argv.slice(2)
来源：http://tk.nszjky.cn

Java: args 数组（main 方法参数）
来源：http://fn.szsharing.cn

Go:   os.Args[1:]
来源：http://wn.shtwfgs.cn

Ruby: ARGV
来源：http://un.asd995.cn

C#:   args 数组（Main 方法参数）
来源：http://pt.panjiajie.cn

[M02] 读取环境变量
来源：http://cz.shxzukj.cn

Py:   os.environ.get("HOME")
来源：http://gu.asd995.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://oy.bjjhwx.cn

JS:   process.env.HOME
来源：http://ck.asd995.cn

TS:   process.env.HOME
来源：http://dc.huanxung.cn

Java: System.getenv("HOME")
来源：http://sa.yuexingan06.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://eo.shtwfgs.cn

Ruby: ENV["HOME"]
来源：http://ej.bookmarksfly.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://sf.nszjky.cn

[M03] 执行外部命令
来源：http://zp.jianghongdianzi.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://iy.yuexingan06.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://vj.shxzukj.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ou.jianghongdianzi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://nr.yuexingan06.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ez.muxihuayi.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://hb.jianghongdianzi.cn

Ruby: system("ls -l");  `ls -l`
来源：http://kd.szsharing.cn

C#:   Process.Start("ls", "-l");
来源：http://qh.hnjuh.cn

[M04] 获取当前工作目录
来源：http://xm.panjiajie.cn

Py:   os.getcwd()
来源：http://yl.9csxet.cn

PHP:  getcwd();
来源：http://ne.szsharing.cn

JS:   process.cwd()
来源：http://cq.huixinmuqiang.cn

TS:   process.cwd()
来源：http://vd.jianghongdianzi.cn

Java: Path.of("").toAbsolutePath()
来源：http://id.szsharing.cn

Go:   os.Getwd()
来源：http://mj.jctech888.com.cn

Ruby: Dir.pwd
来源：http://up.huixiangedu.cn

C#:   Directory.GetCurrentDirectory()
来源：http://au.panjiajie.cn

[M05] 设置退出码
来源：http://di.yuntaijiaju.cn

Py:   sys.exit(1)
来源：http://dr.huixinmuqiang.cn

PHP:  exit(1);
来源：http://uh.gzmigu.cn

JS:   process.exit(1)
来源：http://mp.nicolike.cn

TS:   process.exit(1)
来源：http://zq.huanxung.cn

Java: System.exit(1)
来源：http://xt.yuexingan06.cn

Go:   os.Exit(1)
来源：http://sf.9csxet.cn

Ruby: exit 1
来源：http://sv.shxzskj.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://lf.panjiajie.cn

[M06] 向标准错误输出
来源：http://bg.hnjuh.cn

Py:   print("err", file=sys.stderr)
来源：http://ye.muxihuayi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://mi.521024.cn

JS:   console.error("err")
来源：http://ta.jctech888.com.cn

TS:   console.error("err")
来源：http://vp.shxzskj.cn

Java: System.err.println("err")
来源：http://cu.szxytkj.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://xt.521024.cn

Ruby: warn "err"
来源：http://zd.huixiangedu.cn

C#:   Console.Error.WriteLine("err")
来源：http://oj.yuntaijiaju.cn

[M07] 判断是否为主入口
来源：http://bl.chemitech.net.cn

Py:   if __name__ == "__main__":
来源：http://il.lnxyls.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://fe.huixiangedu.cn

JS:   require.main === module
来源：http://lu.yuexingan06.cn

TS:   require.main === module
来源：http://cf.hnjuh.cn

Java: public static void main(String[] args)
来源：http://oi.nszjky.cn

Go:   func main()
来源：http://nj.hahajie.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://zf.jianghongdianzi.cn

C#:   static void Main(string[] args)
来源：http://st.newstarts.cn

[M08] 获取系统与运行时信息
来源：http://qt.jctech888.com.cn

Py:   platform.system();  platform.python_version()
来源：http://jf.gzmigu.cn

PHP:  PHP_OS;  phpversion();
来源：http://ad.nszjky.cn

JS:   process.platform;  process.version
来源：http://cu.haigaiapp.cn

TS:   process.platform;  process.version
来源：http://qg.lnxyls.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xw.yuntaijiaju.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://lm.shxzukj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://dy.huanxung.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://cn.shxzukj.cn

================================================================================
来源：http://mk.szsharing.cn

N. 数据结构与算法
来源：http://wg.hahajie.cn

================================================================================
来源：http://mc.nicolike.cn

[N01] 二分查找（有序数组）
来源：http://fq.chemitech.net.cn

Py:   bisect.bisect_left(arr, x)
来源：http://qi.nszjky.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://gf.szxytkj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vw.colortex.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vd.shxzukj.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ah.colortex.cn

Go:   sort.SearchInts(arr, x)
来源：http://kz.wgjwhj.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://uz.shtwfgs.cn

C#:   Array.BinarySearch(arr, x)
来源：http://yp.9csxet.cn

[N02] 排序（工程实践用内置实现）
来源：http://ov.lnxyls.cn

Py:   sorted(arr);  arr.sort()
来源：http://zz.hnjuh.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://tm.panjiajie.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ba.bookmarksfly.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://si.lnxyls.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://gx.jianghongdianzi.cn

Go:   slices.Sort(arr)
来源：http://fc.yuntaijiaju.cn

Ruby: arr.sort
来源：http://za.huixinmuqiang.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://qa.asd995.cn

[N03] 快速排序（分治示例）
来源：http://xg.yuntaijiaju.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://xh.nicolike.cn

PHP:  // 递归实现，或用 usort
来源：http://qz.szxytkj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yx.nszjky.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://su.szxytkj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ld.shtwfgs.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://on.9csxet.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hl.muxihuayi.cn

C#:   // 手写递归，或 Array.Sort
来源：http://zc.yuexingan06.cn

[N04] 斐波那契数列
来源：http://rn.yuntaijiaju.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://uc.shtwfgs.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://dg.bookmarksfly.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yu.chemitech.net.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gk.hahajie.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hp.shtwfgs.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://fm.muxihuayi.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ta.shxzskj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://tk.szsharing.cn

[N05] 最大公约数
来源：http://el.lnxyls.cn

Py:   math.gcd(a, b)
来源：http://wu.szxytkj.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://bs.shxzukj.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rr.shtwfgs.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fc.nicolike.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://fv.nicolike.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://az.asd995.cn

Ruby: a.gcd(b)
来源：http://qx.colortex.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://cp.jctech888.com.cn

[N06] 判断回文字符串
来源：http://nw.asd995.cn

Py:   s == s[::-1]
来源：http://mb.hahajie.cn

PHP:  $s === strrev($s);
来源：http://gl.shtwfgs.cn

JS:   s === [...s].reverse().join("")
来源：http://pk.hnjuh.cn

TS:   s === [...s].reverse().join("")
来源：http://pt.wgjwhj.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ts.huanxung.cn

Go:   // 双指针从两端比较
来源：http://xk.asd995.cn

Ruby: s == s.reverse
来源：http://rp.yuntaijiaju.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://pr.asd995.cn

[N07] 两数之和（返回下标）
来源：http://ub.lnxyls.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://rl.shxzskj.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://kk.asd995.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://jb.hnjuh.cn

TS:   // 手写 Map<string, number>
来源：http://mu.jctech888.com.cn

Java: // 手写 HashMap
来源：http://he.asd995.cn

Go:   // 手写 map[int]int
来源：http://rb.shxzukj.cn

Ruby: // 手写 Hash
来源：http://qg.huixinmuqiang.cn

C#:   // 手写 Dictionary<int, int>
来源：http://aj.jianghongdianzi.cn

[N08] 生成全排列
来源：http://zv.bookmarksfly.cn

Py:   itertools.permutations(arr)
来源：http://al.bjjhwx.cn

PHP:  // 手写递归交换
来源：http://za.nszjky.cn

JS:   // 手写回溯递归
来源：http://rl.521024.cn

TS:   // 手写回溯递归
来源：http://bf.nicolike.cn

Java: // 手写回溯递归
来源：http://mr.newstarts.cn

Go:   // 手写回溯递归
来源：http://yj.yuntaijiaju.cn

Ruby: arr.permutation.to_a
来源：http://pu.asd995.cn

C#:   // 手写回溯递归
来源：http://rx.hahajie.cn

[N09] 栈与队列
来源：http://cb.nszjky.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://fo.asd995.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://zc.hnjuh.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ei.9csxet.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://dn.shtwfgs.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://bi.huixinmuqiang.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ne.lnxyls.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ds.hnjuh.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://fj.hahajie.cn

[N10] 链表节点定义
来源：http://tk.huixinmuqiang.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://sy.hnjuh.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ly.gzmigu.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://tx.chemitech.net.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://lb.shxzskj.cn

Java: class Node { int v; Node next; }
来源：http://gn.bjjhwx.cn

Go:   type Node struct { V int; Next *Node }
来源：http://iy.lnxyls.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://da.shxzukj.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ub.chemitech.net.cn

[N11] 二叉树中序遍历
来源：http://tv.huixinmuqiang.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://kw.9csxet.cn

PHP:  // 手写递归函数
来源：http://zh.nicolike.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qm.jctech888.com.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://az.yuntaijiaju.cn

Java: // 手写递归
来源：http://zo.nicolike.cn

Go:   // 手写递归
来源：http://oa.chemitech.net.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://kp.yuntaijiaju.cn

C#:   // 手写递归
来源：http://oi.hahajie.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://lg.yuntaijiaju.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://kl.bjjhwx.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://lg.bjjhwx.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://px.huanxung.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yg.nicolike.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ut.huixinmuqiang.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mo.shtwfgs.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://kx.nicolike.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ex.jianghongdianzi.cn

================================================================================
来源：http://hm.huanxung.cn

O. 并发与异步
来源：http://wb.bookmarksfly.cn

================================================================================
来源：http://ah.jctech888.com.cn

[O01] 启动一个线程
来源：http://fc.asd995.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wv.521024.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://xi.yuntaijiaju.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://xl.nicolike.cn

TS:   // 同 JS
来源：http://rc.shxzskj.cn

Java: new Thread(() -> f()).start()
来源：http://td.nszjky.cn

Go:   go f()
来源：http://yx.panjiajie.cn

Ruby: Thread.new { f }
来源：http://wd.nicolike.cn

C#:   Task.Run(() => F());
来源：http://uf.wgjwhj.cn

[O02] 使用线程池
来源：http://xy.lnxyls.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://cw.nicolike.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://py.asd995.cn

JS:   // worker_threads 线程池
来源：http://tb.bjjhwx.cn

TS:   // worker_threads 线程池
来源：http://jj.szsharing.cn

Java: Executors.newFixedThreadPool(4)
来源：http://qb.huixinmuqiang.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://xc.521024.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://os.bookmarksfly.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://cl.521024.cn

[O03] 加锁保护共享数据
来源：http://yq.shxzskj.cn

Py:   with lock: shared += 1
来源：http://vq.haigaiapp.cn

PHP:  // 用 flock() 做文件锁
来源：http://cc.huanxung.cn


<!-- 参考信息 -->