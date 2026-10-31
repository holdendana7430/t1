代发 wailian999

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ki.asd995.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://eq.jianghongdianzi.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://kw.lnxyls.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://nb.shtwfgs.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://sb.jctech888.com.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://cz.bookmarksfly.cn

[K08] 二进制序列化（非 JSON）
来源：http://td.9csxet.cn

Py:   pickle.dumps(obj)
来源：http://tv.lnxyls.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ey.shxzskj.cn

JS:   v8.serialize(obj)        // Node
来源：http://ti.bjjhwx.cn

TS:   v8.serialize(obj)        // Node
来源：http://em.panjiajie.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mb.shxzskj.cn

Go:   encoding/gob
来源：http://ss.huixiangedu.cn

Ruby: Marshal.dump(obj)
来源：http://vw.szxytkj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://pj.asd995.cn

================================================================================
来源：http://ah.chemitech.net.cn

L. 网络请求
来源：http://rp.panjiajie.cn

================================================================================
来源：http://jh.shtwfgs.cn

[L01] 发送 GET 请求
来源：http://de.jctech888.com.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://aq.yuntaijiaju.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://cb.lnxyls.cn

JS:   await fetch(url)
来源：http://wq.yuexingan06.cn

TS:   await fetch(url)
来源：http://mf.shxzukj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://sv.chemitech.net.cn

Go:   resp, err := http.Get(url)
来源：http://mo.szsharing.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://se.yuntaijiaju.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://gj.bookmarksfly.cn

[L02] 发送 POST JSON
来源：http://ad.lnxyls.cn

Py:   requests.post(url, json={"a": 1})
来源：http://se.haigaiapp.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://jd.hahajie.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qu.nicolike.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bv.colortex.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://dn.yuexingan06.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://fo.jianghongdianzi.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://lf.shtwfgs.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://do.jctech888.com.cn

[L03] 设置自定义请求头
来源：http://im.hahajie.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://rj.521024.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://bz.jianghongdianzi.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qb.muxihuayi.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rt.shtwfgs.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://su.521024.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://uz.colortex.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ti.colortex.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jj.yuntaijiaju.cn

[L04] 设置超时
来源：http://nl.szsharing.cn

Py:   requests.get(url, timeout=5)
来源：http://lo.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ag.yuexingan06.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vo.panjiajie.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mj.nicolike.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wn.szxytkj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ss.jctech888.com.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://kv.hnjuh.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ep.yuntaijiaju.cn

[L05] 上传文件（multipart）
来源：http://jz.wgjwhj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://jq.hnjuh.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://uw.huixiangedu.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ul.hnjuh.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://dq.shxzskj.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://dw.colortex.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://cd.hahajie.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://uq.yuntaijiaju.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://yk.huanxung.cn

[L06] 解析响应为 JSON
来源：http://ig.lnxyls.cn

Py:   resp.json()
来源：http://vr.haigaiapp.cn

PHP:  json_decode($body, true);
来源：http://rh.colortex.cn

JS:   await resp.json()
来源：http://mr.gzmigu.cn

TS:   await resp.json()
来源：http://ju.521024.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://pd.nszjky.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://js.hnjuh.cn

Ruby: JSON.parse(resp.body)
来源：http://eo.9csxet.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ep.hnjuh.cn

[L07] 处理 HTTP 状态码
来源：http://wj.nszjky.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hy.wgjwhj.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qc.huixinmuqiang.cn

JS:   resp.ok;  resp.status
来源：http://wh.wgjwhj.cn

TS:   resp.ok;  resp.status
来源：http://if.huixinmuqiang.cn

Java: resp.statusCode()
来源：http://uc.hahajie.cn

Go:   resp.StatusCode
来源：http://ab.jianghongdianzi.cn

Ruby: resp.code.to_i
来源：http://fn.gzmigu.cn

C#:   (int)resp.StatusCode
来源：http://fz.haigaiapp.cn

[L08] 并发请求多个地址
来源：http://ul.nicolike.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ma.newstarts.cn

PHP:  curl_multi_init() 系列
来源：http://vm.muxihuayi.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dn.jctech888.com.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kr.huanxung.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://dh.yuntaijiaju.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ww.yuntaijiaju.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://jq.panjiajie.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wi.asd995.cn

================================================================================
来源：http://hy.asd995.cn

M. 命令行 / 进程 / 环境
来源：http://nh.huixiangedu.cn

================================================================================
来源：http://ey.haigaiapp.cn

[M01] 读取命令行参数
来源：http://pq.bjjhwx.cn

Py:   sys.argv[1:]
来源：http://qr.jianghongdianzi.cn

PHP:  $argv;  $argc;
来源：http://dt.wgjwhj.cn

JS:   process.argv.slice(2)
来源：http://je.yuexingan06.cn

TS:   process.argv.slice(2)
来源：http://bu.szxytkj.cn

Java: args 数组（main 方法参数）
来源：http://hi.gzmigu.cn

Go:   os.Args[1:]
来源：http://is.chemitech.net.cn

Ruby: ARGV
来源：http://il.nszjky.cn

C#:   args 数组（Main 方法参数）
来源：http://ua.shxzukj.cn

[M02] 读取环境变量
来源：http://yv.yuntaijiaju.cn

Py:   os.environ.get("HOME")
来源：http://el.wgjwhj.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://db.bjjhwx.cn

JS:   process.env.HOME
来源：http://xg.yuexingan06.cn

TS:   process.env.HOME
来源：http://jz.huixiangedu.cn

Java: System.getenv("HOME")
来源：http://vf.bjjhwx.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ld.huanxung.cn

Ruby: ENV["HOME"]
来源：http://yr.nicolike.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://lh.huanxung.cn

[M03] 执行外部命令
来源：http://jk.chemitech.net.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://fv.yuexingan06.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://fq.haigaiapp.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://su.shxzskj.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://di.szxytkj.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hh.shxzskj.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ce.yuexingan06.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ex.hnjuh.cn

C#:   Process.Start("ls", "-l");
来源：http://ww.szxytkj.cn

[M04] 获取当前工作目录
来源：http://tq.haigaiapp.cn

Py:   os.getcwd()
来源：http://vk.panjiajie.cn

PHP:  getcwd();
来源：http://jz.nszjky.cn

JS:   process.cwd()
来源：http://qb.newstarts.cn

TS:   process.cwd()
来源：http://kt.shxzskj.cn

Java: Path.of("").toAbsolutePath()
来源：http://fk.bjjhwx.cn

Go:   os.Getwd()
来源：http://zi.panjiajie.cn

Ruby: Dir.pwd
来源：http://vk.shxzskj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://zv.jianghongdianzi.cn

[M05] 设置退出码
来源：http://ge.huixiangedu.cn

Py:   sys.exit(1)
来源：http://aq.huanxung.cn

PHP:  exit(1);
来源：http://fx.newstarts.cn

JS:   process.exit(1)
来源：http://ne.huixiangedu.cn

TS:   process.exit(1)
来源：http://cf.yuexingan06.cn

Java: System.exit(1)
来源：http://mc.szsharing.cn

Go:   os.Exit(1)
来源：http://ko.panjiajie.cn

Ruby: exit 1
来源：http://ir.colortex.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://vi.shtwfgs.cn

[M06] 向标准错误输出
来源：http://kk.panjiajie.cn

Py:   print("err", file=sys.stderr)
来源：http://ie.jctech888.com.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://sw.shtwfgs.cn

JS:   console.error("err")
来源：http://kh.shxzukj.cn

TS:   console.error("err")
来源：http://pg.szxytkj.cn

Java: System.err.println("err")
来源：http://xf.nszjky.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://yb.hahajie.cn

Ruby: warn "err"
来源：http://gd.lnxyls.cn

C#:   Console.Error.WriteLine("err")
来源：http://gk.newstarts.cn

[M07] 判断是否为主入口
来源：http://hw.shtwfgs.cn

Py:   if __name__ == "__main__":
来源：http://pr.szxytkj.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://sv.huanxung.cn

JS:   require.main === module
来源：http://co.gzmigu.cn

TS:   require.main === module
来源：http://lg.yuexingan06.cn

Java: public static void main(String[] args)
来源：http://cx.shtwfgs.cn

Go:   func main()
来源：http://ux.wgjwhj.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mj.shxzskj.cn

C#:   static void Main(string[] args)
来源：http://qv.wgjwhj.cn

[M08] 获取系统与运行时信息
来源：http://ff.panjiajie.cn

Py:   platform.system();  platform.python_version()
来源：http://kh.szxytkj.cn

PHP:  PHP_OS;  phpversion();
来源：http://bo.shxzskj.cn

JS:   process.platform;  process.version
来源：http://be.shxzukj.cn

TS:   process.platform;  process.version
来源：http://ud.shtwfgs.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hw.jianghongdianzi.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://hn.colortex.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://yu.huanxung.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://az.lnxyls.cn

================================================================================
来源：http://yn.haigaiapp.cn

N. 数据结构与算法
来源：http://nh.muxihuayi.cn

================================================================================
来源：http://ef.muxihuayi.cn

[N01] 二分查找（有序数组）
来源：http://xz.nicolike.cn

Py:   bisect.bisect_left(arr, x)
来源：http://eq.szxytkj.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://cy.huixinmuqiang.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://of.jianghongdianzi.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ss.hnjuh.cn

Java: Arrays.binarySearch(arr, x)
来源：http://qf.shxzskj.cn

Go:   sort.SearchInts(arr, x)
来源：http://wn.huanxung.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://od.nszjky.cn

C#:   Array.BinarySearch(arr, x)
来源：http://vz.bookmarksfly.cn

[N02] 排序（工程实践用内置实现）
来源：http://sq.shxzukj.cn

Py:   sorted(arr);  arr.sort()
来源：http://di.bookmarksfly.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wq.jctech888.com.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://xi.nicolike.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://pe.jctech888.com.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wp.shxzukj.cn

Go:   slices.Sort(arr)
来源：http://dy.bookmarksfly.cn

Ruby: arr.sort
来源：http://os.521024.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ak.newstarts.cn

[N03] 快速排序（分治示例）
来源：http://yb.szsharing.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ui.shtwfgs.cn

PHP:  // 递归实现，或用 usort
来源：http://ra.nszjky.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://at.haigaiapp.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bn.lnxyls.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://rs.asd995.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mj.shxzukj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://rs.newstarts.cn

C#:   // 手写递归，或 Array.Sort
来源：http://hw.9csxet.cn

[N04] 斐波那契数列
来源：http://to.haigaiapp.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zo.9csxet.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://kn.jianghongdianzi.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://up.yuntaijiaju.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pe.bjjhwx.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://xs.lnxyls.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ft.hahajie.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://fy.wgjwhj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://na.wgjwhj.cn

[N05] 最大公约数
来源：http://xw.panjiajie.cn

Py:   math.gcd(a, b)
来源：http://xa.9csxet.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://sa.jianghongdianzi.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qu.szxytkj.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://df.colortex.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://pj.yuntaijiaju.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://pd.huixiangedu.cn

Ruby: a.gcd(b)
来源：http://ci.huanxung.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://un.muxihuayi.cn

[N06] 判断回文字符串
来源：http://tz.muxihuayi.cn

Py:   s == s[::-1]
来源：http://bt.huanxung.cn

PHP:  $s === strrev($s);
来源：http://fs.hnjuh.cn

JS:   s === [...s].reverse().join("")
来源：http://ud.huixiangedu.cn

TS:   s === [...s].reverse().join("")
来源：http://xe.colortex.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xd.asd995.cn

Go:   // 双指针从两端比较
来源：http://eg.wgjwhj.cn

Ruby: s == s.reverse
来源：http://ml.haigaiapp.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://zf.huanxung.cn

[N07] 两数之和（返回下标）
来源：http://kn.bookmarksfly.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ia.szxytkj.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mc.gzmigu.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://hd.wgjwhj.cn

TS:   // 手写 Map<string, number>
来源：http://lt.nicolike.cn

Java: // 手写 HashMap
来源：http://ma.yuntaijiaju.cn

Go:   // 手写 map[int]int
来源：http://cv.hahajie.cn

Ruby: // 手写 Hash
来源：http://sg.hnjuh.cn

C#:   // 手写 Dictionary<int, int>
来源：http://kd.yuexingan06.cn

[N08] 生成全排列
来源：http://zg.9csxet.cn

Py:   itertools.permutations(arr)
来源：http://pu.colortex.cn

PHP:  // 手写递归交换
来源：http://mz.huixinmuqiang.cn

JS:   // 手写回溯递归
来源：http://ck.nicolike.cn

TS:   // 手写回溯递归
来源：http://dk.nszjky.cn

Java: // 手写回溯递归
来源：http://xw.jctech888.com.cn

Go:   // 手写回溯递归
来源：http://yd.bookmarksfly.cn

Ruby: arr.permutation.to_a
来源：http://fv.huixinmuqiang.cn

C#:   // 手写回溯递归
来源：http://fl.bookmarksfly.cn

[N09] 栈与队列
来源：http://ay.newstarts.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ig.huixinmuqiang.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://pn.hnjuh.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://yu.muxihuayi.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://rz.jianghongdianzi.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://fn.521024.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://fo.muxihuayi.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ry.szsharing.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://aq.yuntaijiaju.cn

[N10] 链表节点定义
来源：http://ny.haigaiapp.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://yb.colortex.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://om.nicolike.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://og.panjiajie.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://lp.szxytkj.cn

Java: class Node { int v; Node next; }
来源：http://nv.muxihuayi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://na.newstarts.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://fw.jianghongdianzi.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ow.gzmigu.cn

[N11] 二叉树中序遍历
来源：http://em.huanxung.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://aa.asd995.cn

PHP:  // 手写递归函数
来源：http://fz.panjiajie.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ki.521024.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bm.hnjuh.cn

Java: // 手写递归
来源：http://re.hahajie.cn

Go:   // 手写递归
来源：http://tg.haigaiapp.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://uu.newstarts.cn

C#:   // 手写递归
来源：http://nt.huixinmuqiang.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ch.yuexingan06.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://rl.panjiajie.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://em.haigaiapp.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ne.nicolike.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://iu.newstarts.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://fs.hahajie.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://yq.huixiangedu.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://pn.jianghongdianzi.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://as.bookmarksfly.cn

================================================================================
来源：http://jp.hahajie.cn

O. 并发与异步
来源：http://km.colortex.cn

================================================================================
来源：http://dp.nszjky.cn

[O01] 启动一个线程
来源：http://qd.szsharing.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ch.lnxyls.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://rr.bjjhwx.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://pn.gzmigu.cn

TS:   // 同 JS
来源：http://kr.yuntaijiaju.cn

Java: new Thread(() -> f()).start()
来源：http://nd.huanxung.cn

Go:   go f()
来源：http://mi.jianghongdianzi.cn

Ruby: Thread.new { f }
来源：http://ed.huixinmuqiang.cn

C#:   Task.Run(() => F());
来源：http://op.wgjwhj.cn

[O02] 使用线程池
来源：http://qy.nszjky.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://sr.haigaiapp.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://sj.shtwfgs.cn

JS:   // worker_threads 线程池
来源：http://bm.jctech888.com.cn

TS:   // worker_threads 线程池
来源：http://pf.haigaiapp.cn

Java: Executors.newFixedThreadPool(4)
来源：http://zd.huixiangedu.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://rb.haigaiapp.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://po.jctech888.com.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://sr.9csxet.cn

[O03] 加锁保护共享数据
来源：http://vb.wgjwhj.cn

Py:   with lock: shared += 1
来源：http://me.shxzukj.cn

PHP:  // 用 flock() 做文件锁
来源：http://ha.jctech888.com.cn


<!-- 参考信息 -->