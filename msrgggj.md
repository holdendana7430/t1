代发 wailian999

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://vl.chemitech.net.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://pw.nicolike.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wq.nszjky.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://an.nicolike.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ll.9csxet.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://vf.shtwfgs.cn

[K08] 二进制序列化（非 JSON）
来源：http://fb.huixiangedu.cn

Py:   pickle.dumps(obj)
来源：http://ff.521024.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://nw.nszjky.cn

JS:   v8.serialize(obj)        // Node
来源：http://nr.haigaiapp.cn

TS:   v8.serialize(obj)        // Node
来源：http://bn.colortex.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://nt.shxzukj.cn

Go:   encoding/gob
来源：http://rm.nszjky.cn

Ruby: Marshal.dump(obj)
来源：http://zu.bookmarksfly.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://bg.yuntaijiaju.cn

================================================================================
来源：http://za.asd995.cn

L. 网络请求
来源：http://wv.9csxet.cn

================================================================================
来源：http://ym.haigaiapp.cn

[L01] 发送 GET 请求
来源：http://ek.shtwfgs.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://vq.bookmarksfly.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://me.szxytkj.cn

JS:   await fetch(url)
来源：http://fs.huixiangedu.cn

TS:   await fetch(url)
来源：http://mh.hnjuh.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ti.asd995.cn

Go:   resp, err := http.Get(url)
来源：http://eh.yuntaijiaju.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ou.shxzukj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://eh.asd995.cn

[L02] 发送 POST JSON
来源：http://al.huanxung.cn

Py:   requests.post(url, json={"a": 1})
来源：http://xn.hnjuh.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://pp.chemitech.net.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xu.gzmigu.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cm.szsharing.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://dl.panjiajie.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://xb.shtwfgs.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://co.521024.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://zp.huixiangedu.cn

[L03] 设置自定义请求头
来源：http://ik.muxihuayi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://dg.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ck.haigaiapp.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nk.newstarts.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hn.bookmarksfly.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ee.bjjhwx.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ow.szsharing.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hv.wgjwhj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://bw.muxihuayi.cn

[L04] 设置超时
来源：http://ts.yuntaijiaju.cn

Py:   requests.get(url, timeout=5)
来源：http://ib.szsharing.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://js.huixinmuqiang.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wx.muxihuayi.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gi.nicolike.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://pa.shtwfgs.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ba.szxytkj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://qg.9csxet.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://kp.haigaiapp.cn

[L05] 上传文件（multipart）
来源：http://ea.yuntaijiaju.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://jn.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://az.huixiangedu.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://lk.lnxyls.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://je.szxytkj.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mh.hahajie.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://qz.haigaiapp.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://qx.huixinmuqiang.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://zs.bjjhwx.cn

[L06] 解析响应为 JSON
来源：http://gf.jianghongdianzi.cn

Py:   resp.json()
来源：http://aq.shxzukj.cn

PHP:  json_decode($body, true);
来源：http://bb.shtwfgs.cn

JS:   await resp.json()
来源：http://cn.chemitech.net.cn

TS:   await resp.json()
来源：http://ou.bjjhwx.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://vr.yuexingan06.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://th.9csxet.cn

Ruby: JSON.parse(resp.body)
来源：http://wt.panjiajie.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://qz.shxzukj.cn

[L07] 处理 HTTP 状态码
来源：http://dg.huixinmuqiang.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://qo.panjiajie.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://nh.haigaiapp.cn

JS:   resp.ok;  resp.status
来源：http://ow.shxzskj.cn

TS:   resp.ok;  resp.status
来源：http://mt.hahajie.cn

Java: resp.statusCode()
来源：http://xf.bjjhwx.cn

Go:   resp.StatusCode
来源：http://yp.panjiajie.cn

Ruby: resp.code.to_i
来源：http://fs.szsharing.cn

C#:   (int)resp.StatusCode
来源：http://pj.nicolike.cn

[L08] 并发请求多个地址
来源：http://hd.gzmigu.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://sh.muxihuayi.cn

PHP:  curl_multi_init() 系列
来源：http://hb.hnjuh.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pk.hahajie.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wd.jctech888.com.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ak.szsharing.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qr.9csxet.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://qm.bjjhwx.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xv.asd995.cn

================================================================================
来源：http://sk.haigaiapp.cn

M. 命令行 / 进程 / 环境
来源：http://gx.9csxet.cn

================================================================================
来源：http://ow.szsharing.cn

[M01] 读取命令行参数
来源：http://ik.asd995.cn

Py:   sys.argv[1:]
来源：http://rx.szxytkj.cn

PHP:  $argv;  $argc;
来源：http://os.bookmarksfly.cn

JS:   process.argv.slice(2)
来源：http://ql.jianghongdianzi.cn

TS:   process.argv.slice(2)
来源：http://ty.9csxet.cn

Java: args 数组（main 方法参数）
来源：http://gf.nszjky.cn

Go:   os.Args[1:]
来源：http://go.wgjwhj.cn

Ruby: ARGV
来源：http://wu.jianghongdianzi.cn

C#:   args 数组（Main 方法参数）
来源：http://ll.yuexingan06.cn

[M02] 读取环境变量
来源：http://el.gzmigu.cn

Py:   os.environ.get("HOME")
来源：http://sr.chemitech.net.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://nr.9csxet.cn

JS:   process.env.HOME
来源：http://kt.jianghongdianzi.cn

TS:   process.env.HOME
来源：http://bb.jianghongdianzi.cn

Java: System.getenv("HOME")
来源：http://pp.muxihuayi.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://me.gzmigu.cn

Ruby: ENV["HOME"]
来源：http://zc.nicolike.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://tz.colortex.cn

[M03] 执行外部命令
来源：http://oz.yuexingan06.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://aj.huixinmuqiang.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://sj.szsharing.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://rd.shxzukj.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://tk.yuexingan06.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://rp.jianghongdianzi.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ux.521024.cn

Ruby: system("ls -l");  `ls -l`
来源：http://dd.jianghongdianzi.cn

C#:   Process.Start("ls", "-l");
来源：http://tg.hnjuh.cn

[M04] 获取当前工作目录
来源：http://no.nicolike.cn

Py:   os.getcwd()
来源：http://ni.muxihuayi.cn

PHP:  getcwd();
来源：http://mk.hnjuh.cn

JS:   process.cwd()
来源：http://dq.jianghongdianzi.cn

TS:   process.cwd()
来源：http://et.huixinmuqiang.cn

Java: Path.of("").toAbsolutePath()
来源：http://pt.asd995.cn

Go:   os.Getwd()
来源：http://yu.newstarts.cn

Ruby: Dir.pwd
来源：http://cy.shxzskj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://zk.huixinmuqiang.cn

[M05] 设置退出码
来源：http://tu.jctech888.com.cn

Py:   sys.exit(1)
来源：http://kt.yuexingan06.cn

PHP:  exit(1);
来源：http://nz.chemitech.net.cn

JS:   process.exit(1)
来源：http://up.521024.cn

TS:   process.exit(1)
来源：http://yq.newstarts.cn

Java: System.exit(1)
来源：http://tc.chemitech.net.cn

Go:   os.Exit(1)
来源：http://hu.9csxet.cn

Ruby: exit 1
来源：http://np.yuntaijiaju.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://in.yuntaijiaju.cn

[M06] 向标准错误输出
来源：http://wj.shxzskj.cn

Py:   print("err", file=sys.stderr)
来源：http://kf.hahajie.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://jr.asd995.cn

JS:   console.error("err")
来源：http://jm.colortex.cn

TS:   console.error("err")
来源：http://ew.yuntaijiaju.cn

Java: System.err.println("err")
来源：http://vp.huanxung.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ml.shxzukj.cn

Ruby: warn "err"
来源：http://us.yuexingan06.cn

C#:   Console.Error.WriteLine("err")
来源：http://pr.shtwfgs.cn

[M07] 判断是否为主入口
来源：http://we.szsharing.cn

Py:   if __name__ == "__main__":
来源：http://cy.huanxung.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://jp.wgjwhj.cn

JS:   require.main === module
来源：http://xx.nszjky.cn

TS:   require.main === module
来源：http://fp.yuexingan06.cn

Java: public static void main(String[] args)
来源：http://eb.yuntaijiaju.cn

Go:   func main()
来源：http://mv.colortex.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://vz.shtwfgs.cn

C#:   static void Main(string[] args)
来源：http://nf.yuexingan06.cn

[M08] 获取系统与运行时信息
来源：http://lp.muxihuayi.cn

Py:   platform.system();  platform.python_version()
来源：http://kx.huixiangedu.cn

PHP:  PHP_OS;  phpversion();
来源：http://il.bjjhwx.cn

JS:   process.platform;  process.version
来源：http://yf.panjiajie.cn

TS:   process.platform;  process.version
来源：http://vg.bookmarksfly.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://qc.jianghongdianzi.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://lw.hahajie.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://xh.szxytkj.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://sb.lnxyls.cn

================================================================================
来源：http://ow.hnjuh.cn

N. 数据结构与算法
来源：http://lk.hahajie.cn

================================================================================
来源：http://oz.hahajie.cn

[N01] 二分查找（有序数组）
来源：http://bz.szxytkj.cn

Py:   bisect.bisect_left(arr, x)
来源：http://or.nicolike.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ls.szxytkj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ox.yuntaijiaju.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pz.gzmigu.cn

Java: Arrays.binarySearch(arr, x)
来源：http://dw.jctech888.com.cn

Go:   sort.SearchInts(arr, x)
来源：http://yq.gzmigu.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://cq.9csxet.cn

C#:   Array.BinarySearch(arr, x)
来源：http://bn.yuntaijiaju.cn

[N02] 排序（工程实践用内置实现）
来源：http://sv.szsharing.cn

Py:   sorted(arr);  arr.sort()
来源：http://fh.huixinmuqiang.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://vj.asd995.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ur.panjiajie.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://gm.shxzskj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://li.jianghongdianzi.cn

Go:   slices.Sort(arr)
来源：http://ek.wgjwhj.cn

Ruby: arr.sort
来源：http://sa.colortex.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ta.asd995.cn

[N03] 快速排序（分治示例）
来源：http://yg.lnxyls.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://kv.muxihuayi.cn

PHP:  // 递归实现，或用 usort
来源：http://gk.nicolike.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yw.yuexingan06.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://za.nicolike.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ed.asd995.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://vf.huixiangedu.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wo.9csxet.cn

C#:   // 手写递归，或 Array.Sort
来源：http://kf.yuntaijiaju.cn

[N04] 斐波那契数列
来源：http://lh.jianghongdianzi.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://uy.bjjhwx.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ms.asd995.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ml.huixinmuqiang.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dj.shxzukj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://rf.panjiajie.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://en.shtwfgs.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://bz.colortex.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://xc.nszjky.cn

[N05] 最大公约数
来源：http://nw.9csxet.cn

Py:   math.gcd(a, b)
来源：http://px.jctech888.com.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://yd.9csxet.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bs.nszjky.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ei.asd995.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://bt.hahajie.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://kc.521024.cn

Ruby: a.gcd(b)
来源：http://rz.chemitech.net.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://id.yuntaijiaju.cn

[N06] 判断回文字符串
来源：http://et.bookmarksfly.cn

Py:   s == s[::-1]
来源：http://pb.jctech888.com.cn

PHP:  $s === strrev($s);
来源：http://wt.jctech888.com.cn

JS:   s === [...s].reverse().join("")
来源：http://ku.nicolike.cn

TS:   s === [...s].reverse().join("")
来源：http://wn.bookmarksfly.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://qy.jianghongdianzi.cn

Go:   // 双指针从两端比较
来源：http://bd.gzmigu.cn

Ruby: s == s.reverse
来源：http://fb.shxzskj.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://aq.jianghongdianzi.cn

[N07] 两数之和（返回下标）
来源：http://be.nicolike.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://xu.nszjky.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://dp.shxzukj.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ud.lnxyls.cn

TS:   // 手写 Map<string, number>
来源：http://mo.9csxet.cn

Java: // 手写 HashMap
来源：http://yv.hahajie.cn

Go:   // 手写 map[int]int
来源：http://bt.asd995.cn

Ruby: // 手写 Hash
来源：http://dl.panjiajie.cn

C#:   // 手写 Dictionary<int, int>
来源：http://mf.yuntaijiaju.cn

[N08] 生成全排列
来源：http://qb.hahajie.cn

Py:   itertools.permutations(arr)
来源：http://fs.szxytkj.cn

PHP:  // 手写递归交换
来源：http://io.newstarts.cn

JS:   // 手写回溯递归
来源：http://jx.9csxet.cn

TS:   // 手写回溯递归
来源：http://xl.asd995.cn

Java: // 手写回溯递归
来源：http://wa.panjiajie.cn

Go:   // 手写回溯递归
来源：http://jy.muxihuayi.cn

Ruby: arr.permutation.to_a
来源：http://zm.bjjhwx.cn

C#:   // 手写回溯递归
来源：http://wq.yuntaijiaju.cn

[N09] 栈与队列
来源：http://sf.wgjwhj.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ug.yuntaijiaju.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://sl.shxzskj.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://kr.panjiajie.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://xy.colortex.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ca.haigaiapp.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://iw.huanxung.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ez.lnxyls.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://yt.jianghongdianzi.cn

[N10] 链表节点定义
来源：http://ne.yuexingan06.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ft.newstarts.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://cr.gzmigu.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://fc.shxzskj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://xd.yuntaijiaju.cn

Java: class Node { int v; Node next; }
来源：http://qv.yuexingan06.cn

Go:   type Node struct { V int; Next *Node }
来源：http://xd.shtwfgs.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://pn.shtwfgs.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ch.gzmigu.cn

[N11] 二叉树中序遍历
来源：http://tq.9csxet.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://dt.jctech888.com.cn

PHP:  // 手写递归函数
来源：http://en.panjiajie.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dv.hnjuh.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://el.nicolike.cn

Java: // 手写递归
来源：http://ry.jianghongdianzi.cn

Go:   // 手写递归
来源：http://bt.bjjhwx.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wy.szsharing.cn

C#:   // 手写递归
来源：http://kq.nszjky.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ed.jianghongdianzi.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hl.huixiangedu.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://fr.szxytkj.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rb.szxytkj.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kg.yuexingan06.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mp.521024.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ct.9csxet.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://cs.colortex.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://er.bookmarksfly.cn

================================================================================
来源：http://pn.jianghongdianzi.cn

O. 并发与异步
来源：http://wo.gzmigu.cn

================================================================================
来源：http://no.shxzukj.cn

[O01] 启动一个线程
来源：http://rw.shxzukj.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://jt.newstarts.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ka.wgjwhj.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ba.yuexingan06.cn

TS:   // 同 JS
来源：http://dd.yuntaijiaju.cn

Java: new Thread(() -> f()).start()
来源：http://gb.nszjky.cn

Go:   go f()
来源：http://fg.521024.cn

Ruby: Thread.new { f }
来源：http://hy.colortex.cn

C#:   Task.Run(() => F());
来源：http://yd.panjiajie.cn

[O02] 使用线程池
来源：http://jb.yuexingan06.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ff.asd995.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://rz.hnjuh.cn

JS:   // worker_threads 线程池
来源：http://ou.hahajie.cn

TS:   // worker_threads 线程池
来源：http://rl.yuexingan06.cn

Java: Executors.newFixedThreadPool(4)
来源：http://mv.muxihuayi.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ud.yuntaijiaju.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mk.shxzskj.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://tk.asd995.cn

[O03] 加锁保护共享数据
来源：http://pq.hahajie.cn

Py:   with lock: shared += 1
来源：http://ih.hnjuh.cn

PHP:  // 用 flock() 做文件锁
来源：http://ky.huixiangedu.cn


<!-- 参考信息 -->