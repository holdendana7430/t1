代发 wailian999

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://vt.muxihuayi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://pn.shtwfgs.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://rq.shxzskj.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://zx.shxzskj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://xm.nszjky.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://oa.szsharing.cn

[K08] 二进制序列化（非 JSON）
来源：http://lz.asd995.cn

Py:   pickle.dumps(obj)
来源：http://dz.nszjky.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ba.nszjky.cn

JS:   v8.serialize(obj)        // Node
来源：http://iq.bookmarksfly.cn

TS:   v8.serialize(obj)        // Node
来源：http://uy.jianghongdianzi.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://yy.szsharing.cn

Go:   encoding/gob
来源：http://mz.szsharing.cn

Ruby: Marshal.dump(obj)
来源：http://tm.bookmarksfly.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qk.huanxung.cn

================================================================================
来源：http://xd.nszjky.cn

L. 网络请求
来源：http://na.newstarts.cn

================================================================================
来源：http://nr.huixiangedu.cn

[L01] 发送 GET 请求
来源：http://ai.nszjky.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ps.bjjhwx.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://qm.jctech888.com.cn

JS:   await fetch(url)
来源：http://rv.huixiangedu.cn

TS:   await fetch(url)
来源：http://kg.jianghongdianzi.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://pf.chemitech.net.cn

Go:   resp, err := http.Get(url)
来源：http://cn.hnjuh.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://sm.shtwfgs.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://vl.hahajie.cn

[L02] 发送 POST JSON
来源：http://jb.bjjhwx.cn

Py:   requests.post(url, json={"a": 1})
来源：http://fb.panjiajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://vd.lnxyls.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sw.shxzskj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gw.huixiangedu.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://is.shtwfgs.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://zh.hnjuh.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://dw.huixiangedu.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ja.shxzskj.cn

[L03] 设置自定义请求头
来源：http://ka.huanxung.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://td.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://zb.newstarts.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qx.huixiangedu.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gp.chemitech.net.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://oi.shtwfgs.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://gh.9csxet.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://lw.shtwfgs.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ra.hnjuh.cn

[L04] 设置超时
来源：http://uh.newstarts.cn

Py:   requests.get(url, timeout=5)
来源：http://vg.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ax.hahajie.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jq.lnxyls.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://at.huixiangedu.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://bt.bookmarksfly.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://iv.yuexingan06.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://yq.huixiangedu.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://tb.colortex.cn

[L05] 上传文件（multipart）
来源：http://ri.shxzskj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zg.asd995.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://dg.lnxyls.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://yu.521024.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://qu.chemitech.net.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://zb.nszjky.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mn.521024.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://it.muxihuayi.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://aq.newstarts.cn

[L06] 解析响应为 JSON
来源：http://zd.shxzukj.cn

Py:   resp.json()
来源：http://kp.nicolike.cn

PHP:  json_decode($body, true);
来源：http://ug.nicolike.cn

JS:   await resp.json()
来源：http://ua.yuexingan06.cn

TS:   await resp.json()
来源：http://og.shxzskj.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://vg.hnjuh.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://nf.szsharing.cn

Ruby: JSON.parse(resp.body)
来源：http://yd.bookmarksfly.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ep.huanxung.cn

[L07] 处理 HTTP 状态码
来源：http://mo.hnjuh.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://yz.gzmigu.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://zr.newstarts.cn

JS:   resp.ok;  resp.status
来源：http://vz.huixiangedu.cn

TS:   resp.ok;  resp.status
来源：http://tn.gzmigu.cn

Java: resp.statusCode()
来源：http://vi.jianghongdianzi.cn

Go:   resp.StatusCode
来源：http://db.lnxyls.cn

Ruby: resp.code.to_i
来源：http://th.yuntaijiaju.cn

C#:   (int)resp.StatusCode
来源：http://ll.jianghongdianzi.cn

[L08] 并发请求多个地址
来源：http://uz.asd995.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://sb.shtwfgs.cn

PHP:  curl_multi_init() 系列
来源：http://ch.hnjuh.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ik.521024.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rt.asd995.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://bn.newstarts.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://rx.huixinmuqiang.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://qw.wgjwhj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wz.jctech888.com.cn

================================================================================
来源：http://tg.jianghongdianzi.cn

M. 命令行 / 进程 / 环境
来源：http://zd.chemitech.net.cn

================================================================================
来源：http://zn.asd995.cn

[M01] 读取命令行参数
来源：http://kl.asd995.cn

Py:   sys.argv[1:]
来源：http://in.gzmigu.cn

PHP:  $argv;  $argc;
来源：http://pz.bjjhwx.cn

JS:   process.argv.slice(2)
来源：http://dy.521024.cn

TS:   process.argv.slice(2)
来源：http://sg.chemitech.net.cn

Java: args 数组（main 方法参数）
来源：http://ev.yuexingan06.cn

Go:   os.Args[1:]
来源：http://qo.szxytkj.cn

Ruby: ARGV
来源：http://fu.panjiajie.cn

C#:   args 数组（Main 方法参数）
来源：http://qb.gzmigu.cn

[M02] 读取环境变量
来源：http://ba.haigaiapp.cn

Py:   os.environ.get("HOME")
来源：http://cu.shxzskj.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://eu.huixiangedu.cn

JS:   process.env.HOME
来源：http://ui.szxytkj.cn

TS:   process.env.HOME
来源：http://wj.panjiajie.cn

Java: System.getenv("HOME")
来源：http://rd.muxihuayi.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://im.huanxung.cn

Ruby: ENV["HOME"]
来源：http://hx.yuntaijiaju.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://yj.nicolike.cn

[M03] 执行外部命令
来源：http://qc.yuexingan06.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wj.szxytkj.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ut.bookmarksfly.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://fn.newstarts.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ji.huixinmuqiang.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ao.muxihuayi.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ma.muxihuayi.cn

Ruby: system("ls -l");  `ls -l`
来源：http://sj.huixinmuqiang.cn

C#:   Process.Start("ls", "-l");
来源：http://cq.bookmarksfly.cn

[M04] 获取当前工作目录
来源：http://qh.huixinmuqiang.cn

Py:   os.getcwd()
来源：http://xh.asd995.cn

PHP:  getcwd();
来源：http://ay.wgjwhj.cn

JS:   process.cwd()
来源：http://im.huixiangedu.cn

TS:   process.cwd()
来源：http://gj.bjjhwx.cn

Java: Path.of("").toAbsolutePath()
来源：http://om.9csxet.cn

Go:   os.Getwd()
来源：http://il.9csxet.cn

Ruby: Dir.pwd
来源：http://pt.haigaiapp.cn

C#:   Directory.GetCurrentDirectory()
来源：http://mk.chemitech.net.cn

[M05] 设置退出码
来源：http://ob.muxihuayi.cn

Py:   sys.exit(1)
来源：http://nb.hahajie.cn

PHP:  exit(1);
来源：http://ps.bjjhwx.cn

JS:   process.exit(1)
来源：http://zf.bjjhwx.cn

TS:   process.exit(1)
来源：http://dv.newstarts.cn

Java: System.exit(1)
来源：http://ej.newstarts.cn

Go:   os.Exit(1)
来源：http://dn.yuntaijiaju.cn

Ruby: exit 1
来源：http://ga.szxytkj.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://zq.hahajie.cn

[M06] 向标准错误输出
来源：http://wo.colortex.cn

Py:   print("err", file=sys.stderr)
来源：http://ij.newstarts.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://bo.asd995.cn

JS:   console.error("err")
来源：http://yj.nszjky.cn

TS:   console.error("err")
来源：http://gi.huanxung.cn

Java: System.err.println("err")
来源：http://ky.521024.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://bv.bjjhwx.cn

Ruby: warn "err"
来源：http://ia.huixinmuqiang.cn

C#:   Console.Error.WriteLine("err")
来源：http://fi.asd995.cn

[M07] 判断是否为主入口
来源：http://jv.bjjhwx.cn

Py:   if __name__ == "__main__":
来源：http://zr.muxihuayi.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://da.szxytkj.cn

JS:   require.main === module
来源：http://ey.yuexingan06.cn

TS:   require.main === module
来源：http://re.hnjuh.cn

Java: public static void main(String[] args)
来源：http://di.szsharing.cn

Go:   func main()
来源：http://pv.colortex.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://xv.9csxet.cn

C#:   static void Main(string[] args)
来源：http://ix.shxzukj.cn

[M08] 获取系统与运行时信息
来源：http://ts.shxzukj.cn

Py:   platform.system();  platform.python_version()
来源：http://ah.jctech888.com.cn

PHP:  PHP_OS;  phpversion();
来源：http://wr.muxihuayi.cn

JS:   process.platform;  process.version
来源：http://we.bookmarksfly.cn

TS:   process.platform;  process.version
来源：http://lj.lnxyls.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://va.shxzskj.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://rb.bjjhwx.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://vb.chemitech.net.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://oy.haigaiapp.cn

================================================================================
来源：http://tu.hnjuh.cn

N. 数据结构与算法
来源：http://iu.huanxung.cn

================================================================================
来源：http://lm.lnxyls.cn

[N01] 二分查找（有序数组）
来源：http://xh.colortex.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ti.shtwfgs.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://qk.lnxyls.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ig.panjiajie.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pw.wgjwhj.cn

Java: Arrays.binarySearch(arr, x)
来源：http://xt.gzmigu.cn

Go:   sort.SearchInts(arr, x)
来源：http://dj.shtwfgs.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://cr.yuexingan06.cn

C#:   Array.BinarySearch(arr, x)
来源：http://qt.nicolike.cn

[N02] 排序（工程实践用内置实现）
来源：http://ii.9csxet.cn

Py:   sorted(arr);  arr.sort()
来源：http://xs.huanxung.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://vo.nicolike.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://rw.hahajie.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://co.shtwfgs.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://rb.nicolike.cn

Go:   slices.Sort(arr)
来源：http://ql.szxytkj.cn

Ruby: arr.sort
来源：http://ij.shtwfgs.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://da.wgjwhj.cn

[N03] 快速排序（分治示例）
来源：http://lo.9csxet.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://sx.huixinmuqiang.cn

PHP:  // 递归实现，或用 usort
来源：http://ln.hnjuh.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yb.shxzskj.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yk.9csxet.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ra.shtwfgs.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://fr.asd995.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://nf.521024.cn

C#:   // 手写递归，或 Array.Sort
来源：http://pz.shxzskj.cn

[N04] 斐波那契数列
来源：http://jw.shxzskj.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://tx.bookmarksfly.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://nt.bjjhwx.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sg.nszjky.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lw.chemitech.net.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://bl.jctech888.com.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://no.szxytkj.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ns.panjiajie.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://at.szsharing.cn

[N05] 最大公约数
来源：http://xb.chemitech.net.cn

Py:   math.gcd(a, b)
来源：http://da.huixiangedu.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://au.gzmigu.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://aq.muxihuayi.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bg.asd995.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://vl.wgjwhj.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ws.nszjky.cn

Ruby: a.gcd(b)
来源：http://me.colortex.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://rr.shtwfgs.cn

[N06] 判断回文字符串
来源：http://fl.huixinmuqiang.cn

Py:   s == s[::-1]
来源：http://cu.hnjuh.cn

PHP:  $s === strrev($s);
来源：http://ei.nszjky.cn

JS:   s === [...s].reverse().join("")
来源：http://sf.colortex.cn

TS:   s === [...s].reverse().join("")
来源：http://fo.yuexingan06.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xl.asd995.cn

Go:   // 双指针从两端比较
来源：http://en.asd995.cn

Ruby: s == s.reverse
来源：http://xi.colortex.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://hc.gzmigu.cn

[N07] 两数之和（返回下标）
来源：http://yp.bookmarksfly.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://cn.panjiajie.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jk.panjiajie.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://rd.colortex.cn

TS:   // 手写 Map<string, number>
来源：http://sl.gzmigu.cn

Java: // 手写 HashMap
来源：http://ha.huixiangedu.cn

Go:   // 手写 map[int]int
来源：http://df.hahajie.cn

Ruby: // 手写 Hash
来源：http://vm.panjiajie.cn

C#:   // 手写 Dictionary<int, int>
来源：http://li.huixiangedu.cn

[N08] 生成全排列
来源：http://je.gzmigu.cn

Py:   itertools.permutations(arr)
来源：http://ot.szsharing.cn

PHP:  // 手写递归交换
来源：http://oi.huixiangedu.cn

JS:   // 手写回溯递归
来源：http://oz.nszjky.cn

TS:   // 手写回溯递归
来源：http://fi.lnxyls.cn

Java: // 手写回溯递归
来源：http://wy.wgjwhj.cn

Go:   // 手写回溯递归
来源：http://en.521024.cn

Ruby: arr.permutation.to_a
来源：http://mf.panjiajie.cn

C#:   // 手写回溯递归
来源：http://np.yuexingan06.cn

[N09] 栈与队列
来源：http://de.bookmarksfly.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://gu.yuntaijiaju.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://nl.muxihuayi.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ng.jianghongdianzi.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://cz.wgjwhj.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mc.asd995.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://rr.panjiajie.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ul.wgjwhj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://cg.szsharing.cn

[N10] 链表节点定义
来源：http://nm.nicolike.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ph.haigaiapp.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ul.bookmarksfly.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://vf.shxzukj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://gk.521024.cn

Java: class Node { int v; Node next; }
来源：http://fd.jianghongdianzi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ia.szxytkj.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ja.hnjuh.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://zy.muxihuayi.cn

[N11] 二叉树中序遍历
来源：http://mt.bjjhwx.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://nc.szsharing.cn

PHP:  // 手写递归函数
来源：http://of.hnjuh.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://km.jctech888.com.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mf.panjiajie.cn

Java: // 手写递归
来源：http://hh.chemitech.net.cn

Go:   // 手写递归
来源：http://bm.lnxyls.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://gn.szxytkj.cn

C#:   // 手写递归
来源：http://ry.gzmigu.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://kq.shxzukj.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://bx.hahajie.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://gj.hnjuh.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://go.521024.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ip.asd995.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://lz.huanxung.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://qi.shtwfgs.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://cr.gzmigu.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://jk.nszjky.cn

================================================================================
来源：http://hs.bookmarksfly.cn

O. 并发与异步
来源：http://rp.yuexingan06.cn

================================================================================
来源：http://dp.hnjuh.cn

[O01] 启动一个线程
来源：http://vo.bjjhwx.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://qm.bookmarksfly.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://yu.bjjhwx.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://rr.wgjwhj.cn

TS:   // 同 JS
来源：http://cx.nicolike.cn

Java: new Thread(() -> f()).start()
来源：http://iw.shxzukj.cn

Go:   go f()
来源：http://yn.521024.cn

Ruby: Thread.new { f }
来源：http://vd.521024.cn

C#:   Task.Run(() => F());
来源：http://fn.newstarts.cn

[O02] 使用线程池
来源：http://kw.jctech888.com.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://qq.asd995.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ov.muxihuayi.cn

JS:   // worker_threads 线程池
来源：http://yo.colortex.cn

TS:   // worker_threads 线程池
来源：http://pu.huanxung.cn

Java: Executors.newFixedThreadPool(4)
来源：http://rz.hahajie.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ef.haigaiapp.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://pf.colortex.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://kx.jianghongdianzi.cn

[O03] 加锁保护共享数据
来源：http://mx.bookmarksfly.cn

Py:   with lock: shared += 1
来源：http://qo.haigaiapp.cn

PHP:  // 用 flock() 做文件锁
来源：http://qx.newstarts.cn


<!-- 参考信息 -->