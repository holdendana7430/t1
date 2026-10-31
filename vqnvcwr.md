代发 wailian999

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://pv.lnxyls.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://gv.521024.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://bj.jctech888.com.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://nx.bjjhwx.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ng.hahajie.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://iq.chemitech.net.cn

[K08] 二进制序列化（非 JSON）
来源：http://so.huixinmuqiang.cn

Py:   pickle.dumps(obj)
来源：http://fy.bjjhwx.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://rz.hahajie.cn

JS:   v8.serialize(obj)        // Node
来源：http://dp.huixinmuqiang.cn

TS:   v8.serialize(obj)        // Node
来源：http://jh.gzmigu.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://kn.huixiangedu.cn

Go:   encoding/gob
来源：http://tf.asd995.cn

Ruby: Marshal.dump(obj)
来源：http://df.shxzskj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://no.nicolike.cn

================================================================================
来源：http://qu.gzmigu.cn

L. 网络请求
来源：http://mp.szxytkj.cn

================================================================================
来源：http://bu.gzmigu.cn

[L01] 发送 GET 请求
来源：http://od.shtwfgs.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://tj.chemitech.net.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://sf.huixinmuqiang.cn

JS:   await fetch(url)
来源：http://gi.chemitech.net.cn

TS:   await fetch(url)
来源：http://ng.wgjwhj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://kd.hnjuh.cn

Go:   resp, err := http.Get(url)
来源：http://sw.chemitech.net.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://dh.gzmigu.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://xh.jctech888.com.cn

[L02] 发送 POST JSON
来源：http://zx.hnjuh.cn

Py:   requests.post(url, json={"a": 1})
来源：http://cr.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://kv.huixinmuqiang.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ou.panjiajie.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fu.hnjuh.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://nv.yuexingan06.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://du.muxihuayi.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://fi.jianghongdianzi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://pz.yuexingan06.cn

[L03] 设置自定义请求头
来源：http://oh.yuntaijiaju.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ig.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://az.szsharing.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sw.newstarts.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cy.chemitech.net.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://rz.shtwfgs.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://kq.shtwfgs.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://sf.jianghongdianzi.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://gu.gzmigu.cn

[L04] 设置超时
来源：http://ee.nicolike.cn

Py:   requests.get(url, timeout=5)
来源：http://af.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mw.lnxyls.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pr.bookmarksfly.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qt.hahajie.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://xt.bookmarksfly.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://of.haigaiapp.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://fj.yuntaijiaju.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://yg.hnjuh.cn

[L05] 上传文件（multipart）
来源：http://kp.colortex.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://gs.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://jr.panjiajie.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ca.huixiangedu.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://tc.shxzskj.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://nw.szsharing.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mp.panjiajie.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://lv.newstarts.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://vv.hahajie.cn

[L06] 解析响应为 JSON
来源：http://nh.panjiajie.cn

Py:   resp.json()
来源：http://vd.bookmarksfly.cn

PHP:  json_decode($body, true);
来源：http://rf.yuexingan06.cn

JS:   await resp.json()
来源：http://oa.bjjhwx.cn

TS:   await resp.json()
来源：http://ed.jianghongdianzi.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://zw.lnxyls.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://kl.shxzskj.cn

Ruby: JSON.parse(resp.body)
来源：http://vr.yuntaijiaju.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://dn.shxzskj.cn

[L07] 处理 HTTP 状态码
来源：http://zp.nszjky.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://kv.colortex.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://yw.huixiangedu.cn

JS:   resp.ok;  resp.status
来源：http://iv.9csxet.cn

TS:   resp.ok;  resp.status
来源：http://yz.bookmarksfly.cn

Java: resp.statusCode()
来源：http://wh.bookmarksfly.cn

Go:   resp.StatusCode
来源：http://dk.wgjwhj.cn

Ruby: resp.code.to_i
来源：http://dg.asd995.cn

C#:   (int)resp.StatusCode
来源：http://hf.gzmigu.cn

[L08] 并发请求多个地址
来源：http://mn.hahajie.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wk.panjiajie.cn

PHP:  curl_multi_init() 系列
来源：http://fy.bookmarksfly.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nr.wgjwhj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://di.newstarts.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://cs.haigaiapp.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://tm.bjjhwx.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ek.hnjuh.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://zn.wgjwhj.cn

================================================================================
来源：http://fr.szxytkj.cn

M. 命令行 / 进程 / 环境
来源：http://wk.bjjhwx.cn

================================================================================
来源：http://lu.hahajie.cn

[M01] 读取命令行参数
来源：http://bw.szxytkj.cn

Py:   sys.argv[1:]
来源：http://uq.huanxung.cn

PHP:  $argv;  $argc;
来源：http://ms.yuntaijiaju.cn

JS:   process.argv.slice(2)
来源：http://wp.shxzukj.cn

TS:   process.argv.slice(2)
来源：http://ty.asd995.cn

Java: args 数组（main 方法参数）
来源：http://br.newstarts.cn

Go:   os.Args[1:]
来源：http://sc.shxzukj.cn

Ruby: ARGV
来源：http://rr.szxytkj.cn

C#:   args 数组（Main 方法参数）
来源：http://vo.bookmarksfly.cn

[M02] 读取环境变量
来源：http://ey.szsharing.cn

Py:   os.environ.get("HOME")
来源：http://xl.nicolike.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://el.wgjwhj.cn

JS:   process.env.HOME
来源：http://de.huixiangedu.cn

TS:   process.env.HOME
来源：http://vk.wgjwhj.cn

Java: System.getenv("HOME")
来源：http://jj.hnjuh.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ja.szsharing.cn

Ruby: ENV["HOME"]
来源：http://ak.panjiajie.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://jw.nicolike.cn

[M03] 执行外部命令
来源：http://re.asd995.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vu.newstarts.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://jz.hahajie.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://um.shtwfgs.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://jl.haigaiapp.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://uk.chemitech.net.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://bt.shxzukj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://at.chemitech.net.cn

C#:   Process.Start("ls", "-l");
来源：http://ug.hnjuh.cn

[M04] 获取当前工作目录
来源：http://io.nicolike.cn

Py:   os.getcwd()
来源：http://dd.hahajie.cn

PHP:  getcwd();
来源：http://ed.shtwfgs.cn

JS:   process.cwd()
来源：http://kj.nicolike.cn

TS:   process.cwd()
来源：http://ym.shxzukj.cn

Java: Path.of("").toAbsolutePath()
来源：http://br.shxzukj.cn

Go:   os.Getwd()
来源：http://fp.521024.cn

Ruby: Dir.pwd
来源：http://kc.huanxung.cn

C#:   Directory.GetCurrentDirectory()
来源：http://mr.521024.cn

[M05] 设置退出码
来源：http://gb.bjjhwx.cn

Py:   sys.exit(1)
来源：http://rs.bookmarksfly.cn

PHP:  exit(1);
来源：http://hz.521024.cn

JS:   process.exit(1)
来源：http://rf.haigaiapp.cn

TS:   process.exit(1)
来源：http://dj.panjiajie.cn

Java: System.exit(1)
来源：http://bn.yuexingan06.cn

Go:   os.Exit(1)
来源：http://pk.521024.cn

Ruby: exit 1
来源：http://tv.panjiajie.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://bt.nszjky.cn

[M06] 向标准错误输出
来源：http://cw.huixinmuqiang.cn

Py:   print("err", file=sys.stderr)
来源：http://gt.jianghongdianzi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://lr.chemitech.net.cn

JS:   console.error("err")
来源：http://cq.szxytkj.cn

TS:   console.error("err")
来源：http://wu.szxytkj.cn

Java: System.err.println("err")
来源：http://yu.lnxyls.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://cv.huixiangedu.cn

Ruby: warn "err"
来源：http://um.yuexingan06.cn

C#:   Console.Error.WriteLine("err")
来源：http://dh.szxytkj.cn

[M07] 判断是否为主入口
来源：http://oo.wgjwhj.cn

Py:   if __name__ == "__main__":
来源：http://ao.newstarts.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://bx.yuntaijiaju.cn

JS:   require.main === module
来源：http://bg.521024.cn

TS:   require.main === module
来源：http://lc.panjiajie.cn

Java: public static void main(String[] args)
来源：http://tp.shtwfgs.cn

Go:   func main()
来源：http://pp.gzmigu.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://oa.haigaiapp.cn

C#:   static void Main(string[] args)
来源：http://eu.szsharing.cn

[M08] 获取系统与运行时信息
来源：http://rh.haigaiapp.cn

Py:   platform.system();  platform.python_version()
来源：http://tz.jctech888.com.cn

PHP:  PHP_OS;  phpversion();
来源：http://ei.szsharing.cn

JS:   process.platform;  process.version
来源：http://ur.hahajie.cn

TS:   process.platform;  process.version
来源：http://hx.szsharing.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wu.panjiajie.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://od.shxzukj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://km.521024.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://hf.521024.cn

================================================================================
来源：http://my.hnjuh.cn

N. 数据结构与算法
来源：http://ge.colortex.cn

================================================================================
来源：http://ey.szsharing.cn

[N01] 二分查找（有序数组）
来源：http://xu.lnxyls.cn

Py:   bisect.bisect_left(arr, x)
来源：http://kt.nicolike.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://lw.hahajie.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jk.szsharing.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dx.huixinmuqiang.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ef.szxytkj.cn

Go:   sort.SearchInts(arr, x)
来源：http://cn.gzmigu.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ej.panjiajie.cn

C#:   Array.BinarySearch(arr, x)
来源：http://xt.gzmigu.cn

[N02] 排序（工程实践用内置实现）
来源：http://tk.shxzukj.cn

Py:   sorted(arr);  arr.sort()
来源：http://zq.nszjky.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://db.asd995.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ed.shtwfgs.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://un.9csxet.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://jc.hnjuh.cn

Go:   slices.Sort(arr)
来源：http://vu.9csxet.cn

Ruby: arr.sort
来源：http://of.9csxet.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://oz.bjjhwx.cn

[N03] 快速排序（分治示例）
来源：http://iv.huanxung.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://qa.huanxung.cn

PHP:  // 递归实现，或用 usort
来源：http://iw.521024.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dx.wgjwhj.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://en.huanxung.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://jj.wgjwhj.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://nf.muxihuayi.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://km.szxytkj.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ls.jianghongdianzi.cn

[N04] 斐波那契数列
来源：http://gd.shtwfgs.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://lr.bjjhwx.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ty.newstarts.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://uh.yuexingan06.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nf.jianghongdianzi.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ns.nicolike.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://lc.muxihuayi.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://qi.yuntaijiaju.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://rl.newstarts.cn

[N05] 最大公约数
来源：http://eg.521024.cn

Py:   math.gcd(a, b)
来源：http://ih.chemitech.net.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://kp.shxzukj.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://uf.shxzskj.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wg.lnxyls.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mt.yuexingan06.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ld.bookmarksfly.cn

Ruby: a.gcd(b)
来源：http://bm.szsharing.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://sz.shxzukj.cn

[N06] 判断回文字符串
来源：http://ku.yuntaijiaju.cn

Py:   s == s[::-1]
来源：http://ix.szsharing.cn

PHP:  $s === strrev($s);
来源：http://yc.asd995.cn

JS:   s === [...s].reverse().join("")
来源：http://zl.shxzskj.cn

TS:   s === [...s].reverse().join("")
来源：http://jx.muxihuayi.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ui.shxzskj.cn

Go:   // 双指针从两端比较
来源：http://np.szxytkj.cn

Ruby: s == s.reverse
来源：http://ie.nicolike.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://db.panjiajie.cn

[N07] 两数之和（返回下标）
来源：http://fj.9csxet.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://np.shxzskj.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ic.jctech888.com.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://bv.gzmigu.cn

TS:   // 手写 Map<string, number>
来源：http://yc.9csxet.cn

Java: // 手写 HashMap
来源：http://dv.yuntaijiaju.cn

Go:   // 手写 map[int]int
来源：http://je.huixiangedu.cn

Ruby: // 手写 Hash
来源：http://io.hnjuh.cn

C#:   // 手写 Dictionary<int, int>
来源：http://bf.shxzukj.cn

[N08] 生成全排列
来源：http://hu.lnxyls.cn

Py:   itertools.permutations(arr)
来源：http://zm.huixiangedu.cn

PHP:  // 手写递归交换
来源：http://oy.lnxyls.cn

JS:   // 手写回溯递归
来源：http://az.nicolike.cn

TS:   // 手写回溯递归
来源：http://hf.gzmigu.cn

Java: // 手写回溯递归
来源：http://gn.yuexingan06.cn

Go:   // 手写回溯递归
来源：http://we.haigaiapp.cn

Ruby: arr.permutation.to_a
来源：http://lt.asd995.cn

C#:   // 手写回溯递归
来源：http://py.wgjwhj.cn

[N09] 栈与队列
来源：http://yk.huixinmuqiang.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ff.haigaiapp.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://sw.shxzukj.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://za.haigaiapp.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://qx.bjjhwx.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://cj.newstarts.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://rl.jctech888.com.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://id.szsharing.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://nx.hnjuh.cn

[N10] 链表节点定义
来源：http://le.wgjwhj.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://jp.asd995.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ig.shxzskj.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://oe.panjiajie.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://yj.chemitech.net.cn

Java: class Node { int v; Node next; }
来源：http://qj.hahajie.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ld.521024.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://wz.yuntaijiaju.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://da.muxihuayi.cn

[N11] 二叉树中序遍历
来源：http://bc.panjiajie.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ay.asd995.cn

PHP:  // 手写递归函数
来源：http://rh.huanxung.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://uf.wgjwhj.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xe.shxzskj.cn

Java: // 手写递归
来源：http://mg.muxihuayi.cn

Go:   // 手写递归
来源：http://pj.colortex.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://vs.jianghongdianzi.cn

C#:   // 手写递归
来源：http://bt.szsharing.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://br.huixiangedu.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://cp.shxzukj.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://vc.panjiajie.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ux.muxihuayi.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rd.bjjhwx.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://fa.huanxung.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://lu.jctech888.com.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://lg.bookmarksfly.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://bu.shxzskj.cn

================================================================================
来源：http://hs.muxihuayi.cn

O. 并发与异步
来源：http://de.yuexingan06.cn

================================================================================
来源：http://lr.lnxyls.cn

[O01] 启动一个线程
来源：http://wy.panjiajie.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://fa.hahajie.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://sj.bookmarksfly.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://cf.colortex.cn

TS:   // 同 JS
来源：http://eq.hahajie.cn

Java: new Thread(() -> f()).start()
来源：http://re.colortex.cn

Go:   go f()
来源：http://lq.nicolike.cn

Ruby: Thread.new { f }
来源：http://ep.haigaiapp.cn

C#:   Task.Run(() => F());
来源：http://my.panjiajie.cn

[O02] 使用线程池
来源：http://bw.yuexingan06.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://kb.lnxyls.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://po.9csxet.cn

JS:   // worker_threads 线程池
来源：http://et.jianghongdianzi.cn

TS:   // worker_threads 线程池
来源：http://sk.9csxet.cn

Java: Executors.newFixedThreadPool(4)
来源：http://oo.gzmigu.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://di.haigaiapp.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://bx.shtwfgs.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ze.bjjhwx.cn

[O03] 加锁保护共享数据
来源：http://si.huixinmuqiang.cn

Py:   with lock: shared += 1
来源：http://vr.yuexingan06.cn

PHP:  // 用 flock() 做文件锁
来源：http://hm.colortex.cn


<!-- 参考信息 -->