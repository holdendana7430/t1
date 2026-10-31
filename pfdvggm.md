代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://tc.szxytkj.cn

[K07] 进制转换
来源：http://ek.szsharing.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ht.shtwfgs.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://bx.bookmarksfly.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://uu.bookmarksfly.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://rs.asd995.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://go.yuntaijiaju.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://fm.bjjhwx.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://sg.huanxung.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://rn.chemitech.net.cn

[K08] 二进制序列化（非 JSON）
来源：http://ea.nicolike.cn

Py:   pickle.dumps(obj)
来源：http://rq.shtwfgs.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://qz.shxzskj.cn

JS:   v8.serialize(obj)        // Node
来源：http://ci.panjiajie.cn

TS:   v8.serialize(obj)        // Node
来源：http://rk.jianghongdianzi.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ui.521024.cn

Go:   encoding/gob
来源：http://dr.yuntaijiaju.cn

Ruby: Marshal.dump(obj)
来源：http://zd.yuntaijiaju.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://gs.hahajie.cn

================================================================================
来源：http://so.huixinmuqiang.cn

L. 网络请求
来源：http://al.szsharing.cn

================================================================================
来源：http://vq.shtwfgs.cn

[L01] 发送 GET 请求
来源：http://yx.nszjky.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xd.nszjky.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://sm.hnjuh.cn

JS:   await fetch(url)
来源：http://xs.chemitech.net.cn

TS:   await fetch(url)
来源：http://st.bookmarksfly.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://rs.wgjwhj.cn

Go:   resp, err := http.Get(url)
来源：http://qq.9csxet.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://wb.jianghongdianzi.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://yx.newstarts.cn

[L02] 发送 POST JSON
来源：http://qy.nicolike.cn

Py:   requests.post(url, json={"a": 1})
来源：http://cl.szsharing.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ro.huixinmuqiang.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yp.muxihuayi.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bt.hnjuh.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://id.jctech888.com.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://kd.shtwfgs.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://qn.nszjky.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://cv.haigaiapp.cn

[L03] 设置自定义请求头
来源：http://cg.yuexingan06.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ai.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://oh.chemitech.net.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sz.shxzskj.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kq.huanxung.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ie.haigaiapp.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jj.wgjwhj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://yq.szsharing.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://js.shxzukj.cn

[L04] 设置超时
来源：http://pr.521024.cn

Py:   requests.get(url, timeout=5)
来源：http://xr.szxytkj.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://yi.yuexingan06.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://iz.colortex.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yk.newstarts.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://fc.jctech888.com.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://es.bjjhwx.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://cr.szsharing.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://vg.shxzskj.cn

[L05] 上传文件（multipart）
来源：http://gx.muxihuayi.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ch.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ek.asd995.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://tu.shtwfgs.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://qd.huixinmuqiang.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://qa.newstarts.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://lh.bookmarksfly.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://lp.asd995.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://qh.bjjhwx.cn

[L06] 解析响应为 JSON
来源：http://vx.bjjhwx.cn

Py:   resp.json()
来源：http://cg.yuntaijiaju.cn

PHP:  json_decode($body, true);
来源：http://zu.hnjuh.cn

JS:   await resp.json()
来源：http://es.colortex.cn

TS:   await resp.json()
来源：http://xm.hnjuh.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ya.bjjhwx.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://de.hahajie.cn

Ruby: JSON.parse(resp.body)
来源：http://sh.yuntaijiaju.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://sb.hahajie.cn

[L07] 处理 HTTP 状态码
来源：http://fw.panjiajie.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ep.yuntaijiaju.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hn.szsharing.cn

JS:   resp.ok;  resp.status
来源：http://tx.newstarts.cn

TS:   resp.ok;  resp.status
来源：http://kx.shxzukj.cn

Java: resp.statusCode()
来源：http://no.jctech888.com.cn

Go:   resp.StatusCode
来源：http://rs.yuexingan06.cn

Ruby: resp.code.to_i
来源：http://sw.yuexingan06.cn

C#:   (int)resp.StatusCode
来源：http://yn.huixiangedu.cn

[L08] 并发请求多个地址
来源：http://ry.panjiajie.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://eg.lnxyls.cn

PHP:  curl_multi_init() 系列
来源：http://ig.shtwfgs.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gq.hahajie.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hv.huixiangedu.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ft.muxihuayi.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://iy.shxzskj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://yo.yuntaijiaju.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://so.haigaiapp.cn

================================================================================
来源：http://da.colortex.cn

M. 命令行 / 进程 / 环境
来源：http://ls.szxytkj.cn

================================================================================
来源：http://gx.asd995.cn

[M01] 读取命令行参数
来源：http://cp.lnxyls.cn

Py:   sys.argv[1:]
来源：http://ur.shxzukj.cn

PHP:  $argv;  $argc;
来源：http://ed.yuntaijiaju.cn

JS:   process.argv.slice(2)
来源：http://uk.colortex.cn

TS:   process.argv.slice(2)
来源：http://ta.colortex.cn

Java: args 数组（main 方法参数）
来源：http://dt.yuntaijiaju.cn

Go:   os.Args[1:]
来源：http://op.gzmigu.cn

Ruby: ARGV
来源：http://qq.hahajie.cn

C#:   args 数组（Main 方法参数）
来源：http://uv.asd995.cn

[M02] 读取环境变量
来源：http://uj.huixiangedu.cn

Py:   os.environ.get("HOME")
来源：http://se.9csxet.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zr.panjiajie.cn

JS:   process.env.HOME
来源：http://we.yuexingan06.cn

TS:   process.env.HOME
来源：http://cy.muxihuayi.cn

Java: System.getenv("HOME")
来源：http://mz.newstarts.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://st.huanxung.cn

Ruby: ENV["HOME"]
来源：http://no.newstarts.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://cr.panjiajie.cn

[M03] 执行外部命令
来源：http://ez.shxzskj.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://dn.szxytkj.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.9csxet.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://fd.chemitech.net.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://lw.wgjwhj.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ia.hnjuh.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://us.szsharing.cn

Ruby: system("ls -l");  `ls -l`
来源：http://zc.muxihuayi.cn

C#:   Process.Start("ls", "-l");
来源：http://xr.huanxung.cn

[M04] 获取当前工作目录
来源：http://sn.hnjuh.cn

Py:   os.getcwd()
来源：http://lz.jianghongdianzi.cn

PHP:  getcwd();
来源：http://ts.bookmarksfly.cn

JS:   process.cwd()
来源：http://ql.bookmarksfly.cn

TS:   process.cwd()
来源：http://us.hnjuh.cn

Java: Path.of("").toAbsolutePath()
来源：http://ic.9csxet.cn

Go:   os.Getwd()
来源：http://ns.521024.cn

Ruby: Dir.pwd
来源：http://ly.bookmarksfly.cn

C#:   Directory.GetCurrentDirectory()
来源：http://gn.521024.cn

[M05] 设置退出码
来源：http://ek.nszjky.cn

Py:   sys.exit(1)
来源：http://cy.huixiangedu.cn

PHP:  exit(1);
来源：http://cw.9csxet.cn

JS:   process.exit(1)
来源：http://bz.huixinmuqiang.cn

TS:   process.exit(1)
来源：http://ww.hahajie.cn

Java: System.exit(1)
来源：http://bq.asd995.cn

Go:   os.Exit(1)
来源：http://dz.szsharing.cn

Ruby: exit 1
来源：http://qq.panjiajie.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://fo.shtwfgs.cn

[M06] 向标准错误输出
来源：http://ub.hahajie.cn

Py:   print("err", file=sys.stderr)
来源：http://kw.muxihuayi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ib.shtwfgs.cn

JS:   console.error("err")
来源：http://cp.chemitech.net.cn

TS:   console.error("err")
来源：http://ad.muxihuayi.cn

Java: System.err.println("err")
来源：http://mz.bookmarksfly.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://zs.muxihuayi.cn

Ruby: warn "err"
来源：http://my.szxytkj.cn

C#:   Console.Error.WriteLine("err")
来源：http://fb.9csxet.cn

[M07] 判断是否为主入口
来源：http://lw.yuntaijiaju.cn

Py:   if __name__ == "__main__":
来源：http://wk.newstarts.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ik.bjjhwx.cn

JS:   require.main === module
来源：http://ev.jctech888.com.cn

TS:   require.main === module
来源：http://aa.shxzukj.cn

Java: public static void main(String[] args)
来源：http://dq.colortex.cn

Go:   func main()
来源：http://iv.shtwfgs.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://bl.bookmarksfly.cn

C#:   static void Main(string[] args)
来源：http://cb.szsharing.cn

[M08] 获取系统与运行时信息
来源：http://nh.yuexingan06.cn

Py:   platform.system();  platform.python_version()
来源：http://hw.shxzskj.cn

PHP:  PHP_OS;  phpversion();
来源：http://gt.colortex.cn

JS:   process.platform;  process.version
来源：http://ef.haigaiapp.cn

TS:   process.platform;  process.version
来源：http://pz.shxzskj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ut.lnxyls.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://dd.9csxet.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://zo.colortex.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://sz.asd995.cn

================================================================================
来源：http://sj.gzmigu.cn

N. 数据结构与算法
来源：http://ra.9csxet.cn

================================================================================
来源：http://rs.9csxet.cn

[N01] 二分查找（有序数组）
来源：http://kj.bjjhwx.cn

Py:   bisect.bisect_left(arr, x)
来源：http://qv.gzmigu.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://bb.asd995.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bg.9csxet.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bk.haigaiapp.cn

Java: Arrays.binarySearch(arr, x)
来源：http://yl.hnjuh.cn

Go:   sort.SearchInts(arr, x)
来源：http://sk.gzmigu.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://hx.panjiajie.cn

C#:   Array.BinarySearch(arr, x)
来源：http://zc.muxihuayi.cn

[N02] 排序（工程实践用内置实现）
来源：http://be.shtwfgs.cn

Py:   sorted(arr);  arr.sort()
来源：http://nh.521024.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://it.colortex.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://jr.panjiajie.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ec.hahajie.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ux.9csxet.cn

Go:   slices.Sort(arr)
来源：http://co.huanxung.cn

Ruby: arr.sort
来源：http://ka.lnxyls.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://uk.jianghongdianzi.cn

[N03] 快速排序（分治示例）
来源：http://cw.haigaiapp.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://kk.huanxung.cn

PHP:  // 递归实现，或用 usort
来源：http://az.nicolike.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fc.lnxyls.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qy.panjiajie.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://aa.newstarts.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wa.chemitech.net.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://dn.jctech888.com.cn

C#:   // 手写递归，或 Array.Sort
来源：http://cr.shxzskj.cn

[N04] 斐波那契数列
来源：http://vq.hnjuh.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://cv.chemitech.net.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ia.hahajie.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qw.shtwfgs.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ba.haigaiapp.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://jd.jctech888.com.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://yl.bookmarksfly.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://rv.9csxet.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mb.shtwfgs.cn

[N05] 最大公约数
来源：http://bi.szsharing.cn

Py:   math.gcd(a, b)
来源：http://pk.haigaiapp.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://nl.huixiangedu.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mq.colortex.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dl.shxzukj.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://uj.yuexingan06.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://yk.yuexingan06.cn

Ruby: a.gcd(b)
来源：http://ly.hahajie.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hb.huixinmuqiang.cn

[N06] 判断回文字符串
来源：http://ly.wgjwhj.cn

Py:   s == s[::-1]
来源：http://gr.muxihuayi.cn

PHP:  $s === strrev($s);
来源：http://qj.shxzukj.cn

JS:   s === [...s].reverse().join("")
来源：http://gi.muxihuayi.cn

TS:   s === [...s].reverse().join("")
来源：http://pv.szsharing.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://fb.wgjwhj.cn

Go:   // 双指针从两端比较
来源：http://xc.muxihuayi.cn

Ruby: s == s.reverse
来源：http://fg.nicolike.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://mk.hnjuh.cn

[N07] 两数之和（返回下标）
来源：http://nq.yuntaijiaju.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ac.szsharing.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://cq.szsharing.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://xz.huixiangedu.cn

TS:   // 手写 Map<string, number>
来源：http://an.521024.cn

Java: // 手写 HashMap
来源：http://lf.huixinmuqiang.cn

Go:   // 手写 map[int]int
来源：http://zv.newstarts.cn

Ruby: // 手写 Hash
来源：http://cp.wgjwhj.cn

C#:   // 手写 Dictionary<int, int>
来源：http://va.muxihuayi.cn

[N08] 生成全排列
来源：http://uk.wgjwhj.cn

Py:   itertools.permutations(arr)
来源：http://hx.hnjuh.cn

PHP:  // 手写递归交换
来源：http://gf.jctech888.com.cn

JS:   // 手写回溯递归
来源：http://kb.huixinmuqiang.cn

TS:   // 手写回溯递归
来源：http://rs.huanxung.cn

Java: // 手写回溯递归
来源：http://pt.bookmarksfly.cn

Go:   // 手写回溯递归
来源：http://dw.yuntaijiaju.cn

Ruby: arr.permutation.to_a
来源：http://uq.yuntaijiaju.cn

C#:   // 手写回溯递归
来源：http://rd.newstarts.cn

[N09] 栈与队列
来源：http://ly.shxzukj.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://do.gzmigu.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://se.szxytkj.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://cx.shxzskj.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://gy.bjjhwx.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://bf.shtwfgs.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mn.newstarts.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hm.asd995.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://lm.shxzukj.cn

[N10] 链表节点定义
来源：http://pm.gzmigu.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://kb.szxytkj.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ez.521024.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ae.bookmarksfly.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://zl.yuexingan06.cn

Java: class Node { int v; Node next; }
来源：http://qn.bookmarksfly.cn

Go:   type Node struct { V int; Next *Node }
来源：http://nh.shxzukj.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://rq.hahajie.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://jn.huixinmuqiang.cn

[N11] 二叉树中序遍历
来源：http://ps.yuexingan06.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://bp.chemitech.net.cn

PHP:  // 手写递归函数
来源：http://xb.bookmarksfly.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kh.shxzukj.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pw.shtwfgs.cn

Java: // 手写递归
来源：http://zn.jianghongdianzi.cn

Go:   // 手写递归
来源：http://ht.newstarts.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ru.jctech888.com.cn

C#:   // 手写递归
来源：http://he.huixiangedu.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://xd.hahajie.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://gp.lnxyls.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://tz.jianghongdianzi.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vi.huixiangedu.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://iw.newstarts.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://yw.shxzskj.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://pz.panjiajie.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://xl.hahajie.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://uf.huixinmuqiang.cn

================================================================================
来源：http://ci.shxzskj.cn

O. 并发与异步
来源：http://fn.asd995.cn

================================================================================
来源：http://gn.wgjwhj.cn

[O01] 启动一个线程
来源：http://rk.9csxet.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://kt.521024.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ai.szsharing.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://yl.521024.cn

TS:   // 同 JS
来源：http://vm.chemitech.net.cn

Java: new Thread(() -> f()).start()
来源：http://xy.huixinmuqiang.cn

Go:   go f()
来源：http://sa.yuntaijiaju.cn

Ruby: Thread.new { f }
来源：http://ly.521024.cn

C#:   Task.Run(() => F());
来源：http://jp.jianghongdianzi.cn

[O02] 使用线程池
来源：http://zl.bookmarksfly.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://um.shtwfgs.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://na.wgjwhj.cn

JS:   // worker_threads 线程池
来源：http://nz.shtwfgs.cn

TS:   // worker_threads 线程池
来源：http://ox.hahajie.cn

Java: Executors.newFixedThreadPool(4)
来源：http://fi.hnjuh.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ah.521024.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://dx.lnxyls.cn


<!-- 参考信息 -->